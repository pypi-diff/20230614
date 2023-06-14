# Comparing `tmp/web3cli-1.1.3.tar.gz` & `tmp/web3cli-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3cli-1.1.3.tar", last modified: Mon Jun 12 19:20:41 2023, max compression
+gzip compressed data, was "web3cli-1.1.4.tar", last modified: Wed Jun 14 06:20:01 2023, max compression
```

## Comparing `web3cli-1.1.3.tar` & `web3cli-1.1.4.tar`

### file list

```diff
@@ -1,176 +1,176 @@
--rw-r--r--   0        0        0     1069 2022-10-24 15:49:55.999119 web3cli-1.1.3/LICENSE
--rw-r--r--   0        0        0    12030 2023-06-10 16:07:05.654200 web3cli-1.1.3/README.md
--rw-r--r--   0        0        0     4026 2023-06-12 19:20:14.245354 web3cli-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-11-13 07:56:22.807127 web3cli-1.1.3/src/web3cli/.DS_Store
--rw-r--r--   0        0        0        0 2022-11-18 22:32:14.016225 web3cli-1.1.3/src/web3cli/__init__.py
--rw-r--r--   0        0        0        0 2022-10-24 15:34:40.198985 web3cli-1.1.3/src/web3cli/controllers/__init__.py
--rw-r--r--   0        0        0     4679 2023-06-10 16:49:18.164306 web3cli-1.1.3/src/web3cli/controllers/abi_controller.py
--rw-r--r--   0        0        0     2049 2023-06-10 16:26:02.765052 web3cli-1.1.3/src/web3cli/controllers/app_key_controller.py
--rw-r--r--   0        0        0     1215 2023-06-10 16:26:21.840704 web3cli-1.1.3/src/web3cli/controllers/base_controller.py
--rw-r--r--   0        0        0     3106 2023-06-10 17:02:35.846994 web3cli-1.1.3/src/web3cli/controllers/call_controller.py
--rw-r--r--   0        0        0     2421 2023-06-10 16:26:42.723101 web3cli-1.1.3/src/web3cli/controllers/config_controller.py
--rw-r--r--   0        0        0     1109 2022-12-17 18:21:46.704206 web3cli-1.1.3/src/web3cli/controllers/controller.py
--rw-r--r--   0        0        0        0 2023-03-25 21:06:13.922427 web3cli-1.1.3/src/web3cli/controllers/crud/__init__.py
--rw-r--r--   0        0        0     2530 2023-06-10 16:49:44.923130 web3cli-1.1.3/src/web3cli/controllers/crud/address_controller.py
--rw-r--r--   0        0        0     4413 2023-06-10 16:50:02.537767 web3cli-1.1.3/src/web3cli/controllers/crud/chain_controller.py
--rw-r--r--   0        0        0     4785 2023-06-10 16:50:16.263301 web3cli-1.1.3/src/web3cli/controllers/crud/contract_controller.py
--rw-r--r--   0        0        0     3035 2023-06-10 16:21:12.060981 web3cli-1.1.3/src/web3cli/controllers/crud/history_controller.py
--rw-r--r--   0        0        0     2972 2023-06-10 16:35:01.955138 web3cli-1.1.3/src/web3cli/controllers/crud/rpc_controller.py
--rw-r--r--   0        0        0     5282 2023-06-10 16:51:30.999842 web3cli-1.1.3/src/web3cli/controllers/crud/signer_controller.py
--rw-r--r--   0        0        0     1390 2023-06-10 16:27:14.395424 web3cli-1.1.3/src/web3cli/controllers/db_controller.py
--rw-r--r--   0        0        0      817 2023-06-12 19:19:49.774803 web3cli-1.1.3/src/web3cli/controllers/debug_controller.py
--rw-r--r--   0        0        0     1479 2023-06-10 16:29:57.178158 web3cli-1.1.3/src/web3cli/controllers/keyfile_controller.py
--rw-r--r--   0        0        0     4153 2023-06-10 18:07:14.344855 web3cli-1.1.3/src/web3cli/controllers/misc_controller.py
--rw-r--r--   0        0        0     4471 2023-06-10 16:33:44.421618 web3cli-1.1.3/src/web3cli/controllers/replay_controller.py
--rw-r--r--   0        0        0     2403 2023-06-10 16:33:58.579948 web3cli-1.1.3/src/web3cli/controllers/send_controller.py
--rw-r--r--   0        0        0     4535 2023-06-12 19:19:49.775186 web3cli-1.1.3/src/web3cli/controllers/subscribe_controller.py
--rw-r--r--   0        0        0     6878 2023-05-20 18:17:47.046015 web3cli-1.1.3/src/web3cli/controllers/swap_controller.py
--rw-r--r--   0        0        0     7848 2023-06-10 17:57:16.099321 web3cli-1.1.3/src/web3cli/controllers/token_controller.py
--rw-r--r--   0        0        0     2862 2023-05-20 18:17:47.047364 web3cli-1.1.3/src/web3cli/controllers/transact_controller.py
--rw-r--r--   0        0        0     1239 2023-06-10 17:31:55.330976 web3cli-1.1.3/src/web3cli/controllers/tx_controller.py
--rw-r--r--   0        0        0      341 2023-05-20 18:17:47.049010 web3cli-1.1.3/src/web3cli/exceptions.py
--rw-r--r--   0        0        0     1329 2023-06-12 10:20:17.461216 web3cli-1.1.3/src/web3cli/framework/ext_print.py
--rw-r--r--   0        0        0        0 2022-10-24 15:34:40.191413 web3cli-1.1.3/src/web3cli/helpers/__init__.py
--rw-r--r--   0        0        0    17459 2023-06-12 19:19:49.775633 web3cli-1.1.3/src/web3cli/helpers/args.py
--rw-r--r--   0        0        0     2198 2023-05-20 18:17:47.051274 web3cli-1.1.3/src/web3cli/helpers/client_factory.py
--rw-r--r--   0        0        0     1252 2022-12-28 16:44:58.644508 web3cli-1.1.3/src/web3cli/helpers/config.py
--rw-r--r--   0        0        0     2092 2023-05-18 11:14:15.678582 web3cli-1.1.3/src/web3cli/helpers/crypto.py
--rw-r--r--   0        0        0     1228 2023-02-11 17:24:24.959766 web3cli-1.1.3/src/web3cli/helpers/database.py
--rw-r--r--   0        0        0     1776 2023-06-10 18:08:11.403330 web3cli-1.1.3/src/web3cli/helpers/render.py
--rw-r--r--   0        0        0     4548 2023-06-07 12:09:20.814550 web3cli-1.1.3/src/web3cli/helpers/send.py
--rw-r--r--   0        0        0     2178 2023-05-20 18:17:47.053233 web3cli-1.1.3/src/web3cli/helpers/signer.py
--rw-r--r--   0        0        0     1429 2023-06-12 19:19:49.775947 web3cli-1.1.3/src/web3cli/helpers/telegram.py
--rw-r--r--   0        0        0     2132 2023-06-07 12:22:03.729729 web3cli-1.1.3/src/web3cli/helpers/tx.py
--rw-r--r--   0        0        0      435 2023-06-12 19:20:28.966931 web3cli-1.1.3/src/web3cli/helpers/version.py
--rw-r--r--   0        0        0     2595 2023-02-12 21:33:06.910919 web3cli-1.1.3/src/web3cli/hooks.py
--rw-r--r--   0        0        0     7780 2023-06-12 19:19:49.776256 web3cli-1.1.3/src/web3cli/main.py
--rw-r--r--   0        0        0        0 2023-01-29 11:30:42.897043 web3cli-1.1.3/src/web3cli/templates/__init__.py
--rw-r--r--   0        0        0      243 2023-01-29 11:41:03.173746 web3cli-1.1.3/src/web3cli/templates/balance.jinja2
--rw-r--r--   0        0        0      120 2022-11-03 17:39:28.958124 web3cli-1.1.3/src/web3core/__init__.py
--rw-r--r--   0        0        0       72 2023-02-19 11:02:13.393953 web3cli-1.1.3/src/web3core/constants.py
--rw-r--r--   0        0        0       90 2023-01-18 19:29:57.558367 web3cli-1.1.3/src/web3core/db.py
--rw-r--r--   0        0        0     1762 2023-01-18 20:41:45.295870 web3cli-1.1.3/src/web3core/exceptions.py
--rw-r--r--   0        0        0        0 2022-11-03 17:39:28.958845 web3cli-1.1.3/src/web3core/helpers/__init__.py
--rw-r--r--   0        0        0     9448 2023-04-07 18:14:01.618698 web3cli-1.1.3/src/web3core/helpers/abi.py
--rw-r--r--   0        0        0     1148 2023-05-17 09:47:21.910041 web3cli-1.1.3/src/web3core/helpers/blocks.py
--rw-r--r--   0        0        0     3405 2023-05-20 18:17:47.055119 web3cli-1.1.3/src/web3core/helpers/client_factory.py
--rw-r--r--   0        0        0     1060 2022-12-17 18:21:46.707584 web3cli-1.1.3/src/web3core/helpers/crypto.py
--rw-r--r--   0        0        0      714 2023-02-11 17:32:11.986925 web3cli-1.1.3/src/web3core/helpers/database.py
--rw-r--r--   0        0        0     1582 2023-04-07 18:14:01.619156 web3cli-1.1.3/src/web3core/helpers/dex.py
--rw-r--r--   0        0        0      434 2022-12-19 20:01:36.985004 web3cli-1.1.3/src/web3core/helpers/format.py
--rw-r--r--   0        0        0     2413 2023-05-18 08:42:25.689036 web3cli-1.1.3/src/web3core/helpers/misc.py
--rw-r--r--   0        0        0      532 2022-12-16 06:48:29.391730 web3cli-1.1.3/src/web3core/helpers/os.py
--rw-r--r--   0        0        0     1799 2023-06-10 15:39:08.908650 web3cli-1.1.3/src/web3core/helpers/resolve.py
--rw-r--r--   0        0        0      827 2023-06-10 09:19:32.610030 web3cli-1.1.3/src/web3core/helpers/rpc.py
--rw-r--r--   0        0        0     2158 2023-01-14 21:27:16.459461 web3cli-1.1.3/src/web3core/helpers/seed.py
--rw-r--r--   0        0        0      697 2023-06-12 19:19:49.776495 web3cli-1.1.3/src/web3core/helpers/telegram.py
--rw-r--r--   0        0        0     4697 2023-04-07 18:14:01.620145 web3cli-1.1.3/src/web3core/helpers/tx.py
--rw-r--r--   0        0        0      553 2023-06-12 19:19:49.776790 web3cli-1.1.3/src/web3core/helpers/validation.py
--rw-r--r--   0        0        0     1207 2022-12-28 16:44:58.644659 web3cli-1.1.3/src/web3core/helpers/yaml.py
--rw-r--r--   0        0        0      424 2023-01-18 19:29:57.562778 web3cli-1.1.3/src/web3core/models/__init__.py
--rw-r--r--   0        0        0     1790 2023-01-18 19:29:57.563744 web3cli-1.1.3/src/web3core/models/address.py
--rw-r--r--   0        0        0     3433 2023-05-20 18:17:47.055757 web3cli-1.1.3/src/web3core/models/base_model.py
--rw-r--r--   0        0        0     4923 2023-03-25 21:22:51.453293 web3cli-1.1.3/src/web3core/models/chain.py
--rw-r--r--   0        0        0     4262 2023-05-31 08:53:51.850966 web3cli-1.1.3/src/web3core/models/contract.py
--rw-r--r--   0        0        0     1405 2023-05-18 09:25:11.305140 web3cli-1.1.3/src/web3core/models/signer.py
--rw-r--r--   0        0        0     1054 2022-12-28 16:44:59.161817 web3cli-1.1.3/src/web3core/models/timestamps_model.py
--rw-r--r--   0        0        0     2550 2022-12-28 16:44:59.162568 web3cli-1.1.3/src/web3core/models/tx.py
--rw-r--r--   0        0        0     1449 2023-01-18 19:29:57.566552 web3cli-1.1.3/src/web3core/models/types.py
--rw-r--r--   0        0        0       48 2022-11-18 22:43:37.360850 web3cli-1.1.3/src/web3core/seeds/__init__.py
--rw-r--r--   0        0        0     3164 2023-06-08 14:39:52.689918 web3cli-1.1.3/src/web3core/seeds/chain_seeds.py
--rw-r--r--   0        0        0      521 2023-06-08 14:37:27.133219 web3cli-1.1.3/src/web3core/seeds/contract_seeds.py
--rw-r--r--   0        0        0    49489 2023-02-19 09:09:21.024661 web3cli-1.1.3/src/web3core/seeds/contract_type_seeds.py
--rw-r--r--   0        0        0     9720 2023-02-27 16:48:07.675984 web3cli-1.1.3/src/web3core/seeds/contracts/arb_contract_seeds.py
--rw-r--r--   0        0        0     1881 2023-02-27 19:24:54.136969 web3cli-1.1.3/src/web3core/seeds/contracts/avax_contract_seeds.py
--rw-r--r--   0        0        0      867 2023-06-10 15:43:36.615089 web3cli-1.1.3/src/web3core/seeds/contracts/bnb_contract_seeds.py
--rw-r--r--   0        0        0      611 2023-05-25 15:43:35.647237 web3cli-1.1.3/src/web3core/seeds/contracts/era_contract_seeds.py
--rw-r--r--   0        0        0      997 2023-06-08 14:37:20.947238 web3cli-1.1.3/src/web3core/seeds/contracts/erat_contract_seeds.py
--rw-r--r--   0        0        0     1579 2023-02-27 16:48:24.467166 web3cli-1.1.3/src/web3core/seeds/contracts/eth_contract_seeds.py
--rw-r--r--   0        0        0     1183 2023-05-26 15:20:05.535496 web3cli-1.1.3/src/web3core/seeds/contracts/gno_contract_seeds.py
--rw-r--r--   0        0        0     1448 2023-02-19 10:37:03.165028 web3cli-1.1.3/src/web3core/types.py
--rw-r--r--   0        0        0     6148 2023-02-28 16:18:46.901853 web3cli-1.1.3/tests/.DS_Store
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.296564 web3cli-1.1.3/tests/__init__.py
--rw-r--r--   0        0        0    10244 2023-02-28 16:18:44.627516 web3cli-1.1.3/tests/ape/.DS_Store
--rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.934034 web3cli-1.1.3/tests/ape/.build/Factory_IERC20.json
--rw-r--r--   0        0        0      536 2023-04-06 17:43:03.934442 web3cli-1.1.3/tests/ape/.build/Factory_IUniswapV2Callee.json
--rw-r--r--   0        0        0     3605 2023-04-06 17:43:03.935802 web3cli-1.1.3/tests/ape/.build/Factory_IUniswapV2ERC20.json
--rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.936651 web3cli-1.1.3/tests/ape/.build/Factory_IUniswapV2Factory.json
--rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.938968 web3cli-1.1.3/tests/ape/.build/Factory_IUniswapV2Pair.json
--rw-r--r--   0        0        0      862 2023-04-06 17:43:03.939241 web3cli-1.1.3/tests/ape/.build/Factory_Math.json
--rw-r--r--   0        0        0      866 2023-04-06 17:43:03.939527 web3cli-1.1.3/tests/ape/.build/Factory_SafeMath.json
--rw-r--r--   0        0        0      867 2023-04-06 17:43:03.939780 web3cli-1.1.3/tests/ape/.build/Factory_UQ112x112.json
--rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.916870 web3cli-1.1.3/tests/ape/.build/Router_IERC20.json
--rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.917744 web3cli-1.1.3/tests/ape/.build/Router_IUniswapV2Factory.json
--rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.920204 web3cli-1.1.3/tests/ape/.build/Router_IUniswapV2Pair.json
--rw-r--r--   0        0        0     9213 2023-04-06 17:43:03.922797 web3cli-1.1.3/tests/ape/.build/Router_IUniswapV2Router01.json
--rw-r--r--   0        0        0    11845 2023-04-06 17:43:03.926066 web3cli-1.1.3/tests/ape/.build/Router_IUniswapV2Router02.json
--rw-r--r--   0        0        0      683 2023-04-06 17:43:03.926558 web3cli-1.1.3/tests/ape/.build/Router_IWETH.json
--rw-r--r--   0        0        0      872 2023-04-06 17:43:03.926867 web3cli-1.1.3/tests/ape/.build/Router_SafeMath.json
--rw-r--r--   0        0        0      879 2023-04-06 17:43:03.927162 web3cli-1.1.3/tests/ape/.build/Router_TransferHelper.json
--rw-r--r--   0        0        0      881 2023-04-06 17:43:03.927462 web3cli-1.1.3/tests/ape/.build/Router_UniswapV2Library.json
--rw-r--r--   0        0        0    14895 2023-04-06 17:43:03.932635 web3cli-1.1.3/tests/ape/.build/Token.json
--rw-r--r--   0        0        0      791 2023-04-06 17:43:03.932974 web3cli-1.1.3/tests/ape/.build/Token_SafeMath.json
--rw-r--r--   0        0        0    14014 2023-04-06 17:43:03.941015 web3cli-1.1.3/tests/ape/.build/UniswapV2ERC20.json
--rw-r--r--   0        0        0    46097 2023-04-06 17:43:03.942289 web3cli-1.1.3/tests/ape/.build/UniswapV2Factory.json
--rw-r--r--   0        0        0    44784 2023-04-06 17:43:03.944616 web3cli-1.1.3/tests/ape/.build/UniswapV2Pair.json
--rw-r--r--   0        0        0    85730 2023-04-06 17:43:03.931232 web3cli-1.1.3/tests/ape/.build/UniswapV2Router02.json
--rw-r--r--   0        0        0   324962 2023-06-12 19:20:33.172792 web3cli-1.1.3/tests/ape/.build/__local__.json
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.620721 web3cli-1.1.3/tests/ape/__init__.py
--rw-r--r--   0        0        0     6148 2023-02-28 16:18:44.554061 web3cli-1.1.3/tests/ape/contracts/.DS_Store
--rw-r--r--   0        0        0     4101 2023-04-07 18:14:01.621230 web3cli-1.1.3/tests/ape/contracts/token/Token.sol
--rw-r--r--   0        0        0      646 2023-04-07 18:14:01.621775 web3cli-1.1.3/tests/ape/contracts/token/Token_SafeMath.sol
--rw-r--r--   0        0        0     6148 2023-02-28 15:31:57.501753 web3cli-1.1.3/tests/ape/contracts/uniswap/.DS_Store
--rw-r--r--   0        0        0    21725 2023-04-07 18:14:01.622322 web3cli-1.1.3/tests/ape/contracts/uniswap/UniswapV2Factory.sol
--rw-r--r--   0        0        0    34078 2023-04-07 18:14:01.622848 web3cli-1.1.3/tests/ape/contracts/uniswap/UniswapV2Router02.sol
--rw-r--r--   0        0        0      236 2023-04-07 18:14:01.623357 web3cli-1.1.3/tests/ape/scripts/__init__.py
--rw-r--r--   0        0        0      347 2023-04-07 18:14:01.623719 web3cli-1.1.3/tests/ape/scripts/db.py
--rw-r--r--   0        0        0      200 2023-04-07 18:14:01.624050 web3cli-1.1.3/tests/ape/scripts/token.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624201 web3cli-1.1.3/tests/ape/tests/__init__.py
--rw-r--r--   0        0        0    13902 2023-04-07 18:14:01.624793 web3cli-1.1.3/tests/ape/tests/fixtures.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624997 web3cli-1.1.3/tests/ape/tests/helpers/__init__.py
--rw-r--r--   0        0        0      371 2023-04-07 18:14:01.625481 web3cli-1.1.3/tests/ape/tests/helpers/ape.py
--rw-r--r--   0        0        0      881 2023-04-07 18:14:01.625860 web3cli-1.1.3/tests/ape/tests/helpers/token.py
--rw-r--r--   0        0        0     3790 2023-04-07 18:14:01.626436 web3cli-1.1.3/tests/ape/tests/helpers/uniswap.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.626729 web3cli-1.1.3/tests/ape/tests/token/__init__.py
--rw-r--r--   0        0        0     1983 2023-04-07 18:14:01.627373 web3cli-1.1.3/tests/ape/tests/token/test_ape_token_approve.py
--rw-r--r--   0        0        0     2876 2023-04-07 18:14:01.627765 web3cli-1.1.3/tests/ape/tests/token/test_ape_token_transfer.py
--rw-r--r--   0        0        0     6467 2023-04-07 18:14:01.628071 web3cli-1.1.3/tests/ape/tests/token/test_ape_token_transferFrom.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.628193 web3cli-1.1.3/tests/ape/tests/uniswap/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-07 18:14:01.628531 web3cli-1.1.3/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py
--rw-r--r--   0        0        0      794 2023-04-07 18:14:01.628890 web3cli-1.1.3/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py
--rw-r--r--   0        0        0      487 2023-04-07 18:14:01.629400 web3cli-1.1.3/tests/conftest.py
--rw-r--r--   0        0        0     1130 2023-04-07 12:55:47.114434 web3cli-1.1.3/tests/helper.py
--rw-r--r--   0        0        0     3240 2023-06-08 17:29:54.142209 web3cli-1.1.3/tests/seed.py
--rw-r--r--   0        0        0        0 2022-12-28 17:01:25.438908 web3cli-1.1.3/tests/web3cli/__init__.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.297637 web3cli-1.1.3/tests/web3cli/controllers/__init__.py
--rw-r--r--   0        0        0     3754 2023-05-20 18:17:47.056601 web3cli-1.1.3/tests/web3cli/controllers/crud/test_address_controller.py
--rw-r--r--   0        0        0     3510 2023-06-10 17:49:12.472139 web3cli-1.1.3/tests/web3cli/controllers/crud/test_chain_controller.py
--rw-r--r--   0        0        0     8222 2023-05-20 18:17:47.058165 web3cli-1.1.3/tests/web3cli/controllers/crud/test_contract_controller.py
--rw-r--r--   0        0        0     2870 2023-05-20 18:17:47.058996 web3cli-1.1.3/tests/web3cli/controllers/crud/test_history_controller.py
--rw-r--r--   0        0        0     3741 2023-06-10 17:49:22.329714 web3cli-1.1.3/tests/web3cli/controllers/crud/test_rpc_controller.py
--rw-r--r--   0        0        0     4912 2023-06-10 17:49:27.241897 web3cli-1.1.3/tests/web3cli/controllers/crud/test_signer_controller.py
--rw-r--r--   0        0        0     6497 2023-06-10 17:50:24.793662 web3cli-1.1.3/tests/web3cli/controllers/crud/test_token_controller.py
--rw-r--r--   0        0        0     1848 2023-05-18 10:32:19.351291 web3cli-1.1.3/tests/web3cli/controllers/test_appkey_controller.py
--rw-r--r--   0        0        0     6385 2023-06-10 17:54:02.470548 web3cli-1.1.3/tests/web3cli/controllers/test_call_controller.py
--rw-r--r--   0        0        0     1027 2023-06-10 17:47:40.979271 web3cli-1.1.3/tests/web3cli/controllers/test_db_controller.py
--rw-r--r--   0        0        0     1664 2023-06-10 18:03:21.873923 web3cli-1.1.3/tests/web3cli/controllers/test_keyfile_controller.py
--rw-r--r--   0        0        0     6102 2023-06-10 18:00:00.614466 web3cli-1.1.3/tests/web3cli/controllers/test_misc_controller.py
--rw-r--r--   0        0        0     1210 2023-06-07 17:12:04.381111 web3cli-1.1.3/tests/web3cli/controllers/test_replay_controller.py
--rw-r--r--   0        0        0     3415 2023-05-20 18:17:47.063638 web3cli-1.1.3/tests/web3cli/controllers/test_send_controller.py
--rw-r--r--   0        0        0     9593 2023-05-20 18:17:47.064509 web3cli-1.1.3/tests/web3cli/controllers/test_transact_controller.py
--rw-r--r--   0        0        0     1265 2023-06-07 17:10:04.508480 web3cli-1.1.3/tests/web3cli/controllers/test_tx_controller.py
--rw-r--r--   0        0        0     1293 2023-04-07 18:14:01.632176 web3cli-1.1.3/tests/web3cli/fixtures.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.303802 web3cli-1.1.3/tests/web3cli/helpers/__init__.py
--rw-r--r--   0        0        0      684 2022-12-28 17:00:06.651527 web3cli-1.1.3/tests/web3cli/helpers/test_crypto_helper.py
--rw-r--r--   0        0        0     1455 2023-02-12 12:11:39.416778 web3cli-1.1.3/tests/web3cli/main.py
--rw-r--r--   0        0        0     1171 2023-02-11 18:15:39.713968 web3cli-1.1.3/tests/web3cli/test_db.py
--rw-r--r--   0        0        0      393 2023-02-11 18:16:36.584225 web3cli-1.1.3/tests/web3cli/test_main.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301380 web3cli-1.1.3/tests/web3core/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-18 11:01:18.894137 web3cli-1.1.3/tests/web3core/fixtures.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301610 web3cli-1.1.3/tests/web3core/helpers/__init__.py
--rw-r--r--   0        0        0     8923 2023-01-28 12:36:51.002666 web3cli-1.1.3/tests/web3core/helpers/test_abi_helper.py
--rw-r--r--   0        0        0      528 2022-12-28 16:44:57.745951 web3cli-1.1.3/tests/web3core/helpers/test_crypto_helper.py
--rw-r--r--   0        0        0     4807 2023-02-19 09:09:21.027684 web3cli-1.1.3/tests/web3core/helpers/test_resolve_address_helper.py
--rw-r--r--   0        0        0     1022 2023-01-29 17:56:31.054122 web3cli-1.1.3/tests/web3core/helpers/test_validation_helper.py
--rw-r--r--   0        0        0     1783 2023-01-14 21:27:16.475375 web3cli-1.1.3/tests/web3core/models/test_contract_model.py
--rw-r--r--   0        0        0    12487 1970-01-01 00:00:00.000000 web3cli-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-24 15:49:55.999119 web3cli-1.1.4/LICENSE
+-rw-r--r--   0        0        0    12341 2023-06-12 19:34:10.821303 web3cli-1.1.4/README.md
+-rw-r--r--   0        0        0     4057 2023-06-14 06:17:15.249740 web3cli-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-11-13 07:56:22.807127 web3cli-1.1.4/src/web3cli/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-18 22:32:14.016225 web3cli-1.1.4/src/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.198985 web3cli-1.1.4/src/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     4679 2023-06-10 16:49:18.164306 web3cli-1.1.4/src/web3cli/controllers/abi_controller.py
+-rw-r--r--   0        0        0     2049 2023-06-10 16:26:02.765052 web3cli-1.1.4/src/web3cli/controllers/app_key_controller.py
+-rw-r--r--   0        0        0     1215 2023-06-10 16:26:21.840704 web3cli-1.1.4/src/web3cli/controllers/base_controller.py
+-rw-r--r--   0        0        0     3106 2023-06-10 17:02:35.846994 web3cli-1.1.4/src/web3cli/controllers/call_controller.py
+-rw-r--r--   0        0        0     2421 2023-06-10 16:26:42.723101 web3cli-1.1.4/src/web3cli/controllers/config_controller.py
+-rw-r--r--   0        0        0     1109 2022-12-17 18:21:46.704206 web3cli-1.1.4/src/web3cli/controllers/controller.py
+-rw-r--r--   0        0        0        0 2023-03-25 21:06:13.922427 web3cli-1.1.4/src/web3cli/controllers/crud/__init__.py
+-rw-r--r--   0        0        0     2530 2023-06-10 16:49:44.923130 web3cli-1.1.4/src/web3cli/controllers/crud/address_controller.py
+-rw-r--r--   0        0        0     4413 2023-06-10 16:50:02.537767 web3cli-1.1.4/src/web3cli/controllers/crud/chain_controller.py
+-rw-r--r--   0        0        0     4785 2023-06-10 16:50:16.263301 web3cli-1.1.4/src/web3cli/controllers/crud/contract_controller.py
+-rw-r--r--   0        0        0     3035 2023-06-10 16:21:12.060981 web3cli-1.1.4/src/web3cli/controllers/crud/history_controller.py
+-rw-r--r--   0        0        0     2972 2023-06-10 16:35:01.955138 web3cli-1.1.4/src/web3cli/controllers/crud/rpc_controller.py
+-rw-r--r--   0        0        0     5282 2023-06-10 16:51:30.999842 web3cli-1.1.4/src/web3cli/controllers/crud/signer_controller.py
+-rw-r--r--   0        0        0     1390 2023-06-10 16:27:14.395424 web3cli-1.1.4/src/web3cli/controllers/db_controller.py
+-rw-r--r--   0        0        0      817 2023-06-12 19:19:49.774803 web3cli-1.1.4/src/web3cli/controllers/debug_controller.py
+-rw-r--r--   0        0        0     1479 2023-06-10 16:29:57.178158 web3cli-1.1.4/src/web3cli/controllers/keyfile_controller.py
+-rw-r--r--   0        0        0     4153 2023-06-10 18:07:14.344855 web3cli-1.1.4/src/web3cli/controllers/misc_controller.py
+-rw-r--r--   0        0        0     4471 2023-06-10 16:33:44.421618 web3cli-1.1.4/src/web3cli/controllers/replay_controller.py
+-rw-r--r--   0        0        0     2403 2023-06-10 16:33:58.579948 web3cli-1.1.4/src/web3cli/controllers/send_controller.py
+-rw-r--r--   0        0        0     5359 2023-06-14 06:14:09.058475 web3cli-1.1.4/src/web3cli/controllers/subscribe_controller.py
+-rw-r--r--   0        0        0     6878 2023-05-20 18:17:47.046015 web3cli-1.1.4/src/web3cli/controllers/swap_controller.py
+-rw-r--r--   0        0        0     7848 2023-06-10 17:57:16.099321 web3cli-1.1.4/src/web3cli/controllers/token_controller.py
+-rw-r--r--   0        0        0     2862 2023-05-20 18:17:47.047364 web3cli-1.1.4/src/web3cli/controllers/transact_controller.py
+-rw-r--r--   0        0        0     1239 2023-06-10 17:31:55.330976 web3cli-1.1.4/src/web3cli/controllers/tx_controller.py
+-rw-r--r--   0        0        0      341 2023-05-20 18:17:47.049010 web3cli-1.1.4/src/web3cli/exceptions.py
+-rw-r--r--   0        0        0     1329 2023-06-12 10:20:17.461216 web3cli-1.1.4/src/web3cli/framework/ext_print.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.191413 web3cli-1.1.4/src/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0    17851 2023-06-14 04:52:51.776300 web3cli-1.1.4/src/web3cli/helpers/args.py
+-rw-r--r--   0        0        0     2198 2023-05-20 18:17:47.051274 web3cli-1.1.4/src/web3cli/helpers/client_factory.py
+-rw-r--r--   0        0        0     1252 2022-12-28 16:44:58.644508 web3cli-1.1.4/src/web3cli/helpers/config.py
+-rw-r--r--   0        0        0     2092 2023-05-18 11:14:15.678582 web3cli-1.1.4/src/web3cli/helpers/crypto.py
+-rw-r--r--   0        0        0     1228 2023-02-11 17:24:24.959766 web3cli-1.1.4/src/web3cli/helpers/database.py
+-rw-r--r--   0        0        0     1776 2023-06-10 18:08:11.403330 web3cli-1.1.4/src/web3cli/helpers/render.py
+-rw-r--r--   0        0        0     4548 2023-06-07 12:09:20.814550 web3cli-1.1.4/src/web3cli/helpers/send.py
+-rw-r--r--   0        0        0     2178 2023-05-20 18:17:47.053233 web3cli-1.1.4/src/web3cli/helpers/signer.py
+-rw-r--r--   0        0        0     1429 2023-06-12 19:19:49.775947 web3cli-1.1.4/src/web3cli/helpers/telegram.py
+-rw-r--r--   0        0        0     2132 2023-06-07 12:22:03.729729 web3cli-1.1.4/src/web3cli/helpers/tx.py
+-rw-r--r--   0        0        0      435 2023-06-14 06:05:00.175697 web3cli-1.1.4/src/web3cli/helpers/version.py
+-rw-r--r--   0        0        0     2595 2023-02-12 21:33:06.910919 web3cli-1.1.4/src/web3cli/hooks.py
+-rw-r--r--   0        0        0     7780 2023-06-14 06:02:23.829441 web3cli-1.1.4/src/web3cli/main.py
+-rw-r--r--   0        0        0        0 2023-01-29 11:30:42.897043 web3cli-1.1.4/src/web3cli/templates/__init__.py
+-rw-r--r--   0        0        0      243 2023-01-29 11:41:03.173746 web3cli-1.1.4/src/web3cli/templates/balance.jinja2
+-rw-r--r--   0        0        0      120 2022-11-03 17:39:28.958124 web3cli-1.1.4/src/web3core/__init__.py
+-rw-r--r--   0        0        0       72 2023-02-19 11:02:13.393953 web3cli-1.1.4/src/web3core/constants.py
+-rw-r--r--   0        0        0       90 2023-01-18 19:29:57.558367 web3cli-1.1.4/src/web3core/db.py
+-rw-r--r--   0        0        0     1762 2023-01-18 20:41:45.295870 web3cli-1.1.4/src/web3core/exceptions.py
+-rw-r--r--   0        0        0        0 2022-11-03 17:39:28.958845 web3cli-1.1.4/src/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     9448 2023-04-07 18:14:01.618698 web3cli-1.1.4/src/web3core/helpers/abi.py
+-rw-r--r--   0        0        0     1148 2023-05-17 09:47:21.910041 web3cli-1.1.4/src/web3core/helpers/blocks.py
+-rw-r--r--   0        0        0     3405 2023-05-20 18:17:47.055119 web3cli-1.1.4/src/web3core/helpers/client_factory.py
+-rw-r--r--   0        0        0     1060 2022-12-17 18:21:46.707584 web3cli-1.1.4/src/web3core/helpers/crypto.py
+-rw-r--r--   0        0        0      714 2023-02-11 17:32:11.986925 web3cli-1.1.4/src/web3core/helpers/database.py
+-rw-r--r--   0        0        0     1582 2023-04-07 18:14:01.619156 web3cli-1.1.4/src/web3core/helpers/dex.py
+-rw-r--r--   0        0        0      434 2022-12-19 20:01:36.985004 web3cli-1.1.4/src/web3core/helpers/format.py
+-rw-r--r--   0        0        0     2413 2023-05-18 08:42:25.689036 web3cli-1.1.4/src/web3core/helpers/misc.py
+-rw-r--r--   0        0        0      532 2022-12-16 06:48:29.391730 web3cli-1.1.4/src/web3core/helpers/os.py
+-rw-r--r--   0        0        0     1799 2023-06-10 15:39:08.908650 web3cli-1.1.4/src/web3core/helpers/resolve.py
+-rw-r--r--   0        0        0      827 2023-06-10 09:19:32.610030 web3cli-1.1.4/src/web3core/helpers/rpc.py
+-rw-r--r--   0        0        0     2158 2023-01-14 21:27:16.459461 web3cli-1.1.4/src/web3core/helpers/seed.py
+-rw-r--r--   0        0        0      697 2023-06-12 19:19:49.776495 web3cli-1.1.4/src/web3core/helpers/telegram.py
+-rw-r--r--   0        0        0     4697 2023-04-07 18:14:01.620145 web3cli-1.1.4/src/web3core/helpers/tx.py
+-rw-r--r--   0        0        0      553 2023-06-12 19:19:49.776790 web3cli-1.1.4/src/web3core/helpers/validation.py
+-rw-r--r--   0        0        0     1207 2022-12-28 16:44:58.644659 web3cli-1.1.4/src/web3core/helpers/yaml.py
+-rw-r--r--   0        0        0      424 2023-01-18 19:29:57.562778 web3cli-1.1.4/src/web3core/models/__init__.py
+-rw-r--r--   0        0        0     1790 2023-01-18 19:29:57.563744 web3cli-1.1.4/src/web3core/models/address.py
+-rw-r--r--   0        0        0     3433 2023-05-20 18:17:47.055757 web3cli-1.1.4/src/web3core/models/base_model.py
+-rw-r--r--   0        0        0     4923 2023-03-25 21:22:51.453293 web3cli-1.1.4/src/web3core/models/chain.py
+-rw-r--r--   0        0        0     4262 2023-05-31 08:53:51.850966 web3cli-1.1.4/src/web3core/models/contract.py
+-rw-r--r--   0        0        0     1405 2023-05-18 09:25:11.305140 web3cli-1.1.4/src/web3core/models/signer.py
+-rw-r--r--   0        0        0     1054 2022-12-28 16:44:59.161817 web3cli-1.1.4/src/web3core/models/timestamps_model.py
+-rw-r--r--   0        0        0     2550 2022-12-28 16:44:59.162568 web3cli-1.1.4/src/web3core/models/tx.py
+-rw-r--r--   0        0        0     1449 2023-01-18 19:29:57.566552 web3cli-1.1.4/src/web3core/models/types.py
+-rw-r--r--   0        0        0       48 2022-11-18 22:43:37.360850 web3cli-1.1.4/src/web3core/seeds/__init__.py
+-rw-r--r--   0        0        0     3164 2023-06-08 14:39:52.689918 web3cli-1.1.4/src/web3core/seeds/chain_seeds.py
+-rw-r--r--   0        0        0      521 2023-06-08 14:37:27.133219 web3cli-1.1.4/src/web3core/seeds/contract_seeds.py
+-rw-r--r--   0        0        0    49489 2023-02-19 09:09:21.024661 web3cli-1.1.4/src/web3core/seeds/contract_type_seeds.py
+-rw-r--r--   0        0        0     9720 2023-02-27 16:48:07.675984 web3cli-1.1.4/src/web3core/seeds/contracts/arb_contract_seeds.py
+-rw-r--r--   0        0        0     1881 2023-02-27 19:24:54.136969 web3cli-1.1.4/src/web3core/seeds/contracts/avax_contract_seeds.py
+-rw-r--r--   0        0        0      867 2023-06-10 15:43:36.615089 web3cli-1.1.4/src/web3core/seeds/contracts/bnb_contract_seeds.py
+-rw-r--r--   0        0        0      611 2023-05-25 15:43:35.647237 web3cli-1.1.4/src/web3core/seeds/contracts/era_contract_seeds.py
+-rw-r--r--   0        0        0      997 2023-06-08 14:37:20.947238 web3cli-1.1.4/src/web3core/seeds/contracts/erat_contract_seeds.py
+-rw-r--r--   0        0        0     1579 2023-02-27 16:48:24.467166 web3cli-1.1.4/src/web3core/seeds/contracts/eth_contract_seeds.py
+-rw-r--r--   0        0        0     1183 2023-05-26 15:20:05.535496 web3cli-1.1.4/src/web3core/seeds/contracts/gno_contract_seeds.py
+-rw-r--r--   0        0        0     1448 2023-02-19 10:37:03.165028 web3cli-1.1.4/src/web3core/types.py
+-rw-r--r--   0        0        0     6148 2023-02-28 16:18:46.901853 web3cli-1.1.4/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.296564 web3cli-1.1.4/tests/__init__.py
+-rw-r--r--   0        0        0    10244 2023-02-28 16:18:44.627516 web3cli-1.1.4/tests/ape/.DS_Store
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.934034 web3cli-1.1.4/tests/ape/.build/Factory_IERC20.json
+-rw-r--r--   0        0        0      536 2023-04-06 17:43:03.934442 web3cli-1.1.4/tests/ape/.build/Factory_IUniswapV2Callee.json
+-rw-r--r--   0        0        0     3605 2023-04-06 17:43:03.935802 web3cli-1.1.4/tests/ape/.build/Factory_IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.936651 web3cli-1.1.4/tests/ape/.build/Factory_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.938968 web3cli-1.1.4/tests/ape/.build/Factory_IUniswapV2Pair.json
+-rw-r--r--   0        0        0      862 2023-04-06 17:43:03.939241 web3cli-1.1.4/tests/ape/.build/Factory_Math.json
+-rw-r--r--   0        0        0      866 2023-04-06 17:43:03.939527 web3cli-1.1.4/tests/ape/.build/Factory_SafeMath.json
+-rw-r--r--   0        0        0      867 2023-04-06 17:43:03.939780 web3cli-1.1.4/tests/ape/.build/Factory_UQ112x112.json
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.916870 web3cli-1.1.4/tests/ape/.build/Router_IERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.917744 web3cli-1.1.4/tests/ape/.build/Router_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.920204 web3cli-1.1.4/tests/ape/.build/Router_IUniswapV2Pair.json
+-rw-r--r--   0        0        0     9213 2023-04-06 17:43:03.922797 web3cli-1.1.4/tests/ape/.build/Router_IUniswapV2Router01.json
+-rw-r--r--   0        0        0    11845 2023-04-06 17:43:03.926066 web3cli-1.1.4/tests/ape/.build/Router_IUniswapV2Router02.json
+-rw-r--r--   0        0        0      683 2023-04-06 17:43:03.926558 web3cli-1.1.4/tests/ape/.build/Router_IWETH.json
+-rw-r--r--   0        0        0      872 2023-04-06 17:43:03.926867 web3cli-1.1.4/tests/ape/.build/Router_SafeMath.json
+-rw-r--r--   0        0        0      879 2023-04-06 17:43:03.927162 web3cli-1.1.4/tests/ape/.build/Router_TransferHelper.json
+-rw-r--r--   0        0        0      881 2023-04-06 17:43:03.927462 web3cli-1.1.4/tests/ape/.build/Router_UniswapV2Library.json
+-rw-r--r--   0        0        0    14895 2023-04-06 17:43:03.932635 web3cli-1.1.4/tests/ape/.build/Token.json
+-rw-r--r--   0        0        0      791 2023-04-06 17:43:03.932974 web3cli-1.1.4/tests/ape/.build/Token_SafeMath.json
+-rw-r--r--   0        0        0    14014 2023-04-06 17:43:03.941015 web3cli-1.1.4/tests/ape/.build/UniswapV2ERC20.json
+-rw-r--r--   0        0        0    46097 2023-04-06 17:43:03.942289 web3cli-1.1.4/tests/ape/.build/UniswapV2Factory.json
+-rw-r--r--   0        0        0    44784 2023-04-06 17:43:03.944616 web3cli-1.1.4/tests/ape/.build/UniswapV2Pair.json
+-rw-r--r--   0        0        0    85730 2023-04-06 17:43:03.931232 web3cli-1.1.4/tests/ape/.build/UniswapV2Router02.json
+-rw-r--r--   0        0        0   324962 2023-06-14 06:17:19.321015 web3cli-1.1.4/tests/ape/.build/__local__.json
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.620721 web3cli-1.1.4/tests/ape/__init__.py
+-rw-r--r--   0        0        0     6148 2023-02-28 16:18:44.554061 web3cli-1.1.4/tests/ape/contracts/.DS_Store
+-rw-r--r--   0        0        0     4101 2023-04-07 18:14:01.621230 web3cli-1.1.4/tests/ape/contracts/token/Token.sol
+-rw-r--r--   0        0        0      646 2023-04-07 18:14:01.621775 web3cli-1.1.4/tests/ape/contracts/token/Token_SafeMath.sol
+-rw-r--r--   0        0        0     6148 2023-02-28 15:31:57.501753 web3cli-1.1.4/tests/ape/contracts/uniswap/.DS_Store
+-rw-r--r--   0        0        0    21725 2023-04-07 18:14:01.622322 web3cli-1.1.4/tests/ape/contracts/uniswap/UniswapV2Factory.sol
+-rw-r--r--   0        0        0    34078 2023-04-07 18:14:01.622848 web3cli-1.1.4/tests/ape/contracts/uniswap/UniswapV2Router02.sol
+-rw-r--r--   0        0        0      236 2023-04-07 18:14:01.623357 web3cli-1.1.4/tests/ape/scripts/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-07 18:14:01.623719 web3cli-1.1.4/tests/ape/scripts/db.py
+-rw-r--r--   0        0        0      200 2023-04-07 18:14:01.624050 web3cli-1.1.4/tests/ape/scripts/token.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624201 web3cli-1.1.4/tests/ape/tests/__init__.py
+-rw-r--r--   0        0        0    13902 2023-04-07 18:14:01.624793 web3cli-1.1.4/tests/ape/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624997 web3cli-1.1.4/tests/ape/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      371 2023-04-07 18:14:01.625481 web3cli-1.1.4/tests/ape/tests/helpers/ape.py
+-rw-r--r--   0        0        0      881 2023-04-07 18:14:01.625860 web3cli-1.1.4/tests/ape/tests/helpers/token.py
+-rw-r--r--   0        0        0     3790 2023-04-07 18:14:01.626436 web3cli-1.1.4/tests/ape/tests/helpers/uniswap.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.626729 web3cli-1.1.4/tests/ape/tests/token/__init__.py
+-rw-r--r--   0        0        0     1983 2023-04-07 18:14:01.627373 web3cli-1.1.4/tests/ape/tests/token/test_ape_token_approve.py
+-rw-r--r--   0        0        0     2876 2023-04-07 18:14:01.627765 web3cli-1.1.4/tests/ape/tests/token/test_ape_token_transfer.py
+-rw-r--r--   0        0        0     6467 2023-04-07 18:14:01.628071 web3cli-1.1.4/tests/ape/tests/token/test_ape_token_transferFrom.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.628193 web3cli-1.1.4/tests/ape/tests/uniswap/__init__.py
+-rw-r--r--   0        0        0     4193 2023-04-07 18:14:01.628531 web3cli-1.1.4/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py
+-rw-r--r--   0        0        0      794 2023-04-07 18:14:01.628890 web3cli-1.1.4/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py
+-rw-r--r--   0        0        0      487 2023-04-07 18:14:01.629400 web3cli-1.1.4/tests/conftest.py
+-rw-r--r--   0        0        0     1130 2023-04-07 12:55:47.114434 web3cli-1.1.4/tests/helper.py
+-rw-r--r--   0        0        0     3240 2023-06-08 17:29:54.142209 web3cli-1.1.4/tests/seed.py
+-rw-r--r--   0        0        0        0 2022-12-28 17:01:25.438908 web3cli-1.1.4/tests/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.297637 web3cli-1.1.4/tests/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     3754 2023-05-20 18:17:47.056601 web3cli-1.1.4/tests/web3cli/controllers/crud/test_address_controller.py
+-rw-r--r--   0        0        0     3510 2023-06-10 17:49:12.472139 web3cli-1.1.4/tests/web3cli/controllers/crud/test_chain_controller.py
+-rw-r--r--   0        0        0     8222 2023-05-20 18:17:47.058165 web3cli-1.1.4/tests/web3cli/controllers/crud/test_contract_controller.py
+-rw-r--r--   0        0        0     2870 2023-05-20 18:17:47.058996 web3cli-1.1.4/tests/web3cli/controllers/crud/test_history_controller.py
+-rw-r--r--   0        0        0     3741 2023-06-10 17:49:22.329714 web3cli-1.1.4/tests/web3cli/controllers/crud/test_rpc_controller.py
+-rw-r--r--   0        0        0     4912 2023-06-10 17:49:27.241897 web3cli-1.1.4/tests/web3cli/controllers/crud/test_signer_controller.py
+-rw-r--r--   0        0        0     6497 2023-06-10 17:50:24.793662 web3cli-1.1.4/tests/web3cli/controllers/crud/test_token_controller.py
+-rw-r--r--   0        0        0     1848 2023-05-18 10:32:19.351291 web3cli-1.1.4/tests/web3cli/controllers/test_appkey_controller.py
+-rw-r--r--   0        0        0     6385 2023-06-10 17:54:02.470548 web3cli-1.1.4/tests/web3cli/controllers/test_call_controller.py
+-rw-r--r--   0        0        0     1027 2023-06-10 17:47:40.979271 web3cli-1.1.4/tests/web3cli/controllers/test_db_controller.py
+-rw-r--r--   0        0        0     1664 2023-06-10 18:03:21.873923 web3cli-1.1.4/tests/web3cli/controllers/test_keyfile_controller.py
+-rw-r--r--   0        0        0     6102 2023-06-10 18:00:00.614466 web3cli-1.1.4/tests/web3cli/controllers/test_misc_controller.py
+-rw-r--r--   0        0        0     1210 2023-06-07 17:12:04.381111 web3cli-1.1.4/tests/web3cli/controllers/test_replay_controller.py
+-rw-r--r--   0        0        0     3415 2023-05-20 18:17:47.063638 web3cli-1.1.4/tests/web3cli/controllers/test_send_controller.py
+-rw-r--r--   0        0        0     9593 2023-05-20 18:17:47.064509 web3cli-1.1.4/tests/web3cli/controllers/test_transact_controller.py
+-rw-r--r--   0        0        0     1265 2023-06-07 17:10:04.508480 web3cli-1.1.4/tests/web3cli/controllers/test_tx_controller.py
+-rw-r--r--   0        0        0     1293 2023-04-07 18:14:01.632176 web3cli-1.1.4/tests/web3cli/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.303802 web3cli-1.1.4/tests/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0      684 2022-12-28 17:00:06.651527 web3cli-1.1.4/tests/web3cli/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     1455 2023-02-12 12:11:39.416778 web3cli-1.1.4/tests/web3cli/main.py
+-rw-r--r--   0        0        0     1171 2023-02-11 18:15:39.713968 web3cli-1.1.4/tests/web3cli/test_db.py
+-rw-r--r--   0        0        0      393 2023-02-11 18:16:36.584225 web3cli-1.1.4/tests/web3cli/test_main.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301380 web3cli-1.1.4/tests/web3core/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-18 11:01:18.894137 web3cli-1.1.4/tests/web3core/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301610 web3cli-1.1.4/tests/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     8923 2023-01-28 12:36:51.002666 web3cli-1.1.4/tests/web3core/helpers/test_abi_helper.py
+-rw-r--r--   0        0        0      528 2022-12-28 16:44:57.745951 web3cli-1.1.4/tests/web3core/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     4807 2023-02-19 09:09:21.027684 web3cli-1.1.4/tests/web3core/helpers/test_resolve_address_helper.py
+-rw-r--r--   0        0        0     1022 2023-01-29 17:56:31.054122 web3cli-1.1.4/tests/web3core/helpers/test_validation_helper.py
+-rw-r--r--   0        0        0     1783 2023-01-14 21:27:16.475375 web3cli-1.1.4/tests/web3core/models/test_contract_model.py
+-rw-r--r--   0        0        0    12798 1970-01-01 00:00:00.000000 web3cli-1.1.4/PKG-INFO
```

### Comparing `web3cli-1.1.3/LICENSE` & `web3cli-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/README.md` & `web3cli-1.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: web3cli
+Version: 1.1.4
+Summary: Interact with blockchains and smart contracts using the command line
+License: MIT
+Keywords: web3,w3,cli,evm,blockchain,ethereum,binance,avalanche
+Author-email: coccoinomane <coccoinomane@gmail.com>
+Requires-Python: >=3.9,<3.11
+Project-URL: homepage, https://github.com/coccoinomane/web3cli
+Project-URL: repository, https://github.com/coccoinomane/web3cli
+Description-Content-Type: text/markdown
+
 <!-- https://shields.io/ --> 
 <p align="center">
     <a href="https://github.com/coccoinomane/web3cli/pulse" alt="Activity"><img src="https://img.shields.io/github/commit-activity/m/badges/shields?color=009051"/></a>
     <img src="https://img.shields.io/github/last-commit/coccoinomane/web3cli?color=009051"/>
 </p>
 <p align="center">
         <a href="https://www.alchemy.com/dapps/web3cli"><img style="width:150px;height:33px" src="https://static.alchemyapi.io/images/marketing/badge.png"/></a>
@@ -33,15 +45,15 @@
 
 - Interact with Ethereum and EVM-compatible chains via your terminal
 - Bypass sluggish and potentially compromised frontends
 - No configuration needed
 - Label addresses, tokens and contracts for ease of use
 - Swap with Uniswap, TraderJoe, PancakeSwap, etc
 - Transfer tokens via their ticker
-- Stream pending transactions, new blocks and contract events
+- Set Telegram alerts based on pending transactions, new blocks and contract events
 - Replay transactions just with the tx hash
 - Concatenate commands to build powerful scripts
 - Import signers via private key or keyfile
 - Thoroughly tested using the [Ape Framework](https://github.com/ApeWorX/ape)'s testing framework
 - [Windows compatible](https://github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows)
 
 Soon:
@@ -122,24 +134,26 @@
    ```
    w3 subscribe blocks   # stream blocks as they are mined
    w3 subscribe pending  # stream pending transactions
    w3 subscribe events   # stream all contract events
    ```
   Streaming requires a websocket connection: specify one with the `--rpc wss://...` flag.
 
-- Listen to events from specific contracts with specific topics:
+- Set a Telegram alert for when a specific event is emitted:
    ```bash
-   # Stream all events from USDC token
-   w3 subscribe events --contracts usdc 
-   # Stream only transfer events
-   w3 subscribe events --contracts usdc --topics 0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef
+   # Get notified on Telegram when USDC is transferred
+   transfer=0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef
+   w3 subscribe events --telegram --contracts usdc --topics $transfer
+   # Send a post notification when USDC is transferred
+   w3 subscribe events --post https://www.example.com/ --contracts usdc --topics $transfer
    ```
+  Telegram alerts require setting up a Telegram bot, please find instructions [in the Wiki](https://github.com/coccoinomane/web3cli/wiki/%F0%9F%93%AD-Telegram-alerts).
 
 - Replay a given transactions on the blockchain:
-   ```
+   ```bash
    tx=`w3 send unicef 1 USDC --force` # send 1 USDC to Unicef
    w3 replay $tx                      # re-send 1 USDC to Unicef
    ```
 
 # Smart Contract support
 
 `web3cli` comes preloaded with some popular smart contracts, including ERC20 tokens and Uniswap clones.
@@ -353,7 +367,8 @@
 # Contributing
 
 All contributions are welcome! To start improving `web3cli`, please refer to our [__contribution guide__](./CONTRIBUTING.md).
 
 # Acknowledgements
 
 Thank you very much to the communities behind [web3.py](https://github.com/ethereum/web3.py) and the [Ape Framework](https://github.com/ApeWorX/ape): `web3cli` would not exist without your efforts!
+
```

#### html2text {}

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1 Name: web3cli Version: 1.1.4 Summary: Interact with
+blockchains and smart contracts using the command line License: MIT Keywords:
+web3,w3,cli,evm,blockchain,ethereum,binance,avalanche Author-email:
+coccoinomane
+gmail.com> Requires-Python: >=3.9,<3.11 Project-URL: homepage, https://
+github.com/coccoinomane/web3cli Project-URL: repository, https://github.com/
+coccoinomane/web3cli Description-Content-Type: text/markdown
 [https://img.shields.io/github/commit-activity/m/badges/shields?color=009051]
  [https://img.shields.io/github/last-commit/coccoinomane/web3cli?color=009051]
            [https://static.alchemyapi.io/images/marketing/badge.png]
 Interact with blockchains and smart contracts using the command line: no coding
 needed! # Table of contents - [Features](#features) - [Install](#install) -
 [Simple examples](#simple-examples) - [Advanced examples](#advanced-examples) -
 [Smart Contract support](#smart-contract-support) + [Read from a smart
@@ -11,30 +18,30 @@
 book](#address-book) - [Wallet management](#wallet-management) + [Default
 signer](#default-signer) + [Create new private keys](#create-new-private-keys)
 - [Documentation](#documentation) - [Contributing](#contributing) -
 [Acknowledgements](#acknowledgements) # Features - Interact with Ethereum and
 EVM-compatible chains via your terminal - Bypass sluggish and potentially
 compromised frontends - No configuration needed - Label addresses, tokens and
 contracts for ease of use - Swap with Uniswap, TraderJoe, PancakeSwap, etc -
-Transfer tokens via their ticker - Stream pending transactions, new blocks and
-contract events - Replay transactions just with the tx hash - Concatenate
-commands to build powerful scripts - Import signers via private key or keyfile
-- Thoroughly tested using the [Ape Framework](https://github.com/ApeWorX/ape)'s
-testing framework - [Windows compatible](https://github.com/coccoinomane/
-web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows) Soon: - React to pending
-transactions, new blocks and contract events - Set up scheduled buys and sells
-(DCA) - Automatically buy when slippage is low enough - Get notified on
-Telegram when a pair is liquid enough, or unbalanced - Analyze on-chain data
-for tax or sleuthing purposes - Claim and reinvest yield from DeFi protocols #
-Install Make sure you have at least Python 3.7 installed, then run: ```bash
-pip3 install -U web3cli ``` Windows user? [Here's a tutorial for you](https://
-github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows)! #
-Simple examples - Get the ETH balance of any address: ``` w3 balance
-0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae ``` - Save addresses with easy-to-
-rember tags: ``` w3 address add unicef
+Transfer tokens via their ticker - Set Telegram alerts based on pending
+transactions, new blocks and contract events - Replay transactions just with
+the tx hash - Concatenate commands to build powerful scripts - Import signers
+via private key or keyfile - Thoroughly tested using the [Ape Framework](https:
+//github.com/ApeWorX/ape)'s testing framework - [Windows compatible](https://
+github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows) Soon:
+- React to pending transactions, new blocks and contract events - Set up
+scheduled buys and sells (DCA) - Automatically buy when slippage is low enough
+- Get notified on Telegram when a pair is liquid enough, or unbalanced -
+Analyze on-chain data for tax or sleuthing purposes - Claim and reinvest yield
+from DeFi protocols # Install Make sure you have at least Python 3.7 installed,
+then run: ```bash pip3 install -U web3cli ``` Windows user? [Here's a tutorial
+for you](https://github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-
+on-Windows)! # Simple examples - Get the ETH balance of any address: ``` w3
+balance 0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae ``` - Save addresses with
+easy-to-rember tags: ``` w3 address add unicef
 0xa59b29d7dbc9794d1e7f45123c48b2b8d0a34636 ``` then use the tag in any command:
 ``` w3 balance unicef ``` - Fetch blocks from the blockchain, in easy-to-read
 JSON format: ```bash w3 block latest w3 block finalized w3 block 6094305 ``` -
 Fetch transactions & receipts from the blockchain: ```bash w3 tx get
 0x3bbdcc2c7721521f7c767b7873ccb857f0816ac94e9f32c5601f4b15c87d1ef1 w3 tx rc
 0x3bbdcc2c7721521f7c767b7873ccb857f0816ac94e9f32c5601f4b15c87d1ef1 ``` -
 Extract single fields from blocks or transactions, using `jq` (more details [in
@@ -46,34 +53,39 @@
 send unicef 1 usdc # send 1 USDC ``` - Swap tokens on a DEX: ``` w3 swap
 uniswap_v2 1 usdc usdt # swap 1 USDC for USDT on Uniswap w3avax swap traderjoe
 1 usdc wavax # swap 1 USDC for WAVAX on TraderJoe ``` - Stream blocks,
 transactions and contract events as they happen in realtime: ``` w3 subscribe
 blocks # stream blocks as they are mined w3 subscribe pending # stream pending
 transactions w3 subscribe events # stream all contract events ``` Streaming
 requires a websocket connection: specify one with the `--rpc wss://...` flag. -
-Listen to events from specific contracts with specific topics: ```bash # Stream
-all events from USDC token w3 subscribe events --contracts usdc # Stream only
-transfer events w3 subscribe events --contracts usdc --topics
-0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef ``` - Replay
-a given transactions on the blockchain: ``` tx=`w3 send unicef 1 USDC --force`
-# send 1 USDC to Unicef w3 replay $tx # re-send 1 USDC to Unicef ``` # Smart
-Contract support `web3cli` comes preloaded with some popular smart contracts,
-including ERC20 tokens and Uniswap clones. See the available contracts with `w3
-contract list`: ``` w3 contract list # contracts on Ethereum w3 contract list -
--chain bnb # contracts on BNB chain w3 contract list --type erc20 # tokens on
-Ethereum ``` You can also add custom contracts with `w3 contract add`: ``` w3
-contract add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 --type erc20 w3
-contract add sushi 0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F --type uniswap_v2
-``` To add or list new tokens, you can use the `w3 token` shorthand: ``` w3
-token add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 w3 token list w3
-token delete weth ``` See available functions and events on a contract with `w3
-abi functions` and `w3 abi events`: ``` w3 abi fns weth # functions on WETH
-token w3 abi evs uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json #
-functions of an arbitrary ABI ``` ### Read from a smart contract To read from a
-smart contract, use `w3 call`. For example, to get the total supply of the WETH
-token, run: ``` w3 call weth totalSupply ``` Function arguments are parsed
-automatically, so you can call `balanceOf` with: ``` w3 call weth balanceOf
+Set a Telegram alert for when a specific event is emitted: ```bash # Get
+notified on Telegram when USDC is transferred
+transfer=0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef w3
+subscribe events --telegram --contracts usdc --topics $transfer # Send a post
+notification when USDC is transferred w3 subscribe events --post https://
+www.example.com/ --contracts usdc --topics $transfer ``` Telegram alerts
+require setting up a Telegram bot, please find instructions [in the Wiki]
+(https://github.com/coccoinomane/web3cli/wiki/%F0%9F%93%AD-Telegram-alerts). -
+Replay a given transactions on the blockchain: ```bash tx=`w3 send unicef 1
+USDC --force` # send 1 USDC to Unicef w3 replay $tx # re-send 1 USDC to Unicef
+``` # Smart Contract support `web3cli` comes preloaded with some popular smart
+contracts, including ERC20 tokens and Uniswap clones. See the available
+contracts with `w3 contract list`: ``` w3 contract list # contracts on Ethereum
+w3 contract list --chain bnb # contracts on BNB chain w3 contract list --type
+erc20 # tokens on Ethereum ``` You can also add custom contracts with `w3
+contract add`: ``` w3 contract add weth
+0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 --type erc20 w3 contract add sushi
+0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F --type uniswap_v2 ``` To add or list
+new tokens, you can use the `w3 token` shorthand: ``` w3 token add weth
+0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 w3 token list w3 token delete weth
+``` See available functions and events on a contract with `w3 abi functions`
+and `w3 abi events`: ``` w3 abi fns weth # functions on WETH token w3 abi evs
+uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json # functions of an
+arbitrary ABI ``` ### Read from a smart contract To read from a smart contract,
+use `w3 call`. For example, to get the total supply of the WETH token, run: ```
+w3 call weth totalSupply ``` Function arguments are parsed automatically, so
+you can call `balanceOf` with: ``` w3 call weth balanceOf
 0xA59B29d7dbC9794d1e7f45123C48b2b8d0a34636 ``` You can also do more complex
 stuff like: ```bash # get the amount of USDT you get for 100 USDC w3 call
 uniswap_v2 getAmountsOut 100e6 usdc,usdt | jq -r '.[1]' ``` ### Send a
 transaction to a smart contract To write to the blockchain, use `w3 transact`.
 For example, to transfer 1 ETH to address, run: ``` w3 transact weth transfer
```

### Comparing `web3cli-1.1.3/pyproject.toml` & `web3cli-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "web3cli"
-version = "1.1.3"
+version = "1.1.4"
 description = "Interact with blockchains and smart contracts using the command line"
 authors = [
     { name = "coccoinomane", email = "coccoinomane@gmail.com" },
 ]
 readme = "README.md"
 keywords = [
     "web3",
@@ -20,15 +20,15 @@
 dependencies = [
     "cement>=3.0.8",
     "cement[colorlog]>=3.0.8",
     "cement[jinja2]>=3.0.8",
     "cement[yaml]>=3.0.8",
     "cement[tabulate]>=3.0.8",
     "web3>=6.0.0",
-    "web3client>=1.1.9",
+    "web3client>=1.1.11",
     "peewee>=3.15.3",
     "cryptography>=38.0.3",
     "ruamel.yaml>=0.17.21",
     "typing-extensions>=4.4.0",
     "eth-account>=0.8.0",
 ]
 
@@ -55,14 +55,15 @@
 dev = [
     "mypy>=0.982",
     "eth-ape[recommended-plugins]>=0.6.0",
     "isort>=5.11.3",
     "pre-commit>=2.20.0",
     "autoflake>=2.0.0",
     "black>=22.10",
+    "types-requests>=2.31.0",
 ]
 
 [tool.pdm.scripts]
 test = "ape test tests --network ::foundry"
 test_verbose = "ape test tests -s --network ::foundry"
 test_fast = "ape test tests -m 'not remote' --network ::foundry"
 db_open = "open -a TablePlus $HOME/.web3cli/database/web3cli.sqlite"
```

### Comparing `web3cli-1.1.3/src/web3cli/.DS_Store` & `web3cli-1.1.4/src/web3cli/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/abi_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/abi_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/app_key_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/app_key_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/base_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/call_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/call_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/config_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/config_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/controller.py` & `web3cli-1.1.4/src/web3cli/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/crud/address_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/crud/address_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/crud/chain_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/crud/chain_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/crud/contract_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/crud/contract_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/crud/history_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/crud/history_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/crud/rpc_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/crud/rpc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/crud/signer_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/crud/signer_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/db_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/db_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/debug_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/debug_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/keyfile_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/keyfile_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/misc_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/misc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/replay_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/replay_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/send_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/send_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/subscribe_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/subscribe_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,80 +20,99 @@
     """Handler of the `w3 subscribe` commands"""
 
     class Meta:
         label = "subscribe"
         help = "Subscribe to stuff happening on the blockchain. Requires a websocket connection.  It uses the 'eth_subscribe' RPC method, which is not supported by all chains and nodes.  More details here > https://geth.ethereum.org/docs/interacting-with-geth/rpc/pubsub"
         stacked_type = "nested"
         stacked_on = "base"
+        aliases = ["sub"]
 
     @ex(
         help="Show new blocks as they are mined.  Uses the 'newHeads' subscription.",
         arguments=[*args.subscribe_actions(), *args.chain_and_rpc()],
         aliases=["block", "headers"],
     )
     def blocks(self) -> None:
         check_ws_or_raise(self.app.rpc.url)
+        self.app.log.info("Subscribing to new blocks, press Ctrl+C to stop...")
         asyncio.run(
             make_client(self.app).async_subscribe(
                 on_notification=self.get_callback(),
                 subscription_type="newHeads",
             )
         )
 
     @ex(
         help="Show new transactions before they are mined.  Uses the 'newPendingTransactions' subscription, which is supported only by chains with a mempool.",
-        arguments=[*args.subscribe_actions(), *args.chain_and_rpc()],
+        arguments=[
+            args.subscribe_senders(),
+            *args.subscribe_actions(),
+            *args.chain_and_rpc(),
+        ],
         aliases=["pending_txs", "txs"],
     )
     def pending(self) -> None:
         check_ws_or_raise(self.app.rpc.url)
+        self.app.log.info(
+            "Subscribing to new pending transactions, press Ctrl+C to stop..."
+        )
         asyncio.run(
             make_client(self.app).async_subscribe(
                 on_notification=self.get_callback(),
                 subscription_type="newPendingTransactions",
+                tx_from=[
+                    resolve_address(a, chain=self.app.chain.name)
+                    for a in self.app.pargs.senders
+                ],
+                tx_on_fetch_error=lambda e, data: self.app.log.warning(e),
             )
         )
 
     @ex(
         help="Show contract events as they are emitted.  Uses the 'logs' subscription.",
         arguments=[
             (
-                ["--addresses", "--contracts"],
+                ["--contracts"],
                 {
-                    "help": "Only show events from these addresses",
+                    "help": "Consider only events emitted by these smart contracts",
                     "nargs": "+",
-                    "type": str,
                     "default": [],
                 },
             ),
             (
                 ["--topics"],
                 {
-                    "help": "Only show events with these topics",
+                    "help": "Consider only events with these topics",
                     "nargs": "+",
-                    "type": str,
                     "default": [],
                 },
             ),
+            args.subscribe_senders(),
             *args.subscribe_actions(),
             *args.chain_and_rpc(),
         ],
         aliases=["logs"],
     )
     def events(self) -> None:
         check_ws_or_raise(self.app.rpc.url)
+        self.app.log.info("Subscribing to new events, press Ctrl+C to stop...")
         asyncio.run(
             make_client(self.app).async_subscribe(
                 on_notification=self.get_callback(),
                 subscription_type="logs",
                 logs_addresses=[
                     resolve_address(a, chain=self.app.chain.name)
-                    for a in self.app.pargs.addresses
+                    for a in self.app.pargs.contracts
                 ],
                 logs_topics=self.app.pargs.topics,
+                tx_from=[
+                    resolve_address(a, chain=self.app.chain.name)
+                    for a in self.app.pargs.senders
+                ],
+                tx_on_fetch_error=lambda e, data: self.app.log.warning(e),
             )
         )
 
     def get_callback(self) -> Callable[[Any], Awaitable[None]]:
         """Return the callback to invoke when a notification is received,
         based on the command arguments."""
 
@@ -106,16 +125,16 @@
                 send_tg_message(
                     self.app,
                     body=json.dumps(data, indent=4),
                     chat_id=self.app.pargs.telegram
                     if self.app.pargs.telegram != "config"
                     else None,
                 )
+            # POST CALLBACK
             if self.app.pargs.post:
-                # POST CALLBACK
                 url = self.app.pargs.post[0]
                 if not is_valid_url(url):
                     raise Web3CliError(f"Invalid URL: {url}")
                 requests.post(
                     url=url,
                     data=json.dumps(data),
                     headers={"Content-Type": "application/json"},
```

### Comparing `web3cli-1.1.3/src/web3cli/controllers/swap_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/swap_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/token_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/token_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/transact_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/transact_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/controllers/tx_controller.py` & `web3cli-1.1.4/src/web3cli/controllers/tx_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/framework/ext_print.py` & `web3cli-1.1.4/src/web3cli/framework/ext_print.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/helpers/args.py` & `web3cli-1.1.4/src/web3cli/helpers/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,14 +525,28 @@
             "action": argparse.BooleanOptionalAction,
             "default": True,
         }
         | kwargs,
     )
 
 
+def subscribe_senders(
+    *name_or_flags: str, **kwargs: Any
+) -> Tuple[List[str], dict[str, Any]]:
+    return (
+        list(name_or_flags) or ["--senders", "--from"],
+        {
+            "help": "Consider only transactions initiated by these addresses.  Will result in many requests to the node.",
+            "nargs": "+",
+            "default": [],
+        }
+        | kwargs,
+    )
+
+
 def subscribe_actions() -> List[Tuple[List[str], dict[str, Any]]]:
     """Shortcut for commands that trigger actions"""
     return [
         subscribe_telegram(),
         subscribe_post(),
         subscribe_print(),
     ]
```

### Comparing `web3cli-1.1.3/src/web3cli/helpers/client_factory.py` & `web3cli-1.1.4/src/web3cli/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/helpers/config.py` & `web3cli-1.1.4/src/web3cli/helpers/config.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/helpers/crypto.py` & `web3cli-1.1.4/src/web3cli/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/helpers/database.py` & `web3cli-1.1.4/src/web3cli/helpers/database.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/helpers/render.py` & `web3cli-1.1.4/src/web3cli/helpers/render.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/helpers/send.py` & `web3cli-1.1.4/src/web3cli/helpers/send.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/helpers/signer.py` & `web3cli-1.1.4/src/web3cli/helpers/signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/helpers/telegram.py` & `web3cli-1.1.4/src/web3cli/helpers/telegram.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/helpers/tx.py` & `web3cli-1.1.4/src/web3cli/helpers/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/hooks.py` & `web3cli-1.1.4/src/web3cli/hooks.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3cli/main.py` & `web3cli-1.1.4/src/web3cli/main.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/exceptions.py` & `web3cli-1.1.4/src/web3core/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/abi.py` & `web3cli-1.1.4/src/web3core/helpers/abi.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/blocks.py` & `web3cli-1.1.4/src/web3core/helpers/blocks.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/client_factory.py` & `web3cli-1.1.4/src/web3core/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/crypto.py` & `web3cli-1.1.4/src/web3core/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/database.py` & `web3cli-1.1.4/src/web3core/helpers/database.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/dex.py` & `web3cli-1.1.4/src/web3core/helpers/dex.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/misc.py` & `web3cli-1.1.4/src/web3core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/os.py` & `web3cli-1.1.4/src/web3core/helpers/os.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/resolve.py` & `web3cli-1.1.4/src/web3core/helpers/resolve.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/rpc.py` & `web3cli-1.1.4/src/web3core/helpers/rpc.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/seed.py` & `web3cli-1.1.4/src/web3core/helpers/seed.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/telegram.py` & `web3cli-1.1.4/src/web3core/helpers/telegram.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/tx.py` & `web3cli-1.1.4/src/web3core/helpers/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/validation.py` & `web3cli-1.1.4/src/web3core/helpers/validation.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/helpers/yaml.py` & `web3cli-1.1.4/src/web3core/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/models/address.py` & `web3cli-1.1.4/src/web3core/models/address.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/models/base_model.py` & `web3cli-1.1.4/src/web3core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/models/chain.py` & `web3cli-1.1.4/src/web3core/models/chain.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/models/contract.py` & `web3cli-1.1.4/src/web3core/models/contract.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/models/signer.py` & `web3cli-1.1.4/src/web3core/models/signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/models/timestamps_model.py` & `web3cli-1.1.4/src/web3core/models/timestamps_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/models/tx.py` & `web3cli-1.1.4/src/web3core/models/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/models/types.py` & `web3cli-1.1.4/src/web3core/models/types.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/seeds/chain_seeds.py` & `web3cli-1.1.4/src/web3core/seeds/chain_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/seeds/contract_seeds.py` & `web3cli-1.1.4/src/web3core/seeds/contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/seeds/contract_type_seeds.py` & `web3cli-1.1.4/src/web3core/seeds/contract_type_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/seeds/contracts/arb_contract_seeds.py` & `web3cli-1.1.4/src/web3core/seeds/contracts/arb_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/seeds/contracts/avax_contract_seeds.py` & `web3cli-1.1.4/src/web3core/seeds/contracts/avax_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/seeds/contracts/bnb_contract_seeds.py` & `web3cli-1.1.4/src/web3core/seeds/contracts/bnb_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/seeds/contracts/era_contract_seeds.py` & `web3cli-1.1.4/src/web3core/seeds/contracts/era_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/seeds/contracts/erat_contract_seeds.py` & `web3cli-1.1.4/src/web3core/seeds/contracts/erat_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/seeds/contracts/eth_contract_seeds.py` & `web3cli-1.1.4/src/web3core/seeds/contracts/eth_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/seeds/contracts/gno_contract_seeds.py` & `web3cli-1.1.4/src/web3core/seeds/contracts/gno_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/src/web3core/types.py` & `web3cli-1.1.4/src/web3core/types.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/.DS_Store` & `web3cli-1.1.4/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.DS_Store` & `web3cli-1.1.4/tests/ape/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Factory_IERC20.json` & `web3cli-1.1.4/tests/ape/.build/Factory_IERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Factory_IUniswapV2Callee.json` & `web3cli-1.1.4/tests/ape/.build/Factory_IUniswapV2Callee.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Factory_IUniswapV2ERC20.json` & `web3cli-1.1.4/tests/ape/.build/Factory_IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Factory_IUniswapV2Factory.json` & `web3cli-1.1.4/tests/ape/.build/Factory_IUniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Factory_IUniswapV2Pair.json` & `web3cli-1.1.4/tests/ape/.build/Factory_IUniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Factory_Math.json` & `web3cli-1.1.4/tests/ape/.build/Factory_Math.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Factory_SafeMath.json` & `web3cli-1.1.4/tests/ape/.build/Factory_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Factory_UQ112x112.json` & `web3cli-1.1.4/tests/ape/.build/Factory_UQ112x112.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Router_IERC20.json` & `web3cli-1.1.4/tests/ape/.build/Router_IERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Router_IUniswapV2Factory.json` & `web3cli-1.1.4/tests/ape/.build/Router_IUniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Router_IUniswapV2Pair.json` & `web3cli-1.1.4/tests/ape/.build/Router_IUniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Router_IUniswapV2Router01.json` & `web3cli-1.1.4/tests/ape/.build/Router_IUniswapV2Router01.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Router_IUniswapV2Router02.json` & `web3cli-1.1.4/tests/ape/.build/Router_IUniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Router_IWETH.json` & `web3cli-1.1.4/tests/ape/.build/Router_IWETH.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Router_SafeMath.json` & `web3cli-1.1.4/tests/ape/.build/Router_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Router_TransferHelper.json` & `web3cli-1.1.4/tests/ape/.build/Router_TransferHelper.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Router_UniswapV2Library.json` & `web3cli-1.1.4/tests/ape/.build/Router_UniswapV2Library.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Token.json` & `web3cli-1.1.4/tests/ape/.build/Token.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/Token_SafeMath.json` & `web3cli-1.1.4/tests/ape/.build/Token_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/UniswapV2ERC20.json` & `web3cli-1.1.4/tests/ape/.build/UniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/UniswapV2Factory.json` & `web3cli-1.1.4/tests/ape/.build/UniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/UniswapV2Pair.json` & `web3cli-1.1.4/tests/ape/.build/UniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/UniswapV2Router02.json` & `web3cli-1.1.4/tests/ape/.build/UniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/.build/__local__.json` & `web3cli-1.1.4/tests/ape/.build/__local__.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/contracts/.DS_Store` & `web3cli-1.1.4/tests/ape/contracts/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/contracts/token/Token.sol` & `web3cli-1.1.4/tests/ape/contracts/token/Token.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/contracts/token/Token_SafeMath.sol` & `web3cli-1.1.4/tests/ape/contracts/token/Token_SafeMath.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/contracts/uniswap/.DS_Store` & `web3cli-1.1.4/tests/ape/contracts/uniswap/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/contracts/uniswap/UniswapV2Factory.sol` & `web3cli-1.1.4/tests/ape/contracts/uniswap/UniswapV2Factory.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/contracts/uniswap/UniswapV2Router02.sol` & `web3cli-1.1.4/tests/ape/contracts/uniswap/UniswapV2Router02.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/tests/fixtures.py` & `web3cli-1.1.4/tests/ape/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/tests/helpers/token.py` & `web3cli-1.1.4/tests/ape/tests/helpers/token.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/tests/helpers/uniswap.py` & `web3cli-1.1.4/tests/ape/tests/helpers/uniswap.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/tests/token/test_ape_token_approve.py` & `web3cli-1.1.4/tests/ape/tests/token/test_ape_token_approve.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/tests/token/test_ape_token_transfer.py` & `web3cli-1.1.4/tests/ape/tests/token/test_ape_token_transfer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/tests/token/test_ape_token_transferFrom.py` & `web3cli-1.1.4/tests/ape/tests/token/test_ape_token_transferFrom.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py` & `web3cli-1.1.4/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py` & `web3cli-1.1.4/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/helper.py` & `web3cli-1.1.4/tests/helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/seed.py` & `web3cli-1.1.4/tests/seed.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/crud/test_address_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/crud/test_address_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/crud/test_chain_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/crud/test_chain_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/crud/test_contract_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/crud/test_contract_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/crud/test_history_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/crud/test_history_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/crud/test_rpc_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/crud/test_rpc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/crud/test_signer_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/crud/test_signer_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/crud/test_token_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/crud/test_token_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/test_appkey_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/test_appkey_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/test_call_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/test_call_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/test_db_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/test_db_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/test_keyfile_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/test_keyfile_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/test_misc_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/test_misc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/test_replay_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/test_replay_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/test_send_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/test_send_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/test_transact_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/test_transact_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/controllers/test_tx_controller.py` & `web3cli-1.1.4/tests/web3cli/controllers/test_tx_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/fixtures.py` & `web3cli-1.1.4/tests/web3cli/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/helpers/test_crypto_helper.py` & `web3cli-1.1.4/tests/web3cli/helpers/test_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/main.py` & `web3cli-1.1.4/tests/web3cli/main.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3cli/test_db.py` & `web3cli-1.1.4/tests/web3cli/test_db.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3core/fixtures.py` & `web3cli-1.1.4/tests/web3core/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3core/helpers/test_abi_helper.py` & `web3cli-1.1.4/tests/web3core/helpers/test_abi_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3core/helpers/test_crypto_helper.py` & `web3cli-1.1.4/tests/web3core/helpers/test_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3core/helpers/test_resolve_address_helper.py` & `web3cli-1.1.4/tests/web3core/helpers/test_resolve_address_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3core/helpers/test_validation_helper.py` & `web3cli-1.1.4/tests/web3core/helpers/test_validation_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/tests/web3core/models/test_contract_model.py` & `web3cli-1.1.4/tests/web3core/models/test_contract_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.3/PKG-INFO` & `web3cli-1.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: web3cli
-Version: 1.1.3
-Summary: Interact with blockchains and smart contracts using the command line
-License: MIT
-Keywords: web3,w3,cli,evm,blockchain,ethereum,binance,avalanche
-Author-email: coccoinomane <coccoinomane@gmail.com>
-Requires-Python: >=3.9,<3.11
-Project-URL: homepage, https://github.com/coccoinomane/web3cli
-Project-URL: repository, https://github.com/coccoinomane/web3cli
-Description-Content-Type: text/markdown
-
 <!-- https://shields.io/ --> 
 <p align="center">
     <a href="https://github.com/coccoinomane/web3cli/pulse" alt="Activity"><img src="https://img.shields.io/github/commit-activity/m/badges/shields?color=009051"/></a>
     <img src="https://img.shields.io/github/last-commit/coccoinomane/web3cli?color=009051"/>
 </p>
 <p align="center">
         <a href="https://www.alchemy.com/dapps/web3cli"><img style="width:150px;height:33px" src="https://static.alchemyapi.io/images/marketing/badge.png"/></a>
@@ -45,15 +33,15 @@
 
 - Interact with Ethereum and EVM-compatible chains via your terminal
 - Bypass sluggish and potentially compromised frontends
 - No configuration needed
 - Label addresses, tokens and contracts for ease of use
 - Swap with Uniswap, TraderJoe, PancakeSwap, etc
 - Transfer tokens via their ticker
-- Stream pending transactions, new blocks and contract events
+- Set Telegram alerts based on pending transactions, new blocks and contract events
 - Replay transactions just with the tx hash
 - Concatenate commands to build powerful scripts
 - Import signers via private key or keyfile
 - Thoroughly tested using the [Ape Framework](https://github.com/ApeWorX/ape)'s testing framework
 - [Windows compatible](https://github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows)
 
 Soon:
@@ -134,24 +122,26 @@
    ```
    w3 subscribe blocks   # stream blocks as they are mined
    w3 subscribe pending  # stream pending transactions
    w3 subscribe events   # stream all contract events
    ```
   Streaming requires a websocket connection: specify one with the `--rpc wss://...` flag.
 
-- Listen to events from specific contracts with specific topics:
+- Set a Telegram alert for when a specific event is emitted:
    ```bash
-   # Stream all events from USDC token
-   w3 subscribe events --contracts usdc 
-   # Stream only transfer events
-   w3 subscribe events --contracts usdc --topics 0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef
+   # Get notified on Telegram when USDC is transferred
+   transfer=0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef
+   w3 subscribe events --telegram --contracts usdc --topics $transfer
+   # Send a post notification when USDC is transferred
+   w3 subscribe events --post https://www.example.com/ --contracts usdc --topics $transfer
    ```
+  Telegram alerts require setting up a Telegram bot, please find instructions [in the Wiki](https://github.com/coccoinomane/web3cli/wiki/%F0%9F%93%AD-Telegram-alerts).
 
 - Replay a given transactions on the blockchain:
-   ```
+   ```bash
    tx=`w3 send unicef 1 USDC --force` # send 1 USDC to Unicef
    w3 replay $tx                      # re-send 1 USDC to Unicef
    ```
 
 # Smart Contract support
 
 `web3cli` comes preloaded with some popular smart contracts, including ERC20 tokens and Uniswap clones.
@@ -365,8 +355,7 @@
 # Contributing
 
 All contributions are welcome! To start improving `web3cli`, please refer to our [__contribution guide__](./CONTRIBUTING.md).
 
 # Acknowledgements
 
 Thank you very much to the communities behind [web3.py](https://github.com/ethereum/web3.py) and the [Ape Framework](https://github.com/ApeWorX/ape): `web3cli` would not exist without your efforts!
-
```

#### html2text {}

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1 Name: web3cli Version: 1.1.3 Summary: Interact with
-blockchains and smart contracts using the command line License: MIT Keywords:
-web3,w3,cli,evm,blockchain,ethereum,binance,avalanche Author-email:
-coccoinomane
-gmail.com> Requires-Python: >=3.9,<3.11 Project-URL: homepage, https://
-github.com/coccoinomane/web3cli Project-URL: repository, https://github.com/
-coccoinomane/web3cli Description-Content-Type: text/markdown
 [https://img.shields.io/github/commit-activity/m/badges/shields?color=009051]
  [https://img.shields.io/github/last-commit/coccoinomane/web3cli?color=009051]
            [https://static.alchemyapi.io/images/marketing/badge.png]
 Interact with blockchains and smart contracts using the command line: no coding
 needed! # Table of contents - [Features](#features) - [Install](#install) -
 [Simple examples](#simple-examples) - [Advanced examples](#advanced-examples) -
 [Smart Contract support](#smart-contract-support) + [Read from a smart
@@ -18,30 +11,30 @@
 book](#address-book) - [Wallet management](#wallet-management) + [Default
 signer](#default-signer) + [Create new private keys](#create-new-private-keys)
 - [Documentation](#documentation) - [Contributing](#contributing) -
 [Acknowledgements](#acknowledgements) # Features - Interact with Ethereum and
 EVM-compatible chains via your terminal - Bypass sluggish and potentially
 compromised frontends - No configuration needed - Label addresses, tokens and
 contracts for ease of use - Swap with Uniswap, TraderJoe, PancakeSwap, etc -
-Transfer tokens via their ticker - Stream pending transactions, new blocks and
-contract events - Replay transactions just with the tx hash - Concatenate
-commands to build powerful scripts - Import signers via private key or keyfile
-- Thoroughly tested using the [Ape Framework](https://github.com/ApeWorX/ape)'s
-testing framework - [Windows compatible](https://github.com/coccoinomane/
-web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows) Soon: - React to pending
-transactions, new blocks and contract events - Set up scheduled buys and sells
-(DCA) - Automatically buy when slippage is low enough - Get notified on
-Telegram when a pair is liquid enough, or unbalanced - Analyze on-chain data
-for tax or sleuthing purposes - Claim and reinvest yield from DeFi protocols #
-Install Make sure you have at least Python 3.7 installed, then run: ```bash
-pip3 install -U web3cli ``` Windows user? [Here's a tutorial for you](https://
-github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows)! #
-Simple examples - Get the ETH balance of any address: ``` w3 balance
-0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae ``` - Save addresses with easy-to-
-rember tags: ``` w3 address add unicef
+Transfer tokens via their ticker - Set Telegram alerts based on pending
+transactions, new blocks and contract events - Replay transactions just with
+the tx hash - Concatenate commands to build powerful scripts - Import signers
+via private key or keyfile - Thoroughly tested using the [Ape Framework](https:
+//github.com/ApeWorX/ape)'s testing framework - [Windows compatible](https://
+github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows) Soon:
+- React to pending transactions, new blocks and contract events - Set up
+scheduled buys and sells (DCA) - Automatically buy when slippage is low enough
+- Get notified on Telegram when a pair is liquid enough, or unbalanced -
+Analyze on-chain data for tax or sleuthing purposes - Claim and reinvest yield
+from DeFi protocols # Install Make sure you have at least Python 3.7 installed,
+then run: ```bash pip3 install -U web3cli ``` Windows user? [Here's a tutorial
+for you](https://github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-
+on-Windows)! # Simple examples - Get the ETH balance of any address: ``` w3
+balance 0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae ``` - Save addresses with
+easy-to-rember tags: ``` w3 address add unicef
 0xa59b29d7dbc9794d1e7f45123c48b2b8d0a34636 ``` then use the tag in any command:
 ``` w3 balance unicef ``` - Fetch blocks from the blockchain, in easy-to-read
 JSON format: ```bash w3 block latest w3 block finalized w3 block 6094305 ``` -
 Fetch transactions & receipts from the blockchain: ```bash w3 tx get
 0x3bbdcc2c7721521f7c767b7873ccb857f0816ac94e9f32c5601f4b15c87d1ef1 w3 tx rc
 0x3bbdcc2c7721521f7c767b7873ccb857f0816ac94e9f32c5601f4b15c87d1ef1 ``` -
 Extract single fields from blocks or transactions, using `jq` (more details [in
@@ -53,34 +46,39 @@
 send unicef 1 usdc # send 1 USDC ``` - Swap tokens on a DEX: ``` w3 swap
 uniswap_v2 1 usdc usdt # swap 1 USDC for USDT on Uniswap w3avax swap traderjoe
 1 usdc wavax # swap 1 USDC for WAVAX on TraderJoe ``` - Stream blocks,
 transactions and contract events as they happen in realtime: ``` w3 subscribe
 blocks # stream blocks as they are mined w3 subscribe pending # stream pending
 transactions w3 subscribe events # stream all contract events ``` Streaming
 requires a websocket connection: specify one with the `--rpc wss://...` flag. -
-Listen to events from specific contracts with specific topics: ```bash # Stream
-all events from USDC token w3 subscribe events --contracts usdc # Stream only
-transfer events w3 subscribe events --contracts usdc --topics
-0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef ``` - Replay
-a given transactions on the blockchain: ``` tx=`w3 send unicef 1 USDC --force`
-# send 1 USDC to Unicef w3 replay $tx # re-send 1 USDC to Unicef ``` # Smart
-Contract support `web3cli` comes preloaded with some popular smart contracts,
-including ERC20 tokens and Uniswap clones. See the available contracts with `w3
-contract list`: ``` w3 contract list # contracts on Ethereum w3 contract list -
--chain bnb # contracts on BNB chain w3 contract list --type erc20 # tokens on
-Ethereum ``` You can also add custom contracts with `w3 contract add`: ``` w3
-contract add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 --type erc20 w3
-contract add sushi 0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F --type uniswap_v2
-``` To add or list new tokens, you can use the `w3 token` shorthand: ``` w3
-token add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 w3 token list w3
-token delete weth ``` See available functions and events on a contract with `w3
-abi functions` and `w3 abi events`: ``` w3 abi fns weth # functions on WETH
-token w3 abi evs uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json #
-functions of an arbitrary ABI ``` ### Read from a smart contract To read from a
-smart contract, use `w3 call`. For example, to get the total supply of the WETH
-token, run: ``` w3 call weth totalSupply ``` Function arguments are parsed
-automatically, so you can call `balanceOf` with: ``` w3 call weth balanceOf
+Set a Telegram alert for when a specific event is emitted: ```bash # Get
+notified on Telegram when USDC is transferred
+transfer=0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef w3
+subscribe events --telegram --contracts usdc --topics $transfer # Send a post
+notification when USDC is transferred w3 subscribe events --post https://
+www.example.com/ --contracts usdc --topics $transfer ``` Telegram alerts
+require setting up a Telegram bot, please find instructions [in the Wiki]
+(https://github.com/coccoinomane/web3cli/wiki/%F0%9F%93%AD-Telegram-alerts). -
+Replay a given transactions on the blockchain: ```bash tx=`w3 send unicef 1
+USDC --force` # send 1 USDC to Unicef w3 replay $tx # re-send 1 USDC to Unicef
+``` # Smart Contract support `web3cli` comes preloaded with some popular smart
+contracts, including ERC20 tokens and Uniswap clones. See the available
+contracts with `w3 contract list`: ``` w3 contract list # contracts on Ethereum
+w3 contract list --chain bnb # contracts on BNB chain w3 contract list --type
+erc20 # tokens on Ethereum ``` You can also add custom contracts with `w3
+contract add`: ``` w3 contract add weth
+0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 --type erc20 w3 contract add sushi
+0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F --type uniswap_v2 ``` To add or list
+new tokens, you can use the `w3 token` shorthand: ``` w3 token add weth
+0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 w3 token list w3 token delete weth
+``` See available functions and events on a contract with `w3 abi functions`
+and `w3 abi events`: ``` w3 abi fns weth # functions on WETH token w3 abi evs
+uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json # functions of an
+arbitrary ABI ``` ### Read from a smart contract To read from a smart contract,
+use `w3 call`. For example, to get the total supply of the WETH token, run: ```
+w3 call weth totalSupply ``` Function arguments are parsed automatically, so
+you can call `balanceOf` with: ``` w3 call weth balanceOf
 0xA59B29d7dbC9794d1e7f45123C48b2b8d0a34636 ``` You can also do more complex
 stuff like: ```bash # get the amount of USDT you get for 100 USDC w3 call
 uniswap_v2 getAmountsOut 100e6 usdc,usdt | jq -r '.[1]' ``` ### Send a
 transaction to a smart contract To write to the blockchain, use `w3 transact`.
 For example, to transfer 1 ETH to address, run: ``` w3 transact weth transfer
```

