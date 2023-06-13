# Comparing `tmp/djangofoundry-0.0.2.tar.gz` & `tmp/djangofoundry-0.0.3.tar.gz`

## Comparing `djangofoundry-0.0.2.tar` & `djangofoundry-0.0.3.tar`

### file list

```diff
@@ -1,114 +1,120 @@
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/.prospector.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/__init__.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/logging.conf
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/package.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/__init__.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/urls.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/controllers/__init__.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/controllers/angular.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/controllers/detail.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/controllers/generic.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/controllers/list.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/controllers/memory.py
--rw-r--r--   0        0        0    15726 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/controllers/responses.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/decorators/__init__.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/decorators/queryset_filter.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/decorators/retry.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/decorators/timeout.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/exceptions/__init__.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/exceptions/app.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/__init__.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/logging.py
--rw-r--r--   0        0        0    11832 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/progress.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/encoders/__init__.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/encoders/json.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/__init__.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/exceptions.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/hook.py
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/hooks.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/waypoint.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/meta/__init__.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/meta/constants.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/meta/types.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/queue/__init__.py
--rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/queue/queue.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/queue/signals.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/render/__init__.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/render/template.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/__init__.py
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/template.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/code/__init__.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/code/css.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/code/javascript.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/code/template.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/code/python/__init__.py
--rw-r--r--   0        0        0     9047 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/code/python/model.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/code/python/template.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/render/meta/__init__.py
--rw-r--r--   0        0        0     9226 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/helpers/render/meta/model.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/matching/__init__.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/matching/engine.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/matching/fuzzy/__init__.py
--rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/matching/fuzzy/thefuzz.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/mixins/__init__.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/mixins/dirtyfields.py
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/mixins/hasParams.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/mixins/hookable.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/mixins/jsonResponse.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/__init__.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/choices.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/manager.py
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/model.py
--rw-r--r--   0        0        0    53465 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/queryset.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/serializer.py
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/viewset.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/exceptions/__init__.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/exceptions/get.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/fields/__init__.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/fields/boolean.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/fields/char.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/fields/date.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/fields/number.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/fields/objects.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/models/fields/relationships.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/scripts/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/scripts/__init__.py
--rw-r--r--   0        0        0    12830 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/scripts/app.py
--rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/scripts/db.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/scripts/lint.py
--rw-r--r--   0        0        0     8970 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/scripts/summarize.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/scripts/conf/sample-settings.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/scripts/utils/README.md
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/scripts/utils/__init__.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/scripts/utils/action.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/scripts/utils/exceptions.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/scripts/utils/settings.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/scripts/utils/types.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/signals/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/signals/abstract.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/templates/memory.html
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/templates/angular/base.html
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/templates/jinja/model.py.jinja
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/templatetags/__init__.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/templatetags/syntax_highlight.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/types/__init__.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/src/djangofoundry/types/request.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/tests/foundry/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/tests/foundry/test_matching.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/tests/foundry/controllers/__init__.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/tests/foundry/controllers/test_mixins.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/tests/foundry/decorators/__init__.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/tests/foundry/decorators/test_timeout.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/tests/foundry/helpers/__init__.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/tests/foundry/helpers/test_hooks.py
--rw-r--r--   0        0        0     8773 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/tests/foundry/helpers/test_queue.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/tests/foundry/models/__init__.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/tests/foundry/models/test_choices.py
--rw-r--r--   0        0        0    10262 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/tests/foundry/models/test_queryset.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/.gitignore
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/LICENSE.md
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/README.md
--rw-r--r--   0        0        0    22035 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 djangofoundry-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/.dockerignore
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/.prospector.yaml
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/Dockerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/docker-compose.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/logging.conf
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/package.json
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/.devcontainer/docker-compose.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/__init__.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/urls.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/__init__.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/angular.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/detail.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/generic.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/list.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/memory.py
+-rw-r--r--   0        0        0    15504 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/controllers/responses.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/decorators/__init__.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/decorators/queryset_filter.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/decorators/retry.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/decorators/timeout.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/exceptions/__init__.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/exceptions/app.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/__init__.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/logging.py
+-rw-r--r--   0        0        0    11832 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/progress.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/encoders/__init__.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/encoders/json.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/__init__.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/exceptions.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/hook.py
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/hooks.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/waypoint.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/meta/__init__.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/meta/constants.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/meta/types.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/queue/__init__.py
+-rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/queue/queue.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/queue/signals.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/__init__.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/template.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/__init__.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/template.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/__init__.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/css.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/javascript.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/template.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/python/__init__.py
+-rw-r--r--   0        0        0     9053 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/python/model.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/python/template.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/meta/__init__.py
+-rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/helpers/render/meta/model.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/matching/__init__.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/matching/engine.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/matching/fuzzy/__init__.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/matching/fuzzy/thefuzz.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/meta/__init__.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/meta/request.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/mixins/__init__.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/mixins/dirtyfields.py
+-rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/mixins/hasParams.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/mixins/hookable.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/mixins/jsonResponse.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/__init__.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/choices.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/manager.py
+-rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/model.py
+-rw-r--r--   0        0        0    53573 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/queryset.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/serializer.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/viewset.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/exceptions/__init__.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/exceptions/get.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/__init__.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/boolean.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/char.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/date.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/number.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/objects.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/models/fields/relationships.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/README.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/__init__.py
+-rw-r--r--   0        0        0    19911 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/app.py
+-rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/db.py
+-rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/lint.py
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/summarize.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/conf/sample-settings.yaml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/utils/README.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/utils/__init__.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/utils/action.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/utils/exceptions.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/utils/settings.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/scripts/utils/types.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/signals/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/signals/abstract.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/templates/memory.html
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/templates/angular/base.html
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/templates/jinja/model.py.jinja
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/templatetags/__init__.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/src/djangofoundry/templatetags/syntax_highlight.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/test_matching.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/controllers/__init__.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/controllers/test_mixins.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/decorators/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/decorators/test_timeout.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/helpers/__init__.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/helpers/test_hooks.py
+-rw-r--r--   0        0        0     8781 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/helpers/test_queue.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/models/__init__.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/models/test_choices.py
+-rw-r--r--   0        0        0    10267 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/tests/foundry/models/test_queryset.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/README.md
+-rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 djangofoundry-0.0.3/PKG-INFO
```

### Comparing `djangofoundry-0.0.2/.prospector.yaml` & `djangofoundry-0.0.3/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/package.json` & `djangofoundry-0.0.3/package.json`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/urls.py` & `djangofoundry-0.0.3/src/djangofoundry/urls.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/controllers/angular.py` & `djangofoundry-0.0.3/src/djangofoundry/controllers/angular.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 
 		Returns:
 			An empty object.
 		"""
 		return {}
 
 	def get(self, request, *args, **kwargs):
-			return render(request, self.template_name)
+		return render(request, self.template_name)
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/controllers/detail.py` & `djangofoundry-0.0.3/src/djangofoundry/controllers/detail.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 		Copyright (c) 2022 Jess Mann
 
 """
 # Generic imports
 from __future__ import annotations
 from typing import TYPE_CHECKING, Any
 # Django Imports
-from django.core import serializers
 from django.views import generic
 from django.http import JsonResponse, HttpRequest
 # App Imports
 from djangofoundry.mixins import JSONResponseMixin
 
 if TYPE_CHECKING:
 	pass
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/controllers/generic.py` & `djangofoundry-0.0.3/src/djangofoundry/controllers/generic.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/controllers/list.py` & `djangofoundry-0.0.3/src/djangofoundry/controllers/list.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 		-----
 
 		Copyright (c) 2022 Jess Mann
 
 """
 # Generic imports
 from __future__ import annotations
-import re
 # Django Imports
 from django.views import generic
 # Lib Imports
 # App Imports
 
 
 class ListController(generic.ListView):
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/controllers/memory.py` & `djangofoundry-0.0.3/src/djangofoundry/controllers/memory.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/controllers/responses.py` & `djangofoundry-0.0.3/src/djangofoundry/controllers/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 #
 # Generic Responses
 #
 class Response(response.Response):
 	"""
 	Represents a generic response. This is the base class for all responses.
 	"""
-	def __init__(self, data=None, status=None, template_name=None, headers=None, exception=False, content_type=None):
-		super().__init__(data, status, template_name, headers, exception, content_type)
 
 class SuccessResponse(Response):
 	"""
 	Represents a successful response. This is the base class for all successful responses.
 	"""
 	def __init__(self, data=None, status=200, template_name=None, headers=None, exception=False, content_type=None):
 		if not data:
@@ -67,16 +65,14 @@
 	def __init__(self, data=dict, status=200, template_name=None, headers=None, exception=False, content_type=None):
 		super().__init__(data, status, template_name, headers, exception, content_type)
 
 class PaginatedResponse(DataResponse):
 	"""
 	Represents a successful HTTP Code 200 response with paginated data. This is the base class for all successful responses with paginated data.
 	"""
-	from typing import Any
-
 	class DataResponse(OkResponse):
 		"""
 		Represents a successful HTTP Code 200 response with data. This is the base class for all successful responses with data.
 		"""
 		def __init__(self, data: Optional[dict[str, Any]] = None, status=200, template_name=None, headers=None, exception=False, content_type=None):
 			if not data:
 				data = {}
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/decorators/queryset_filter.py` & `djangofoundry-0.0.3/src/djangofoundry/decorators/queryset_filter.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/decorators/retry.py` & `djangofoundry-0.0.3/src/djangofoundry/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/decorators/timeout.py` & `djangofoundry-0.0.3/src/djangofoundry/decorators/timeout.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/exceptions/app.py` & `djangofoundry-0.0.3/src/djangofoundry/exceptions/app.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/logging.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/progress.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/progress.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/__init__.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/exceptions.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/exceptions.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/hook.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/hooks.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/hooks.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/waypoint.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/waypoint.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 """
 # Generic imports
 from __future__ import annotations
 from typing import TYPE_CHECKING, Any, Iterable, Optional
 from djangofoundry.helpers.hooks.meta.constants import DEFAULT_NAMESPACE
 
 if TYPE_CHECKING:
-	from .hook import Hook
+	from djangofoundry.helpers.hooks.hook import Hook
 
 class Waypoint:
 	"""
 	A waypoint is a place in our code where a hook can be registered and run.
 
 	Attributes:
 		name (str):
@@ -51,17 +51,17 @@
 	return_type : Any
 	hooks : list[Hook]
 
 	def __init__(self,
 			name : str,
 			namespace : str = DEFAULT_NAMESPACE,
 			positional_arguments : int = 0,
-	 		named_arguments : list[str] = [],
+	 		named_arguments : list[str] = list,
 		 	return_type : Any = Any,
-		  	hooks : list[Hook] = []):
+		  	hooks : list[Hook] = list):
 		self.name = name
 		self.namespace = namespace
 		self.positional_arguments = positional_arguments
 		self.named_arguments = named_arguments
 		self.return_type = return_type
 		self.hooks = hooks
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/meta/constants.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/meta/constants.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/hooks/meta/types.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/hooks/meta/types.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/queue/queue.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/queue/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 
 		-----
 
 		Copyright (c) 2022 Jess Mann
 """
 # Generic imports
 from __future__ import annotations
-from ctypes import Array
-from typing import Any, Callable, Iterable, Optional
+from typing import Any, Callable, Optional
 from typing_extensions import Self
 from psqlextra.query import ConflictAction
 import queue
 from collections import deque
 # Django Imports
 # Lib Imports
 from djangofoundry.helpers.queue import signals
@@ -177,15 +176,15 @@
 
 		# Initialize the callbacks and merge with anything we passed in.
 		if self.callbacks is None:
 			self.callbacks = { callback : None for callback, _x in Callbacks.choices }
 		else:
 			# Allow setting callbacks in the subclass definition (even though doing that is probably a bad idea... supporting it eliminates unexpected behavior)
 			self.callbacks = { callback : None for callback, _x in Callbacks.choices } | self.callbacks
-		
+
 		if callbacks:
 			self.callbacks.update(callbacks)
 
 	def __enter__(self) -> Self:
 		'''
 		Allow this to be used in a with block.
 		'''
@@ -224,15 +223,15 @@
 			return None
 
 		# Call the callback with any args we passed in, and return any result we get.
 		cb = self.callbacks[callback_name]
 
 		if cb:
 			return cb(**kwargs)
-		
+
 		return None
 
 	# TODO: warning on unsaved queue on __del__
 
 	def defer_save(self, value: bool = True) -> None:
 		"""
 		Convenience method for queue.save_deferred = True; queue.allow_save()
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/queue/signals.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/queue/signals.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/render/template.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/render/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/template.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 			template_suffix (str, optional): The suffix for the templates. Defaults to '.jinja'.
 
 		Raises:
 			ValueError: If app_name is None.
 		"""
 		if app_name is None:
 			raise ValueError('app_name cannot be None')
-		
+
 		if autoescape is None:
 			autoescape = ['html', 'xml']
 
 		super().__init__(app_name, template_path, template_suffix)
 
 		self.autoescape = autoescape
 
@@ -76,15 +76,15 @@
 		"""
 		logger.debug(f'Setting up jinja environment: {self.app_name} : {self.template_path}')
 		self._env = Environment(
 			loader=PackageLoader(self.app_name, self.template_path),
 			autoescape=select_autoescape(self.autoescape)
 		)
 
-	def render(self, template_name: str, variables: dict) -> str | None:
+	def render(self, variables: dict, template_name: str) -> str | None:
 		"""
 		Render a template with the given variables.
 
 		Args:
 			template_name (str): The name of the template to render.
 			variables (dict): The variables to pass to the template.
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/code/css.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/css.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/code/javascript.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/javascript.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/code/template.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/template.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,25 +29,25 @@
 	"""
 	A helper class for rendering jinja templates that create code.
 
 	Attributes:
 		env (Environment): The jinja environment.
 	"""
 
-	def suggest_class_name(self, input: str) -> str:
+	def suggest_class_name(self, input_str: str) -> str:
 		"""
 		Suggest a class name based on a set of input. This method exists primarily to establish an interface for subclasses.
 
 		Args:
 			input (str): The input to base the suggested name on
 
 		Returns:
 			str: The suggested class name
 		"""
 
 		# Remove any non-alpha and title case
-		cleaned_name = re.sub(r'[^a-zA-Z]+', ' ', input).title().replace(' ', '')
+		cleaned_name = re.sub(r'[^a-zA-Z]+', ' ', input_str).title().replace(' ', '')
 
 		# Limit to 30 characters
 		cleaned_name = cleaned_name[:30]
 
 		return cleaned_name
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/code/python/model.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/python/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from jinja2 import TemplateNotFound
 # DJANGO imports
 from django.db import connections
 from django.db.backends.utils import CursorWrapper
 # LIB imports
 from djangofoundry.helpers.render.meta.model import IndexInfo, IndexColumnInfo, ColumnInfo, ConstraintInfo
 from djangofoundry.helpers.render.jinja.code.python.template import PythonHelper
+from djangofoundry.models import Model
 
 # Set up logging for this module
 logger = logging.getLogger(__name__)
 
 class ModelHelper(PythonHelper):
 	"""
 	A helper class for rendering jinja templates that create django models.
@@ -102,15 +103,15 @@
 		if not table_name:
 			table_name = self.table_name
 
 		# Remove any prefixes or suffixes (e.g. PS_, _TMP)
 		cleaned_name = self.humanize_table_name(table_name)
 		result = "".join(part.capitalize() for part in cleaned_name.split(' '))
 		if len(result) < 2:
-			logger.warn(f'suggest_model_name too short for {table_name} -> {cleaned_name} -> {result}')
+			logger.warning(f'suggest_model_name too short for {table_name} -> {cleaned_name} -> {result}')
 			return table_name
 
 		return result
 
 	def humanize_table_name(self, table_name : Optional[str] = None) -> str:
 		"""
 		Converts a messy table name to a cleaner, more human-readable format.
@@ -131,15 +132,15 @@
 		if not cleaned_name or len(cleaned_name) < 3:
 			logger.warning(f'Could not clean table name: "{table_name}" -> "{cleaned_name}"')
 			return table_name
 
 		# Split into words, and capitalize each word
 		result = re.sub(r'[\s_]+', ' ', cleaned_name).title()
 		if len(result) < 2:
-			logger.warn(f'humanize_name too short for {table_name} -> {cleaned_name} -> {result}')
+			logger.warning(f'humanize_name too short for {table_name} -> {cleaned_name} -> {result}')
 			return table_name
 		return result
 
 	@classmethod
 	def remove_duplicate_indexes(cls, indexes: List[IndexInfo]) -> List[IndexInfo]:
 		"""
 		Remove duplicate indexes from the list of indexes.
@@ -162,15 +163,14 @@
 
 		Args:
 			table_name (str): The name of the table to get columns for
 
 		Returns:
 			List[ColumnInfo]: The list of columns for the given table
 		"""
-		from models.abstract import Model
 		if not table_name:
 			table_name = self.table_name
 
 		# Query the DB for the columns directly using connection.cursor().execute()
 		with self.cursor as cursor:
 			# Get the column details from the ALL_TAB_COLUMNS view
 			cursor.execute(f"""
@@ -285,15 +285,15 @@
 		# Query the DB for the row count directly using connection.cursor().execute()
 		with self.cursor as cursor:
 			cursor.execute(f'SELECT COUNT(*) FROM "{self.schema}"."{self.table_name}"')
 			result = cursor.fetchone()
 
 			if not result:
 				return 0
-			
+
 			return result[0]
 
 	def render(self, variables: dict, template_name: str = 'model') -> str | None:
 		"""
 		Render a template with the given variables.
 
 		Args:
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/render/jinja/code/python/template.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/render/jinja/code/python/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/helpers/render/meta/model.py` & `djangofoundry-0.0.3/src/djangofoundry/helpers/render/meta/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 		data_type: str,
 		data_length: int,
 		nullable: str,
 		data_default: Any,
 		precision: Optional[int] = None,
 		scale: Optional[int] = None,
 	):
-		self.name = name
+		super().__init__(name)
 		self.data_type = data_type
 		self.data_length = data_length
 		self.precision = precision
 		self.scale = scale
 		self.default = data_default
 
 		match nullable.lower():
@@ -191,15 +191,15 @@
 	Store information about a column in an index in Oracle.
 
 	Atributes:
 		name (str): The name of the column
 		position (int): The position of the column in the index
 	"""
 	def __init__(self, name: str, position: int):
-		self.name = name
+		super().__init__(name)
 		self.position = position
 
 	def __eq__(self, other: 'IndexColumnInfo') -> bool:
 		return self.name == other.name and self.position == other.position
 
 	def __hash__(self) -> int:
 		return hash((self.name, self.position))
@@ -228,15 +228,15 @@
 		uniqueness (str): Whether or not the index is unique
 		columns (list[IndexColumnInfo]): The columns in the index
 	"""
 
 	def __init__(self, name: str, columns: Optional[list[IndexColumnInfo]] = None, uniqueness: str = ''):
 		if not name or name == '':
 			name = f'index.{"-".join([column.name for column in columns or []])}'
-		self.name = name
+		super().__init__(name)
 		self.uniqueness = uniqueness
 		self.columns = columns if columns is not None else []
 
 	def add_column(self, column_name: str, column_position: int):
 		"""
 		Add a column to the index.
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/matching/engine.py` & `djangofoundry-0.0.3/src/djangofoundry/matching/engine.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/matching/fuzzy/thefuzz.py` & `djangofoundry-0.0.3/src/djangofoundry/matching/fuzzy/thefuzz.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 
 from __future__ import annotations
 from typing import Iterable
 from thefuzz import fuzz, process
 from djangofoundry.matching.engine import MatchingEngine
 
 class TheFuzz(MatchingEngine):
+	"""
+	A matching engine that uses thefuzz library to match strings
+	"""
 
 	def choose( self, input_str : str, choices : Iterable[str], required_confidence : int = 90 ) -> tuple[str | None, int]:
 		"""
 		Use the matching engine to pick the best option from a group of options
 
 		Args:
 			input_str (str):
@@ -45,15 +48,15 @@
 			Match: The matching choice, or None
 			Confidence: The confidence of the match, from 1-100
 		"""
 		results = process.extractOne(str(input_str), choices, score_cutoff=required_confidence)
 
 		if results is None:
 			return (None, 0)
-		
+
 		# Check if there are 2 or 3 values in the tuple, and unpack
 		if len(results) == 2:
 			(matching_key, confidence) = results
 		else:
 			(matching_key, confidence, _index) = results
 
 		# Sufficient match!
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/mixins/dirtyfields.py` & `djangofoundry-0.0.3/src/djangofoundry/mixins/dirtyfields.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/mixins/hasParams.py` & `djangofoundry-0.0.3/src/djangofoundry/mixins/hasParams.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 		-----
 
 		Copyright (c) 2022 Jess Mann
 """
 from __future__ import annotations
 # Generic imports
-from typing import Any, Iterable, TypeVar
+from typing import Iterable, TypeVar
 import re
 import logging
 
 # Get a logger for logging messages
 #
 # Set up logging for this module. __name__ includes the namespace (e.g. dashboard.models.cases).
 #
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/mixins/hookable.py` & `djangofoundry-0.0.3/src/djangofoundry/mixins/hookable.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/mixins/jsonResponse.py` & `djangofoundry-0.0.3/src/djangofoundry/mixins/jsonResponse.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/models/choices.py` & `djangofoundry-0.0.3/src/djangofoundry/models/choices.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/models/manager.py` & `djangofoundry-0.0.3/src/djangofoundry/models/manager.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/models/model.py` & `djangofoundry-0.0.3/src/djangofoundry/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from typing import Iterable, Optional
 import logging
 # Django Imports
 from django.db import models
 # Django extensions
 import auto_prefetch
 # Lib Imports
-from mixins import Hookable
+from djangofoundry.mixins import Hookable
 # App Imports
 from djangofoundry.models.manager import PostgresManager
 
 # Set up a logger for this module.
 #
 # Set up logging for this module. __name__ includes the namespace (e.g. dashboard.models.cases).
 #
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/models/queryset.py` & `djangofoundry-0.0.3/src/djangofoundry/models/queryset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-
-
 	Metadata:
 
 		File: queryset.py
 		Project: Django Foundry
 		Created Date: 18 Aug 2022
 		Author: Jess Mann
 		Email: jess.a.mann@gmail.com
@@ -332,18 +330,18 @@
 		raise NotImplementedError(f'Bad Queryset filter requested: {filter_name}')
 
 	def filter_by_related(self, foreign_key: str, filter_expression: Q, alias_name: Optional[str] = None) -> Self:
 		'''
 		Filters this model based on the existence of a related model with a given property
 
 		Args:
-			filter (django.db.models.Q):
-				The filter to test against the related model
 			foreign_key (str):
 				The name of the foreign key on this model
+			filter_expression (Q):
+				The filter to apply to the related model
 			alias_name (str, optional):
 				The name of the alias to use. If None is provided, we will generate one. Defaults to None.
 
 		Returns:
 			QuerySet: A filtered copy of this queryset
 
 		Example:
@@ -1002,22 +1000,22 @@
 			List[str]: The names of the fields that are correlated with the given field
 
 		Example:
 			>>> Case.objects.find_correlated_fields('processing_time')
 			['tasks']
 		"""
 		# Get the correlation of the field with every other field
-		correlations = {field_name: self.correlation(field_name, field_name) for field_name in self.model._meta.get_fields() if (field_name != field_name and self.field_is_numeric(field_name))}
-		correlations = {field_name: correlation for field_name, correlation in correlations.items() if correlation >= threshold}
+		correlations = {correlated_field_name: self.correlation(field_name, correlated_field_name) for correlated_field_name in self.model._meta.get_fields() if (field_name != correlated_field_name and self.field_is_numeric(correlated_field_name))}
+		correlations = {correlated_field_name: correlation for correlated_field_name, correlation in correlations.items() if correlation >= threshold}
 
 		# Sort the correlations by their correlation
 		correlations = sorted(correlations.items(), key=lambda item: item[1], reverse=True)
 
 		# Return the names of the correlated fields
-		return [field_name for field_name, _correlation in correlations]
+		return [correlated_field_name for correlated_field_name, _correlation in correlations]
 
 	def linear_regression(self, field_name_x: str, field_name_y: str) -> Tuple[float, float]:
 		"""
 		Get the linear regression of two fields.
 
 		The linear regression is a tuple of the slope and y-intercept of the line of best fit.
 		It is useful for predicting the value of one field given the value of another field.
@@ -1172,15 +1170,15 @@
 		"""
 		# Get the entries that match the search term
 		if fields is None:
 
 			# Get fields that are searchable
 			fields = [field.name for field in self.model._meta.get_fields() if not field.is_relation]
 
-		entries = self.filter(Q(**{'{}__icontains'.format(field): search_term}) for field in fields)
+		entries = self.filter(Q(**{f'{format(field)}__icontains': search_term}) for field in fields)
 		return entries
 
 	def annotate_duration(self, start_field: str, end_field: str, alias: str = 'duration') -> Self:
 		"""
 		Annotate the entries with the duration between two fields.
 
 		Args:
@@ -1212,15 +1210,15 @@
 			Self: The entries within the date range
 
 		Example:
 			>>> Case.objects.date_range(datetime(2020, 1, 1), datetime(2020, 1, 31), 'date')
 			[<Case: Case object (1)>, <Case: Case object (2)>, <Case: Case object (3)>, <Case: Case object (4)>, <Case: Case object (5)>]
 		"""
 		# Get the entries within a date range
-		entries = self.filter(**{'{}__range'.format(date_field): [start_date, end_date]})
+		entries = self.filter(**{f"{format(date_field)}__range": [start_date, end_date]})
 		return entries
 
 	def rolling_mean(self, field_name: str, window: int) -> List[float]:
 		"""
 		Get the rolling mean of a field.
 
 		The rolling mean represents the average of the last n values, where n is the window size.
@@ -1474,17 +1472,17 @@
 			QuerySet: The anomalies
 
 		Example:
 			>>> Case.objects.detect_anomalies()
 			<QuerySet [<Case: Case object (1)>, <Case: Case object (2)>]>
 		"""
 		# Get all fields that are numeric
-		fields = [field.name for field in self.model._meta.get_fields() if self.field_is_numeric(field)]
+		numeric_fields = [field.name for field in self.model._meta.get_fields() if self.field_is_numeric(field)]
 
 		# Construct a filter for each field, so that we return all anomalies (using OR) rather than just entries that are anomalous in all fields (using AND)
 		filters = []
-		for i, field in enumerate(fields):
-			filter = Q(**{f"{field}__in": self.filter_anomalies_in(field, method, z_threshold, iqr_multiplier).values_list(field, flat=True)})
-			filters.append(filter)
+		for _i, field in enumerate(numeric_fields):
+			filter_q = Q(**{f"{field}__in": self.filter_anomalies_in(field, method, z_threshold, iqr_multiplier).values_list(field, flat=True)})
+			filters.append(filter_q)
 
 		# Filter the queryset using the OR of all the filters
 		return self.filter(reduce(operator.or_, filters))
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/models/serializer.py` & `djangofoundry-0.0.3/src/djangofoundry/models/serializer.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 		Copyright (c) 2022 Jess Mann
 """
 # Generic imports
 from __future__ import annotations
 from rest_framework import serializers
 
 class Serializer(serializers.ModelSerializer):
+	"""
+	A base serializer class that can be used to dynamically include or exclude fields based on context.
+	"""
 
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 
 		# Dynamically include or exclude fields based on context
 		context = kwargs.get('context', {})
 		exclude_fields = context.get('exclude_fields', [])
@@ -40,14 +43,17 @@
 			allowed = set(include_fields)
 			for field in list(self.fields):
 				if field not in allowed:
 					self.fields.pop(field)
 
 	@classmethod
 	def get_fieldnames(cls) -> list:
+		"""
+		Get a list of field names for this model.
+		"""
 		return cls.Meta.fields
 
 	@classmethod
 	def get_native_fields(cls) -> list:
 		"""
 		Get fields that are native to this model, (i.e. normal fields), not generated or calculated properties.
 
@@ -57,11 +63,14 @@
 		fields = cls.get_fieldnames()
 		for field in cls.Meta.generated_fields:
 			if field in fields:
 				fields.remove(field)
 		return fields
 
 	class Meta:
+		"""
+		Serializer metadata.
+		"""
 		fields = [
 			'id'
 		]
 		generated_fields = []
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/models/viewset.py` & `djangofoundry-0.0.3/src/djangofoundry/models/viewset.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/models/exceptions/get.py` & `djangofoundry-0.0.3/src/djangofoundry/models/exceptions/get.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/models/fields/__init__.py` & `djangofoundry-0.0.3/src/djangofoundry/models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/models/fields/char.py` & `djangofoundry-0.0.3/src/djangofoundry/models/fields/char.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 		if max_length > 1:
 			raise ValueError(f'Trying to initialize a single character field with a length of {max_length}')
 
 		super().__init__(max_length=max_length, **kwargs)
 
 
 class RowIdField(CharField):
+	"""
+	A charfield that is used for storing row ids (from databases like Oracle)
+	"""
 	def __init__(self, *,
 				 map_field  : Optional[str] = None,
 				 max_length : int = 18,
 				 unique	 : bool = True,
 				 null	   : bool = False,
 				 blank	  : bool = False,
 				 editable   : bool = False,
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/models/fields/date.py` & `djangofoundry-0.0.3/src/djangofoundry/models/fields/date.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/models/fields/number.py` & `djangofoundry-0.0.3/src/djangofoundry/models/fields/number.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/models/fields/objects.py` & `djangofoundry-0.0.3/src/djangofoundry/models/fields/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,17 @@
 		-----
 
 		Copyright (c) 2022 Jess Mann
 
 """
 # Generic imports
 from __future__ import annotations
-from typing import Any
 # Django imports
 from django.db import models
 from django.db.models import Func
-from django.db.models.expressions import Combinable
 # 3rd Party imports
 from psqlextra import fields
 import picklefield.fields
 
 class HStoreField(fields.HStoreField):
 	"""
 	An HStoreField that uses the psqlextra library.
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/models/fields/relationships.py` & `djangofoundry-0.0.3/src/djangofoundry/models/fields/relationships.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/scripts/__init__.py` & `djangofoundry-0.0.3/src/djangofoundry/scripts/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,11 +21,19 @@
 		Last Modified: Sat Dec 03 2022
 		Modified By: Jess Mann
 
 		-----
 
 		Copyright (c) 2022 Jess Mann
 """
-# Do not import anything here, because we don't want these files imported elsewhere.
-from djangofoundry.scripts.utils import *
+from djangofoundry.scripts.utils import (
+    EnumAction,
+    Settings,
+    AppException,
+    FileEmptyError,
+    DbError,
+    DbConnectionError,
+    DbStartError,
+    UnsupportedCommandError
+)
 from djangofoundry.scripts.app import App
 from djangofoundry.scripts.db import Db
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/scripts/db.py` & `djangofoundry-0.0.3/src/djangofoundry/scripts/db.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/scripts/lint.py` & `djangofoundry-0.0.3/src/djangofoundry/scripts/lint.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 		Copyright (c) 2023 Jess Mann
 """
 from __future__ import annotations
 import os
 import argparse
 import re
-import yaml
 import glob
+import yaml
 import openai
 from tqdm import tqdm
 
 class ChatGPTBugFixer:
 	def __init__(self, api_key, project_path):
 		openai.api_key = api_key
 		self.project_path = project_path
@@ -169,27 +169,27 @@
 						print(f"\nChatGPT did not return suggestions for {file_path}")
 			except Exception as e:
 				print(f"\nError processing file {file_path}: {e}")
 
 def main(args):
 	try:
 		try:
-			with open(args.settings, "r") as file:
+			with open(args.settings, "r", encoding="utf-8") as file:
 				settings = yaml.safe_load(file)
 				openai_api_key = settings['lint']["key"]
 		except Exception as e:
 			print(f"Error loading settings: {e}")
 			return
 
 		bugfixer = ChatGPTBugFixer(openai_api_key, args.path)
 		bugfixer.process_python_files()
-	except KeyboardInterrupt as e:
+	except KeyboardInterrupt:
 		print("Exiting...")
 
 if __name__ == "__main__":
 	parser = argparse.ArgumentParser(description="Check Python files for bugfixes and improvements using ChatGPT")
 	parser.add_argument("--settings", default="conf/settings.yaml", help="Path to the settings.yaml file")
 	parser.add_argument("--path", "-p", default="../lib/", help="Path to the project folder")
 	parser.add_argument("--max", "-m", default=0, type=int, help="Maximum number of files to process (default: 0, i.e. no limit)")
-	args = parser.parse_args()
+	parser_args = parser.parse_args()
 
-	main(args)
+	main(parser_args)
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/scripts/conf/sample-settings.yaml` & `djangofoundry-0.0.3/src/djangofoundry/scripts/conf/sample-settings.yaml`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/scripts/utils/action.py` & `djangofoundry-0.0.3/src/djangofoundry/scripts/utils/action.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/scripts/utils/exceptions.py` & `djangofoundry-0.0.3/src/djangofoundry/scripts/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/scripts/utils/settings.py` & `djangofoundry-0.0.3/src/djangofoundry/scripts/utils/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 
 		Copyright (c) 2022 Jess Mann
 """
 # Generic imports
 from __future__ import annotations
 import os
 from typing import Any
-import yaml
-from yaml.loader import SafeLoader
 import logging
 import logging.config
+import yaml
+from yaml.loader import SafeLoader
 # App imports
 from djangofoundry.scripts.utils.exceptions import FileEmptyError
-from djangofoundry.scripts.utils.types import *
+from djangofoundry.scripts.utils.types import SettingsFile, SettingsLog
 
 SETTINGS_PATH : str = '../conf/settings.yaml'
 
 class Settings:
 	"""
 	Settings for our application (used in /bin files only).
 
@@ -43,33 +43,33 @@
 	def __init__(self, settings_path : str = SETTINGS_PATH):
 		# Load our settings
 		self.load_config(settings_path)
 
 		# If we still don't have any settings, then raise an error
 		if not self._settings:
 			raise FileEmptyError(f'No settings found in {settings_path}')
-	
+
 	@property
 	def settings(self) -> SettingsFile:
 		# If settings has never been loaded, then load it.
 		if not self._settings:
 			self.load_config()
 
 			if not self._settings:
 				raise FileEmptyError(f'No settings found in {SETTINGS_PATH}')
 
 		# It should exist now
 		return self._settings
 
-	
+
 	@property
 	def logging(self) -> SettingsLog:
 		return self.settings.get('logging')
 
-	
+
 	def getLogger(self, namespace : str):
 		"""
 		Sets up the logger once (and only once), then returns a logger for the module requested.
 		"""
 		# Setup logging if it isn't already
 		if self._logging_setup is not True:
 			try:
@@ -78,45 +78,45 @@
 				print(f'Unable to set up logging: {e}')
 				raise e from e
 			self._logging_setup = True
 
 		# Create a new logger
 		return logging.getLogger(namespace)
 
-	
+
 	def load_config(self, settings_path : str = SETTINGS_PATH) -> SettingsFile:
 		# Read our default sensitivity settings (if available)
 		filepath = os.path.join(os.path.dirname(os.path.abspath(__file__)), settings_path)
 
 		if os.path.exists(filepath):
 			# If it exists, then open it
-			with open(filepath) as file:
-				# Load the contents into a variable
+			with open(filepath, encoding='utf-8') as file:
+	     		# Load the contents into a variable
 				self._settings = yaml.load(file, Loader=SafeLoader)
 		else:
 			# Let everyone know we couldn't find the settings. This likely exits.
 			raise FileNotFoundError(f"Could not load bin settings from {filepath}")
 
 		# Validate contents of settings file.
 		if self._settings == {}:
 			raise FileEmptyError(f'No data in settings file at f{filepath}')
 
 		return self._settings
 
-	
+
 	def all(self) -> SettingsFile:
 		"""
 		Makes the syntax for getting the settings dict a little less clunky (i.e. Settings.all() instead of Settings.settings)
 
 		Returns:
 			dict: A dictionary of settings.
   		"""
 		return self.settings
 
-	
+
 	def get(self, key : str) -> Any:
 		"""
 		Retrieves the value at the provided key.
 
 		Args:
 			key (str): A key to retrieve
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/scripts/utils/types.py` & `djangofoundry-0.0.3/src/djangofoundry/scripts/utils/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 		-----
 
 		Copyright (c) 2022 Jess Mann
 """
 # Generic imports
 from __future__ import annotations
 from enum import Enum
-from typing import Any, TypedDict
+from typing import TypedDict
 
 class LoggerLevels(Enum):
 	"""
 	Enum for the different logging levels.
 	"""
 	DEBUG = 'debug'
 	INFO = 'info'
@@ -61,14 +61,17 @@
 	"""
 	level: LoggerLevels
 	formatter: str
 	stream: str
 	#class: str
 
 class LogRoot(TypedDict):
+	"""
+	Expected format for the "root" logger in the settings file.
+	"""
 	level: LoggerLevels
 	handlers: list[LogHandler]
 
 class SettingsLog(TypedDict):
 	"""
 	Expected format for the logging portion of the settings file.
```

### Comparing `djangofoundry-0.0.2/src/djangofoundry/signals/abstract.py` & `djangofoundry-0.0.3/src/djangofoundry/signals/abstract.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/templates/memory.html` & `djangofoundry-0.0.3/src/djangofoundry/templates/memory.html`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/templates/angular/base.html` & `djangofoundry-0.0.3/src/djangofoundry/templates/angular/base.html`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/templates/jinja/model.py.jinja` & `djangofoundry-0.0.3/src/djangofoundry/templates/jinja/model.py.jinja`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/src/djangofoundry/templatetags/syntax_highlight.py` & `djangofoundry-0.0.3/src/djangofoundry/templatetags/syntax_highlight.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/tests/foundry/test_matching.py` & `djangofoundry-0.0.3/tests/foundry/test_matching.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/tests/foundry/controllers/test_mixins.py` & `djangofoundry-0.0.3/tests/foundry/controllers/test_mixins.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from __future__ import annotations
 
 import re
 # Django imports
 from django.test import TestCase
 from django.views import View
 # Lib imports
-from controllers.mixins import HasParams
+from djangofoundry.controllers.mixins import HasParams
 # App imports
 
 class Sample(HasParams, View):
 	pass
 
 class HasParamsTest(TestCase):
```

### Comparing `djangofoundry-0.0.2/tests/foundry/decorators/test_timeout.py` & `djangofoundry-0.0.3/tests/foundry/decorators/test_timeout.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 		-----
 
 		Copyright (c) 2023 Jess Mann
 """
 from time import sleep
 from django.test import TestCase
-from decorators.timeout import timeout
+from djangofoundry.decorators.timeout import timeout
 
 '''
 class TimeoutTestCase(TestCase):
 	def test_timeout_decorator(self):
 		@timeout(1)
 		def sample_function():
 			sleep(2)
```

### Comparing `djangofoundry-0.0.2/tests/foundry/helpers/test_hooks.py` & `djangofoundry-0.0.3/tests/foundry/helpers/test_hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 		Modified By: Jess Mann
 
 		-----
 
 		Copyright (c) 2023 Jess Mann
 """
 from django.test import TestCase
-from helpers.hooks.meta.types import WaypointMap
-from helpers.hooks.waypoint import Waypoint
-from helpers.hooks.hook import Hook, DEFAULT_NAMESPACE, DEFAULT_PRIORITY
+from djangofoundry.helpers.hooks.meta.types import WaypointMap
+from djangofoundry.helpers.hooks.waypoint import Waypoint
+from djangofoundry.helpers.hooks.hook import Hook, DEFAULT_NAMESPACE, DEFAULT_PRIORITY
 
 class TestHook(TestCase):
 
 	def setUp(self):
 		self.action = lambda x: x * 2
 		self.hook = Hook("test_hook", self.action)
```

### Comparing `djangofoundry-0.0.2/tests/foundry/helpers/test_queue.py` & `djangofoundry-0.0.3/tests/foundry/helpers/test_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import re
 from collections import deque
 # Django imports
 from django.test import TestCase
 from model_bakery import baker
 # Lib imports
-from helpers.queue.queue import Queue
+from djangofoundry.helpers.queue import Queue
 # App imports
 
 MAX_SIZE = 3
 
 '''
 class QueueTest(TestCase):
```

### Comparing `djangofoundry-0.0.2/tests/foundry/models/test_choices.py` & `djangofoundry-0.0.3/tests/foundry/models/test_choices.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from datetime import date, datetime
 import decimal
 from typing import Iterable
 from dateutil.parser import ParserError
 # Django imports
 from django.test import TestCase
 # Lib imports
-from models.choices import TextChoices
+from djangofoundry.models.choices import TextChoices
 # App imports
 
 
 class ChoicesTest(TestCase):
 
 	def setUp(self):
 		pass
```

### Comparing `djangofoundry-0.0.2/tests/foundry/models/test_queryset.py` & `djangofoundry-0.0.3/tests/foundry/models/test_queryset.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 		-----
 
 		Copyright (c) 2023 Jess Mann
 """
 from math import sqrt
 from django.test import TestCase
 from model_bakery import baker
-from models.abstract import QuerySet
 from django.db.models import Q
 from unittest.mock import MagicMock
+from djangofoundry.models import QuerySet
 
 # Create a mock model using model_bakery
 class Case:
 	objects = QuerySet.as_manager()
 
 class QuerySetTestCase(TestCase):
 	model = Case
```

### Comparing `djangofoundry-0.0.2/LICENSE.md` & `djangofoundry-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/README.md` & `djangofoundry-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.2/pyproject.toml` & `djangofoundry-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "djangofoundry"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Jess Mann", email="jess.a.mann+df@gmail.com" },
 ]
 description = "A collection of classes built on Django to make it easier to build web applications."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -376,15 +376,15 @@
 # multiple times (only on the command line, not in the configuration file where
 # it should appear only once). You can also use "--disable=all" to disable
 # everything first and then re-enable specific checks. For example, if you want
 # to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use "--disable=all --enable=classes
 # --disable=W".
-disable = ["raw-checker-failed", "bad-inline-option", "locally-disabled", "file-ignored", "suppressed-message", "useless-suppression", "deprecated-pragma", "use-symbolic-message-instead", "missing-function-docstring", "redundant-returns-doc", "pointless-string-statement", "multiple-imports", "missing-final-newline", "empty-comment", "too-few-public-methods", "too-many-lines", "broad-exception-caught", "invalid-name", "logging-fstring-interpolation", "too-many-ancestors"]
+disable = ["raw-checker-failed", "bad-inline-option", "locally-disabled", "file-ignored", "suppressed-message", "useless-suppression", "deprecated-pragma", "use-symbolic-message-instead", "missing-function-docstring", "redundant-returns-doc", "pointless-string-statement", "multiple-imports", "missing-final-newline", "empty-comment", "too-few-public-methods", "too-many-lines", "broad-exception-caught", "invalid-name", "logging-fstring-interpolation", "too-many-ancestors", "too-many-public-methods", "too-many-arguments", "trailing-newlines", "too-many-instance-attributes", "unnecessary-pass"]
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where it
 # should appear only once). See also the "--disable" option for examples.
 enable = ["c-extension-no-member"]
```

### Comparing `djangofoundry-0.0.2/PKG-INFO` & `djangofoundry-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangofoundry
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of classes built on Django to make it easier to build web applications.
 Project-URL: Homepage, https://github.com/avranu/Django-Foundry
 Project-URL: Bug Tracker, https://github.com/avranu/Django-Foundry/issues
 Author-email: Jess Mann <jess.a.mann+df@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

