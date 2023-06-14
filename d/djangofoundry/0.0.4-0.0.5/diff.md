# Comparing `tmp/djangofoundry-0.0.4.tar.gz` & `tmp/djangofoundry-0.0.5.tar.gz`

## Comparing `djangofoundry-0.0.4.tar` & `djangofoundry-0.0.5.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/.dockerignore
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/.prospector.yaml
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/Dockerfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/docker-compose.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/logging.conf
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/package.json
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/requirements.txt
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/.devcontainer/docker-compose.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/__init__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/__init__.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/urls.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/__init__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/angular.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/detail.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/generic.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/list.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/memory.py
--rw-r--r--   0        0        0    15504 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/responses.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/decorators/__init__.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/decorators/queryset_filter.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/decorators/retry.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/decorators/timeout.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/exceptions/__init__.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/exceptions/app.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/__init__.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/logging.py
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/progress.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/encoders/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/encoders/json.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/__init__.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/exceptions.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/hook.py
--rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/hooks.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/waypoint.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/meta/__init__.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/meta/constants.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/meta/types.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/queue/__init__.py
--rw-r--r--   0        0        0    14036 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/queue/queue.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/queue/signals.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/__init__.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/template.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/__init__.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/template.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/__init__.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/css.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/javascript.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/template.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/python/__init__.py
--rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/python/model.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/python/template.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/meta/__init__.py
--rw-r--r--   0        0        0     9232 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/meta/model.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/matching/__init__.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/matching/engine.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/matching/fuzzy/__init__.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/matching/fuzzy/thefuzz.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/mixins/__init__.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/mixins/dirtyfields.py
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/mixins/hasParams.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/mixins/hookable.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/mixins/jsonResponse.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/__init__.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/choices.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/manager.py
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/model.py
--rw-r--r--   0        0        0    53644 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/queryset.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/serializer.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/viewset.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/exceptions/__init__.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/exceptions/get.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/__init__.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/boolean.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/char.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/date.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/number.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/objects.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/relationships.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/options/__init__.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/options/request.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/README.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/__init__.py
--rw-r--r--   0        0        0    19911 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/app.py
--rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/db.py
--rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/lint.py
--rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/summarize.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/conf/sample-settings.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/utils/README.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/utils/__init__.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/utils/action.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/utils/exceptions.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/utils/settings.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/utils/types.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/signals/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/signals/abstract.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/templates/memory.html
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/templates/angular/base.html
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/templates/jinja/model.py.jinja
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/templatetags/__init__.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/templatetags/syntax_highlight.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/test_matching.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/controllers/__init__.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/controllers/test_mixins.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/decorators/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/decorators/test_timeout.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/helpers/__init__.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/helpers/test_hooks.py
--rw-r--r--   0        0        0     8781 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/helpers/test_queue.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/models/__init__.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/models/test_choices.py
--rw-r--r--   0        0        0    10267 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/models/test_queryset.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/.gitignore
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/LICENSE.md
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/README.md
--rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/.dockerignore
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/.prospector.yaml
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/Dockerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/docker-compose.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/logging.conf
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/package.json
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/.devcontainer/docker-compose.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/__init__.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/urls.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/angular.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/detail.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/generic.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/list.py
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/memory.py
+-rw-r--r--   0        0        0    15504 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/responses.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/decorators/__init__.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/decorators/queryset_filter.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/decorators/retry.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/decorators/timeout.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/exceptions/__init__.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/exceptions/app.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/__init__.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/logging.py
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/progress.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/encoders/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/encoders/json.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/__init__.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/exceptions.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/hook.py
+-rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/hooks.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/waypoint.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/meta/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/meta/constants.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/meta/types.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/queue/__init__.py
+-rw-r--r--   0        0        0    14036 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/queue/queue.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/queue/signals.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/__init__.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/template.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/__init__.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/template.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/__init__.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/css.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/javascript.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/template.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/python/__init__.py
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/python/model.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/python/template.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/meta/__init__.py
+-rw-r--r--   0        0        0     9232 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/meta/model.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/matching/__init__.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/matching/engine.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/matching/fuzzy/__init__.py
+-rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/matching/fuzzy/thefuzz.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/mixins/__init__.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/mixins/dirtyfields.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/mixins/hasParams.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/mixins/hookable.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/mixins/jsonResponse.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/__init__.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/choices.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/manager.py
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/model.py
+-rw-r--r--   0        0        0    53639 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/queryset.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/serializer.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/viewset.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/exceptions/__init__.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/exceptions/get.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/__init__.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/boolean.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/char.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/date.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/number.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/objects.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/relationships.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/options/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/options/request.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/README.md
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/__init__.py
+-rw-r--r--   0        0        0    20059 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/app.py
+-rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/db.py
+-rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/lint.py
+-rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/summarize.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/conf/sample-settings.yaml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/utils/README.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/utils/__init__.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/utils/action.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/utils/exceptions.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/utils/settings.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/utils/types.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/signals/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/signals/abstract.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/templates/memory.html
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/templates/angular/base.html
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/templates/jinja/model.py.jinja
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/templatetags/__init__.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/templatetags/syntax_highlight.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/test_matching.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/controllers/__init__.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/controllers/test_mixins.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/decorators/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/decorators/test_timeout.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/helpers/__init__.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/helpers/test_hooks.py
+-rw-r--r--   0        0        0     8781 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/helpers/test_queue.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/models/__init__.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/models/test_choices.py
+-rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/models/test_queryset.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/README.md
+-rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/PKG-INFO
```

### Comparing `djangofoundry-0.0.4/Dockerfile` & `djangofoundry-0.0.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/package.json` & `djangofoundry-0.0.5/package.json`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/.devcontainer/devcontainer.json` & `djangofoundry-0.0.5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/.devcontainer/docker-compose.yml` & `djangofoundry-0.0.5/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/urls.py` & `djangofoundry-0.0.5/src/djangofoundry/urls.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/controllers/angular.py` & `djangofoundry-0.0.5/src/djangofoundry/controllers/angular.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/controllers/detail.py` & `djangofoundry-0.0.5/src/djangofoundry/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/controllers/generic.py` & `djangofoundry-0.0.5/src/djangofoundry/controllers/generic.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/controllers/list.py` & `djangofoundry-0.0.5/src/djangofoundry/controllers/list.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/controllers/memory.py` & `djangofoundry-0.0.5/src/djangofoundry/controllers/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 class MemoryMonitorView(View):
 	"""
 	Display the current memory usage of the application
 	"""
 	template_name = 'memory.html'
 
 	def get(self, request, *args, **kwargs):
-		return render(request, self.template_name)
+		return render(request, self.template_name, *args, **kwargs)
+
 
 def memory_usage(request):
 	"""
 	Return the current memory usage of the application
 	"""
 	process = psutil.Process()
 	mem_info = process.memory_info()
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/controllers/responses.py` & `djangofoundry-0.0.5/src/djangofoundry/controllers/responses.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/decorators/queryset_filter.py` & `djangofoundry-0.0.5/src/djangofoundry/decorators/queryset_filter.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/decorators/retry.py` & `djangofoundry-0.0.5/src/djangofoundry/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/decorators/timeout.py` & `djangofoundry-0.0.5/src/djangofoundry/decorators/timeout.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/exceptions/app.py` & `djangofoundry-0.0.5/src/djangofoundry/exceptions/app.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/logging.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/progress.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/progress.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/__init__.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/exceptions.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/exceptions.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/hook.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/hook.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,38 +36,38 @@
 
 	@property
 	def executions(self):
 		"""
 		Indicates the number of times this hook has been run.
 
 		Represented as a property to discourage editing the executions variable.
-  		"""
+		"""
 		return self._executions
 
 	def __init__(self,
 			  name : str,
 			  action : Callable,
 			  namespace : str = DEFAULT_NAMESPACE,
 			  priority : int = DEFAULT_PRIORITY,
 			  max_executions : int = -1):
 		"""
 		Args:
 			name (str):
-   				The name of the hook
+				The name of the hook
 			action (Callable):
-   				The action to perform when the hook is run.
+				The action to perform when the hook is run.
 			namespace (str):
-   				The namespace of the hook (defaults to the DEFAULT_NAMESPACE constant)
+				The namespace of the hook (defaults to the DEFAULT_NAMESPACE constant)
 			priority (int):
 				The priority of the hook (defaults to the DEFAULT_PRIORITY constant).
 				Hooks execute in the order of their priority.
 				Lower priorities will execute first.
 			max_executions (int):
-   				The maximum number of times this hook can be run. Defaults to -1 (no maximum)
-  		"""
+				The maximum number of times this hook can be run. Defaults to -1 (no maximum)
+		"""
 		self.namespace = namespace
 		self.name = name
 		self.action = action
 		self.max_executions = max_executions
 		self.priority = priority
 
 		# Sanity checking
@@ -80,33 +80,33 @@
 
 		This is determined by checking the number of executions against max_executions.
 
 		Examples:
 			>>> hook = Hook('test', lambda: 1, max_executions = 1)
 			>>> hook.run()
 			>>> hook.run()
-   			Traceback (most recent call last):
+			Traceback (most recent call last):
 			...
 			MaxExecutionsError: Hook application.test has already been run 1 times.
-  		"""
+		"""
 		return self.executions < self.max_executions > -1
 
 	def run(self, *args, **kwargs) -> Tuple[bool, Any]:
 		"""
 		Request that the hook action be run if it is allowed to.
 
 		Args:
 			*args:
-   				Any positional arguments to pass to the action
+				Any positional arguments to pass to the action
 			**kwargs:
-   				Any keyword arguments to pass to the action
+				Any keyword arguments to pass to the action
 
 		Returns:
 			(bool, Any): Returns a boolean to indicate whether the action run, and the return value of the action (or None)
-  		"""
+		"""
 		# Check if we're allowed to run
 		if self.can_run() is False:
 			return (False, None)
 
 		# Run the action and capture its return value
 		result = self.action(*args, **kwargs)
 		# Indicate we ran and pass the result back
@@ -116,33 +116,33 @@
 		"""
 		Runs this hook action with the provided arguments, regardless of max_executions.
 
 		This is not the standard way of running a hook. Most hooks are run with Hook.request_run().
 
 		Args:
 			*args:
-   				Any positional arguments to pass to the action
+				Any positional arguments to pass to the action
 			**kwargs:
-   				Any keyword arguments to pass to the action
+				Any keyword arguments to pass to the action
 
 		Returns:
 			Any: Hooks may define their own return values
-  		"""
+		"""
 		# Increase the executions (perhaps beyond the max)
 		self._executions += 1
 
 		# Return whatever the hook action says to return
 		return self.action(*args, **kwargs)
 
 
 if __name__ == "__main__":
 	"""
 	This code is only called if this module is executed directly (i.e. outside of django)
 
 	Its purpose is to run basic unit tests to ensure the module operates the way we intend it to.
- 	"""
+	"""
 	# Import the doctest module, which runs tests based on Examples in our comments.
 	import doctest
 
 	# Run every test we can find in our comments.
 	# No output means success.
 	doctest.testmod()
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/hooks.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/hooks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 	Assists with registering and calling hooks for arbitrary points in the code.
 
 	This allows our software to be modular:
- 	addons can be included which modify core behavior of our software without subclassing or overriding anything.
+	addons can be included which modify core behavior of our software without subclassing or overriding anything.
 
 	Metadata:
 
 		File: hooks.py
 		Project: Django Foundry
 		Created Date: 02 Sep 2022
 		Author: Jess Mann
@@ -27,36 +27,36 @@
 from djangofoundry.helpers.hooks.meta import NamespaceMap, DEFAULT_NAMESPACE, DEFAULT_PRIORITY
 from djangofoundry.helpers.hooks.hook import Hook
 from djangofoundry.helpers.hooks.waypoint import Waypoint
 
 class Hooks:
 	"""
 	The Hooks class allows registration of modular hooks throughout the application.
- 	"""
+	"""
 	# A map of hooks in the format: {namespace: {name: list(Callable())}}
 	_hooks : NamespaceMap
 
 	@classmethod
 	def run(cls, name : str, namespace : str = DEFAULT_NAMESPACE, *args, **kwargs) -> Iterable[Any]:
 		"""
 		Run any hooks registered to this name and namespace.
 
 		Args:
 			name (str, optional):
-   				The name of the hook
+				The name of the hook
 			namespace (str, optional):
-   				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
+				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
 			*args:
 				Positional arguments to pass to the hook
 			**kwargs:
 				Named arguments to pass to the hook
 
 		Returns:
 			Iterable[Any]: Returns a list of all retur values for the hooks run.
-  		"""
+		"""
 		# Get all hooks that match this criteria
 		hooks : list[Hook] = cls.get(name=name, namespace=namespace)
 
 		# Sort the hooks by priority
 		hooks.sort(key = lambda x: x.priority, reverse=True)
 
 		# Initialize a list of all return values from each hook run
@@ -85,19 +85,19 @@
 		"""
 		Register a new hook to this name and namespace.
 
 		After being registered, the provided callable will be executed when Hook.run() is called.
 
 		Args:
 			name (str):
-   				The name of the hook
+				The name of the hook
 			action (Callable):
 				The callable function to execute when this hook is run.
 			namespace (str, optional):
-   				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
+				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
 			priority (int, optional):
 				The priority of the hook. Defaults to the DEFAULT_PRIORITY constant
 			max_executions (int, optional):
 				The maximum number of times this hook should be executed. Defaults to -1 (no maximum).
 
 		Returns:
 			None
@@ -114,50 +114,50 @@
 	@classmethod
 	def get(cls, name : Optional[str] = None, namespace : str = DEFAULT_NAMESPACE) -> list[Hook]:
 		"""
 		Get a list of hooks registered to this name and namespace.
 
 		Args:
 			name (str, optional):
-   				The name of the hook
+				The name of the hook
 			namespace (str, optional):
-   				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
+				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
 
 		Raises:
 			ValueError: If a name is specified, but namespace is None
 
 		Note:
 			If name is None, get all hooks registered to the entire namespace.
 			If name AND namespace are both None, get all hooks registered anywhere.
 			If namespace is None, but name is provided, raises a ValueError.
 
 		Returns:
 			int: The number of hooks registered to this name and namespace.
-  		"""
+		"""
 		# Grab all waypoints that match the criteria
 		waypoints = cls.get_waypoints(name, namespace)
 
 		# Return all hooks in every waypoint we found.
 		return [waypoint.hooks for waypoint in waypoints]
 
 
 	@classmethod
 	def has_waypoint(cls, name: str, namespace: str = DEFAULT_NAMESPACE) -> bool:
 		"""
 		Returns whether a waypoint exists at the given name and namespace.
 
 		Args:
 			name (str):
-   				The name of the hook
+				The name of the hook
 			namespace (str, optional):
-   				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
+				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
 
 		Returns:
 			bool: True if a waypoint exists here, False if no waypoint can be found with this name/namespace.
-  		"""
+		"""
 		# No waypoint registered because this name/namespace hasn't been defined.
 		if namespace not in cls._hooks or name not in cls._hooks[namespace]:
 			return False
 
 		# This name/namespace was defined, but no waypoint is there.
 		if cls._hooks[namespace][name] is None:
 			return False
@@ -169,21 +169,21 @@
 	@classmethod
 	def get_waypoint(cls, name: str, namespace: str = DEFAULT_NAMESPACE) -> Waypoint | None:
 		"""
 		Gets the waypoint at the specified name and namespace.
 
 		Args:
 			name (str):
-   				The name of the hook
+				The name of the hook
 			namespace (str, optional):
-   				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
+				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
 
 		Returns:
 			Waypoint | None: A waypoint, if one was registered. Otherwise None.
-  		"""
+		"""
 		# No waypoint registered because this name/namespace hasn't been defined.
 		if namespace not in cls._hooks or name not in cls._hooks[namespace]:
 			return None
 
 		# Return whatever happens to be there (i.e. a Waypoint or None)
 		return cls._hooks[namespace][name]
 
@@ -191,24 +191,24 @@
 	@classmethod
 	def get_waypoints(cls, name: Optional[str] = None, namespace: str = DEFAULT_NAMESPACE) -> Iterable[Waypoint]:
 		"""
 		Gets all waypoints matching the criteria passed in.
 
 		Args:
 			name (str, optional):
-   				The name of the waypoint. If None, returns all waypoints with any name.
+				The name of the waypoint. If None, returns all waypoints with any name.
 			namespace (str, optional):
-   				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
+				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
 
 		Returns:
 			Waypoint | None: A waypoint, if one was registered. Otherwise None.
 
 		Raises:
 			ValueError: If a name is specified, but namespace is None
-  		"""
+		"""
 		if namespace is None:
 			if name is None:
 				# No name or namespace, return all waypoints
 				return [names.values() for names in cls._hooks.values()]
 
 			# Name but no namespace, raise an error
 			raise ValueError(f'Requesting all waypoints with a name ({name}) but no namespace specified.')
@@ -223,42 +223,42 @@
 	@classmethod
 	def count(cls, name : Optional[str] = None, namespace : str = DEFAULT_NAMESPACE) -> int:
 		"""
 		Counts the number of hooks registered to this name and namespace.
 
 		Args:
 			name (str, optional):
-   				The name of the hook
+				The name of the hook
 			namespace (str, optional):
-   				The namespace to search for hooks.
-	   			To search for hooks with the default namespace, set this to the DEFAULT_NAMESPACE constant.
+				The namespace to search for hooks.
+				To search for hooks with the default namespace, set this to the DEFAULT_NAMESPACE constant.
 
 		Note:
 			If name is None, counts all hooks registered to the entire namespace.
 			If namespace is None, counts all hooks with the given name in any namespace.
 			If name AND namespace are both None, counts all hooks registered anywhere.
 
 		Returns:
 			int: The number of hooks registered to this name and namespace.
-  		"""
+		"""
 		# Allow get() to do the heavy lifting.
 		return len(cls.get(name, namespace))
 
 	@classmethod
 	def register_waypoint(
 			cls,
 			name : str,
 			namespace : str = DEFAULT_NAMESPACE,
 			positional_arguments : int = 0,
-	 		named_arguments : Optional[list[str]] = None,
-		 	return_type : Any = Any,
-		  	hooks : Optional[list[Hook]] = None) -> Waypoint:
+			named_arguments : Optional[list[str]] = None,
+			return_type : Any = Any,
+			hooks : Optional[list[Hook]] = None) -> Waypoint:
 		"""
 		Creates and registers a new waypoint.
-  		"""
+		"""
 		if named_arguments is None:
 			named_arguments = []
 		if hooks is None:
 			hooks = []
 
 		# Make sure one doesn't exist first.
 		if cls.has_waypoint(name=name, namespace=namespace):
@@ -284,24 +284,24 @@
 
 		This is used to determine what hook points are available to register hooks to.
 
 		TODO: [AUTO-369] Allow initializing metadata details about hook points for documentation
 
 		Args:
 			name (str, optional):
-   				The name of the hook
+				The name of the hook
 			namespace (str, optional):
-   				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
+				The namespace to search for hooks. defaults to the DEFAULT_NAMESPACE constant.
 			waypoint (Waypoint, optional):
 				The waypoint to set at this name/namespace if it does not already exist.
 				If waypoint is None, a new waypoint with no extra parameters will be created.
 
 		Returns:
 			None
-  		"""
+		"""
 		if namespace not in cls._hooks:
 			# initialize the namespace
 			cls._hooks[namespace] = {}
 
 		if name not in cls._hooks[namespace]:
 			# initialize the hook name by creating a new waypoint
 			if waypoint is not None:
@@ -314,14 +314,14 @@
 
 
 if __name__ == "__main__":
 	"""
 	This code is only called if this module is executed directly (i.e. outside of django)
 
 	Its purpose is to run basic unit tests to ensure the module operates the way we intend it to.
- 	"""
+	"""
 	# Import the doctest module, which runs tests based on Examples in our comments.
 	import doctest
 
 	# Run every test we can find in our comments.
 	# No output means success.
 	doctest.testmod()
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/waypoint.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/waypoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 	return_type : Any
 	hooks : list[Hook]
 
 	def __init__(self,
 			name : str,
 			namespace : str = DEFAULT_NAMESPACE,
 			positional_arguments : int = 0,
-	 		named_arguments : list[str] = list,
-		 	return_type : Any = Any,
-		  	hooks : list[Hook] = list):
+			named_arguments : list[str] = list,
+			return_type : Any = Any,
+			hooks : list[Hook] = list):
 		self.name = name
 		self.namespace = namespace
 		self.positional_arguments = positional_arguments
 		self.named_arguments = named_arguments
 		self.return_type = return_type
 		self.hooks = hooks
 
@@ -77,17 +77,17 @@
 			*args:
 				Position arguments to pass on to the hook
 			**kwargs:
 				Named arguments to pass on to the hook
 
 		Returns:
 			Iterable[Any]:
-   				Returns a list of all return values for the hooks run.
+				Returns a list of all return values for the hooks run.
 				This will actually be an iterable of self.return_type, but we can't typehint based on variables passed in during init.
-  		"""
+		"""
 		# Sort the hooks by priority
 		self.hooks.sort(key = lambda x: x.priority, reverse=True)
 
 		# Initialize a list of all return values from each hook run
 		results = []
 
 		# Run each one in order
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/meta/constants.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/meta/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 	This module defines constants that relate to our hook classes.
 
- 	These can be imported in other packages with minimal dependencies that could cause a circular import.
+	These can be imported in other packages with minimal dependencies that could cause a circular import.
 
 	Metadata:
 
 		File: constants.py
 		Project: Django Foundry
 		Created Date: 02 Sep 2022
 		Author: Jess Mann
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/meta/types.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/meta/types.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/queue/queue.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/queue/queue.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/queue/signals.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/queue/signals.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/render/template.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/render/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/template.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/css.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/css.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/javascript.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/javascript.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/template.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/python/model.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/python/model.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/python/template.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/python/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/helpers/render/meta/model.py` & `djangofoundry-0.0.5/src/djangofoundry/helpers/render/meta/model.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/matching/engine.py` & `djangofoundry-0.0.5/src/djangofoundry/matching/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 				The input_str to attempt to match
 			compare (str):
 				The string to compare against
 
 		Returns:
 			int:
 				The confidence that these two strings match.
-			 	1 - 100
+				1 - 100
 
 				100 means we are certain they match.
 				1 means we are certain they do not match.
 		"""
 
 	@abstractmethod
 	def partial_match( self, input_str : str, compare : str ) -> int:
@@ -87,15 +87,15 @@
 				The input_str to attempt to match
 			compare (str):
 				The string to compare against
 
 		Returns:
 			int:
 				The confidence that these two strings match.
-			 	1 - 100
+				1 - 100
 
 				100 means we are certain they match.
 				1 means we are certain they do not match.
 		"""
 
 	@abstractmethod
 	def token_match( self, input_str : str, compare : str ) -> int:
@@ -110,15 +110,15 @@
 				The input_str to attempt to match
 			compare (str):
 				The string to compare against
 
 		Returns:
 			int:
 				The confidence that these two strings match.
-			 	1 - 100
+				1 - 100
 
 				100 means we are certain they match.
 				1 means we are certain they do not match.
 		"""
 
 	@abstractmethod
 	def token_partial_match( self, input_str : str, compare : str ) -> int:
@@ -133,12 +133,12 @@
 				The input_str to attempt to match
 			compare (str):
 				The string to compare against
 
 		Returns:
 			int:
 				The confidence that these two strings match.
-			 	1 - 100
+				1 - 100
 
 				100 means we are certain they match.
 				1 means we are certain they do not match.
 		"""
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/matching/fuzzy/thefuzz.py` & `djangofoundry-0.0.5/src/djangofoundry/matching/fuzzy/thefuzz.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 				The input_str to attempt to match
 			compare (str):
 				The string to compare against
 
 		Returns:
 			int:
 				The confidence that these two strings match.
-			 	1 - 100
+				1 - 100
 
 				100 means we are certain they match.
 				1 means we are certain they do not match.
 		"""
 		return fuzz.ratio(input_str, compare)
 
 	def partial_match( self, input_str : str, compare : str ) -> int:
@@ -99,15 +99,15 @@
 				The input_str to attempt to match
 			compare (str):
 				The string to compare against
 
 		Returns:
 			int:
 				The confidence that these two strings match.
-			 	1 - 100
+				1 - 100
 
 				100 means we are certain they match.
 				1 means we are certain they do not match.
 		"""
 		return fuzz.partial_ratio(input_str, compare)
 
 	def token_match( self, input_str : str, compare : str ) -> int:
@@ -122,15 +122,15 @@
 				The input_str to attempt to match
 			compare (str):
 				The string to compare against
 
 		Returns:
 			int:
 				The confidence that these two strings match.
-			 	1 - 100
+				1 - 100
 
 				100 means we are certain they match.
 				1 means we are certain they do not match.
 		"""
 		return fuzz.token_sort_ratio(input_str, compare)
 
 	def token_partial_match( self, input_str : str, compare : str ) -> int:
@@ -145,13 +145,13 @@
 				The input_str to attempt to match
 			compare (str):
 				The string to compare against
 
 		Returns:
 			int:
 				The confidence that these two strings match.
-			 	1 - 100
+				1 - 100
 
 				100 means we are certain they match.
 				1 means we are certain they do not match.
 		"""
 		return fuzz.token_set_ratio(input_str, compare)
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/mixins/dirtyfields.py` & `djangofoundry-0.0.5/src/djangofoundry/mixins/dirtyfields.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/mixins/hasParams.py` & `djangofoundry-0.0.5/src/djangofoundry/mixins/hasParams.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,71 +39,71 @@
 	A mixin for Controllers to handle parameters passed in via url.
 
 	This is used on several extensions of base django controllers, as well as django rest api viewsets.
 
 	Attributes:
 		kwargs (Iterable[dict]):
 			The (unsanitized) parameters passed to us via url.
-  			NOTE: This is defined by django controllers and overrides our definition. We include it here only for standalone type checking purposes.
+			NOTE: This is defined by django controllers and overrides our definition. We include it here only for standalone type checking purposes.
 	"""
 	kwargs: Iterable[dict]
 
 	def get_param(self, name : str, sanitize : bool = True, required : bool = False) -> str | None:
 		"""
 		Convenience method for accessing self.kwargs[] to rerieve data passed in the url.
 
 		Attributes:
 			name (str):
-   				The name of the parameter
+				The name of the parameter
 			sanitize (bool):
 				If False, return the user input unmodified. Otherwise, sanitize the user input (default).
 			required (bool):
-   				If true, we will throw an exception if the parameter is missing. If false, we return null for missing parameters.
+				If true, we will throw an exception if the parameter is missing. If false, we return null for missing parameters.
 
 		Returns:
 			str: The value of the parameter, or None if not found.
 
 		Raises:
 			ReferenceError: If the parameter is missing and required is True.
-  		"""
+		"""
 		# If it's found, then return it.
 		if name in self.kwargs:
 			if sanitize is False:
 				# Return it unsanitized
 				logger.warning(f'Returning user input {name} unsanitized.')
 				return self.kwargs[name]
-			else:
-				# Unless explicitly False, return a sanitized string.
-				return self.sanitize_str(self.kwargs[name])
+			
+			# Unless explicitly False, return a sanitized string.
+			return self.sanitize_str(self.kwargs[name])
 
 		# Not found, determine what to do...
 		if required is True:
 			raise ReferenceError(f"Required param {name} is missing.")
 
 		return None
 
 	def get_required_param(self, name : str, sanitize : bool = True) -> str:
 		"""
 		Retrieves data passed in the url.
 
 		Convenience method for accessing get_param(name,True) and ensuring the return value is a str.
 
-  		Attributes:
+		Attributes:
 			name (str):
-   				The name of the parameter
+				The name of the parameter
 			sanitize (bool):
 				If False, return the user input unmodified. Otherwise, sanitize the user input (default).
 
 		Returns:
 			str: The value of the parameter
 
 		Raises:
 			ReferenceError: If the parameter is missing
 			TypeError: If the parameter is found but is None
-  		"""
+		"""
 		value = self.get_param(name, sanitize=sanitize, required=True)
 
 		# This should never happen, because required=True should throw a ReferenceError if the value is null.
 		# This check is here for future proofing.
 		if value is None:
 			raise TypeError(f"Internal error: required param {name} is None.")
 
@@ -153,24 +153,24 @@
 
 		This is handled by django in the url, but we do it here as well to future proof against unexpected changes.
 
 		If no sanitizing is done at all (by django or by us), it could conceievably open us up to injection attacks.
 
 		Args:
 			value (str):
-   				The value of the user input string to sanitize.
+				The value of the user input string to sanitize.
 			param_type (str|int):
-   				A variable type. This function currently supports string and int.
+				A variable type. This function currently supports string and int.
 
 		Returns:
 			str | int: The sanitized value
 
 		Raises:
 			ValueError: If param_type is not a supported type.
-  		"""
+		"""
 		match param_type:
 			case str():
 				return self.sanitize_str(value)
 			case int():
 				return self.sanitize_int(value)
 
 		raise ValueError(f"Unsupported type {T}")
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/mixins/hookable.py` & `djangofoundry-0.0.5/src/djangofoundry/mixins/hookable.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/mixins/jsonResponse.py` & `djangofoundry-0.0.5/src/djangofoundry/mixins/jsonResponse.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/models/choices.py` & `djangofoundry-0.0.5/src/djangofoundry/models/choices.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/models/manager.py` & `djangofoundry-0.0.5/src/djangofoundry/models/manager.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/models/model.py` & `djangofoundry-0.0.5/src/djangofoundry/models/model.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/models/queryset.py` & `djangofoundry-0.0.5/src/djangofoundry/models/queryset.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 from statsmodels.tsa.seasonal import seasonal_decompose
 from statsmodels.tsa.stattools import grangercausalitytests
 from scipy import stats
 import pandas as pd
 import numpy as np
 # Django Imports
 from django.db.models import (
-	Sum, Count, Q, Avg, Min, Max, StdDev, ExpressionWrapper, F, 
-	FloatField, IntegerField, DecimalField, BigIntegerField, PositiveIntegerField, 
+	Sum, Count, Q, Avg, Min, Max, StdDev, ExpressionWrapper, F,
+	FloatField, IntegerField, DecimalField, BigIntegerField, PositiveIntegerField,
 	PositiveSmallIntegerField, SmallIntegerField, DurationField, PositiveBigIntegerField
 )
 from django.db.models.query import RawQuerySet
 # Django extensions
 import auto_prefetch
 # App Imports
 
@@ -546,15 +546,15 @@
 		'''
 		# Get the min and max of the field
 		min_value = self.aggregate(Min(y_field_name))[f"{y_field_name}__min"]
 		max_value = self.aggregate(Max(y_field_name))[f"{y_field_name}__max"]
 
 		# Get the distribution
 		distribution = (self.values(x_field_name, y_field_name).annotate(bin=ExpressionWrapper(F(y_field_name) - min_value, output_field=IntegerField()) // ((max_value - min_value) // bins)).values(x_field_name,
-																																														   					 "bin").annotate(count=Count("bin")).order_by(x_field_name, "bin"))
+																																																			 "bin").annotate(count=Count("bin")).order_by(x_field_name, "bin"))
 
 		# Convert the distribution to a dictionary
 		distribution_dict = {}
 		for result in distribution:
 			if result[x_field_name] not in distribution_dict:
 				distribution_dict[result[x_field_name]] = {}
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/models/serializer.py` & `djangofoundry-0.0.5/src/djangofoundry/models/serializer.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/models/viewset.py` & `djangofoundry-0.0.5/src/djangofoundry/models/viewset.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/models/exceptions/get.py` & `djangofoundry-0.0.5/src/djangofoundry/models/exceptions/get.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/models/fields/__init__.py` & `djangofoundry-0.0.5/src/djangofoundry/models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/models/fields/char.py` & `djangofoundry-0.0.5/src/djangofoundry/models/fields/char.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,35 +52,35 @@
 				 max_length : int = 18,
 				 unique	 : bool = True,
 				 null	   : bool = False,
 				 blank	  : bool = False,
 				 editable   : bool = False,
 				 **kwargs):
 		# Call the parent init function first
-		super().__init__(max_length  = max_length,
-								unique	  = unique,
-								null		= null,
-								blank	   = blank,
-								editable	= editable,
+		super().__init__(max_length 	 = max_length,
+								unique	 = unique,
+								null	 = null,
+								blank 	 = blank,
+								editable = editable,
 								**kwargs)
 
 class GuidField(CharField):
 	"""
 	A charfield that is used for storing GUIDs (UUID v4)
 	"""
 	def __init__(self, *,
-				 max_length : int = 38,
-				 unique	 : bool = True,
-				 null	   : bool = False,
-				 blank	  : bool = False,
-				 editable   : bool = False,
+				 max_length : int 	= 38,
+				 unique	 : bool 	= True,
+				 null : bool 		= False,
+				 blank : bool 		= False,
+				 editable : bool 	= False,
 				 **kwargs):
 		'''
 		Redefine init to only accept named args
 		'''
 		# Call the parent init function first
-		super().__init__(max_length  = max_length,
-								unique	  = unique,
-								null		= null,
-								blank	   = blank,
-								editable	= editable,
+		super().__init__(max_length		 = max_length,
+								unique	 = unique,
+								null	 = null,
+								blank	 = blank,
+								editable = editable,
 								**kwargs)
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/models/fields/date.py` & `djangofoundry-0.0.5/src/djangofoundry/models/fields/date.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/models/fields/number.py` & `djangofoundry-0.0.5/src/djangofoundry/models/fields/number.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/models/fields/objects.py` & `djangofoundry-0.0.5/src/djangofoundry/models/fields/objects.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/models/fields/relationships.py` & `djangofoundry-0.0.5/src/djangofoundry/models/fields/relationships.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/scripts/__init__.py` & `djangofoundry-0.0.5/src/djangofoundry/scripts/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 		Modified By: Jess Mann
 
 		-----
 
 		Copyright (c) 2022 Jess Mann
 """
 from djangofoundry.scripts.utils import (
-    EnumAction,
-    Settings,
-    AppException,
-    FileEmptyError,
-    DbError,
-    DbConnectionError,
-    DbStartError,
-    UnsupportedCommandError
+	EnumAction,
+	Settings,
+	AppException,
+	FileEmptyError,
+	DbError,
+	DbConnectionError,
+	DbStartError,
+	UnsupportedCommandError
 )
 from djangofoundry.scripts.app import App
 from djangofoundry.scripts.db import Db
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/scripts/app.py` & `djangofoundry-0.0.5/src/djangofoundry/scripts/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 
 		Copyright (c) 2022 Jess Mann
 """
 #!/usr/bin/env python
 
 # Generic imports
 from __future__ import annotations
-import argparse, textwrap, os, re, sys
+import argparse
+import os
+import re
+import sys
 import platform
 import shutil
 from enum import Enum
 import subprocess
 from typing import Any, Callable, Optional
 import json
 import getpass
@@ -89,15 +92,15 @@
 		self.author_name = author_name or getpass.getuser()
 		self.settings = settings
 
 	@property
 	def command(self) -> Actions:
 		"""
 		Get the currently executing command. This is typically set by self.perform()
-  		"""
+		"""
 		if self._command is None:
 			raise ValueError('Command has not been set yet')
 		return self._command
 
 	def django_setup(self) -> str:
 		"""
 		Setup the Django project and app with given names.
@@ -122,26 +125,26 @@
 		Returns:
 			A string indicating the status of the setup.
 		"""
 		os.makedirs(self.frontend_dir, exist_ok=True)
 		os.chdir(self.frontend_dir) # Switch to the frontend directory before running Angular commands
 		self.run_subprocess(["npm", "init", "-y"])
 
-		with open('package.json') as f:
+		with open('package.json', encoding="utf-8") as f:
 			data = json.load(f)
 
 		data['name'] = self.project_name
 		data['version'] = '1.0.0'
 		data['description'] = f'{self.project_name} - an Angular-Django project'
 		data['main'] = 'index.js'
 		data['scripts'] = { 'test': 'echo "Error: no test specified" && exit 1' }
 		data['author'] = getpass.getuser()
 		data['license'] = 'BSD-3-Clause'
 
-		with open('package.json', 'w') as f:
+		with open('package.json', 'w', encoding="utf-8") as f:
 			json.dump(data, f, indent=2)
 
 		self.run_subprocess(["npm", "install"])
 		self.run_subprocess(["npm", "install", "@angular/cli"])
 		self.run_subprocess(["ng", "new", self.project_name, "--skip-git", "--skip-install"])
 		os.chdir(self.directory) # Switch back to the original directory
 		return f"Angular setup completed for {self.project_name}"
@@ -162,26 +165,26 @@
 		Attempt to install npm on the system.
 
 		Returns:
 			A string indicating the status of the installation.
 		"""
 		os_name = platform.system()
 
-		if os_name == 'Linux' or os_name == 'Darwin':
+		if os_name in ['Linux', 'Darwin']:
 			try:
 				self.run_subprocess(['curl', 'https://www.npmjs.com/install.sh', '|', 'sh'])
 				return "npm installed successfully on Linux or macOS"
 			except subprocess.CalledProcessError as process_e:
-				raise EnvironmentError(f"Error installing npm on Linux or macOS: {process_e}")
+				raise EnvironmentError(f"Error installing npm on Linux or macOS: {process_e}") from process_e
 		elif os_name == 'Windows':
 			try:
 				self.run_subprocess(['powershell', '-Command', 'iex (New-Object Net.WebClient).DownloadString("https://www.npmjs.com/install.ps1")'])
 				return "npm installed successfully on Windows"
 			except subprocess.CalledProcessError as process_e:
-				raise EnvironmentError(f"Error installing npm on Windows: {process_e}")
+				raise EnvironmentError(f"Error installing npm on Windows: {process_e}") from process_e
 		else:
 			raise EnvironmentError("Unsupported operating system")
 
 
 	def check_environment(self) -> None:
 		"""
 		Check the environment to make sure the setup will run smoothly.
@@ -216,18 +219,18 @@
 		logger.debug("RAM check passed.")
 
 		logger.info("All environment checks passed.")
 
 	def confirm_setup(self) -> None:
 		"""
 		Confirm the setup has been completed successfully.
-		
+
 		Returns:
 			None
-			
+
 		Raises:
 			EnvironmentError: If the setup was not completed successfully.
 		"""
 		# Check for package dependencies
 		dependencies = ["npm"]
 		for dependency in dependencies:
 			if not shutil.which(dependency):
@@ -235,16 +238,16 @@
 		logger.debug("npm dependency check passed.")
 
 		# Check for pip dependencies via imports
 		dependencies = ["django", "psutil"]
 		for dependency in dependencies:
 			try:
 				__import__(dependency)
-			except ImportError:
-				raise EnvironmentError(f"The {dependency} package isn't available. Please install it.")
+			except ImportError as ie:
+				raise EnvironmentError(f"The {dependency} package isn't available. Please install it.") from ie
 		logger.debug("python dependency check passed.")
 
 	def setup(self) -> None:
 		"""
 		Setup both Django and Angular projects and apps with given names.
 
 		Returns:
@@ -281,32 +284,32 @@
 		# Run the django dev server in a subprocess, and pipe output to the command.stdout property.
 		try:
 			# Clear the output buffer for this run
 			self._output_buffer = ''
 
 			# Subprocess wants each arg as a separate entry in a list... combine args into our known command string.
 			script_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), '../manage.py')
-			input_str = ['python', script_path, f'{command}'] + [arg for arg in args]
-			process = subprocess.Popen(input_str, stdout=subprocess.PIPE, encoding="utf-8")
+			input_str = ['python', script_path, f'{command}'] + list(args)
 
-			if not process.stdout:
-				raise ValueError('No output from subprocess')
-
-			# Stdout is a stream, so this acts like a while() loop as long as django is running.
-			for line in process.stdout:
-				# Pass all output to our handler, which may trigger events.
-				self.handle_output(line)
-
-			# Wait for output that may not have hit the stream yet. (TODO: This may not be necessary?)
-			process.wait()
-
-			# Issue our callback, as we're now finished.
-			if callback is not None:
-				logger.debug('Issuing callback on completion')
-				callback(process)
+			with subprocess.Popen(input_str, stdout=subprocess.PIPE, encoding="utf-8") as process:
+				if not process.stdout:
+					raise ValueError('No output from subprocess')
+
+				# Stdout is a stream, so this acts like a while() loop as long as django is running.
+				for line in process.stdout:
+					# Pass all output to our handler, which may trigger events.
+					self.handle_output(line)
+
+				# Wait for output that may not have hit the stream yet. (TODO: This may not be necessary?)
+				process.wait()
+
+				# Issue our callback, as we're now finished.
+				if callback is not None:
+					logger.debug('Issuing callback on completion')
+					callback(process)
 
 		except KeyboardInterrupt:
 			# Allow terminating the dev server from the command line.
 			logger.info('Stopping server...')
 
 		return self._output_buffer
 
@@ -319,22 +322,21 @@
 				A list of strings to pass to the subprocess.
 			print_output (bool):
 				Whether to print the output of the subprocess to the console.
 
 		Raises:
 			ValueError: If the subprocess has no output.
 		"""
-		process = subprocess.Popen(cmd_list, stdout=subprocess.PIPE, encoding="utf-8")
-		if not process.stdout:
-			raise ValueError('No output from subprocess')
-
-		for line in process.stdout:
-			self.handle_output(line, print_output)
-		process.wait()
+		with subprocess.Popen(cmd_list, stdout=subprocess.PIPE, encoding="utf-8") as process:
+			if not process.stdout:
+				raise ValueError('No output from subprocess')
 
+			for line in process.stdout:
+				self.handle_output(line, print_output)
+			process.wait()
 
 	def run_typical_command(self, command : Actions, callback : Optional[Callable] = None, *args, **kwargs) -> str:
 		"""
 		Runs a command that requires our normal tool suite (such as the DB) to be running.
 
 		Args:
 			command (str):
@@ -392,35 +394,35 @@
 		return False
 
 	def sync_browser(self):
 		"""
 		Start a process to sync the browser with the application state.
 
 		We currently use browser-sync for this. When our app files change, the browser will automatically refresh the page.
-  		"""
+		"""
 		# Subprocess wants each arg as a separate entry in a list... combine args into our known command string.
 		input_str = ['npm', 'run', 'serve']
 		logger.debug('Starting browsersync')
-		process = subprocess.Popen(input_str, stdout=subprocess.PIPE, encoding="utf-8", shell=True)
+		with subprocess.Popen(input_str, stdout=subprocess.PIPE, encoding="utf-8", shell=True) as process:
 
-		if not process.stdout:
-			raise ValueError('No output from subprocess')
+			if not process.stdout:
+				raise ValueError('No output from subprocess')
 
-		# Stdout is a stream, so this acts like a while() loop as long as django is running.
-		for line in process.stdout:
-			# Pass all output to our handler, which may trigger events.
-			self.handle_output(line)
+			# Stdout is a stream, so this acts like a while() loop as long as django is running.
+			for line in process.stdout:
+				# Pass all output to our handler, which may trigger events.
+				self.handle_output(line)
 
-		# Wait for output that may not have hit the stream yet. (TODO: This may not be necessary?)
-		process.wait()
+			# Wait for output that may not have hit the stream yet. (TODO: This may not be necessary?)
+			process.wait()
 
 	def on_django_started(self) -> None:
 		"""
 		Called when the django dev server is fully started.
-  		"""
+		"""
 		# If we're trying to start our app, then run our next action
 		if self.command == Actions.START:
 			self.sync_browser()
 
 	def handle_output(self, line : str, print_output: bool = True) -> None:
 		"""
 		Called for each line of input from django.
@@ -451,15 +453,15 @@
 		Args:
 			command (Actions): The action to perform.
 			page_name (str): The name of the page to create.
 			model_name (str): The name of the model to create.
 
 		Returns:
 			Any: The result of the action.
-  		"""
+		"""
 		# Save the command for later
 		self._command = command
 
 		# Determine what method to run.
 		match command:
 			case Actions.START:
 				# Start our entire app
@@ -518,16 +520,16 @@
 			None
 		"""
 		try:
 			self.create_angular_component(page_name)
 			self.setup_routing(page_name)
 			self.create_django_controller(page_name)
 			logging.info(f"Successfully created new page '{page_name}' in Django and Angular.")
-		except Exception as e:
-			logging.error(f"Failed to create new page '{page_name}': {e}")
+		except Exception as new_page_exception:
+			logging.error(f"Failed to create new page '{page_name}': {new_page_exception}")
 
 	def create_angular_component(self, page_name: str) -> None:
 		"""
 		Create a new Angular component.
 
 		Args:
 			page_name (str): The name of the page to create.
@@ -585,16 +587,16 @@
 			None
 		"""
 		controllers_dir = "backend/controllers"
 		os.makedirs(controllers_dir, exist_ok=True)
 
 		controller_file = os.path.join(controllers_dir, f"{page_name}.py")
 		try:
-			with open(controller_file, "w") as file:
-				file.write(f"from django.shortcuts import render\n\n")
+			with open(controller_file, "w", encoding="utf-8") as file:
+				file.write("from django.shortcuts import render\n\n")
 				file.write(f"def {page_name}_view(request):\n")
 				file.write(f"    return render(request, '{page_name}.html')\n")
 		except IOError as ioe:
 			logging.error(f"Failed to create Django controller '{page_name}': {ioe}")
 			raise
 
 	def create_new_model(self, model_name: str) -> None:
@@ -646,15 +648,15 @@
 	if result is not None:
 		print(f'App returned ({result})')
 
 if __name__ == '__main__':
 	try:
 		main()
 	except KeyboardInterrupt:
-		logger.info(f'Shutting down server...')
+		logger.info('Shutting down server...')
 		sys.exit(0)
 	except DbStartError:
 		logger.error('Could not start DB. Cannot continue')
 		sys.exit(0)
 	except EnvironmentError as env_error:
 		logger.error(f'Cannot run script in the current environment. {env_error}')
 		sys.exit(0)
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/scripts/db.py` & `djangofoundry-0.0.5/src/djangofoundry/scripts/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,28 +77,28 @@
 		Sets the log path. Assumes that input_path is user input and sanitizes it accordingly.
 
 		Args:
 			user_input_path (str): The path provided via user input to sanitize and set.
 
 		Returns:
 			None
-  		"""
+		"""
 		self._log_path = self.sanitize_path(user_input_path)
 
 	@data_path.setter
 	def data_path(self, user_input_path : str) -> None:
 		"""
 		Sets the data directory path. Assumes that input_path is user input and sanitizes it accordingly.
 
 		Args:
 			user_input_path(str): The path provided via user input to sanitize and set.
 
 		Returns:
 			None
-  		"""
+		"""
 		self._data_path = self.sanitize_path(user_input_path)
 
 	def __init__(self, data_path: str = DEFAULT_DATA_PATH, log_path: str = DEFAULT_LOG_PATH):
 		"""
 		Sets up our Db object with config options we'll use for this run.
 
 		Args:
@@ -112,15 +112,15 @@
 				Note: This is sanitized and only accepts these characters: a-zA-Z0-9/_.-
 				On windows, this also accepts colons and backslashes.
 				Defaults to the DEFAULT_LOG_PATH constant.
 
 		Raises:
 			ValueError: If the config options provided are not valid, or the files they reference are not found.
 			FileNotFoundError: If the postgres executable cannot be found.
-  		"""
+		"""
 		# Validation
 		if not os.path.isdir(data_path):
 			raise ValueError(f'Data path not found: "{data_path}"')
 		if not os.path.isfile(log_path):
 			raise ValueError(f'Log path not found: "{log_path}"')
 		if which(EXE) is None:
 			raise FileNotFoundError(f'DB executable not found. Is "{EXE}" in your path?')
@@ -136,48 +136,48 @@
 		"""
 		Starts the PostgresSQL server (if it is not running) and prints all output to stdout.
 
 		If the server is already running, prints a message indicating so, but does NOT attempt to restart.
 
 		Returns:
 			int: The exit code returned from executing the postgres command (pg_ctl), or -1 if the server is already running.
-  		"""
+		"""
 		# If we're already running, then just return right away.
 		if self.is_running():
 			print("Postgres server already running")
 			return -1
 
 		# Okay, not running. Try starting it with subprocess.run
 		return subprocess.run([EXE, '-D', self.data_path, '-l', self.log_path, 'start'], check=True).returncode
 
 	def restart(self) -> int:
 		"""
 		Restarts the PostgresSQL server and prints all output to stdout.
 
 		Returns:
 			int: The exit code returned from executing the postgres command (pg_ctl)
-  		"""
+		"""
 		return subprocess.run([EXE, '-D', self.data_path, '-l', self.log_path, 'restart'], check=True).returncode
 
 	def stop(self) -> int:
 		"""
 		Stops the PostgresSQL server and prints all output to stdout.
 
 		Returns:
 			int: The exit code returned from executing the postgres command (pg_ctl)
-  		"""
+		"""
 		return subprocess.run([EXE, '-D', self.data_path, '-l', self.log_path, 'stop'], check=True).returncode
 
 	def status(self) -> int:
 		"""
 		Checks the status of the postgres server and prints all output to stdout.
 
 		Returns:
 			int: The exit code returned from executing the postgres command (pg_ctl)
-  		"""
+		"""
 		return subprocess.run([EXE, '-D', self.data_path, '-l', self.log_path, 'status'], check=True).returncode
 
 	def check_errors(self) -> int:
 		"""
 		Checks the postgres server for errors and prints all output to stdout.
 		"""
 		cmd = ['psql', '-U', self.user, '-d', self.database, '-c', "SELECT * FROM pg_stat_database_conflicts WHERE datname = current_database();"]
@@ -236,37 +236,37 @@
 		Determines if the postgres server is running, without printing anything to stdout.
 
 		Returns:
 			bool: True if the server is running, False otherwise.
 
 		Raises:
 			FileNotFoundError: If postgres is not able to find the data directory
-  		"""
+		"""
 		# Create a child process, supressing output
 		child = subprocess.run([EXE, '-D', self.data_path, 'status'], stdout = subprocess.PIPE, check=True)
 
 		"""
-  		Postgres returns exit code 3 if the server is NOT running, and 4 on error. It returns 0 otherwise.
+		Postgres returns exit code 3 if the server is NOT running, and 4 on error. It returns 0 otherwise.
 
 		See here: https://www.postgresql.org/docs/current/app-pg-ctl.html
 			status mode checks whether a server is running in the specified data directory. If it is,
-	  		the server's PID and the command line options that were used to invoke it are displayed.
+			the server's PID and the command line options that were used to invoke it are displayed.
 			If the server is not running, pg_ctl returns an exit status of 3.
-		 	If an accessible data directory is not specified, pg_ctl returns an exit status of 4.
+			If an accessible data directory is not specified, pg_ctl returns an exit status of 4.
 		"""
 		if child.returncode == 4:
 			raise FileNotFoundError(f'Postgres is not able to find the data directory: {self.data_path}')
 		return not child.returncode
 
 	def sanitize_path(self, user_input_path : str) -> str:
 		"""
 		Takes arbitrary user input, and sanitizes it to prevent injection attacks.
 
 		NOTE: The return value from this function will generally be passed directly to the command line,
-  		so we must be especially careful with what we return.
+		so we must be especially careful with what we return.
 
 		Args:
 			user_input_path (str): The user input to turn into a path
 
 		Returns:
 			str: The sanitized path
 		"""
@@ -310,55 +310,55 @@
 		Turns an option into a string representation
 		"""
 		return self.value
 
 
 if __name__ == '__main__':
 	"""
- 		This code is only run when this script is called directly (i.e. python bin/db.py)
-   	"""
+		This code is only run when this script is called directly (i.e. python bin/db.py)
+	"""
 
 	# Setup the basic configuration for the parser
 	parser = argparse.ArgumentParser(
 			formatter_class=argparse.RawTextHelpFormatter,
-	 		description=textwrap.dedent("""
+			description=textwrap.dedent("""
 				Interact with the application's local DB
 			"""),
 			epilog="",
 	)
 
 	# Define the arguments we will accept from the command line.
 	parser.add_argument('action',
-					 type=Actions,
-					 action=EnumAction,
-					 help=textwrap.dedent("""\
+					type=Actions,
+					action=EnumAction,
+					help=textwrap.dedent("""\
 						Start the local application DB
 
 						status: check the DB status
 						start: start the DB (if it is not already running)
 						restart: stop the DB (if it is running) and start it again.
 						stop: stop the DB (if it is running)
 						check_errors: check for errors in the DB
 						repair_errors: repair errors in the DB
 						analyze: analyze the DB
 						dead_rows: check for dead rows in the DB
 						long_queries: check for long running queries in the DB
 						locks: check for locks in the DB
 						manage: manage the DB, restarting it if it is not running
-					 """))
+					"""))
 	parser.add_argument('-l', '--log',
-					 	type=str,
+						type=str,
 						metavar='path',
 						default=DEFAULT_LOG_PATH,
-	  					help="Path to the log file for the DB.")
+						help="Path to the log file for the DB.")
 	parser.add_argument('-d', '--data',
-					 	type=str,
+						type=str,
 						metavar='path',
 						default=DEFAULT_DATA_PATH,
-	  					help="Path to the data directory for postgres.")
+						help="Path to the data directory for postgres.")
 
 	# Parse the arguments provided to our script from the command line
 	# These are used as attributes. For example: options.action
 	options = parser.parse_args()
 
 	try:
 		# Instantiate a new DB object based on our arguments
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/scripts/lint.py` & `djangofoundry-0.0.5/src/djangofoundry/scripts/lint.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 import re
 import glob
 import yaml
 import openai
 from tqdm import tqdm
 
 class ChatGPTBugFixer:
-	def __init__(self, api_key, project_path):
+	def __init__(self, api_key, args):
 		openai.api_key = api_key
-		self.project_path = project_path
+		self.args = args
+		self.project_path = args.path
 		self.max_chars = 10000
 
 	def strip_comments(self, code : str) -> str:
 		# Strip comments beginning with a hash
 		code = re.sub(r"(?m)^\s*#.*\n?", "", code)
 
 		# Strip comments beginning with a triple quote
@@ -79,25 +80,25 @@
 		code = self.lint_code(code)
 
 		return code
 
 	def submit_code_to_chatgpt(self, code, file_path) -> str:
 		try:
 			response = openai.ChatCompletion.create(
-				model="gpt-4",
+				model = "gpt-4",
 				messages = [
-					{"role": "system", "content": "Your job is to identify bugs in python code and suggest improvements, adhering to modern best "+
-	  											  "practices, such as DRY. Review the code supplied and list specific changes to the code. If "+
-												  "functionality can be added to the code, suggest them. Use the following format for your "+
-												  "suggestions: 'Change Y to Z'. If there are no changes needed, respond with 'no changes proposed'. "+
-												  "Example response format: In the `calculate` method, change 'area = length * length' to 'area = "+
-												  "length * width'. All code submitted will be from a large django project using python 3.10.4, which "+
-												  "is focused on data analytics and running background automation tasks. The code snippet provided "+
-												  "is not the full file; it excludes all imports and comments in the original. When you are finished, "+
-												  "adding as much functionality as you can and identifying bugs, please write django unit tests for "+
+					{"role": "system", "content": "Your job is to identify bugs in python code and suggest improvements, adhering to modern best " +
+												  "practices, such as DRY. Review the code supplied and list specific changes to the code. If " +
+												  "functionality can be added to the code, suggest them. Use the following format for your " +
+												  "suggestions: 'Change Y to Z'. If there are no changes needed, respond with 'no changes proposed'. " +
+												  "Example response format: In the `calculate` method, change 'area = length * length' to 'area = " +
+												  "length * width'. All code submitted will be from a large django project using python 3.10.4, which " +
+												  "is focused on data analytics and running background automation tasks. The code snippet provided " +
+												  "is not the full file; it excludes all imports and comments in the original. When you are finished, " +
+												  "adding as much functionality as you can and identifying bugs, please write django unit tests for " +
 												  "the code for 100% code coverage"},
 					{"role": "user", "content": f"File: `{file_path}`, Code: \n\n{code}"},
 				]
 			)
 			# print the full response
 			print(response)
 
@@ -117,31 +118,31 @@
 	def process_python_files(self):
 		python_files = glob.glob(f"{self.project_path}/**/*.py", recursive=True)
 
 		# Exclude __init__.py, and other files that we don't want to check
 		exclude = ["__init__.py", "settings.py", "urls.py", "wsgi.py", "asgi.py", "manage.py"]
 		python_files = [file for file in python_files if os.path.basename(file) not in exclude]
 		excluded_dirs = ['migrations', 'logs', 'tests', 'conf', 'settings', 'static', 'templates',
-				   		 'node_modules', 'venv', 'build', 'dist', 'public', 'docs']
+						 'node_modules', 'venv', 'build', 'dist', 'public', 'docs']
 		for excluded_dir in excluded_dirs:
 			python_files = [file for file in python_files if excluded_dir not in file]
 		count = 0
 
 		for file_path in tqdm(python_files, desc="Processing files", unit="file"):
 			# Check if we've reached the max number of files to process
-			if args.max > 0 and count > args.max:
+			if self.args.max > 0 and count > self.args.max:
 				break
 
 			diff_file_path = file_path + ".diff"
 			if os.path.exists(diff_file_path):
 				print(f"\nSkipping {file_path} as it already has a diff file.")
 				continue
 
 			try:
-				with open(file_path, "r") as source_code:
+				with open(file_path, "r", encoding="utf-8") as source_code:
 					code = source_code.read()
 					code_no_comments = self.trim_code(code)
 
 					# Exclude files that are too short
 					if len(code_no_comments) < 300:
 						print(f"\nSkipping {file_path} as it is too short.")
 						continue
@@ -158,15 +159,15 @@
 
 					if suggestions:
 						# Check if the suggestions are the same as the code we submitted
 						if suggestions == code_no_comments or suggestions.lower() == "no changes proposed":
 							print(f"\nNo suggestions found for {file_path}")
 							continue
 
-						with open(diff_file_path, "w") as diff_file:
+						with open(diff_file_path, "w", encoding="utf-8") as diff_file:
 							diff_file.write(suggestions)
 						print(f"\nSuggestions saved to {diff_file_path}")
 					else:
 						print(f"\nChatGPT did not return suggestions for {file_path}")
 			except Exception as e:
 				print(f"\nError processing file {file_path}: {e}")
 
@@ -176,15 +177,15 @@
 			with open(args.settings, "r", encoding="utf-8") as file:
 				settings = yaml.safe_load(file)
 				openai_api_key = settings['lint']["key"]
 		except Exception as e:
 			print(f"Error loading settings: {e}")
 			return
 
-		bugfixer = ChatGPTBugFixer(openai_api_key, args.path)
+		bugfixer = ChatGPTBugFixer(openai_api_key, args)
 		bugfixer.process_python_files()
 	except KeyboardInterrupt:
 		print("Exiting...")
 
 if __name__ == "__main__":
 	parser = argparse.ArgumentParser(description="Check Python files for bugfixes and improvements using ChatGPT")
 	parser.add_argument("--settings", default="conf/settings.yaml", help="Path to the settings.yaml file")
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/scripts/summarize.py` & `djangofoundry-0.0.5/src/djangofoundry/scripts/summarize.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Configure logger to print to output
 logging.basicConfig(level=logging.DEBUG, handlers=[logging.StreamHandler()])
 logger = logging.getLogger(__name__)
 
 class PythonClassParser:
 	"""
-	Parser for Python classes in a directory. 
+	Parser for Python classes in a directory.
 
 	This class will parse all Python files in a directory and output a summary of all classes found in those files, which can be used
 	to generate documentation for the project, or to pass to other tools (like LLMs).
 	"""
 	def __init__(self, directory: str, output_file: str, ignored_paths: List[str], recursive: bool) -> None:
 		logger.debug(f"Initializing PythonClassParser: {directory} : {output_file}")
 		self.directory: str = directory
@@ -225,17 +225,17 @@
 	parser.add_argument('-i', '--ignore', nargs='*', default=[], help="Directories or files to ignore")
 	parser.add_argument('-l', '--logfile', type=str, help="Log file")
 	parser.add_argument('-r', '--recursive', action='store_true', help="Enable or disable recursive search in subdirectories", default=True)
 	parser.add_argument('-v', '--verbose', action='store_true', help="Print debug messages")
 	return parser.parse_args()
 
 if __name__ == "__main__":
-	args: argparse.Namespace = parse_args()
+	args : argparse.Namespace = parse_args()
 	if args.verbose:
 		logger.setLevel(logging.DEBUG)
 
 	if args.logfile:
 		file_handler = logging.FileHandler(args.logfile)
 		logger.addHandler(file_handler)
 
-	parser: PythonClassParser = PythonClassParser(args.directory, args.output, args.ignore, args.recursive)
-	parser.run()
+	arg_parser : PythonClassParser = PythonClassParser(args.directory, args.output, args.ignore, args.recursive)
+	arg_parser.run()
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/scripts/conf/sample-settings.yaml` & `djangofoundry-0.0.5/src/djangofoundry/scripts/conf/sample-settings.yaml`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/scripts/utils/__init__.py` & `djangofoundry-0.0.5/src/djangofoundry/scripts/utils/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 		-----
 
 		Copyright (c) 2022 Jess Mann
 """
 from djangofoundry.scripts.utils.action import EnumAction
 from djangofoundry.scripts.utils.exceptions import (
-    AppException,
-    FileEmptyError,
-    DbError,
-    DbConnectionError,
-    DbStartError,
-    UnsupportedCommandError
+	AppException,
+	FileEmptyError,
+	DbError,
+	DbConnectionError,
+	DbStartError,
+	UnsupportedCommandError
 )
 from djangofoundry.scripts.utils.settings import Settings
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/scripts/utils/action.py` & `djangofoundry-0.0.5/src/djangofoundry/scripts/utils/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 		Last Modified: Sat Dec 03 2022
 		Modified By: Jess Mann
 
 		-----
 
 		Copyright (c) 2022 Jess Mann
 """
-import argparse, enum
+import argparse
+import enum
 from typing import Any, Optional
 
 class EnumAction(argparse.Action):
 	"""
 	Argparse action for handling Enums
 	"""
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/scripts/utils/exceptions.py` & `djangofoundry-0.0.5/src/djangofoundry/scripts/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/scripts/utils/settings.py` & `djangofoundry-0.0.5/src/djangofoundry/scripts/utils/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 	def load_config(self, settings_path : str = SETTINGS_PATH) -> SettingsFile:
 		# Read our default sensitivity settings (if available)
 		filepath = os.path.join(os.path.dirname(os.path.abspath(__file__)), settings_path)
 
 		if os.path.exists(filepath):
 			# If it exists, then open it
 			with open(filepath, encoding='utf-8') as file:
-	     		# Load the contents into a variable
+				# Load the contents into a variable
 				self._settings = yaml.load(file, Loader=SafeLoader)
 		else:
 			# Let everyone know we couldn't find the settings. This likely exits.
 			raise FileNotFoundError(f"Could not load bin settings from {filepath}")
 
 		# Validate contents of settings file.
 		if self._settings == {}:
@@ -105,26 +105,26 @@
 
 	def all(self) -> SettingsFile:
 		"""
 		Makes the syntax for getting the settings dict a little less clunky (i.e. Settings.all() instead of Settings.settings)
 
 		Returns:
 			dict: A dictionary of settings.
-  		"""
+		"""
 		return self.settings
 
 
 	def get(self, key : str) -> Any:
 		"""
 		Retrieves the value at the provided key.
 
 		Args:
 			key (str): A key to retrieve
 
 		Returns:
 			Any: The value stored at the provided key
-  		"""
+		"""
 		return self.settings.get(key)
 
 if __name__ == '__main__':
 	conf = Settings.settings
 	print(conf)
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/scripts/utils/types.py` & `djangofoundry-0.0.5/src/djangofoundry/scripts/utils/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 class LogHandler(TypedDict):
 	"""
 	Expected format for a "handler" in the settings file.
 	"""
 	level: LoggerLevels
 	formatter: str
 	stream: str
-	#class: str
+	# class: str
 
 class LogRoot(TypedDict):
 	"""
 	Expected format for the "root" logger in the settings file.
 	"""
 	level: LoggerLevels
 	handlers: list[LogHandler]
```

### Comparing `djangofoundry-0.0.4/src/djangofoundry/signals/abstract.py` & `djangofoundry-0.0.5/src/djangofoundry/signals/abstract.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/templates/memory.html` & `djangofoundry-0.0.5/src/djangofoundry/templates/memory.html`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/templates/angular/base.html` & `djangofoundry-0.0.5/src/djangofoundry/templates/angular/base.html`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/templates/jinja/model.py.jinja` & `djangofoundry-0.0.5/src/djangofoundry/templates/jinja/model.py.jinja`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/src/djangofoundry/templatetags/syntax_highlight.py` & `djangofoundry-0.0.5/src/djangofoundry/templatetags/syntax_highlight.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/tests/foundry/test_matching.py` & `djangofoundry-0.0.5/tests/foundry/test_matching.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/tests/foundry/controllers/test_mixins.py` & `djangofoundry-0.0.5/tests/foundry/controllers/test_mixins.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/tests/foundry/decorators/test_timeout.py` & `djangofoundry-0.0.5/tests/foundry/decorators/test_timeout.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/tests/foundry/helpers/test_hooks.py` & `djangofoundry-0.0.5/tests/foundry/helpers/test_hooks.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/tests/foundry/helpers/test_queue.py` & `djangofoundry-0.0.5/tests/foundry/helpers/test_queue.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/tests/foundry/models/test_choices.py` & `djangofoundry-0.0.5/tests/foundry/models/test_choices.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/tests/foundry/models/test_queryset.py` & `djangofoundry-0.0.5/tests/foundry/models/test_queryset.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 
 		-----
 
 		Copyright (c) 2023 Jess Mann
 """
 from math import sqrt
 from django.test import TestCase
-from model_bakery import baker
 from django.db.models import Q
-from unittest.mock import MagicMock
+from model_bakery import baker
 from djangofoundry.models import QuerySet
 
 # Create a mock model using model_bakery
 class Case:
 	objects = QuerySet.as_manager()
 
 class QuerySetTestCase(TestCase):
```

### Comparing `djangofoundry-0.0.4/LICENSE.md` & `djangofoundry-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/README.md` & `djangofoundry-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.4/pyproject.toml` & `djangofoundry-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "djangofoundry"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Jess Mann", email="jess.a.mann+df@gmail.com" },
 ]
 description = "A collection of classes built on Django to make it easier to build web applications."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `djangofoundry-0.0.4/PKG-INFO` & `djangofoundry-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangofoundry
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of classes built on Django to make it easier to build web applications.
 Project-URL: Homepage, https://github.com/avranu/Django-Foundry
 Project-URL: Bug Tracker, https://github.com/avranu/Django-Foundry/issues
 Author-email: Jess Mann <jess.a.mann+df@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

