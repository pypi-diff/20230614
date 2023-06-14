# Comparing `tmp/servicefoundry-0.9.6rc2.tar.gz` & `tmp/servicefoundry-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicefoundry-0.9.6rc2.tar", max compression
+gzip compressed data, was "servicefoundry-0.9.7.tar", max compression
```

## Comparing `servicefoundry-0.9.6rc2.tar` & `servicefoundry-0.9.7.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0      672 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/README.md
--rw-r--r--   0        0        0     2119 2023-06-12 05:29:35.283041 servicefoundry-0.9.6rc2/pyproject.toml
--rw-r--r--   0        0        0     1365 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/__init__.py
--rw-r--r--   0        0        0    40084 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/auto_gen/models.py
--rw-r--r--   0        0        0     4294 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/builder/__init__.py
--rw-r--r--   0        0        0      632 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/builder/builders/__init__.py
--rw-r--r--   0        0        0     1506 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/builder/builders/dockerfile.py
--rw-r--r--   0        0        0     1317 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py
--rw-r--r--   0        0        0     1369 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     1357 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
--rw-r--r--   0        0        0     6496 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     7019 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/builder/docker_service.py
--rw-r--r--   0        0        0       66 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/__init__.py
--rw-r--r--   0        0        0      494 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/__main__.py
--rw-r--r--   0        0        0     3089 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/cli_main.py
--rw-r--r--   0        0        0      958 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1232 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/build_command.py
--rw-r--r--   0        0        0     2788 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/build_logs_command.py
--rw-r--r--   0        0        0     1834 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/create_command.py
--rw-r--r--   0        0        0     2358 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/delete_command.py
--rw-r--r--   0        0        0     1227 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/deploy_v2_command.py
--rw-r--r--   0        0        0     3536 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/get_command.py
--rw-r--r--   0        0        0     2944 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/infra_bootstrap.py
--rw-r--r--   0        0        0     4462 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/list_command.py
--rw-r--r--   0        0        0      938 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/login_command.py
--rw-r--r--   0        0        0      534 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/logout_command.py
--rw-r--r--   0        0        0     4134 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/logs_command.py
--rw-r--r--   0        0        0     1670 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/patch_command.py
--rw-r--r--   0        0        0     1020 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/redeploy_command.py
--rw-r--r--   0        0        0     2752 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/commands/trigger_command.py
--rw-r--r--   0        0        0      206 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/config.py
--rw-r--r--   0        0        0      242 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/console.py
--rw-r--r--   0        0        0      510 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/const.py
--rw-r--r--   0        0        0     2970 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/display_util.py
--rw-r--r--   0        0        0     2500 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/cli/util.py
--rw-r--r--   0        0        0      132 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/core/__init__.py
--rw-r--r--   0        0        0      232 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/core/login.py
--rw-r--r--   0        0        0       76 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/core/logout.py
--rw-r--r--   0        0        0      188 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/__init__.py
--rw-r--r--   0        0        0      775 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/__main__.py
--rw-r--r--   0        0        0     2857 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/app.py
--rw-r--r--   0        0        0     1844 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/build.py
--rw-r--r--   0        0        0        0 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
--rw-r--r--   0        0        0      673 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
--rw-r--r--   0        0        0      185 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
--rw-r--r--   0        0        0      600 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
--rw-r--r--   0        0        0      297 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
--rw-r--r--   0        0        0     1772 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
--rw-r--r--   0        0        0      369 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/model_composition/model.py
--rw-r--r--   0        0        0     1513 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
--rw-r--r--   0        0        0      153 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/model_composition/utils.py
--rw-r--r--   0        0        0        0 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
--rw-r--r--   0        0        0      406 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
--rw-r--r--   0        0        0      518 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
--rw-r--r--   0        0        0      191 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/remote/__init__.py
--rw-r--r--   0        0        0       67 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/remote/context.py
--rw-r--r--   0        0        0     1875 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/remote/method.py
--rw-r--r--   0        0        0     4210 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/remote/remote.py
--rw-r--r--   0        0        0     4494 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/route.py
--rw-r--r--   0        0        0     4139 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/service.py
--rw-r--r--   0        0        0     1231 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/function_service/utils.py
--rw-r--r--   0        0        0        0 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/internal/__init__.py
--rw-r--r--   0        0        0      960 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/internal/experimental.py
--rw-r--r--   0        0        0        0 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/io/__init__.py
--rw-r--r--   0        0        0      604 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/io/output_callback.py
--rw-r--r--   0        0        0      825 2023-06-12 05:29:21.246771 servicefoundry-0.9.6rc2/servicefoundry/io/rich_output_callback.py
--rw-r--r--   0        0        0      175 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/json_util.py
--rw-r--r--   0        0        0        0 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/__init__.py
--rw-r--r--   0        0        0     2906 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/auth/auth_service_client.py
--rw-r--r--   0        0        0     4228 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/auth/credential_file_manager.py
--rw-r--r--   0        0        0     4268 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/auth/credential_provider.py
--rw-r--r--   0        0        0     1854 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/auth/servicefoundry_session.py
--rw-r--r--   0        0        0     7447 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/binarydownloader.py
--rw-r--r--   0        0        0        0 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/clients/__init__.py
--rw-r--r--   0        0        0      671 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/clients/cookiecutter_client.py
--rw-r--r--   0        0        0     2563 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/clients/git_client.py
--rw-r--r--   0        0        0    25229 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/clients/service_foundry_client.py
--rw-r--r--   0        0        0      455 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/clients/shell_client.py
--rw-r--r--   0        0        0     1455 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/clients/terragrunt_client.py
--rw-r--r--   0        0        0     1122 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/clients/utils.py
--rw-r--r--   0        0        0     1331 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/config/config_manager.py
--rw-r--r--   0        0        0     2237 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/config/dict_questionaire.py
--rw-r--r--   0        0        0    10594 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/config/infra_config.py
--rw-r--r--   0        0        0     1886 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/config/installation_config.py
--rw-r--r--   0        0        0     1752 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/const.py
--rw-r--r--   0        0        0        0 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/dao/__init__.py
--rw-r--r--   0        0        0     6485 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/dao/application.py
--rw-r--r--   0        0        0     1123 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/dao/version.py
--rw-r--r--   0        0        0     2344 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/dao/workspace.py
--rw-r--r--   0        0        0      588 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/exceptions.py
--rw-r--r--   0        0        0      288 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/infra/argo-secrets.mustache
--rw-r--r--   0        0        0      918 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/infra/argo-ubermold.mustache
--rw-r--r--   0        0        0    23708 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/infra/install_truefoundry.py
--rw-r--r--   0        0        0     1411 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/infra/nats-bootstrap.sh
--rw-r--r--   0        0        0      328 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/infra/tfy-agent.mustache
--rw-r--r--   0        0        0     1137 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/infra/tfy-control-plane.mustache
--rw-r--r--   0        0        0     6290 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/infra/utils.py
--rw-r--r--   0        0        0     1463 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/logs_utils.py
--rw-r--r--   0        0        0      861 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/messages.py
--rw-r--r--   0        0        0        0 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/model/__init__.py
--rw-r--r--   0        0        0    10866 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/model/entity.py
--rw-r--r--   0        0        0     5208 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/session.py
--rw-r--r--   0        0        0     1664 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/util.py
--rw-r--r--   0        0        0     4995 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/lib/win32.py
--rw-r--r--   0        0        0      688 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/logger.py
--rw-r--r--   0        0        0        0 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/__init__.py
--rw-r--r--   0        0        0      517 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/examples/job_deployment/deploy.py
--rw-r--r--   0        0        0      305 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/examples/job_deployment/main.py
--rw-r--r--   0        0        0      303 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      441 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
--rw-r--r--   0        0        0      524 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
--rw-r--r--   0        0        0      639 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/examples/model_deployment/hf/deploy.py
--rw-r--r--   0        0        0      190 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
--rw-r--r--   0        0        0      579 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
--rw-r--r--   0        0        0      313 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
--rw-r--r--   0        0        0      764 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/examples/service_deployment/deploy.py
--rw-r--r--   0        0        0      117 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/examples/service_deployment/main.py
--rw-r--r--   0        0        0      482 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      188 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/lib/__init__.py
--rw-r--r--   0        0        0    10072 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/lib/deploy.py
--rw-r--r--   0        0        0     1876 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/lib/deployable_patched_models.py
--rw-r--r--   0        0        0     1105 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/lib/models.py
--rw-r--r--   0        0        0     5921 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/lib/patched_models.py
--rw-r--r--   0        0        0     8988 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/v2/lib/source.py
--rw-r--r--   0        0        0      130 2023-06-12 05:29:21.250771 servicefoundry-0.9.6rc2/servicefoundry/version.py
--rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 servicefoundry-0.9.6rc2/PKG-INFO
+-rw-r--r--   0        0        0      672 2023-06-14 09:58:52.197705 servicefoundry-0.9.7/README.md
+-rw-r--r--   0        0        0     2116 2023-06-14 09:59:06.666795 servicefoundry-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     1365 2023-06-14 09:58:52.197705 servicefoundry-0.9.7/servicefoundry/__init__.py
+-rw-r--r--   0        0        0    40084 2023-06-14 09:58:52.197705 servicefoundry-0.9.7/servicefoundry/auto_gen/models.py
+-rw-r--r--   0        0        0     4294 2023-06-14 09:58:52.197705 servicefoundry-0.9.7/servicefoundry/builder/__init__.py
+-rw-r--r--   0        0        0      632 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/builders/__init__.py
+-rw-r--r--   0        0        0     1506 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/builders/dockerfile.py
+-rw-r--r--   0        0        0     1317 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py
+-rw-r--r--   0        0        0     1369 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     1357 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
+-rw-r--r--   0        0        0     6496 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     7019 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/docker_service.py
+-rw-r--r--   0        0        0       66 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/__main__.py
+-rw-r--r--   0        0        0     3089 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/cli_main.py
+-rw-r--r--   0        0        0      958 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1232 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/build_command.py
+-rw-r--r--   0        0        0     2788 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/build_logs_command.py
+-rw-r--r--   0        0        0     1834 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/create_command.py
+-rw-r--r--   0        0        0     2358 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/delete_command.py
+-rw-r--r--   0        0        0     1227 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/deploy_v2_command.py
+-rw-r--r--   0        0        0     3536 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/get_command.py
+-rw-r--r--   0        0        0     2944 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/infra_bootstrap.py
+-rw-r--r--   0        0        0     4462 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/list_command.py
+-rw-r--r--   0        0        0      938 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/login_command.py
+-rw-r--r--   0        0        0      534 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/logout_command.py
+-rw-r--r--   0        0        0     4134 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/logs_command.py
+-rw-r--r--   0        0        0     1670 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/patch_command.py
+-rw-r--r--   0        0        0     1020 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/redeploy_command.py
+-rw-r--r--   0        0        0     2752 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/trigger_command.py
+-rw-r--r--   0        0        0      206 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/config.py
+-rw-r--r--   0        0        0      242 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/console.py
+-rw-r--r--   0        0        0      510 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/const.py
+-rw-r--r--   0        0        0     2970 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/display_util.py
+-rw-r--r--   0        0        0     2500 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/util.py
+-rw-r--r--   0        0        0      132 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/core/__init__.py
+-rw-r--r--   0        0        0      232 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/core/login.py
+-rw-r--r--   0        0        0       76 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/core/logout.py
+-rw-r--r--   0        0        0      188 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/__init__.py
+-rw-r--r--   0        0        0      775 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/__main__.py
+-rw-r--r--   0        0        0     2857 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/app.py
+-rw-r--r--   0        0        0     1844 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/build.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
+-rw-r--r--   0        0        0      673 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
+-rw-r--r--   0        0        0      185 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
+-rw-r--r--   0        0        0      600 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
+-rw-r--r--   0        0        0      297 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
+-rw-r--r--   0        0        0     1772 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
+-rw-r--r--   0        0        0      369 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/model.py
+-rw-r--r--   0        0        0     1513 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
+-rw-r--r--   0        0        0      153 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/utils.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
+-rw-r--r--   0        0        0      406 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
+-rw-r--r--   0        0        0      518 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
+-rw-r--r--   0        0        0      191 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/remote/__init__.py
+-rw-r--r--   0        0        0       67 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/remote/context.py
+-rw-r--r--   0        0        0     1875 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/remote/method.py
+-rw-r--r--   0        0        0     4210 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/remote/remote.py
+-rw-r--r--   0        0        0     4494 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/route.py
+-rw-r--r--   0        0        0     4139 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/service.py
+-rw-r--r--   0        0        0     1231 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/utils.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/internal/__init__.py
+-rw-r--r--   0        0        0      960 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/internal/experimental.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/io/__init__.py
+-rw-r--r--   0        0        0      604 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/io/output_callback.py
+-rw-r--r--   0        0        0      825 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/io/rich_output_callback.py
+-rw-r--r--   0        0        0      175 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/json_util.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/__init__.py
+-rw-r--r--   0        0        0     2906 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/auth/auth_service_client.py
+-rw-r--r--   0        0        0     4228 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/auth/credential_file_manager.py
+-rw-r--r--   0        0        0     4268 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/auth/credential_provider.py
+-rw-r--r--   0        0        0     1854 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/auth/servicefoundry_session.py
+-rw-r--r--   0        0        0     7447 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/binarydownloader.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/__init__.py
+-rw-r--r--   0        0        0      671 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/cookiecutter_client.py
+-rw-r--r--   0        0        0     2563 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/git_client.py
+-rw-r--r--   0        0        0    25229 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/service_foundry_client.py
+-rw-r--r--   0        0        0      455 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/shell_client.py
+-rw-r--r--   0        0        0     1455 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/terragrunt_client.py
+-rw-r--r--   0        0        0     1122 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/utils.py
+-rw-r--r--   0        0        0     1331 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/config/config_manager.py
+-rw-r--r--   0        0        0     2237 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/config/dict_questionaire.py
+-rw-r--r--   0        0        0    10594 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/config/infra_config.py
+-rw-r--r--   0        0        0     1886 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/config/installation_config.py
+-rw-r--r--   0        0        0     1752 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/const.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/dao/__init__.py
+-rw-r--r--   0        0        0     6485 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/dao/application.py
+-rw-r--r--   0        0        0     1123 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/dao/version.py
+-rw-r--r--   0        0        0     2344 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/dao/workspace.py
+-rw-r--r--   0        0        0      588 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/exceptions.py
+-rw-r--r--   0        0        0      288 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/infra/argo-secrets.mustache
+-rw-r--r--   0        0        0      918 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/infra/argo-ubermold.mustache
+-rw-r--r--   0        0        0    23708 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/infra/install_truefoundry.py
+-rw-r--r--   0        0        0     1411 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/infra/nats-bootstrap.sh
+-rw-r--r--   0        0        0      328 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/infra/tfy-agent.mustache
+-rw-r--r--   0        0        0     1137 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/infra/tfy-control-plane.mustache
+-rw-r--r--   0        0        0     6290 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/infra/utils.py
+-rw-r--r--   0        0        0     1463 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/logs_utils.py
+-rw-r--r--   0        0        0      861 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/messages.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/model/__init__.py
+-rw-r--r--   0        0        0    10866 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/model/entity.py
+-rw-r--r--   0        0        0     5208 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/session.py
+-rw-r--r--   0        0        0     1664 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/util.py
+-rw-r--r--   0        0        0     4995 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/win32.py
+-rw-r--r--   0        0        0      688 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/logger.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/__init__.py
+-rw-r--r--   0        0        0      517 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/deploy.py
+-rw-r--r--   0        0        0      305 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/main.py
+-rw-r--r--   0        0        0      303 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      441 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
+-rw-r--r--   0        0        0      524 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
+-rw-r--r--   0        0        0      639 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/model_deployment/hf/deploy.py
+-rw-r--r--   0        0        0      190 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
+-rw-r--r--   0        0        0      579 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
+-rw-r--r--   0        0        0      313 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
+-rw-r--r--   0        0        0      764 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/service_deployment/deploy.py
+-rw-r--r--   0        0        0      117 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/service_deployment/main.py
+-rw-r--r--   0        0        0      482 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      188 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/lib/__init__.py
+-rw-r--r--   0        0        0    10072 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/lib/deploy.py
+-rw-r--r--   0        0        0     1876 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/lib/deployable_patched_models.py
+-rw-r--r--   0        0        0     1105 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/lib/models.py
+-rw-r--r--   0        0        0     5921 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/lib/patched_models.py
+-rw-r--r--   0        0        0     8988 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/lib/source.py
+-rw-r--r--   0        0        0      130 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/version.py
+-rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 servicefoundry-0.9.7/PKG-INFO
```

### Comparing `servicefoundry-0.9.6rc2/README.md` & `servicefoundry-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/pyproject.toml` & `servicefoundry-0.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicefoundry"
-version = "0.9.6rc2"  # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.9.7"  # do not change, auto-generated by poetry-dynamic-versioning
 description = "Generate deployed services from code"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/innoavator/servicefoundry"
 repository = "https://github.com/innoavator/servicefoundry"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/__init__.py` & `servicefoundry-0.9.7/servicefoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/auto_gen/models.py` & `servicefoundry-0.9.7/servicefoundry/auto_gen/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/builder/__init__.py` & `servicefoundry-0.9.7/servicefoundry/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/builder/builders/__init__.py` & `servicefoundry-0.9.7/servicefoundry/builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/builder/builders/dockerfile.py` & `servicefoundry-0.9.7/servicefoundry/builder/builders/dockerfile.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py` & `servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py` & `servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py` & `servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py` & `servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/builder/docker_service.py` & `servicefoundry-0.9.7/servicefoundry/builder/docker_service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/cli_main.py` & `servicefoundry-0.9.7/servicefoundry/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/__init__.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/build_command.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/build_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/build_logs_command.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/build_logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/create_command.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/create_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/delete_command.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/delete_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/deploy_v2_command.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/deploy_v2_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/get_command.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/get_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/infra_bootstrap.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/infra_bootstrap.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/list_command.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/list_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/login_command.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/login_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/logout_command.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/logout_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/logs_command.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/patch_command.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/patch_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/redeploy_command.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/redeploy_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/commands/trigger_command.py` & `servicefoundry-0.9.7/servicefoundry/cli/commands/trigger_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/display_util.py` & `servicefoundry-0.9.7/servicefoundry/cli/display_util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/cli/util.py` & `servicefoundry-0.9.7/servicefoundry/cli/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/function_service/__main__.py` & `servicefoundry-0.9.7/servicefoundry/function_service/__main__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/function_service/app.py` & `servicefoundry-0.9.7/servicefoundry/function_service/app.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/function_service/build.py` & `servicefoundry-0.9.7/servicefoundry/function_service/build.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py` & `servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py` & `servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/model_composition/deployment.py` & `servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py` & `servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py` & `servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/function_service/remote/method.py` & `servicefoundry-0.9.7/servicefoundry/function_service/remote/method.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/function_service/remote/remote.py` & `servicefoundry-0.9.7/servicefoundry/function_service/remote/remote.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/function_service/route.py` & `servicefoundry-0.9.7/servicefoundry/function_service/route.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/function_service/service.py` & `servicefoundry-0.9.7/servicefoundry/function_service/service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/function_service/utils.py` & `servicefoundry-0.9.7/servicefoundry/function_service/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/internal/experimental.py` & `servicefoundry-0.9.7/servicefoundry/internal/experimental.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/io/output_callback.py` & `servicefoundry-0.9.7/servicefoundry/io/output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/io/rich_output_callback.py` & `servicefoundry-0.9.7/servicefoundry/io/rich_output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/auth/auth_service_client.py` & `servicefoundry-0.9.7/servicefoundry/lib/auth/auth_service_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/auth/credential_file_manager.py` & `servicefoundry-0.9.7/servicefoundry/lib/auth/credential_file_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/auth/credential_provider.py` & `servicefoundry-0.9.7/servicefoundry/lib/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/auth/servicefoundry_session.py` & `servicefoundry-0.9.7/servicefoundry/lib/auth/servicefoundry_session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/binarydownloader.py` & `servicefoundry-0.9.7/servicefoundry/lib/binarydownloader.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/clients/cookiecutter_client.py` & `servicefoundry-0.9.7/servicefoundry/lib/clients/cookiecutter_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/clients/git_client.py` & `servicefoundry-0.9.7/servicefoundry/lib/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/clients/service_foundry_client.py` & `servicefoundry-0.9.7/servicefoundry/lib/clients/service_foundry_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/clients/terragrunt_client.py` & `servicefoundry-0.9.7/servicefoundry/lib/clients/terragrunt_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/clients/utils.py` & `servicefoundry-0.9.7/servicefoundry/lib/clients/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/config/config_manager.py` & `servicefoundry-0.9.7/servicefoundry/lib/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/config/dict_questionaire.py` & `servicefoundry-0.9.7/servicefoundry/lib/config/dict_questionaire.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/config/infra_config.py` & `servicefoundry-0.9.7/servicefoundry/lib/config/infra_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/config/installation_config.py` & `servicefoundry-0.9.7/servicefoundry/lib/config/installation_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/const.py` & `servicefoundry-0.9.7/servicefoundry/lib/const.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/dao/application.py` & `servicefoundry-0.9.7/servicefoundry/lib/dao/application.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/dao/version.py` & `servicefoundry-0.9.7/servicefoundry/lib/dao/version.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/dao/workspace.py` & `servicefoundry-0.9.7/servicefoundry/lib/dao/workspace.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/exceptions.py` & `servicefoundry-0.9.7/servicefoundry/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/infra/argo-ubermold.mustache` & `servicefoundry-0.9.7/servicefoundry/lib/infra/argo-ubermold.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/infra/install_truefoundry.py` & `servicefoundry-0.9.7/servicefoundry/lib/infra/install_truefoundry.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/infra/nats-bootstrap.sh` & `servicefoundry-0.9.7/servicefoundry/lib/infra/nats-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/infra/tfy-control-plane.mustache` & `servicefoundry-0.9.7/servicefoundry/lib/infra/tfy-control-plane.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/infra/utils.py` & `servicefoundry-0.9.7/servicefoundry/lib/infra/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/logs_utils.py` & `servicefoundry-0.9.7/servicefoundry/lib/logs_utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/messages.py` & `servicefoundry-0.9.7/servicefoundry/lib/messages.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/model/entity.py` & `servicefoundry-0.9.7/servicefoundry/lib/model/entity.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/session.py` & `servicefoundry-0.9.7/servicefoundry/lib/session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/util.py` & `servicefoundry-0.9.7/servicefoundry/lib/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/lib/win32.py` & `servicefoundry-0.9.7/servicefoundry/lib/win32.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/logger.py` & `servicefoundry-0.9.7/servicefoundry/logger.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/v2/examples/job_deployment/deploy.py` & `servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml` & `servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/v2/examples/model_deployment/hf/deploy.py` & `servicefoundry-0.9.7/servicefoundry/v2/examples/model_deployment/hf/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py` & `servicefoundry-0.9.7/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/v2/examples/service_deployment/deploy.py` & `servicefoundry-0.9.7/servicefoundry/v2/examples/service_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/v2/lib/deploy.py` & `servicefoundry-0.9.7/servicefoundry/v2/lib/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/v2/lib/deployable_patched_models.py` & `servicefoundry-0.9.7/servicefoundry/v2/lib/deployable_patched_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from servicefoundry.v2.lib.deploy import deploy_component
 
 
 class Service(models.Service):
     type: constr(regex=r"service") = "service"
     resources: models.Resources = Field(default_factory=models.Resources)
     # This is being patched because cue export marks this as a "number"
-    replicas: Union[conint(ge=1, le=20), models.Autoscaling] = Field(
+    replicas: Union[conint(ge=0, le=20), models.Autoscaling] = Field(
         1,
         description="+label=Replicas\n+usage=Replicas of service you want to run\n+icon=fa-clone\n+sort=3",
     )
 
     class Config:
         extra = "forbid"
```

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/v2/lib/models.py` & `servicefoundry-0.9.7/servicefoundry/v2/lib/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/v2/lib/patched_models.py` & `servicefoundry-0.9.7/servicefoundry/v2/lib/patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/servicefoundry/v2/lib/source.py` & `servicefoundry-0.9.7/servicefoundry/v2/lib/source.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.6rc2/PKG-INFO` & `servicefoundry-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicefoundry
-Version: 0.9.6rc2
+Version: 0.9.7
 Summary: Generate deployed services from code
 Home-page: https://github.com/innoavator/servicefoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

