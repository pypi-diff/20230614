# Comparing `tmp/rasa-3.6.0.tar.gz` & `tmp/rasa-3.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa-3.6.0.tar", max compression
+gzip compressed data, was "rasa-3.6.0a1.tar", max compression
```

## Comparing `rasa-3.6.0.tar` & `rasa-3.6.0a1.tar`

### file list

```diff
@@ -1,315 +1,314 @@
--rw-r--r--   0        0        0    11352 2023-06-14 15:11:25.707869 rasa-3.6.0/LICENSE.txt
--rw-r--r--   0        0        0    21489 2023-06-14 15:11:25.707869 rasa-3.6.0/README.md
--rw-r--r--   0        0        0     9927 2023-06-14 15:11:25.891866 rasa-3.6.0/pyproject.toml
--rw-r--r--   0        0        0      280 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/__init__.py
--rw-r--r--   0        0        0     5441 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/__main__.py
--rw-r--r--   0        0        0     5314 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/api.py
--rw-r--r--   0        0        0      115 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/arguments/__init__.py
--rw-r--r--   0        0        0     2388 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/arguments/data.py
--rw-r--r--   0        0        0     5242 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/arguments/default_arguments.py
--rw-r--r--   0        0        0     2199 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/arguments/evaluate.py
--rw-r--r--   0        0        0     1499 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/arguments/export.py
--rw-r--r--   0        0        0     2685 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/arguments/interactive.py
--rw-r--r--   0        0        0     5674 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/arguments/run.py
--rw-r--r--   0        0        0      367 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/arguments/shell.py
--rw-r--r--   0        0        0     6853 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/arguments/test.py
--rw-r--r--   0        0        0     8279 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/arguments/train.py
--rw-r--r--   0        0        0      861 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/arguments/visualize.py
--rw-r--r--   0        0        0     1027 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/arguments/x.py
--rw-r--r--   0        0        0     9506 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/data.py
--rw-r--r--   0        0        0     7948 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/evaluate.py
--rw-r--r--   0        0        0     8204 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/export.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/initial_project/actions/__init__.py
--rw-r--r--   0        0        0      742 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/initial_project/actions/actions.py
--rw-r--r--   0        0        0     1505 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/initial_project/config.yml
--rw-r--r--   0        0        0      998 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/initial_project/credentials.yml
--rw-r--r--   0        0        0     1433 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/initial_project/data/nlu.yml
--rw-r--r--   0        0        0      244 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/initial_project/data/rules.yml
--rw-r--r--   0        0        0      542 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/initial_project/data/stories.yml
--rw-r--r--   0        0        0      565 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/initial_project/domain.yml
--rw-r--r--   0        0        0     1411 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/initial_project/endpoints.yml
--rw-r--r--   0        0        0     1664 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/initial_project/tests/test_stories.yml
--rw-r--r--   0        0        0     5943 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/interactive.py
--rw-r--r--   0        0        0     4196 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/run.py
--rw-r--r--   0        0        0     6846 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/scaffold.py
--rw-r--r--   0        0        0     4264 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/shell.py
--rw-r--r--   0        0        0     3118 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/telemetry.py
--rw-r--r--   0        0        0     8888 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/test.py
--rw-r--r--   0        0        0     7798 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/train.py
--rw-r--r--   0        0        0    11981 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/utils.py
--rw-r--r--   0        0        0     1256 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/visualize.py
--rw-r--r--   0        0        0     6785 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/cli/x.py
--rw-r--r--   0        0        0     1172 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/constants.py
--rw-r--r--   0        0        0      123 2023-06-14 15:11:25.891866 rasa-3.6.0/rasa/core/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/actions/__init__.py
--rw-r--r--   0        0        0    46526 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/actions/action.py
--rw-r--r--   0        0        0       78 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/actions/constants.py
--rw-r--r--   0        0        0    26542 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/actions/forms.py
--rw-r--r--   0        0        0     3322 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/actions/loops.py
--rw-r--r--   0        0        0     6078 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/actions/two_stage_fallback.py
--rw-r--r--   0        0        0    20445 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/agent.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/brokers/__init__.py
--rw-r--r--   0        0        0     4398 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/brokers/broker.py
--rw-r--r--   0        0        0     1801 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/brokers/file.py
--rw-r--r--   0        0        0    11975 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/brokers/kafka.py
--rw-r--r--   0        0        0    14118 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/brokers/pika.py
--rw-r--r--   0        0        0     2754 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/brokers/sql.py
--rw-r--r--   0        0        0     1656 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/__init__.py
--rw-r--r--   0        0        0    11685 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/botframework.py
--rw-r--r--   0        0        0     2746 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/callback.py
--rw-r--r--   0        0        0    13331 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/channel.py
--rw-r--r--   0        0        0     8073 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/console.py
--rw-r--r--   0        0        0    15755 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/facebook.py
--rw-r--r--   0        0        0    11442 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/hangouts.py
--rw-r--r--   0        0        0     7743 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/mattermost.py
--rw-r--r--   0        0        0     4814 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/rasa_chat.py
--rw-r--r--   0        0        0     6814 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/rest.py
--rw-r--r--   0        0        0     5999 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/rocketchat.py
--rw-r--r--   0        0        0    24405 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/slack.py
--rw-r--r--   0        0        0    10163 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/socketio.py
--rw-r--r--   0        0        0    10630 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/telegram.py
--rw-r--r--   0        0        0     5938 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/twilio.py
--rw-r--r--   0        0        0    13181 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/twilio_voice.py
--rw-r--r--   0        0        0     4845 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/channels/webexteams.py
--rw-r--r--   0        0        0     3047 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/constants.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/evaluation/__init__.py
--rw-r--r--   0        0        0     9154 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/evaluation/marker.py
--rw-r--r--   0        0        0    38043 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/evaluation/marker_base.py
--rw-r--r--   0        0        0    12086 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/evaluation/marker_stats.py
--rw-r--r--   0        0        0     3658 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/evaluation/marker_tracker_loader.py
--rw-r--r--   0        0        0      901 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/exceptions.py
--rw-r--r--   0        0        0    10220 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/exporter.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/featurizers/__init__.py
--rw-r--r--   0        0        0    17964 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/featurizers/precomputation.py
--rw-r--r--   0        0        0    15447 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/featurizers/single_state_featurizer.py
--rw-r--r--   0        0        0    43363 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/featurizers/tracker_featurizers.py
--rw-r--r--   0        0        0     2905 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/http_interpreter.py
--rw-r--r--   0        0        0     2018 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/jobs.py
--rw-r--r--   0        0        0     4719 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/lock.py
--rw-r--r--   0        0        0    11678 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/lock_store.py
--rw-r--r--   0        0        0    14821 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/migrate.py
--rw-r--r--   0        0        0      240 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/nlg/__init__.py
--rw-r--r--   0        0        0     3870 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/nlg/callback.py
--rw-r--r--   0        0        0     3285 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/nlg/generator.py
--rw-r--r--   0        0        0     2608 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/nlg/interpolator.py
--rw-r--r--   0        0        0     7503 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/nlg/response.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/policies/__init__.py
--rw-r--r--   0        0        0    12959 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/policies/ensemble.py
--rw-r--r--   0        0        0    19148 2023-06-14 15:11:25.895866 rasa-3.6.0/rasa/core/policies/memoization.py
--rw-r--r--   0        0        0    25038 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/policies/policy.py
--rw-r--r--   0        0        0    50266 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/policies/rule_policy.py
--rw-r--r--   0        0        0    86521 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/policies/ted_policy.py
--rw-r--r--   0        0        0    39329 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/policies/unexpected_intent_policy.py
--rw-r--r--   0        0        0    40691 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/processor.py
--rw-r--r--   0        0        0     9150 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/run.py
--rw-r--r--   0        0        0    48935 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/test.py
--rw-r--r--   0        0        0    58040 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/tracker_store.py
--rw-r--r--   0        0        0     3543 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/train.py
--rw-r--r--   0        0        0     3218 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/training/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/training/converters/__init__.py
--rw-r--r--   0        0        0     3889 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/training/converters/responses_prefix_converter.py
--rw-r--r--   0        0        0    59595 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/training/interactive.py
--rw-r--r--   0        0        0    13604 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/training/story_conflict.py
--rw-r--r--   0        0        0     3067 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/training/training.py
--rw-r--r--   0        0        0    10995 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/utils.py
--rw-r--r--   0        0        0     2125 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/core/visualize.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/__init__.py
--rw-r--r--   0        0        0    16744 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/caching.py
--rw-r--r--   0        0        0      469 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/constants.py
--rw-r--r--   0        0        0      437 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/exceptions.py
--rw-r--r--   0        0        0    22105 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/graph.py
--rw-r--r--   0        0        0     1384 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/loader.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/recipes/__init__.py
--rw-r--r--   0        0        0     1139 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/recipes/config_files/default_config.yml
--rw-r--r--   0        0        0     3244 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/recipes/default_components.py
--rw-r--r--   0        0        0    43587 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/recipes/default_recipe.py
--rw-r--r--   0        0        0     3301 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/recipes/graph_recipe.py
--rw-r--r--   0        0        0     3354 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/recipes/recipe.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/runner/__init__.py
--rw-r--r--   0        0        0     4302 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/runner/dask.py
--rw-r--r--   0        0        0     1672 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/runner/interface.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/storage/__init__.py
--rw-r--r--   0        0        0     9581 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/storage/local_model_storage.py
--rw-r--r--   0        0        0     3931 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/storage/resource.py
--rw-r--r--   0        0        0     6923 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/storage/storage.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/training/__init__.py
--rw-r--r--   0        0        0     6524 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/training/components.py
--rw-r--r--   0        0        0     1848 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/training/fingerprinting.py
--rw-r--r--   0        0        0    10516 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/training/graph_trainer.py
--rw-r--r--   0        0        0     5036 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/training/hooks.py
--rw-r--r--   0        0        0    22697 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/engine/validation.py
--rw-r--r--   0        0        0     2132 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/graph_components/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.899866 rasa-3.6.0/rasa/graph_components/converters/__init__.py
--rw-r--r--   0        0        0     1576 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/graph_components/converters/nlu_message_converter.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/graph_components/providers/__init__.py
--rw-r--r--   0        0        0     3832 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/graph_components/providers/domain_for_core_training_provider.py
--rw-r--r--   0        0        0     2571 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/graph_components/providers/domain_provider.py
--rw-r--r--   0        0        0     1294 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/graph_components/providers/forms_provider.py
--rw-r--r--   0        0        0     2119 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/graph_components/providers/nlu_training_data_provider.py
--rw-r--r--   0        0        0     1354 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/graph_components/providers/responses_provider.py
--rw-r--r--   0        0        0     1540 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/graph_components/providers/rule_only_provider.py
--rw-r--r--   0        0        0     1466 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/graph_components/providers/story_graph_provider.py
--rw-r--r--   0        0        0     1965 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/graph_components/providers/training_tracker_provider.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/graph_components/validators/__init__.py
--rw-r--r--   0        0        0    22668 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/graph_components/validators/default_recipe_validator.py
--rw-r--r--   0        0        0    12863 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/graph_components/validators/finetuning_validator.py
--rw-r--r--   0        0        0     1782 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/jupyter.py
--rw-r--r--   0        0        0      101 2023-06-14 15:11:44.707560 rasa-3.6.0/rasa/keys
--rw-r--r--   0        0        0     3490 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/model.py
--rw-r--r--   0        0        0    14961 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/model_testing.py
--rw-r--r--   0        0        0    16836 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/model_training.py
--rw-r--r--   0        0        0      123 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/__init__.py
--rw-r--r--   0        0        0      118 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/classifiers/__init__.py
--rw-r--r--   0        0        0      133 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/classifiers/classifier.py
--rw-r--r--   0        0        0    71637 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/classifiers/diet_classifier.py
--rw-r--r--   0        0        0     7150 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/classifiers/fallback_classifier.py
--rw-r--r--   0        0        0     7581 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/classifiers/keyword_intent_classifier.py
--rw-r--r--   0        0        0     7568 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/classifiers/logistic_regression_classifier.py
--rw-r--r--   0        0        0     5559 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/classifiers/mitie_intent_classifier.py
--rw-r--r--   0        0        0     1989 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/classifiers/regex_message_handler.py
--rw-r--r--   0        0        0    11915 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/classifiers/sklearn_intent_classifier.py
--rw-r--r--   0        0        0     2757 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/constants.py
--rw-r--r--   0        0        0     1317 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/convert.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/emulators/__init__.py
--rw-r--r--   0        0        0     1748 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/emulators/dialogflow.py
--rw-r--r--   0        0        0     1367 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/emulators/emulator.py
--rw-r--r--   0        0        0     3032 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/emulators/luis.py
--rw-r--r--   0        0        0      334 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/emulators/no_emulator.py
--rw-r--r--   0        0        0     1930 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/emulators/wit.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/extractors/__init__.py
--rw-r--r--   0        0        0    26499 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/extractors/crf_entity_extractor.py
--rw-r--r--   0        0        0     7685 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/extractors/duckling_entity_extractor.py
--rw-r--r--   0        0        0     7160 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/extractors/entity_synonyms.py
--rw-r--r--   0        0        0    17530 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/extractors/extractor.py
--rw-r--r--   0        0        0    10973 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/extractors/mitie_entity_extractor.py
--rw-r--r--   0        0        0     8289 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/extractors/regex_entity_extractor.py
--rw-r--r--   0        0        0     3366 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/extractors/spacy_entity_extractor.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/featurizers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/featurizers/dense_featurizer/__init__.py
--rw-r--r--   0        0        0    17142 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py
--rw-r--r--   0        0        0     2433 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py
--rw-r--r--   0        0        0    30361 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py
--rw-r--r--   0        0        0     5861 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py
--rw-r--r--   0        0        0     4888 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py
--rw-r--r--   0        0        0     3347 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/featurizers/featurizer.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/featurizers/sparse_featurizer/__init__.py
--rw-r--r--   0        0        0    33295 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py
--rw-r--r--   0        0        0    21810 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py
--rw-r--r--   0        0        0    10289 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py
--rw-r--r--   0        0        0      220 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/featurizers/sparse_featurizer/sparse_featurizer.py
--rw-r--r--   0        0        0      557 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/model.py
--rw-r--r--   0        0        0     8333 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/persistor.py
--rw-r--r--   0        0        0      803 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/run.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.903866 rasa-3.6.0/rasa/nlu/selectors/__init__.py
--rw-r--r--   0        0        0    39012 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/selectors/response_selector.py
--rw-r--r--   0        0        0    67582 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/test.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/tokenizers/__init__.py
--rw-r--r--   0        0        0     5374 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/tokenizers/jieba_tokenizer.py
--rw-r--r--   0        0        0     2618 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/tokenizers/mitie_tokenizer.py
--rw-r--r--   0        0        0     2378 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/tokenizers/spacy_tokenizer.py
--rw-r--r--   0        0        0     8196 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     3750 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/tokenizers/whitespace_tokenizer.py
--rw-r--r--   0        0        0      928 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/utils/__init__.py
--rw-r--r--   0        0        0    14703 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/utils/bilou_utils.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/utils/hugging_face/__init__.py
--rw-r--r--   0        0        0     3380 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/utils/hugging_face/registry.py
--rw-r--r--   0        0        0     9143 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py
--rw-r--r--   0        0        0     3887 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/utils/mitie_utils.py
--rw-r--r--   0        0        0     5386 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/utils/pattern_utils.py
--rw-r--r--   0        0        0    11795 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/nlu/utils/spacy_utils.py
--rw-r--r--   0        0        0     4509 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/plugin.py
--rw-r--r--   0        0        0    55589 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/server.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/__init__.py
--rw-r--r--   0        0        0     4294 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/constants.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/__init__.py
--rw-r--r--   0        0        0     4346 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/constants.py
--rw-r--r--   0        0        0     1366 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/conversation.py
--rw-r--r--   0        0        0    77445 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/domain.py
--rw-r--r--   0        0        0    65797 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/events.py
--rw-r--r--   0        0        0    35597 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/generator.py
--rw-r--r--   0        0        0     8286 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/slot_mappings.py
--rw-r--r--   0        0        0    16371 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/slots.py
--rw-r--r--   0        0        0    33790 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/trackers.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/training_data/__init__.py
--rw-r--r--   0        0        0     2895 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/training_data/loading.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/training_data/story_reader/__init__.py
--rw-r--r--   0        0        0     4449 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/training_data/story_reader/story_reader.py
--rw-r--r--   0        0        0     6671 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/training_data/story_reader/story_step_builder.py
--rw-r--r--   0        0        0    32919 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/training_data/story_reader/yaml_story_reader.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/training_data/story_writer/__init__.py
--rw-r--r--   0        0        0     2543 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/training_data/story_writer/story_writer.py
--rw-r--r--   0        0        0    14903 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/training_data/story_writer/yaml_story_writer.py
--rw-r--r--   0        0        0    29313 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/training_data/structures.py
--rw-r--r--   0        0        0     3500 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/training_data/visualization.html
--rw-r--r--   0        0        0    20341 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/core/training_data/visualization.py
--rw-r--r--   0        0        0     5479 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/data.py
--rw-r--r--   0        0        0     3633 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.907866 rasa-3.6.0/rasa/shared/importers/__init__.py
--rw-r--r--   0        0        0    21866 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/importers/importer.py
--rw-r--r--   0        0        0     7836 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/importers/multi_project.py
--rw-r--r--   0        0        0     3388 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/importers/rasa.py
--rw-r--r--   0        0        0      861 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/importers/utils.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/__init__.py
--rw-r--r--   0        0        0     1388 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/constants.py
--rw-r--r--   0        0        0      188 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/interpreter.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/__init__.py
--rw-r--r--   0        0        0     6759 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/entities_parser.py
--rw-r--r--   0        0        0    14835 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/features.py
--rw-r--r--   0        0        0      453 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/formats/__init__.py
--rw-r--r--   0        0        0     6123 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/formats/dialogflow.py
--rw-r--r--   0        0        0     3014 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/formats/luis.py
--rw-r--r--   0        0        0     4495 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/formats/rasa.py
--rw-r--r--   0        0        0    22353 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/formats/rasa_yaml.py
--rw-r--r--   0        0        0     8540 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/formats/readerwriter.py
--rw-r--r--   0        0        0     1820 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/formats/wit.py
--rw-r--r--   0        0        0     4258 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/loading.py
--rw-r--r--   0        0        0     1116 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/lookup_tables_parser.py
--rw-r--r--   0        0        0    16662 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/message.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/schemas/__init__.py
--rw-r--r--   0        0        0     2565 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/schemas/data_schema.py
--rw-r--r--   0        0        0     1179 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/schemas/nlu.yml
--rw-r--r--   0        0        0     1661 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/schemas/responses.yml
--rw-r--r--   0        0        0     1476 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/synonyms_parser.py
--rw-r--r--   0        0        0    28493 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/training_data.py
--rw-r--r--   0        0        0     7040 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/nlu/training_data/util.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/utils/__init__.py
--rw-r--r--   0        0        0     2078 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/utils/cli.py
--rw-r--r--   0        0        0     8731 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/utils/common.py
--rw-r--r--   0        0        0    20533 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/utils/io.py
--rw-r--r--   0        0        0      883 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/utils/pykwalify_extensions.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/utils/schemas/__init__.py
--rw-r--r--   0        0        0       27 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/utils/schemas/config.yml
--rw-r--r--   0        0        0     3267 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/utils/schemas/domain.yml
--rw-r--r--   0        0        0     5569 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/utils/schemas/events.py
--rw-r--r--   0        0        0      998 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/utils/schemas/model_config.yml
--rw-r--r--   0        0        0     4034 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/utils/schemas/stories.yml
--rw-r--r--   0        0        0    10317 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/shared/utils/validation.py
--rw-r--r--   0        0        0    36084 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/telemetry.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/__init__.py
--rw-r--r--   0        0        0    19532 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/common.py
--rw-r--r--   0        0        0     1647 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/converter.py
--rw-r--r--   0        0        0     8796 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/endpoints.py
--rw-r--r--   0        0        0     7831 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/io.py
--rw-r--r--   0        0        0     4327 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/log_utils.py
--rw-r--r--   0        0        0    12246 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/plotting.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/tensorflow/__init__.py
--rw-r--r--   0        0        0     4036 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/tensorflow/callback.py
--rw-r--r--   0        0        0     3140 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/tensorflow/constants.py
--rw-r--r--   0        0        0     9020 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/tensorflow/crf.py
--rw-r--r--   0        0        0    15526 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/tensorflow/data_generator.py
--rw-r--r--   0        0        0     5576 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/tensorflow/environment.py
--rw-r--r--   0        0        0      168 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/tensorflow/exceptions.py
--rw-r--r--   0        0        0    59313 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/tensorflow/layers.py
--rw-r--r--   0        0        0     3319 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/tensorflow/layers_utils.py
--rw-r--r--   0        0        0    34572 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/tensorflow/model_data.py
--rw-r--r--   0        0        0    18667 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/tensorflow/model_data_utils.py
--rw-r--r--   0        0        0    36004 2023-06-14 15:11:25.911866 rasa-3.6.0/rasa/utils/tensorflow/models.py
--rw-r--r--   0        0        0    49066 2023-06-14 15:11:25.915866 rasa-3.6.0/rasa/utils/tensorflow/rasa_layers.py
--rw-r--r--   0        0        0    25509 2023-06-14 15:11:25.915866 rasa-3.6.0/rasa/utils/tensorflow/transformer.py
--rw-r--r--   0        0        0      204 2023-06-14 15:11:25.915866 rasa-3.6.0/rasa/utils/tensorflow/types.py
--rw-r--r--   0        0        0    20984 2023-06-14 15:11:25.915866 rasa-3.6.0/rasa/utils/train_utils.py
--rw-r--r--   0        0        0    17708 2023-06-14 15:11:25.915866 rasa-3.6.0/rasa/validator.py
--rw-r--r--   0        0        0      116 2023-06-14 15:11:25.915866 rasa-3.6.0/rasa/version.py
--rw-r--r--   0        0        0    28238 1970-01-01 00:00:00.000000 rasa-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11352 2023-05-19 14:34:46.563489 rasa-3.6.0a1/LICENSE.txt
+-rw-r--r--   0        0        0    21489 2023-05-19 14:34:46.563489 rasa-3.6.0a1/README.md
+-rw-r--r--   0        0        0     9471 2023-05-19 14:34:46.751494 rasa-3.6.0a1/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/__init__.py
+-rw-r--r--   0        0        0     5188 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/__main__.py
+-rw-r--r--   0        0        0     5314 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/api.py
+-rw-r--r--   0        0        0      115 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/__init__.py
+-rw-r--r--   0        0        0     2388 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/data.py
+-rw-r--r--   0        0        0     5242 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/default_arguments.py
+-rw-r--r--   0        0        0     2199 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/evaluate.py
+-rw-r--r--   0        0        0     1499 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/export.py
+-rw-r--r--   0        0        0     2685 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/interactive.py
+-rw-r--r--   0        0        0     5674 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/run.py
+-rw-r--r--   0        0        0      367 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/shell.py
+-rw-r--r--   0        0        0     6853 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/test.py
+-rw-r--r--   0        0        0     8279 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/train.py
+-rw-r--r--   0        0        0      861 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/visualize.py
+-rw-r--r--   0        0        0     1027 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/x.py
+-rw-r--r--   0        0        0     9506 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/data.py
+-rw-r--r--   0        0        0     7948 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/evaluate.py
+-rw-r--r--   0        0        0     8204 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/export.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/actions/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/actions/actions.py
+-rw-r--r--   0        0        0     1505 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/config.yml
+-rw-r--r--   0        0        0      998 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/credentials.yml
+-rw-r--r--   0        0        0     1433 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/data/nlu.yml
+-rw-r--r--   0        0        0      244 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/data/rules.yml
+-rw-r--r--   0        0        0      542 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/data/stories.yml
+-rw-r--r--   0        0        0      565 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/domain.yml
+-rw-r--r--   0        0        0     1411 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/endpoints.yml
+-rw-r--r--   0        0        0     1664 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/tests/test_stories.yml
+-rw-r--r--   0        0        0     5943 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/interactive.py
+-rw-r--r--   0        0        0     4196 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/run.py
+-rw-r--r--   0        0        0     6846 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/scaffold.py
+-rw-r--r--   0        0        0     4264 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/shell.py
+-rw-r--r--   0        0        0     3118 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/telemetry.py
+-rw-r--r--   0        0        0     8888 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/test.py
+-rw-r--r--   0        0        0     7798 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/train.py
+-rw-r--r--   0        0        0    11981 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/utils.py
+-rw-r--r--   0        0        0     1256 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/visualize.py
+-rw-r--r--   0        0        0     6785 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/x.py
+-rw-r--r--   0        0        0     1172 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/constants.py
+-rw-r--r--   0        0        0      123 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/actions/__init__.py
+-rw-r--r--   0        0        0    45908 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/actions/action.py
+-rw-r--r--   0        0        0       78 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/actions/constants.py
+-rw-r--r--   0        0        0    25982 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/actions/forms.py
+-rw-r--r--   0        0        0     3322 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/actions/loops.py
+-rw-r--r--   0        0        0     6078 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/actions/two_stage_fallback.py
+-rw-r--r--   0        0        0    20968 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/agent.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/brokers/__init__.py
+-rw-r--r--   0        0        0     4398 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/brokers/broker.py
+-rw-r--r--   0        0        0     1801 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/brokers/file.py
+-rw-r--r--   0        0        0    11870 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/brokers/kafka.py
+-rw-r--r--   0        0        0    14045 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/brokers/pika.py
+-rw-r--r--   0        0        0     2754 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/brokers/sql.py
+-rw-r--r--   0        0        0     1656 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/__init__.py
+-rw-r--r--   0        0        0    11685 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/botframework.py
+-rw-r--r--   0        0        0     2746 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/callback.py
+-rw-r--r--   0        0        0    13331 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/channel.py
+-rw-r--r--   0        0        0     8073 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/console.py
+-rw-r--r--   0        0        0    15789 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/facebook.py
+-rw-r--r--   0        0        0    11532 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/hangouts.py
+-rw-r--r--   0        0        0     7743 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/mattermost.py
+-rw-r--r--   0        0        0     4814 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/rasa_chat.py
+-rw-r--r--   0        0        0     6937 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/rest.py
+-rw-r--r--   0        0        0     5999 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/rocketchat.py
+-rw-r--r--   0        0        0    24405 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/slack.py
+-rw-r--r--   0        0        0    10163 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/socketio.py
+-rw-r--r--   0        0        0    10630 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/telegram.py
+-rw-r--r--   0        0        0     5938 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/twilio.py
+-rw-r--r--   0        0        0    13181 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/twilio_voice.py
+-rw-r--r--   0        0        0     4845 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/webexteams.py
+-rw-r--r--   0        0        0     3047 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/constants.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/evaluation/__init__.py
+-rw-r--r--   0        0        0     9154 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/evaluation/marker.py
+-rw-r--r--   0        0        0    36811 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/evaluation/marker_base.py
+-rw-r--r--   0        0        0    12086 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/evaluation/marker_stats.py
+-rw-r--r--   0        0        0     3658 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/evaluation/marker_tracker_loader.py
+-rw-r--r--   0        0        0      901 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/exceptions.py
+-rw-r--r--   0        0        0    10220 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/exporter.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/featurizers/__init__.py
+-rw-r--r--   0        0        0    17964 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/featurizers/precomputation.py
+-rw-r--r--   0        0        0    15447 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/featurizers/single_state_featurizer.py
+-rw-r--r--   0        0        0    43363 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/featurizers/tracker_featurizers.py
+-rw-r--r--   0        0        0     2906 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/http_interpreter.py
+-rw-r--r--   0        0        0     2018 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/jobs.py
+-rw-r--r--   0        0        0     4719 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/lock.py
+-rw-r--r--   0        0        0    11678 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/lock_store.py
+-rw-r--r--   0        0        0    14821 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/migrate.py
+-rw-r--r--   0        0        0      240 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/nlg/__init__.py
+-rw-r--r--   0        0        0     3745 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/nlg/callback.py
+-rw-r--r--   0        0        0     3285 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/nlg/generator.py
+-rw-r--r--   0        0        0     2794 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/nlg/interpolator.py
+-rw-r--r--   0        0        0     7503 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/nlg/response.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/__init__.py
+-rw-r--r--   0        0        0    12959 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/ensemble.py
+-rw-r--r--   0        0        0    19062 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/memoization.py
+-rw-r--r--   0        0        0    25038 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/policy.py
+-rw-r--r--   0        0        0    50189 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/rule_policy.py
+-rw-r--r--   0        0        0    86521 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/ted_policy.py
+-rw-r--r--   0        0        0    39329 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/unexpected_intent_policy.py
+-rw-r--r--   0        0        0    40540 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/processor.py
+-rw-r--r--   0        0        0     9150 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/run.py
+-rw-r--r--   0        0        0    48935 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/test.py
+-rw-r--r--   0        0        0    58040 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/tracker_store.py
+-rw-r--r--   0        0        0     3543 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/train.py
+-rw-r--r--   0        0        0     3218 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/training/converters/__init__.py
+-rw-r--r--   0        0        0     3889 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/training/converters/responses_prefix_converter.py
+-rw-r--r--   0        0        0    59595 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/training/interactive.py
+-rw-r--r--   0        0        0    13604 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/training/story_conflict.py
+-rw-r--r--   0        0        0     3067 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/core/training/training.py
+-rw-r--r--   0        0        0    11447 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/core/utils.py
+-rw-r--r--   0        0        0     2125 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/core/visualize.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/__init__.py
+-rw-r--r--   0        0        0    16744 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/caching.py
+-rw-r--r--   0        0        0      469 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/constants.py
+-rw-r--r--   0        0        0      437 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/exceptions.py
+-rw-r--r--   0        0        0    22105 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/graph.py
+-rw-r--r--   0        0        0     1384 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/loader.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/recipes/__init__.py
+-rw-r--r--   0        0        0     1139 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/recipes/config_files/default_config.yml
+-rw-r--r--   0        0        0     3244 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/recipes/default_components.py
+-rw-r--r--   0        0        0    43587 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/recipes/default_recipe.py
+-rw-r--r--   0        0        0     3301 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/recipes/graph_recipe.py
+-rw-r--r--   0        0        0     3354 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/recipes/recipe.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/runner/__init__.py
+-rw-r--r--   0        0        0     4302 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/runner/dask.py
+-rw-r--r--   0        0        0     1672 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/runner/interface.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/storage/__init__.py
+-rw-r--r--   0        0        0     9581 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/storage/local_model_storage.py
+-rw-r--r--   0        0        0     3931 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/storage/resource.py
+-rw-r--r--   0        0        0     6923 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/storage/storage.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/training/__init__.py
+-rw-r--r--   0        0        0     6524 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/training/components.py
+-rw-r--r--   0        0        0     1848 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/training/fingerprinting.py
+-rw-r--r--   0        0        0    10516 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/training/graph_trainer.py
+-rw-r--r--   0        0        0     5036 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/training/hooks.py
+-rw-r--r--   0        0        0    22697 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/validation.py
+-rw-r--r--   0        0        0     2132 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/converters/__init__.py
+-rw-r--r--   0        0        0     1576 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/converters/nlu_message_converter.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/__init__.py
+-rw-r--r--   0        0        0     3832 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/domain_for_core_training_provider.py
+-rw-r--r--   0        0        0     2571 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/domain_provider.py
+-rw-r--r--   0        0        0     1294 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/forms_provider.py
+-rw-r--r--   0        0        0     2119 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/nlu_training_data_provider.py
+-rw-r--r--   0        0        0     1354 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/responses_provider.py
+-rw-r--r--   0        0        0     1540 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/rule_only_provider.py
+-rw-r--r--   0        0        0     1466 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/story_graph_provider.py
+-rw-r--r--   0        0        0     1965 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/training_tracker_provider.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/validators/__init__.py
+-rw-r--r--   0        0        0    22668 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/validators/default_recipe_validator.py
+-rw-r--r--   0        0        0    12863 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/validators/finetuning_validator.py
+-rw-r--r--   0        0        0     1782 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/jupyter.py
+-rw-r--r--   0        0        0      101 2023-05-19 14:35:05.111915 rasa-3.6.0a1/rasa/keys
+-rw-r--r--   0        0        0     3490 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/model.py
+-rw-r--r--   0        0        0    14961 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/model_testing.py
+-rw-r--r--   0        0        0    16836 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/model_training.py
+-rw-r--r--   0        0        0      123 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/__init__.py
+-rw-r--r--   0        0        0      133 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/classifier.py
+-rw-r--r--   0        0        0    71637 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/diet_classifier.py
+-rw-r--r--   0        0        0     7150 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/fallback_classifier.py
+-rw-r--r--   0        0        0     7581 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/keyword_intent_classifier.py
+-rw-r--r--   0        0        0     7568 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/logistic_regression_classifier.py
+-rw-r--r--   0        0        0     5559 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/mitie_intent_classifier.py
+-rw-r--r--   0        0        0     1989 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/regex_message_handler.py
+-rw-r--r--   0        0        0    11915 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/sklearn_intent_classifier.py
+-rw-r--r--   0        0        0     2757 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/constants.py
+-rw-r--r--   0        0        0     1317 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/convert.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/emulators/__init__.py
+-rw-r--r--   0        0        0     1748 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/emulators/dialogflow.py
+-rw-r--r--   0        0        0     1367 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/emulators/emulator.py
+-rw-r--r--   0        0        0     3032 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/emulators/luis.py
+-rw-r--r--   0        0        0      334 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/emulators/no_emulator.py
+-rw-r--r--   0        0        0     1930 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/emulators/wit.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/extractors/__init__.py
+-rw-r--r--   0        0        0    26499 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/crf_entity_extractor.py
+-rw-r--r--   0        0        0     7685 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/duckling_entity_extractor.py
+-rw-r--r--   0        0        0     7160 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/entity_synonyms.py
+-rw-r--r--   0        0        0    17530 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/extractor.py
+-rw-r--r--   0        0        0    10973 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/mitie_entity_extractor.py
+-rw-r--r--   0        0        0     8289 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/regex_entity_extractor.py
+-rw-r--r--   0        0        0     3366 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/spacy_entity_extractor.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/__init__.py
+-rw-r--r--   0        0        0    17142 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py
+-rw-r--r--   0        0        0     2433 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py
+-rw-r--r--   0        0        0    30361 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py
+-rw-r--r--   0        0        0     5861 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py
+-rw-r--r--   0        0        0     4888 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py
+-rw-r--r--   0        0        0     3347 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/featurizer.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/__init__.py
+-rw-r--r--   0        0        0    33295 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py
+-rw-r--r--   0        0        0    21810 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py
+-rw-r--r--   0        0        0    10289 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py
+-rw-r--r--   0        0        0      220 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/sparse_featurizer.py
+-rw-r--r--   0        0        0      557 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/model.py
+-rw-r--r--   0        0        0     8333 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/persistor.py
+-rw-r--r--   0        0        0      803 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/run.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/selectors/__init__.py
+-rw-r--r--   0        0        0    39012 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/selectors/response_selector.py
+-rw-r--r--   0        0        0    67521 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/test.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/tokenizers/__init__.py
+-rw-r--r--   0        0        0     5374 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/tokenizers/jieba_tokenizer.py
+-rw-r--r--   0        0        0     2618 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/tokenizers/mitie_tokenizer.py
+-rw-r--r--   0        0        0     2378 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/tokenizers/spacy_tokenizer.py
+-rw-r--r--   0        0        0     8196 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     3750 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/tokenizers/whitespace_tokenizer.py
+-rw-r--r--   0        0        0      928 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/__init__.py
+-rw-r--r--   0        0        0    14703 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/bilou_utils.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/hugging_face/__init__.py
+-rw-r--r--   0        0        0     3380 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/hugging_face/registry.py
+-rw-r--r--   0        0        0     9143 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py
+-rw-r--r--   0        0        0     3887 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/mitie_utils.py
+-rw-r--r--   0        0        0     5386 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/pattern_utils.py
+-rw-r--r--   0        0        0    11795 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/spacy_utils.py
+-rw-r--r--   0        0        0     4628 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/plugin.py
+-rw-r--r--   0        0        0    55589 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/server.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/shared/__init__.py
+-rw-r--r--   0        0        0     4294 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/shared/constants.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/shared/core/__init__.py
+-rw-r--r--   0        0        0     4346 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/shared/core/constants.py
+-rw-r--r--   0        0        0     1366 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/shared/core/conversation.py
+-rw-r--r--   0        0        0    75018 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/domain.py
+-rw-r--r--   0        0        0    65833 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/events.py
+-rw-r--r--   0        0        0    35597 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/generator.py
+-rw-r--r--   0        0        0     8286 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/slot_mappings.py
+-rw-r--r--   0        0        0    16371 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/slots.py
+-rw-r--r--   0        0        0    33790 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/trackers.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/__init__.py
+-rw-r--r--   0        0        0     2895 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/loading.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/__init__.py
+-rw-r--r--   0        0        0     4449 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/story_reader.py
+-rw-r--r--   0        0        0     6671 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/story_step_builder.py
+-rw-r--r--   0        0        0    32873 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/yaml_story_reader.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_writer/__init__.py
+-rw-r--r--   0        0        0     2543 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_writer/story_writer.py
+-rw-r--r--   0        0        0    14903 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_writer/yaml_story_writer.py
+-rw-r--r--   0        0        0    29313 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/structures.py
+-rw-r--r--   0        0        0     3500 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/visualization.html
+-rw-r--r--   0        0        0    20341 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/visualization.py
+-rw-r--r--   0        0        0     5479 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/data.py
+-rw-r--r--   0        0        0     3633 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/importers/__init__.py
+-rw-r--r--   0        0        0    21866 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/importers/importer.py
+-rw-r--r--   0        0        0     7836 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/importers/multi_project.py
+-rw-r--r--   0        0        0     3388 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/importers/rasa.py
+-rw-r--r--   0        0        0      861 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/importers/utils.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/__init__.py
+-rw-r--r--   0        0        0     1388 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/constants.py
+-rw-r--r--   0        0        0      188 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/interpreter.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/__init__.py
+-rw-r--r--   0        0        0     6759 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/entities_parser.py
+-rw-r--r--   0        0        0    14835 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/features.py
+-rw-r--r--   0        0        0      453 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/__init__.py
+-rw-r--r--   0        0        0     6123 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/dialogflow.py
+-rw-r--r--   0        0        0     3014 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/luis.py
+-rw-r--r--   0        0        0     4495 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/rasa.py
+-rw-r--r--   0        0        0    22353 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/rasa_yaml.py
+-rw-r--r--   0        0        0     8540 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/readerwriter.py
+-rw-r--r--   0        0        0     1820 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/wit.py
+-rw-r--r--   0        0        0     4258 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/loading.py
+-rw-r--r--   0        0        0     1116 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/lookup_tables_parser.py
+-rw-r--r--   0        0        0    16662 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/message.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/__init__.py
+-rw-r--r--   0        0        0     2565 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/data_schema.py
+-rw-r--r--   0        0        0     1179 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/nlu.yml
+-rw-r--r--   0        0        0     1595 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/responses.yml
+-rw-r--r--   0        0        0     1476 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/synonyms_parser.py
+-rw-r--r--   0        0        0    28493 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/training_data.py
+-rw-r--r--   0        0        0     7040 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/util.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/__init__.py
+-rw-r--r--   0        0        0     2078 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/cli.py
+-rw-r--r--   0        0        0     8731 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/common.py
+-rw-r--r--   0        0        0    20533 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/io.py
+-rw-r--r--   0        0        0      883 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/pykwalify_extensions.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/schemas/__init__.py
+-rw-r--r--   0        0        0       27 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/schemas/config.yml
+-rw-r--r--   0        0        0     3267 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/schemas/domain.yml
+-rw-r--r--   0        0        0     5569 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/schemas/events.py
+-rw-r--r--   0        0        0      998 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/schemas/model_config.yml
+-rw-r--r--   0        0        0     4034 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/schemas/stories.yml
+-rw-r--r--   0        0        0    10317 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/validation.py
+-rw-r--r--   0        0        0    36084 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/telemetry.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/__init__.py
+-rw-r--r--   0        0        0    19852 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/common.py
+-rw-r--r--   0        0        0     1647 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/converter.py
+-rw-r--r--   0        0        0     8796 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/endpoints.py
+-rw-r--r--   0        0        0     7831 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/io.py
+-rw-r--r--   0        0        0    12246 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/plotting.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/__init__.py
+-rw-r--r--   0        0        0     4036 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/callback.py
+-rw-r--r--   0        0        0     3140 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/constants.py
+-rw-r--r--   0        0        0     9020 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/crf.py
+-rw-r--r--   0        0        0    15526 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/data_generator.py
+-rw-r--r--   0        0        0     5576 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/environment.py
+-rw-r--r--   0        0        0      168 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/exceptions.py
+-rw-r--r--   0        0        0    59313 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/layers.py
+-rw-r--r--   0        0        0     3319 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/layers_utils.py
+-rw-r--r--   0        0        0    34572 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/model_data.py
+-rw-r--r--   0        0        0    18667 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/model_data_utils.py
+-rw-r--r--   0        0        0    36004 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/models.py
+-rw-r--r--   0        0        0    49066 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/rasa_layers.py
+-rw-r--r--   0        0        0    25509 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/transformer.py
+-rw-r--r--   0        0        0      204 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/types.py
+-rw-r--r--   0        0        0    20984 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/train_utils.py
+-rw-r--r--   0        0        0    17708 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/validator.py
+-rw-r--r--   0        0        0      118 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/version.py
+-rw-r--r--   0        0        0    28015 1970-01-01 00:00:00.000000 rasa-3.6.0a1/PKG-INFO
```

### Comparing `rasa-3.6.0/LICENSE.txt` & `rasa-3.6.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/README.md` & `rasa-3.6.0a1/README.md`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/pyproject.toml` & `rasa-3.6.0a1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.black]
 line-length = 88
 target-version = [ "py37", "py38", "py39", "py310",]
 exclude = "((.eggs | .git | .pytest_cache | build | dist))"
 
 [tool.poetry]
 name = "rasa"
-version = "3.6.0"
+version = "3.6.0a1"
 description = "Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants"
 authors = [ "Rasa Technologies GmbH <hi@rasa.com>",]
 maintainers = [ "Tom Bocklisch <tom@rasa.com>",]
 homepage = "https://rasa.com"
 repository = "https://github.com/rasahq/rasa"
 documentation = "https://rasa.com/docs"
 classifiers = [ "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "License :: OSI Approved :: Apache Software License", "Topic :: Software Development :: Libraries",]
@@ -84,38 +84,38 @@
 [tool.ruff]
 ignore = [ "D100", "D104", "D105", "RUF001", "RUF002", "RUF003", "RUF005",]
 line-length = 88
 select = [ "D", "E", "F", "W", "RUF",]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-boto3 = "^1.26.136"
+boto3 = "^1.26.124"
 requests = "^2.23"
 matplotlib = ">=3.1,<3.6"
 attrs = ">=19.3,<22.2"
 jsonpickle = ">=1.3,<3.1"
 redis = ">=4.5.3, <5.0"
-absl-py = ">=0.9,<1.5"
+absl-py = ">=0.9,<1.4"
 apscheduler = ">=3.6,<3.10"
 tqdm = "^4.31"
 networkx = ">=2.4,<2.7"
 fbmessenger = "~6.0.0"
 pykwalify = ">=1.7,<1.9"
 coloredlogs = ">=10,<16"
 "ruamel.yaml" = ">=0.16.5,<0.18.0"
 pyyaml = ">=5.3.1,<6.0"
-twilio = ">=6.26,<8.3"
+twilio = ">=6.26,<8.2"
 webexteamssdk = ">=1.1.1,<1.7.0"
 mattermostwrapper = "~2.2"
-rocketchat_API = ">=0.6.31,<1.31.0"
+rocketchat_API = ">=0.6.31,<1.30.0"
 colorhash = ">=1.0.2,<1.3.0"
 jsonschema = ">=3.2,<4.18"
 packaging = ">=20.0,<21.0"
 pytz = ">=2019.1,<2023.0"
-rasa-sdk = "~3.6.0"
+rasa-sdk = "~3.6.0a1"
 colorclass = "~2.2"
 terminaltables = "~3.1.0"
 sanic = "~21.12"
 sanic-cors = "~2.0.0"
 sanic-jwt = "^1.6.0"
 sanic-routing = "^0.7.2"
 websockets = ">=10.0,<11.0"
@@ -145,16 +145,14 @@
 google-auth = "<3"
 CacheControl = "^0.12.9"
 randomname = "^0.1.5"
 pluggy = "^1.0.0"
 slack-sdk = "^3.19.2"
 confluent-kafka = ">=1.9.2,<3.0.0"
 portalocker = "^2.7.0"
-structlog = "^23.1.0"
-structlog-sentry = "^2.0.2"
 [[tool.poetry.dependencies.dask]]
 version = "2022.2.0"
 python = "~=3.7.0"
 
 [[tool.poetry.dependencies.dask]]
 version = "2022.10.2"
 python = ">=3.8,<3.11"
@@ -163,21 +161,14 @@
 version = ">=1.19.2,<1.22.0"
 python = "~=3.7.0"
 
 [[tool.poetry.dependencies.numpy]]
 version = ">=1.19.2,<1.25.0"
 python = ">=3.8,<3.11"
 
-# Pinning numpy version for windows because of the issue mentioned below:
-#https://github.com/scipy/scipy/blob/c58b608c83d30800aceee6a4dab5c3464cb1de7d/pyproject.toml#L38-L41
-[[tool.poetry.dependencies.numpy]]
-version = "1.22.3"
-markers = "sys_platform =='Windows' and platform_python_implementation != 'PyPy'"
-python = "3.10"
-
 [[tool.poetry.dependencies.scipy]]
 version = ">=1.4.1,<1.7.3"
 python = "~=3.7.0"
 
 [[tool.poetry.dependencies.scipy]]
 version = ">=1.4.1,<1.9.0"
 python = ">=3.8,<3.11"
@@ -208,14 +199,50 @@
 version = ">=0.18,<0.20"
 markers = "sys_platform != 'linux' or (platform_machine != 'arm64' and platform_machine != 'aarch64')"
 
 [[tool.poetry.dependencies.tensorflow-addons]]
 version = "0.19.0"
 markers = "sys_platform == 'linux' and (platform_machine == 'arm64' or platform_machine == 'aarch64')"
 
+[tool.poetry.dev-dependencies]
+pytest-cov = "^4.0.0"
+pytest-asyncio = "^0.20.0"
+pytest-xdist = "^3.2.1"
+pytest = "^7.1.3"
+freezegun = "^1.0.0"
+responses = "^0.22.0"
+aioresponses = "^0.7.2"
+moto = "~=4.1.2"
+fakeredis = "^2.11.2"
+mongomock = "^4.1.2"
+black = "^22.10.0"
+google-cloud-storage = "^2.4.0"
+azure-storage-blob = "<12.16.0"
+coveralls = "^3.0.1"
+towncrier = "^22.8.0"
+toml = "^0.10.0"
+pep440-version-utils = "^0.3.0"
+pydoc-markdown = "^4.5.1"
+pytest-timeout = "^2.1.0"
+mypy = "^1.0.0"
+bandit = "^1.6.3"
+types-pytz = "^2022.1.1"
+types-python-dateutil = "^2.8.19"
+types-requests = "^2.25.0"
+types-setuptools = "^67.2.0"
+memory-profiler = "^0.61.0"
+psutil = "^5.8.0"
+mypy-extensions = "^0.4.3"
+sanic-testing = ">=21.12.0,<22.9.0"
+analytics-python = "^1.4.0"
+datadog-api-client = "^2.0.0"
+datadog = "^0.45.0"
+types-redis = "^4.3.20"
+httpx = "0.23.3"
+
 [tool.poetry.extras]
 spacy = [ "spacy",]
 jieba = [ "jieba",]
 transformers = [ "transformers", "sentencepiece",]
 full = [ "spacy", "transformers", "sentencepiece", "jieba",]
 gh-release-notes = [ "github3.py",]
 metal = [ "tensorflow-metal",]
@@ -237,31 +264,30 @@
 log_cli = true
 markers = [ "skip_on_windows", "skip_on_ci", "sequential", "category_cli", "category_core_featurizers", "category_policies", "category_nlu_featurizers", "category_nlu_predictors", "category_full_model_training", "category_other_unit_tests", "category_performance", "flaky",]
 timeout = 60
 timeout_func_only = true
 asyncio_mode = "auto"
 
 [tool.poetry.dependencies.tensorflow]
-version = "2.11.1"
+version = "2.11.0"
 markers = "sys_platform != 'darwin' or platform_machine != 'arm64'"
 
 [tool.poetry.dependencies.tensorflow-intel]
-version = "2.11.1"
+version = "2.11.0"
 markers = "sys_platform == 'win32'"
 
 [tool.poetry.dependencies.tensorflow-io-gcs-filesystem]
 version = ">=0.23.1,<0.32"
 markers = "sys_platform == 'win32'"
 
 [tool.poetry.dependencies.tensorflow-cpu-aws]
-version = "2.11.1"
+version = "2.11.0"
 markers = "sys_platform == 'linux' and (platform_machine == 'arm64' or platform_machine == 'aarch64')"
 
 [tool.poetry.dependencies.tensorflow-macos]
-# Updated tensorflow to 2.11.1 for other platforms except Apple Silicon - 2.11.1 is not available there
 version = "2.11.0"
 markers = "sys_platform == 'darwin' and platform_machine == 'arm64'"
 
 [tool.poetry.dependencies.PyJWT]
 version = "^2.0.0"
 extras = [ "crypto",]
 
@@ -300,43 +326,9 @@
 extras = [ "tls", "srv",]
 
 [tool.poetry.dev-dependencies.pytest-sanic]
 git = "https://github.com/RasaHQ/pytest-sanic"
 branch = "fix_signal_issue"
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.255,<0.0.270"
+ruff = "^0.0.255"
 docker = "^6.0.1"
-pytest-cov = "^4.0.0"
-pytest-asyncio = "^0.20.0"
-pytest-xdist = "^3.2.1"
-pytest = "^7.1.3"
-freezegun = "^1.0.0"
-responses = "^0.22.0"
-aioresponses = "^0.7.2"
-moto = "~=4.1.2"
-fakeredis = "^2.11.2"
-mongomock = "^4.1.2"
-black = "^22.10.0"
-google-cloud-storage = "^2.4.0"
-azure-storage-blob = "<12.16.0"
-coveralls = "^3.0.1"
-towncrier = "^22.8.0"
-toml = "^0.10.0"
-pep440-version-utils = "^0.3.0"
-pydoc-markdown = "^4.5.1"
-pytest-timeout = "^2.1.0"
-mypy = "^1.0.0"
-bandit = "^1.6.3"
-types-pytz = "^2022.1.1"
-types-python-dateutil = "^2.8.19"
-types-requests = "^2.25.0"
-types-setuptools = "^67.2.0"
-memory-profiler = "^0.61.0"
-psutil = "^5.8.0"
-mypy-extensions = "^0.4.3"
-sanic-testing = ">=21.12.0,<22.9.0"
-analytics-python = "^1.4.0"
-datadog-api-client = "^2.0.0"
-datadog = "^0.45.0"
-types-redis = "^4.3.20"
-httpx = "0.23.3"
```

### Comparing `rasa-3.6.0/rasa/__main__.py` & `rasa-3.6.0a1/rasa/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 import os
 import platform
 import sys
 
 from rasa_sdk import __version__ as rasa_sdk_version
 from rasa.constants import MINIMUM_COMPATIBLE_VERSION
-from rasa.utils.log_utils import configure_structlog
 
 import rasa.telemetry
 import rasa.utils.io
 import rasa.utils.tensorflow.environment as tf_env
 from rasa import version
 from rasa.cli import (
     data,
@@ -120,19 +119,14 @@
             )
             endpoints_file = result[0] if result else None
 
             rasa.telemetry.initialize_telemetry()
             rasa.telemetry.initialize_error_reporting()
             plugin_manager().hook.init_telemetry(endpoints_file=endpoints_file)
             plugin_manager().hook.init_managers(endpoints_file=endpoints_file)
-            plugin_manager().hook.init_anonymization_pipeline(
-                endpoints_file=endpoints_file
-            )
-            # configure structlog
-            configure_structlog(log_level)
 
             cmdline_arguments.func(cmdline_arguments)
         elif hasattr(cmdline_arguments, "version"):
             print_version()
         else:
             # user has not provided a subcommand, let's print the help
             logger.error("No command specified.")
```

### Comparing `rasa-3.6.0/rasa/api.py` & `rasa-3.6.0a1/rasa/api.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/arguments/data.py` & `rasa-3.6.0a1/rasa/cli/arguments/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/arguments/default_arguments.py` & `rasa-3.6.0a1/rasa/cli/arguments/default_arguments.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/arguments/evaluate.py` & `rasa-3.6.0a1/rasa/cli/arguments/evaluate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/arguments/export.py` & `rasa-3.6.0a1/rasa/cli/arguments/export.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/arguments/interactive.py` & `rasa-3.6.0a1/rasa/cli/arguments/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/arguments/run.py` & `rasa-3.6.0a1/rasa/cli/arguments/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/arguments/test.py` & `rasa-3.6.0a1/rasa/cli/arguments/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/arguments/train.py` & `rasa-3.6.0a1/rasa/cli/arguments/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/arguments/visualize.py` & `rasa-3.6.0a1/rasa/cli/arguments/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/arguments/x.py` & `rasa-3.6.0a1/rasa/cli/arguments/x.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/data.py` & `rasa-3.6.0a1/rasa/cli/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/evaluate.py` & `rasa-3.6.0a1/rasa/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/export.py` & `rasa-3.6.0a1/rasa/cli/export.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/initial_project/actions/actions.py` & `rasa-3.6.0a1/rasa/cli/initial_project/actions/actions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/initial_project/config.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/initial_project/credentials.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/credentials.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/initial_project/data/nlu.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/data/nlu.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/initial_project/data/stories.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/data/stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/initial_project/domain.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/domain.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/initial_project/endpoints.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/endpoints.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/initial_project/tests/test_stories.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/tests/test_stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/interactive.py` & `rasa-3.6.0a1/rasa/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/run.py` & `rasa-3.6.0a1/rasa/cli/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/scaffold.py` & `rasa-3.6.0a1/rasa/cli/scaffold.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/shell.py` & `rasa-3.6.0a1/rasa/cli/shell.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/telemetry.py` & `rasa-3.6.0a1/rasa/cli/telemetry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/test.py` & `rasa-3.6.0a1/rasa/cli/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/train.py` & `rasa-3.6.0a1/rasa/cli/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/utils.py` & `rasa-3.6.0a1/rasa/cli/utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/visualize.py` & `rasa-3.6.0a1/rasa/cli/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/cli/x.py` & `rasa-3.6.0a1/rasa/cli/x.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/constants.py` & `rasa-3.6.0a1/rasa/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/actions/action.py` & `rasa-3.6.0a1/rasa/core/actions/action.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import rasa.core
 from rasa.core.actions.constants import DEFAULT_SELECTIVE_DOMAIN, SELECTIVE_DOMAIN
 from rasa.core.constants import (
     DEFAULT_REQUEST_TIMEOUT,
     COMPRESS_ACTION_SERVER_REQUEST_ENV_NAME,
     DEFAULT_COMPRESS_ACTION_SERVER_REQUEST,
 )
-from rasa.core.nlg.callback import RESPONSE_ID_KEY
 from rasa.core.policies.policy import PolicyPrediction
 from rasa.nlu.constants import (
     RESPONSE_SELECTOR_DEFAULT_INTENT,
     RESPONSE_SELECTOR_PROPERTY_NAME,
     RESPONSE_SELECTOR_PREDICTION_KEY,
     RESPONSE_SELECTOR_UTTER_ACTION_KEY,
 )
@@ -302,31 +301,15 @@
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
         domain: "Domain",
     ) -> List[Event]:
         """Simple run implementation uttering a (hopefully defined) response."""
-        response_ids_for_response = domain.response_ids_per_response.get(
-            self.utter_action, set()
-        )
-
-        response_id_list = list(response_ids_for_response)
-        response_id_list.sort()
-
-        kwargs = {
-            RESPONSE_ID_KEY: response_id_list,
-        }
-
-        message = await nlg.generate(
-            self.utter_action,
-            tracker,
-            output_channel.name(),
-            **kwargs,
-        )
+        message = await nlg.generate(self.utter_action, tracker, output_channel.name())
         if message is None:
             if not self.silent_fail:
                 logger.error(
                     "Couldn't create message for response '{}'."
                     "".format(self.utter_action)
                 )
             return []
@@ -522,15 +505,14 @@
     """The first action in any turn - bot waits for a user message.
 
     The bot should stop taking further actions and wait for the user to say
     something.
     """
 
     def name(self) -> Text:
-        """Returns action listen name."""
         return ACTION_LISTEN_NAME
 
     async def run(
         self,
         output_channel: "OutputChannel",
         nlg: "NaturalLanguageGenerator",
         tracker: "DialogueStateTracker",
@@ -851,15 +833,14 @@
 
 class ActionExecutionRejection(RasaException):
     """Raising this exception will allow other policies
     to predict a different action.
     """
 
     def __init__(self, action_name: Text, message: Optional[Text] = None) -> None:
-        """Create a new ActionExecutionRejection exception."""
         self.action_name = action_name
         self.message = message or "Custom action '{}' rejected to run".format(
             action_name
         )
         super(ActionExecutionRejection, self).__init__()
 
     def __str__(self) -> Text:
@@ -1083,17 +1064,14 @@
             if active_loop and active_loop == tracker.active_loop_name:
                 condition_requested_slot = condition.get(REQUESTED_SLOT)
                 if not condition_requested_slot:
                     return True
                 if condition_requested_slot == tracker.get_slot(REQUESTED_SLOT):
                     return True
 
-            if active_loop is None and tracker.active_loop_name is None:
-                return True
-
         return False
 
     @staticmethod
     def _verify_mapping_conditions(
         mapping: Dict[Text, Any], tracker: "DialogueStateTracker", slot_name: Text
     ) -> bool:
         if mapping.get(MAPPING_CONDITIONS) and mapping[MAPPING_TYPE] != str(
```

### Comparing `rasa-3.6.0/rasa/core/actions/forms.py` & `rasa-3.6.0a1/rasa/core/actions/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Text, List, Optional, Union, Any, Dict, Set
 import itertools
 import logging
-import structlog
 import json
 
 from rasa.core.actions import action
 from rasa.core.actions.loops import LoopAction
 from rasa.core.channels import OutputChannel
 from rasa.shared.core.domain import Domain, KEY_SLOTS
 from rasa.shared.core.constants import SlotMappingType, SLOT_MAPPINGS, MAPPING_TYPE
@@ -28,15 +27,14 @@
 from rasa.core.nlg import NaturalLanguageGenerator
 from rasa.shared.core.slot_mappings import SlotMapping
 from rasa.shared.core.slots import ListSlot
 from rasa.shared.core.trackers import DialogueStateTracker
 from rasa.utils.endpoints import EndpointConfig
 
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 
 class FormAction(LoopAction):
     """Action which implements and executes the form logic."""
 
     def __init__(
         self, form_name: Text, action_endpoint: Optional[EndpointConfig]
@@ -252,15 +250,15 @@
         Returns:
             The validation events including potential bot messages and `SlotSet` events
             for the validated slots, if the custom form validation action is present in
             domain actions.
             Otherwise, returns empty list since the extracted slots already have
             corresponding `SlotSet` events in the tracker.
         """
-        structlogger.debug("forms.slots.validate", slot_candidates=slot_candidates)
+        logger.debug(f"Validating extracted slots: {slot_candidates}")
         events: List[Union[SlotSet, Event]] = [
             SlotSet(slot_name, value) for slot_name, value in slot_candidates.items()
         ]
 
         validate_name = f"validate_{self.name()}"
 
         if validate_name not in domain.action_names_or_texts:
@@ -536,18 +534,15 @@
         # no active_loop means that it is called during activation
         needs_validation = not tracker.active_loop or (
             tracker.latest_action_name == ACTION_LISTEN_NAME
             and not tracker.is_active_loop_interrupted
         )
 
         if needs_validation:
-            structlogger.debug(
-                "forms.validation.required",
-                tracker_latest_message=tracker.latest_message,
-            )
+            logger.debug(f"Validating user input '{tracker.latest_message}'.")
             return await self.validate(tracker, domain, output_channel, nlg)
         else:
             # Needed to determine which slots to request although there are no slots
             # to actually validate, which happens when coming back to the form after
             # an unhappy path
             return await self.validate_slots({}, tracker, domain, output_channel, nlg)
 
@@ -606,29 +601,17 @@
 
         for slot_name in self.required_slots(domain):
             if not self._should_request_slot(tracker, slot_name):
                 prefilled_slots[slot_name] = tracker.get_slot(slot_name)
 
         if not prefilled_slots:
             logger.debug("No pre-filled required slots to validate.")
-        else:
-            structlogger.debug("forms.activate.form", prefilled_slots=prefilled_slots)
-
-        validate_name = f"validate_{self.name()}"
-
-        if validate_name not in domain.action_names_or_texts:
-            logger.debug(
-                f"There is no validation action '{validate_name}' "
-                f"to execute at form activation."
-            )
-            return [event for event in extraction_events if isinstance(event, SlotSet)]
+            return [e for e in extraction_events if isinstance(e, SlotSet)]
 
-        logger.debug(
-            f"Executing validation action '{validate_name}' at form activation."
-        )
+        logger.debug(f"Validating pre-filled required slots: {prefilled_slots}")
 
         validated_events = await self.validate_slots(
             prefilled_slots, tracker, domain, output_channel, nlg
         )
 
         validated_slot_names = [
             event.key for event in validated_events if isinstance(event, SlotSet)
```

### Comparing `rasa-3.6.0/rasa/core/actions/loops.py` & `rasa-3.6.0a1/rasa/core/actions/loops.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/actions/two_stage_fallback.py` & `rasa-3.6.0a1/rasa/core/actions/two_stage_fallback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/agent.py` & `rasa-3.6.0a1/rasa/core/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import aiohttp
 from aiohttp import ClientError
 
 from rasa.core import jobs
 from rasa.core.channels.channel import OutputChannel, UserMessage
 from rasa.core.constants import DEFAULT_REQUEST_TIMEOUT
 from rasa.core.http_interpreter import RasaNLUHttpInterpreter
+from rasa.plugin import plugin_manager
 from rasa.shared.core.domain import Domain
 from rasa.core.exceptions import AgentNotReady
 from rasa.shared.constants import DEFAULT_SENDER_ID
 from rasa.core.lock_store import InMemoryLockStore, LockStore
 from rasa.core.nlg import NaturalLanguageGenerator, TemplatedNaturalLanguageGenerator
 from rasa.core.policies.policy import PolicyPrediction
 from rasa.core.processor import MessageProcessor
@@ -215,35 +216,42 @@
     from rasa.core.brokers.broker import EventBroker
 
     tracker_store = None
     lock_store = None
     generator = None
     action_endpoint = None
     http_interpreter = None
+    anonymization_pipeline = None
 
     if endpoints:
         broker = await EventBroker.create(endpoints.event_broker, loop=loop)
         tracker_store = TrackerStore.create(
             endpoints.tracker_store, event_broker=broker
         )
         lock_store = LockStore.create(endpoints.lock_store)
         generator = endpoints.nlg
         action_endpoint = endpoints.action
         model_server = endpoints.model if endpoints.model else model_server
         if endpoints.nlu:
             http_interpreter = RasaNLUHttpInterpreter(endpoints.nlu)
 
+        anonymization_pipeline = plugin_manager().hook.create_anonymization_pipeline(
+            anonymization_rules=endpoints.anonymization_rules,
+            event_broker_config=endpoints.event_broker,
+        )
+
     agent = Agent(
         generator=generator,
         tracker_store=tracker_store,
         lock_store=lock_store,
         action_endpoint=action_endpoint,
         model_server=model_server,
         remote_storage=remote_storage,
         http_interpreter=http_interpreter,
+        anonymization_pipeline=anonymization_pipeline,
     )
 
     try:
         if model_server is not None:
             return await load_from_server(agent, model_server)
 
         elif remote_storage is not None:
@@ -297,28 +305,30 @@
         tracker_store: Optional[TrackerStore] = None,
         lock_store: Optional[LockStore] = None,
         action_endpoint: Optional[EndpointConfig] = None,
         fingerprint: Optional[Text] = None,
         model_server: Optional[EndpointConfig] = None,
         remote_storage: Optional[Text] = None,
         http_interpreter: Optional[RasaNLUHttpInterpreter] = None,
+        anonymization_pipeline: Optional[Any] = None,
     ):
         """Initializes an `Agent`."""
         self.domain = domain
         self.processor: Optional[MessageProcessor] = None
 
         self.nlg = NaturalLanguageGenerator.create(generator, self.domain)
         self.tracker_store = self._create_tracker_store(tracker_store, self.domain)
         self.lock_store = self._create_lock_store(lock_store)
         self.action_endpoint = action_endpoint
         self.http_interpreter = http_interpreter
 
         self._set_fingerprint(fingerprint)
         self.model_server = model_server
         self.remote_storage = remote_storage
+        self.anonymization_pipeline = anonymization_pipeline
 
     @classmethod
     def load(
         cls,
         model_path: Union[Text, Path],
         domain: Optional[Domain] = None,
         generator: Union[EndpointConfig, NaturalLanguageGenerator, None] = None,
@@ -352,14 +362,15 @@
         self.processor = MessageProcessor(
             model_path=model_path,
             tracker_store=self.tracker_store,
             lock_store=self.lock_store,
             action_endpoint=self.action_endpoint,
             generator=self.nlg,
             http_interpreter=self.http_interpreter,
+            anonymization_pipeline=self.anonymization_pipeline,
         )
         self.domain = self.processor.domain
 
         self._set_fingerprint(fingerprint)
 
         # update domain on all instances
         self.tracker_store.domain = self.domain
```

### Comparing `rasa-3.6.0/rasa/core/brokers/broker.py` & `rasa-3.6.0a1/rasa/core/brokers/broker.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/brokers/file.py` & `rasa-3.6.0a1/rasa/core/brokers/file.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/brokers/kafka.py` & `rasa-3.6.0a1/rasa/core/brokers/kafka.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio
 import os
 import json
 import logging
-import structlog
 import threading
 from asyncio import AbstractEventLoop
 from typing import Any, Text, List, Optional, Union, Dict, TYPE_CHECKING
 import time
 
 from rasa.core.brokers.broker import EventBroker
 from rasa.core.exceptions import KafkaProducerInitializationError
@@ -14,15 +13,14 @@
 from rasa.utils.endpoints import EndpointConfig
 import rasa.shared.utils.common
 
 if TYPE_CHECKING:
     from confluent_kafka import KafkaError, Producer, Message
 
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 
 class KafkaEventBroker(EventBroker):
     """Kafka event broker."""
 
     def __init__(
         self,
@@ -235,20 +233,17 @@
             headers = [
                 (
                     "RASA_ENVIRONMENT",
                     bytes(self.rasa_environment, encoding=DEFAULT_ENCODING),
                 )
             ]
 
-        structlogger.debug(
-            "kafka.publish.event",
-            topic=self.topic,
-            rasa_event=event,
-            partition_key=partition_key,
-            headers=headers,
+        logger.debug(
+            f"Calling kafka send({self.topic}, value={event},"
+            f" key={partition_key!s}, headers={headers})"
         )
 
         serialized_event = json.dumps(event).encode(DEFAULT_ENCODING)
 
         if self.producer is not None:
             self.producer.produce(
                 self.topic,
```

### Comparing `rasa-3.6.0/rasa/core/brokers/pika.py` & `rasa-3.6.0a1/rasa/core/brokers/pika.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 import json
 import logging
-import structlog
 import os
 import ssl
 from asyncio import AbstractEventLoop
 from collections import deque
 from typing import Deque, Dict, Optional, Text, Union, Any, List, Set, Tuple, cast
 from urllib.parse import urlparse
 
@@ -16,15 +15,14 @@
 from rasa.core.brokers.broker import EventBroker
 import rasa.shared.utils.io
 from rasa.utils.endpoints import EndpointConfig
 from rasa.shared.utils.io import DEFAULT_ENCODING
 import rasa.shared.utils.common
 
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 RABBITMQ_EXCHANGE = "rasa-exchange"
 DEFAULT_QUEUE_NAME = "rasa_core_events"
 
 
 class PikaEventBroker(EventBroker):
     """Pika-based event broker for publishing messages to RabbitMQ."""
@@ -296,25 +294,22 @@
     ) -> None:
         if self._exchange is None:
             return
 
         try:
             await self._exchange.publish(self._message(event, headers), "")
 
-            structlogger.debug(
-                "pika.events.publish",
-                rabbitmq_exchange=RABBITMQ_EXCHANGE,
-                host=self.host,
-                rasa_event=event,
+            logger.debug(
+                f"Published Pika events to exchange '{RABBITMQ_EXCHANGE}' on host "
+                f"'{self.host}':\n{event}"
             )
         except Exception as e:
-            structlogger.error(
-                "pika.events.publish.failed",
-                host=self.host,
-                rasa_event=event,
+            logger.error(
+                f"Failed to publish Pika event on host '{self.host}' due to "
+                f"error '{e}'. The message was: \n{event}"
             )
             if self.should_keep_unpublished_messages:
                 self._unpublished_events.append(event)
 
             if self.raise_on_failure:
                 self.close()  # type: ignore[unused-coroutine]
                 raise e
```

### Comparing `rasa-3.6.0/rasa/core/brokers/sql.py` & `rasa-3.6.0a1/rasa/core/brokers/sql.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/__init__.py` & `rasa-3.6.0a1/rasa/core/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/botframework.py` & `rasa-3.6.0a1/rasa/core/channels/botframework.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/callback.py` & `rasa-3.6.0a1/rasa/core/channels/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/channel.py` & `rasa-3.6.0a1/rasa/core/channels/channel.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/console.py` & `rasa-3.6.0a1/rasa/core/channels/console.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/facebook.py` & `rasa-3.6.0a1/rasa/core/channels/facebook.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import hashlib
 import hmac
 import logging
-import structlog
 from fbmessenger import MessengerClient
 from fbmessenger.attachments import Image
 from fbmessenger.elements import Text as FBText
 from fbmessenger.quick_replies import QuickReplies, QuickReply
 from fbmessenger.sender_actions import SenderAction
 
 import rasa.shared.utils.io
@@ -13,15 +12,14 @@
 from sanic.request import Request
 from typing import Text, List, Dict, Any, Callable, Awaitable, Iterable, Optional, Union
 
 from rasa.core.channels.channel import UserMessage, OutputChannel, InputChannel
 from sanic.response import HTTPResponse
 
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 
 class Messenger:
     """Implement a fbmessenger to parse incoming webhooks and send msgs."""
 
     @classmethod
     def name(cls) -> Text:
@@ -74,15 +72,15 @@
             "message" in message
             and "attachments" in message["message"]
             and message["message"]["attachments"][0]["type"] == "file"
         )
 
     @staticmethod
     def _is_user_message(message: Dict[Text, Any]) -> bool:
-        """Check if the message is a message from the user."""
+        """Check if the message is a message from the user"""
         return (
             "message" in message
             and "text" in message["message"]
             and not message["message"].get("is_echo")
         )
 
     @staticmethod
@@ -103,14 +101,15 @@
                 elif message.get("postback"):
                     return await self.postback(message, metadata)
 
     async def message(
         self, message: Dict[Text, Any], metadata: Optional[Dict[Text, Any]]
     ) -> None:
         """Handle an incoming event from the fb webhook."""
+
         # quick reply and user message both share 'text' attribute
         # so quick reply should be checked first
         if self._is_quick_reply_message(message):
             text = message["message"]["quick_reply"]["payload"]
         elif self._is_user_message(message):
             text = message["message"]["text"]
         elif self._is_audio_message(message):
@@ -122,30 +121,35 @@
         elif self._is_video_message(message):
             attachment = message["message"]["attachments"][0]
             text = attachment["payload"]["url"]
         elif self._is_file_message(message):
             attachment = message["message"]["attachments"][0]
             text = attachment["payload"]["url"]
         else:
-            structlogger.warning("facebook.message.handle", message=message)
+            logger.warning(
+                "Received a message from facebook that we can not "
+                f"handle. Message: {message}"
+            )
             return
 
         await self._handle_user_message(text, self.get_user_id(), metadata)
 
     async def postback(
         self, message: Dict[Text, Any], metadata: Optional[Dict[Text, Any]]
     ) -> None:
         """Handle a postback (e.g. quick reply button)."""
+
         text = message["postback"]["payload"]
         await self._handle_user_message(text, self.get_user_id(), metadata)
 
     async def _handle_user_message(
         self, text: Text, sender_id: Text, metadata: Optional[Dict[Text, Any]]
     ) -> None:
         """Pass on the text to the dialogue engine for processing."""
+
         out_channel = MessengerBot(self.client)
         await out_channel.send_action(sender_id, sender_action="mark_seen")
 
         user_msg = UserMessage(
             text, out_channel, sender_id, input_channel=self.name(), metadata=metadata
         )
         await out_channel.send_action(sender_id, sender_action="typing_on")
@@ -171,51 +175,56 @@
     def __init__(self, messenger_client: MessengerClient) -> None:
 
         self.messenger_client = messenger_client
         super().__init__()
 
     def send(self, recipient_id: Text, element: Any) -> None:
         """Sends a message to the recipient using the messenger client."""
+
         # this is a bit hacky, but the client doesn't have a proper API to
         # send messages but instead expects the incoming sender to be present
         # which we don't have as it is stored in the input channel.
         self.messenger_client.send(element.to_dict(), recipient_id, "RESPONSE")
 
     async def send_text_message(
         self, recipient_id: Text, text: Text, **kwargs: Any
     ) -> None:
         """Send a message through this channel."""
+
         for message_part in text.strip().split("\n\n"):
             self.send(recipient_id, FBText(text=message_part))
 
     async def send_image_url(
         self, recipient_id: Text, image: Text, **kwargs: Any
     ) -> None:
         """Sends an image. Default will just post the url as a string."""
+
         self.send(recipient_id, Image(url=image))
 
     async def send_action(self, recipient_id: Text, sender_action: Text) -> None:
         """Sends a sender action to facebook (e.g. "typing_on").
 
         Args:
             recipient_id: recipient
             sender_action: action to send, e.g. "typing_on" or "mark_seen"
         """
+
         self.messenger_client.send_action(
             SenderAction(sender_action).to_dict(), recipient_id
         )
 
     async def send_text_with_buttons(
         self,
         recipient_id: Text,
         text: Text,
         buttons: List[Dict[Text, Any]],
         **kwargs: Any,
     ) -> None:
         """Sends buttons to the output."""
+
         # buttons is a list of tuples: [(option_name,payload)]
         if len(buttons) > 3:
             rasa.shared.utils.io.raise_warning(
                 "Facebook API currently allows only up to 3 buttons. "
                 "If you add more, all will be ignored."
             )
             await self.send_text_message(recipient_id, text, **kwargs)
@@ -241,21 +250,23 @@
         self,
         recipient_id: Text,
         text: Text,
         quick_replies: List[Dict[Text, Any]],
         **kwargs: Any,
     ) -> None:
         """Sends quick replies to the output."""
+
         quick_replies = self._convert_to_quick_reply(quick_replies)
         self.send(recipient_id, FBText(text=text, quick_replies=quick_replies))
 
     async def send_elements(
         self, recipient_id: Text, elements: Iterable[Dict[Text, Any]], **kwargs: Any
     ) -> None:
         """Sends elements to the output."""
+
         for element in elements:
             if "buttons" in element:
                 self._add_postback_info(element["buttons"])
 
         payload = {
             "attachment": {
                 "type": "template",
@@ -286,15 +297,16 @@
         """Make sure every button has a type. Modifications happen in place."""
         for button in buttons:
             if "type" not in button:
                 button["type"] = "postback"
 
     @staticmethod
     def _convert_to_quick_reply(quick_replies: List[Dict[Text, Any]]) -> QuickReplies:
-        """Convert quick reply dictionary to FB QuickReplies object."""
+        """Convert quick reply dictionary to FB QuickReplies object"""
+
         fb_quick_replies = []
         for quick_reply in quick_replies:
             try:
                 fb_quick_replies.append(
                     QuickReply(
                         title=quick_reply["title"],
                         payload=quick_reply["payload"],
@@ -395,14 +407,15 @@
             app_secret: Secret Key for application
             request_payload: request body
             hub_signature_header: X-Hub-Signature header sent with request
 
         Returns:
             bool: indicated that hub signature is validated
         """
+
         # noinspection PyBroadException
         try:
             hash_method, hub_signature = hub_signature_header.split("=")
         except Exception:
             pass
         else:
             digest_module = getattr(hashlib, hash_method)
```

### Comparing `rasa-3.6.0/rasa/core/channels/hangouts.py` & `rasa-3.6.0a1/rasa/core/channels/hangouts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import structlog
 import google.auth.transport.requests
 import cachecontrol
 import requests
 
 from asyncio import CancelledError
 from sanic import Blueprint, response
 from sanic.request import Request
@@ -12,15 +11,14 @@
 from google.oauth2 import id_token
 from sanic.response import HTTPResponse
 from sanic.exceptions import SanicException
 
 from rasa.core.channels.channel import InputChannel, OutputChannel, UserMessage
 
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 CHANNEL_NAME = "hangouts"
 CERTS_URL = (
     "https://www.googleapis.com/service_accounts/"
     "v1/metadata/x509/chat@system.gserviceaccount.com"
 )
 
@@ -317,14 +315,19 @@
                         collector,
                         sender_id,
                         input_channel=input_channel,
                         metadata={"room": room_name},
                     )
                 )
             except CancelledError:
-                structlogger.error("hangouts.message.blueprint", text=text)
-            except Exception:
-                structlogger.exception("hangouts.message.blueprint.failure", text=text)
+                logger.error(
+                    "Message handling timed out for " "user message '{}'.".format(text)
+                )
+            except Exception as e:
+                logger.exception(
+                    f"An exception occurred while handling user message: {e}, "
+                    f"text: {text}"
+                )
 
             return response.json(collector.messages)
 
         return custom_webhook
```

### Comparing `rasa-3.6.0/rasa/core/channels/mattermost.py` & `rasa-3.6.0a1/rasa/core/channels/mattermost.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/rasa_chat.py` & `rasa-3.6.0a1/rasa/core/channels/rasa_chat.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/rest.py` & `rasa-3.6.0a1/rasa/core/channels/rest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio
 import inspect
 import json
 import logging
-import structlog
 from asyncio import Queue, CancelledError
 from sanic import Blueprint, response
 from sanic.request import Request
 from sanic.response import HTTPResponse, ResponseStream
 from typing import Text, Dict, Any, Optional, Callable, Awaitable, NoReturn, Union
 
 import rasa.utils.endpoints
@@ -14,24 +13,22 @@
     InputChannel,
     CollectingOutputChannel,
     UserMessage,
 )
 
 
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 
 class RestInput(InputChannel):
     """A custom http input channel.
 
     This implementation is the basis for a custom implementation of a chat
     frontend. You can customize this to send messages to Rasa and
-    retrieve responses from the assistant.
-    """
+    retrieve responses from the assistant."""
 
     @classmethod
     def name(cls) -> Text:
         return "rest"
 
     @staticmethod
     async def on_message_wrapper(
@@ -164,27 +161,32 @@
                             collector,
                             sender_id,
                             input_channel=input_channel,
                             metadata=metadata,
                         )
                     )
                 except CancelledError:
-                    structlogger.error("rest.message.received", text=text)
+                    logger.error(
+                        f"Message handling timed out for user message '{text}'.",
+                        exc_info=True,
+                    )
                 except Exception:
-                    structlogger.exception("rest.message.received.failure", text=text)
+                    logger.exception(
+                        f"An exception occured while handling "
+                        f"user message '{text}'."
+                    )
                 return response.json(collector.messages)
 
         return custom_webhook
 
 
 class QueueOutputChannel(CollectingOutputChannel):
-    """Output channel that collects send messages in a list.
+    """Output channel that collects send messages in a list
 
-    (doesn't send them anywhere, just collects them).
-    """
+    (doesn't send them anywhere, just collects them)."""
 
     # FIXME: this is breaking Liskov substitution principle
     # and would require some user-facing refactoring to address
     messages: Queue  # type: ignore[assignment]
 
     @classmethod
     def name(cls) -> Text:
```

### Comparing `rasa-3.6.0/rasa/core/channels/rocketchat.py` & `rasa-3.6.0a1/rasa/core/channels/rocketchat.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/slack.py` & `rasa-3.6.0a1/rasa/core/channels/slack.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/socketio.py` & `rasa-3.6.0a1/rasa/core/channels/socketio.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/telegram.py` & `rasa-3.6.0a1/rasa/core/channels/telegram.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/twilio.py` & `rasa-3.6.0a1/rasa/core/channels/twilio.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/twilio_voice.py` & `rasa-3.6.0a1/rasa/core/channels/twilio_voice.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/channels/webexteams.py` & `rasa-3.6.0a1/rasa/core/channels/webexteams.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/constants.py` & `rasa-3.6.0a1/rasa/core/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/evaluation/marker.py` & `rasa-3.6.0a1/rasa/core/evaluation/marker.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/evaluation/marker_base.py` & `rasa-3.6.0a1/rasa/core/evaluation/marker_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,29 +157,22 @@
     does not apply to the conversation so far.
     """
 
     # Identifier for an artificial marker that is created when loading markers
     # from a dictionary of configs. For more details, see `from_config_dict`.
     ANY_MARKER = "<any_marker>"
 
-    def __init__(
-        self,
-        name: Optional[Text] = None,
-        negated: bool = False,
-        description: Optional[Text] = None,
-    ) -> None:
+    def __init__(self, name: Optional[Text] = None, negated: bool = False) -> None:
         """Instantiates a marker.
 
         Args:
             name: a custom name that can be used to replace the default string
                 conversion of this marker
             negated: whether this marker should be negated (i.e. a negated marker
                 applies if and only if the non-negated marker does not apply)
-            description: an optional description of the marker. It is not used
-                internally but can be used to document the marker.
         Raises:
             `InvalidMarkerConfig` if the chosen *name* of the marker is the tag of
             a predefined marker.
         """
         if name == Marker.ANY_MARKER or name in MarkerRegistry.all_tags:
             raise InvalidMarkerConfig(
                 f"You must not use the special marker name {Marker.ANY_MARKER}. "
@@ -190,15 +183,14 @@
             )
         self.name = name
         self.history: List[bool] = []
         # Note: we allow negation here even though there might not be a negated tag
         # for 2 reasons: testing and the fact that the `MarkerRegistry`+`from_config`
         # won't allow to create a negated marker if there is no negated tag.
         self.negated: bool = negated
-        self.description = description
 
     def __str__(self) -> Text:
         return self.name or repr(self)
 
     def __repr__(self) -> Text:
         return self._to_str_with(self.get_tag())
 
@@ -553,41 +545,34 @@
         Returns:
             the configured marker
         """
         # Triggers the import of all modules containing marker classes in order to
         # register all configurable markers.
         MarkerRegistry.register_builtin_markers()
 
-        if not isinstance(config, dict) or len(config) not in [1, 2]:
+        if not isinstance(config, dict) or len(config) != 1:
             raise InvalidMarkerConfig(
                 "To configure a marker, please define a dictionary that maps a "
                 "single operator tag or a single condition tag to the "
                 "corresponding parameter configuration or a list of marker "
                 "configurations, respectively. "
                 f"Refer to the docs for more information: {DOCS_URL_MARKERS} "
             )
 
-        description = config.pop("description", None)
         tag = next(iter(config))
         sub_marker_config = config[tag]
 
         tag, _ = MarkerRegistry.get_non_negated_tag(tag_or_negated_tag=tag)
         if tag in MarkerRegistry.operator_tag_to_marker_class:
             return OperatorMarker.from_tag_and_sub_config(
-                tag=tag,
-                sub_config=sub_marker_config,
-                name=name,
-                description=description,
+                tag=tag, sub_config=sub_marker_config, name=name
             )
         elif tag in MarkerRegistry.condition_tag_to_marker_class:
             return ConditionMarker.from_tag_and_sub_config(
-                tag=tag,
-                sub_config=sub_marker_config,
-                name=name,
-                description=description,
+                tag=tag, sub_config=sub_marker_config, name=name
             )
 
         raise InvalidMarkerConfig(
             f"Expected a marker configuration with a key that specifies"
             f" an operator or a condition but found {tag}. "
             f"Available conditions and operators are: "
             f"{sorted(MarkerRegistry.all_tags)}. "
@@ -696,35 +681,29 @@
                 )
 
 
 class OperatorMarker(Marker, ABC):
     """Combines several markers into one."""
 
     def __init__(
-        self,
-        markers: List[Marker],
-        negated: bool = False,
-        name: Optional[Text] = None,
-        description: Optional[Text] = None,
+        self, markers: List[Marker], negated: bool = False, name: Optional[Text] = None
     ) -> None:
         """Instantiates a marker.
 
         Args:
             markers: the list of markers to combine
             negated: whether this marker should be negated (i.e. a negated marker
                 applies if and only if the non-negated marker does not apply)
             name: a custom name that can be used to replace the default string
                 conversion of this marker
-            description: an optional description of the marker. It is not used
-                internally but can be used to document the marker.
         Raises:
             `InvalidMarkerConfig` if the given number of sub-markers does not match
             the expected number of sub-markers
         """
-        super().__init__(name=name, negated=negated, description=description)
+        super().__init__(name=name, negated=negated)
         self.sub_markers: List[Marker] = markers
         expected_num = self.expected_number_of_sub_markers()
         if expected_num is not None and len(markers) != expected_num:
             raise InvalidMarkerConfig(
                 f"Expected {expected_num} sub-marker(s) to be specified for marker "
                 f"'{self}' ({self.get_tag()}) but found {len(markers)}. "
                 f"Please adapt your configuration so that there are exactly "
@@ -787,29 +766,25 @@
 
     def max_depth(self) -> int:
         """Gets the maximum depth from this point in the marker tree."""
         return 1 + max(child.max_depth() for child in self.sub_markers)
 
     @staticmethod
     def from_tag_and_sub_config(
-        tag: Text,
-        sub_config: Any,
-        name: Optional[Text] = None,
-        description: Optional[Text] = None,
+        tag: Text, sub_config: Any, name: Optional[Text] = None
     ) -> OperatorMarker:
         """Creates an operator marker from the given config.
 
         The configuration must consist of a list of marker configurations.
         See `Marker.from_config` for more details.
 
         Args:
             tag: the tag identifying an operator
             sub_config: a list of marker configs
             name: an optional custom name to be attached to the resulting marker
-            description: an optional description of the marker
         Returns:
            the configured operator marker
         Raises:
             `InvalidMarkerConfig` if the given config or the tag are not well-defined
         """
         positive_tag, is_negation = MarkerRegistry.get_non_negated_tag(tag)
         operator_class = MarkerRegistry.operator_tag_to_marker_class.get(positive_tag)
@@ -838,42 +813,34 @@
             # we don't re-raise here because the stack trace would only be
             # printed when we run rasa evaluate with --debug flag
             raise InvalidMarkerConfig(
                 f"Could not create operator '{tag}' with sub-markers "
                 f"{collected_sub_markers}. Reason: {str(e)}"
             )
         marker.name = name
-        marker.description = description
         return marker
 
 
 class ConditionMarker(Marker, ABC):
     """A marker that does not contain any sub-markers."""
 
     def __init__(
-        self,
-        text: Text,
-        negated: bool = False,
-        name: Optional[Text] = None,
-        description: Optional[Text] = None,
+        self, text: Text, negated: bool = False, name: Optional[Text] = None
     ) -> None:
         """Instantiates an atomic marker.
 
         Args:
             text: some text used to decide whether the marker applies
             negated: whether this marker should be negated (i.e. a negated marker
                 applies if and only if the non-negated marker does not apply)
             name: a custom name that can be used to replace the default string
                 conversion of this marker
-            description: an optional description of the marker. It is not used
-                internally but can be used to document the marker.
         """
         super().__init__(name=name, negated=negated)
         self.text = text
-        self.description = description
 
     def _to_str_with(self, tag: Text) -> Text:
         return f"({tag}: {self.text})"
 
     def flatten(self) -> Iterator[ConditionMarker]:
         """Returns an iterator that just returns this `AtomicMarker`.
 
@@ -884,18 +851,15 @@
 
     def max_depth(self) -> int:
         """Gets the maximum depth from this point in the marker tree."""
         return 1
 
     @staticmethod
     def from_tag_and_sub_config(
-        tag: Text,
-        sub_config: Any,
-        name: Optional[Text] = None,
-        description: Optional[Text] = None,
+        tag: Text, sub_config: Any, name: Optional[Text] = None
     ) -> ConditionMarker:
         """Creates an atomic marker from the given config.
 
         Args:
             tag: the tag identifying a condition
             sub_config: a single text parameter expected by all condition markers;
                e.g. if the tag is for an `intent_detected` marker then the `config`
@@ -913,9 +877,8 @@
 
         if not isinstance(sub_config, str):
             raise InvalidMarkerConfig(
                 f"Expected a text parameter to be specified for marker '{tag}'."
             )
         marker = marker_class(sub_config, negated=is_negation)
         marker.name = name
-        marker.description = description
         return marker
```

### Comparing `rasa-3.6.0/rasa/core/evaluation/marker_stats.py` & `rasa-3.6.0a1/rasa/core/evaluation/marker_stats.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/evaluation/marker_tracker_loader.py` & `rasa-3.6.0a1/rasa/core/evaluation/marker_tracker_loader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/exceptions.py` & `rasa-3.6.0a1/rasa/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/exporter.py` & `rasa-3.6.0a1/rasa/core/exporter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/featurizers/precomputation.py` & `rasa-3.6.0a1/rasa/core/featurizers/precomputation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/featurizers/single_state_featurizer.py` & `rasa-3.6.0a1/rasa/core/featurizers/single_state_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/featurizers/tracker_featurizers.py` & `rasa-3.6.0a1/rasa/core/featurizers/tracker_featurizers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/http_interpreter.py` & `rasa-3.6.0a1/rasa/core/http_interpreter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import aiohttp
 
 import logging
-import structlog
 
 from typing import Text, Dict, Any, Optional
 
 from rasa.core import constants
 from rasa.core.channels import UserMessage
 from rasa.shared.nlu.constants import INTENT_NAME_KEY
 from rasa.utils.endpoints import EndpointConfig
 
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 
 class RasaNLUHttpInterpreter:
     """Allows for an HTTP endpoint to be used to parse messages."""
 
     def __init__(self, endpoint_config: Optional[EndpointConfig] = None) -> None:
         """Initializes a `RasaNLUHttpInterpreter`."""
@@ -42,17 +40,17 @@
         self, text: Text, message_id: Optional[Text] = None
     ) -> Optional[Dict[Text, Any]]:
         """Send a text message to a running rasa NLU http server.
 
         Return `None` on failure.
         """
         if not self.endpoint_config or self.endpoint_config.url is None:
-            structlogger.error(
-                "http.parse.text",
-                text=text,
+            logger.error(
+                f"Failed to parse text '{text}' using rasa NLU over http. "
+                f"No rasa NLU server specified!"
             )
             return None
 
         params = {
             "token": self.endpoint_config.token,
             "text": text,
             "message_id": message_id,
@@ -67,18 +65,17 @@
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.post(url, json=params) as resp:
                     if resp.status == 200:
                         return await resp.json()
                     else:
                         response_text = await resp.text()
-                        structlogger.error(
-                            "http.parse.text.failure",
-                            text=text,
-                            response_text=response_text,
+                        logger.error(
+                            f"Failed to parse text '{text}' using rasa NLU over "
+                            f"http. Error: {response_text}"
                         )
                         return None
         except Exception:  # skipcq: PYL-W0703
             # need to catch all possible exceptions when doing http requests
             # (timeouts, value errors, parser errors, ...)
-            structlogger.exception("http.parse.text.exception", text=text)
+            logger.exception(f"Failed to parse text '{text}' using rasa NLU over http.")
             return None
```

### Comparing `rasa-3.6.0/rasa/core/jobs.py` & `rasa-3.6.0a1/rasa/core/jobs.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/lock.py` & `rasa-3.6.0a1/rasa/core/lock.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/lock_store.py` & `rasa-3.6.0a1/rasa/core/lock_store.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/migrate.py` & `rasa-3.6.0a1/rasa/core/migrate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/nlg/callback.py` & `rasa-3.6.0a1/rasa/core/nlg/callback.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,59 +9,52 @@
 
 logger = logging.getLogger(__name__)
 
 
 def nlg_response_format_spec() -> Dict[Text, Any]:
     """Expected response schema for an NLG endpoint.
 
-    Used for validation of the response returned from the NLG endpoint.
-    """
+    Used for validation of the response returned from the NLG endpoint."""
     return {
         "type": "object",
         "properties": {
             "text": {"type": "string"},
             "buttons": {"type": ["array", "null"], "items": {"type": "object"}},
             "elements": {"type": ["array", "null"], "items": {"type": "object"}},
             "attachment": {"type": ["object", "null"]},
             "image": {"type": ["string", "null"]},
             "custom": {"type": "object"},
         },
     }
 
 
-RESPONSE_ID_KEY = "response_ids"
-
-
 def nlg_request_format(
     utter_action: Text,
     tracker: DialogueStateTracker,
     output_channel: Text,
     **kwargs: Any,
 ) -> Dict[Text, Any]:
     """Create the json body for the NLG json body for the request."""
     tracker_state = tracker.current_state(EventVerbosity.ALL)
-    response_ids = kwargs.pop(RESPONSE_ID_KEY, [])
 
     return {
         "response": utter_action,
-        "ids": response_ids,
         "arguments": kwargs,
         "tracker": tracker_state,
         "channel": {"name": output_channel},
     }
 
 
 class CallbackNaturalLanguageGenerator(NaturalLanguageGenerator):
     """Generate bot utterances by using a remote endpoint for the generation.
 
     The generator will call the endpoint for each message it wants to
     generate. The endpoint needs to respond with a properly formatted
     json. The generator will use this message to create a response for
-    the bot.
-    """
+    the bot."""
 
     def __init__(self, endpoint_config: EndpointConfig) -> None:
 
         self.nlg_endpoint = endpoint_config
 
     async def generate(
         self,
```

### Comparing `rasa-3.6.0/rasa/core/nlg/generator.py` & `rasa-3.6.0a1/rasa/core/nlg/generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/nlg/interpolator.py` & `rasa-3.6.0a1/rasa/core/nlg/interpolator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import re
 import logging
-import structlog
 from typing import Text, Dict, Union, Any, List
 
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 
 def interpolate_text(response: Text, values: Dict[Text, Text]) -> Text:
     """Interpolate values into responses with placeholders.
 
     Transform response tags from "{tag_name}" to "{0[tag_name]}" as described here:
     https://stackoverflow.com/questions/7934620/python-dots-in-the-name-of-variable-in-a-format-string#comment9695339_7934969
@@ -33,18 +31,21 @@
             # in double curly and format func simply escaped it.
             # we don't want to return {0[SLOTNAME]} thus
             # restoring original value with { being escaped.
             return response.format({})
 
         return text
     except KeyError as e:
-        structlogger.exception(
-            "interpolator.interpolate.text",
-            response=response,
-            placeholder_key=e.args[0],
+        logger.exception(
+            f"Failed to replace placeholders in response '{response}'. "
+            f"Tried to replace '{e.args[0]}' but could not find "
+            f"a value for it. There is no slot with this "
+            f"name nor did you pass the value explicitly "
+            f"when calling the response. Return response "
+            f"without filling the response. "
         )
         return response
 
 
 def interpolate(
     response: Union[List[Any], Dict[Text, Any], Text], values: Dict[Text, Text]
 ) -> Union[List[Any], Dict[Text, Any], Text]:
```

### Comparing `rasa-3.6.0/rasa/core/nlg/response.py` & `rasa-3.6.0a1/rasa/core/nlg/response.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/policies/ensemble.py` & `rasa-3.6.0a1/rasa/core/policies/ensemble.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/policies/memoization.py` & `rasa-3.6.0a1/rasa/core/policies/memoization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 import zlib
 
 import base64
 import json
 import logging
-import structlog
 
 from tqdm import tqdm
 from typing import Optional, Any, Dict, List, Text
 from pathlib import Path
 
 import rasa.utils.io
 import rasa.shared.utils.io
@@ -31,15 +30,14 @@
     DEFAULT_MAX_HISTORY,
     POLICY_MAX_HISTORY,
     POLICY_PRIORITY,
 )
 from rasa.shared.core.constants import ACTION_LISTEN_NAME
 
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 
 @DefaultV1Recipe.register(
     DefaultV1Recipe.ComponentType.POLICY_WITHOUT_END_TO_END_SUPPORT, is_trainable=True
 )
 class MemoizationPolicy(Policy):
     """A policy that follows exact examples of `max_history` turns in training stories.
@@ -249,15 +247,15 @@
 
         Returns:
              The policy's prediction (e.g. the probabilities for the actions).
         """
         result = self._default_predictions(domain)
 
         states = self._prediction_states(tracker, domain, rule_only_data=rule_only_data)
-        structlogger.debug("memoization.predict.actions", tracker_states=states)
+        logger.debug(f"Current tracker state:{self.format_tracker_states(states)}")
         predicted_action_name = self.recall(
             states, tracker, domain, rule_only_data=rule_only_data
         )
         if predicted_action_name is not None:
             logger.debug(f"There is a memorised next action '{predicted_action_name}'")
             result = self._prediction_result(predicted_action_name, tracker, domain)
         else:
@@ -424,25 +422,25 @@
                 truncated_tracker, domain, rule_only_data=rule_only_data
             )
 
             if old_states != states:
                 # check if we like new futures
                 memorised = self._recall_states(states)
                 if memorised is not None:
-                    structlogger.debug("memoization.states_recall", states=states)
+                    logger.debug(f"Current tracker state {states}")
                     return memorised
                 old_states = states
 
             # go back again
             truncated_tracker = self._strip_leading_events_until_action_executed(
                 truncated_tracker, again=True
             )
 
         # No match found
-        structlogger.debug("memoization.states_recall", old_states=old_states)
+        logger.debug(f"Current tracker state {old_states}")
         return None
 
     def recall(
         self,
         states: List[State],
         tracker: DialogueStateTracker,
         domain: Domain,
```

### Comparing `rasa-3.6.0/rasa/core/policies/policy.py` & `rasa-3.6.0a1/rasa/core/policies/policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/policies/rule_policy.py` & `rasa-3.6.0a1/rasa/core/policies/rule_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 import functools
 import logging
-import structlog
 from typing import Any, List, DefaultDict, Dict, Text, Optional, Set, Tuple, cast
 
 from tqdm import tqdm
 import numpy as np
 import json
 from collections import defaultdict
 
@@ -52,15 +51,14 @@
 )
 from rasa.shared.core.domain import InvalidDomain, State, Domain
 from rasa.shared.nlu.constants import ACTION_NAME, INTENT_NAME_KEY
 import rasa.core.test
 from rasa.core.training.training import create_action_fingerprints, ActionFingerprint
 
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 
 # These are Rasa Open Source default actions and overrule everything at any time.
 DEFAULT_ACTION_MAPPINGS = {
     USER_INTENT_RESTART: ACTION_RESTART_NAME,
     USER_INTENT_BACK: ACTION_BACK_NAME,
     USER_INTENT_SESSION_START: ACTION_SESSION_START_NAME,
@@ -1018,15 +1016,15 @@
             tracker,
             domain,
             use_text_for_last_user_input,
             rule_only_data=self._get_rule_only_data(),
         )
 
         current_states = self.format_tracker_states(states)
-        structlogger.debug("rule_policy.actions.find", current_states=current_states)
+        logger.debug(f"Current tracker state:{current_states}")
 
         # Tracks if we are returning after an unhappy loop path. If this becomes `True`
         # the policy returns an event which notifies the loop action that it
         # is returning after an unhappy path. For example, the `FormAction` uses this
         # to skip the validation of slots for its first execution after an unhappy path.
         returning_from_unhappy_path = False
```

### Comparing `rasa-3.6.0/rasa/core/policies/ted_policy.py` & `rasa-3.6.0a1/rasa/core/policies/ted_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/policies/unexpected_intent_policy.py` & `rasa-3.6.0a1/rasa/core/policies/unexpected_intent_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/processor.py` & `rasa-3.6.0a1/rasa/core/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import logging
-import structlog
 import os
 from pathlib import Path
 import tarfile
 import time
 from types import LambdaType
 from typing import Any, Dict, List, Optional, Text, Tuple, Union
 
 from rasa.core.http_interpreter import RasaNLUHttpInterpreter
 from rasa.engine import loader
 from rasa.engine.constants import PLACEHOLDER_MESSAGE, PLACEHOLDER_TRACKER
 from rasa.engine.runner.dask import DaskGraphRunner
 from rasa.engine.storage.local_model_storage import LocalModelStorage
 from rasa.engine.storage.storage import ModelMetadata
 from rasa.model import get_latest_model
-from rasa.plugin import plugin_manager
 from rasa.shared.data import TrainingType
 import rasa.shared.utils.io
 import rasa.core.actions.action
 from rasa.core import jobs
 from rasa.core.actions.action import Action
 from rasa.core.channels.channel import (
     CollectingOutputChannel,
@@ -67,15 +65,14 @@
     INTENT_NAME_KEY,
     PREDICTED_CONFIDENCE_KEY,
     TEXT,
 )
 from rasa.utils.endpoints import EndpointConfig
 
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 MAX_NUMBER_OF_PREDICTIONS = int(os.environ.get("MAX_NUMBER_OF_PREDICTIONS", "10"))
 
 
 class MessageProcessor:
     """The message processor is interface for communicating with a bot model."""
 
@@ -85,14 +82,15 @@
         tracker_store: rasa.core.tracker_store.TrackerStore,
         lock_store: LockStore,
         generator: NaturalLanguageGenerator,
         action_endpoint: Optional[EndpointConfig] = None,
         max_number_of_predictions: int = MAX_NUMBER_OF_PREDICTIONS,
         on_circuit_break: Optional[LambdaType] = None,
         http_interpreter: Optional[RasaNLUHttpInterpreter] = None,
+        anonymization_pipeline: Optional[Any] = None,
     ) -> None:
         """Initializes a `MessageProcessor`."""
         self.nlg = generator
         self.tracker_store = tracker_store
         self.lock_store = lock_store
         self.max_number_of_predictions = max_number_of_predictions
         self.on_circuit_break = on_circuit_break
@@ -110,14 +108,15 @@
                 f"streaming events without a unique assistant identifier.",
                 UserWarning,
             )
 
         self.model_path = Path(model_path)
         self.domain = self.model_metadata.domain
         self.http_interpreter = http_interpreter
+        self.anonymization_pipeline = anonymization_pipeline
 
     @staticmethod
     def _load_model(
         model_path: Union[Text, Path]
     ) -> Tuple[Text, ModelMetadata, GraphRunner]:
         """Unpacks a model from a given path using the graph model loader."""
         try:
@@ -191,42 +190,40 @@
             output_channel, self.nlg, tracker, self.domain
         )
 
         await self._send_bot_messages(extraction_events, tracker, output_channel)
 
         tracker.update_with_events(extraction_events, self.domain)
 
-        structlogger.debug(
-            "processor.extract.slots",
-            action_extract_slot=ACTION_EXTRACT_SLOTS,
-            len_extraction_events=len(extraction_events),
-            rasa_events=extraction_events,
+        events_as_str = ", ".join([repr(e) or str(e) for e in extraction_events])
+        logger.debug(
+            f"Default action '{ACTION_EXTRACT_SLOTS}' was executed, "
+            f"resulting in {len(extraction_events)} events: {events_as_str}"
         )
 
         return tracker
 
     async def run_anonymization_pipeline(self, tracker: DialogueStateTracker) -> None:
         """Run the anonymization pipeline on the new tracker events.
 
         Args:
             tracker: A tracker representing a conversation state.
         """
-        anonymization_pipeline = plugin_manager().hook.get_anonymization_pipeline()
-        if anonymization_pipeline is None:
+        if self.anonymization_pipeline is None:
             return None
 
         old_tracker = await self.tracker_store.retrieve(tracker.sender_id)
         new_events = rasa.shared.core.trackers.TrackerEventDiffEngine.event_difference(
             old_tracker, tracker
         )
 
         for event in new_events:
             body = {"sender_id": tracker.sender_id}
             body.update(event.as_dict())
-            anonymization_pipeline.run(body)
+            self.anonymization_pipeline.run(body)
 
     async def predict_next_for_sender_id(
         self, sender_id: Text
     ) -> Optional[Dict[Text, Any]]:
         """Predict the next action for the given sender_id.
 
         Args:
@@ -645,15 +642,15 @@
     @staticmethod
     def _log_slots(tracker: DialogueStateTracker) -> None:
         # Log currently set slots
         slot_values = "\n".join(
             [f"\t{s.name}: {s.value}" for s in tracker.slots.values()]
         )
         if slot_values.strip():
-            structlogger.debug("processor.slots.log", slot_values=slot_values)
+            logger.debug(f"Current slot values: \n{slot_values}")
 
     def _check_for_unseen_features(self, parse_data: Dict[Text, Any]) -> None:
         """Warns the user if the NLU parse data contains unrecognized features.
 
         Checks intents and entities picked up by the NLU parsing
         against the domain and warns the user of those that don't match.
         Also considers a list of default intents that are valid but don't
@@ -714,19 +711,19 @@
         else:
             if tracker is None:
                 tracker = DialogueStateTracker.from_events(message.sender_id, [])
             parse_data = self._parse_message_with_graph(
                 message, tracker, only_output_properties
             )
 
-        structlogger.debug(
-            "processor.message.parse",
-            parse_data_text=parse_data["text"],
-            parse_data_intent=parse_data["intent"],
-            parse_data_entities=parse_data["entities"],
+        logger.debug(
+            "Received user message '{}' with intent '{}' "
+            "and entities '{}'".format(
+                parse_data["text"], parse_data["intent"], parse_data["entities"]
+            )
         )
 
         self._check_for_unseen_features(parse_data)
 
         return parse_data
 
     def _parse_message_with_graph(
@@ -1006,26 +1003,21 @@
         if events is None:
             events = []
 
         action_was_rejected_manually = any(
             isinstance(event, ActionExecutionRejected) for event in events
         )
         if not action_was_rejected_manually:
-            structlogger.debug(
-                "processor.actions.policy_prediction",
-                prediction_events=prediction.events,
-            )
+            logger.debug(f"Policy prediction ended with events '{prediction.events}'.")
             tracker.update_with_events(prediction.events, self.domain)
 
             # log the action and its produced events
             tracker.update(action.event_for_successful_execution(prediction))
 
-        structlogger.debug(
-            "processor.actions.log", action_name=action.name(), rasa_events=events
-        )
+        logger.debug(f"Action '{action.name()}' ended with events '{events}'.")
         tracker.update_with_events(events, self.domain)
 
     def _has_session_expired(self, tracker: DialogueStateTracker) -> bool:
         """Determine whether the latest session in `tracker` has expired.
 
         Args:
             tracker: Tracker to inspect.
```

### Comparing `rasa-3.6.0/rasa/core/run.py` & `rasa-3.6.0a1/rasa/core/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/test.py` & `rasa-3.6.0a1/rasa/core/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/tracker_store.py` & `rasa-3.6.0a1/rasa/core/tracker_store.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/train.py` & `rasa-3.6.0a1/rasa/core/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/training/__init__.py` & `rasa-3.6.0a1/rasa/core/training/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/training/converters/responses_prefix_converter.py` & `rasa-3.6.0a1/rasa/core/training/converters/responses_prefix_converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/training/interactive.py` & `rasa-3.6.0a1/rasa/core/training/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/training/story_conflict.py` & `rasa-3.6.0a1/rasa/core/training/story_conflict.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/training/training.py` & `rasa-3.6.0a1/rasa/core/training/training.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/core/utils.py` & `rasa-3.6.0a1/rasa/core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 import logging
 import os
 from decimal import Decimal
 from pathlib import Path
-from typing import Any, Dict, Optional, Set, Text, Tuple, Union
+from typing import Any, Dict, List, Optional, Set, Text, Tuple, Union
 
 import numpy as np
 
 import rasa.shared.utils.io
 from rasa.constants import DEFAULT_SANIC_WORKERS, ENV_SANIC_WORKERS
+from rasa.plugin import plugin_manager
 from rasa.shared.constants import DEFAULT_ENDPOINTS_PATH, TCP_PROTOCOL
 
 from rasa.core.lock_store import LockStore, RedisLockStore, InMemoryLockStore
 from rasa.utils.endpoints import EndpointConfig, read_endpoint_config
 from sanic import Sanic
 from socket import SOCK_DGRAM, SOCK_STREAM
 import rasa.cli.utils as cli_utils
@@ -179,42 +180,53 @@
         model = read_endpoint_config(endpoint_file, endpoint_type="models")
         tracker_store = read_endpoint_config(
             endpoint_file, endpoint_type="tracker_store"
         )
         lock_store = read_endpoint_config(endpoint_file, endpoint_type="lock_store")
         event_broker = read_endpoint_config(endpoint_file, endpoint_type="event_broker")
 
+        anonymization_rules = plugin_manager().hook.read_anonymization_rules(
+            endpoints_file=endpoint_file
+        )
+
+        # explicitly set to `None` if the list is empty
+        if not anonymization_rules:
+            anonymization_rules = None
+
         return cls(
             nlg,
             nlu,
             action,
             model,
             tracker_store,
             lock_store,
             event_broker,
+            anonymization_rules,
         )
 
     def __init__(
         self,
         nlg: Optional[EndpointConfig] = None,
         nlu: Optional[EndpointConfig] = None,
         action: Optional[EndpointConfig] = None,
         model: Optional[EndpointConfig] = None,
         tracker_store: Optional[EndpointConfig] = None,
         lock_store: Optional[EndpointConfig] = None,
         event_broker: Optional[EndpointConfig] = None,
+        anonymization_rules: Optional[List[Any]] = None,
     ) -> None:
         """Create an `AvailableEndpoints` object."""
         self.model = model
         self.action = action
         self.nlu = nlu
         self.nlg = nlg
         self.tracker_store = tracker_store
         self.lock_store = lock_store
         self.event_broker = event_broker
+        self.anonymization_rules = anonymization_rules
 
 
 def read_endpoints_from_path(
     endpoints_path: Optional[Union[Path, Text]] = None
 ) -> AvailableEndpoints:
     """Get `AvailableEndpoints` object from specified path.
```

### Comparing `rasa-3.6.0/rasa/core/visualize.py` & `rasa-3.6.0a1/rasa/core/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/caching.py` & `rasa-3.6.0a1/rasa/engine/caching.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/graph.py` & `rasa-3.6.0a1/rasa/engine/graph.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/loader.py` & `rasa-3.6.0a1/rasa/engine/loader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/recipes/config_files/default_config.yml` & `rasa-3.6.0a1/rasa/engine/recipes/config_files/default_config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/recipes/default_components.py` & `rasa-3.6.0a1/rasa/engine/recipes/default_components.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/recipes/default_recipe.py` & `rasa-3.6.0a1/rasa/engine/recipes/default_recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/recipes/graph_recipe.py` & `rasa-3.6.0a1/rasa/engine/recipes/graph_recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/recipes/recipe.py` & `rasa-3.6.0a1/rasa/engine/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/runner/dask.py` & `rasa-3.6.0a1/rasa/engine/runner/dask.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/runner/interface.py` & `rasa-3.6.0a1/rasa/engine/runner/interface.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/storage/local_model_storage.py` & `rasa-3.6.0a1/rasa/engine/storage/local_model_storage.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/storage/resource.py` & `rasa-3.6.0a1/rasa/engine/storage/resource.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/storage/storage.py` & `rasa-3.6.0a1/rasa/engine/storage/storage.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/training/components.py` & `rasa-3.6.0a1/rasa/engine/training/components.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/training/fingerprinting.py` & `rasa-3.6.0a1/rasa/engine/training/fingerprinting.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/training/graph_trainer.py` & `rasa-3.6.0a1/rasa/engine/training/graph_trainer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/training/hooks.py` & `rasa-3.6.0a1/rasa/engine/training/hooks.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/engine/validation.py` & `rasa-3.6.0a1/rasa/engine/validation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/exceptions.py` & `rasa-3.6.0a1/rasa/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/graph_components/converters/nlu_message_converter.py` & `rasa-3.6.0a1/rasa/graph_components/converters/nlu_message_converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/graph_components/providers/domain_for_core_training_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/domain_for_core_training_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/graph_components/providers/domain_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/domain_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/graph_components/providers/forms_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/forms_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/graph_components/providers/nlu_training_data_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/nlu_training_data_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/graph_components/providers/responses_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/responses_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/graph_components/providers/rule_only_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/rule_only_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/graph_components/providers/story_graph_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/story_graph_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/graph_components/providers/training_tracker_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/training_tracker_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/graph_components/validators/default_recipe_validator.py` & `rasa-3.6.0a1/rasa/graph_components/validators/default_recipe_validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/graph_components/validators/finetuning_validator.py` & `rasa-3.6.0a1/rasa/graph_components/validators/finetuning_validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/jupyter.py` & `rasa-3.6.0a1/rasa/jupyter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/model.py` & `rasa-3.6.0a1/rasa/model.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/model_testing.py` & `rasa-3.6.0a1/rasa/model_testing.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/model_training.py` & `rasa-3.6.0a1/rasa/model_training.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/classifiers/diet_classifier.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/diet_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/classifiers/fallback_classifier.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/fallback_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/classifiers/keyword_intent_classifier.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/keyword_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/classifiers/logistic_regression_classifier.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/logistic_regression_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/classifiers/mitie_intent_classifier.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/mitie_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/classifiers/regex_message_handler.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/regex_message_handler.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/classifiers/sklearn_intent_classifier.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/sklearn_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/constants.py` & `rasa-3.6.0a1/rasa/nlu/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/convert.py` & `rasa-3.6.0a1/rasa/nlu/convert.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/emulators/dialogflow.py` & `rasa-3.6.0a1/rasa/nlu/emulators/dialogflow.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/emulators/emulator.py` & `rasa-3.6.0a1/rasa/nlu/emulators/emulator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/emulators/luis.py` & `rasa-3.6.0a1/rasa/nlu/emulators/luis.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/emulators/wit.py` & `rasa-3.6.0a1/rasa/nlu/emulators/wit.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/extractors/crf_entity_extractor.py` & `rasa-3.6.0a1/rasa/nlu/extractors/crf_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/extractors/duckling_entity_extractor.py` & `rasa-3.6.0a1/rasa/nlu/extractors/duckling_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/extractors/entity_synonyms.py` & `rasa-3.6.0a1/rasa/nlu/extractors/entity_synonyms.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/extractors/extractor.py` & `rasa-3.6.0a1/rasa/nlu/extractors/extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/extractors/mitie_entity_extractor.py` & `rasa-3.6.0a1/rasa/nlu/extractors/mitie_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/extractors/regex_entity_extractor.py` & `rasa-3.6.0a1/rasa/nlu/extractors/regex_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/extractors/spacy_entity_extractor.py` & `rasa-3.6.0a1/rasa/nlu/extractors/spacy_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/featurizers/featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/model.py` & `rasa-3.6.0a1/rasa/nlu/model.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/persistor.py` & `rasa-3.6.0a1/rasa/nlu/persistor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/run.py` & `rasa-3.6.0a1/rasa/nlu/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/selectors/response_selector.py` & `rasa-3.6.0a1/rasa/nlu/selectors/response_selector.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/test.py` & `rasa-3.6.0a1/rasa/nlu/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import itertools
 import os
 import logging
-import structlog
 from pathlib import Path
 
 import numpy as np
 from collections import defaultdict, namedtuple
 from tqdm import tqdm
 from typing import (
     Iterable,
@@ -72,15 +71,14 @@
         {
             "text": Text,
             "entities": List[Dict[Text, Any]],
             "predicted_entities": List[Dict[Text, Any]],
         },
     )
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 # Exclude 'EntitySynonymMapper' and 'ResponseSelector' as their super class
 # performs entity extraction but those two classifiers don't
 ENTITY_PROCESSORS = {"EntitySynonymMapper", "ResponseSelector"}
 
 EXTRACTORS_WITH_CONFIDENCES = {"CRFEntityExtractor", "DIETClassifier"}
 
@@ -281,15 +279,17 @@
         for r in response_results
         if r.intent_response_key_prediction == r.intent_response_key_target
     ]
 
     if successes:
         rasa.shared.utils.io.dump_obj_as_json_to_file(successes_filename, successes)
         logger.info(f"Successful response predictions saved to {successes_filename}.")
-        structlogger.debug("test.write.response", successes=successes)
+        logger.debug(
+            f"\n\nSuccessfully predicted the following responses: \n{successes}"
+        )
     else:
         logger.info("No successful response predictions found.")
 
 
 def _response_errors(
     response_results: List[ResponseSelectionEvaluationResult],
 ) -> List[Dict]:
@@ -793,15 +793,17 @@
     successes = collect_successful_entity_predictions(
         entity_results, merged_predictions, merged_targets
     )
 
     if successes:
         rasa.shared.utils.io.dump_obj_as_json_to_file(successes_filename, successes)
         logger.info(f"Successful entity predictions saved to {successes_filename}.")
-        structlogger.debug("test.write.entities", successes=successes)
+        logger.debug(
+            f"\n\nSuccessfully predicted the following entities: \n{successes}"
+        )
     else:
         logger.info("No successful entity prediction found.")
 
 
 def collect_successful_entity_predictions(
     entity_results: List[EntityEvaluationResult],
     merged_predictions: List[Text],
@@ -983,17 +985,15 @@
     for i in range(len(sorted_entities) - 1):
         curr_ent = sorted_entities[i]
         next_ent = sorted_entities[i + 1]
         if (
             next_ent["start"] < curr_ent["end"]
             and next_ent["entity"] != curr_ent["entity"]
         ):
-            structlogger.warning(
-                "test.overlaping.entities", curr_ent=curr_ent, next_ent=next_ent
-            )
+            logger.warning(f"Overlapping entity {curr_ent} with {next_ent}")
             return True
 
     return False
 
 
 def find_intersecting_entities(token: Token, entities: List[Dict]) -> List[Dict]:
     """Finds the entities that intersect with a token.
@@ -1006,20 +1006,18 @@
     """
     candidates = []
     for e in entities:
         if is_token_within_entity(token, e):
             candidates.append(e)
         elif does_token_cross_borders(token, e):
             candidates.append(e)
-            structlogger.debug(
-                "test.intersecting.entities",
-                token_text=token.text,
-                token_start=token.start,
-                token_end=token.end,
-                entity=e,
+            logger.debug(
+                "Token boundary error for token {}({}, {}) "
+                "and entity {}"
+                "".format(token.text, token.start, token.end, e)
             )
     return candidates
 
 
 def pick_best_entity_fit(
     token: Token, candidates: List[Dict[Text, Any]]
 ) -> Optional[Dict[Text, Any]]:
```

### Comparing `rasa-3.6.0/rasa/nlu/tokenizers/jieba_tokenizer.py` & `rasa-3.6.0a1/rasa/nlu/tokenizers/jieba_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/tokenizers/mitie_tokenizer.py` & `rasa-3.6.0a1/rasa/nlu/tokenizers/mitie_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/tokenizers/spacy_tokenizer.py` & `rasa-3.6.0a1/rasa/nlu/tokenizers/spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/tokenizers/tokenizer.py` & `rasa-3.6.0a1/rasa/nlu/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/tokenizers/whitespace_tokenizer.py` & `rasa-3.6.0a1/rasa/nlu/tokenizers/whitespace_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/utils/__init__.py` & `rasa-3.6.0a1/rasa/nlu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/utils/bilou_utils.py` & `rasa-3.6.0a1/rasa/nlu/utils/bilou_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/utils/hugging_face/registry.py` & `rasa-3.6.0a1/rasa/nlu/utils/hugging_face/registry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py` & `rasa-3.6.0a1/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/utils/mitie_utils.py` & `rasa-3.6.0a1/rasa/nlu/utils/mitie_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/utils/pattern_utils.py` & `rasa-3.6.0a1/rasa/nlu/utils/pattern_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/nlu/utils/spacy_utils.py` & `rasa-3.6.0a1/rasa/nlu/utils/spacy_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/plugin.py` & `rasa-3.6.0a1/rasa/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,16 +75,17 @@
     """Hook specification to modify the default recipe graph for prediction.
 
     Modifications are made in-place.
     """
 
 
 @hookspec  # type: ignore[misc]
-def get_version_info() -> Tuple[Text, Text]:  # type: ignore[empty-body]
+def get_version_info() -> Tuple[Text, Text]:
     """Hook specification for getting plugin version info."""
+    return "", ""
 
 
 @hookspec  # type: ignore[misc]
 def configure_commandline(cmdline_arguments: argparse.Namespace) -> Optional[Text]:
     """Hook specification for configuring plugin CLI."""
 
 
@@ -132,14 +133,19 @@
     domain: "Domain",
     event_broker: Optional["EventBroker"],
 ) -> "TrackerStore":
     """Hook specification for wrapping with AuthRetryTrackerStore."""
 
 
 @hookspec(firstresult=True)  # type: ignore[misc]
-def init_anonymization_pipeline(endpoints_file: Optional[Text]) -> None:
-    """Hook specification for initialising the anonymization pipeline."""
+def read_anonymization_rules(  # type: ignore[empty-body]
+    endpoints_file: Optional[Text],
+) -> List[Any]:
+    """Hook specification for reading anonymization rules."""
 
 
 @hookspec(firstresult=True)  # type: ignore[misc]
-def get_anonymization_pipeline() -> Optional[Any]:
-    """Hook specification for getting the anonymization pipeline."""
+def create_anonymization_pipeline(
+    anonymization_rules: Optional[List[Any]],
+    event_broker_config: Optional["EndpointConfig"],
+) -> Optional[Any]:
+    """Hook specification for creating the anonymization pipeline."""
```

### Comparing `rasa-3.6.0/rasa/server.py` & `rasa-3.6.0a1/rasa/server.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/constants.py` & `rasa-3.6.0a1/rasa/shared/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/constants.py` & `rasa-3.6.0a1/rasa/shared/core/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/conversation.py` & `rasa-3.6.0a1/rasa/shared/core/conversation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/domain.py` & `rasa-3.6.0a1/rasa/shared/core/domain.py`

 * *Files 3% similar despite different names*

```diff
@@ -235,15 +235,14 @@
             The instantiated `Domain` object.
         """
         duplicates = data.pop("duplicates", None)
         if duplicates:
             warn_about_duplicates_found_during_domain_merging(duplicates)
 
         responses = data.get(KEY_RESPONSES, {})
-        response_ids_per_response = cls._collect_response_ids(responses)
 
         domain_slots = data.get(KEY_SLOTS, {})
         if domain_slots:
             rasa.shared.core.slot_mappings.validate_slot_mappings(domain_slots)
         slots = cls.collect_slots(domain_slots)
         domain_actions = data.get(KEY_ACTIONS, [])
         actions = cls._collect_action_names(domain_actions)
@@ -266,15 +265,14 @@
             slots=slots,
             responses=responses,
             action_names=actions,
             forms=data.get(KEY_FORMS, {}),
             data=Domain._cleaned_data(data),
             action_texts=data.get(KEY_E2E_ACTIONS, []),
             session_config=session_config,
-            response_ids_per_response=response_ids_per_response,
             **additional_arguments,
         )
 
     @staticmethod
     def _get_session_config(session_config: Dict) -> SessionConfig:
         session_expiration_time_min = session_config.get(SESSION_EXPIRATION_TIME_KEY)
 
@@ -766,15 +764,14 @@
 
         self.form_names, self.forms, overridden_form_actions = self._initialize_forms(
             forms
         )
         action_names += overridden_form_actions
 
         self.responses = responses
-        self.response_ids_per_response = kwargs.get("response_ids_per_response", {})
 
         self.action_texts = action_texts if action_texts is not None else []
 
         data_copy = copy.deepcopy(data)
         self._data = self._preprocess_domain_dict(
             data_copy,
             store_entities_as_slots,
@@ -1915,74 +1912,14 @@
                         action_names += [action_name]
 
             elif action.startswith("validate_"):
                 action_names += [action]
 
         return action_names
 
-    @staticmethod
-    def _collect_response_ids(
-        responses: Dict[Text, List[Dict[Text, Any]]]
-    ) -> Dict[Text, Set[Text]]:
-        """Collects all response ids.
-
-        Args:
-            responses: The responses to collect the ids from.
-
-        Returns:
-            A dictionary mapping the response names to the set of response ids.
-        """
-        response_ids: Set[Text] = set()
-        response_ids_per_response: Dict[Text, Set[Text]] = {}
-        for response_name, response_variations in responses.items():
-            response_ids_for_response = (
-                Domain._collect_response_ids_for_response_variations(
-                    response_variations
-                )
-            )
-
-            already_present_response_ids = response_ids_for_response.intersection(
-                response_ids
-            )
-
-            if len(already_present_response_ids) > 0:
-                rasa.shared.utils.io.raise_warning(
-                    f"Duplicate response ids "
-                    f"'{already_present_response_ids}' "
-                    f"defined in domain."
-                )
-
-            response_ids.update(response_ids_for_response)
-            response_ids_per_response[response_name] = response_ids_for_response
-        return response_ids_per_response
-
-    @staticmethod
-    def _collect_response_ids_for_response_variations(
-        response_variations: List[Dict[Text, Any]]
-    ) -> Set[Text]:
-        """Collects all response ids of a particular response key name.
-
-        Args:
-            response_variations: The responses variations to collect the ids from.
-
-        Returns:
-            A set of response ids.
-        """
-        response_ids = set()
-        for response_variation in response_variations:
-            response_variation_id = response_variation.get("id")
-            if response_variation_id:
-                if response_variation_id in response_ids:
-                    rasa.shared.utils.io.raise_warning(
-                        f"Duplicate response id '{response_variation_id}' "
-                        f"defined in domain."
-                    )
-                response_ids.add(response_variation_id)
-        return response_ids
-
 
 def warn_about_duplicates_found_during_domain_merging(
     duplicates: Dict[Text, List[Text]]
 ) -> None:
     """Emits warning about found duplicates while loading multiple domain paths."""
     message = ""
     for key in [
```

### Comparing `rasa-3.6.0/rasa/shared/core/events.py` & `rasa-3.6.0a1/rasa/shared/core/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import abc
 import json
 import logging
-import structlog
 import re
 from abc import ABC
 
 import jsonpickle
 import time
 import uuid
 from dateutil import parser
@@ -95,32 +94,35 @@
             ENTITIES: List[EntityPrediction],
             "message_id": Optional[Text],
             "metadata": Dict,
         },
         total=False,
     )
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 
 def deserialise_events(serialized_events: List[Dict[Text, Any]]) -> List["Event"]:
     """Convert a list of dictionaries to a list of corresponding events.
 
     Example format:
         [{"event": "slot", "value": 5, "name": "my_slot"}]
     """
+
     deserialised = []
 
     for e in serialized_events:
         if "event" in e:
             event = Event.from_parameters(e)
             if event:
                 deserialised.append(event)
             else:
-                structlogger.warning("event.deserialization.failed", rasa_event=event)
+                logger.warning(
+                    f"Unable to parse event '{event}' while deserialising. The event"
+                    " will be ignored."
+                )
 
     return deserialised
 
 
 def deserialise_entities(entities: Union[Text, List[Any]]) -> List[Dict[Text, Any]]:
     if isinstance(entities, str):
         entities = json.loads(entities)
@@ -352,14 +354,15 @@
         return result[0] if result else None
 
     @staticmethod
     def resolve_by_type(
         type_name: Text, default: Optional[Type["Event"]] = None
     ) -> Optional[Type["Event"]]:
         """Returns a slots class by its type name."""
+
         for cls in rasa.shared.utils.common.all_subclasses(Event):
             if cls.type_name == type_name:
                 return cls
         if type_name == "topic":
             return None  # backwards compatibility to support old TopicSet evts
         elif default is not None:
             return default
```

### Comparing `rasa-3.6.0/rasa/shared/core/generator.py` & `rasa-3.6.0a1/rasa/shared/core/generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/slot_mappings.py` & `rasa-3.6.0a1/rasa/shared/core/slot_mappings.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/slots.py` & `rasa-3.6.0a1/rasa/shared/core/slots.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/trackers.py` & `rasa-3.6.0a1/rasa/shared/core/trackers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/training_data/loading.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/loading.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/training_data/story_reader/story_reader.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/story_reader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/training_data/story_reader/story_step_builder.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/story_step_builder.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/training_data/story_reader/yaml_story_reader.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/yaml_story_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import functools
 import json
 from json import JSONDecodeError
 import logging
-import structlog
 from pathlib import Path
 import re
 from re import Match, Pattern
 from typing import Dict, Text, List, Any, Optional, Union, Tuple
 
 from rasa.shared.core.domain import Domain
 import rasa.shared.data
@@ -43,15 +42,14 @@
 from rasa.shared.core.constants import RULE_SNIPPET_ACTION_NAME
 from rasa.shared.core.events import UserUttered, SlotSet, ActiveLoop
 from rasa.shared.core.training_data.story_reader.story_reader import StoryReader
 from rasa.shared.core.training_data.structures import StoryStep
 from rasa.shared.nlu.training_data.message import Message
 
 logger = logging.getLogger(__name__)
-structlogger = structlog.get_logger()
 
 KEY_STORIES = "stories"
 KEY_STORY_NAME = "story"
 KEY_RULES = "rules"
 KEY_RULE_NAME = "rule"
 KEY_STEPS = "steps"
 KEY_ENTITIES = "entities"
@@ -142,14 +140,15 @@
 
         Args:
             parsed_content: The parsed YAML as a dictionary.
 
         Returns:
             The parsed stories or rules.
         """
+
         if not rasa.shared.utils.validation.validate_training_data_format_version(
             parsed_content, self.source_name
         ):
             return []
 
         for key, parser_class in {
             KEY_STORIES: StoryParser,
@@ -199,14 +198,15 @@
 
         Args:
             file_path: Path of the file which should be checked.
 
         Returns:
             `True` if it's a conversation test file, otherwise `False`.
         """
+
         return cls._has_test_prefix(file_path) and cls.is_stories_file(file_path)
 
     def get_steps(self) -> List[StoryStep]:
         self._add_current_stories_to_result()
         return self.story_steps
 
     def parse_data(self, data: List[Dict[Text, Any]]) -> None:
@@ -624,15 +624,15 @@
         # Try to match the pattern.
         match = YAMLStoryReader._regex_message_pattern().match(user_text)
 
         # If it doesn't match, then (potentially) something went wrong, because the
         # message text did start with the special prefix -- however, a user might
         # just have decided to start their text this way.
         if not match:
-            structlogger.warning("message.parsing.failed", user_text=user_text)
+            logger.warning(f"Failed to parse intent end entities from '{user_text}'.")
             return message
 
         # Extract attributes from the match - and validate it via the domain.
         intent_name = YAMLStoryReader._intent_name_from_regex_match(match, domain)
         confidence = YAMLStoryReader._confidences_from_regex_match(match)
         entities = YAMLStoryReader._entities_from_regex_match(
             match, domain, entity_extractor_name
```

### Comparing `rasa-3.6.0/rasa/shared/core/training_data/story_writer/story_writer.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/story_writer/story_writer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/training_data/story_writer/yaml_story_writer.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/story_writer/yaml_story_writer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/training_data/structures.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/structures.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/training_data/visualization.html` & `rasa-3.6.0a1/rasa/shared/core/training_data/visualization.html`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/core/training_data/visualization.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/visualization.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/data.py` & `rasa-3.6.0a1/rasa/shared/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/exceptions.py` & `rasa-3.6.0a1/rasa/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/importers/importer.py` & `rasa-3.6.0a1/rasa/shared/importers/importer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/importers/multi_project.py` & `rasa-3.6.0a1/rasa/shared/importers/multi_project.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/importers/rasa.py` & `rasa-3.6.0a1/rasa/shared/importers/rasa.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/importers/utils.py` & `rasa-3.6.0a1/rasa/shared/importers/utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/constants.py` & `rasa-3.6.0a1/rasa/shared/nlu/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/entities_parser.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/entities_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/features.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/features.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/formats/dialogflow.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/dialogflow.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/formats/luis.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/luis.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/formats/rasa.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/rasa.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/formats/rasa_yaml.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/rasa_yaml.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/formats/readerwriter.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/readerwriter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/formats/wit.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/wit.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/loading.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/loading.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/lookup_tables_parser.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/lookup_tables_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/message.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/message.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/schemas/data_schema.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/data_schema.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/schemas/nlu.yml` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/nlu.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/schemas/responses.yml` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/responses.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,14 @@
       nullable: False
       func: require_response_keys
       sequence:
       - type: "map"
         required: True
         allowempty: False
         mapping:
-          id:
-            type: "str"
-            required: False
           text:
             type: "str"
           image:
             type: "str"
           custom:
             type: "map"
             allowempty: True
```

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/synonyms_parser.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/synonyms_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/training_data.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/training_data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/nlu/training_data/util.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/util.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/utils/cli.py` & `rasa-3.6.0a1/rasa/shared/utils/cli.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/utils/common.py` & `rasa-3.6.0a1/rasa/shared/utils/common.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/utils/io.py` & `rasa-3.6.0a1/rasa/shared/utils/io.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/utils/pykwalify_extensions.py` & `rasa-3.6.0a1/rasa/shared/utils/pykwalify_extensions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/utils/schemas/domain.yml` & `rasa-3.6.0a1/rasa/shared/utils/schemas/domain.yml`

 * *Files 3% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                   conditions:
                     type: "seq"
                     sequence:
                       - type: "map"
                         mapping:
                           active_loop:
                             type: "str"
-                            nullable: True
+                            required: True
                           requested_slot:
                             type: "str"
   forms:
     type: "map"
     required: False
     mapping:
       regex;([A-Za-z]+):
```

### Comparing `rasa-3.6.0/rasa/shared/utils/schemas/events.py` & `rasa-3.6.0a1/rasa/shared/utils/schemas/events.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/utils/schemas/model_config.yml` & `rasa-3.6.0a1/rasa/shared/utils/schemas/model_config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/utils/schemas/stories.yml` & `rasa-3.6.0a1/rasa/shared/utils/schemas/stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/shared/utils/validation.py` & `rasa-3.6.0a1/rasa/shared/utils/validation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/telemetry.py` & `rasa-3.6.0a1/rasa/telemetry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/common.py` & `rasa-3.6.0a1/rasa/utils/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -515,14 +515,19 @@
     # bytes to MiB
     return size / 1_048_576
 
 
 def copy_directory(source: Path, destination: Path) -> None:
     """Copies the content of one directory into another.
 
+    Unlike `shutil.copytree` this doesn't raise if `destination` already exists.
+
+    # TODO: Drop this in favor of `shutil.copytree(..., dirs_exist_ok=True)` when
+    # dropping Python 3.7.
+
     Args:
         source: The directory whose contents should be copied to `destination`.
         destination: The directory which should contain the content `source` in the end.
 
     Raises:
         ValueError: If destination is not empty.
     """
@@ -531,15 +536,19 @@
 
     if list(destination.glob("*")):
         raise ValueError(
             f"Destination path '{destination}' is not empty. Directories "
             f"can only be copied to empty directories."
         )
 
-    shutil.copytree(source, destination, dirs_exist_ok=True)
+    for item in source.glob("*"):
+        if item.is_dir():
+            shutil.copytree(item, destination / item.name)
+        else:
+            shutil.copy2(item, destination / item.name)
 
 
 def find_unavailable_packages(package_names: List[Text]) -> Set[Text]:
     """Tries to import all package names and returns the packages where it failed.
 
     Args:
         package_names: The package names to import.
```

### Comparing `rasa-3.6.0/rasa/utils/converter.py` & `rasa-3.6.0a1/rasa/utils/converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/endpoints.py` & `rasa-3.6.0a1/rasa/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/io.py` & `rasa-3.6.0a1/rasa/utils/io.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/plotting.py` & `rasa-3.6.0a1/rasa/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/tensorflow/callback.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/tensorflow/constants.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/tensorflow/crf.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/crf.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/tensorflow/data_generator.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/data_generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/tensorflow/environment.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/environment.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/tensorflow/layers.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/layers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/tensorflow/layers_utils.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/layers_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/tensorflow/model_data.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/model_data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/tensorflow/model_data_utils.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/model_data_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/tensorflow/models.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/models.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/tensorflow/rasa_layers.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/rasa_layers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/tensorflow/transformer.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/transformer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/utils/train_utils.py` & `rasa-3.6.0a1/rasa/utils/train_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/rasa/validator.py` & `rasa-3.6.0a1/rasa/validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.6.0/PKG-INFO` & `rasa-3.6.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasa
-Version: 3.6.0
+Version: 3.6.0a1
 Summary: Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants
 Home-page: https://rasa.com
 License: Apache-2.0
 Keywords: nlp,machine-learning,machine-learning-library,bot,bots,botkit,rasa conversational-agents,conversational-ai,chatbot,chatbot-framework,bot-framework
 Author: Rasa Technologies GmbH
 Author-email: hi@rasa.com
 Maintainer: Tom Bocklisch
@@ -23,21 +23,21 @@
 Provides-Extra: jieba
 Provides-Extra: metal
 Provides-Extra: spacy
 Provides-Extra: transformers
 Requires-Dist: CacheControl (>=0.12.9,<0.13.0)
 Requires-Dist: PyJWT[crypto] (>=2.0.0,<3.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.0,<1.5.0)
-Requires-Dist: absl-py (>=0.9,<1.5)
+Requires-Dist: absl-py (>=0.9,<1.4)
 Requires-Dist: aio-pika (>=6.7.1,<8.2.4)
 Requires-Dist: aiogram (<2.26)
 Requires-Dist: aiohttp (>=3.6,!=3.7.4.post0,<3.9)
 Requires-Dist: apscheduler (>=3.6,<3.10)
 Requires-Dist: attrs (>=19.3,<22.2)
-Requires-Dist: boto3 (>=1.26.136,<2.0.0)
+Requires-Dist: boto3 (>=1.26.124,<2.0.0)
 Requires-Dist: cloudpickle (>=1.2,<2.3)
 Requires-Dist: colorama (>=0.4.4,<0.5.0) ; sys_platform == "win32"
 Requires-Dist: colorclass (>=2.2,<2.3)
 Requires-Dist: coloredlogs (>=10,<16)
 Requires-Dist: colorhash (>=1.0.2,<1.3.0)
 Requires-Dist: confluent-kafka (>=1.9.2,<3.0.0)
 Requires-Dist: dask (==2022.10.2) ; python_version >= "3.8" and python_version < "3.11"
@@ -48,15 +48,14 @@
 Requires-Dist: jieba (>=0.39,<0.43) ; extra == "jieba" or extra == "full"
 Requires-Dist: joblib (>=0.15.1,<1.3.0)
 Requires-Dist: jsonpickle (>=1.3,<3.1)
 Requires-Dist: jsonschema (>=3.2,<4.18)
 Requires-Dist: matplotlib (>=3.1,<3.6)
 Requires-Dist: mattermostwrapper (>=2.2,<2.3)
 Requires-Dist: networkx (>=2.4,<2.7)
-Requires-Dist: numpy (==1.22.3) ; sys_platform == "Windows" and platform_python_implementation != "PyPy" and python_version == "3.10"
 Requires-Dist: numpy (>=1.19.2,<1.22.0) ; python_full_version >= "3.7.0" and python_full_version < "3.8.0"
 Requires-Dist: numpy (>=1.19.2,<1.25.0) ; python_version >= "3.8" and python_version < "3.11"
 Requires-Dist: packaging (>=20.0,<21.0)
 Requires-Dist: pluggy (>=1.0.0,<2.0.0)
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: prompt-toolkit (>=3.0,<3.0.29)
 Requires-Dist: protobuf (>=3.9.2,<3.20)
@@ -68,19 +67,19 @@
 Requires-Dist: python-dateutil (>=2.8,<2.9)
 Requires-Dist: python-engineio (>=4,<6,!=5.0.0)
 Requires-Dist: python-socketio (>=4.4,<6)
 Requires-Dist: pytz (>=2019.1,<2023.0)
 Requires-Dist: pyyaml (>=5.3.1,<6.0)
 Requires-Dist: questionary (>=1.5.1,<1.11.0)
 Requires-Dist: randomname (>=0.1.5,<0.2.0)
-Requires-Dist: rasa-sdk (>=3.6.0,<3.7.0)
+Requires-Dist: rasa-sdk (>=3.6.0a1,<3.7.0)
 Requires-Dist: redis (>=4.5.3,<5.0)
 Requires-Dist: regex (>=2020.6,<2022.11)
 Requires-Dist: requests (>=2.23,<3.0)
-Requires-Dist: rocketchat_API (>=0.6.31,<1.31.0)
+Requires-Dist: rocketchat_API (>=0.6.31,<1.30.0)
 Requires-Dist: ruamel.yaml (>=0.16.5,<0.18.0)
 Requires-Dist: sanic (>=21.12,<21.13)
 Requires-Dist: sanic-cors (>=2.0.0,<2.1.0)
 Requires-Dist: sanic-jwt (>=1.6.0,<2.0.0)
 Requires-Dist: sanic-routing (>=0.7.2,<0.8.0)
 Requires-Dist: scikit-learn (>=0.22,<1.1) ; python_full_version >= "3.7.0" and python_full_version < "3.8.0"
 Requires-Dist: scikit-learn (>=0.22,<1.2) ; python_version >= "3.8" and python_version < "3.11"
@@ -89,31 +88,29 @@
 Requires-Dist: sentencepiece[sentencepiece] (>=0.1.99,<0.2.0) ; extra == "transformers" or extra == "full"
 Requires-Dist: sentry-sdk (>=0.17.0,<1.15.0)
 Requires-Dist: setuptools (>=41.0.0)
 Requires-Dist: sklearn-crfsuite (>=0.3,<0.4)
 Requires-Dist: slack-sdk (>=3.19.2,<4.0.0)
 Requires-Dist: spacy (>=3.1,<3.5) ; (sys_platform != "darwin" or platform_machine != "arm64") and (extra == "spacy" or extra == "full")
 Requires-Dist: spacy (>=3.4,<4.0) ; (sys_platform == "darwin" and platform_machine == "arm64") and (extra == "spacy" or extra == "full")
-Requires-Dist: structlog (>=23.1.0,<24.0.0)
-Requires-Dist: structlog-sentry (>=2.0.2,<3.0.0)
 Requires-Dist: tarsafe (>=0.0.3,<0.0.5)
-Requires-Dist: tensorflow (==2.11.1) ; sys_platform != "darwin" or platform_machine != "arm64"
+Requires-Dist: tensorflow (==2.11.0) ; sys_platform != "darwin" or platform_machine != "arm64"
 Requires-Dist: tensorflow-addons (==0.19.0) ; sys_platform == "linux" and platform_machine == "arm64" or sys_platform == "linux" and platform_machine == "aarch64"
 Requires-Dist: tensorflow-addons (>=0.18,<0.20) ; sys_platform != "linux" or platform_machine != "arm64" and platform_machine != "aarch64"
-Requires-Dist: tensorflow-cpu-aws (==2.11.1) ; sys_platform == "linux" and platform_machine == "arm64" or sys_platform == "linux" and platform_machine == "aarch64"
-Requires-Dist: tensorflow-intel (==2.11.1) ; sys_platform == "win32"
+Requires-Dist: tensorflow-cpu-aws (==2.11.0) ; sys_platform == "linux" and platform_machine == "arm64" or sys_platform == "linux" and platform_machine == "aarch64"
+Requires-Dist: tensorflow-intel (==2.11.0) ; sys_platform == "win32"
 Requires-Dist: tensorflow-io-gcs-filesystem (>=0.23.1,<0.32) ; sys_platform == "win32"
 Requires-Dist: tensorflow-macos (==2.11.0) ; sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: tensorflow-metal (==0.5.1) ; (sys_platform == "darwin" and platform_machine == "arm64") and (extra == "metal")
 Requires-Dist: tensorflow-text (==2.11.0) ; sys_platform != "win32" and platform_machine != "arm64" and platform_machine != "aarch64"
 Requires-Dist: tensorflow_hub (>=0.12.0,<0.13.0)
 Requires-Dist: terminaltables (>=3.1.0,<3.2.0)
 Requires-Dist: tqdm (>=4.31,<5.0)
 Requires-Dist: transformers (>=4.13.0,<=4.26.0) ; extra == "transformers" or extra == "full"
-Requires-Dist: twilio (>=6.26,<8.3)
+Requires-Dist: twilio (>=6.26,<8.2)
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
 Requires-Dist: typing-utils (>=0.1.0,<0.2.0)
 Requires-Dist: ujson (>=1.35,<6.0)
 Requires-Dist: webexteamssdk (>=1.1.1,<1.7.0)
 Requires-Dist: websockets (>=10.0,<11.0)
 Project-URL: Documentation, https://rasa.com/docs
 Project-URL: Repository, https://github.com/rasahq/rasa
```

