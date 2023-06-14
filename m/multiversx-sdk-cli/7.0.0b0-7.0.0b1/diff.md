# Comparing `tmp/multiversx_sdk_cli-7.0.0b0.tar.gz` & `tmp/multiversx_sdk_cli-7.0.0b1.tar.gz`

## Comparing `multiversx_sdk_cli-7.0.0b0.tar` & `multiversx_sdk_cli-7.0.0b1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/__init__.py
--rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/accounts.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_accounts.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_block.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_config.py
--rw-r--r--   0        0        0    19541 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_contracts.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_data.py
--rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_delegation.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_deps.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_dns.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_ledger.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_localnet.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_network.py
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_output.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_password.py
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_shared.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_transactions.py
--rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_validators.py
--rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_wallet.py
--rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/config.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/constants.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/contract_verification.py
--rw-r--r--   0        0        0     9712 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/contracts.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cosign_transaction.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/diskcache.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dns.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/docker.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/downloader.py
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/errors.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/guards.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/interfaces.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/myprocess.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/simulation.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/transactions.py
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/utils.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ux.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/version.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/workstation.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/.vscode/settings.json
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/delegation/__init__.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/delegation/staking_provider.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dependencies/__init__.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dependencies/install.py
--rw-r--r--   0        0        0    16479 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dependencies/modules.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dependencies/resolution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/config.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/ledger_app_handler.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/ledger_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/__init__.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_default.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_general.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_networking.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_part.py
--rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_root.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_sharding.py
--rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_software.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/constants.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/genesis.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/genesis_json.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/genesis_smart_contracts_json.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/libraries.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/node.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/node_config_toml.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/nodes_setup_json.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/p2p_toml.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/seednode_p2pKey.pem
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_build_software.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_clean.py
--rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_config.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_new.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_prerequisites.py
--rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_start.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/wallets.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/constants.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/core.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/interfaces.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/migrations.py
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_base.py
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_clang.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_cpp.py
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_rust.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_sol.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/shared.py
--rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/templates.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/templates_config.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/templates_repository.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/do_report.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/report_creator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/__init__.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/common.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/extracted_feature.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/folder_report.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/project_report.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/wasm_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/__init__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/features.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/report_option.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/size.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/format/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/format/change_type.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/format/format_options.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/validators/__init__.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/validators/core.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/validators/validators_file.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/LICENSE
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/pyproject.toml
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/__init__.py
+-rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/accounts.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_accounts.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_block.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_config.py
+-rw-r--r--   0        0        0    19784 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_contracts.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_data.py
+-rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_delegation.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_deps.py
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_dns.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_ledger.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_localnet.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_network.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_output.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_password.py
+-rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_shared.py
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_transactions.py
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_validators.py
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_wallet.py
+-rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/config.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/constants.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/contract_verification.py
+-rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/contracts.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cosign_transaction.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/diskcache.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dns.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/docker.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/downloader.py
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/errors.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/guards.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/interfaces.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/myprocess.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/simulation.py
+-rw-r--r--   0        0        0    11018 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/transactions.py
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/utils.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ux.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/version.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/workstation.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/.vscode/settings.json
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/delegation/__init__.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/delegation/staking_provider.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dependencies/__init__.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dependencies/install.py
+-rw-r--r--   0        0        0    16479 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dependencies/modules.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dependencies/resolution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/config.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/ledger_app_handler.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/ledger_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/__init__.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_default.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_general.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_networking.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_part.py
+-rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_root.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_sharding.py
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_software.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/constants.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/genesis.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/genesis_json.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/genesis_smart_contracts_json.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/libraries.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/node.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/node_config_toml.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/nodes_setup_json.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/p2p_toml.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/seednode_p2pKey.pem
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_build_software.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_clean.py
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_config.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_new.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_prerequisites.py
+-rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_start.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/wallets.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/constants.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/core.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/interfaces.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/migrations.py
+-rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_base.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_clang.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_cpp.py
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_rust.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_sol.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/shared.py
+-rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/templates.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/templates_config.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/templates_repository.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/do_report.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/report_creator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/__init__.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/common.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/extracted_feature.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/folder_report.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/project_report.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/wasm_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/__init__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/features.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/report_option.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/size.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/format/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/format/change_type.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/format/format_options.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/validators/__init__.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/validators/core.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/validators/validators_file.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/LICENSE
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/PKG-INFO
```

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/accounts.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_accounts.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_block.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_block.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_config.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_contracts.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 from multiversx_sdk_cli.accounts import Account, Address, LedgerAccount
 from multiversx_sdk_cli.cli_output import CLIOutputBuilder
 from multiversx_sdk_cli.cli_password import load_password
 from multiversx_sdk_cli.contract_verification import \
     trigger_contract_verification
 from multiversx_sdk_cli.contracts import CodeMetadata, SmartContract
 from multiversx_sdk_cli.docker import is_docker_installed, run_docker
-from multiversx_sdk_cli.errors import DockerMissingError
-from multiversx_sdk_cli.projects import load_project
+from multiversx_sdk_cli.errors import DockerMissingError, NoWalletProvided
 from multiversx_sdk_cli.projects.core import get_project_paths_recursively
 from multiversx_sdk_cli.transactions import Transaction
 from multiversx_sdk_cli.cosign_transaction import cosign_transaction
 
 logger = logging.getLogger("cli.contracts")
 
 
@@ -67,26 +66,27 @@
     sub.add_argument("--output-file", type=Path, help="if specified, the output is written to a file, otherwise it's written to the standard output")
     sub.add_argument("--compare", type=Path, nargs='+', metavar=("report-1.json", "report-2.json"), help="create a comparison from two or more reports")
     _add_build_options_args(sub)
     sub.set_defaults(func=do_report)
 
     output_description = CLIOutputBuilder.describe(with_contract=True, with_transaction_on_network=True, with_simulation=True)
     sub = cli_shared.add_command_subparser(subparsers, "contract", "deploy", f"Deploy a Smart Contract.{output_description}")
-    _add_project_or_bytecode_arg(sub)
+    _add_bytecode_arg(sub)
     _add_metadata_arg(sub)
     cli_shared.add_outfile_arg(sub)
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_proxy_arg(sub)
     cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_guardian=True)
     _add_arguments_arg(sub)
     sub.add_argument("--wait-result", action="store_true", default=False,
                      help="signal to wait for the transaction result - only valid if --send is set")
     sub.add_argument("--timeout", default=100, help="max num of seconds to wait for result"
                                                     " - only valid if --wait-result is set")
     cli_shared.add_broadcast_args(sub)
+    cli_shared.add_guardian_wallet_args(args, sub)
 
     sub.set_defaults(func=deploy)
 
     sub = cli_shared.add_command_subparser(subparsers, "contract", "call",
                                            f"Interact with a Smart Contract (execute function).{output_description}")
     _add_contract_arg(sub)
     cli_shared.add_outfile_arg(sub)
@@ -96,32 +96,34 @@
     _add_function_arg(sub)
     _add_arguments_arg(sub)
     sub.add_argument("--wait-result", action="store_true", default=False,
                      help="signal to wait for the transaction result - only valid if --send is set")
     sub.add_argument("--timeout", default=100, help="max num of seconds to wait for result"
                                                     " - only valid if --wait-result is set")
     cli_shared.add_broadcast_args(sub, relay=True)
+    cli_shared.add_guardian_wallet_args(args, sub)
 
     sub.set_defaults(func=call)
 
     sub = cli_shared.add_command_subparser(subparsers, "contract", "upgrade",
                                            f"Upgrade a previously-deployed Smart Contract.{output_description}")
     _add_contract_arg(sub)
     cli_shared.add_outfile_arg(sub)
-    _add_project_or_bytecode_arg(sub)
+    _add_bytecode_arg(sub)
     _add_metadata_arg(sub)
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_proxy_arg(sub)
     cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_guardian=True)
     _add_arguments_arg(sub)
     sub.add_argument("--wait-result", action="store_true", default=False,
                      help="signal to wait for the transaction result - only valid if --send is set")
     sub.add_argument("--timeout", default=100, help="max num of seconds to wait for result"
                                                     " - only valid if --wait-result is set")
     cli_shared.add_broadcast_args(sub)
+    cli_shared.add_guardian_wallet_args(args, sub)
 
     sub.set_defaults(func=upgrade)
 
     sub = cli_shared.add_command_subparser(subparsers, "contract", "query",
                                            "Query a Smart Contract (call a pure function)")
     _add_contract_arg(sub)
     cli_shared.add_proxy_arg(sub)
@@ -143,14 +145,15 @@
     _add_contract_arg(sub)
     sub.add_argument(
         "--verifier-url",
         required=True,
         help="the url of the service that validates the contract",
     )
     sub.add_argument("--docker-image", required=True, help="the docker image used for the build")
+    sub.add_argument("--contract-variant", required=False, default=None, help="in case of a multicontract, specify the contract variant you want to verify")
     cli_shared.add_wallet_args(args, sub)
     sub.set_defaults(func=verify)
 
     sub = cli_shared.add_command_subparser(subparsers, "contract", "reproducible-build",
                                            "Build a Smart Contract and get the same output as a previously built Smart Contract")
     _add_project_arg(sub)
     _add_build_options_args(sub)
@@ -187,20 +190,17 @@
                      help="for rust projects, optionally specify the suffix of the wasm bytecode output file")
 
 
 def _add_recursive_arg(sub: Any):
     sub.add_argument("-r", "--recursive", dest="recursive", action="store_true", help="locate projects recursively")
 
 
-def _add_project_or_bytecode_arg(sub: Any):
-    group = sub.add_mutually_exclusive_group(required=True)
-    group.add_argument("--project", default=os.getcwd(),
-                       help="🗀 the project directory (default: current directory)")
-    group.add_argument("--bytecode", type=str,
-                       help="the file containing the WASM bytecode")
+def _add_bytecode_arg(sub: Any):
+    sub.add_argument("--bytecode", type=str, required=True,
+                     help="the file containing the WASM bytecode")
 
 
 def _add_contract_arg(sub: Any):
     sub.add_argument("contract", help="🖄 the address of the Smart Contract")
 
 
 def _add_function_arg(sub: Any):
@@ -281,45 +281,38 @@
     project_paths = get_project_paths(args)
     for project in project_paths:
         projects.run_tests(project, args)
 
 
 def deploy(args: Any):
     logger.debug("deploy")
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
 
     arguments = args.arguments
     gas_price = args.gas_price
     gas_limit = args.gas_limit
     value = args.value
     chain = args.chain
     version = args.version
 
     contract = _prepare_contract(args)
     sender = _prepare_sender(args)
 
     tx = contract.deploy(sender, arguments, gas_price, gas_limit, value, chain, version, args.guardian, args.options)
-
-    if args.guardian:
-        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
+    tx = _sign_guarded_tx(args, tx)
 
     logger.info("Contract address: %s", contract.address)
     utils.log_explorer_contract_address(chain, contract.address)
 
     _send_or_simulate(tx, contract, args)
 
 
 def _prepare_contract(args: Any) -> SmartContract:
-    if args.bytecode and len(args.bytecode):
-        bytecode = utils.read_binary_file(Path(args.bytecode)).hex()
-    else:
-        project_path = Path(args.project)
-        project = load_project(project_path)
-        bytecode = project.get_bytecode()
+    bytecode = utils.read_binary_file(Path(args.bytecode)).hex()
 
     metadata = CodeMetadata(upgradeable=args.metadata_upgradeable, readable=args.metadata_readable,
                             payable=args.metadata_payable, payable_by_sc=args.metadata_payable_by_sc)
     contract = SmartContract(bytecode=bytecode, metadata=metadata)
     return contract
 
 
@@ -356,17 +349,36 @@
         sender = Account(key_file=args.keyfile, password=password)
     else:
         raise errors.NoWalletProvided()
 
     return sender
 
 
+def _sign_guarded_tx(args: Any, tx: Transaction) -> Transaction:
+    signature = tx.signature
+    tx.signature = ""
+
+    try:
+        guardian_account = cli_shared.prepare_guardian_account(args)
+    except NoWalletProvided:
+        guardian_account = None
+
+    if guardian_account:
+        tx.guardianSignature = guardian_account.sign_transaction(tx)
+    elif args.guardian:
+        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)  # type: ignore
+
+    tx.signature = signature
+
+    return tx
+
+
 def call(args: Any):
     logger.debug("call")
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
 
     contract_address = args.contract
     function = args.function
     arguments = args.arguments
     gas_price = args.gas_price
     gas_limit = args.gas_limit
@@ -374,17 +386,15 @@
     chain = args.chain
     version = args.version
 
     contract = SmartContract(contract_address)
     sender = _prepare_sender(args)
 
     tx = contract.execute(sender, function, arguments, gas_price, gas_limit, value, chain, version, args.guardian, args.options)
-
-    if args.guardian:
-        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
+    tx = _sign_guarded_tx(args, tx)
 
     _send_or_simulate(tx, contract, args)
 
 
 def upgrade(args: Any):
     logger.debug("upgrade")
     cli_shared.check_broadcast_args(args)
@@ -397,18 +407,16 @@
     chain = args.chain
     version = args.version
 
     contract = _prepare_contract(args)
     contract.address = Address(contract_address)
     sender = _prepare_sender(args)
 
-    tx = contract.upgrade(sender, arguments, gas_price, gas_limit, value, chain, version, args.guardian_address, args.options)
-
-    if args.guardian:
-        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
+    tx = contract.upgrade(sender, arguments, gas_price, gas_limit, value, chain, version, args.guardian, args.options)
+    tx = _sign_guarded_tx(args, tx)
 
     _send_or_simulate(tx, contract, args)
 
 
 def query(args: Any):
     logger.debug("query")
 
@@ -431,17 +439,18 @@
     contract = Address(args.contract)
     verifier_url = args.verifier_url
 
     packaged_src = Path(args.packaged_src).expanduser().resolve()
 
     owner = _prepare_signer(args)
     docker_image = args.docker_image
+    contract_variant = args.contract_variant
 
     trigger_contract_verification(
-        packaged_src, owner, contract, verifier_url, docker_image
+        packaged_src, owner, contract, verifier_url, docker_image, contract_variant
     )
     logger.info("Contract verification request completed!")
 
 
 def do_reproducible_build(args: Any):
     project_path = args.project
     docker_image = args.docker_image
```

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_data.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_data.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_delegation.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_delegation.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,18 +130,19 @@
 
 def _add_common_arguments(args: List[str], sub: Any):
     cli_shared.add_proxy_arg(sub)
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_estimate_gas=True, with_guardian=True)
     cli_shared.add_broadcast_args(sub, relay=False)
     cli_shared.add_outfile_arg(sub, what="signed transaction, hash")
+    cli_shared.add_guardian_wallet_args(args, sub)
 
 
 def do_create_delegation_contract(args: Any):
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_create_new_staking_contract(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
@@ -157,114 +158,114 @@
         contract_address = transaction_events[0].address
         print(contract_address.bech32())
     else:
         raise errors.ProgrammingError("Tx has more than one event. Make sure it's a staking provider SC Deploy transaction.")
 
 
 def add_new_nodes(args: Any):
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_add_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def remove_nodes(args: Any):
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_remove_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def stake_nodes(args: Any):
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_stake_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def unbond_nodes(args: Any):
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_unbond_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def unstake_nodes(args: Any):
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_unstake_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def unjail_nodes(args: Any):
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_unjail_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def change_service_fee(args: Any):
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_change_service_fee(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def modify_delegation_cap(args: Any):
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_modify_delegation_cap(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def automatic_activation(args: Any):
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_automatic_activation(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def redelegate_cap(args: Any):
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_redelegate_cap(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def set_metadata(args: Any):
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_set_metadata(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
```

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_deps.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_deps.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_dns.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_dns.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
     sub = cli_shared.add_command_subparser(subparsers, "dns", "register", "Send a register transaction to the appropriate DNS contract from given user and with given name")
     cli_shared.add_outfile_arg(sub)
     cli_shared.add_broadcast_args(sub, relay=True)
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_proxy_arg(sub)
     cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_guardian=True)
+    cli_shared.add_guardian_wallet_args(args, sub)
     sub.add_argument("--name", help="the name to register")
     sub.set_defaults(func=register)
 
     sub = cli_shared.add_command_subparser(subparsers, "dns", "resolve", "Find the address for a name")
     _add_name_arg(sub)
     cli_shared.add_proxy_arg(sub)
     sub.set_defaults(func=dns_resolve)
```

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_ledger.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_ledger.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_localnet.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_localnet.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_network.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_network.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_output.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_output.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_shared.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_shared.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from multiversx_sdk_network_providers.proxy_network_provider import \
     ProxyNetworkProvider
 
 from multiversx_sdk_cli import config, errors, utils
 from multiversx_sdk_cli.accounts import Account
 from multiversx_sdk_cli.cli_output import CLIOutputBuilder
-from multiversx_sdk_cli.cli_password import load_password
+from multiversx_sdk_cli.cli_password import load_password, load_guardian_password
 from multiversx_sdk_cli.ledger.ledger_functions import do_get_ledger_address
 from multiversx_sdk_cli.simulation import Simulator
 from multiversx_sdk_cli.transactions import Transaction
 from multiversx_sdk_cli.constants import TRANSACTION_OPTIONS_TX_GUARDED
 
 
 def wider_help_formatter(prog: Text):
@@ -75,32 +75,46 @@
     if with_data:
         sub.add_argument("--data", default="", help="the payload, or 'memo' of the transaction (default: %(default)s)")
 
     sub.add_argument("--chain", default=config.get_chain_id(), help="the chain identifier (default: %(default)s)")
     sub.add_argument("--version", type=int, default=config.get_tx_version(), help="the transaction version (default: %(default)s)")
 
     if with_guardian:
-        sub.add_argument("--guardian", type=str, help="the address of the guradian")
-        sub.add_argument("--guardian-service-url", type=str, help="the url of the guardian service")
-        sub.add_argument("--guardian-2fa-code", type=str, help="the 2fa code for the guardian")
+        add_guardian_args(sub)
 
     sub.add_argument("--options", type=int, default=0, help="the transaction options (default: 0)")
 
 
+def add_guardian_args(sub: Any):
+    sub.add_argument("--guardian", type=str, help="the address of the guradian")
+    sub.add_argument("--guardian-service-url", type=str, help="the url of the guardian service")
+    sub.add_argument("--guardian-2fa-code", type=str, help="the 2fa code for the guardian")
+
+
 def add_wallet_args(args: List[str], sub: Any):
     sub.add_argument("--pem", required=check_if_sign_method_required(args, "--pem"), help="🔑 the PEM file, if keyfile not provided")
     sub.add_argument("--pem-index", default=0, help="🔑 the index in the PEM file (default: %(default)s)")
     sub.add_argument("--keyfile", required=check_if_sign_method_required(args, "--keyfile"), help="🔑 a JSON keyfile, if PEM not provided")
     sub.add_argument("--passfile", help="🔑 a file containing keyfile's password, if keyfile provided")
     sub.add_argument("--ledger", action="store_true", required=check_if_sign_method_required(args, "--ledger"), default=False, help="🔐 bool flag for signing transaction using ledger")
     sub.add_argument("--ledger-account-index", type=int, default=0, help="🔐 the index of the account when using Ledger")
     sub.add_argument("--ledger-address-index", type=int, default=0, help="🔐 the index of the address when using Ledger")
     sub.add_argument("--sender-username", required=False, help="🖄 the username of the sender")
 
 
+def add_guardian_wallet_args(args: List[str], sub: Any):
+    sub.add_argument("--guardian-pem", required=check_if_sign_method_required(args, "--guardian-pem"), help="🔑 the PEM file, if keyfile not provided")
+    sub.add_argument("--guardian-pem-index", default=0, help="🔑 the index in the PEM file (default: %(default)s)")
+    sub.add_argument("--guardian-keyfile", required=check_if_sign_method_required(args, "--guardian-keyfile"), help="🔑 a JSON keyfile, if PEM not provided")
+    sub.add_argument("--guardian-passfile", help="🔑 a file containing keyfile's password, if keyfile provided")
+    sub.add_argument("--guardian-ledger", action="store_true", required=check_if_sign_method_required(args, "--guardian-ledger"), default=False, help="🔐 bool flag for signing transaction using ledger")
+    sub.add_argument("--guardian-ledger-account-index", type=int, default=0, help="🔐 the index of the account when using Ledger")
+    sub.add_argument("--guardian-ledger-address-index", type=int, default=0, help="🔐 the index of the address when using Ledger")
+
+
 def add_proxy_arg(sub: Any):
     sub.add_argument("--proxy", default=config.get_proxy(), help="🔗 the URL of the proxy (default: %(default)s)")
 
 
 def add_outfile_arg(sub: Any, what: str = ""):
     what = f"({what})" if what else ""
     sub.add_argument("--outfile", type=FileType("w"), default=sys.stdout, help=f"where to save the output {what} (default: stdout)")
@@ -117,27 +131,47 @@
 
 def parse_omit_fields_arg(args: Any) -> List[str]:
     literal = args.omit_fields
     parsed = ast.literal_eval(literal)
     return cast(List[str], parsed)
 
 
+def prepare_account(args: Any):
+    if args.pem:
+        account = Account(pem_file=args.pem, pem_index=args.pem_index)
+    elif args.keyfile:
+        password = load_password(args)
+        account = Account(key_file=args.keyfile, password=password)
+    elif args.ledger:
+        address = do_get_ledger_address(account_index=args.ledger_account_index, address_index=args.ledger_address_index)
+        account = Account(address=address)
+    else:
+        raise errors.NoWalletProvided()
+
+    return account
+
+
+def prepare_guardian_account(args: Any):
+    if args.guardian_pem:
+        account = Account(pem_file=args.guardian_pem, pem_index=args.guardian_pem_index)
+    elif args.guardian_keyfile:
+        password = load_guardian_password(args)
+        account = Account(key_file=args.guardian_keyfile, password=password)
+    elif args.guardian_ledger:
+        address = do_get_ledger_address(account_index=args.guardian_ledger_account_index, address_index=args.guardian_ledger_address_index)
+        account = Account(address=address)
+    else:
+        raise errors.NoWalletProvided()
+
+    return account
+
+
 def prepare_nonce_in_args(args: Any):
     if args.recall_nonce:
-        if args.pem:
-            account = Account(pem_file=args.pem, pem_index=args.pem_index)
-        elif args.keyfile:
-            password = load_password(args)
-            account = Account(key_file=args.keyfile, password=password)
-        elif args.ledger:
-            address = do_get_ledger_address(account_index=args.ledger_account_index, address_index=args.ledger_address_index)
-            account = Account(address=address)
-        else:
-            raise errors.NoWalletProvided()
-
+        account = prepare_account(args)
         account.sync_nonce(ProxyNetworkProvider(args.proxy))
         args.nonce = account.nonce
 
 
 def add_broadcast_args(sub: Any, simulate: bool = True, relay: bool = False):
     sub.add_argument("--send", action="store_true", default=False, help="✓ whether to broadcast the transaction (default: %(default)s)")
 
@@ -150,21 +184,40 @@
 def check_broadcast_args(args: Any):
     if hasattr(args, "relay") and args.relay and args.send:
         raise errors.BadUsage("Cannot directly send a relayed transaction. Use 'mxpy tx new --relay' first, then 'mxpy tx send --data-file'")
     if args.send and args.simulate:
         raise errors.BadUsage("Cannot both 'simulate' and 'send' a transaction")
 
 
+def check_guardian_and_options_args(args: Any):
+    check_guardian_args(args)
+    if args.guardian:
+        check_options_for_guarded_tx(args.options)
+
+
 def check_guardian_args(args: Any):
-    if any([args.guardian, args.guardian_service_url, args.guardian_2fa_code]):
-        if not all([args.guardian, args.guardian_service_url, args.guardian_2fa_code]):
-            raise errors.BadUsage("All guardian arguments must be provided")
+    if args.guardian:
+        if should_sign_with_cosigner_service(args) and should_sign_with_guardian_key(args):
+            raise errors.BadUsage("Guarded tx should be signed using either a cosigning service or a guardian key")
+
+        if not should_sign_with_cosigner_service(args) and not should_sign_with_guardian_key(args):
+            raise errors.BadUsage("Missing guardian signing arguments")
+
+
+def should_sign_with_cosigner_service(args: Any) -> bool:
+    return all([args.guardian_service_url, args.guardian_2fa_code])
+
+
+def should_sign_with_guardian_key(args: Any) -> bool:
+    return any([args.guardian_pem, args.guardian_keyfile, args.guardian_ledger])
+
 
-        if not args.options & TRANSACTION_OPTIONS_TX_GUARDED == TRANSACTION_OPTIONS_TX_GUARDED:
-            raise errors.BadUsage("For guarded transactions the guarded flag must be set.")
+def check_options_for_guarded_tx(options: int):
+    if not options & TRANSACTION_OPTIONS_TX_GUARDED == TRANSACTION_OPTIONS_TX_GUARDED:
+        raise errors.BadUsage("Invalid guarded transaction's options. The second least significant bit must be set.")
 
 
 def send_or_simulate(tx: Transaction, args: Any, dump_output: bool = True) -> CLIOutputBuilder:
     proxy = ProxyNetworkProvider(args.proxy)
 
     is_set_wait_result = hasattr(args, "wait_result") and args.wait_result
     is_set_send = hasattr(args, "send") and args.send
```

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_transactions.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_transactions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from pathlib import Path
 from typing import Any, List
 
 from multiversx_sdk_cli import cli_shared, utils
 from multiversx_sdk_cli.cli_output import CLIOutputBuilder
 from multiversx_sdk_network_providers.proxy_network_provider import ProxyNetworkProvider
+from multiversx_sdk_cli.errors import NoWalletProvided
 from multiversx_sdk_cli.transactions import Transaction, do_prepare_transaction
+from multiversx_sdk_cli.cosign_transaction import cosign_transaction
 
 
 def setup_parser(args: List[str], subparsers: Any) -> Any:
     parser = cli_shared.add_group_subparser(subparsers, "tx", "Create and broadcast Transactions")
     subparsers = parser.add_subparsers()
 
     sub = cli_shared.add_command_subparser(subparsers, "tx", "new", f"Create a new transaction.{CLIOutputBuilder.describe()}")
     _add_common_arguments(args, sub)
     cli_shared.add_outfile_arg(sub, what="signed transaction, hash")
     cli_shared.add_broadcast_args(sub, relay=True)
     cli_shared.add_proxy_arg(sub)
+    cli_shared.add_guardian_wallet_args(args, sub)
     sub.add_argument("--wait-result", action="store_true", default=False,
                      help="signal to wait for the transaction result - only valid if --send is set")
     sub.add_argument("--timeout", default=100, help="max num of seconds to wait for result"
                                                     " - only valid if --wait-result is set")
     sub.set_defaults(func=create_transaction)
 
     sub = cli_shared.add_command_subparser(subparsers, "tx", "send", f"Send a previously saved transaction.{CLIOutputBuilder.describe()}")
@@ -32,28 +35,38 @@
     sub.add_argument("--hash", required=True, help="the hash")
     sub.add_argument("--sender", required=False, help="the sender address")
     sub.add_argument("--with-results", action="store_true", help="will also return the results of transaction")
     cli_shared.add_proxy_arg(sub)
     cli_shared.add_omit_fields_arg(sub)
     sub.set_defaults(func=get_transaction)
 
+    sub = cli_shared.add_command_subparser(subparsers, "tx", "sign", f"Sign a previously saved transaction.{CLIOutputBuilder.describe()}")
+    cli_shared.add_wallet_args(args, sub)
+    cli_shared.add_infile_arg(sub, what="a previously saved transaction")
+    cli_shared.add_outfile_arg(sub, what="the signed transaction")
+    cli_shared.add_broadcast_args(sub, relay=True)
+    cli_shared.add_proxy_arg(sub)
+    cli_shared.add_guardian_args(sub)
+    cli_shared.add_guardian_wallet_args(args, sub)
+    sub.set_defaults(func=sign_transaction)
+
     parser.epilog = cli_shared.build_group_epilog(subparsers)
     return subparsers
 
 
 def _add_common_arguments(args: List[str], sub: Any):
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_tx_args(args, sub, with_guardian=True)
     sub.add_argument("--data-file", type=str, default=None, help="a file containing transaction data")
 
 
 def create_transaction(args: Any):
     args = utils.as_object(args)
 
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
 
     if args.data_file:
         args.data = Path(args.data_file).read_text()
 
     tx = do_prepare_transaction(args)
@@ -81,7 +94,39 @@
     args = utils.as_object(args)
     omit_fields = cli_shared.parse_omit_fields_arg(args)
     proxy = ProxyNetworkProvider(args.proxy)
 
     transaction = proxy.get_transaction(args.hash)
     output = CLIOutputBuilder().set_transaction_on_network(transaction, omit_fields).build()
     utils.dump_out_json(output)
+
+
+def sign_transaction(args: Any):
+    args = utils.as_object(args)
+
+    cli_shared.check_guardian_args(args)
+    cli_shared.check_broadcast_args(args)
+
+    tx = Transaction.load_from_file(args.infile)
+    if args.guardian:
+        cli_shared.check_options_for_guarded_tx(tx.options)
+
+    # clear existing signatures, if any
+    tx.guardianSignature = ""
+    tx.signature = ""
+
+    account = cli_shared.prepare_account(args)
+    signature = account.sign_transaction(tx)
+
+    try:
+        guardian_account = cli_shared.prepare_guardian_account(args)
+    except NoWalletProvided:
+        guardian_account = None
+
+    if guardian_account:
+        tx.guardianSignature = guardian_account.sign_transaction(tx)
+    elif args.guardian:
+        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
+
+    tx.signature = signature
+
+    cli_shared.send_or_simulate(tx, args)
```

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_validators.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
 def _add_common_arguments(args: List[str], sub: Any):
     cli_shared.add_proxy_arg(sub)
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_estimate_gas=True, with_guardian=True)
     cli_shared.add_broadcast_args(sub, relay=False)
     cli_shared.add_outfile_arg(sub, what="signed transaction, hash")
+    cli_shared.add_guardian_wallet_args(args, sub)
 
 
 def _add_nodes_arg(sub: Any):
     sub.add_argument("--nodes-public-keys", required=True, help="the public keys of the nodes as CSV (addrA,addrB)")
 
 
 def do_stake(args: Any):
```

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_wallet.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_wallet.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/config.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/contract_verification.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/contract_verification.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import hashlib
 import json
 import logging
 import time
 from pathlib import Path
-from typing import Any, Dict, Tuple
+from typing import Any, Dict, Tuple, Optional
 
 import requests
 
 from multiversx_sdk_cli.accounts import Account, Address
 from multiversx_sdk_cli.errors import KnownError
 from multiversx_sdk_cli.utils import dump_out_json, read_json_file
 
@@ -20,59 +20,64 @@
 class ContractVerificationRequest:
     def __init__(
         self,
         contract: Address,
         source_code: Dict[str, Any],
         signature: bytes,
         docker_image: str,
+        contract_variant: Optional[str]
     ) -> None:
         self.contract = contract
         self.source_code = source_code
         self.signature = signature
         self.docker_image = docker_image
+        self.contract_variant = contract_variant
 
     def to_dictionary(self) -> Dict[str, Any]:
         return {
             "signature": self.signature.hex(),
             "payload": {
                 "contract": self.contract.bech32(),
                 "dockerImage": self.docker_image,
-                "sourceCode": self.source_code
+                "sourceCode": self.source_code,
+                "contractVariant": self.contract_variant
             }
         }
 
 
 class ContractVerificationPayload:
-    def __init__(self, contract: Address, source_code: Dict[str, Any], docker_image: str,) -> None:
+    def __init__(self, contract: Address, source_code: Dict[str, Any], docker_image: str, contract_variant: Optional[str]) -> None:
         self.contract = contract
         self.source_code = source_code
         self.docker_image = docker_image
+        self.contract_variant = contract_variant
 
-    def serialize(self):
+    def serialize(self) -> str:
         payload = {
             "contract": self.contract.bech32(),
             "dockerImage": self.docker_image,
-            "sourceCode": self.source_code
+            "sourceCode": self.source_code,
+            "contractVariant": self.contract_variant
         }
 
         return json.dumps(payload, separators=(',', ':'))
 
 
 def trigger_contract_verification(
-    packaged_source: Path,
-    owner: Account,
-    contract: Address,
-    verifier_url: str,
-    docker_image: str,
-):
+        packaged_source: Path,
+        owner: Account,
+        contract: Address,
+        verifier_url: str,
+        docker_image: str,
+        contract_variant: Optional[str]):
     source_code = read_json_file(packaged_source)
 
-    payload = ContractVerificationPayload(contract, source_code, docker_image).serialize()
+    payload = ContractVerificationPayload(contract, source_code, docker_image, contract_variant).serialize()
     signature = _create_request_signature(owner, contract, payload.encode())
-    contract_verification = ContractVerificationRequest(contract, source_code, signature, docker_image)
+    contract_verification = ContractVerificationRequest(contract, source_code, signature, docker_image, contract_variant)
 
     request_dictionary = contract_verification.to_dictionary()
 
     url = f"{verifier_url}/verifier"
     status_code, message, data = _do_post(url, request_dictionary)
 
     if status_code == HTTP_REQUEST_TIMEOUT:
@@ -96,15 +101,15 @@
 
 
 def _create_request_signature(account: Account, contract_address: Address, request_payload: bytes) -> bytes:
     hashed_payload: str = hashlib.sha256(request_payload).hexdigest()
     raw_data_to_sign = f"{contract_address.bech32()}{hashed_payload}"
 
     signature_hex = account.sign_message(raw_data_to_sign.encode())
-    signature: bytes = bytes.fromhex(signature_hex)
+    signature = bytes.fromhex(signature_hex)
 
     return signature
 
 
 def query_status_with_task_id(url: str, task_id: str, interval: int = 10):
     logger.info(f"Please wait while we verify your contract. This may take a while.")
     old_status = ""
```

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/contracts.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/contracts.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class INetworkProvider(Protocol):
     def query_contract(self, query: Any) -> 'IContractQueryResponse':
         ...
 
 
 class QueryResult(Object):
-    def __init__(self, as_base64: str, as_hex: str, as_number: int):
+    def __init__(self, as_base64: str, as_hex: str, as_number: Optional[int]):
         self.base64 = as_base64
         self.hex = as_hex
         self.number = as_number
 
 
 class ContractQuery(IContractQuery):
     def __init__(self, address: Address, function: str, value: int, arguments: List[bytes], caller: Optional[Address] = None):
@@ -204,23 +204,37 @@
     def _interpret_return_data(self, data: str) -> Any:
         if not data:
             return data
 
         try:
             as_bytes = base64.b64decode(data)
             as_hex = as_bytes.hex()
-            as_number = int(as_hex, 16)
+            as_number = _interpret_as_number_if_safely(as_hex)
 
             result = QueryResult(data, as_hex, as_number)
             return result
         except Exception:
             logger.warn(f"Cannot interpret return data: {data}")
             return None
 
 
+def _interpret_as_number_if_safely(as_hex: str) -> Optional[int]:
+    """
+    Makes sure the string can be safely converted to an int (and then back to a string).
+
+    See:
+        - https://stackoverflow.com/questions/73693104/valueerror-exceeds-the-limit-4300-for-integer-string-conversion 
+        - https://github.com/python/cpython/issues/95778
+    """
+    try:
+        return int(str(int(as_hex or "0", 16)))
+    except:
+        return None
+
+
 def _prepare_argument(argument: Any):
     as_str = str(argument)
     as_hex = _to_hex(as_str)
     return as_hex
 
 
 def _to_hex(arg: str):
```

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cosign_transaction.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cosign_transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 from typing import Dict, Any, Protocol
 from multiversx_sdk_cli.errors import GuardianServiceError
 
 
 class ITransaction(Protocol):
-    guardian_signature: str
+    guardianSignature: str
 
     def to_dictionary(self) -> Dict[str, Any]:
         ...
 
 
 def cosign_transaction(transaction: ITransaction, service_url: str, guardian_code: str) -> ITransaction:
     payload = {
@@ -17,15 +17,15 @@
     }
 
     url = f"{service_url}/sign-transaction"
     response = requests.post(url, json=payload)
     check_for_guardian_error(response.json())
 
     tx_as_dict = response.json()["data"]["transaction"]
-    transaction.guardian_signature = tx_as_dict["guardianSignature"]
+    transaction.guardianSignature = tx_as_dict["guardianSignature"]
 
     return transaction
 
 
 def check_for_guardian_error(response: Dict[str, Any]):
     error = response["error"]
```

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/diskcache.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/diskcache.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dns.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     contract = SmartContract(dns_address)
     contract.query(proxy, "validateName", [name_arg])
 
 
 def register(args: Any):
     args = utils.as_object(args)
 
-    cli_shared.check_guardian_args(args)
+    cli_shared.check_guardian_and_options_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     args.receiver = dns_address_for_name(args.name).bech32()
     args.data = dns_register_data(args.name)
 
     tx = do_prepare_transaction(args)
```

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/docker.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/docker.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/downloader.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/downloader.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/errors.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/errors.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/guards.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/guards.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/interfaces.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/interfaces.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/myprocess.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/myprocess.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/simulation.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/simulation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/transactions.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/transactions.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 import logging
 import time
 from collections import OrderedDict
 from typing import Any, Dict, List, Protocol, Sequence, TextIO, Tuple
 
 from multiversx_sdk_cli import config, errors, utils
 from multiversx_sdk_cli.accounts import Account, Address, LedgerAccount
-from multiversx_sdk_cli.cli_password import load_password
+from multiversx_sdk_cli.cli_password import load_password, load_guardian_password
+from multiversx_sdk_cli.errors import NoWalletProvided
 from multiversx_sdk_cli.interfaces import ITransaction
 from multiversx_sdk_cli.cosign_transaction import cosign_transaction
+from multiversx_sdk_cli.ledger.ledger_functions import do_get_ledger_address
 
 logger = logging.getLogger("transactions")
 
 
 class ITransactionOnNetwork(Protocol):
     hash: str
     is_completed: bool
@@ -46,15 +48,15 @@
         self.gasLimit = 0
         self.data: str = ""
         self.chainID = ""
         self.version = 0
         self.options = 0
         self.signature = ""
         self.guardian = ""
-        self.guardian_signature = ""
+        self.guardianSignature = ""
 
     # The data field is base64-encoded. Here, we only support utf-8 "data" at this moment.
     def data_encoded(self) -> str:
         return self._field_encoded("data")
 
     # Useful when loading a tx from a file (when data is already encoded in base64)
     def data_decoded(self) -> str:
@@ -176,22 +178,22 @@
 
         if self.version:
             dictionary["version"] = int(self.version)
 
         if self.options:
             dictionary["options"] = int(self.options)
 
-        if self.signature:
-            dictionary["signature"] = self.signature
-
         if self.guardian:
             dictionary["guardian"] = self.guardian
 
-        if self.guardian_signature:
-            dictionary["guardianSignature"] = self.guardian_signature
+        if self.signature:
+            dictionary["signature"] = self.signature
+
+        if self.guardianSignature:
+            dictionary["guardianSignature"] = self.guardianSignature
 
         return dictionary
 
     # Creates the payload for a "user" / "inner" transaction
     def to_dictionary_as_inner(self) -> Dict[str, Any]:
         dictionary = self.to_dictionary()
         dictionary["receiver"] = base64.b64encode(Address(self.receiver).pubkey()).decode()
@@ -275,12 +277,46 @@
     tx.data = args.data
     tx.chainID = args.chain
     tx.version = int(args.version)
     tx.options = int(args.options)
     tx.guardian = args.guardian
 
     tx.sign(account)
+    tx = sign_tx_by_guardian(args, tx)
 
-    if args.guardian:
-        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
+    return tx
+
+
+def sign_tx_by_guardian(args: Any, tx: Transaction) -> Transaction:
+    try:
+        guardian_account = get_guardian_account_from_args(args)
+    except NoWalletProvided:
+        guardian_account = None
+
+    # empty sender signature
+    sender_signature = tx.signature
+    tx.signature = ""
+
+    if guardian_account:
+        tx.guardianSignature = guardian_account.sign_transaction(tx)
+    elif args.guardian:
+        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)  # type: ignore
+
+    tx.signature = sender_signature
 
     return tx
+
+
+# TODO: this is duplicated code; a proper refactoring will come later
+def get_guardian_account_from_args(args: Any):
+    if args.guardian_pem:
+        account = Account(pem_file=args.guardian_pem, pem_index=args.guardian_pem_index)
+    elif args.guardian_keyfile:
+        password = load_guardian_password(args)
+        account = Account(key_file=args.guardian_keyfile, password=password)
+    elif args.guardian_ledger:
+        address = do_get_ledger_address(account_index=args.guardian_ledger_account_index, address_index=args.guardian_ledger_address_index)
+        account = Account(address=address)
+    else:
+        raise errors.NoWalletProvided()
+
+    return account
```

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/utils.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/utils.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/version.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/version.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/workstation.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/workstation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/delegation/__init__.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/delegation/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/delegation/staking_provider.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/delegation/staking_provider.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dependencies/install.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dependencies/install.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dependencies/modules.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dependencies/modules.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/config.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/ledger_app_handler.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/ledger_app_handler.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/ledger_functions.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/ledger_functions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_default.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_default.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_general.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_general.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_networking.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_networking.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_part.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_part.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_root.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_root.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_sharding.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_sharding.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_software.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_software.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/genesis.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/genesis.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/genesis_json.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/genesis_json.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/libraries.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/libraries.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/node.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/node.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/node_config_toml.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/node_config_toml.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/nodes_setup_json.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/nodes_setup_json.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/p2p_toml.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/p2p_toml.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_build_software.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_build_software.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_config.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_prerequisites.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_prerequisites.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_start.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_start.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/wallets.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/wallets.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/__init__.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/core.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/migrations.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/migrations.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_base.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_base.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_clang.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_clang.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_cpp.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_cpp.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_rust.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_rust.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/shared.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/shared.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/templates.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/templates.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/templates_config.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/templates_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/templates_repository.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/templates_repository.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/do_report.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/do_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/report_creator.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/report_creator.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/common.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/common.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/extracted_feature.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/extracted_feature.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/folder_report.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/folder_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/project_report.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/project_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/report.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/wasm_report.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/wasm_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/report_option.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/report_option.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/format/change_type.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/format/change_type.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/validators/__init__.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/validators/core.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/validators/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/validators/validators_file.py` & `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/validators/validators_file.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/LICENSE` & `multiversx_sdk_cli-7.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/README.md` & `multiversx_sdk_cli-7.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b0/pyproject.toml` & `multiversx_sdk_cli-7.0.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "multiversx-sdk-cli"
-version = "7.0.0b0"
+version = "7.0.0b1"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "MultiversX Smart Contracts Tools"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -23,15 +23,15 @@
   "requests",
   "prettytable",
   "ledgercomm[hid]",
   "semver",
   "requests-cache",
   "rich==13.3.4",
   "multiversx-sdk-network-providers==0.6.*",
-  "multiversx-sdk-wallet==0.6.*",
+  "multiversx-sdk-wallet==0.7.*",
   "multiversx-sdk-core>=0.4.1"
 ]
 
 [tool.hatch.build]
 include = [
   "multiversx_sdk_cli/**"
 ]
```

### Comparing `multiversx_sdk_cli-7.0.0b0/PKG-INFO` & `multiversx_sdk_cli-7.0.0b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: multiversx-sdk-cli
-Version: 7.0.0b0
+Version: 7.0.0b1
 Summary: MultiversX Smart Contracts Tools
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-cli
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: ledgercomm[hid]
 Requires-Dist: multiversx-sdk-core>=0.4.1
 Requires-Dist: multiversx-sdk-network-providers==0.6.*
-Requires-Dist: multiversx-sdk-wallet==0.6.*
+Requires-Dist: multiversx-sdk-wallet==0.7.*
 Requires-Dist: prettytable
 Requires-Dist: requests
 Requires-Dist: requests-cache
 Requires-Dist: rich==13.3.4
 Requires-Dist: semver
 Requires-Dist: toml>=0.10.2
 Description-Content-Type: text/markdown
```

