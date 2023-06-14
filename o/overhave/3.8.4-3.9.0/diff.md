# Comparing `tmp/overhave-3.8.4.tar.gz` & `tmp/overhave-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overhave-3.8.4.tar", max compression
+gzip compressed data, was "overhave-3.9.0.tar", max compression
```

## Comparing `overhave-3.8.4.tar` & `overhave-3.9.0.tar`

### file list

```diff
@@ -1,235 +1,236 @@
--rw-r--r--   0        0        0    23315 2022-08-22 07:42:20.286683 overhave-3.8.4/README.rst
--rw-r--r--   0        0        0     3075 2022-08-22 07:42:20.302683 overhave-3.8.4/overhave/__init__.py
--rw-r--r--   0        0        0       63 2022-08-22 07:42:20.302683 overhave-3.8.4/overhave/admin/__init__.py
--rw-r--r--   0        0        0     5109 2022-08-22 07:42:20.302683 overhave-3.8.4/overhave/admin/app.py
--rw-r--r--   0        0        0   735118 2022-08-22 07:42:20.302683 overhave-3.8.4/overhave/admin/files/ace-src/ace.js
--rw-r--r--   0        0        0     5426 2022-08-22 07:42:20.302683 overhave-3.8.4/overhave/admin/files/ace-src/mode-gherkin.js
--rw-r--r--   0        0        0     1263 2022-08-22 07:42:20.302683 overhave-3.8.4/overhave/admin/files/css/overhave.css
--rw-r--r--   0        0        0    38062 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/files/favicon.ico
--rw-r--r--   0        0        0      138 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/flask/__init__.py
--rw-r--r--   0        0        0     1819 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/flask/flask_admin.py
--rw-r--r--   0        0        0      459 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/flask/flask_app.py
--rw-r--r--   0        0        0      946 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/flask/login_manager.py
--rw-r--r--   0        0        0      187 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/draft_detail.html
--rw-r--r--   0        0        0      405 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/emulation.html
--rw-r--r--   0        0        0      194 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/emulation_create.html
--rw-r--r--   0        0        0      190 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/emulation_edit.html
--rw-r--r--   0        0        0      860 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/emulation_run_detail.html
--rw-r--r--   0        0        0    10445 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/feature.html
--rw-r--r--   0        0        0      404 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/feature_create.html
--rw-r--r--   0        0        0      400 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/feature_edit.html
--rw-r--r--   0        0        0      177 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/index.html
--rw-r--r--   0        0        0     2414 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/login.html
--rw-r--r--   0        0        0      149 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/overhave_master.html
--rw-r--r--   0        0        0     1696 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/test_run.html
--rw-r--r--   0        0        0     1469 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/test_run_detail.html
--rw-r--r--   0        0        0      189 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/test_run_list.html
--rw-r--r--   0        0        0      606 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/test_user.html
--rw-r--r--   0        0        0      210 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/test_user_create.html
--rw-r--r--   0        0        0      208 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/templates/test_user_edit.html
--rw-r--r--   0        0        0      451 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/__init__.py
--rw-r--r--   0        0        0     1382 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/access.py
--rw-r--r--   0        0        0     2914 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/base.py
--rw-r--r--   0        0        0     1105 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/draft.py
--rw-r--r--   0        0        0     3441 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/emulation.py
--rw-r--r--   0        0        0     1620 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/emulation_run.py
--rw-r--r--   0        0        0     9557 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/feature.py
--rw-r--r--   0        0        0      306 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/formatters/__init__.py
--rw-r--r--   0        0        0     5169 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/formatters/formatters.py
--rw-r--r--   0        0        0      669 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/formatters/helpers.py
--rw-r--r--   0        0        0     1429 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/formatters/safe_formatter.py
--rw-r--r--   0        0        0       51 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/index/__init__.py
--rw-r--r--   0        0        0     1680 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/index/custom_page.py
--rw-r--r--   0        0        0     1536 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/index/login_form.py
--rw-r--r--   0        0        0     2658 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/index/view.py
--rw-r--r--   0        0        0     1794 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/scenario_test_run.py
--rw-r--r--   0        0        0     1378 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/tag.py
--rw-r--r--   0        0        0     3603 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/admin/views/testing_users.py
--rw-r--r--   0        0        0       52 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/__init__.py
--rw-r--r--   0        0        0     5426 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/app.py
--rw-r--r--   0        0        0      212 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/asgi.py
--rw-r--r--   0        0        0      143 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/auth/__init__.py
--rw-r--r--   0        0        0      348 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/auth/models.py
--rw-r--r--   0        0        0     1271 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/auth/regular.py
--rw-r--r--   0        0        0      902 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/auth/token.py
--rw-r--r--   0        0        0     1914 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/deps.py
--rw-r--r--   0        0        0      848 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/settings.py
--rw-r--r--   0        0        0      521 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/views/__init__.py
--rw-r--r--   0        0        0     1304 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/views/auth_views.py
--rw-r--r--   0        0        0      574 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/views/emulation_views.py
--rw-r--r--   0        0        0      586 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/views/extra_views.py
--rw-r--r--   0        0        0     1224 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/views/feature_views.py
--rw-r--r--   0        0        0      993 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/views/tags_views.py
--rw-r--r--   0        0        0     1816 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/views/testrun_views.py
--rw-r--r--   0        0        0     4383 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/api/views/testuser_views.py
--rw-r--r--   0        0        0     3802 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/base_settings.py
--rw-r--r--   0        0        0      164 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/cli/__init__.py
--rw-r--r--   0        0        0      553 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/cli/admin.py
--rw-r--r--   0        0        0      534 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/cli/api.py
--rw-r--r--   0        0        0      643 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/cli/consumers.py
--rw-r--r--   0        0        0       84 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/cli/db_cmds/__init__.py
--rw-r--r--   0        0        0      830 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/cli/db_cmds/group.py
--rw-r--r--   0        0        0     1520 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/cli/db_cmds/regular.py
--rw-r--r--   0        0        0      358 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/cli/group.py
--rw-r--r--   0        0        0     3048 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/cli/s3.py
--rw-r--r--   0        0        0     1567 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/cli/synchronizer.py
--rw-r--r--   0        0        0      443 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/db/__init__.py
--rw-r--r--   0        0        0     2483 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/db/base.py
--rw-r--r--   0        0        0     1352 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/db/statuses.py
--rw-r--r--   0        0        0     9112 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/db/tables.py
--rw-r--r--   0        0        0     1051 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/db/users.py
--rw-r--r--   0        0        0     1239 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/db/utils.py
--rw-r--r--   0        0        0       46 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/emulation/__init__.py
--rw-r--r--   0        0        0     3629 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/emulation/emulator.py
--rw-r--r--   0        0        0      924 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/__init__.py
--rw-r--r--   0        0        0     1231 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/archiver.py
--rw-r--r--   0        0        0      247 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/auth_managers/__init__.py
--rw-r--r--   0        0        0      347 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/auth_managers/abstract.py
--rw-r--r--   0        0        0      497 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/auth_managers/base.py
--rw-r--r--   0        0        0      588 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/auth_managers/default.py
--rw-r--r--   0        0        0      116 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/auth_managers/ldap/__init__.py
--rw-r--r--   0        0        0     2928 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/auth_managers/ldap/manager.py
--rw-r--r--   0        0        0      198 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/auth_managers/ldap/settings.py
--rw-r--r--   0        0        0     1394 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/auth_managers/secret_mixin.py
--rw-r--r--   0        0        0     1289 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/auth_managers/simple.py
--rw-r--r--   0        0        0      169 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/feature/__init__.py
--rw-r--r--   0        0        0      455 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/feature/abstract.py
--rw-r--r--   0        0        0      221 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/feature/errors.py
--rw-r--r--   0        0        0     2839 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/feature/extractor.py
--rw-r--r--   0        0        0     1092 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/file_extractor.py
--rw-r--r--   0        0        0     1760 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/git_initializer.py
--rw-r--r--   0        0        0       55 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/language/__init__.py
--rw-r--r--   0        0        0     1288 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/language/prefixes.py
--rw-r--r--   0        0        0      102 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/report_manager/__init__.py
--rw-r--r--   0        0        0      447 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/report_manager/models.py
--rw-r--r--   0        0        0     5844 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/report_manager/report_manager.py
--rw-r--r--   0        0        0     7181 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/entities/settings.py
--rw-r--r--   0        0        0       54 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/extra/__init__.py
--rw-r--r--   0        0        0      386 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/extra/prefixes.py
--rw-r--r--   0        0        0      739 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/__init__.py
--rw-r--r--   0        0        0     7159 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/base_factory.py
--rw-r--r--   0        0        0      418 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/components/__init__.py
--rw-r--r--   0        0        0      306 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/components/abstract_consumer.py
--rw-r--r--   0        0        0     4135 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/components/admin_factory.py
--rw-r--r--   0        0        0      994 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/components/emulation_factory.py
--rw-r--r--   0        0        0     3691 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/components/publication_factory.py
--rw-r--r--   0        0        0      486 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/components/s3_init_factory.py
--rw-r--r--   0        0        0     2163 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/components/synchronizer_factory.py
--rw-r--r--   0        0        0     1623 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/components/test_execution_factory.py
--rw-r--r--   0        0        0     1659 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/consumer_factory.py
--rw-r--r--   0        0        0      550 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/context/__init__.py
--rw-r--r--   0        0        0     2974 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/context/admin_context.py
--rw-r--r--   0        0        0     3702 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/context/base_context.py
--rw-r--r--   0        0        0      538 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/context/emulation_context.py
--rw-r--r--   0        0        0     2085 2022-08-22 07:42:20.306683 overhave-3.8.4/overhave/factory/context/publication_context.py
--rw-r--r--   0        0        0     1332 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/factory/context/synchronizer_context.py
--rw-r--r--   0        0        0     2581 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/factory/context/test_execution_context.py
--rw-r--r--   0        0        0      769 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/factory/getters.py
--rw-r--r--   0        0        0      342 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/__init__.py
--rw-r--r--   0        0        0      365 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/abstract_publisher.py
--rw-r--r--   0        0        0     4659 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/base_publisher.py
--rw-r--r--   0        0        0     5369 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/git_publisher.py
--rw-r--r--   0        0        0      224 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/gitlab/__init__.py
--rw-r--r--   0        0        0     4742 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/gitlab/gitlab_publisher.py
--rw-r--r--   0        0        0     1446 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/gitlab/settings.py
--rw-r--r--   0        0        0      171 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/gitlab/tokenizer/__init__.py
--rw-r--r--   0        0        0     2065 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/gitlab/tokenizer/client.py
--rw-r--r--   0        0        0      894 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/gitlab/tokenizer/settings.py
--rw-r--r--   0        0        0      180 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/objects.py
--rw-r--r--   0        0        0      834 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/settings.py
--rw-r--r--   0        0        0      119 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/stash/__init__.py
--rw-r--r--   0        0        0     1697 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/stash/settings.py
--rw-r--r--   0        0        0     3814 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/publication/stash/stash_publisher.py
--rw-r--r--   0        0        0      371 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/__init__.py
--rw-r--r--   0        0        0     3584 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/config_injector.py
--rw-r--r--   0        0        0      827 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/deps.py
--rw-r--r--   0        0        0      530 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/helpers/__init__.py
--rw-r--r--   0        0        0      305 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/helpers/allure_utils/__init__.py
--rw-r--r--   0        0        0      952 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/helpers/allure_utils/description_manager.py
--rw-r--r--   0        0        0     1111 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/helpers/allure_utils/links.py
--rw-r--r--   0        0        0     1276 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/helpers/allure_utils/severity.py
--rw-r--r--   0        0        0     2470 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py
--rw-r--r--   0        0        0     1648 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/helpers/bdd_item.py
--rw-r--r--   0        0        0      994 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/helpers/parsed_info.py
--rw-r--r--   0        0        0     2900 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/helpers/tag_controller.py
--rw-r--r--   0        0        0     7321 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/plugin.py
--rw-r--r--   0        0        0     2274 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/plugin_resolver.py
--rw-r--r--   0        0        0     3957 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/pytest_plugin/proxy_manager.py
--rw-r--r--   0        0        0      498 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/scenario/__init__.py
--rw-r--r--   0        0        0      157 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/scenario/compiler/__init__.py
--rw-r--r--   0        0        0     5240 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/scenario/compiler/compiler.py
--rw-r--r--   0        0        0      631 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/scenario/compiler/settings.py
--rw-r--r--   0        0        0      150 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/scenario/file_manager/__init__.py
--rw-r--r--   0        0        0     3494 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/scenario/file_manager/file_manager.py
--rw-r--r--   0        0        0     2803 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/scenario/file_manager/settings.py
--rw-r--r--   0        0        0      230 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/scenario/parser/__init__.py
--rw-r--r--   0        0        0      918 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/scenario/parser/models.py
--rw-r--r--   0        0        0     8480 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/scenario/parser/parser.py
--rw-r--r--   0        0        0      263 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/scenario/parser/settings.py
--rw-r--r--   0        0        0      235 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/scenario/prefix_mixin.py
--rw-r--r--   0        0        0     2786 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/scenario/validator.py
--rw-r--r--   0        0        0     1229 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/storage/__init__.py
--rw-r--r--   0        0        0     1214 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/storage/api_auth_storage.py
--rw-r--r--   0        0        0     3694 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/storage/converters.py
--rw-r--r--   0        0        0     4377 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/storage/draft_storage.py
--rw-r--r--   0        0        0     6055 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/storage/emulation_storage.py
--rw-r--r--   0        0        0     4729 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/storage/feature_storage.py
--rw-r--r--   0        0        0     1802 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/storage/feature_tag_storage.py
--rw-r--r--   0        0        0     1596 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/storage/feature_type_storage.py
--rw-r--r--   0        0        0     2343 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/storage/scenario_storage.py
--rw-r--r--   0        0        0      617 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/storage/system_user_group_storage.py
--rw-r--r--   0        0        0     2896 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/storage/system_user_storage.py
--rw-r--r--   0        0        0     2900 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/storage/test_run_storage.py
--rw-r--r--   0        0        0     4560 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/storage/test_user_storage.py
--rw-r--r--   0        0        0      192 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/synchronization/__init__.py
--rw-r--r--   0        0        0      260 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/synchronization/abstract.py
--rw-r--r--   0        0        0     3737 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/synchronization/storage_manager.py
--rw-r--r--   0        0        0     6564 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/synchronization/synchronizer.py
--rw-r--r--   0        0        0      263 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/test_execution/__init__.py
--rw-r--r--   0        0        0     4360 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/test_execution/executor.py
--rw-r--r--   0        0        0      575 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/test_execution/objects.py
--rw-r--r--   0        0        0     1596 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/test_execution/settings.py
--rw-r--r--   0        0        0     3546 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/test_execution/step_collector.py
--rw-r--r--   0        0        0     1672 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/test_execution/test_runner.py
--rw-r--r--   0        0        0      933 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/__init__.py
--rw-r--r--   0        0        0      658 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/__init__.py
--rw-r--r--   0        0        0      122 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/api_client/__init__.py
--rw-r--r--   0        0        0     1841 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/api_client/authenticator.py
--rw-r--r--   0        0        0      237 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/api_client/models.py
--rw-r--r--   0        0        0      485 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/api_client/settings.py
--rw-r--r--   0        0        0      208 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/base_client/__init__.py
--rw-r--r--   0        0        0      547 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/base_client/auth.py
--rw-r--r--   0        0        0     2282 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/base_client/client.py
--rw-r--r--   0        0        0      112 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/base_client/objects.py
--rw-r--r--   0        0        0      743 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/base_client/settings.py
--rw-r--r--   0        0        0      289 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/gitlab_client/__init__.py
--rw-r--r--   0        0        0     1847 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/gitlab_client/client.py
--rw-r--r--   0        0        0     1109 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/gitlab_client/models.py
--rw-r--r--   0        0        0      144 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/gitlab_client/objects.py
--rw-r--r--   0        0        0      409 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/gitlab_client/settings.py
--rw-r--r--   0        0        0      707 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/gitlab_client/utils.py
--rw-r--r--   0        0        0      326 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/stash_client/__init__.py
--rw-r--r--   0        0        0     2115 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/stash_client/client.py
--rw-r--r--   0        0        0     2807 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/stash_client/models.py
--rw-r--r--   0        0        0      555 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/http/stash_client/settings.py
--rw-r--r--   0        0        0      109 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/ldap/__init__.py
--rw-r--r--   0        0        0     1936 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/ldap/authenticator.py
--rw-r--r--   0        0        0      420 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/ldap/settings.py
--rw-r--r--   0        0        0      336 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/redis/__init__.py
--rw-r--r--   0        0        0     2672 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/redis/consumer.py
--rw-r--r--   0        0        0     2335 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/redis/objects.py
--rw-r--r--   0        0        0     1061 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/redis/producer.py
--rw-r--r--   0        0        0     1396 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/redis/runner.py
--rw-r--r--   0        0        0      435 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/redis/template.py
--rw-r--r--   0        0        0      132 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/s3/__init__.py
--rw-r--r--   0        0        0     8513 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/s3/manager.py
--rw-r--r--   0        0        0     2122 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/s3/models.py
--rw-r--r--   0        0        0      181 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/s3/objects.py
--rw-r--r--   0        0        0      913 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/transport/s3/settings.py
--rw-r--r--   0        0        0      103 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/utils/__init__.py
--rw-r--r--   0        0        0       84 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/utils/mocks.py
--rw-r--r--   0        0        0      139 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/utils/time.py
--rw-r--r--   0        0        0      179 2022-08-22 07:42:20.310683 overhave-3.8.4/overhave/utils/url.py
--rw-r--r--   0        0        0     3493 2022-08-22 07:42:20.314683 overhave-3.8.4/pyproject.toml
--rw-r--r--   0        0        0    27109 2022-08-22 07:44:11.967871 overhave-3.8.4/setup.py
--rw-r--r--   0        0        0    25560 2022-08-22 07:44:11.969263 overhave-3.8.4/PKG-INFO
+-rw-r--r--   0        0        0    23315 2022-08-22 13:34:13.941154 overhave-3.9.0/README.rst
+-rw-r--r--   0        0        0     3075 2022-08-22 13:34:13.953154 overhave-3.9.0/overhave/__init__.py
+-rw-r--r--   0        0        0       63 2022-08-22 13:34:13.953154 overhave-3.9.0/overhave/admin/__init__.py
+-rw-r--r--   0        0        0     5109 2022-08-22 13:34:13.953154 overhave-3.9.0/overhave/admin/app.py
+-rw-r--r--   0        0        0   735118 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/files/ace-src/ace.js
+-rw-r--r--   0        0        0     5426 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/files/ace-src/mode-gherkin.js
+-rw-r--r--   0        0        0     1263 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/files/css/overhave.css
+-rw-r--r--   0        0        0    38062 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/files/favicon.ico
+-rw-r--r--   0        0        0      138 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/flask/__init__.py
+-rw-r--r--   0        0        0     1819 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/flask/flask_admin.py
+-rw-r--r--   0        0        0      459 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/flask/flask_app.py
+-rw-r--r--   0        0        0      946 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/flask/login_manager.py
+-rw-r--r--   0        0        0      187 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/templates/draft_detail.html
+-rw-r--r--   0        0        0      405 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/templates/emulation.html
+-rw-r--r--   0        0        0      194 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/templates/emulation_create.html
+-rw-r--r--   0        0        0      190 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/templates/emulation_edit.html
+-rw-r--r--   0        0        0      860 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/emulation_run_detail.html
+-rw-r--r--   0        0        0    10445 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/feature.html
+-rw-r--r--   0        0        0      404 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/feature_create.html
+-rw-r--r--   0        0        0      400 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/feature_edit.html
+-rw-r--r--   0        0        0      177 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/index.html
+-rw-r--r--   0        0        0     2414 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/login.html
+-rw-r--r--   0        0        0      149 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/overhave_master.html
+-rw-r--r--   0        0        0     1696 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/test_run.html
+-rw-r--r--   0        0        0     1469 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/test_run_detail.html
+-rw-r--r--   0        0        0      189 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/test_run_list.html
+-rw-r--r--   0        0        0      606 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/test_user.html
+-rw-r--r--   0        0        0      210 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/test_user_create.html
+-rw-r--r--   0        0        0      208 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/test_user_edit.html
+-rw-r--r--   0        0        0      451 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/__init__.py
+-rw-r--r--   0        0        0     1382 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/access.py
+-rw-r--r--   0        0        0     2914 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/base.py
+-rw-r--r--   0        0        0     1105 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/draft.py
+-rw-r--r--   0        0        0     3441 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/emulation.py
+-rw-r--r--   0        0        0     1620 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/emulation_run.py
+-rw-r--r--   0        0        0     9557 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/feature.py
+-rw-r--r--   0        0        0      306 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/formatters/__init__.py
+-rw-r--r--   0        0        0     5169 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/formatters/formatters.py
+-rw-r--r--   0        0        0      669 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/formatters/helpers.py
+-rw-r--r--   0        0        0     1429 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/formatters/safe_formatter.py
+-rw-r--r--   0        0        0       51 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/index/__init__.py
+-rw-r--r--   0        0        0     1680 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/index/custom_page.py
+-rw-r--r--   0        0        0     1536 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/index/login_form.py
+-rw-r--r--   0        0        0     2658 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/index/view.py
+-rw-r--r--   0        0        0     1794 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/scenario_test_run.py
+-rw-r--r--   0        0        0     1378 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/tag.py
+-rw-r--r--   0        0        0     3603 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/testing_users.py
+-rw-r--r--   0        0        0       52 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/__init__.py
+-rw-r--r--   0        0        0     6002 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/app.py
+-rw-r--r--   0        0        0      212 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/asgi.py
+-rw-r--r--   0        0        0      143 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/auth/__init__.py
+-rw-r--r--   0        0        0      348 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/auth/models.py
+-rw-r--r--   0        0        0     1271 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/auth/regular.py
+-rw-r--r--   0        0        0      902 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/auth/token.py
+-rw-r--r--   0        0        0     1914 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/deps.py
+-rw-r--r--   0        0        0      848 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/settings.py
+-rw-r--r--   0        0        0      580 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/__init__.py
+-rw-r--r--   0        0        0     1304 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/auth_views.py
+-rw-r--r--   0        0        0      574 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/emulation_views.py
+-rw-r--r--   0        0        0      586 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/extra_views.py
+-rw-r--r--   0        0        0      491 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/feature_type_views.py
+-rw-r--r--   0        0        0     1224 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/feature_views.py
+-rw-r--r--   0        0        0      993 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/tags_views.py
+-rw-r--r--   0        0        0     1816 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/testrun_views.py
+-rw-r--r--   0        0        0     4383 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/testuser_views.py
+-rw-r--r--   0        0        0     3802 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/base_settings.py
+-rw-r--r--   0        0        0      164 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/__init__.py
+-rw-r--r--   0        0        0      553 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/admin.py
+-rw-r--r--   0        0        0      534 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/api.py
+-rw-r--r--   0        0        0      643 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/consumers.py
+-rw-r--r--   0        0        0       84 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/db_cmds/__init__.py
+-rw-r--r--   0        0        0      830 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/db_cmds/group.py
+-rw-r--r--   0        0        0     1520 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/db_cmds/regular.py
+-rw-r--r--   0        0        0      358 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/group.py
+-rw-r--r--   0        0        0     3048 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/s3.py
+-rw-r--r--   0        0        0     1567 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/synchronizer.py
+-rw-r--r--   0        0        0      443 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/db/__init__.py
+-rw-r--r--   0        0        0     2483 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/db/base.py
+-rw-r--r--   0        0        0     1352 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/db/statuses.py
+-rw-r--r--   0        0        0     9112 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/db/tables.py
+-rw-r--r--   0        0        0     1051 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/db/users.py
+-rw-r--r--   0        0        0     1239 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/db/utils.py
+-rw-r--r--   0        0        0       46 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/emulation/__init__.py
+-rw-r--r--   0        0        0     3629 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/emulation/emulator.py
+-rw-r--r--   0        0        0      924 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/__init__.py
+-rw-r--r--   0        0        0     1231 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/archiver.py
+-rw-r--r--   0        0        0      247 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/__init__.py
+-rw-r--r--   0        0        0      347 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/abstract.py
+-rw-r--r--   0        0        0      497 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/base.py
+-rw-r--r--   0        0        0      588 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/default.py
+-rw-r--r--   0        0        0      116 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/ldap/__init__.py
+-rw-r--r--   0        0        0     2928 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/ldap/manager.py
+-rw-r--r--   0        0        0      198 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/ldap/settings.py
+-rw-r--r--   0        0        0     1394 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/secret_mixin.py
+-rw-r--r--   0        0        0     1289 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/simple.py
+-rw-r--r--   0        0        0      169 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/feature/__init__.py
+-rw-r--r--   0        0        0      455 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/feature/abstract.py
+-rw-r--r--   0        0        0      221 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/feature/errors.py
+-rw-r--r--   0        0        0     2839 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/feature/extractor.py
+-rw-r--r--   0        0        0     1092 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/file_extractor.py
+-rw-r--r--   0        0        0     1760 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/git_initializer.py
+-rw-r--r--   0        0        0       55 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/language/__init__.py
+-rw-r--r--   0        0        0     1288 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/language/prefixes.py
+-rw-r--r--   0        0        0      102 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/report_manager/__init__.py
+-rw-r--r--   0        0        0      447 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/report_manager/models.py
+-rw-r--r--   0        0        0     5844 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/report_manager/report_manager.py
+-rw-r--r--   0        0        0     7181 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/settings.py
+-rw-r--r--   0        0        0       54 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/extra/__init__.py
+-rw-r--r--   0        0        0      386 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/extra/prefixes.py
+-rw-r--r--   0        0        0      739 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/__init__.py
+-rw-r--r--   0        0        0     7159 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/base_factory.py
+-rw-r--r--   0        0        0      418 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/__init__.py
+-rw-r--r--   0        0        0      306 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/abstract_consumer.py
+-rw-r--r--   0        0        0     4135 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/admin_factory.py
+-rw-r--r--   0        0        0      994 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/emulation_factory.py
+-rw-r--r--   0        0        0     3691 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/publication_factory.py
+-rw-r--r--   0        0        0      486 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/s3_init_factory.py
+-rw-r--r--   0        0        0     2163 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/synchronizer_factory.py
+-rw-r--r--   0        0        0     1623 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/test_execution_factory.py
+-rw-r--r--   0        0        0     1659 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/consumer_factory.py
+-rw-r--r--   0        0        0      550 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/__init__.py
+-rw-r--r--   0        0        0     2974 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/admin_context.py
+-rw-r--r--   0        0        0     3702 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/base_context.py
+-rw-r--r--   0        0        0      538 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/emulation_context.py
+-rw-r--r--   0        0        0     2085 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/publication_context.py
+-rw-r--r--   0        0        0     1332 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/synchronizer_context.py
+-rw-r--r--   0        0        0     2581 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/test_execution_context.py
+-rw-r--r--   0        0        0      769 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/getters.py
+-rw-r--r--   0        0        0      342 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/publication/__init__.py
+-rw-r--r--   0        0        0      365 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/publication/abstract_publisher.py
+-rw-r--r--   0        0        0     4659 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/publication/base_publisher.py
+-rw-r--r--   0        0        0     5369 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/publication/git_publisher.py
+-rw-r--r--   0        0        0      224 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/publication/gitlab/__init__.py
+-rw-r--r--   0        0        0     4742 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/gitlab/gitlab_publisher.py
+-rw-r--r--   0        0        0     1446 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/gitlab/settings.py
+-rw-r--r--   0        0        0      171 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/gitlab/tokenizer/__init__.py
+-rw-r--r--   0        0        0     2065 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/gitlab/tokenizer/client.py
+-rw-r--r--   0        0        0      894 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/gitlab/tokenizer/settings.py
+-rw-r--r--   0        0        0      180 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/objects.py
+-rw-r--r--   0        0        0      834 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/settings.py
+-rw-r--r--   0        0        0      119 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/stash/__init__.py
+-rw-r--r--   0        0        0     1697 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/stash/settings.py
+-rw-r--r--   0        0        0     3814 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/stash/stash_publisher.py
+-rw-r--r--   0        0        0      371 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/__init__.py
+-rw-r--r--   0        0        0     3584 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/config_injector.py
+-rw-r--r--   0        0        0      827 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/deps.py
+-rw-r--r--   0        0        0      530 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/__init__.py
+-rw-r--r--   0        0        0      305 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/__init__.py
+-rw-r--r--   0        0        0      952 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/description_manager.py
+-rw-r--r--   0        0        0     1111 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/links.py
+-rw-r--r--   0        0        0     1276 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/severity.py
+-rw-r--r--   0        0        0     2470 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py
+-rw-r--r--   0        0        0     1648 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/bdd_item.py
+-rw-r--r--   0        0        0      994 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/parsed_info.py
+-rw-r--r--   0        0        0     2900 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/tag_controller.py
+-rw-r--r--   0        0        0     7321 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/plugin.py
+-rw-r--r--   0        0        0     2274 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/plugin_resolver.py
+-rw-r--r--   0        0        0     3957 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/proxy_manager.py
+-rw-r--r--   0        0        0      498 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/__init__.py
+-rw-r--r--   0        0        0      157 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/compiler/__init__.py
+-rw-r--r--   0        0        0     5240 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/compiler/compiler.py
+-rw-r--r--   0        0        0      631 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/compiler/settings.py
+-rw-r--r--   0        0        0      150 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/file_manager/__init__.py
+-rw-r--r--   0        0        0     3494 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/file_manager/file_manager.py
+-rw-r--r--   0        0        0     2803 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/file_manager/settings.py
+-rw-r--r--   0        0        0      230 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/parser/__init__.py
+-rw-r--r--   0        0        0      918 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/parser/models.py
+-rw-r--r--   0        0        0     8480 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/parser/parser.py
+-rw-r--r--   0        0        0      263 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/parser/settings.py
+-rw-r--r--   0        0        0      235 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/prefix_mixin.py
+-rw-r--r--   0        0        0     2786 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/validator.py
+-rw-r--r--   0        0        0     1229 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/__init__.py
+-rw-r--r--   0        0        0     1214 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/api_auth_storage.py
+-rw-r--r--   0        0        0     3694 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/converters.py
+-rw-r--r--   0        0        0     4377 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/draft_storage.py
+-rw-r--r--   0        0        0     6055 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/emulation_storage.py
+-rw-r--r--   0        0        0     4729 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/feature_storage.py
+-rw-r--r--   0        0        0     1802 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/feature_tag_storage.py
+-rw-r--r--   0        0        0     2013 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/feature_type_storage.py
+-rw-r--r--   0        0        0     2343 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/scenario_storage.py
+-rw-r--r--   0        0        0      617 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/system_user_group_storage.py
+-rw-r--r--   0        0        0     2896 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/system_user_storage.py
+-rw-r--r--   0        0        0     2900 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/test_run_storage.py
+-rw-r--r--   0        0        0     4560 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/test_user_storage.py
+-rw-r--r--   0        0        0      192 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/synchronization/__init__.py
+-rw-r--r--   0        0        0      260 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/synchronization/abstract.py
+-rw-r--r--   0        0        0     3737 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/synchronization/storage_manager.py
+-rw-r--r--   0        0        0     6564 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/synchronization/synchronizer.py
+-rw-r--r--   0        0        0      263 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/test_execution/__init__.py
+-rw-r--r--   0        0        0     4360 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/test_execution/executor.py
+-rw-r--r--   0        0        0      575 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/test_execution/objects.py
+-rw-r--r--   0        0        0     1596 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/test_execution/settings.py
+-rw-r--r--   0        0        0     3546 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/test_execution/step_collector.py
+-rw-r--r--   0        0        0     1672 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/test_execution/test_runner.py
+-rw-r--r--   0        0        0      933 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/__init__.py
+-rw-r--r--   0        0        0      658 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/__init__.py
+-rw-r--r--   0        0        0      122 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/api_client/__init__.py
+-rw-r--r--   0        0        0     1841 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/api_client/authenticator.py
+-rw-r--r--   0        0        0      237 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/api_client/models.py
+-rw-r--r--   0        0        0      485 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/api_client/settings.py
+-rw-r--r--   0        0        0      208 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/base_client/__init__.py
+-rw-r--r--   0        0        0      547 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/base_client/auth.py
+-rw-r--r--   0        0        0     2282 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/base_client/client.py
+-rw-r--r--   0        0        0      112 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/base_client/objects.py
+-rw-r--r--   0        0        0      743 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/base_client/settings.py
+-rw-r--r--   0        0        0      289 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/gitlab_client/__init__.py
+-rw-r--r--   0        0        0     1847 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/gitlab_client/client.py
+-rw-r--r--   0        0        0     1109 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/gitlab_client/models.py
+-rw-r--r--   0        0        0      144 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/gitlab_client/objects.py
+-rw-r--r--   0        0        0      409 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/gitlab_client/settings.py
+-rw-r--r--   0        0        0      707 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/gitlab_client/utils.py
+-rw-r--r--   0        0        0      326 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/stash_client/__init__.py
+-rw-r--r--   0        0        0     2115 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/stash_client/client.py
+-rw-r--r--   0        0        0     2807 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/stash_client/models.py
+-rw-r--r--   0        0        0      555 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/stash_client/settings.py
+-rw-r--r--   0        0        0      109 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/ldap/__init__.py
+-rw-r--r--   0        0        0     1936 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/ldap/authenticator.py
+-rw-r--r--   0        0        0      420 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/ldap/settings.py
+-rw-r--r--   0        0        0      336 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/redis/__init__.py
+-rw-r--r--   0        0        0     2672 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/redis/consumer.py
+-rw-r--r--   0        0        0     2335 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/redis/objects.py
+-rw-r--r--   0        0        0     1061 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/redis/producer.py
+-rw-r--r--   0        0        0     1396 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/redis/runner.py
+-rw-r--r--   0        0        0      435 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/redis/template.py
+-rw-r--r--   0        0        0      132 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/s3/__init__.py
+-rw-r--r--   0        0        0     8513 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/s3/manager.py
+-rw-r--r--   0        0        0     2122 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/s3/models.py
+-rw-r--r--   0        0        0      181 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/s3/objects.py
+-rw-r--r--   0        0        0      913 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/s3/settings.py
+-rw-r--r--   0        0        0      103 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/utils/__init__.py
+-rw-r--r--   0        0        0       84 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/utils/mocks.py
+-rw-r--r--   0        0        0      139 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/utils/time.py
+-rw-r--r--   0        0        0      179 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/utils/url.py
+-rw-r--r--   0        0        0     3493 2022-08-22 13:34:13.969154 overhave-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0    27109 2022-08-22 13:36:02.605930 overhave-3.9.0/setup.py
+-rw-r--r--   0        0        0    25560 2022-08-22 13:36:02.607434 overhave-3.9.0/PKG-INFO
```

### Comparing `overhave-3.8.4/README.rst` & `overhave-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/__init__.py` & `overhave-3.9.0/overhave/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/app.py` & `overhave-3.9.0/overhave/admin/app.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/files/ace-src/ace.js` & `overhave-3.9.0/overhave/admin/files/ace-src/ace.js`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/files/ace-src/mode-gherkin.js` & `overhave-3.9.0/overhave/admin/files/ace-src/mode-gherkin.js`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/files/css/overhave.css` & `overhave-3.9.0/overhave/admin/files/css/overhave.css`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/files/favicon.ico` & `overhave-3.9.0/overhave/admin/files/favicon.ico`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/flask/flask_admin.py` & `overhave-3.9.0/overhave/admin/flask/flask_admin.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/flask/login_manager.py` & `overhave-3.9.0/overhave/admin/flask/login_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/templates/emulation_run_detail.html` & `overhave-3.9.0/overhave/admin/templates/emulation_run_detail.html`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/templates/feature.html` & `overhave-3.9.0/overhave/admin/templates/feature.html`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/templates/login.html` & `overhave-3.9.0/overhave/admin/templates/login.html`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/templates/test_run.html` & `overhave-3.9.0/overhave/admin/templates/test_run.html`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/templates/test_run_detail.html` & `overhave-3.9.0/overhave/admin/templates/test_run_detail.html`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/templates/test_user.html` & `overhave-3.9.0/overhave/admin/templates/test_user.html`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/access.py` & `overhave-3.9.0/overhave/admin/views/access.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/base.py` & `overhave-3.9.0/overhave/admin/views/base.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/draft.py` & `overhave-3.9.0/overhave/admin/views/draft.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/emulation.py` & `overhave-3.9.0/overhave/admin/views/emulation.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/emulation_run.py` & `overhave-3.9.0/overhave/admin/views/emulation_run.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/feature.py` & `overhave-3.9.0/overhave/admin/views/feature.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/formatters/formatters.py` & `overhave-3.9.0/overhave/admin/views/formatters/formatters.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/formatters/helpers.py` & `overhave-3.9.0/overhave/admin/views/formatters/helpers.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/formatters/safe_formatter.py` & `overhave-3.9.0/overhave/admin/views/formatters/safe_formatter.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/index/custom_page.py` & `overhave-3.9.0/overhave/admin/views/index/custom_page.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/index/login_form.py` & `overhave-3.9.0/overhave/admin/views/index/login_form.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/index/view.py` & `overhave-3.9.0/overhave/admin/views/index/view.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/scenario_test_run.py` & `overhave-3.9.0/overhave/admin/views/scenario_test_run.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/tag.py` & `overhave-3.9.0/overhave/admin/views/tag.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/admin/views/testing_users.py` & `overhave-3.9.0/overhave/admin/views/testing_users.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/api/app.py` & `overhave-3.9.0/overhave/api/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from overhave.api.auth import get_authorized_user
 from overhave.api.views import (
     delete_test_user_handler,
     docs,
     emulation_run_list_handler,
     favicon,
+    feature_types_list_handler,
     get_features_handler,
     get_test_run_handler,
     get_test_user_handler,
     login_for_access_token,
     run_tests_by_tag_handler,
     tags_item_handler,
     tags_list_handler,
@@ -19,14 +20,15 @@
     test_user_list_handler,
     test_user_put_spec_handler,
 )
 from overhave.storage import (
     AuthToken,
     EmulationRunModel,
     FeatureModel,
+    FeatureTypeModel,
     TagModel,
     TestRunModel,
     TestUserModel,
     TestUserSpecification,
 )
 
 
@@ -47,14 +49,27 @@
         methods=["GET"],
         summary="Get FeatureTags",
         description="Get list of feature tags like `value`",
     )
     return tags_router
 
 
+def _get_feature_type_router() -> fastapi.APIRouter:
+    feature_router = fastapi.APIRouter()
+    feature_router.add_api_route(
+        "/list",
+        feature_types_list_handler,
+        methods=["GET"],
+        response_model=List[FeatureTypeModel],
+        summary="Get list of FeatureType info",
+        description="Get list of feature types",
+    )
+    return feature_router
+
+
 def _get_feature_router() -> fastapi.APIRouter:
     feature_router = fastapi.APIRouter()
     feature_router.add_api_route(
         "/",
         get_features_handler,
         methods=["GET"],
         response_model=List[FeatureModel],
@@ -157,14 +172,17 @@
 
 
 def create_overhave_api() -> fastapi.FastAPI:
     app = fastapi.FastAPI()
     auth_deps = [fastapi.Depends(get_authorized_user)]
 
     app.include_router(_get_tags_router(), dependencies=auth_deps, prefix="/feature/tags", tags=["feature_tags"])
+    app.include_router(
+        _get_feature_type_router(), dependencies=auth_deps, prefix="/feature/types", tags=["feature_types"]
+    )
     app.include_router(_get_feature_router(), dependencies=auth_deps, prefix="/feature", tags=["features"])
     app.include_router(_get_testuser_router(), dependencies=auth_deps, prefix="/test_user", tags=["test_users"])
     app.include_router(_get_testrun_router(), dependencies=auth_deps, prefix="/test_run", tags=["test_runs"])
     app.include_router(_get_emulation_router(), dependencies=auth_deps, prefix="/emulation", tags=["emulations"])
 
     app.include_router(_get_auth_router())
     app.add_api_route("/", docs, methods=["GET"], include_in_schema=False)
```

### Comparing `overhave-3.8.4/overhave/api/auth/regular.py` & `overhave-3.9.0/overhave/api/auth/regular.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/api/auth/token.py` & `overhave-3.9.0/overhave/api/auth/token.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/api/deps.py` & `overhave-3.9.0/overhave/api/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/api/settings.py` & `overhave-3.9.0/overhave/api/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/api/views/auth_views.py` & `overhave-3.9.0/overhave/api/views/auth_views.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/api/views/emulation_views.py` & `overhave-3.9.0/overhave/api/views/emulation_views.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/api/views/extra_views.py` & `overhave-3.9.0/overhave/api/views/extra_views.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/api/views/feature_views.py` & `overhave-3.9.0/overhave/api/views/feature_views.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/api/views/tags_views.py` & `overhave-3.9.0/overhave/api/views/tags_views.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/api/views/testrun_views.py` & `overhave-3.9.0/overhave/api/views/testrun_views.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/api/views/testuser_views.py` & `overhave-3.9.0/overhave/api/views/testuser_views.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/base_settings.py` & `overhave-3.9.0/overhave/base_settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/cli/admin.py` & `overhave-3.9.0/overhave/cli/admin.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/cli/api.py` & `overhave-3.9.0/overhave/cli/api.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/cli/consumers.py` & `overhave-3.9.0/overhave/cli/consumers.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/cli/db_cmds/group.py` & `overhave-3.9.0/overhave/cli/db_cmds/group.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/cli/db_cmds/regular.py` & `overhave-3.9.0/overhave/cli/db_cmds/regular.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/cli/s3.py` & `overhave-3.9.0/overhave/cli/s3.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/cli/synchronizer.py` & `overhave-3.9.0/overhave/cli/synchronizer.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/db/base.py` & `overhave-3.9.0/overhave/db/base.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/db/statuses.py` & `overhave-3.9.0/overhave/db/statuses.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/db/tables.py` & `overhave-3.9.0/overhave/db/tables.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/db/users.py` & `overhave-3.9.0/overhave/db/users.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/db/utils.py` & `overhave-3.9.0/overhave/db/utils.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/emulation/emulator.py` & `overhave-3.9.0/overhave/emulation/emulator.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/entities/__init__.py` & `overhave-3.9.0/overhave/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/entities/archiver.py` & `overhave-3.9.0/overhave/entities/archiver.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/entities/auth_managers/default.py` & `overhave-3.9.0/overhave/entities/auth_managers/default.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/entities/auth_managers/ldap/manager.py` & `overhave-3.9.0/overhave/entities/auth_managers/ldap/manager.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/entities/auth_managers/secret_mixin.py` & `overhave-3.9.0/overhave/entities/auth_managers/secret_mixin.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/entities/auth_managers/simple.py` & `overhave-3.9.0/overhave/entities/auth_managers/simple.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/entities/feature/extractor.py` & `overhave-3.9.0/overhave/entities/feature/extractor.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/entities/file_extractor.py` & `overhave-3.9.0/overhave/entities/file_extractor.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/entities/git_initializer.py` & `overhave-3.9.0/overhave/entities/git_initializer.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/entities/language/prefixes.py` & `overhave-3.9.0/overhave/entities/language/prefixes.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/entities/report_manager/report_manager.py` & `overhave-3.9.0/overhave/entities/report_manager/report_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/entities/settings.py` & `overhave-3.9.0/overhave/entities/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/__init__.py` & `overhave-3.9.0/overhave/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/base_factory.py` & `overhave-3.9.0/overhave/factory/base_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/components/admin_factory.py` & `overhave-3.9.0/overhave/factory/components/admin_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/components/emulation_factory.py` & `overhave-3.9.0/overhave/factory/components/emulation_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/components/publication_factory.py` & `overhave-3.9.0/overhave/factory/components/publication_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/components/synchronizer_factory.py` & `overhave-3.9.0/overhave/factory/components/synchronizer_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/components/test_execution_factory.py` & `overhave-3.9.0/overhave/factory/components/test_execution_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/consumer_factory.py` & `overhave-3.9.0/overhave/factory/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/context/__init__.py` & `overhave-3.9.0/overhave/factory/context/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/context/admin_context.py` & `overhave-3.9.0/overhave/factory/context/admin_context.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/context/base_context.py` & `overhave-3.9.0/overhave/factory/context/base_context.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/context/emulation_context.py` & `overhave-3.9.0/overhave/factory/context/emulation_context.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/context/publication_context.py` & `overhave-3.9.0/overhave/factory/context/publication_context.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/context/synchronizer_context.py` & `overhave-3.9.0/overhave/factory/context/synchronizer_context.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/context/test_execution_context.py` & `overhave-3.9.0/overhave/factory/context/test_execution_context.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/factory/getters.py` & `overhave-3.9.0/overhave/factory/getters.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/publication/base_publisher.py` & `overhave-3.9.0/overhave/publication/base_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/publication/git_publisher.py` & `overhave-3.9.0/overhave/publication/git_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/publication/gitlab/gitlab_publisher.py` & `overhave-3.9.0/overhave/publication/gitlab/gitlab_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/publication/gitlab/settings.py` & `overhave-3.9.0/overhave/publication/gitlab/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/publication/gitlab/tokenizer/client.py` & `overhave-3.9.0/overhave/publication/gitlab/tokenizer/client.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/publication/gitlab/tokenizer/settings.py` & `overhave-3.9.0/overhave/publication/gitlab/tokenizer/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/publication/settings.py` & `overhave-3.9.0/overhave/publication/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/publication/stash/settings.py` & `overhave-3.9.0/overhave/publication/stash/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/publication/stash/stash_publisher.py` & `overhave-3.9.0/overhave/publication/stash/stash_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/pytest_plugin/config_injector.py` & `overhave-3.9.0/overhave/pytest_plugin/config_injector.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/pytest_plugin/deps.py` & `overhave-3.9.0/overhave/pytest_plugin/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/pytest_plugin/helpers/__init__.py` & `overhave-3.9.0/overhave/pytest_plugin/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/pytest_plugin/helpers/allure_utils/description_manager.py` & `overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/description_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/pytest_plugin/helpers/allure_utils/links.py` & `overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/links.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/pytest_plugin/helpers/allure_utils/severity.py` & `overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/severity.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py` & `overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/pytest_plugin/helpers/bdd_item.py` & `overhave-3.9.0/overhave/pytest_plugin/helpers/bdd_item.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/pytest_plugin/helpers/parsed_info.py` & `overhave-3.9.0/overhave/pytest_plugin/helpers/parsed_info.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/pytest_plugin/helpers/tag_controller.py` & `overhave-3.9.0/overhave/pytest_plugin/helpers/tag_controller.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/pytest_plugin/plugin.py` & `overhave-3.9.0/overhave/pytest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/pytest_plugin/plugin_resolver.py` & `overhave-3.9.0/overhave/pytest_plugin/plugin_resolver.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/pytest_plugin/proxy_manager.py` & `overhave-3.9.0/overhave/pytest_plugin/proxy_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/scenario/compiler/compiler.py` & `overhave-3.9.0/overhave/scenario/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/scenario/compiler/settings.py` & `overhave-3.9.0/overhave/scenario/compiler/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/scenario/file_manager/file_manager.py` & `overhave-3.9.0/overhave/scenario/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/scenario/file_manager/settings.py` & `overhave-3.9.0/overhave/scenario/file_manager/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/scenario/parser/models.py` & `overhave-3.9.0/overhave/scenario/parser/models.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/scenario/parser/parser.py` & `overhave-3.9.0/overhave/scenario/parser/parser.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/scenario/validator.py` & `overhave-3.9.0/overhave/scenario/validator.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/storage/__init__.py` & `overhave-3.9.0/overhave/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/storage/api_auth_storage.py` & `overhave-3.9.0/overhave/storage/api_auth_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/storage/converters.py` & `overhave-3.9.0/overhave/storage/converters.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/storage/draft_storage.py` & `overhave-3.9.0/overhave/storage/draft_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/storage/emulation_storage.py` & `overhave-3.9.0/overhave/storage/emulation_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/storage/feature_storage.py` & `overhave-3.9.0/overhave/storage/feature_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/storage/feature_tag_storage.py` & `overhave-3.9.0/overhave/storage/feature_tag_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/storage/feature_type_storage.py` & `overhave-3.9.0/overhave/storage/feature_type_storage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import abc
-from typing import cast
+from typing import List, cast
 
 from overhave import db
 from overhave.storage.converters import FeatureTypeModel
 
 
 class BaseFeatureTypeStorageException(Exception):
     """Base exception for :class:`FeatureTypeStorage`."""
@@ -22,14 +22,19 @@
         pass
 
     @staticmethod
     @abc.abstractmethod
     def get_feature_type_by_name(name: str) -> FeatureTypeModel:
         pass
 
+    @staticmethod
+    @abc.abstractmethod
+    def get_all_feature_types() -> List[FeatureTypeModel]:
+        pass
+
 
 class FeatureTypeStorage(IFeatureTypeStorage):
     """Class for feature type storage."""
 
     @staticmethod
     def get_default_feature_type() -> FeatureTypeModel:
         with db.create_session() as session:
@@ -41,7 +46,13 @@
         with db.create_session() as session:
             feature_type: db.FeatureType = (
                 session.query(db.FeatureType).filter(db.FeatureType.name == name).one_or_none()
             )
             if feature_type is None:
                 raise FeatureTypeNotExistsError(f"Could not find feature type with name='{name}'!")
             return cast(FeatureTypeModel, FeatureTypeModel.from_orm(feature_type))
+
+    @staticmethod
+    def get_all_feature_types() -> List[FeatureTypeModel]:
+        with db.create_session() as session:
+            db_feature_types = session.query(db.FeatureType).all()
+            return cast(List[FeatureTypeModel], [FeatureTypeModel.from_orm(x) for x in db_feature_types])
```

### Comparing `overhave-3.8.4/overhave/storage/scenario_storage.py` & `overhave-3.9.0/overhave/storage/scenario_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/storage/system_user_group_storage.py` & `overhave-3.9.0/overhave/storage/system_user_group_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/storage/system_user_storage.py` & `overhave-3.9.0/overhave/storage/system_user_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/storage/test_run_storage.py` & `overhave-3.9.0/overhave/storage/test_run_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/storage/test_user_storage.py` & `overhave-3.9.0/overhave/storage/test_user_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/synchronization/storage_manager.py` & `overhave-3.9.0/overhave/synchronization/storage_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/synchronization/synchronizer.py` & `overhave-3.9.0/overhave/synchronization/synchronizer.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/test_execution/executor.py` & `overhave-3.9.0/overhave/test_execution/executor.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/test_execution/objects.py` & `overhave-3.9.0/overhave/test_execution/objects.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/test_execution/settings.py` & `overhave-3.9.0/overhave/test_execution/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/test_execution/step_collector.py` & `overhave-3.9.0/overhave/test_execution/step_collector.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/test_execution/test_runner.py` & `overhave-3.9.0/overhave/test_execution/test_runner.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/__init__.py` & `overhave-3.9.0/overhave/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/http/__init__.py` & `overhave-3.9.0/overhave/transport/http/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/http/api_client/authenticator.py` & `overhave-3.9.0/overhave/transport/http/api_client/authenticator.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/http/base_client/auth.py` & `overhave-3.9.0/overhave/transport/http/base_client/auth.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/http/base_client/client.py` & `overhave-3.9.0/overhave/transport/http/base_client/client.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/http/base_client/settings.py` & `overhave-3.9.0/overhave/transport/http/base_client/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/http/gitlab_client/client.py` & `overhave-3.9.0/overhave/transport/http/gitlab_client/client.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/http/gitlab_client/models.py` & `overhave-3.9.0/overhave/transport/http/gitlab_client/models.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/http/gitlab_client/utils.py` & `overhave-3.9.0/overhave/transport/http/gitlab_client/utils.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/http/stash_client/client.py` & `overhave-3.9.0/overhave/transport/http/stash_client/client.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/http/stash_client/models.py` & `overhave-3.9.0/overhave/transport/http/stash_client/models.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/http/stash_client/settings.py` & `overhave-3.9.0/overhave/transport/http/stash_client/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/ldap/authenticator.py` & `overhave-3.9.0/overhave/transport/ldap/authenticator.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/redis/consumer.py` & `overhave-3.9.0/overhave/transport/redis/consumer.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/redis/objects.py` & `overhave-3.9.0/overhave/transport/redis/objects.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/redis/producer.py` & `overhave-3.9.0/overhave/transport/redis/producer.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/redis/runner.py` & `overhave-3.9.0/overhave/transport/redis/runner.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/s3/manager.py` & `overhave-3.9.0/overhave/transport/s3/manager.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/s3/models.py` & `overhave-3.9.0/overhave/transport/s3/models.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/overhave/transport/s3/settings.py` & `overhave-3.9.0/overhave/transport/s3/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.8.4/pyproject.toml` & `overhave-3.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "overhave"
-version = "3.8.4"
+version = "3.9.0"
 description = "Overhave - web-framework for BDD"
 readme = "README.rst"
 authors = [
     "Vladislav Mukhamatnurov <livestreamepidemz@yandex.ru>",
     "Tinkoff Backend Dialog System Team <bds-dev@tinkoff.ru>"
 ]
 classifiers = [
```

### Comparing `overhave-3.8.4/setup.py` & `overhave-3.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 entry_points = \
 {'console_scripts': ['overhave = overhave.cli:overhave',
                      'overhave-demo = demo:overhave_demo'],
  'pytest11': ['overhave = overhave.pytest_plugin.plugin']}
 
 setup_kwargs = {
     'name': 'overhave',
-    'version': '3.8.4',
+    'version': '3.9.0',
     'description': 'Overhave - web-framework for BDD',
     'long_description': '========\nOverhave\n========\n\n.. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/label_img.png\n  :width: 700\n  :align: center\n  :alt: Overhave framework\n\n  `Overhave`_ is the web-framework for BDD: scalable, configurable, easy to use, based on\n  `Flask Admin`_ and `Pydantic`_.\n\n  .. image:: https://github.com/TinkoffCreditSystems/overhave/workflows/CI/badge.svg\n    :target: https://github.com/TinkoffCreditSystems/overhave/actions?query=workflow%3ACI\n    :alt: CI\n\n  .. image:: https://img.shields.io/pypi/pyversions/overhave.svg\n    :target: https://pypi.org/project/overhave\n    :alt: Python versions\n\n  .. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/TinkoffCreditSystems/overhave\n    :alt: Code style\n\n  .. image:: https://img.shields.io/pypi/v/overhave?color=%2334D058&label=pypi%20package\n    :target: https://pypi.org/project/overhave\n    :alt: Package version\n\n  .. image:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/coverage.svg\n    :target: https://github.com/TinkoffCreditSystems/overhave\n    :alt: PyTest Coverage percent\n    \n  .. image:: https://img.shields.io/pypi/dm/overhave.svg\n    :target: https://pypi.org/project/overhave\n    :alt: Downloads per month\n\n--------\nFeatures\n--------\n\n* Ready web-interface for easy BDD features management with `Ace`_ editor\n* Traditional Gherkin format for scenarios provided by `pytest-bdd`_\n* Execution and reporting of BDD features based on `Allure`_\n* Auto-collection of `pytest-bdd`_ steps and display on web-interface\n* Simple scenarios structure, easy horizontal scaling\n* Built-in wrappers for `pytest-bdd`_ hooks to supplement `Allure`_ report\n* Ability to create and use several BDD keywords dictionary with different languages\n* Versioning and deployment of scenario drafts to `Bitbucket`_ or `GitLab`_\n* Synchronization between `git`_ repository and database with features\n* Built-in configurable access management of users and groups\n* Configurable strategy for user authorization (LDAP also provided)\n* Database schema based on `SQLAlchemy`_ models and works with PostgreSQL\n* Still configurable as `Flask Admin`_, supports plug-ins and extensions\n* Has built-in API application with Swagger docs, based on `FastAPI`_\n* Distributed `producer-consumer` architecture based on `Walrus`_ Redis streams\n* Command-line interface, provided with `Typer`_\n* Integrated interaction for files storage with s3-cloud based on `boto3`_\n* Web-browser emulation ability with custom toolkit (`GoTTY`_, for example)\n\n------------\nInstallation\n------------\n\nYou can install **Overhave** via pip from PyPI:\n\n.. code-block:: shell\n\n    pip install overhave\n\n--------\nOverview\n--------\n\nWeb-interface\n-------------\n\nThe web-interface is a basic tool for BDD features management. It consists of:\n\n* `Info` - index page with optional information about your tool or project;\n* `Scenarios` - section for features management, contains subsections\n    `Features`, `Test runs`, `Versions` and `Tags`:\n\n    * `Features`\n        gives an interface for features records management and provides info\n        about id, name author, time, editor and publishing status; it is possible\n        to search, edit or delete items through Script panel.\n\n        .. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/label_img.png\n          :width: 500\n          :align: center\n          :alt: Features list\n\n    * `Test runs`\n        gives an interface for test runs management and provides info about.\n\n        .. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/test_runs_img.png\n          :width: 500\n          :align: center\n          :alt: Test runs list\n\n    * Versions\n        contains feature versions in corresponding to test runs; versions contains PR-links to\n        the remote Git repository.\n\n        .. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/versions_img.png\n          :width: 500\n          :align: center\n          :alt: Feature published versions list\n\n    * Tags\n        contains tags values, which are used for feature\'s tagging.\n\n        .. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/tags_img.png\n          :width: 500\n          :align: center\n          :alt: Feature published versions list\n\n* `Test users` - section for viewing and configuring test users;\n* `Access` - section for access management, contains `Users` and\n    `Groups` subsections;\n* `Emulation` - experimental section for alternative tools implementation\n    (in development).\n\n**Overhave** features could be created and/or edited through special\n*script panel* in feature edit mode. Feature should have type registered by the\napplication, unique name, specified tasks list with the traditional format\n```PRJ-NUMBER``` and scenario text.\n\n**Script panel** has `pytest-bdd`_ steps table on the right side of interface.\nThese steps should be defined in appropriate fixture modules and registered\nat the application on start-up to be displayed.\n\n\n.. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/panel_img.png\n  :width: 600\n  :align: center\n  :alt: Script panel\n\n  Example of **Overhave** script panel in feature edit mode\n\nAllure report\n-------------\n\n**Overhave** generates `Allure`_ report after tests execution in web-interface.\nIf you execute tests manually through `PyTest`_, these results are could be\nconverted into the `Allure`_ report also with the `Allure CLI`_ tool.\nThis report contains scenarios descriptions as they are described in features.\n\n.. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/report_img.png\n  :width: 600\n  :align: center\n  :alt: Allure test-case report\n\n  Example of generated `Allure`_ report after execution of **Overhave**\'s feature\n\nDemo-mode (Quickstart)\n----------------------\n\n**Overhave** has special demo-mode (in development), which could be possibly\nused for framework demonstration and manual debugging / testing. The framework\nprovides a CLI entrypoints for easy server run in debug mode:\n\n.. code-block:: shell\n\n    make up  # start PostgreSQL database and Redis\n    overhave db create-all  # create Overhave database schema\n    overhave-demo admin  # start Overhave admin on port 8076 in debug mode\n    overhave-demo consumer -s test  # start Overhave test execution consumer\n\n**Note**: you could run admin in special mode, which does not require\nconsumers. This mode uses *threadpool* for running testing and publication\ntasks asynchronously:\n\n.. code-block:: shell\n\n    overhave-demo admin --threadpool --language=ru\n\nBut this *threadpool* mode is unscalable in *kubernetes* paradigm. So,\nit\'s highly recommended to use corresponding consumers exactly.\n\nCommand-line interface\n----------------------\n\n**Overhave** has a CLI that provides a simple way to start service web-interface,\nrun consumer and execute basic database operations. Examples are below:\n\n.. code-block:: shell\n\n    overhave db create-all\n    overhave admin --port 8080\n    overhave consumer -s publication\n    overhave api -p 8000 -w 4\n\n**Note**: service start-up takes a set of settings, so you can set them through\nvirtual environment with prefix ```OVERHAVE_```, for example ```OVERHAVE_DB_URL```.\nIf you want to configure settings in more explicit way through context injection,\nplease see next part of docs.\n\nContext injection\n-----------------\n\nContext setting\n^^^^^^^^^^^^^^^\n\nService could be configured via application context injection with prepared\ninstance of `OverhaveContext` object. This context could be set using\n```set_context``` function of initialized ```ProxyFactory``` instance.\n\nFor example, ```my_custom_context``` prepared. So, application start-up could\nbe realised with follow code:\n\n.. code-block:: python\n\n    from overhave import overhave_app, overhave_admin_factory\n\n    factory = overhave_admin_factory()\n    factory.set_context(my_custom_context)\n    overhave_app(factory).run(host=\'localhost\', port=8080, debug=True)\n\n**Note**:\n\n* ```overhave_app``` is the prepared `Flask` application with already enabled\n    Flask Admin and Login Manager plug-ins;\n* ```overhave_factory``` is a function for LRU cached instance of the **Overhave**\n    factory ```ProxyFactory```; the instance has an access to application components,\n    directly used in ```overhave_app```.\n* ```my_custom_context``` is an example of context configuration, see an\n    example code in `context_example.rst`_.\n\nEnabling of injection\n^^^^^^^^^^^^^^^^^^^^^\n\n**Overhave** has it\'s own built-in `PyTest`_ plugin, which is used to enable\nand configure injection of prepared context into application core instance.\nThe plugin provides one option:\n\n* `--enable-injection` - flag to enable context injection.\n\nThe `PyTest` usage should be similar to:\n\n.. code-block:: bash\n\n    pytest --enable-injection\n\nConsumers\n---------\n\n**Overhave** has `producer-consumer` architecture, based on Redis streams,\nand supported 3 consumer\'s types:\n\n* **TEST** - consumer for test execution with it\'s own factory\n    ```overhave_test_execution_factory```;\n\n* **PUBLICATION** - consumer for features publication with it\'s own factory\n    ```overhave_publication_factory```;\n\n* **EMULATION** - consumer for specific emulation with it\'s own factory\n    ```overhave_emulation_factory```.\n\n**Note**: the ```overhave_test_execution_factory``` has ability for context injection\nand could be enriched with the custom context as the ```overhave_admin_factory```.\n\nProject structure\n-----------------\n\n**Overhave** supports it\'s own special project structure:\n\n.. image:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/project_structure.png\n  :width: 300\n  :alt: **Overhave** project structure\n\nThe right approach is to create a **root directory** (like "demo" inside the current\nrepository) that contains **features**, **fixtures** and **steps** directories.\n\nThe **Features** directory contains different feature types as\nseparate directories, each of them corresponds to predefined `pytest-bdd`_\nset of steps.\n\nThe **Fixtures** directory contains typical `PyTest`_ modules splitted by different\nfeature types. These modules are used for `pytest-bdd`_ isolated test runs. It is\nnecessary because of special mechanism of `pytest-bdd`_ steps collection.\n\nThe **Steps** directory contains `pytest-bdd`_ steps packages splitted by differrent\nfeature types also. Each steps subdirectory has it\'s own declared steps in according\nto supported feature type.\n\nSo, it is possible to create your own horizontal structure of\ndifferent product directions with unique steps and `PyTest`_ fixtures.\n\n**Note**: this structure is used in **Overhave** application. The formed data\ngives a possibility to specify registered feature type in the web-interface\n*script panel*. Also, this structure defines which steps will be displayed in\nthe right side of *script panel*.\n\nFeature format\n--------------\n\n**Overhave** has it\'s own special feature\'s text format, which inherits\nGherkin from `pytest-bdd`_ with unique updates:\n\n* required tag that is related to existing feature type directory, where\n    current feature is located;\n* any amount of arbitrary tags;\n* severity tag - implements `Allure`_ severity to feature or just tagged\n    scenario (for example: ```@severity.blocker```);\n* info about feature - who is creator, last editor and publisher;\n* task tracker\'s tickets with format ```PRJ-1234```;\n\nAn example of filled feature content is located in\n`feature_example.rst`_.\n\nPytest markers\n--------------\n\n**Overhave** implements solution for `PyTest`_ markers usage with custom\nadditional information:\n\n* "`disabled`": same as `skip` marker, but it\'s necessary to setup reason;\n* "`xfail`": traditional `xfail` with strict reason presence.\n\nExamples:\n\n.. code-block:: gherkin\n\n    @disabled(not ready)\n    Feature: My business feature\n\n.. code-block:: gherkin\n\n    @disabled(TODO: https://tracker.myorg.com/browse/PRJ-333; deadline 01.01.25)\n    Scenario: Yet another business feature\n\n\n.. code-block:: gherkin\n\n    @xfail(bug: https://tracker.myorg.com/browse/PRJ-555)\n    Scenario outline: Other business feature\n\nIf reason contains URL, so **Overhave** will attach `Allure` link to report:\nfor `disabled` - it will be `LinkType.LINK`, for `xfail` - `LinkType.ISSUE`.\n\nFeature links\n-------------\n\n**Overhave** has ability to set links to it\'s own admin service in `Allure`_\ntest-cases. Link will be set automatically when you generate `Allure`_ report.\nThis function can be enabled via setup of environment variable\n```OVERHAVE_ADMIN_URL```:\n\n.. code-block:: bash\n\n    export OVERHAVE_ADMIN_URL=https://overhave-admin.myorg.com\n\nAlso, **Overhave** has ability to set links to feature file in `Git`_ repository.\nLink will be set automatically when you generate `Allure`_ report. This function\ncan be enabled via setup of environment variable\n```OVERHAVE_GIT_PROJECT_URL```:\n\n.. code-block:: bash\n\n    export OVERHAVE_GIT_PROJECT_URL=https://git.myorg.com/bdd-features-repo\n\n\nLanguage\n--------\n\nThe web-interface language is ENG by default and could not be switched\n(if it\'s necessary - please, create a ```feature request``` or contribute\nyourself).\n\nThe feature text as well as `pytest-bdd`_ BDD keywords are configurable\nwith **Overhave** extra models, for example RUS keywords are already defined\nin framework and available for usage:\n\n.. code-block:: python\n\n    from overhave.extra import RUSSIAN_PREFIXES\n\n    language_settings = OverhaveLanguageSettings(step_prefixes=RUSSIAN_PREFIXES)\n\n**Note**: you could create your own prefix-value mapping for your language:\n\n.. code-block:: python\n\n    from overhave import StepPrefixesModel\n\n    GERMAN_PREFIXES = StepPrefixesModel(\n        FEATURE="Merkmal:",\n        SCENARIO_OUTLINE="Szenarioübersicht:",\n        SCENARIO="Szenario:",\n        BACKGROUND="Hintergrund:",\n        EXAMPLES="Beispiele:",\n        EXAMPLES_VERTICAL="Beispiele: Vertikal",\n        GIVEN="Gegeben ",\n        WHEN="Wann ",\n        THEN="Dann ",\n        AND="Und ",\n        BUT="Aber ",\n    )\n\nGit integration\n---------------\n\n**Overhave** gives an ability to sent your new features or changes to\nremote git repository, which is hosted by `Bitbucket`_ or `GitLab`_.\nIntegration with bitbucket is native, while integration with GitLab\nuses `python-gitlab`_ library.\n\nYou are able to set necessary settings for your project:\n\n.. code-block:: python\n\n    publisher_settings = OverhaveGitlabPublisherSettings(\n        repository_id=\'123\',\n        default_target_branch_name=\'master\',\n    )\n    client_settings=OverhaveGitlabClientSettings(\n        url="https://gitlab.mycompany.com",\n        auth_token=os.environ.get("MY_GITLAB_AUTH_TOKEN"),\n    )\n\nThe pull-request (for Bitbucket) or merge-request (for GitLab)\ncreated when you click the button `Create pull request` on\ntest run result\'s page. This button is available only for `success`\ntest run\'s result.\n\n**Note**: one of the most popular cases of GitLab API\nauthentication is the OAUTH2 schema with service account.\nIn according to this schema, you should have OAUTH2 token,\nwhich is might have a short life-time and could not be\nspecified through environment. For this situation, **Overhave**\nhas special `TokenizerClient` with it\'s own\n`TokenizerClientSettings` - this simple client could take\nthe token from a remote custom GitLab tokenizer service.\n\nGit-to-DataBase synchronization\n-------------------------------\n\n**Overhave** gives an ability to synchronize your current `git`_\nrepository\'s state with database. It means that your features,\nwhich are located on the database, could be updated - and the source\nof updates is your repository.\n\n**For example**: you had to do bulk data replacement in `git`_\nrepository, and now you want to deliver changes to remote database.\nThis not so easy matter could be solved with **Overhave** special\ntooling:\n\nYou are able to set necessary settings for your project:\n\n.. code-block:: bash\n\n    overhave sync run  # only update existing features\n    overhave sync run --create-db-features  # update + create new features\n    overhave sync run --pull-repository  # pull git repo and run sync\n\nYou are able to test this tool with **Overhave** demo mode.\nBy default, 3 features are created in demo database. Just try\nto change them or create new features and run synchronization\ncommand - you will get the result.\n\n.. code-block:: bash\n\n    overhave-demo sync-run  # or with \'--create-db-features\'\n\n**Overhave** supports validation of existing feature files.\nCommand try to parse features and fill defined feature info format.\nIf there is any problem, special error will be thrown.\n\n.. code-block:: bash\n\n    overhave sync validate-features\n    overhave sync validate-features --raise-if-nullable-id\n    overhave sync validate-features --pull-repository\n\nAnd yes, your are able to try it with demo mode:\n\n.. code-block:: bash\n\n    overhave-demo validate-features\n    overhave sync validate-features -r  # --raise-if-nullable-id\n\nCustom index\n------------\n\n**Overhave** gives an ability to set custom index.html file for rendering. Path\nto file could be set through environment as well as set with context:\n\n.. code-block:: python\n\n    admin_settings = OverhaveAdminSettings(\n        index_template_path="/path/to/index.html"\n    )\n\nAuthorization strategy\n----------------------\n\n**Overhave** provides several authorization strategies, declared by\n```AuthorizationStrategy``` enum:\n\n* `Simple` - strategy without real authorization.\n    Each user could use preferred name. This name will be used for user\n    authority. Each user is unique. Password not required.\n\n* `Default` - strategy with real authorization.\n    Each user could use only registered credentials.\n\n* `LDAP` - strategy with authorization using remote LDAP server.\n    Each user should use his LDAP credentials. LDAP\n    server returns user groups. If user in default \'admin\' group or his groups\n    list contains admin group - user will be authorized. If user already placed\n    in database - user will be authorized too. No one password stores.\n\nAppropriate strategy and additional data should be placed into\n```OverhaveAuthorizationSettings```, for example LDAP strategy could be\nconfigured like this:\n\n.. code-block:: python\n\n    auth_settings = OverhaveAuthorizationSettings(auth_strategy=AuthorizationStrategy.LDAP)\n    ldap_manager_settings = OverhaveLdapManagerSettings(ldap_admin_group="admin")\n\nS3 cloud\n--------\n\n**Overhave** implements functionality for *s3* cloud interactions, such as\nbucket creation and deletion, files uploading, downloading and deletion.\nThe framework provides an ability to store reports and other files in\nthe remote s3 cloud storage. You could enrich your environment with following\nsettings:\n\n.. code-block:: shell\n\n    OVERHAVE_S3_ENABLED=true\n    OVERHAVE_S3_URL=https://s3.example.com\n    OVERHAVE_S3_ACCESS_KEY=<MY_ACCESS_KEY>\n    OVERHAVE_S3_SECRET_KEY=<MY_SECRET_KEY>\n\nOptionally, you could change default settings also:\n\n.. code-block:: shell\n\n    OVERHAVE_S3_VERIFY=false\n    OVERHAVE_S3_AUTOCREATE_BUCKETS=true\n\nThe framework with enabled ```OVERHAVE_S3_AUTOCREATE_BUCKETS``` flag will create\napplication buckets in remote storage if buckets don\'t exist.\n\nAPI\n---\n**Overhave** has it\'s own application programming interface, based on\n`FastAPI`_.\n\n.. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/api_img.png\n  :width: 600\n  :align: center\n  :alt: Allure test-case report\n\n  **Overhave** openapi.json through `Swagger`_\n\nCurrent possibilities could be displayed through built-in\n`Swagger`_ - just run the API and open http://localhost:8000 in your\nbrowser.\n\n.. code-block:: bash\n\n    overhave api -p 8000\n\nInterface has authorization through `oauth2`_ scheme, so you should setup\n```OVERHAVE_API_AUTH_SECRET_KEY``` for usage.\n\nRight now, API implements types of resources:\n\n* `feature_tags`\n    get feature tag or get list of feature tags;\n* `features`\n    get features info by tag ID or tag value;\n* `test_users`\n    get test user info, specification, put new specification or delete\n    test user;\n* `test_runs`\n    get test run info or create test run with given parameters;\n* `emulations`\n    get emulation runs by test user id.\n\n------------\nContributing\n------------\n\nContributions are very welcome.\n\nPreparation\n-----------\n\nProject installation is very easy\nand takes just few prepared commands (`make pre-init` works only for Ubuntu;\nso you can install same packages for your OS manually):\n\n.. code-block:: shell\n\n    make pre-init\n    make init\n\nPackages management is provided by `Poetry`_.\n\nCheck\n-----\n\nTests can be run with `Tox`_. `Docker-compose`_ is used for other services\npreparation and serving, such as database. Simple tests and linters execution:\n\n.. code-block:: shell\n\n    make up\n    make test\n    make lint\n\nPlease, see `make` file and discover useful shortcuts. You could run tests\nin docker container also:\n\n.. code-block:: shell\n\n    make test-docker\n\nDocumentation build\n-------------------\n\nProject documentation could be built via `Sphinx`_ and simple `make` command:\n\n.. code-block:: shell\n\n    make build-docs\n\nBy default, the documentation will be built using `html` builder into `_build`\ndirectory.\n\n-------\nLicense\n-------\n\nDistributed under the terms of the `GNU GPLv2`_ license.\n\n------\nIssues\n------\n\nIf you encounter any problems, please report them here in section `Issues`\nwith a detailed description.\n\n.. _`Overhave`: https://github.com/TinkoffCreditSystems/overhave\n.. _`Pydantic`: https://github.com/samuelcolvin/pydantic\n.. _`Flask Admin`: https://github.com/flask-admin/flask-admin\n.. _`Ace`: https://github.com/ajaxorg/ace\n.. _`PyTest`: https://github.com/pytest-dev/pytest\n.. _`pytest-bdd`: https://github.com/pytest-dev/pytest-bdd\n.. _`Allure`: https://github.com/allure-framework/allure-python\n.. _`Allure CLI`: https://docs.qameta.io/allure/#_get_started\n.. _`Bitbucket`: https://www.atlassian.com/git\n.. _`GitLab`: https://about.gitlab.com\n.. _`python-gitlab`: https://python-gitlab.readthedocs.io\n.. _`SQLAlchemy`: https://github.com/sqlalchemy/sqlalchemy\n.. _`Walrus`: https://github.com/coleifer/walrus\n.. _`GoTTY`: https://github.com/yudai/gotty\n.. _`GNU GPLv2`: http://www.apache.org/licenses/LICENSE-2.0\n.. _`Tox`: https://github.com/tox-dev/tox\n.. _`Poetry`: https://github.com/python-poetry/poetry\n.. _`Docker-compose`: https://docs.docker.com/compose\n.. _`Typer`: https://github.com/tiangolo/typer\n.. _`Sphinx`: https://github.com/sphinx-doc/sphinx\n.. _`boto3`: https://github.com/boto/boto3\n.. _`git`: https://git-scm.com/\n.. _`FastAPI`: https://github.com/tiangolo/fastapi\n.. _`Swagger`: https://swagger.io\n.. _`oauth2`: https://oauth.net/2/\n.. _`context_example.rst`: https://github.com/TinkoffCreditSystems/overhave/blob/master/docs/includes/context_example.rst\n.. _`feature_example.rst`: https://github.com/TinkoffCreditSystems/overhave/blob/master/docs/includes/features_structure_example/feature_type_1/full_feature_example_en.feature\n',
     'author': 'Vladislav Mukhamatnurov',
     'author_email': 'livestreamepidemz@yandex.ru',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `overhave-3.8.4/PKG-INFO` & `overhave-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overhave
-Version: 3.8.4
+Version: 3.9.0
 Summary: Overhave - web-framework for BDD
 Author: Vladislav Mukhamatnurov
 Author-email: livestreamepidemz@yandex.ru
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

