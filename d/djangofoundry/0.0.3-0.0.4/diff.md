# Comparing `tmp/djangofoundry-0.0.3.tar.gz` & `tmp/djangofoundry-0.0.4.tar.gz`

## Comparing `djangofoundry-0.0.3.tar` & `djangofoundry-0.0.4.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/.dockerignore
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/.prospector.yaml
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/Dockerfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/docker-compose.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/logging.conf
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/package.json
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/requirements.txt
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/.devcontainer/docker-compose.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/__init__.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/urls.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/__init__.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/angular.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/detail.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/generic.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/list.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/memory.py
--rw-r--r--   0        0        0    15504 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/responses.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/decorators/__init__.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/decorators/queryset_filter.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/decorators/retry.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/decorators/timeout.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/exceptions/__init__.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/exceptions/app.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/__init__.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/logging.py
--rw-r--r--   0        0        0    11832 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/progress.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/encoders/__init__.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/encoders/json.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/__init__.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/exceptions.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/hook.py
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/hooks.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/waypoint.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/meta/__init__.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/meta/constants.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/meta/types.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/queue/__init__.py
--rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/queue/queue.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/queue/signals.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/__init__.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/template.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/__init__.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/template.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/__init__.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/css.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/javascript.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/template.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/python/__init__.py
--rw-r--r--   0        0        0     9053 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/python/model.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/python/template.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/meta/__init__.py
--rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/meta/model.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/matching/__init__.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/matching/engine.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/matching/fuzzy/__init__.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/matching/fuzzy/thefuzz.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/meta/__init__.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/meta/request.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/mixins/__init__.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/mixins/dirtyfields.py
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/mixins/hasParams.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/mixins/hookable.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/mixins/jsonResponse.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/__init__.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/choices.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/manager.py
--rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/model.py
--rw-r--r--   0        0        0    53573 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/queryset.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/serializer.py
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/viewset.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/exceptions/__init__.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/exceptions/get.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/__init__.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/boolean.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/char.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/date.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/number.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/objects.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/relationships.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/README.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/__init__.py
--rw-r--r--   0        0        0    19911 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/app.py
--rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/db.py
--rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/lint.py
--rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/summarize.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/conf/sample-settings.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/utils/README.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/utils/__init__.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/utils/action.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/utils/exceptions.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/utils/settings.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/utils/types.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/signals/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/signals/abstract.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/templates/memory.html
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/templates/angular/base.html
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/templates/jinja/model.py.jinja
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/templatetags/__init__.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/templatetags/syntax_highlight.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/test_matching.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/controllers/__init__.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/controllers/test_mixins.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/decorators/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/decorators/test_timeout.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/helpers/__init__.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/helpers/test_hooks.py
--rw-r--r--   0        0        0     8781 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/helpers/test_queue.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/models/__init__.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/models/test_choices.py
--rw-r--r--   0        0        0    10267 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/models/test_queryset.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/.gitignore
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/README.md
--rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/.dockerignore
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/.prospector.yaml
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/Dockerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/docker-compose.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/logging.conf
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/package.json
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/.devcontainer/docker-compose.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/__init__.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/urls.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/angular.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/detail.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/generic.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/list.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/memory.py
+-rw-r--r--   0        0        0    15504 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/controllers/responses.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/decorators/__init__.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/decorators/queryset_filter.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/decorators/retry.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/decorators/timeout.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/exceptions/__init__.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/exceptions/app.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/__init__.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/logging.py
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/progress.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/encoders/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/encoders/json.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/__init__.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/exceptions.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/hook.py
+-rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/hooks.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/waypoint.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/meta/__init__.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/meta/constants.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/meta/types.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/queue/__init__.py
+-rw-r--r--   0        0        0    14036 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/queue/queue.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/queue/signals.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/__init__.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/template.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/__init__.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/template.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/__init__.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/css.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/javascript.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/template.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/python/__init__.py
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/python/model.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/python/template.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/meta/__init__.py
+-rw-r--r--   0        0        0     9232 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/helpers/render/meta/model.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/matching/__init__.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/matching/engine.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/matching/fuzzy/__init__.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/matching/fuzzy/thefuzz.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/mixins/__init__.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/mixins/dirtyfields.py
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/mixins/hasParams.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/mixins/hookable.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/mixins/jsonResponse.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/__init__.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/choices.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/manager.py
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/model.py
+-rw-r--r--   0        0        0    53644 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/queryset.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/serializer.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/viewset.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/exceptions/__init__.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/exceptions/get.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/__init__.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/boolean.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/char.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/date.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/number.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/objects.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/models/fields/relationships.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/options/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/options/request.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/README.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/__init__.py
+-rw-r--r--   0        0        0    19911 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/app.py
+-rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/db.py
+-rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/lint.py
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/summarize.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/conf/sample-settings.yaml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/utils/README.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/utils/__init__.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/utils/action.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/utils/exceptions.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/utils/settings.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/scripts/utils/types.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/signals/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/signals/abstract.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/templates/memory.html
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/templates/angular/base.html
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/templates/jinja/model.py.jinja
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/templatetags/__init__.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/src/djangofoundry/templatetags/syntax_highlight.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/test_matching.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/controllers/__init__.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/controllers/test_mixins.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/decorators/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/decorators/test_timeout.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/helpers/__init__.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/helpers/test_hooks.py
+-rw-r--r--   0        0        0     8781 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/helpers/test_queue.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/models/__init__.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/models/test_choices.py
+-rw-r--r--   0        0        0    10267 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/tests/foundry/models/test_queryset.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/README.md
+-rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 djangofoundry-0.0.4/PKG-INFO
```

### Comparing `djangofoundry-0.0.3/.prospector.yaml` & `djangofoundry-0.0.4/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/Dockerfile` & `djangofoundry-0.0.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/package.json` & `djangofoundry-0.0.4/package.json`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/.devcontainer/devcontainer.json` & `djangofoundry-0.0.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/.devcontainer/docker-compose.yml` & `djangofoundry-0.0.4/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/urls.py` & `djangofoundry-0.0.4/src/djangofoundry/urls.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/controllers/__init__.py` & `djangofoundry-0.0.4/src/djangofoundry/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/controllers/angular.py` & `djangofoundry-0.0.4/src/djangofoundry/controllers/angular.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 
 		Returns:
 			An empty object.
 		"""
 		return {}
 
 	def get(self, request, *args, **kwargs):
-		return render(request, self.template_name)
+		return render(request, self.template_name, *args, **kwargs)
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/controllers/detail.py` & `djangofoundry-0.0.4/src/djangofoundry/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/controllers/generic.py` & `djangofoundry-0.0.4/src/djangofoundry/controllers/generic.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/controllers/list.py` & `djangofoundry-0.0.4/src/djangofoundry/controllers/list.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/controllers/memory.py` & `djangofoundry-0.0.4/src/djangofoundry/controllers/memory.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/controllers/responses.py` & `djangofoundry-0.0.4/src/djangofoundry/controllers/responses.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/decorators/queryset_filter.py` & `djangofoundry-0.0.4/src/djangofoundry/decorators/queryset_filter.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/decorators/retry.py` & `djangofoundry-0.0.4/src/djangofoundry/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/decorators/timeout.py` & `djangofoundry-0.0.4/src/djangofoundry/decorators/timeout.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/exceptions/app.py` & `djangofoundry-0.0.4/src/djangofoundry/exceptions/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 
 	Metadata:
 
-		File: exceptions.py
+		File: exceptions/app.py
 		Project: Django Foundry
 		Created Date: 17 Dec 2022
 		Author: Jess Mann
 		Email: jess.a.mann@gmail.com
 
 		-----
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/logging.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 		Copyright (c) 2022 Jess Mann
 """
 from __future__ import annotations
 import logging
 
 # Set up logging for this module. __name__ includes the namespace (e.g. dashboard.models.cases).
 #
-# We can adjust logging settings from the namespace down to the module level in EmtAutomation/settings
+# We can adjust logging settings from the namespace down to the module level in project/settings
 #
 logger = logging.getLogger(__name__)
 
 def log_object( obj, level : str = 'DEBUG', name : str = 'Reference', use_logger = None ) -> None:
 	if use_logger is None:
 		use_logger = logger
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/progress.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 """
 # Generic imports
 from __future__ import annotations
 
 from decimal import Decimal
 from time import perf_counter_ns
 from typing import Optional
+from datetime import timedelta
 from typing_extensions import Self
 from celery_progress.backend import ProgressRecorder, PROGRESS_STATE
 from celery.app.task import Task
 import humanize
-from datetime import timedelta
 # Django Imports
 from django.db.models import TextChoices
 # Lib Imports
 # App Imports
 
 class ProgressStates(TextChoices):
 	"""
@@ -109,24 +109,23 @@
 			progress.update()
 
 		Allow None for task, which will effectively suppress output
 		'''
 		if settings is None:
 			settings = {}
 
-		# Set our task if we were provided one
-		self.task = task
-
 		# Set the total early so we can be sure it isn't None when calculations are requested.
 		self.total = total
 
 		# Allow settings to be passed in completely, partially, or changed later.
 		# This notation indicates a dict merge. Default settings are overwritten by any settings passed in.
 		self.settings = default_settings | settings
 
+		super().__init__(task)
+
 		# Start the clock on init
 		self._init_start()
 
 	@property
 	def meta(self) -> dict:
 		return {
 			'pending': self.pending,
@@ -292,15 +291,15 @@
 		return self.current
 
 	def advance(self, amount : int, description: Optional[str] = None) -> int:
 		"""
 		Convenience function for self.next(advance = amount).
 
 		Args:
-			advance (int):
+			amount (int):
 				The amount to increase in the current task.
 			description (str, optional):
 				An optional description to set
 
 		Returns:
 			int: The current counter after increasing it
 		"""
@@ -360,15 +359,15 @@
 		if current is None and total is None and description is None:
 			raise ValueError('ProgressBar.update: no values set')
 
 		if current is not None:
 			self._current = int(current)
 		if total is not None:
 			self._total = int(total)
-		if description is not None:
+		if description:
 			self._description = str(description)
 
 		# If a task exists, refresh it
 		self.refresh_task_state()
 
 	def set_progress(self, current: int, total: int = 100, description: str = ""):
 		'''
@@ -388,15 +387,15 @@
 	def refresh_task_state(self) -> None:
 		'''
 		Update the task state based on our instance attributes
 		'''
 
 		# Update to running if we 1) haven't yet and 2) have done anything at all.
 		# -- otherwise, trust the end user to update states appropriately
-		if not ProgressStates.has_started(self.state) and (self._current > 0 or self._description != ''):
+		if not ProgressStates.has_started(self.state) and (self._current > 0 or self._description):
 			self._state = PROGRESS_STATE
 
 		# If we don't have a task, there's nothing to refresh
 		if self.task is None:
 			return
 
 		# Refresh the state of the task we have based on our local values here
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/__init__.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/exceptions.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/exceptions.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/hook.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/hooks.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 				return [names.values() for names in cls._hooks.values()]
 
 			# Name but no namespace, raise an error
 			raise ValueError(f'Requesting all waypoints with a name ({name}) but no namespace specified.')
 
 		if name is None:
 			# No name, but a namespace. Return all waypoints in that namespace.
-			return [waypoint for waypoint in cls._hooks[namespace].values()]
+			return list(cls._hooks[namespace].values())
 
 		# Both a name and a namespace. Return the single waypoint as a list to match our return type.
 		return list(cls._hooks[namespace][name])
 
 	@classmethod
 	def count(cls, name : Optional[str] = None, namespace : str = DEFAULT_NAMESPACE) -> int:
 		"""
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/waypoint.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/waypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 		-----
 
 		Copyright (c) 2022 Jess Mann
 """
 # Generic imports
 from __future__ import annotations
-from typing import TYPE_CHECKING, Any, Iterable, Optional
+from typing import TYPE_CHECKING, Any, Iterable
 from djangofoundry.helpers.hooks.meta.constants import DEFAULT_NAMESPACE
 
 if TYPE_CHECKING:
 	from djangofoundry.helpers.hooks.hook import Hook
 
 class Waypoint:
 	"""
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/meta/constants.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/meta/constants.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/meta/types.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/hooks/meta/types.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/queue/queue.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/queue/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,29 @@
 		-----
 
 		Copyright (c) 2022 Jess Mann
 """
 # Generic imports
 from __future__ import annotations
 from typing import Any, Callable, Optional
-from typing_extensions import Self
-from psqlextra.query import ConflictAction
 import queue
 from collections import deque
+from typing_extensions import Self
+from psqlextra.query import ConflictAction
 # Django Imports
 # Lib Imports
 from djangofoundry.helpers.queue import signals
 from djangofoundry.models import Model
 from djangofoundry.models.choices import TextChoices
 # App Imports
 
 class Callbacks(TextChoices):
+	"""
+	Constants for the callback points on a queue
+	"""
 	SAVE = 'save'
 	CLEAR = 'clear'
 	APPEND = 'append'
 
 class Queue(queue.Queue):
 	'''
 	This class handles queueing models for a bulk save. When the queue reaches its limit, it will automatically save the queued models and empty the queue
@@ -61,22 +64,22 @@
 		queue.size(Case) # --> 0
 	'''
 
 	# The point at which we automatically trigger save()
 	limit: int = 100
 
 	# The key on this model to check for collisions during save() - if a collision happens, we update instead
-	unique_key: list[str] = list()
+	unique_key: list[str] = []
 
 	# A queue ONLY works on a single model. This can be specified in __init__, or determined by the first append
 	model: Model
 
 	# Optional callbacks to be used when certain actions occur (like saving the queue, clearing the queue, etc)
 	# NOTE: The signature uses "str" instead of "Callbacks" so that subclasses of Queue can implement additional callback points.
-	callbacks: dict[str, Callable | None] = dict()
+	callbacks: dict[str, Callable | None] = {}
 
 	# If True, saving the queue will be deferred until it is turned back on
 	# Saving will still occur at the end of a with block.
 	_save_deferred : bool = False
 
 	# A queue for one specific model. For example:
 	# case_queue = [Case(), Case()]
@@ -203,14 +206,15 @@
 
 	def callback(self, callback_name : str, **kwargs) -> Any:
 		"""
 		Issue a callback (if it is defined)
 
 		Args:
 			callback_name (str): The name of the callback (specified in __init__ or the class definition)
+			**kwargs: Any additional arguments to pass to the callback
 
 		Returns:
 			Any: Special callbacks may define what kinds of data they wish to return.
 
 		Raises:
 			ValueError: If the callback_name is not set (i.e. there is a typo)
 		"""
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/queue/signals.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/queue/signals.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/render/template.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/render/template.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,14 @@
 
 	@abstractmethod
 	def render(self, variables: dict, template_name: str) -> str | None:
 		"""
 		Render a template with the given variables.
 
 		Args:
-			template_name (str): The name of the template to render.
 			variables (dict): The variables to pass to the template.
+			template_name (str): The name of the template to render.
 
 		Returns:
 			str: The rendered template.
 		"""
 		raise NotImplementedError("Subclasses of TemplateHelper must implement render()")
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/template.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/template.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -81,16 +81,16 @@
 		)
 
 	def render(self, variables: dict, template_name: str) -> str | None:
 		"""
 		Render a template with the given variables.
 
 		Args:
-			template_name (str): The name of the template to render.
 			variables (dict): The variables to pass to the template.
+			template_name (str): The name of the template to render.
 
 		Returns:
 			str: The rendered template.
 		"""
 		try:
 			template = self.env.get_template(template_name + self.template_suffix)
 			return template.render(variables)
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/css.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/css.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/javascript.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/javascript.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/template.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 	"""
 
 	def suggest_class_name(self, input_str: str) -> str:
 		"""
 		Suggest a class name based on a set of input. This method exists primarily to establish an interface for subclasses.
 
 		Args:
-			input (str): The input to base the suggested name on
+			input_str (str): The input to base the suggested name on
 
 		Returns:
 			str: The suggested class name
 		"""
 
 		# Remove any non-alpha and title case
 		cleaned_name = re.sub(r'[^a-zA-Z]+', ' ', input_str).title().replace(' ', '')
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/python/model.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/python/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 	@property
 	def cursor(self) -> CursorWrapper:
 		"""
 		The django connection handler cursor for the database to generate a model for.
 		"""
 		return self.connection.cursor()
 
-	def __init__(self, table_name: str, database: str, schema: Optional[str] = None, app_name: str = 'lib', template_path: str = 'templates/jinja', autoescape: list = [], template_suffix: str = '.py.jinja'):
+	def __init__(self, table_name: str, database: str, schema: Optional[str] = None, app_name: str = 'lib', template_path: str = 'templates/jinja', autoescape: list = list, template_suffix: str = '.py.jinja'):
 		"""
 		Initializes a new instance of the ModelHelper class.
 
 		Args:
 			template_suffix (str): The suffix to use for template files (defaults to ".py.jinja")
 			table_name (str): The name of the table to generate a model for
 		"""
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/python/template.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/render/jinja/code/python/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/helpers/render/meta/model.py` & `djangofoundry-0.0.4/src/djangofoundry/helpers/render/meta/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 		Modified By: Jess Mann
 
 		-----
 
 		Copyright (c) 2023 Jess Mann
 """
 from __future__ import annotations
-from typing import Any, List, Optional
+from typing import Any, Optional
 from enum import Enum
-from typing import Any
 
 class ConstraintType(Enum):
 	"""
 	Possible constraints for a column in Oracle
 	"""
 	PRIMARY_KEY = 'P'
 	UNIQUE = 'U'
@@ -169,19 +168,20 @@
 		deferrable (str): Whether or not the constraint is deferrable
 		deferred (str): Whether or not the constraint is deferred
 		validated (str): Whether or not the constraint is validated
 		generated (str): Whether or not the constraint is generated
 		last_change (str): The last time the constraint was changed
 	"""
 	def __init__(self, name, constraint_type: ConstraintType, column_name, search_condition : Optional[str] = None, r_constraint_name : Optional[str] = None, r_owner : Optional[Any] = None, delete_rule : Optional[str] = None, status : Optional[str] = None, deferrable : Optional[str] = None, deferred : Optional[str] = None, validated : Optional[str] = None, generated : Optional[str] = None, last_change : Optional[str] = None, *args, **kwargs):
-		self.name = name
+		super().__init__(name)
 		self.constraint_type = constraint_type
 		self.column_name = column_name
 		self.search_condition = search_condition
 		self.r_constraint_name = r_constraint_name
+		self.r_owner = r_owner
 		self.delete_rule = delete_rule
 		self.status = status
 		self.deferrable = deferrable
 		self.deferred = deferred
 		self.validated = validated
 		self.generated = generated
 		self.last_change = last_change
@@ -226,15 +226,15 @@
 	Atributes:
 		name (str): The name of the index
 		uniqueness (str): Whether or not the index is unique
 		columns (list[IndexColumnInfo]): The columns in the index
 	"""
 
 	def __init__(self, name: str, columns: Optional[list[IndexColumnInfo]] = None, uniqueness: str = ''):
-		if not name or name == '':
+		if not name:
 			name = f'index.{"-".join([column.name for column in columns or []])}'
 		super().__init__(name)
 		self.uniqueness = uniqueness
 		self.columns = columns if columns is not None else []
 
 	def add_column(self, column_name: str, column_position: int):
 		"""
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/matching/engine.py` & `djangofoundry-0.0.4/src/djangofoundry/matching/engine.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/matching/fuzzy/thefuzz.py` & `djangofoundry-0.0.4/src/djangofoundry/matching/fuzzy/thefuzz.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/mixins/dirtyfields.py` & `djangofoundry-0.0.4/src/djangofoundry/mixins/dirtyfields.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/mixins/hasParams.py` & `djangofoundry-0.0.4/src/djangofoundry/mixins/hasParams.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import re
 import logging
 
 # Get a logger for logging messages
 #
 # Set up logging for this module. __name__ includes the namespace (e.g. dashboard.models.cases).
 #
-# We can adjust logging settings from the namespace down to the module level in EmtAutomation/settings
+# We can adjust logging settings from the namespace down to the module level in project/settings
 #
 logger = logging.getLogger(__name__)
 
 # A generic type we use in some of our sanitizing methods.
 T = TypeVar('T')
 
 class HasParams:
@@ -94,14 +94,15 @@
 				If False, return the user input unmodified. Otherwise, sanitize the user input (default).
 
 		Returns:
 			str: The value of the parameter
 
 		Raises:
 			ReferenceError: If the parameter is missing
+			TypeError: If the parameter is found but is None
   		"""
 		value = self.get_param(name, sanitize=sanitize, required=True)
 
 		# This should never happen, because required=True should throw a ReferenceError if the value is null.
 		# This check is here for future proofing.
 		if value is None:
 			raise TypeError(f"Internal error: required param {name} is None.")
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/mixins/hookable.py` & `djangofoundry-0.0.4/src/djangofoundry/mixins/hookable.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/mixins/jsonResponse.py` & `djangofoundry-0.0.4/src/djangofoundry/mixins/jsonResponse.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # Django imports
 from django.http import JsonResponse
 
 # Get a logger for logging messages
 #
 # Set up logging for this module. __name__ includes the namespace (e.g. dashboard.models.cases).
 #
-# We can adjust logging settings from the namespace down to the module level in EmtAutomation/settings
+# We can adjust logging settings from the namespace down to the module level in project/settings
 #
 logger = logging.getLogger(__name__)
 
 class JSONResponseMixin:
 	"""
 	Mixin for a controller that render JSON responses.
 	"""
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/__init__.py` & `djangofoundry-0.0.4/src/djangofoundry/models/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/choices.py` & `djangofoundry-0.0.4/src/djangofoundry/models/choices.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/manager.py` & `djangofoundry-0.0.4/src/djangofoundry/models/manager.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/model.py` & `djangofoundry-0.0.4/src/djangofoundry/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 import logging
 # Django Imports
 from django.db import models
 # Django extensions
 import auto_prefetch
 # Lib Imports
 from djangofoundry.mixins import Hookable
-# App Imports
 from djangofoundry.models.manager import PostgresManager
 
 # Set up a logger for this module.
 #
 # Set up logging for this module. __name__ includes the namespace (e.g. dashboard.models.cases).
 #
 # We can adjust logging settings from the namespace down to the module level in DjangoFoundry/settings
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/queryset.py` & `djangofoundry-0.0.4/src/djangofoundry/models/queryset.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,19 @@
 from typing_extensions import Self
 from statsmodels.tsa.seasonal import seasonal_decompose
 from statsmodels.tsa.stattools import grangercausalitytests
 from scipy import stats
 import pandas as pd
 import numpy as np
 # Django Imports
-from django.db.models import Sum, Count, Q, Avg, Min, Max, StdDev, ExpressionWrapper, fields, F, FloatField
+from django.db.models import (
+	Sum, Count, Q, Avg, Min, Max, StdDev, ExpressionWrapper, F, 
+	FloatField, IntegerField, DecimalField, BigIntegerField, PositiveIntegerField, 
+	PositiveSmallIntegerField, SmallIntegerField, DurationField, PositiveBigIntegerField
+)
 from django.db.models.query import RawQuerySet
 # Django extensions
 import auto_prefetch
 # App Imports
 
 #
 # Set up logging for this module. __name__ includes the namespace (e.g. dashboard.models.cases).
@@ -95,23 +99,23 @@
 			False
 		"""
 		if not hasattr(self.model, field_name):
 			raise ValueError(f"No field '{field_name}' on queryset")
 
 		# List of all fields that are numeric
 		numeric_fields = [
-			fields.IntegerField,
-			fields.FloatField,
-			fields.DecimalField,
-			fields.BigIntegerField,
-			fields.PositiveIntegerField,
-			fields.SmallIntegerField,
-			fields.PositiveSmallIntegerField,
-			fields.DurationField,
-			fields.PositiveBigIntegerField,
+			IntegerField,
+			FloatField,
+			DecimalField,
+			BigIntegerField,
+			PositiveIntegerField,
+			SmallIntegerField,
+			PositiveSmallIntegerField,
+			DurationField,
+			PositiveBigIntegerField,
 		]
 		attr = getattr(self.model, field_name)
 
 		return any(isinstance(attr, field) for field in numeric_fields)
 
 	def latest_value(self, property_name: str) -> Any:
 		'''
@@ -512,15 +516,15 @@
 			{ 0: 1, 1: 2, 2: 1, 3: 1, 4: 1 }
 		'''
 		# Get the min and max of the field
 		min_value = self.aggregate(Min(field_name))[f"{field_name}__min"]
 		max_value = self.aggregate(Max(field_name))[f"{field_name}__max"]
 
 		# Get the distribution
-		distribution = (self.values(field_name).annotate(bin=ExpressionWrapper(F(field_name) - min_value, output_field=fields.IntegerField()) // ((max_value - min_value) // bins)).values("bin").annotate(count=Count("bin")).order_by("bin"))
+		distribution = (self.values(field_name).annotate(bin=ExpressionWrapper(F(field_name) - min_value, output_field=IntegerField()) // ((max_value - min_value) // bins)).values("bin").annotate(count=Count("bin")).order_by("bin"))
 
 		return {result["bin"]: result["count"] for result in distribution}
 
 	def summarize_x_by_y_distribution(self, x_field_name: str, y_field_name: str, bins: int = 10) -> dict[str, dict[int, int]]:
 		'''
 		Summarizes the distribution of a field by another field. This is used to summarize the distribution of a field in a queryset by another field.
 		For example, if we have a queryset of cases, we get a list of the distribution of the processing time field by status.
@@ -541,16 +545,16 @@
 			{ 'open': { 0: 1, 1: 1, 2: 1, 3: 1, 4: 1 }, 'closed': { 0: 1, 1: 1, 2: 1, 3: 1, 4: 1 } }
 		'''
 		# Get the min and max of the field
 		min_value = self.aggregate(Min(y_field_name))[f"{y_field_name}__min"]
 		max_value = self.aggregate(Max(y_field_name))[f"{y_field_name}__max"]
 
 		# Get the distribution
-		distribution = (self.values(x_field_name, y_field_name).annotate(bin=ExpressionWrapper(F(y_field_name) - min_value, output_field=fields.IntegerField()) // ((max_value - min_value) // bins)).values(x_field_name,
-																																														   			         "bin").annotate(count=Count("bin")).order_by(x_field_name, "bin"))
+		distribution = (self.values(x_field_name, y_field_name).annotate(bin=ExpressionWrapper(F(y_field_name) - min_value, output_field=IntegerField()) // ((max_value - min_value) // bins)).values(x_field_name,
+																																														   					 "bin").annotate(count=Count("bin")).order_by(x_field_name, "bin"))
 
 		# Convert the distribution to a dictionary
 		distribution_dict = {}
 		for result in distribution:
 			if result[x_field_name] not in distribution_dict:
 				distribution_dict[result[x_field_name]] = {}
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/serializer.py` & `djangofoundry-0.0.4/src/djangofoundry/models/serializer.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 		-----
 
 		Copyright (c) 2022 Jess Mann
 """
 # Generic imports
 from __future__ import annotations
-from rest_framework import serializers
+from rest_framework.serializers import ModelSerializer
 
-class Serializer(serializers.ModelSerializer):
+class Serializer(ModelSerializer):
 	"""
 	A base serializer class that can be used to dynamically include or exclude fields based on context.
 	"""
 
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/viewset.py` & `djangofoundry-0.0.4/src/djangofoundry/models/viewset.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,28 +15,33 @@
 
 		-----
 
 		Copyright (c) 2022 Jess Mann
 """
 # Generic imports
 from __future__ import annotations
+from typing import TYPE_CHECKING
 # Django Imports
 # Third party imports
-from rest_framework import viewsets, filters
+from rest_framework.filters import OrderingFilter
+from rest_framework.viewsets import ReadOnlyModelViewSet
 # App imports
 from djangofoundry.mixins import HasParams
-from djangofoundry.models.queryset import QuerySet
 from djangofoundry.models.serializer import Serializer
 
-class ViewSet(HasParams, viewsets.ReadOnlyModelViewSet):
+if TYPE_CHECKING:
+	from djangofoundry.models.queryset import QuerySet
+
+
+class ViewSet(HasParams, ReadOnlyModelViewSet):
 	"""
 	An abstract viewset class that provides a default implementation for the get_queryset method, and allows for filtering and ordering of the queryset.
 	"""
 	serializer_class = Serializer
-	filter_backends = [filters.OrderingFilter]
+	filter_backends = [OrderingFilter]
 	filterset_fields : list[str] = []
 	ordering_fields = ['__all__']
 	ordering = ['id']
 
 	def apply_filters(self, queryset : QuerySet) -> QuerySet:
 		"""
 		Apply filters to the queryset. This is applied automatically in the get_queryset method using the filterset_fields attribute and request params.
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/exceptions/get.py` & `djangofoundry-0.0.4/src/djangofoundry/models/exceptions/get.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/fields/__init__.py` & `djangofoundry-0.0.4/src/djangofoundry/models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/fields/char.py` & `djangofoundry-0.0.4/src/djangofoundry/models/fields/char.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 
 		-----
 
 		Copyright (c) 2022 Jess Mann
 """
 # Generic imports
 from __future__ import annotations
-
-from typing import Optional
 # Django Imports
 from django.db import models
 # Lib Imports
 # App Imports
 
 class CharField(models.CharField):
 	'''
@@ -47,46 +45,42 @@
 
 
 class RowIdField(CharField):
 	"""
 	A charfield that is used for storing row ids (from databases like Oracle)
 	"""
 	def __init__(self, *,
-				 map_field  : Optional[str] = None,
 				 max_length : int = 18,
 				 unique	 : bool = True,
 				 null	   : bool = False,
 				 blank	  : bool = False,
 				 editable   : bool = False,
 				 **kwargs):
 		# Call the parent init function first
 		super().__init__(max_length  = max_length,
-								map_field   = map_field,
 								unique	  = unique,
 								null		= null,
 								blank	   = blank,
 								editable	= editable,
 								**kwargs)
 
 class GuidField(CharField):
 	"""
 	A charfield that is used for storing GUIDs (UUID v4)
 	"""
 	def __init__(self, *,
-				 map_field  : Optional[str] = None,
 				 max_length : int = 38,
 				 unique	 : bool = True,
 				 null	   : bool = False,
 				 blank	  : bool = False,
 				 editable   : bool = False,
 				 **kwargs):
 		'''
 		Redefine init to only accept named args
 		'''
 		# Call the parent init function first
 		super().__init__(max_length  = max_length,
-								map_field   = map_field,
 								unique	  = unique,
 								null		= null,
 								blank	   = blank,
 								editable	= editable,
 								**kwargs)
```

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/fields/date.py` & `djangofoundry-0.0.4/src/djangofoundry/models/fields/date.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/fields/number.py` & `djangofoundry-0.0.4/src/djangofoundry/models/fields/number.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/fields/objects.py` & `djangofoundry-0.0.4/src/djangofoundry/models/fields/objects.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/models/fields/relationships.py` & `djangofoundry-0.0.4/src/djangofoundry/models/fields/relationships.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/scripts/__init__.py` & `djangofoundry-0.0.4/src/djangofoundry/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/scripts/app.py` & `djangofoundry-0.0.4/src/djangofoundry/scripts/app.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/scripts/db.py` & `djangofoundry-0.0.4/src/djangofoundry/scripts/db.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/scripts/lint.py` & `djangofoundry-0.0.4/src/djangofoundry/scripts/lint.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/scripts/summarize.py` & `djangofoundry-0.0.4/src/djangofoundry/scripts/summarize.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/scripts/conf/sample-settings.yaml` & `djangofoundry-0.0.4/src/djangofoundry/scripts/conf/sample-settings.yaml`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/scripts/utils/__init__.py` & `djangofoundry-0.0.4/src/djangofoundry/scripts/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/scripts/utils/action.py` & `djangofoundry-0.0.4/src/djangofoundry/scripts/utils/action.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/scripts/utils/exceptions.py` & `djangofoundry-0.0.4/src/djangofoundry/scripts/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/scripts/utils/settings.py` & `djangofoundry-0.0.4/src/djangofoundry/scripts/utils/settings.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/scripts/utils/types.py` & `djangofoundry-0.0.4/src/djangofoundry/scripts/utils/types.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/signals/abstract.py` & `djangofoundry-0.0.4/src/djangofoundry/signals/abstract.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/templates/memory.html` & `djangofoundry-0.0.4/src/djangofoundry/templates/memory.html`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/templates/angular/base.html` & `djangofoundry-0.0.4/src/djangofoundry/templates/angular/base.html`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/templates/jinja/model.py.jinja` & `djangofoundry-0.0.4/src/djangofoundry/templates/jinja/model.py.jinja`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/src/djangofoundry/templatetags/syntax_highlight.py` & `djangofoundry-0.0.4/src/djangofoundry/templatetags/syntax_highlight.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/tests/foundry/test_matching.py` & `djangofoundry-0.0.4/tests/foundry/test_matching.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/tests/foundry/controllers/test_mixins.py` & `djangofoundry-0.0.4/tests/foundry/controllers/test_mixins.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/tests/foundry/decorators/test_timeout.py` & `djangofoundry-0.0.4/tests/foundry/decorators/test_timeout.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/tests/foundry/helpers/test_hooks.py` & `djangofoundry-0.0.4/tests/foundry/helpers/test_hooks.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/tests/foundry/helpers/test_queue.py` & `djangofoundry-0.0.4/tests/foundry/helpers/test_queue.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/tests/foundry/models/test_choices.py` & `djangofoundry-0.0.4/tests/foundry/models/test_choices.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/tests/foundry/models/test_queryset.py` & `djangofoundry-0.0.4/tests/foundry/models/test_queryset.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/LICENSE.md` & `djangofoundry-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/README.md` & `djangofoundry-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.3/pyproject.toml` & `djangofoundry-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "djangofoundry"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jess Mann", email="jess.a.mann+df@gmail.com" },
 ]
 description = "A collection of classes built on Django to make it easier to build web applications."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `djangofoundry-0.0.3/PKG-INFO` & `djangofoundry-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangofoundry
-Version: 0.0.3
+Version: 0.0.4
 Summary: A collection of classes built on Django to make it easier to build web applications.
 Project-URL: Homepage, https://github.com/avranu/Django-Foundry
 Project-URL: Bug Tracker, https://github.com/avranu/Django-Foundry/issues
 Author-email: Jess Mann <jess.a.mann+df@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

