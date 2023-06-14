# Comparing `tmp/citrine-2.24.1.tar.gz` & `tmp/citrine-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/citrine-2.24.1.tar", last modified: Wed Jun 14 18:21:18 2023, max compression
+gzip compressed data, was "dist/citrine-2.8.0.tar", last modified: Thu Mar 16 19:22:06 2023, max compression
```

## Comparing `citrine-2.24.1.tar` & `citrine-2.8.0.tar`

### file list

```diff
@@ -1,177 +1,171 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11349 2023-06-14 18:18:57.000000 citrine-2.24.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1172 2023-06-14 18:21:18.000000 citrine-2.24.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      544 2023-06-14 18:18:57.000000 citrine-2.24.1/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-14 18:21:18.000000 citrine-2.24.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1860 2023-06-14 18:18:57.000000 citrine-2.24.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/
--rw-rw-r--   0 travis    (2000) travis    (2000)      343 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/__version__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/_rest/
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_rest/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2222 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_rest/ai_resource_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1316 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_rest/asynchronous_object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5877 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_rest/collection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3499 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_rest/engine_resource.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4354 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_rest/pageable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5112 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_rest/paginator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3870 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_rest/resource.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/_serialization/
--rw-rw-r--   0 travis    (2000) travis    (2000)       31 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_serialization/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      963 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_serialization/include_parent_properties.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      643 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_serialization/polymorphic_serializable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40558 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_serialization/properties.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      912 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_serialization/serializable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13685 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_session.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/_utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)       31 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5085 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_utils/batcher.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11282 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_utils/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2930 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/_utils/template_util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/builders/
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/builders/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30500 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/builders/auto_configure.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9238 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/builders/descriptors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13111 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/builders/design_spaces.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10073 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/builders/predictors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2891 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/builders/scores.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2109 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/citrine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5654 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/gemtables/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/gemtables/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16098 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/gemtables/columns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2522 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/gemtables/rows.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51566 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/gemtables/variables.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/informatics/
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/informatics/constraints/
--rw-rw-r--   0 travis    (2000) travis    (2000)      291 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/constraints/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1245 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/constraints/categorical_constraint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1441 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/constraints/constraint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1709 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/constraints/ingredient_count_constraint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2105 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/constraints/ingredient_fraction_constraint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7647 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/constraints/ingredient_ratio_constraint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1978 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/constraints/label_fraction_constraint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2099 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/constraints/scalar_range_constraint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5387 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/data_sources.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8896 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/descriptors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8590 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/design_candidate.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/informatics/design_spaces/
--rw-rw-r--   0 travis    (2000) travis    (2000)      198 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/design_spaces/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1526 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/design_spaces/data_source_design_space.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1802 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/design_spaces/design_space.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2124 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/design_spaces/enumerated_design_space.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3321 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/design_spaces/formulation_design_space.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3015 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/design_spaces/product_design_space.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      526 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/design_spaces/sample_design_space.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2775 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/dimensions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/informatics/executions/
--rw-rw-r--   0 travis    (2000) travis    (2000)      136 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/executions/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/executions/design_execution.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2775 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/executions/execution.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1940 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/executions/generative_design_execution.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2321 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/executions/predictor_evaluation_execution.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3478 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/executions/sample_design_space_execution.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/experiment_values.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5865 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/generative_design.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1218 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/modules.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1901 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/objectives.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1147 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predict_request.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6619 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictor_evaluation_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10281 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictor_evaluation_result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7653 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictor_evaluator.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/informatics/predictors/
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4133 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/auto_ml_predictor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7381 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/chemical_formula_featurizer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1944 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/expression_predictor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5645 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/graph_predictor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1579 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/ingredient_fractions_predictor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2560 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/ingredients_to_formulation_predictor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1477 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/label_fractions_predictor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5444 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/mean_property_predictor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7508 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/molecular_structure_featurizer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6938 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/node.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      277 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/predictor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3361 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/simple_mixture_predictor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1064 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/single_predict_request.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      852 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/predictors/single_prediction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/reports.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4835 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/scores.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/informatics/workflows/
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/workflows/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2694 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/workflows/design_workflow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2183 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/workflows/predictor_evaluation_workflow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/informatics/workflows/workflow.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/jobs/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/jobs/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5243 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/jobs/job.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5735 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/jobs/waiting.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/resources/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1326 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/api_error.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1069 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/attribute_templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1699 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/audit_info.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10984 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/branch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2643 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/condition_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29166 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/data_concepts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6996 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/data_objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2135 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/data_version_update.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21551 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/dataset.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4401 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/delete.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2766 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/descriptors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4390 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/design_execution.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6818 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/design_space.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6577 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/design_workflow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6887 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/experiment_datasource.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38729 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/file_link.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9098 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/gemd_resource.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14882 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/gemtables.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3198 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/generative_design_execution.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9602 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/ingestion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7574 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/ingredient_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6994 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/ingredient_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1388 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/job.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7854 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/material_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5779 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/material_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4501 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/material_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6434 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/measurement_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4878 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/measurement_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7130 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/measurement_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2471 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/module.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      610 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/object_runs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      563 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/object_specs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      897 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/object_templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2625 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/parameter_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27663 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/predictor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6688 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/predictor_evaluation_execution.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4185 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/predictor_evaluation_workflow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5179 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/process_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5202 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/process_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6076 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/process_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24308 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/project.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      725 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/project_member.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      146 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/project_roles.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2598 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/property_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1478 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/report.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      873 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/response.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3562 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/sample_design_space_execution.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      880 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/status_detail.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25626 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/table_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14286 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/team.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      702 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2847 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/resources/user.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine/seeding/
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/seeding/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6541 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/seeding/find_or_create.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      903 2023-06-14 18:18:57.000000 citrine-2.24.1/src/citrine/seeding/sort_gems.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1172 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     6613 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      311 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-14 18:21:18.000000 citrine-2.24.1/src/citrine.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 18:21:18.000000 citrine-2.24.1/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3620 2023-06-14 18:18:57.000000 citrine-2.24.1/tests/test_citrine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11073 2023-06-14 18:18:57.000000 citrine-2.24.1/tests/test_session.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11349 2023-03-16 19:20:10.000000 citrine-2.8.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1097 2023-03-16 19:22:06.000000 citrine-2.8.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      544 2023-03-16 19:20:10.000000 citrine-2.8.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-03-16 19:22:06.000000 citrine-2.8.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1773 2023-03-16 19:20:10.000000 citrine-2.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      343 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/__version__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/_rest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       58 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_rest/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2222 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_rest/ai_resource_metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1316 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_rest/asynchronous_object.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5408 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_rest/collection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3499 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_rest/engine_resource.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4185 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_rest/pageable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5112 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_rest/paginator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1992 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_rest/resource.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/_serialization/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       31 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_serialization/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      963 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_serialization/include_parent_properties.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      643 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_serialization/polymorphic_serializable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34446 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_serialization/properties.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      912 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_serialization/serializable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13685 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_session.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/_utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       31 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5085 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_utils/batcher.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7598 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_utils/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2930 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/_utils/template_util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/builders/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       55 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/builders/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30465 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/builders/auto_configure.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9238 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/builders/descriptors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13111 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/builders/design_spaces.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10073 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/builders/predictors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2891 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/builders/scores.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2109 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/citrine.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4263 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/exceptions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/gemtables/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/gemtables/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16098 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/gemtables/columns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2522 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/gemtables/rows.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51689 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/gemtables/variables.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/informatics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       64 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/informatics/constraints/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      291 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/constraints/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1245 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/constraints/categorical_constraint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1441 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/constraints/constraint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1717 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/constraints/ingredient_count_constraint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2109 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/constraints/ingredient_fraction_constraint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4286 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/constraints/ingredient_ratio_constraint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2022 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/constraints/label_fraction_constraint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2099 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/constraints/scalar_range_constraint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5387 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/data_sources.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8969 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/descriptors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5189 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/design_candidate.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/informatics/design_spaces/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      198 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/design_spaces/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1526 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/design_spaces/data_source_design_space.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/design_spaces/design_space.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2124 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/design_spaces/enumerated_design_space.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3321 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/design_spaces/formulation_design_space.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3502 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/design_spaces/product_design_space.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2775 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/dimensions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/informatics/executions/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      136 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/executions/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5324 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/executions/design_execution.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4495 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/executions/generative_design_execution.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3848 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/executions/predictor_evaluation_execution.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/experiment_values.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3458 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/generative_design.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1218 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/modules.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1901 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/objectives.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1147 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predict_request.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6619 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictor_evaluation_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10281 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictor_evaluation_result.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7653 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictor_evaluator.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/informatics/predictors/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      447 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4096 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/auto_ml_predictor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7520 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/chemical_formula_featurizer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2078 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/expression_predictor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3168 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/graph_predictor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1688 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/ingredient_fractions_predictor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2333 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/ingredients_to_formulation_predictor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1586 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/label_fractions_predictor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5458 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/mean_property_predictor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7593 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/molecular_structure_featurizer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4837 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/predictor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2670 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/simple_mixture_predictor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1028 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/single_predict_request.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      820 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/predictors/single_prediction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/reports.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4835 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/scores.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/informatics/workflows/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      115 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/workflows/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2694 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/workflows/design_workflow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2183 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/workflows/predictor_evaluation_workflow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/informatics/workflows/workflow.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/jobs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/jobs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5105 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/jobs/job.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5458 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/jobs/waiting.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/resources/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      140 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/api_error.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      617 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/attribute_templates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1781 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/audit_info.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10482 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/branch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/condition_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35612 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/data_concepts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6530 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/data_objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2135 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/data_version_update.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20037 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/dataset.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4405 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/delete.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2487 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/descriptors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4022 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/design_execution.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5981 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/design_space.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6795 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/design_workflow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6887 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/experiment_datasource.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33712 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/file_link.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9098 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/gemd_resource.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14898 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/gemtables.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3198 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/generative_design_execution.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7882 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/ingredient_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7209 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/ingredient_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      227 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/job.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8812 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/material_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5874 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/material_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4570 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/material_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6682 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/measurement_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5113 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/measurement_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/measurement_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2471 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/module.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      553 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/object_runs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      563 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/object_specs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      592 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/object_templates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3197 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/parameter_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18640 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/predictor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6100 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/predictor_evaluation_execution.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4185 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/predictor_evaluation_workflow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5570 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/process_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5473 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/process_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/process_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24305 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/project.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      725 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/project_member.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      146 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/project_roles.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3095 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/property_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1478 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/report.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      873 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/response.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      948 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/status_detail.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25639 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/table_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14278 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/team.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      702 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/templates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2847 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/resources/user.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine/seeding/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       50 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/seeding/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6541 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/seeding/find_or_create.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      903 2023-03-16 19:20:10.000000 citrine-2.8.0/src/citrine/seeding/sort_gems.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1097 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6303 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      313 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-03-16 19:22:06.000000 citrine-2.8.0/src/citrine.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-16 19:22:06.000000 citrine-2.8.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3620 2023-03-16 19:20:10.000000 citrine-2.8.0/tests/test_citrine.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11073 2023-03-16 19:20:10.000000 citrine-2.8.0/tests/test_session.py
```

### Comparing `citrine-2.24.1/LICENSE` & `citrine-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/PKG-INFO` & `citrine-2.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: citrine
-Version: 2.24.1
+Version: 2.8.0
 Summary: Python library for the Citrine Platform
 Home-page: http://github.com/CitrineInformatics/citrine-python
 Author: Citrine Informatics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: builders
 Provides-Extra: ../tests
 License-File: LICENSE
 
 # Getting Started
 `citrine-python` is the Python library for the Citrine Platform. To get started, install `citrine-python`:
```

### Comparing `citrine-2.24.1/README.md` & `citrine-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/setup.py` & `citrine-2.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,48 +9,46 @@
 about = {}
 with open(path.join(this_directory, 'src', 'citrine', '__version__.py'), 'r') as f:
     exec(f.read(), about)
 
 setup(name='citrine',
       # Update this in src/citrine/__version__.py
       version=about['__version__'],
-      python_requires='>=3.7',
       url='http://github.com/CitrineInformatics/citrine-python',
       description='Python library for the Citrine Platform',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Citrine Informatics',
       package_dir={'': 'src'},
       packages=find_packages(where='src'),
       install_requires=[
-          "requests>=2.31.0,<3",
+          "requests>=2.25.1,<3",
           "pyjwt>=2,<3",
-          "arrow>=0.15.4,<2",
-          "gemd>=1.15.0,<2",
+          "arrow>=0.15.4,<0.16",
+          "gemd>=1.9.0,<2",
           "boto3>=1.17.93,<2",
           "botocore>=1.20.95,<2",
-          "deprecation>=2.1.0,<3",
-          "urllib3>=1.26.5,<3",
+          "deprecation>=2.0.7,<3",
+          "urllib3>=1.26.5,<2",
           "tqdm>=4.62.3,<5"
       ],
       extras_require={
           "builders": [
-              "pandas>=1.3.5,<3"
+              "pandas>=1.1.5,<2"
           ],
           "../tests": [
-              "factory-boy>=2.12.0,<4",
-              "mock>=3.0.5,<5",
-              "pandas>=1.3.5,<3",
-              "pytest>=6.2.5,<8",
-              "pytz>=2020.1",
+              "factory-boy>=2.12.0,<3",
+              "mock>=3.0.5,<4",
+              "pandas>=1.1.5,<2",
+              "pytest>=6.2.5,<7",
+              "pytz>=2019.3",
               "requests-mock>=1.7.0,<2",
           ]
       },
       classifiers=[
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
-          'Programming Language :: Python :: 3.11',
       ],
-      )
+)
```

### Comparing `citrine-2.24.1/src/citrine/_rest/ai_resource_metadata.py` & `citrine-2.8.0/src/citrine/_rest/ai_resource_metadata.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/_rest/asynchronous_object.py` & `citrine-2.8.0/src/citrine/_rest/asynchronous_object.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/_rest/collection.py` & `citrine-2.8.0/src/citrine/_rest/collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from abc import abstractmethod
 from logging import getLogger
-from typing import Optional, Union, Generic, TypeVar, Iterable, Iterator, Sequence, Dict
-from urllib.parse import urlparse, urlencode
+from typing import Optional, Union, Generic, TypeVar, Iterable, Iterator
 from uuid import UUID
 
 from citrine._rest.pageable import Pageable
 from citrine._rest.paginator import Paginator
 from citrine._rest.resource import ResourceRef
 from citrine._utils.functions import format_escaped_url
 from citrine.exceptions import ModuleRegistrationFailedException, NonRetryableException
@@ -33,41 +32,24 @@
     _api_version: str = "v1"
 
     def _put_resource_ref(self, subpath: str, uid: Union[UUID, str]):
         url = self._get_path(subpath)
         ref = ResourceRef(uid)
         return self.session.put_resource(url, ref.dump(), version=self._api_version)
 
-    def _get_path(self,
-                  uid: Optional[Union[UUID, str]] = None,
-                  *,
-                  ignore_dataset: bool = False,
-                  action: Union[str, Sequence[str]] = [],
-                  query_terms: Dict[str, str] = {},
-                  ) -> str:
-        """Construct a url from __base_path__ and, optionally, id and/or action."""
+    def _get_path(self, uid: Optional[Union[UUID, str]] = None,
+                  ignore_dataset: Optional[bool] = False) -> str:
+        """Construct a url from __base_path__ and, optionally, id."""
+        subpath = format_escaped_url('/{}', uid) if uid else ''
         if ignore_dataset:
-            base = urlparse(self._dataset_agnostic_path_template)
+            return format_escaped_url(self._dataset_agnostic_path_template + subpath,
+                                      **self.__dict__)
         else:
-            base = urlparse(self._path_template)
-        path = base.path.split('/')
-
-        if uid is not None:
-            path.append("{uid}")
-
-        if isinstance(action, str):
-            action = [action]
-        else:
-            action = list(action)
-        path.extend(["{}"] * len(action))
-
-        query = urlencode(query_terms)
-        new_url = base._replace(path='/'.join(path), query=query).geturl()
-
-        return format_escaped_url(new_url, *action, **self.__dict__, uid=uid)
+            return format_escaped_url(self._path_template + subpath,
+                                      **self.__dict__)
 
     @abstractmethod
     def build(self, data: dict):
         """Build an individual element of the collection."""
 
     def get(self, uid: Union[UUID, str]) -> ResourceType:
         """Get a particular element of the collection."""
```

### Comparing `citrine-2.24.1/src/citrine/_rest/engine_resource.py` & `citrine-2.8.0/src/citrine/_rest/engine_resource.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/_rest/pageable.py` & `citrine-2.8.0/src/citrine/_rest/pageable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 from logging import getLogger
-from typing import Optional, Iterable, Dict, Tuple, Callable, Union, Sequence
+from typing import Optional, Iterable, Dict, Tuple, Callable, Union
 from uuid import UUID
 
 
 logger = getLogger(__name__)
 
 
 class Pageable():
     """Class that allows paging."""
 
     _collection_key: str = NotImplemented
     _api_version: str = "v1"
 
-    def _get_path(self,
-                  uid: Optional[Union[UUID, str]] = None,
-                  *,
-                  ignore_dataset: bool = False,
-                  action: Union[str, Sequence[str]] = [],
-                  query_terms: Dict[str, str] = {},
-                  ) -> str:
+    def _get_path(self, uid: Optional[Union[UUID, str]] = None,
+                  ignore_dataset: Optional[bool] = False) -> str:
         """Construct a url from __base_path__ and, optionally, id."""
         raise NotImplementedError  # pragma: no cover
 
     def _fetch_page(self,
                     path: Optional[str] = None,
                     fetch_func: Optional[Callable[..., dict]] = None,
                     page: Optional[int] = None,
```

### Comparing `citrine-2.24.1/src/citrine/_rest/paginator.py` & `citrine-2.8.0/src/citrine/_rest/paginator.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/_serialization/include_parent_properties.py` & `citrine-2.8.0/src/citrine/_serialization/include_parent_properties.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/_serialization/polymorphic_serializable.py` & `citrine-2.8.0/src/citrine/_serialization/polymorphic_serializable.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/_serialization/properties.py` & `citrine-2.8.0/src/citrine/_serialization/properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Property objects for typed setting and ser/de."""
 from abc import abstractmethod
 import typing
+from typing import Optional
 from datetime import datetime
-from inspect import signature
 from itertools import chain
 import uuid
 import arrow
-from functools import lru_cache
-import re
 
 from gemd.enumeration.base_enumeration import BaseEnumeration
 from gemd.entity.link_by_uid import LinkByUID
 from gemd.entity.dict_serializable import DictSerializable
 from gemd.util.impl import cached_isinstance as isinstance
 
 from citrine._serialization.serializable import Serializable
@@ -20,101 +18,64 @@
 SerializedType = typing.TypeVar('SerializedType')
 DeserializedType = typing.TypeVar('DeserializedType')
 SerializedInteger = typing.TypeVar('SerializedInteger', int, str)
 SerializedFloat = typing.TypeVar('SerializedFloat', float, str)
 
 
 class Property(typing.Generic[DeserializedType, SerializedType]):
-    """
-    Basic operating unit of a serialization layer.
-
-    By defining a Property as a class variable, access methods are defined and
-    a type-aware deserialization method is implemented for translating between
-    a dictionary-based representation and a Python object based representation.
-
-    Parameters
-    ----------
-    serialization_path: str
-        The location in the serialized structure where the value of interest can be
-        found.  The value can be nested in the structure, where separate keys are
-        joined by `.`.  Required in a top level property, but not necessary if
-        a property is wrapped by a container.
-    serializable: bool
-        Include the field when serializing an object to a dictionary; default: True
-    deserializable: bool
-        Look for the field when deserializing a dictionary into an object; default: True
-    default:  DeserializedType
-        If no value is found in an incoming dictionary, which value to use; default: None
-    override: bool
-        Use a parent class' accessor methods; default: False
-    use_init: bool
-        When deserializing, use the __init__ method instead of the setter
-
-    """
 
     def __init__(self,
                  serialization_path: typing.Optional[str] = None,
-                 *,
                  serializable: bool = True,
                  deserializable: bool = True,
                  default: typing.Optional[DeserializedType] = None,
-                 override: bool = False,
-                 use_init: bool = False
+                 override: bool = False
                  ):
         self.serialization_path = serialization_path
-        if override:
-            self._key: None = None
-        else:
-            self._key: str = '__' + str(uuid.uuid4())  # Make this object key human-readable
+        self._key: str = '__' + str(uuid.uuid4())  # Make this object key human readable
         self.serializable: bool = serializable
         self.deserializable: bool = deserializable
         self.default: typing.Optional[DeserializedType] = default
         # Distinguish between no default being provided and the default being None
-        self.optional: bool = False
-        self.use_init: bool = use_init
+        self.optional = False
+        self.override = override
 
     @property
     @abstractmethod
     def underlying_types(self) -> typing.Union[DeserializedType, typing.Tuple[DeserializedType]]:
         """Return the python types handled by this property."""
 
     @property
     @abstractmethod
     def serialized_types(self) -> typing.Union[SerializedType, typing.Tuple[SerializedType]]:
         """Return the types used to serialize this property."""
 
     def _error_source(self, base_class: type) -> str:
         """Construct a string of the base class name and the parameter that failed."""
         if base_class is not None:
-            return ' for {}:{}'.format(base_class.__name__, self.serialization_path)
+            return 'for {}:{}'.format(base_class.__name__, self.serialization_path)
         elif self.serialization_path:
-            return ' for {}'.format(self.serialization_path)
+            return 'for {}'.format(self.serialization_path)
         else:
             return ''
 
     def serialize(self, value: DeserializedType,
-                  base_class: typing.Optional[type] = None) -> SerializedType:
+                  base_class: Optional[type] = None) -> SerializedType:
         if not isinstance(value, self.underlying_types):
             base_name = self._error_source(base_class)
-            raise ValueError(
-                f'{type(value)} {value} is not one of valid types: '
-                f'{self.underlying_types}{base_name}'
-            )
+            raise ValueError('{} is not one of valid types: {} {}'.format(
+                value, self.underlying_types, base_name))
         return self._serialize(value)
 
     def deserialize(self, value: SerializedType,
-                    base_class: typing.Optional[type] = None) -> DeserializedType:
+                    base_class: Optional[type] = None) -> DeserializedType:
         if not isinstance(value, self.serialized_types):
-            if isinstance(value, self.underlying_types):
-                return value  # Don't worry if it was already deserialized
             base_name = self._error_source(base_class)
-            raise ValueError(
-                f'{type(value)} {value} is not one of valid types: '
-                f'{self.serialized_types}{base_name}'
-            )
+            raise ValueError('{} is not one of valid types: {} {}'.format(
+                value, self.serialized_types, base_name))
         return self._deserialize(value)
 
     @abstractmethod
     def _serialize(self, value: DeserializedType) -> SerializedType:
         """Perform serialization."""
 
     @abstractmethod
@@ -136,62 +97,48 @@
                 # or if its value is null.
                 # Use the default value and stop traversing, even if we have not yet reached
                 # the last field in the serialization path.
                 value = self.serialize(self.default)
                 break
             else:
                 value = next_value
-        return self.deserialize(value, base_class=None)  # always a dict
+        base_class = _get_base_class(data, self.serialization_path)
+        return self.deserialize(value, base_class=base_class)
 
     def serialize_to_dict(self, data: dict, value: DeserializedType) -> dict:
         if self.serialization_path is None:
             raise ValueError('No serialization path set!')
-
-        _data = data
-        fields = self.serialization_path.split('.')
-        for field in fields[:-1]:
-            _data = _data.setdefault(field, {})
-        _data[fields[-1]] = self.serialize(value, base_class=None)  # Always a dict
-        return data
+        else:
+            base_class = _get_base_class(data, self.serialization_path)
+            _data = data
+            fields = self.serialization_path.split('.')
+            for field in fields[:-1]:
+                _data = _data.setdefault(field, {})
+            _data[fields[-1]] = self.serialize(value, base_class=base_class)
+            return data
 
     def __get__(self, obj, objtype=None) -> DeserializedType:
         """Property getter, deferring to the getter of the parent class, if applicable."""
-        if self._key is None:
-            property_name, base_class = _get_key_and_base_class(self, type(obj))
-            if base_class is not None:
-                return getattr(base_class, property_name).fget(obj)
-            else:
-                raise AttributeError(
-                    f"No parent class could be resolved for '{property_name}' "
-                    f"in {obj.__class__}.  'override' should probably be false."
-                )
+        base_class = _get_base_class(obj, self.serialization_path)
+        if base_class is not None and self.override:
+            return getattr(base_class, self.serialization_path).fget(obj)
         else:
             return getattr(obj, self._key, self.default)
 
     def __set__(self, obj, value: typing.Union[SerializedType, DeserializedType]):
         """Property setter, deferring to the setter of the parent class, if applicable."""
-        property_name, base_class = _get_key_and_base_class(self, type(obj))
+        base_class = _get_base_class(obj, self.serialization_path)
         if issubclass(type(value), self.underlying_types):
             value_to_set = value
         else:
             # if value is not an underlying type, set its deserialized version.
             value_to_set = self.deserialize(value, base_class=base_class)
 
-        if self._key is None:
-            if base_class is not None:
-                prop = getattr(base_class, property_name)
-                if prop.fset is not None:  # It's a property with a setter
-                    prop.fset(obj, value_to_set)
-                else:  # It's a read-only property
-                    raise AttributeError(f"can't set attribute '{property_name}'")
-            else:
-                raise AttributeError(
-                    f"No parent class could be resolved for '{property_name}' in "
-                    f"{obj.__class__}.  'override' should probably be false."
-                )
+        if base_class is not None and self.override:
+            getattr(base_class, self.serialization_path).fset(obj, value_to_set)
         else:
             setattr(obj, self._key, value_to_set)
 
     def __str__(self):
         return '<Property {!r}>'.format(self.serialization_path)
 
 
@@ -199,65 +146,55 @@
 
     def __set__(self, obj, value: typing.Union[SerializedType, DeserializedType]):
         """
         Property setter for container property types.
 
         This setter defers to the subclass to implement the `_set_elements` logic
         """
-        property_name, base_class = _get_key_and_base_class(self, type(obj))
+        base_class = _get_base_class(obj, self.serialization_path)
         if issubclass(type(value), self.underlying_types):
             value_to_set = self._set_elements(value)
-        elif issubclass(type(value), self.serialized_types):
+        else:
             # if value is not an underlying type, set its deserialized version.
             value_to_set = self.deserialize(value, base_class=base_class)
-        else:
-            raise TypeError(
-                f"{value} is a {type(value)}, but {property_name} expects one of: "
-                f"{self.underlying_types}"
-            )
-
-        if self._key is None:
-            if base_class is not None:
-                prop = getattr(base_class, property_name)
-                if prop.fset is not None:  # It's a property with a setter
-                    prop.fset(obj, value_to_set)
-                else:  # It's a read-only property
-                    raise AttributeError(f"can't set attribute '{property_name}'")
-            else:
-                raise AttributeError(
-                    f"No parent class could be resolved for '{property_name}' "
-                    f"in {obj.__class__}.  'override' should probably be false."
-                )
+
+        if base_class is not None and self.override:
+            prop = getattr(base_class, self.serialization_path)
+            if prop.fset is not None:  # It's a property with a setter
+                prop.fset(obj, value_to_set)
+            else:  # It's a read-only property
+                setattr(obj, self._key, value_to_set)
         else:
             setattr(obj, self._key, value_to_set)
 
     @abstractmethod
     def _set_elements(self, value: typing.Union[SerializedType, DeserializedType]):
         """
         Perform any needed underlying element specific deserialization.
 
         Return the appropriate value to set
         """
 
 
-@lru_cache(maxsize=1024)
-def _get_key_and_base_class(prop: Property, klass: typing.Any) -> \
-        typing.Tuple[typing.Optional[str], typing.Optional[str]]:
+def _get_base_class(obj: object, key: str) -> type:
     """
-    Return the base class and class attribute name for the object and property.
+    Return the base class that has key as an attribute, if it exists.
 
-    Uses method resolution order to determine which base class would handle it.
+    If there are no base classes with key as an attribute, OR if there are multiple base classes
+    with key as an attribute, return None.
     """
-    mro = klass.__mro__  # Tuple of all base classes of obj
-    key = next((k for c in mro for k, v in c.__dict__.items() if v == prop), None)
-    if key is None:
-        return None, None
-
-    base_class = next((b for b in klass.__bases__ if hasattr(b, key)), None)
-    return key, base_class
+    base_classes = obj.__class__.__bases__  # Tuple of all base classes of obj
+    try:
+        classes_with_key = [base_class for base_class in base_classes if hasattr(base_class, key)]
+    except TypeError:
+        return None
+    if len(classes_with_key) == 1:
+        return classes_with_key[0]
+    else:
+        return None
 
 
 class Integer(Property[int, SerializedInteger]):
 
     @property
     def underlying_types(self):
         return int
@@ -412,28 +349,23 @@
 
 
 class List(PropertyCollection[list, list]):
 
     def __init__(self,
                  element_type: typing.Union[Property, typing.Type[Property]],
                  serialization_path: typing.Optional[str] = None,
-                 *,
                  serializable: bool = True,
                  deserializable: bool = True,
                  default: typing.Optional[DeserializedType] = None,
-                 override: bool = False,
-                 use_init: bool = False
-                 ):
-        super().__init__(serialization_path=serialization_path,
-                         serializable=serializable,
-                         deserializable=deserializable,
-                         default=default,
-                         override=override,
-                         use_init=use_init
-                         )
+                 override: bool = False):
+        super().__init__(serialization_path,
+                         serializable,
+                         deserializable,
+                         default,
+                         override)
         self.element_type = element_type if isinstance(element_type, Property) else element_type()
 
     @property
     def underlying_types(self):
         return list, set, tuple
 
     @property
@@ -466,27 +398,23 @@
 
 
 class Set(PropertyCollection[set, typing.Iterable]):
 
     def __init__(self,
                  element_type: typing.Union[Property, typing.Type[Property]],
                  serialization_path: typing.Optional[str] = None,
-                 *,
                  serializable: bool = True,
                  deserializable: bool = True,
                  default: typing.Optional[DeserializedType] = None,
-                 override: bool = False,
-                 use_init: bool = False
-                 ):
-        super().__init__(serialization_path=serialization_path,
-                         serializable=serializable,
-                         deserializable=deserializable,
-                         default=default,
-                         override=override,
-                         use_init=use_init)
+                 override: bool = False):
+        super().__init__(serialization_path,
+                         serializable,
+                         deserializable,
+                         default,
+                         override)
         self.element_type = element_type if isinstance(element_type, Property) else element_type()
 
     @property
     def underlying_types(self):
         return set, list, tuple
 
     @property
@@ -527,27 +455,23 @@
 
     Attempted de/serialization is done in the order in which types are provided in the constructor.
     """
 
     def __init__(self,
                  element_types: typing.Sequence[typing.Union[Property, typing.Type[Property]]],
                  serialization_path: typing.Optional[str] = None,
-                 *,
                  serializable: bool = True,
                  deserializable: bool = True,
                  default: typing.Optional[DeserializedType] = None,
-                 override: bool = False,
-                 use_init: bool = False
-                 ):
-        super().__init__(serialization_path=serialization_path,
-                         serializable=serializable,
-                         deserializable=deserializable,
-                         default=default,
-                         override=override,
-                         use_init=use_init)
+                 override: bool = False):
+        super().__init__(serialization_path,
+                         serializable,
+                         deserializable,
+                         default,
+                         override)
         if not isinstance(element_types, typing.Iterable):
             raise ValueError("element types must be iterable: {}".format(element_types))
         self.element_types: typing.List[Property, ...] = \
             [el if isinstance(el, Property) else el() for el in element_types]
 
     @property
     def underlying_types(self):
@@ -582,27 +506,23 @@
 
 class SpecifiedMixedList(PropertyCollection[list, list]):
     """A finite list in which the type of each entry is specified."""
 
     def __init__(self,
                  element_types: typing.Sequence[typing.Union[Property, typing.Type[Property]]],
                  serialization_path: typing.Optional[str] = None,
-                 *,
                  serializable: bool = True,
                  deserializable: bool = True,
                  default: typing.Optional[DeserializedType] = None,
-                 override: bool = False,
-                 use_init: bool = False
-                 ):
-        super().__init__(serialization_path=serialization_path,
-                         serializable=serializable,
-                         deserializable=deserializable,
-                         default=default,
-                         override=override,
-                         use_init=use_init)
+                 override: bool = False):
+        super().__init__(serialization_path,
+                         serializable,
+                         deserializable,
+                         default,
+                         override)
         if not isinstance(element_types, list):
             raise ValueError("element types must be a list: {}".format(element_types))
         self.element_types: typing.List[Property, ...] = \
             [el if isinstance(el, Property) else el() for el in element_types]
 
     @property
     def underlying_types(self):
@@ -662,75 +582,62 @@
 
 
 class Enumeration(Property[BaseEnumeration, str]):
 
     def __init__(self,
                  klass: typing.Type[typing.Any],
                  serialization_path: typing.Optional[str] = None,
-                 *,
                  serializable: bool = True,
                  deserializable: bool = True,
                  default: typing.Optional[DeserializedType] = None,
-                 override: bool = False,
-                 use_init: bool = False
-                 ):
-        super().__init__(serialization_path=serialization_path,
-                         serializable=serializable,
-                         deserializable=deserializable,
-                         default=default,
-                         override=override,
-                         use_init=use_init)
+                 override: bool = False):
+        super().__init__(serialization_path,
+                         serializable,
+                         deserializable,
+                         default,
+                         override)
         self.klass = klass
 
     @property
     def underlying_types(self):
         return self.klass
 
     @property
     def serialized_types(self):
         return str
 
-    def _deserialize(self, value: str) -> BaseEnumeration:
-        return self.klass.from_str(value, exception=True)
+    def _deserialize(self, value: str) -> uuid.UUID:
+        return self.klass.get_enum(value)
 
     def _serialize(self, value: typing.Any) -> str:
-        return self.klass.from_str(value, exception=True).value
-
-
-@lru_cache(maxsize=1024)
-def _fields_map(klass: typing.Type) -> typing.Dict[str, Property]:
-    """Compute the properties-relevant fields in a given class."""
-    return {
-        k: v
-        for x in reversed(klass.__mro__)  # Classes at the front trump
-        for k, v in x.__dict__.items() if isinstance(v, Property)
-    }
+        return self.klass.get_value(value)
 
 
 class Object(PropertyCollection[typing.Any, dict]):
 
     def __init__(self,
                  klass: typing.Type[typing.Any],
                  serialization_path: typing.Optional[str] = None,
-                 *,
                  serializable: bool = True,
                  deserializable: bool = True,
                  default: typing.Optional[DeserializedType] = None,
-                 override: bool = False,
-                 use_init: bool = False
-                 ):
-        super().__init__(serialization_path=serialization_path,
-                         serializable=serializable,
-                         deserializable=deserializable,
-                         default=default,
-                         override=override,
-                         use_init=use_init)
+                 override: bool = False):
+        super().__init__(serialization_path,
+                         serializable,
+                         deserializable,
+                         default,
+                         override)
         self.klass = klass
         # We need to use __dict__ here because other access methods will invoke __get__
-        self.fields: typing.Dict[str, Property] = _fields_map(self.klass)
+        # Start with the fields from the parent classes, overwriting with any newer classes
+        self.fields = {k: v
+                       for x in self.klass.__bases__
+                       for k, v in x.__dict__.items() if isinstance(v, Property)}
+        self.fields.update(
+            {k: v for k, v in self.klass.__dict__.items() if isinstance(v, Property)})
         self.polymorphic = "get_type" in self.klass.__dict__ and\
                            issubclass(self.klass, PolymorphicSerializable)
 
     @property
     def underlying_types(self):
         return self.klass
 
@@ -744,45 +651,19 @@
         if not self.fields:
             # Maybe there are no fields because we hit a gemd-python class
             if issubclass(self.klass, DictSerializable):
                 return DictSerializable.build(data)
             raise AttributeError("Tried to deserialize to {!r}, which has no fields and is not an"
                                  " explicitly serializable class".format(self.klass))
 
-        values = {}
-        init_props = set()
+        instance = self.klass.__new__(self.klass, {})
         for property_name, field in self.fields.items():
-            if field.use_init:
-                init_props.add(property_name)
             if field.deserializable:
-                values[property_name] = field.deserialize_from_dict(data)
-            elif field.default is not None:
-                values[property_name] = field.default
-
-        if len(init_props) > 0:
-            try:
-                instance = self.klass(**{k: v for k, v in values.items() if k in init_props})
-            except TypeError as e:
-                # Check if it's because the signature was wrong
-                sig = signature(self.klass.__init__)
-                for arg, param in sig.parameters.items():
-                    if arg not in init_props | {'self'}:
-                        if param.default is param.empty:
-                            raise AttributeError(
-                                f"{self.klass} has at least 1 property marked as `use_init`, "
-                                f"but required arguments weren't: {e}"
-                            )
-                else:
-                    raise e
-        else:
-            instance = self.klass.__new__(self.klass)
-        for property_name in values:
-            if property_name not in init_props:
-                setattr(instance, property_name, values[property_name])
-
+                value = field.deserialize_from_dict(data)
+                setattr(instance, property_name, value)
         return instance
 
     def _serialize(self, obj: typing.Any) -> dict:
         serialized = {}
         if type(obj) != self.klass and isinstance(obj, Serializable):
             # If the object class doesn't match this one, then it is a subclass
             # that may have more fields, so defer to them by calling the dump method
@@ -822,95 +703,74 @@
     Serialization is done by converting the object to a dict. If it is a Serializable object
     it has a dump() method. LinkByUID has the as_dict() method.
 
     Deserialization to a LinkByUID is easy--it is constructed using value. Deserialization to
     a Serializable object is more difficult because this class does not know what object it is
     supposed to deserialize to (passing that information results in a circular import, because the
     objects that need to be deserialized in this use case have their own Property serde schema).
-    Instead, we rely on the fact that all the Serializable classes with serde schema
+    Instead, we rely on the fact that all of the Serializable classes with serde schema
     (data concepts objects, templates, etc.) know how to deserialize themselves through a
     build() method that doesn't call _deserialize().
 
     This is currently tied to LinkByUID in gemd, but could be modified to work with a
     generic Link object.
     """
 
     def __init__(self,
-                 klass: typing.Type[typing.Any] = Serializable,
                  serialization_path: typing.Optional[str] = None,
-                 *,
                  serializable: bool = True,
                  deserializable: bool = True,
                  default: typing.Optional[DeserializedType] = None,
-                 override: bool = False,
-                 use_init: bool = False
-                 ):
-        super().__init__(
-            serialization_path=serialization_path,
-            serializable=serializable,
-            deserializable=deserializable,
-            default=default,
-            override=override,
-            use_init=use_init)
-        self.klass = klass
+                 override: bool = False):
+        super().__init__(serialization_path, serializable, deserializable, default, override)
 
     @property
     def underlying_types(self):
-        return self.klass, LinkByUID
+        return Serializable, LinkByUID
 
     @property
     def serialized_types(self):
         return dict
 
     def _serialize(self, value: typing.Any) -> dict:
         if isinstance(value, LinkByUID):
             return value.as_dict()
         elif isinstance(value, Serializable):
             return value.dump()
 
     def _deserialize(self, value: dict):
-        if 'type' in value:
-            target = DictSerializable.class_mapping[value['type']]
-            try:
-                return target.build(value)
-            except TypeError as e:
-                # TODO: Consider migrating this ValueError to a TypeError for 3
-                match = re.search(r"__init__.* missing (\d+) required \w+ arguments: (.+)", str(e))
-                if match:
-                    raise ValueError(
-                        f"{match.group(1)} missing required "
-                        f"field{'s' if match.group(1) != '1' else ''}: {match.group(2)}"
-                    )
-                else:
-                    raise e
+        if 'type' in value and value['type'] == LinkByUID.typ:
+            if 'scope' in value and 'id' in value:
+                value.pop('type')
+                return LinkByUID(**value)
+            else:
+                raise ValueError("LinkByUID dictionary must have both scope and id fields")
+
         raise Exception("Serializable object that is being pointed to must have a self-contained "
                         "build() method that does not call deserialize().")
 
     def _set_elements(self, value):
         return value
 
 
 class Optional(PropertyCollection[typing.Optional[typing.Any], typing.Optional[typing.Any]]):
 
     def __init__(self,
                  prop: typing.Union[Property, typing.Type[Property]],
                  serialization_path: typing.Optional[str] = None,
-                 *,
                  serializable: bool = True,
                  deserializable: bool = True,
                  default: typing.Optional[DeserializedType] = None,
-                 override: bool = False,
-                 use_init: bool = False
+                 override: bool = False
                  ):
-        super().__init__(serialization_path=serialization_path,
-                         serializable=serializable,
-                         deserializable=deserializable,
-                         default=default,
-                         override=override,
-                         use_init=use_init)
+        super().__init__(serialization_path,
+                         serializable,
+                         deserializable,
+                         default,
+                         override)
         self.prop = prop if isinstance(prop, Property) else prop()
         self.optional = True
 
     @property
     def underlying_types(self):
         constituent_types = self.prop.underlying_types
         if isinstance(constituent_types, tuple):
@@ -957,28 +817,24 @@
     key value pairs and converts them to a dict.
     """
 
     def __init__(self,
                  keys_type: typing.Union[Property, typing.Type[Property]],
                  values_type: typing.Union[Property, typing.Type[Property]],
                  serialization_path: typing.Optional[str] = None,
-                 *,
                  serializable: bool = True,
                  deserializable: bool = True,
                  default: typing.Optional[dict] = None,
                  override: bool = False,
-                 use_init: bool = False,
                  ser_as_list_of_pairs: bool = False):
-        super().__init__(serialization_path=serialization_path,
-                         serializable=serializable,
-                         deserializable=deserializable,
-                         default=default,
-                         override=override,
-                         use_init=use_init
-                         )
+        super().__init__(serialization_path,
+                         serializable,
+                         deserializable,
+                         default,
+                         override)
 
         self.keys_type = keys_type if isinstance(keys_type, Property) else keys_type()
         self.values_type = values_type if isinstance(values_type, Property) else values_type()
         self.ser_as_list_of_pairs = ser_as_list_of_pairs
 
     @property
     def underlying_types(self):
```

### Comparing `citrine-2.24.1/src/citrine/_serialization/serializable.py` & `citrine-2.8.0/src/citrine/_serialization/serializable.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/_session.py` & `citrine-2.8.0/src/citrine/_session.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/_utils/batcher.py` & `citrine-2.8.0/src/citrine/_utils/batcher.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/_utils/template_util.py` & `citrine-2.8.0/src/citrine/_utils/template_util.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/builders/auto_configure.py` & `citrine-2.8.0/src/citrine/builders/auto_configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from citrine.informatics.predictor_evaluator import PredictorEvaluator
 from citrine.informatics.objectives import Objective
 from citrine.informatics.scores import Score
 from citrine.informatics.workflows import DesignWorkflow, PredictorEvaluationWorkflow
 
 from citrine.resources.gemtables import GemTable
 from citrine.resources.material_run import MaterialRun
-from citrine.resources.predictor import GraphPredictor, AutoConfigureMode
+from citrine.resources.predictor import Predictor, AutoConfigureMode
 from citrine.resources.project import Project
 from citrine.resources.table_config import TableConfig, TableBuildAlgorithm
 
 from citrine.builders.scores import create_default_score
 
 logger = getLogger(__name__)
 
@@ -166,15 +166,15 @@
 
     @property
     def table(self) -> Optional[GemTable]:
         """Get the GEM table associated with this workflow."""
         return self._table
 
     @property
-    def predictor(self) -> Optional[GraphPredictor]:
+    def predictor(self) -> Optional[Predictor]:
         """Get the predictor associated with this workflow."""
         return self._predictor
 
     @property
     def predictor_evaluation_workflow(self) -> Optional[PredictorEvaluationWorkflow]:
         """Get the predictor evaluation workflow associated with this workflow."""
         return self._predictor_evaluation_workflow
@@ -493,15 +493,15 @@
             predictor=predictor, score=score, evaluator=evaluator,
             design_space=design_space, print_status_info=print_status_info
         )
 
     def from_predictor(
             self,
             *,
-            predictor: GraphPredictor,
+            predictor: Predictor,
             evaluator: Optional[PredictorEvaluator] = None,
             design_space: Optional[DesignSpace] = None,
             score: Optional[Union[Score, Objective]] = None,
             print_status_info: bool = False
     ):
         """[ALPHA] Auto configure platform assets from predictor to design workflow.
 
@@ -593,15 +593,15 @@
         self._table_config = table_config
         self._table = self.project.tables.build_from_config(self.table_config)
         self._status = AutoConfigureStatus.TABLE_CREATED
 
     def _predictor_registration_stage(
             self,
             *,
-            predictor: GraphPredictor,
+            predictor: Predictor,
             print_status_info: bool
     ):
         """Register and validate a provided predictor."""
         self._print_status("Configuring predictor...")
 
         predictor.name = self._default_asset_names["PREDICTOR"]
         predictor = create_or_update(
@@ -622,15 +622,15 @@
             self._status = AutoConfigureStatus.PREDICTOR_INVALID
             raise RuntimeError("Predictor is invalid,"
                                " cannot proceed to design space configuration.")
 
     def _predictor_evaluation_stage(
             self,
             *,
-            predictor: GraphPredictor,
+            predictor: Predictor,
             evaluator: Optional[PredictorEvaluator],
             print_status_info: bool
     ):
         """Evaluate the predictor with the specified evaluator, or create a default workflow."""
         self._print_status("Configuring predictor evaluation...")
 
         if evaluator is None:
@@ -668,15 +668,15 @@
         elif evaluator is not None:
             # Manually trigger execution
             pew.executions.trigger(predictor.uid)
 
     def _design_space_build_stage(
             self,
             *,
-            predictor: GraphPredictor,
+            predictor: Predictor,
             design_space: Optional[DesignSpace],
             print_status_info: bool
     ):
         """Create a design space from a specified predictor, or use the provided one."""
         self._print_status("Configuring design space...")
 
         if design_space is None:
@@ -700,15 +700,15 @@
             self._status = AutoConfigureStatus.DESIGN_SPACE_INVALID
             raise RuntimeError("Design space is invalid,"
                                " cannot proceed to design workflow configuration.")
 
     def _design_workflow_build_stage(
             self,
             *,
-            predictor: GraphPredictor,
+            predictor: Predictor,
             design_space: DesignSpace,
             score: Optional[Union[Score, Objective]],
             print_status_info: bool
     ):
         """Create a design workflow, and optionally trigger a design execution."""
         self._print_status("Configuring design workflow...")
```

### Comparing `citrine-2.24.1/src/citrine/builders/descriptors.py` & `citrine-2.8.0/src/citrine/builders/descriptors.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/builders/design_spaces.py` & `citrine-2.8.0/src/citrine/builders/design_spaces.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/builders/predictors.py` & `citrine-2.8.0/src/citrine/builders/predictors.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/builders/scores.py` & `citrine-2.8.0/src/citrine/builders/scores.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/citrine.py` & `citrine-2.8.0/src/citrine/citrine.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/gemtables/columns.py` & `citrine-2.8.0/src/citrine/gemtables/columns.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/gemtables/rows.py` & `citrine-2.8.0/src/citrine/gemtables/rows.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/gemtables/variables.py` & `citrine-2.8.0/src/citrine/gemtables/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -568,16 +568,17 @@
         self.name = name
         self.headers = headers
         self.process_template = _make_link_by_uid(process_template)
         self.ingredient_name = ingredient_name
         self.type_selector = type_selector
 
         # Cast to make sure the string is valid
-        self.quantity_dimension = IngredientQuantityDimension.from_str(quantity_dimension,
-                                                                       exception=True)
+        if not isinstance(quantity_dimension, IngredientQuantityDimension):
+            quantity_dimension = IngredientQuantityDimension.get_enum(quantity_dimension)
+        self.quantity_dimension = quantity_dimension
 
         if quantity_dimension == IngredientQuantityDimension.ABSOLUTE:
             if unit is None:
                 raise ValueError("Absolute Quantity variables require that 'unit' is set")
         else:
             if unit is not None and unit != "":
                 raise ValueError("Fractional variables cannot take a 'unit'")
@@ -922,16 +923,17 @@
         self.name = name
         self.headers = headers
         self.ingredient_name = ingredient_name
         self.process_templates = [_make_link_by_uid(x) for x in process_templates]
         self.type_selector = type_selector
 
         # Cast to make sure the string is valid
-        self.quantity_dimension = IngredientQuantityDimension.from_str(quantity_dimension,
-                                                                       exception=True)
+        if not isinstance(quantity_dimension, IngredientQuantityDimension):
+            quantity_dimension = IngredientQuantityDimension.get_enum(quantity_dimension)
+        self.quantity_dimension = quantity_dimension
 
         if quantity_dimension == IngredientQuantityDimension.ABSOLUTE:
             if unit is None:
                 raise ValueError("Absolute Quantity variables require that 'unit' is set")
         else:
             if unit is not None and unit != "":
                 raise ValueError("Fractional variables cannot take a 'unit'")
@@ -1080,16 +1082,17 @@
                  unit: Optional[str] = None):
         self.name = name
         self.headers = headers
         self.ingredient_name = ingredient_name
         self.type_selector = type_selector
 
         # Cast to make sure the string is valid
-        self.quantity_dimension = IngredientQuantityDimension.from_str(quantity_dimension,
-                                                                       exception=True)
+        if not isinstance(quantity_dimension, IngredientQuantityDimension):
+            quantity_dimension = IngredientQuantityDimension.get_enum(quantity_dimension)
+        self.quantity_dimension = quantity_dimension
 
         if quantity_dimension == IngredientQuantityDimension.ABSOLUTE:
             if unit is None:
                 raise ValueError("Absolute Quantity variables require that 'unit' is set")
         else:
             if unit is not None and unit != "":
                 raise ValueError("Fractional variables cannot take a 'unit'")
```

### Comparing `citrine-2.24.1/src/citrine/informatics/constraints/categorical_constraint.py` & `citrine-2.8.0/src/citrine/informatics/constraints/categorical_constraint.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/constraints/constraint.py` & `citrine-2.8.0/src/citrine/informatics/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/constraints/ingredient_count_constraint.py` & `citrine-2.8.0/src/citrine/informatics/constraints/ingredient_count_constraint.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,8 +39,8 @@
                  label: Optional[str] = None):
         self.formulation_descriptor: FormulationDescriptor = formulation_descriptor
         self.min: int = min
         self.max: int = max
         self.label: Optional[str] = label
 
     def __str__(self):
-        return f"<IngredientCountConstraint '{self.formulation_descriptor.key}'>"
+        return '<IngredientCountConstraint {!r}>'.format(self.formulation_descriptor.key)
```

### Comparing `citrine-2.24.1/src/citrine/informatics/constraints/ingredient_fraction_constraint.py` & `citrine-2.8.0/src/citrine/informatics/constraints/ingredient_fraction_constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,11 +43,11 @@
         self.formulation_descriptor: FormulationDescriptor = formulation_descriptor
         self.ingredient: str = ingredient
         self.min: float = min
         self.max: float = max
         self.is_required: bool = is_required
 
     def __str__(self):
-        return (
-            f"<IngredientFractionConstraint "
-            f"'{self.formulation_descriptor.key}'::'{self.ingredient}'>"
+        return '<IngredientFractionConstraint {!r}::{!r}>'.format(
+            self.formulation_descriptor.key,
+            self.ingredient
         )
```

### Comparing `citrine-2.24.1/src/citrine/informatics/constraints/ingredient_ratio_constraint.py` & `citrine-2.8.0/src/citrine/resources/design_workflow.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,174 +1,171 @@
-import warnings
-from typing import Set, Mapping, Optional, Tuple, Union
-
-from citrine._serialization import properties
-from citrine._serialization.serializable import Serializable
-from citrine.informatics.constraints.constraint import Constraint
-from citrine.informatics.descriptors import FormulationDescriptor
-
-__all__ = ['IngredientRatioConstraint']
-
-
-class IngredientRatioConstraint(Serializable['IngredientRatioConstraint'], Constraint):
-    """A formulation constraint operating on the ratio of quantities of ingredients and a basis.
-
-    Example: "6 to 7 parts ingredient A per 100 parts ingredient B" becomes
-    .. code:: python
-        IngredientRatioConstraint(min=6, max=7, ingredient=("A", 100), basis_ingredients=["B"])
-
-    Parameters
-    ----------
-    formulation_descriptor: FormulationDescriptor
-        descriptor to constrain
-    min: float
-        minimum value for the ratio
-    max: float
-        maximum value for the ratio
-    ingredient: Optional[tuple[str, float]]
-        multiplier for an ingredient in the numerator of the ratio
-    label: Optional[tuple[str, float]]
-        multiplier for a label in the numerator of the ratio
-    basis_ingredients: Optional[Union[list[str], dict[str, float]]]
-        the ingredients which should appear in the denominator of the ratio
-    basis_labels: Optional[Union[list[str], dict[str, float]]]
-        the labels which should appear in the denominator of the ratio
-
-    """
-
-    formulation_descriptor = properties.Object(FormulationDescriptor, 'formulation_descriptor')
-    min = properties.Float('min')
-    max = properties.Float('max')
-
-    # The backend provides ingredients and labels as dictionaries, but presently only allows one
-    # between them. To clarify customer interaction, we only allow a single one of each to be set.
-    # Since our serde library doesn't allow extracting from a dict with unknown keys, we do it by
-    # hiding the dictionaries and exposing properties.
-    _ingredients = properties.Mapping(
-        properties.String, properties.Float, 'ingredients', default={})
-    _labels = properties.Mapping(properties.String, properties.Float, 'labels', default={})
-
-    # The backend provides basis ingredients and basis labels as a dictionary from the key to a
-    # multiplier. However, for ingredient ratio constraints, the multiplier in the denominator
-    # should always be one, so we can't allow users to enter it. We need to use properties for this
-    # behavior. It also allows us to display deprecation warnings for the coming type change.
-    _basis_ingredients = properties.Mapping(
-        properties.String, properties.Float, 'basis_ingredients', default={})
-    _basis_labels = properties.Mapping(
-        properties.String, properties.Float, 'basis_labels', default={})
-
-    typ = properties.String('type', default='IngredientRatio')
-
-    def __init__(self, *,
-                 formulation_descriptor: FormulationDescriptor,
-                 min: float,
-                 max: float,
-                 ingredient: Optional[Tuple[str, float]] = None,
-                 label: Optional[Tuple[str, float]] = None,
-                 basis_ingredients: Union[Set[str], Mapping[str, float]] = set(),
-                 basis_labels: Union[Set[str], Mapping[str, float]] = set()):
-        self.formulation_descriptor = formulation_descriptor
-        self.min = min
-        self.max = max
-        self.ingredient = ingredient
-        self.label = label
-        self.basis_ingredients = basis_ingredients
-        self.basis_labels = basis_labels
-
-    @property
-    def ingredient(self):
-        """Retrieve the ingredient and its multiplier from the numerator, if it's been set."""
-        return self._numerator_read(self._ingredients)
-
-    @ingredient.setter
-    def ingredient(self, value: Optional[Tuple[str, float]]):
-        """Set the ingredient and its multiplier in the numerator."""
-        self._ingredients = self._numerator_validate(value, "Ingredient")
-
-    @property
-    def label(self):
-        """Retrieve the label and its multiplier from the numerator, if it's been set."""
-        return self._numerator_read(self._labels)
-
-    @label.setter
-    def label(self, value: Optional[Tuple[str, float]]):
-        """Set the label and its multiplier in the numerator."""
-        self._labels = self._numerator_validate(value, "Label")
-
-    @property
-    def basis_ingredients(self) -> Mapping[str, float]:
-        """Retrieve the ingredients in the denominator of the ratio."""
-        warnings.warn("basis_ingredients is deprecated as of 2.13.0 and will change in 3.0. "
-                      "Please use basis_ingredient_names instead.", DeprecationWarning)
-        return self._basis_ingredients
-
-    @basis_ingredients.setter
-    def basis_ingredients(self, value: Union[Set[str], Mapping[str, float]]):
-        """Set the ingredients in the denominator of the ratio."""
-        if isinstance(value, dict):
-            warnings.warn("As of version 2.13.0, multipliers for all basis ingredients are "
-                          "ignored, so basis_ingredients should be a list of ingredient names.",
-                          DeprecationWarning)
-            value = set(value.keys())
-
-        self.basis_ingredient_names = value
-
-    @property
-    def basis_ingredient_names(self) -> Set[str]:
-        """Retrieve the names of all ingredients in the denominator of the ratio."""
-        return set(self._basis_ingredients.keys())
-
-    # This is for symmetry; it's not strictly necessary.
-    @basis_ingredient_names.setter
-    def basis_ingredient_names(self, value: Set[str]):
-        """Set the names of all ingredients in the denominator of the ratio."""
-        self._basis_ingredients = dict.fromkeys(value, 1)
-
-    @property
-    def basis_labels(self) -> Mapping[str, float]:
-        """Retrieve the labels in the denominator of the ratio."""
-        warnings.warn("basis_labels is deprecated as of 2.13.0 and will change in 3.0. Please use "
-                      "basis_label_names instead.", DeprecationWarning)
-        return self._basis_labels
-
-    @basis_labels.setter
-    def basis_labels(self, value: Union[Set[str], Mapping[str, float]]):
-        """Set the labels in the denominator of the ratio."""
-        if isinstance(value, dict):
-            warnings.warn("As of version 2.13.0, multipliers for all basis labels are ignored, so "
-                          "basis_labels should be a list of label names.", DeprecationWarning)
-            value = set(value.keys())
-
-        self.basis_label_names = value
-
-    @property
-    def basis_label_names(self) -> Set[str]:
-        """Retrieve the names of all labels in the denominator of the ratio."""
-        return set(self._basis_labels.keys())
-
-    # This is for symmetry; it's not strictly necessary.
-    @basis_label_names.setter
-    def basis_label_names(self, value: Set[str]):
-        """Set the names of all labels in the denominator of the ratio."""
-        self._basis_labels = dict.fromkeys(value, 1)
-
-    def _numerator_read(self, num_dict):
-        if num_dict:
-            return tuple(num_dict.items())[0]
+from copy import deepcopy
+from typing import Callable, Union, Iterable, Optional, Tuple
+from uuid import UUID
+
+from citrine._rest.collection import Collection
+from citrine._session import Session
+from citrine._utils.functions import format_escaped_url
+from citrine.informatics.workflows import DesignWorkflow
+from citrine.resources.response import Response
+from functools import partial
+
+
+class DesignWorkflowCollection(Collection[DesignWorkflow]):
+    """A collection of DesignWorkflows."""
+
+    _path_template = '/projects/{project_id}/design-workflows'
+    _individual_key = None
+    _collection_key = 'response'
+    _resource = DesignWorkflow
+    _api_version = "v2"
+
+    def __init__(self, project_id: UUID, session: Session, branch_id: UUID = None):
+        self.project_id: UUID = project_id
+        self.session: Session = session
+        self.branch_id: UUID = branch_id
+
+    def register(self, model: DesignWorkflow) -> DesignWorkflow:
+        """
+        Upload a new design workflow.
+
+        The model's branch ID is ignored in favor of this collection's. If this
+        collection has a null branch ID, then a branch is first created, then
+        the design workflow is created on it.
+
+        Parameters
+        ----------
+        model: DesignWorkflow
+            The design workflow to be uploaded.
+
+        Return
+        -------
+        DesignWorkflow
+            The newly created design workflow.
+
+        """
+        if self.branch_id is None:
+            # There are a number of contexts in which hitting design workflow endpoints without a
+            # branch ID is valid, so only this particular usage is deprecated.
+            msg = ('A design workflow must be created with a branch. Please use'
+                   'branch.design_workflows.register() instead of '
+                   'project.design_workflows.register().')
+            raise RuntimeError(msg)
         else:
-            return None
-
-    def _numerator_validate(self, value, input_type):
-        if value:
-            if len(value) != 2:
-                raise ValueError(f"{input_type} must be a name and a multiplier.")
-
-            name, mult = value
-            if mult <= 0.0:
-                raise ValueError(f"{input_type} multipler must be greater than 0.")
-
-            return {name: mult}
-        else:
-            return {}
-
-    def __str__(self):
-        return f"<IngredientRatioConstraint '{self.formulation_descriptor.key}'>"
+            # branch_id is in the body of design workflow endpoints, so it must be serialized.
+            # This means the collection branch_id might not match the workflow branch_id. The
+            # collection should win out, since the user is explicitly referencing the branch
+            # represented by this collection.
+            # To avoid modifying the parameter, and to ensure the only change is the branch_id, we
+            # deepcopy, modify, then register it.
+            model_copy = deepcopy(model)
+            model_copy.branch_id = self.branch_id
+            return super().register(model_copy)
+
+    def build(self, data: dict) -> DesignWorkflow:
+        """
+        Build an individual design workflow from a dictionary.
+
+        Parameters
+        ----------
+        data: dict
+            A dictionary representing the design workflow.
+
+        Return
+        -------
+        DesignWorkflow
+            The design workflow created from data.
+
+        """
+        workflow = DesignWorkflow.build(data)
+        workflow._session = self.session
+        workflow.project_id = self.project_id
+        return workflow
+
+    def update(self, model: DesignWorkflow) -> DesignWorkflow:
+        """Update a design workflow.
+
+        Identifies the workflow by the model's uid. It must have a branch_id, and if this
+        collection also has a branch_id, they must match. Prefer updating a workflow through
+        Project.design_workflows.update.
+
+        Parameters
+        ----------
+        model: DesignWorkflow
+            The design workflow values that are desired, identified by the uid.
+
+        Return
+        -------
+        DesignWorkflow
+            The design workflow resulting from the update.
+
+        """
+        if self.branch_id is not None:
+            if self.branch_id != model.branch_id:
+                raise ValueError('To move a design workflow to another branch, please use '
+                                 'Project.design_workflows.update')
+
+        if model.branch_id is None:
+            raise ValueError('Cannot update a design workflow unless its branch_id is set.')
+
+        # If executions have already been done, warn about future behavior change
+        executions = model.design_executions.list()
+        if next(executions, None) is not None:
+            raise RuntimeError("Cannot update a design workflow after candidate generation, "
+                               "please register a new design workflow instead")
+
+        return super().update(model)
+
+    def archive(self, uid: Union[UUID, str]):
+        """Archive a design workflow.
+
+        Parameters
+        ----------
+        uid: Union[UUID, str]
+            Unique identifier of the workflow to archive
+
+        """
+        url = format_escaped_url(self._path_template, project_id=self.project_id) \
+            + format_escaped_url("/{}/archive", uid)
+        self.session.put_resource(url, {}, version=self._api_version)
+
+    def restore(self, uid: Union[UUID, str]):
+        """Restore an archived design workflow.
+
+        Parameters
+        ----------
+        uid: Union[UUID, str]
+            Unique identifier of the workflow to restore
+
+        """
+        url = format_escaped_url(self._path_template, project_id=self.project_id) \
+            + format_escaped_url("/{}/restore", uid)
+        self.session.put_resource(url, {}, version=self._api_version)
+
+    def delete(self, uid: Union[UUID, str]) -> Response:
+        """Design Workflows cannot be deleted; they can be archived instead."""
+        raise NotImplementedError(
+            "Design Workflows cannot be deleted; they can be archived instead.")
+
+    def list_archived(self, *, per_page: int = 500) -> Iterable[DesignWorkflow]:
+        """List archived Design Workflows."""
+        fetcher = partial(self._fetch_page, additional_params={"filter": "archived eq 'true'"})
+        return self._paginator.paginate(page_fetcher=fetcher,
+                                        collection_builder=self._build_collection_elements,
+                                        per_page=per_page)
+
+    def _fetch_page(self,
+                    path: Optional[str] = None,
+                    fetch_func: Optional[Callable[..., dict]] = None,
+                    page: Optional[int] = None,
+                    per_page: Optional[int] = None,
+                    json_body: Optional[dict] = None,
+                    additional_params: Optional[dict] = None,
+                    ) -> Tuple[Iterable[dict], str]:
+        params = additional_params or {}
+        params["branch"] = self.branch_id
+        return super()._fetch_page(path=path,
+                                   fetch_func=fetch_func,
+                                   page=page,
+                                   per_page=per_page,
+                                   json_body=json_body,
+                                   additional_params=params)
```

### Comparing `citrine-2.24.1/src/citrine/informatics/constraints/label_fraction_constraint.py` & `citrine-2.8.0/src/citrine/informatics/constraints/label_fraction_constraint.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,8 +43,11 @@
         self.formulation_descriptor: FormulationDescriptor = formulation_descriptor
         self.label: str = label
         self.min: float = min
         self.max: float = max
         self.is_required: bool = is_required
 
     def __str__(self):
-        return f"<LabelFractionConstraint '{self.formulation_descriptor.key}'::'{self.label}'>"
+        return '<LabelFractionConstraint {!r}::{!r}>'.format(
+            self.formulation_descriptor.key,
+            self.label
+        )
```

### Comparing `citrine-2.24.1/src/citrine/informatics/constraints/scalar_range_constraint.py` & `citrine-2.8.0/src/citrine/informatics/constraints/scalar_range_constraint.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/data_sources.py` & `citrine-2.8.0/src/citrine/informatics/data_sources.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/descriptors.py` & `citrine-2.8.0/src/citrine/informatics/descriptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,21 +257,23 @@
     """
 
     typ = properties.String(
         'type', default=FormulationKey.HIERARCHICAL.value, deserializable=False
     )
 
     def __init__(self, key: Union[FormulationKey, str]):
-        self.key = FormulationKey.from_str(key, exception=True)
+        if not isinstance(key, FormulationKey):
+            key = FormulationKey.get_enum(key)
+        self.key: str = key.value
 
     def __eq__(self, other):
         return self._equals(other, ["key", "typ"])
 
     def __str__(self):
-        return f"<FormulationDescriptor '{self.key}'>"
+        return "<FormulationDescriptor {!r}>".format(self.key)
 
     def __repr__(self):
         return "FormulationDescriptor(key={})".format(self.key)
 
     @classmethod
     def hierarchical(cls) -> "FormulationDescriptor":
         """The hierarchical formulation descriptor with key 'Formulation'."""
```

### Comparing `citrine-2.24.1/src/citrine/informatics/design_candidate.py` & `citrine-2.8.0/src/citrine/informatics/design_candidate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-from typing import Type, Optional
+from typing import Type
 
 from citrine._serialization import properties
 from citrine._serialization.polymorphic_serializable import PolymorphicSerializable
 from citrine._serialization.serializable import Serializable
 
 
 __all__ = [
     'DesignCandidate',
-    'HierarchicalDesignCandidate',
     'DesignMaterial',
-    'HierarchicalDesignMaterial',
-    'SampleSearchSpaceResultCandidate',
     'DesignVariable',
     'MeanAndStd',
     'TopCategories',
     'Mixture',
     'ChemicalFormula',
     'MolecularStructure',
 ]
@@ -83,22 +80,19 @@
 
     This is a complete list of components with non-zero quantities; there is no
     truncation (but there may be rounding).
     """
 
     quantities = properties.Mapping(properties.String, properties.Float, 'q')
     """:Dict[str, float]: mapping from ingredient identifiers to their quantities"""
-    labels = properties.Mapping(properties.String, properties.Set(properties.String), 'l')
-    """:Dict[str, Set[str]]: mapping from label identifiers to their associated ingredients"""
     typ = properties.String('type', default='M', deserializable=False)
     """:str: polymorphic type code"""
 
-    def __init__(self, *, quantities: dict, labels: Optional[dict] = None):
+    def __init__(self, *, quantities: dict):
         self.quantities = quantities
-        self.labels = labels or {}
         pass  # pragma: no cover
 
 
 class ChemicalFormula(Serializable["ChemicalFormula"], DesignVariable):
     """Chemical formula as a string."""
 
     formula = properties.String('f')
@@ -123,49 +117,24 @@
         self.smiles = smiles
         pass  # pragma: no cover
 
 
 class DesignMaterial(Serializable["DesignMaterial"]):
     """Description of the material that was designed, as a set of DesignVariables."""
 
-    material_id = properties.UUID('identifiers.id')
-    """:UUID: unique internal Citrine id of the material"""
-    identifiers = properties.List(properties.String, 'identifiers.external', default=[])
-    """:List[str]: globally unique identifiers assigned to the material"""
-    process_template = properties.Optional(properties.UUID, 'identifiers.process_template')
-    """:Optional[UUID]: GEMD process template that describes the process to create this material"""
-    material_template = properties.Optional(properties.UUID, 'identifiers.material_template')
-    """:Optional[UUID]: GEMD material template that describes this material"""
     values = properties.Mapping(properties.String, properties.Object(DesignVariable), 'vars')
     """:Dict[str, DesignVariable]: mapping from descriptor keys to the value for this material"""
 
     def __init__(self, *, values: dict):
         self.values = values
         pass
 
 
-class HierarchicalDesignMaterial(Serializable["HierarchicalDesignMaterial"]):
-    """Description of a designed material as a set of connected individual materials.
-
-    A hierarchical material contains a root material, containing identifiers and variables,
-    along any of sub-materials appearing in the history of the root.
-    Connections between the root and sub-materials are contained in the mixtures dictionary
-    that associates each material (by Citrine ID) with the ingredients that comprise it.
-    """
-
-    root = properties.Object(DesignMaterial, 'terminal')
-    """:DesignMaterial: root material containing features and predicted properties"""
-    sub_materials = properties.List(properties.Object(DesignMaterial), 'sub_materials')
-    """:List[DesignMaterial]: all other materials appearing in the history of the root"""
-    mixtures = properties.Mapping(properties.UUID, properties.Object(Mixture), 'mixtures')
-    """:Dict[UUID, Mixture]: mapping from Citrine ID to components the material is composed of"""
-
-
 class DesignCandidate(Serializable["DesignCandidate"]):
-    """A candidate material generated by the Citrine Platform.
+    """A Citrine Predictor Evaluation Result.
 
     This class represents the candidate computed by a design execution.
     """
 
     uid = properties.UUID('id')
     """:UUID: unique external Citrine id of the material"""
     material_id = properties.UUID('material_id')
@@ -174,37 +143,9 @@
     """:List[str]: globally unique identifiers assigned to the material"""
     primary_score = properties.Float('primary_score')
     """:float: numerical score describing how well the candidate satisfies the objectives
     and constraints (higher is better)"""
     material = properties.Object(DesignMaterial, 'material')
     """:DesignMaterial: the material returned by the design workflow"""
 
-
-class HierarchicalDesignCandidate(Serializable["HierarchicalDesignCandidate"]):
-    """A hierarchical candidate material generated by the Citrine Platform.
-
-    This class represents the candidate computed by a design execution.
-    """
-
-    uid = properties.UUID('id')
-    """:UUID: unique external Citrine ID of the material"""
-    primary_score = properties.Float('primary_score')
-    """:float: numerical score describing how well the candidate satisfies the objectives
-    and constraints (higher is better)"""
-    rank = properties.Integer("rank")
-    """:int: rank by score amongst other candidates produced by the design workflow"""
-    material = properties.Object(HierarchicalDesignMaterial, "material")
-    """:HierarchicalDesignMaterial: the material returned by the design workflow"""
-
-
-class SampleSearchSpaceResultCandidate(Serializable["SampleSearchSpaceResultCandidate"]):
-    """A hierarchical candidate material generated by the Citrine Platform.
-
-    This class represents the candidate computed by a design execution.
-    """
-
-    uid = properties.UUID('id')
-    """:UUID: unique external Citrine ID of the material"""
-    execution_uid = properties.UUID('id')
-    """:UUID: unique external Citrine ID of the execution"""
-    material = properties.Object(HierarchicalDesignMaterial, "material")
-    """:HierarchicalDesignMaterial: the material returned by the design workflow"""
+    def __init__(self):
+        pass  # pragma: no cover
```

### Comparing `citrine-2.24.1/src/citrine/informatics/design_spaces/data_source_design_space.py` & `citrine-2.8.0/src/citrine/informatics/design_spaces/data_source_design_space.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/design_spaces/enumerated_design_space.py` & `citrine-2.8.0/src/citrine/informatics/design_spaces/enumerated_design_space.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/design_spaces/formulation_design_space.py` & `citrine-2.8.0/src/citrine/informatics/design_spaces/formulation_design_space.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/design_spaces/product_design_space.py` & `citrine-2.8.0/src/citrine/informatics/design_spaces/product_design_space.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List, Union, Optional
 from uuid import UUID
+from copy import deepcopy
 
 from citrine._rest.resource import Resource, ResourceTypeEnum
 from citrine._serialization import properties
 from citrine.informatics.design_spaces.design_space import DesignSpace
 from citrine.informatics.dimensions import Dimension
 from citrine._rest.ai_resource_metadata import AIResourceMetadata
 
@@ -50,14 +51,23 @@
                  subspaces: Optional[List[Union[UUID, DesignSpace]]] = None,
                  dimensions: Optional[List[Dimension]] = None):
         self.name: str = name
         self.description: str = description
         self.subspaces: List[Union[UUID, DesignSpace]] = subspaces or []
         self.dimensions: List[Dimension] = dimensions or []
 
+    def dump(self) -> dict:
+        """Override dump to replace on-platform subspaces with their uids."""
+        model_copy = deepcopy(self)
+        for i, subspace in enumerate(model_copy.subspaces):
+            if isinstance(subspace, DesignSpace) and subspace.uid is not None:
+                model_copy.subspaces[i] = subspace.uid
+        serialized = properties.Object(ProductDesignSpace).serialize(model_copy)
+        return self._post_dump(serialized)
+
     def _post_dump(self, data: dict) -> dict:
         data['display_name'] = data['config']['name']
         for i, subspace in enumerate(data['config']['subspaces']):
             if isinstance(subspace, dict):
                 # embedded design spaces are not modules, so only serialize their config
                 data['config']['subspaces'][i] = subspace['config']
         return data
```

### Comparing `citrine-2.24.1/src/citrine/informatics/dimensions.py` & `citrine-2.8.0/src/citrine/informatics/dimensions.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/executions/predictor_evaluation_execution.py` & `citrine-2.8.0/src/citrine/informatics/workflows/design_workflow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,64 @@
-from functools import lru_cache
+from typing import Optional, Union
+from uuid import UUID
 
-from citrine._serialization import properties
-from citrine._utils.functions import format_escaped_url
-from citrine.informatics.predictor_evaluation_result import PredictorEvaluationResult
-from citrine.informatics.executions.execution import Execution
 from citrine._rest.resource import Resource
-
-
-class PredictorEvaluationExecution(Resource['PredictorEvaluationExecution'], Execution):
-    """The execution of a PredictorEvaluationWorkflow.
-
-    Possible statuses are INPROGRESS, SUCCEEDED, and FAILED.
-    Predictor evaluation executions also have a ``status_description`` field with more information.
+from citrine._serialization import properties
+from citrine.informatics.workflows.workflow import Workflow
+from citrine.resources.design_execution import DesignExecutionCollection
+from citrine._rest.ai_resource_metadata import AIResourceMetadata
+
+__all__ = ['DesignWorkflow']
+
+
+class DesignWorkflow(Resource['DesignWorkflow'], Workflow, AIResourceMetadata):
+    """Object that generates scored materials that may approach higher values of the score.
+
+    Parameters
+    ----------
+    name: str
+        the name of the workflow
+    design_space_id: Optional[UUID]
+        the UUID corresponding to the design space to use
+    predictor_id: Optional[UUID]
+        the UUID corresponding to the predictor to use
+    predictor_version: Optional[Union[int, str]]
+        the version of the predictor to use
+    description: Optional[str]
+        a description of the workflow
 
     """
 
-    evaluator_names = properties.List(properties.String, "evaluator_names", serializable=False)
-    """:List[str]: names of the predictor evaluators that were executed. These are used
-    when calling the ``results()`` method."""
-    workflow_id = properties.UUID('workflow_id', serializable=False)
-    """:UUID: Unique identifier of the workflow that was executed"""
-    predictor_id = properties.UUID('predictor_id', serializable=False)
-    predictor_version = properties.Integer('predictor_version', serializable=False)
-
-    def _path(self):
-        return format_escaped_url(
-            '/projects/{project_id}/predictor-evaluation-executions/{execution_id}',
-            project_id=self.project_id,
-            execution_id=self.uid
-        )
-
-    @lru_cache()
-    def results(self, evaluator_name: str) -> PredictorEvaluationResult:
-        """
-        Get a specific evaluation result by the name of the evaluator that produced it.
-
-        Parameters
-        ----------
-        evaluator_name: str
-            Name of the evaluator for which to get the results
-
-        Returns
-        -------
-        PredictorEvaluationResult
-            The evaluation result from the evaluator with the given name
-
-        """
-        params = {"evaluator_name": evaluator_name}
-        resource = self._session.get_resource(self._path() + "/results", params=params)
-        return PredictorEvaluationResult.build(resource)
-
-    def __getitem__(self, item):
-        if isinstance(item, str):
-            return self.results(item)
-        else:
-            raise TypeError("Results are accessed by string names")
-
-    def __iter__(self):
-        return iter(self.evaluator_names)
+    design_space_id = properties.Optional(properties.UUID, 'design_space_id')
+    predictor_id = properties.Optional(properties.UUID, 'predictor_id')
+    predictor_version = properties.Optional(
+        properties.Union([properties.Integer(), properties.String()]), 'predictor_version')
+    branch_id: Optional[UUID] = properties.Optional(properties.UUID, 'branch_id')
+    """:Optional[UUID]: Unique ID of the branch that contains this workflow."""
+
+    status_description = properties.String('status_description', serializable=False)
+    """:str: more detailed description of the workflow's status"""
+    typ = properties.String('type', default='DesignWorkflow', deserializable=False)
+
+    def __init__(self,
+                 name: str,
+                 *,
+                 design_space_id: Optional[UUID] = None,
+                 predictor_id: Optional[UUID] = None,
+                 predictor_version: Optional[Union[int, str]] = None,
+                 description: Optional[str] = None):
+        self.name = name
+        self.design_space_id = design_space_id
+        self.predictor_id = predictor_id
+        self.predictor_version = predictor_version
+        self.description = description
+
+    def __str__(self):
+        return '<DesignWorkflow {!r}>'.format(self.name)
+
+    @property
+    def design_executions(self) -> DesignExecutionCollection:
+        """Return a resource representing all visible executions of this workflow."""
+        if getattr(self, 'project_id', None) is None:
+            raise AttributeError('Cannot initialize execution without project reference!')
+        return DesignExecutionCollection(
+            project_id=self.project_id, session=self._session, workflow_id=self.uid)
```

### Comparing `citrine-2.24.1/src/citrine/informatics/experiment_values.py` & `citrine-2.8.0/src/citrine/informatics/experiment_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     def get_type(cls, data) -> Type[Serializable]:
         """Return the subtype."""
         return {
             "RealValue": RealExperimentValue,
             "IntegerValue": IntegerExperimentValue,
             "CategoricalValue": CategoricalExperimentValue,
             "MixtureValue": MixtureExperimentValue,
-            "InorganicValue": ChemicalFormulaExperimentValue,
-            "OrganicValue": MolecularStructureExperimentValue,
+            "OrganicValue": ChemicalFormulaExperimentValue,
+            "InorganicValue": MolecularStructureExperimentValue,
         }[data["type"]]
 
     def __str__(self):
         return f"<{self.__class__.__name__} {self.value!r}>"
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.value})"
@@ -109,22 +109,22 @@
 
 
 class ChemicalFormulaExperimentValue(Serializable['ChemicalFormulaExperimentValue'],
                                      ExperimentValue):
     """Experiment value for a chemical formula."""
 
     value = properties.String('value')
-    typ = properties.String('type', default='InorganicValue', deserializable=False)
+    typ = properties.String('type', default='OrganicValue', deserializable=False)
 
     def __init__(self, value: str):
         self.value = value
 
 
 class MolecularStructureExperimentValue(Serializable['MolecularStructureExperimentValue'],
                                         ExperimentValue):
     """Experiment value for a molecular structure."""
 
     value = properties.String('value')
-    typ = properties.String('type', default='OrganicValue', deserializable=False)
+    typ = properties.String('type', default='InorganicValue', deserializable=False)
 
     def __init__(self, value: str):
         self.value = value
```

### Comparing `citrine-2.24.1/src/citrine/informatics/modules.py` & `citrine-2.8.0/src/citrine/informatics/modules.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/objectives.py` & `citrine-2.8.0/src/citrine/informatics/objectives.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/predict_request.py` & `citrine-2.8.0/src/citrine/informatics/predict_request.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/predictor_evaluation_metrics.py` & `citrine-2.8.0/src/citrine/informatics/predictor_evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/predictor_evaluation_result.py` & `citrine-2.8.0/src/citrine/informatics/predictor_evaluation_result.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/predictor_evaluator.py` & `citrine-2.8.0/src/citrine/informatics/predictor_evaluator.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/predictors/auto_ml_predictor.py` & `citrine-2.8.0/src/citrine/informatics/predictors/auto_ml_predictor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import List, Optional, Set
 
 from gemd.enumeration.base_enumeration import BaseEnumeration
 
-from citrine._rest.resource import Resource
+from citrine._rest.engine_resource import VersionedEngineResource
 from citrine._serialization import properties as _properties
 from citrine.informatics.data_sources import DataSource
 from citrine.informatics.descriptors import Descriptor
-from citrine.informatics.predictors import PredictorNode
-from citrine.informatics.predictors.node import _check_deprecated_training_data
+from citrine.informatics.predictors import Predictor
 
 __all__ = ['AutoMLPredictor', 'AutoMLEstimator']
 
 
 class AutoMLEstimator(BaseEnumeration):
     """[ALPHA] Algorithms to be used during AutoML model selection.
 
@@ -29,15 +28,15 @@
     LINEAR = "LINEAR"
     RANDOM_FOREST = "RANDOM_FOREST"
     GAUSSIAN_PROCESS = "GAUSSIAN_PROCESS"
     SUPPORT_VECTOR_MACHINE = "SUPPORT_VECTOR_MACHINE"
     ALL = "ALL"
 
 
-class AutoMLPredictor(Resource["AutoMLPredictor"], PredictorNode):
+class AutoMLPredictor(VersionedEngineResource['AutoMLPredictor'], Predictor):
     """A predictor interface that builds a single ML model.
 
     The model uses the set of inputs to predict the output(s).
     Only one machine learning model is built.
 
     Parameters
     ----------
@@ -59,41 +58,39 @@
         identifiers. De-duplication is performed if a uid or identifier is shared between two or
         more rows. The content of a de-duplicated row will contain the union of data across all
         rows that share the same uid or at least 1 identifier. Training data is unnecessary if the
         predictor is part of a graph that includes all training data required by this predictor.
 
     """
 
-    inputs = _properties.List(_properties.Object(Descriptor), 'inputs')
-    outputs = _properties.List(_properties.Object(Descriptor), 'outputs')
+    inputs = _properties.List(_properties.Object(Descriptor), 'data.instance.inputs')
+    outputs = _properties.List(_properties.Object(Descriptor), 'data.instance.outputs')
     estimators = _properties.Set(
         _properties.Enumeration(AutoMLEstimator),
-        'estimators',
+        'data.instance.estimators',
         default={AutoMLEstimator.RANDOM_FOREST}
     )
     training_data = _properties.List(
         _properties.Object(DataSource),
-        'training_data',
+        'data.instance.training_data',
         default=[]
     )
 
-    typ = _properties.String('type', default='AutoML', deserializable=False)
+    typ = _properties.String('data.instance.type', default='AutoML', deserializable=False)
 
     def __init__(self,
                  name: str,
                  *,
                  description: str,
                  outputs: List[Descriptor],
                  inputs: List[Descriptor],
                  estimators: Optional[Set[AutoMLEstimator]] = None,
                  training_data: Optional[List[DataSource]] = None):
         self.name: str = name
         self.description: str = description
         self.inputs: List[Descriptor] = inputs
         self.estimators: Set[AutoMLEstimator] = estimators or {AutoMLEstimator.RANDOM_FOREST}
-        self.outputs = outputs
-
-        _check_deprecated_training_data(training_data)
         self.training_data: List[DataSource] = training_data or []
+        self.outputs = outputs
 
     def __str__(self):
         return '<AutoMLPredictor {!r}>'.format(self.name)
```

### Comparing `citrine-2.24.1/src/citrine/informatics/predictors/chemical_formula_featurizer.py` & `citrine-2.8.0/src/citrine/informatics/predictors/chemical_formula_featurizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import List, Optional
 
-from citrine._rest.resource import Resource
-from citrine._serialization import properties
+from citrine._rest.engine_resource import VersionedEngineResource
+from citrine._serialization import properties as _properties
 from citrine.informatics.descriptors import ChemicalFormulaDescriptor, Descriptor
-from citrine.informatics.predictors import PredictorNode
+from citrine.informatics.predictors import Predictor
 
 __all__ = ['ChemicalFormulaFeaturizer']
 
 
-class ChemicalFormulaFeaturizer(Resource["ChemicalFormulaFeaturizer"], PredictorNode):
+class ChemicalFormulaFeaturizer(VersionedEngineResource['ChemicalFormulaFeaturizer'], Predictor):
     """
     A featurizer for chemical formulae. Inspired by Magpie.
 
     The ChemicalFormulaFeaturizer computes a configurable set of features on chemical formula data.
     The features are functions of element-level properties, which are inspired by
     `Magpie <https://bitbucket.org/wolverton/magpie/src/master/>`_. The features are configured
     using the ``features`` and ``excludes`` arguments, which accept either feature names or
@@ -126,20 +126,21 @@
         The final set of features generated by the predictor is set(features) - set(excludes).
     powers: Optional[List[int]]
         The list of powers to use when computing generalized weighted means of element properties.
         p=1 corresponds to the ordinary mean, p=2 is the root mean square, etc.
 
     """
 
-    input_descriptor = properties.Object(Descriptor, 'input')
-    features = properties.List(properties.String, 'features')
-    excludes = properties.List(properties.String, 'excludes', default=[])
-    powers = properties.List(properties.Integer, 'powers')
+    input_descriptor = _properties.Object(Descriptor, 'data.instance.input')
+    features = _properties.List(_properties.String, 'data.instance.features')
+    excludes = _properties.List(_properties.String, 'data.instance.excludes')
+    powers = _properties.List(_properties.Integer, 'data.instance.powers')
 
-    typ = properties.String('type', default='ChemicalFormulaFeaturizer', deserializable=False)
+    typ = _properties.String('data.instance.type', default='ChemicalFormulaFeaturizer',
+                             deserializable=False)
 
     def __init__(self,
                  name: str,
                  *,
                  description: str,
                  input_descriptor: ChemicalFormulaDescriptor,
                  features: Optional[List[str]] = None,
```

### Comparing `citrine-2.24.1/src/citrine/informatics/predictors/expression_predictor.py` & `citrine-2.8.0/src/citrine/informatics/predictors/expression_predictor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Mapping
 
-from citrine._rest.resource import Resource
+from citrine._rest.engine_resource import VersionedEngineResource
 from citrine._serialization import properties as _properties
 from citrine.informatics.descriptors import RealDescriptor
-from citrine.informatics.predictors import PredictorNode
+from citrine.informatics.predictors import Predictor
 
 __all__ = ['ExpressionPredictor']
 
 
-class ExpressionPredictor(Resource["ExpressionPredictor"], PredictorNode):
+class ExpressionPredictor(VersionedEngineResource['ExpressionPredictor'], Predictor):
     """A predictor that computes an output from an expression and set of bounded inputs.
 
     For a discussion of expression syntax and a list of allowed symbols,
     please see the :ref:`documentation<Expression Predictor>`.
 
     Parameters
     ----------
@@ -26,21 +26,21 @@
         descriptor that represents the output of the expression
     aliases: Mapping[str, RealDescriptor]
         a mapping from each unknown argument to its descriptor.
         All unknown arguments must have an associated descriptor.
 
     """
 
-    expression = _properties.String('expression')
-    output = _properties.Object(RealDescriptor, 'output')
-    aliases = _properties.Mapping(
-        _properties.String, _properties.Object(RealDescriptor), 'aliases'
-    )
+    expression = _properties.String('data.instance.expression')
+    output = _properties.Object(RealDescriptor, 'data.instance.output')
+    aliases = _properties.Mapping(_properties.String, _properties.Object(RealDescriptor),
+                                  'data.instance.aliases')
 
-    typ = _properties.String('type', default='AnalyticExpression', deserializable=False)
+    typ = _properties.String('data.instance.type',
+                             default='AnalyticExpression', deserializable=False)
 
     def __init__(self,
                  name: str,
                  *,
                  description: str,
                  expression: str,
                  output: RealDescriptor,
```

### Comparing `citrine-2.24.1/src/citrine/informatics/predictors/graph_predictor.py` & `citrine-2.8.0/src/citrine/informatics/predictors/predictor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,55 @@
-import warnings
-from typing import List, Optional, Union
+from typing import Optional, Type
 from uuid import UUID
 
 from citrine._rest.asynchronous_object import AsynchronousObject
-from citrine._rest.engine_resource import VersionedEngineResource
-from citrine._serialization import properties as properties
+from citrine._serialization import properties
+from citrine._serialization.polymorphic_serializable import PolymorphicSerializable
 from citrine._session import Session
-from citrine._utils.functions import format_escaped_url
-from citrine.informatics.data_sources import DataSource
+from citrine.resources.report import ReportResource
 from citrine.informatics.predictors.single_predict_request import SinglePredictRequest
 from citrine.informatics.predictors.single_prediction import SinglePrediction
-from citrine.informatics.predictors import PredictorNode, Predictor
-from citrine.resources.report import ReportResource
-
-__all__ = ['GraphPredictor']
+from citrine._utils.functions import format_escaped_url
 
+__all__ = ['Predictor']
 
-class GraphPredictor(VersionedEngineResource['GraphPredictor'], AsynchronousObject, Predictor):
-    """A predictor interface that stitches individual predictor nodes together.
 
-    The GraphPredictor is the only predictor that can be registered on the Citrine Platform
-    and carries along its meta-data regarding versioning, platform identifiers, and updates.
+class Predictor(PolymorphicSerializable['Predictor'], AsynchronousObject):
+    """Module that describes the ability to compute/predict properties of materials.
 
-    Parameters
-    ----------
-    name: str
-        name of the configuration
-    description: str
-        the description of the predictor
-    predictors: List[Union[UUID, PredictorNode]],
-        the list of individual predictors to use in the graph
-    training_data: Optional[List[DataSource]]
-        Optional sources of training data shared by all predictors in the graph.
-        Training data provided by this graph predictor does not need to be specified as part of the
-        configuration of sub-predictors. Shared training data and any training data specified
-        by a sub-predictor will be combined into a flattened list and de-duplicated
-        by uid and identifiers. De-duplication is performed if a uid or identifier is shared
-        between two or more rows. The content of a de-duplicated row will contain the union of
-        data across all rows that share the same uid or at least 1 identifier.
+    Abstract type that returns the proper type given a serialized dict. Subtype
+    based on the 'type' value of the passed in dict.
 
     """
 
     uid = properties.Optional(properties.UUID, 'id', serializable=False)
     """:Optional[UUID]: Citrine Platform unique identifier"""
-
     name = properties.String('data.name')
     description = properties.Optional(properties.String(), 'data.description')
-    predictors = properties.List(properties.Object(PredictorNode), 'data.instance.predictors')
-
-    # the default seems to be defined in instances, not the class itself
-    # this is tested in test_graph_default_training_data
-    training_data = properties.List(
-        properties.Object(DataSource), 'data.instance.training_data', default=[]
-    )
-
     version = properties.Optional(
         properties.Union([properties.Integer(), properties.String()]),
-        'metadata.version',
-        serializable=False
-    )
+        'metadata.version', serializable=False)
 
-    _api_version = "v3"
     _response_key = None
     _project_id: Optional[UUID] = None
     _session: Optional[Session] = None
     _in_progress_statuses = ["VALIDATING", "CREATED"]
     _succeeded_statuses = ["READY"]
     _failed_statuses = ["INVALID", "ERROR"]
+    _api_version = "v3"
 
-    def __init__(self,
-                 name: str,
-                 *,
-                 description: str,
-                 predictors: List[Union[UUID, PredictorNode]],
-                 training_data: Optional[List[DataSource]] = None):
-        self.name: str = name
-        self.description: str = description
-        self.training_data: List[DataSource] = training_data or []
-
-        uid_predictors = [x for x in predictors if isinstance(x, UUID)]
-        if len(uid_predictors) > 0:
-            warnings.warn(
-                "Referencing predictors by a UUID inside a GraphPredictor is no longer supported "
-                "on the Citrine Platform. Please remove all references to predictors "
-                "and add only PredictorNode objects to the `predictors` field.",
-                DeprecationWarning
-            )
-
-        self.predictors: List[PredictorNode] = [
-            x for x in predictors if isinstance(x, PredictorNode)
-        ]
-
-    def __str__(self):
-        return '<GraphPredictor {!r}>'.format(self.name)
-
-    def _path(self):
-        return format_escaped_url(
-            '/projects/{project_id}/predictors/{predictor_id}/versions/{version}',
-            project_id=self._project_id,
-            predictor_id=str(self.uid),
-            version=self.version
-        )
+    @property
+    def report(self):
+        """Fetch the predictor report."""
+        if self.uid is None or self._session is None or self._project_id is None \
+                or getattr(self, "version", None) is None:
+            msg = "Cannot get the report for a predictor that wasn't read from the platform"
+            raise ValueError(msg)
+        report_resource = ReportResource(self._project_id, self._session)
+        return report_resource.get(predictor_id=self.uid, predictor_version=self.version)
 
     @staticmethod
     def wrap_instance(predictor_data: dict) -> dict:
         """Insert a serialized embedded predictor into a module envelope.
 
         This facilitates deserialization.
         """
@@ -112,22 +57,56 @@
             "data": {
                 "name": predictor_data.get("name", ""),
                 "description": predictor_data.get("description", ""),
                 "instance": predictor_data
             }
         }
 
-    @property
-    def report(self):
-        """Fetch the predictor report."""
-        if self.uid is None or self._session is None or self._project_id is None \
-                or getattr(self, "version", None) is None:
-            msg = "Cannot get the report for a predictor that wasn't read from the platform"
-            raise ValueError(msg)
-        report_resource = ReportResource(self._project_id, self._session)
-        return report_resource.get(predictor_id=self.uid, predictor_version=self.version)
+    @classmethod
+    def get_type(cls, data) -> Type['Predictor']:
+        """Return the subtype."""
+        from .graph_predictor import GraphPredictor
+        from .expression_predictor import ExpressionPredictor
+        from .molecular_structure_featurizer import MolecularStructureFeaturizer
+        from .ingredients_to_formulation_predictor import IngredientsToFormulationPredictor
+        from .label_fractions_predictor import LabelFractionsPredictor
+        from .simple_mixture_predictor import SimpleMixturePredictor
+        from .ingredient_fractions_predictor import IngredientFractionsPredictor
+        from .auto_ml_predictor import AutoMLPredictor
+        from .mean_property_predictor import MeanPropertyPredictor
+        from .chemical_formula_featurizer import ChemicalFormulaFeaturizer
+        type_dict = {
+            "Graph": GraphPredictor,
+            "AnalyticExpression": ExpressionPredictor,
+            "MoleculeFeaturizer": MolecularStructureFeaturizer,
+            "IngredientsToSimpleMixture": IngredientsToFormulationPredictor,
+            "MeanProperty": MeanPropertyPredictor,
+            "LabelFractions": LabelFractionsPredictor,
+            "SimpleMixture": SimpleMixturePredictor,
+            "IngredientFractions": IngredientFractionsPredictor,
+            "ChemicalFormulaFeaturizer": ChemicalFormulaFeaturizer,
+            "AutoML": AutoMLPredictor,
+        }
+        typ = type_dict.get(data['data']['instance']['type'])
+
+        if typ is not None:
+            return typ
+        else:
+            raise ValueError(
+                '{} is not a valid predictor type. '
+                'Must be in {}.'.format(data['data']['instance']['type'], type_dict.keys())
+            )
+
+    def _path(self):
+        return format_escaped_url(
+            '/projects/{project_id}/predictors/{predictor_id}/versions/{version}',
+            project_id=self._project_id,
+            predictor_id=str(self.uid),
+            version=self.version
+        )
 
-    def predict(self, predict_request: SinglePredictRequest) -> SinglePrediction:
+    def predict(self,
+                predict_request: SinglePredictRequest) -> SinglePrediction:
         """Make a one-off prediction with this predictor."""
         path = self._path() + '/predict'
         res = self._session.post_resource(path, predict_request.dump(), version=self._api_version)
         return SinglePrediction.build(res)
```

### Comparing `citrine-2.24.1/src/citrine/informatics/predictors/ingredient_fractions_predictor.py` & `citrine-2.8.0/src/citrine/informatics/predictors/ingredient_fractions_predictor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Set
 
-from citrine._rest.resource import Resource
+from citrine._rest.engine_resource import VersionedEngineResource
 from citrine._serialization import properties as _properties
 from citrine.informatics.descriptors import FormulationDescriptor
-from citrine.informatics.predictors import PredictorNode
+from citrine.informatics.predictors import Predictor
 
 __all__ = ['IngredientFractionsPredictor']
 
 
-class IngredientFractionsPredictor(Resource["IngredientFractionsPredictor"], PredictorNode):
+class IngredientFractionsPredictor(
+        VersionedEngineResource["IngredientFractionsPredictor"], Predictor):
     """A predictor interface that computes ingredient fractions.
 
     Parameters
     ----------
     name: str
         name of the configuration
     description: str
@@ -21,18 +22,19 @@
         descriptor that represents the input formulation
     ingredients: Set[str]
         set of ingredients to featurize.
         If an unknown ingredient is encountered, an error will be thrown.
 
     """
 
-    input_descriptor = _properties.Object(FormulationDescriptor, 'input')
-    ingredients = _properties.Set(_properties.String, 'ingredients')
+    input_descriptor = _properties.Object(FormulationDescriptor, 'data.instance.input')
+    ingredients = _properties.Set(_properties.String, 'data.instance.ingredients')
 
-    typ = _properties.String('type', default='IngredientFractions', deserializable=False)
+    typ = _properties.String('data.instance.type', default='IngredientFractions',
+                             deserializable=False)
 
     def __init__(self,
                  name: str,
                  *,
                  description: str,
                  input_descriptor: FormulationDescriptor,
                  ingredients: Set[str]):
```

### Comparing `citrine-2.24.1/src/citrine/informatics/predictors/label_fractions_predictor.py` & `citrine-2.8.0/src/citrine/informatics/predictors/label_fractions_predictor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Set
 
-from citrine._rest.resource import Resource
+from citrine._rest.engine_resource import VersionedEngineResource
 from citrine._serialization import properties as _properties
 from citrine.informatics.descriptors import FormulationDescriptor
-from citrine.informatics.predictors import PredictorNode
+from citrine.informatics.predictors import Predictor
 
 __all__ = ['LabelFractionsPredictor']
 
 
-class LabelFractionsPredictor(Resource["LabelFractionsPredictor"], PredictorNode):
+class LabelFractionsPredictor(
+        VersionedEngineResource['LabelFractionsPredictor'], Predictor):
     """A predictor interface that computes the relative proportions of labeled ingredients.
 
     Parameters
     ----------
     name: str
         name of the configuration
     description: str
@@ -20,18 +21,19 @@
     input_descriptor: FormulationDescriptor
         descriptor that contains formulation data
     labels: Set[str]
         labels to compute the quantity fractions of
 
     """
 
-    input_descriptor = _properties.Object(FormulationDescriptor, 'input')
-    labels = _properties.Set(_properties.String, 'labels')
+    input_descriptor = _properties.Object(FormulationDescriptor, 'data.instance.input')
+    labels = _properties.Set(_properties.String, 'data.instance.labels')
 
-    typ = _properties.String('type', default='LabelFractions', deserializable=False)
+    typ = _properties.String('data.instance.type', default='LabelFractions',
+                             deserializable=False)
 
     def __init__(self,
                  name: str,
                  *,
                  description: str,
                  input_descriptor: FormulationDescriptor,
                  labels: Set[str]):
```

### Comparing `citrine-2.24.1/src/citrine/informatics/predictors/mean_property_predictor.py` & `citrine-2.8.0/src/citrine/informatics/predictors/mean_property_predictor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import List, Optional, Mapping, Union
 
-from citrine._rest.resource import Resource
+from citrine._rest.engine_resource import VersionedEngineResource
 from citrine._serialization import properties as _properties
 from citrine.informatics.data_sources import DataSource
 from citrine.informatics.descriptors import (
     FormulationDescriptor, RealDescriptor, CategoricalDescriptor
 )
-from citrine.informatics.predictors import PredictorNode
-from citrine.informatics.predictors.node import _check_deprecated_training_data
+from citrine.informatics.predictors import Predictor
 
 __all__ = ['MeanPropertyPredictor']
 
 
-class MeanPropertyPredictor(Resource["MeanPropertyPredictor"], PredictorNode):
+class MeanPropertyPredictor(
+        VersionedEngineResource['MeanPropertyPredictor'], Predictor):
     """A predictor that computes a component-weighted mean of real or categorical properties.
 
     Each component in a formulation contributes to the mean property
     a weight equal to its quantity raised to the power `p`.
     For real-valued properties, the property values of each component are averaged
     with these weights to yield the component-weighted mean property.
     For categorical-valued properties, these weights are accumulated to yield a
@@ -59,36 +59,36 @@
         identifiers. De-duplication is performed if a uid or identifier is shared between two or
         more rows. The content of a de-duplicated row will contain the union of data across all
         rows that share the same uid or at least 1 identifier. Training data is unnecessary if the
         predictor is part of a graph that includes all training data required by this predictor.
 
     """
 
-    input_descriptor = _properties.Object(FormulationDescriptor, 'input')
+    input_descriptor = _properties.Object(FormulationDescriptor, 'data.instance.input')
     properties = _properties.List(
         _properties.Union(
             [_properties.Object(RealDescriptor), _properties.Object(CategoricalDescriptor)]
         ),
-        'properties'
+        'data.instance.properties'
     )
-    p = _properties.Float('p')
-    impute_properties = _properties.Boolean('impute_properties')
-    label = _properties.Optional(_properties.String, 'label')
+    p = _properties.Float('data.instance.p')
+    impute_properties = _properties.Boolean('data.instance.impute_properties')
+    label = _properties.Optional(_properties.String, 'data.instance.label')
     default_properties = _properties.Optional(
         _properties.Mapping(
             _properties.String,
             _properties.Union([_properties.String, _properties.Float])
         ),
-        'default_properties'
+        'data.instance.default_properties'
     )
     training_data = _properties.List(
-        _properties.Object(DataSource), 'training_data', default=[]
+        _properties.Object(DataSource), 'data.instance.training_data', default=[]
     )
 
-    typ = _properties.String('type', default='MeanProperty', deserializable=False)
+    typ = _properties.String('data.instance.type', default='MeanProperty', deserializable=False)
 
     def __init__(self,
                  name: str,
                  *,
                  description: str,
                  input_descriptor: FormulationDescriptor,
                  properties: List[Union[RealDescriptor, CategoricalDescriptor]],
@@ -101,13 +101,11 @@
         self.description: str = description
         self.input_descriptor: FormulationDescriptor = input_descriptor
         self.properties: List[Union[RealDescriptor, CategoricalDescriptor]] = properties
         self.p: float = p
         self.impute_properties: bool = impute_properties
         self.label: Optional[str] = label
         self.default_properties: Optional[Mapping[str, Union[str, float]]] = default_properties
-
-        _check_deprecated_training_data(training_data)
         self.training_data: List[DataSource] = training_data or []
 
     def __str__(self):
         return '<MeanPropertyPredictor {!r}>'.format(self.name)
```

### Comparing `citrine-2.24.1/src/citrine/informatics/predictors/molecular_structure_featurizer.py` & `citrine-2.8.0/src/citrine/informatics/predictors/molecular_structure_featurizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # flake8: noqa
 # The docstring includes many long links that violate flake8, and it's easier to noqa
 # the whole file than to pick out the offending lines.
 from typing import List, Optional
 
-from citrine._rest.resource import Resource
+from citrine._rest.engine_resource import VersionedEngineResource
 from citrine._serialization import properties as _properties
 from citrine.informatics.descriptors import Descriptor, MolecularStructureDescriptor
-from citrine.informatics.predictors import PredictorNode
+from citrine.informatics.predictors import Predictor
 
 __all__ = ['MolecularStructureFeaturizer']
 
 
-class MolecularStructureFeaturizer(Resource["MolecularStructureFeaturizer"], PredictorNode):
+class MolecularStructureFeaturizer(VersionedEngineResource['MolecularStructureFeaturizer'], Predictor):
     """
     A featurizer for molecular structures, powered by CDK.
 
     The MolecularStructureFeaturizer will compute a configurable set of features on molecular
     structure data, e.g., SMILES or InChI strings.  The features are computed using the
     `Chemistry Development Kit (CDK) <https://cdk.github.io/>`_.  The features are configured
     using the ``features`` and ``excludes`` arguments, which accept either feature names or predefined
@@ -74,19 +74,19 @@
         the list of features to compute, either by name or by group alias.
     excludes: List[str]
         list of features to exclude (accepts same set of values as features). The final set
         of outputs generated by the predictor is set(features) - set(excludes).
 
     """
 
-    input_descriptor = _properties.Object(Descriptor, 'descriptor')
-    features = _properties.List(_properties.String, 'features')
-    excludes = _properties.List(_properties.String, 'excludes')
+    input_descriptor = _properties.Object(Descriptor, 'data.instance.descriptor')
+    features = _properties.List(_properties.String, 'data.instance.features')
+    excludes = _properties.List(_properties.String, 'data.instance.excludes')
 
-    typ = _properties.String('type', default='MoleculeFeaturizer', deserializable=False)
+    typ = _properties.String('data.instance.type', default='MoleculeFeaturizer', deserializable=False)
 
     def __init__(self,
                  name: str,
                  *,
                  description: str,
                  input_descriptor: MolecularStructureDescriptor,
                  features: Optional[List[str]] = None,
```

### Comparing `citrine-2.24.1/src/citrine/informatics/predictors/single_predict_request.py` & `citrine-2.8.0/src/citrine/informatics/predictors/single_predict_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import List, Optional
 from uuid import UUID
 
 from citrine._serialization import properties
 from citrine._serialization.serializable import Serializable
 from citrine.informatics.design_candidate import DesignMaterial
 
-__all__ = ['SinglePredictRequest']
-
 
 class SinglePredictRequest(Serializable["SinglePredictRequest"]):
     """A Citrine Single Predict Request.
 
     This class represents a request to make a prediction against a predictor.
     """
```

### Comparing `citrine-2.24.1/src/citrine/informatics/predictors/single_prediction.py` & `citrine-2.8.0/src/citrine/informatics/predictors/single_prediction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import List
 from uuid import UUID
 
 from citrine._serialization import properties
 from citrine._serialization.serializable import Serializable
 from citrine.informatics.design_candidate import DesignMaterial
 
-__all__ = ['SinglePrediction']
-
 
 class SinglePrediction(Serializable["SinglePrediction"]):
     """A Citrine Single Prediction.
 
     This class represents the result of a prediction made using a predictor.
     """
```

### Comparing `citrine-2.24.1/src/citrine/informatics/reports.py` & `citrine-2.8.0/src/citrine/informatics/reports.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/scores.py` & `citrine-2.8.0/src/citrine/informatics/scores.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/workflows/design_workflow.py` & `citrine-2.8.0/src/citrine/resources/user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,103 @@
-from typing import Optional, Union
-from uuid import UUID
+"""Resources that represent both individual and collections of users."""
+from typing import Optional
 
-from citrine._rest.resource import Resource
+from citrine._rest.collection import Collection
+from citrine._rest.resource import Resource, ResourceTypeEnum
 from citrine._serialization import properties
-from citrine.informatics.workflows.workflow import Workflow
-from citrine.resources.design_execution import DesignExecutionCollection
-from citrine._rest.ai_resource_metadata import AIResourceMetadata
+from citrine._session import Session
 
-__all__ = ['DesignWorkflow']
 
-
-class DesignWorkflow(Resource['DesignWorkflow'], Workflow, AIResourceMetadata):
-    """Object that generates scored materials that may approach higher values of the score.
+class User(Resource['User']):
+    """
+    A Citrine User.
 
     Parameters
     ----------
-    name: str
-        the name of the workflow
-    design_space_id: Optional[UUID]
-        the UUID corresponding to the design space to use
-    predictor_id: Optional[UUID]
-        the UUID corresponding to the predictor to use
-    predictor_version: Optional[Union[int, str]]
-        the version of the predictor to use
-    description: Optional[str]
-        a description of the workflow
+    screen_name: str
+        Screen name of the user.
+    email: str
+        Email address of the user.
+    position: str
+        Position of the user.
+    is_admin: bool
+        Whether or not the user is an administrator.
+    session: Session, optional
+        Citrine session used to connect to the database.
 
     """
 
-    design_space_id = properties.Optional(properties.UUID, 'design_space_id')
-    predictor_id = properties.Optional(properties.UUID, 'predictor_id')
-    predictor_version = properties.Optional(
-        properties.Union([properties.Integer(), properties.String()]), 'predictor_version')
-    branch_id: Optional[UUID] = properties.Optional(properties.UUID, 'branch_id')
-    """:Optional[UUID]: Unique ID of the branch that contains this workflow."""
-
-    status_description = properties.String('status_description', serializable=False)
-    """:str: more detailed description of the workflow's status"""
-    typ = properties.String('type', default='DesignWorkflow', deserializable=False)
+    _resource_type = ResourceTypeEnum.USER
+    _session: Optional[Session] = None
+
+    uid = properties.Optional(properties.UUID, 'id')
+    screen_name = properties.String('screen_name')
+    position = properties.Optional(properties.String(), 'position')
+    email = properties.String('email')
+    is_admin = properties.Boolean('is_admin')
 
     def __init__(self,
-                 name: str,
                  *,
-                 design_space_id: Optional[UUID] = None,
-                 predictor_id: Optional[UUID] = None,
-                 predictor_version: Optional[Union[int, str]] = None,
-                 description: Optional[str] = None):
-        self.name = name
-        self.design_space_id = design_space_id
-        self.predictor_id = predictor_id
-        self.predictor_version = predictor_version
-        self.description = description
+                 screen_name: str,
+                 email: str,
+                 position: Optional[str],
+                 is_admin: bool):
+        self.email: str = email
+        self.position: Optional[str] = position
+        self.screen_name: str = screen_name
+        self.is_admin: bool = is_admin
 
     def __str__(self):
-        return '<DesignWorkflow {!r}>'.format(self.name)
+        return '<User {!r}>'.format(self.screen_name)
+
+    def get(self):
+        """Retrieve a specific user from the database."""
+        raise NotImplementedError("Get Not Implemented in Citrine Platform")
+
+
+class UserCollection(Collection[User]):
+    """Represents the collection of all users."""
+
+    _path_template = '/users'
+    _collection_key = 'users'
+    _individual_key = 'user'
+    _resource = User
 
-    @property
-    def design_executions(self) -> DesignExecutionCollection:
-        """Return a resource representing all visible executions of this workflow."""
-        if getattr(self, 'project_id', None) is None:
-            raise AttributeError('Cannot initialize execution without project reference!')
-        return DesignExecutionCollection(
-            project_id=self.project_id, session=self._session, workflow_id=self.uid)
+    def __init__(self, session: Session):
+        self.session: Session = session
+
+    def me(self):
+        """Get information about the current user."""
+        data = self.session.get_resource(self._path_template + '/me')
+        return self.build(data)
+
+    def build(self, data):
+        """
+        Build an individual user from a dictionary.
+
+        Parameters
+        ----------
+        data: dict
+          A dictionary representing the user.
+
+        Returns
+        -------
+        User
+          The user created from data.
+
+        """
+        user = User.build(data)
+        user._session = self.session
+        return user
+
+    def register(self,
+                 *,
+                 screen_name: str,
+                 email: str,
+                 position: str,
+                 is_admin: bool) -> User:
+        """Register a User."""
+        return super().register(User(
+            screen_name=screen_name,
+            email=email,
+            position=position,
+            is_admin=is_admin))
```

### Comparing `citrine-2.24.1/src/citrine/informatics/workflows/predictor_evaluation_workflow.py` & `citrine-2.8.0/src/citrine/informatics/workflows/predictor_evaluation_workflow.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/informatics/workflows/workflow.py` & `citrine-2.8.0/src/citrine/informatics/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/jobs/job.py` & `citrine-2.8.0/src/citrine/jobs/job.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,23 +10,26 @@
 from citrine._session import Session
 from citrine._utils.functions import format_escaped_url
 from citrine.exceptions import PollingTimeoutError, JobFailureError
 
 logger = getLogger(__name__)
 
 
-class JobSubmissionResponse(Resource['JobSubmissionResponse']):
+class JobSubmissionResponse(Resource['AraJobStatus']):
     """A response to a submit-job request for the job submission framework.
 
     This is returned as a successful response from the remote service.
     """
 
     job_id = properties.UUID("job_id")
     """:UUID: job id of the job submission request"""
 
+    def __init__(self):
+        pass  # pragma: no cover
+
 
 class TaskNode(Resource['TaskNode']):
     """Individual task status.
 
     The TaskNode describes a component of an overall job.
     """
 
@@ -57,41 +60,38 @@
     status = properties.String("status")
     """:str: The status of the job. One of "Running", "Success", or "Failure"."""
     tasks = properties.List(Object(TaskNode), "tasks")
     """:List[TaskNode]: all of the constituent task required to complete this job"""
     output = properties.Optional(properties.Mapping(String, String), 'output')
     """:Optional[dict[str, str]]: job output properties and results"""
 
+    def __init__(self):
+        pass  # pragma: no cover
+
 
-def _poll_for_job_completion(session: Session,
-                             project_id: Union[UUID, str],
-                             job: Union[JobSubmissionResponse, UUID, str],
-                             *,
+def _poll_for_job_completion(session: Session, project_id: Union[UUID, str],
+                             job: Union[JobSubmissionResponse, UUID, str], *,
                              timeout: float = 2 * 60,
-                             polling_delay: float = 2.0,
-                             raise_errors: bool = True,
-                             ) -> JobStatusResponse:
+                             polling_delay: float = 2.0) -> JobStatusResponse:
     """
-    Polls for job completion given a timeout.
+    Polls for job completion given a timeout, failing with an exception on job failure.
 
     This polls for job completion given the Job ID, failing appropriately if the job result
     was not successful.
 
     Parameters
     ----------
     job
         The job submission object or job ID that was given from a job submission.
     timeout
         Amount of time to wait on the job (in seconds) before giving up. Defaults
         to 2 minutes. Note that this number has no effect on the underlying job
         itself, which can also time out server-side.
     polling_delay:
         How long to delay between each polling retry attempt.
-    raise_errors:
-        Whether to raise a JobFailureError on job failure.
 
     Returns
     -------
     JobStatusResponse
         The job response information that can be used to extract relevant
         information from the completed job.
 
@@ -115,20 +115,19 @@
             sleep(polling_delay)
         else:
             logger.error('Job exceeded user timeout of {} seconds.'.format(timeout))
             logger.debug('Last status: {}'.format(status.dump()))
             raise PollingTimeoutError('Job {} timed out.'.format(job_id))
     if status.status == 'Failure':
         logger.debug('Job terminated with Failure status: {}'.format(status.dump()))
-        if raise_errors:
-            failure_reasons = []
-            for task in status.tasks:
-                if task.status == 'Failure':
-                    logger.error('Task {} failed with reason "{}"'.format(
-                        task.id, task.failure_reason))
-                    failure_reasons.append(task.failure_reason)
-            raise JobFailureError(
-                message='Job {} terminated with Failure status. Failure reasons: {}'.format(
-                    job_id, failure_reasons), job_id=job_id,
-                failure_reasons=failure_reasons)
+        failure_reasons = []
+        for task in status.tasks:
+            if task.status == 'Failure':
+                logger.error('Task {} failed with reason "{}"'.format(
+                    task.id, task.failure_reason))
+                failure_reasons.append(task.failure_reason)
+        raise JobFailureError(
+            message='Job {} terminated with Failure status. Failure reasons: {}'.format(
+                job_id, failure_reasons), job_id=job_id,
+            failure_reasons=failure_reasons)
 
     return status
```

### Comparing `citrine-2.24.1/src/citrine/jobs/waiting.py` & `citrine-2.8.0/src/citrine/jobs/waiting.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from pprint import pprint
 from typing import Union
 
 from citrine._rest.collection import Collection
 from citrine._rest.asynchronous_object import AsynchronousObject
 from citrine.informatics.executions.design_execution import DesignExecution
 from citrine.informatics.executions.generative_design_execution import GenerativeDesignExecution
-from citrine.informatics.executions.sample_design_space_execution import SampleDesignSpaceExecution
 from citrine.informatics.executions import PredictorEvaluationExecution
 from citrine.informatics.modules import Module
 
 
 class ConditionTimeoutError(RuntimeError):
     """Error that is raised when timeout is reached but the checked condition is still False."""
 
@@ -129,32 +128,21 @@
 
 
 def wait_while_executing(
     *,
     collection: Union[
         Collection[PredictorEvaluationExecution],
         Collection[DesignExecution],
-        Collection[GenerativeDesignExecution],
-        Collection[SampleDesignSpaceExecution]
-    ],
-    execution: Union[
-        PredictorEvaluationExecution,
-        DesignExecution,
-        GenerativeDesignExecution,
-        SampleDesignSpaceExecution
+        Collection[GenerativeDesignExecution]
     ],
+    execution: Union[PredictorEvaluationExecution, DesignExecution, GenerativeDesignExecution],
     print_status_info: bool = False,
     timeout: float = 1800.0,
     interval: float = 3.0,
-) -> Union[
-        PredictorEvaluationExecution,
-        DesignExecution,
-        GenerativeDesignExecution,
-        SampleDesignSpaceExecution,
-]:
+) -> Union[PredictorEvaluationExecution, DesignExecution, GenerativeDesignExecution]:
     """
     Wait until execution is finished.
 
     Parameters
     ----------
     execution : Union[PredictorEvaluationExecution, DesignExecution]
         an execution to monitor
```

### Comparing `citrine-2.24.1/src/citrine/resources/audit_info.py` & `citrine-2.8.0/src/citrine/resources/audit_info.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from citrine._serialization.serializable import Serializable
 from citrine._serialization import properties
 from gemd.entity.dict_serializable import DictSerializable
 
 
-class AuditInfo(Serializable, DictSerializable, typ="audit_info"):
+class AuditInfo(Serializable, DictSerializable):
     """Model that holds audit metadata. AuditInfo objects should not be created by the user."""
 
     created_by = properties.Optional(properties.UUID, 'created_by')
     """:Optional[UUID]: ID of the user who created the object"""
     created_at = properties.Optional(properties.Datetime, 'created_at')
     """:Optional[datetime]: Time, in ms since epoch, at which the object was created"""
     updated_by = properties.Optional(properties.UUID, 'updated_by')
@@ -32,7 +32,11 @@
                 self.updated_by, self.updated_at)
         else:
             update_str = ''
         return create_str + update_str
 
     def __eq__(self, other):
         return self.__repr__() == other.__repr__()
+
+    def as_dict(self):
+        """Return the object as a dictionary."""
+        return self.dump()
```

### Comparing `citrine-2.24.1/src/citrine/resources/branch.py` & `citrine-2.8.0/src/citrine/resources/branch.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Iterator, Optional, Union
 from uuid import UUID
 
 from citrine._rest.collection import Collection
 from citrine._rest.resource import Resource
 from citrine._serialization import properties
 from citrine._session import Session
-from citrine.exceptions import NotFound
+from citrine._utils.functions import format_escaped_url
 from citrine.resources.data_version_update import BranchDataUpdate, NextBranchVersionRequest
 from citrine.resources.design_workflow import DesignWorkflowCollection
 from citrine.resources.experiment_datasource import (ExperimentDataSourceCollection,
                                                      ExperimentDataSource)
 
 
 class Branch(Resource['Branch']):
@@ -96,41 +96,14 @@
 
         """
         branch = Branch.build(data)
         branch.session = self.session
         branch.project_id = self.project_id
         return branch
 
-    def get_by_root_id(self, *, branch_root_id: Union[UUID, str]) -> Branch:
-        """
-        Given a branch root ID, retrieve the latest version of the branch.
-
-        Parameters
-        ---------
-        branch_root_id:  Union[UUID, str]
-            Unique identifier of the branch root
-
-        Returns
-        -------
-        Branch
-            The latest version of the branch.
-
-        """
-        params = {"root": str(branch_root_id), "version": "latest"}
-        branch = next(self._list_with_params(per_page=1, **params), None)
-        if branch:
-            return branch
-        else:
-            raise NotFound.build(
-                message=f"Branch root '{branch_root_id}' not found",
-                method="GET",
-                path=self._get_path(),
-                params=params
-            )
-
     def list(self, *, per_page: int = 20) -> Iterator[Branch]:
         """
         List active branches using pagination.
 
         Yields all active branches, paginating over all available pages.
 
         Parameters
@@ -161,47 +134,46 @@
 
         Returns
         -------
         Iterator[Branch]
             Archived branches in this collection.
 
         """
-        return self._list_with_params(per_page=per_page, archived=True)
-
-    def _list_with_params(self, *, per_page, **kwargs):
-        fetcher = functools.partial(self._fetch_page, additional_params=kwargs)
+        fetcher = functools.partial(self._fetch_page, additional_params={"archived": True})
         return self._paginator.paginate(page_fetcher=fetcher,
                                         collection_builder=self._build_collection_elements,
                                         per_page=per_page)
 
     def archive(self, uid: Union[UUID, str] = None):
         """
         Archive a branch.
 
         Parameters
         ----------
         uid: Union[UUID, str]
             Unique identifier of the branch to archive
 
         """
-        url = self._get_path(uid, action="archive")
+        archive_path_template = f'{self._get_path(uid)}/archive'
+        url = format_escaped_url(archive_path_template, project_id=self.project_id, branch_id=uid)
         data = self.session.put_resource(url, {}, version=self._api_version)
         return self.build(data)
 
     def restore(self, uid: Union[UUID, str] = None):
         """
         Restore an archived branch.
 
         Parameters
         ----------
         uid: Union[UUID, str]
             Unique identifier of the branch to restore
 
         """
-        url = self._get_path(uid, action="restore")
+        restore_path_template = f'{self._get_path(uid)}/restore'
+        url = format_escaped_url(restore_path_template, project_id=self.project_id, branch_id=uid)
         data = self.session.put_resource(url, {}, version=self._api_version)
         return self.build(data)
 
     def update_data(self,
                     branch: Union[UUID, str, Branch],
                     *,
                     use_existing: bool = True,
@@ -260,15 +232,16 @@
 
         Returns
         -------
         BranchDataUpdate
             A list of data updates and compatible predictors
 
         """
-        path = self._get_path(uid=uid, action="data-version-updates-predictor")
+        path_template = f'{self._path_template}/{{branch_id}}/data-version-updates-predictor'
+        path = format_escaped_url(path_template, project_id=self.project_id, branch_id=uid)
         data = self.session.get_resource(path, version=self._api_version)
         return BranchDataUpdate.build(data)
 
     def next_version(self,
                      branch_root_id: Union[UUID, str],
                      *,
                      branch_instructions: NextBranchVersionRequest,
@@ -295,14 +268,16 @@
 
         Returns
         -------
         Branch
             The new branch record after version update
 
         """
-        path = self._get_path(action="next-version-predictor")
+        path_template = f'{self._path_template}/next-version-predictor'
+
+        path = format_escaped_url(path_template, project_id=self.project_id)
         data = self.session.post_resource(path, branch_instructions.dump(),
                                           version=self._api_version,
                                           params={
                                               'root': str(branch_root_id),
                                               'retrain_models': retrain_models})
         return self.build(data)
```

### Comparing `citrine-2.24.1/src/citrine/resources/condition_template.py` & `citrine-2.8.0/src/citrine/resources/condition_template.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Resources that represent condition templates."""
 from typing import List, Dict, Optional, Type
 
-from citrine._rest.resource import GEMDResource
+from citrine._rest.resource import Resource
+from citrine._serialization.properties import List as PropertyList
+from citrine._serialization.properties import Optional as PropertyOptional
+from citrine._serialization.properties import String, Mapping, Object
 from citrine.resources.attribute_templates import AttributeTemplate, AttributeTemplateCollection
+from citrine.resources.data_concepts import DataConcepts
 from gemd.entity.bounds.base_bounds import BaseBounds
 from gemd.entity.template.condition_template import ConditionTemplate as GEMDConditionTemplate
 
 
-class ConditionTemplate(
-    GEMDResource['ConditionTemplate'],
-    AttributeTemplate,
-    GEMDConditionTemplate,
-    typ=GEMDConditionTemplate.typ
-):
+class ConditionTemplate(AttributeTemplate, Resource['ConditionTemplate'], GEMDConditionTemplate):
     """
     A condition template.
 
     Parameters
     ----------
     name: str
         The name of the condition template.
@@ -33,25 +32,32 @@
         are hierarchical strings that store information about an entity. They can be used
         for filtering and discoverability.
 
     """
 
     _response_key = GEMDConditionTemplate.typ  # 'condition_template'
 
+    name = String('name', override=True)
+    description = PropertyOptional(String(), 'description', override=True)
+    uids = Mapping(String('scope'), String('id'), 'uids', override=True)
+    tags = PropertyOptional(PropertyList(String()), 'tags', override=True)
+    bounds = Object(BaseBounds, 'bounds', override=True)
+    typ = String('type')
+
     def __init__(self,
                  name: str,
                  *,
                  bounds: BaseBounds,
                  uids: Optional[Dict[str, str]] = None,
                  description: Optional[str] = None,
                  tags: Optional[List[str]] = None
                  ):
         if uids is None:
             uids = dict()
-        super(AttributeTemplate, self).__init__()
+        DataConcepts.__init__(self, GEMDConditionTemplate.typ)
         GEMDConditionTemplate.__init__(self, name=name, bounds=bounds, tags=tags,
                                        uids=uids, description=description)
 
     def __str__(self):
         return '<Condition template {!r}>'.format(self.name)
```

### Comparing `citrine-2.24.1/src/citrine/resources/data_concepts.py` & `citrine-2.8.0/src/citrine/resources/data_concepts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 """Top-level class for all data concepts objects and collections thereof."""
 from abc import abstractmethod, ABC
 import re
 from typing import TypeVar, Type, List, Union, Optional, Iterator, Iterable
 from uuid import UUID, uuid4
 
-from gemd.entity.dict_serializable import DictSerializable, DictSerializableMeta
+from gemd.entity.dict_serializable import DictSerializable
 from gemd.entity.base_entity import BaseEntity
 from gemd.entity.link_by_uid import LinkByUID
 from gemd.json import GEMDJson
 from gemd.util import recursive_foreach, set_uuids
 
 from citrine._rest.collection import Collection
 from citrine._serialization.polymorphic_serializable import PolymorphicSerializable
-from citrine._serialization.properties import String, Mapping, Object
-from citrine._serialization.properties import Optional as PropertyOptional
-from citrine._serialization.properties import List as PropertyList
+from citrine._serialization.properties import Property as SerializableProperty
 from citrine._serialization.properties import UUID as PropertyUUID
 from citrine._serialization.serializable import Serializable
 from citrine._session import Session
 from citrine._utils.functions import scrub_none, replace_objects_with_links, \
     format_escaped_url
 from citrine.exceptions import BadRequest
 from citrine.resources.audit_info import AuditInfo
 from citrine.jobs.job import _poll_for_job_completion
 from citrine.resources.response import Response
 
 CITRINE_SCOPE = 'id'
 CITRINE_TAG_PREFIX = 'citr_auto'
 
 
-class DataConceptsMeta(DictSerializableMeta):
-    """Data Concepts metaclass for handling serialization."""
-
-    def __init__(cls, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        resolved = next((b.typ for b in cls.__bases__ if getattr(b, "typ", None) is not None),
-                        None)
-        if resolved is not None:
-            cls._typ_stash = resolved
-        cls.typ = String("type")
-
-
-class DataConcepts(
-    PolymorphicSerializable['DataConcepts'],
-    BaseEntity,
-    metaclass=DataConceptsMeta
-):
+class DataConcepts(DictSerializable, PolymorphicSerializable['DataConcepts'], ABC):
     """
     An abstract data concepts object.
 
     DataConcepts must be extended along with `Resource`.
 
     Parameters
     ----------
     typ: str
         A string denoting what type of DataConcepts class a particular instantiation is.
 
     """
 
-    """Properties inherited from GEMD Base Entitiy."""
-    uids = PropertyOptional(Mapping(String('scope'), String('id')), 'uids', override=True)
-    tags = PropertyOptional(PropertyList(String()), 'tags', override=True)
-
     _type_key = "type"
     """str: key used to determine type of serialized object."""
 
+    _client_keys = []
+    """list of str: keys that are in the serialized object, but are only relevant to the client.
+    These keys are not passed to the data model during deserialization.
+    """
+
+    class_dict = dict()
+    """
+    Dict[str, class]: dictionary from the type key to the class for every class \
+    that extends DataConcepts.
+
+    Only populated if the :func:`get_type` method is invoked.
+    """
+
     collection_dict = dict()
     """
     Dict[str, class]: dictionary from the type key to the associated collection \
      for every class that extends DataConcepts.
 
     Only populated if the :func:`get_collection_type` method is invoked.
     """
 
+    json_support = None
+    """
+    Custom json support object, which knows how to serialize and deserialize DataConcepts classes.
+    """
+
+    client_specific_fields = {
+        "audit_info": AuditInfo,
+        "dataset": PropertyUUID,
+    }
     """
     Fields that are added to the gemd data objects when they are used in this client
 
     * audit_info contains who/when information about the resource on the citrine platform
     * dataset is the unique Citrine id of the dataset that owns this resource
     """
-    _audit_info = PropertyOptional(Object(AuditInfo), "audit_info", serializable=False)
-    _dataset = PropertyOptional(PropertyUUID, "dataset", serializable=False)
 
-    def __init__(self):
-        self.typ = self._typ_stash
+    def __init__(self, typ: str):
+        self.typ = typ
+        for field in self.client_specific_fields:
+            self.__setattr__("_{}".format(field), None)
 
     @property
     def audit_info(self) -> Optional[AuditInfo]:
         """Get the audit info object."""
         return self._audit_info
 
     @property
@@ -97,14 +97,74 @@
 
     @property
     def dataset(self) -> Optional[UUID]:
         """Get the dataset of this object, if it was returned by the backend."""
         return self._dataset
 
     @classmethod
+    def from_dict(cls, d: dict):
+        """
+        Build a data concepts object from a dictionary.
+
+        This is an internal method, and should not be called directly by users.  First,
+        it removes client_specific_fields from d, if present, and then calls the gemd
+        object's from_dict method.  Finally, it adds those fields back.
+
+        Parameters
+        ----------
+        d: dict
+            A representation of the object that will be shallowly loaded into the object.
+
+        """
+        popped = {k: d.pop(k, None) for k in cls.client_specific_fields}
+        obj = super().from_dict(d)
+
+        for field, clazz in cls.client_specific_fields.items():
+            value = popped[field]
+            if value is None:
+                deserialized = None
+            elif issubclass(clazz, DictSerializable):
+                if not isinstance(value, dict):
+                    raise TypeError(
+                        "{} must be a dictionary or None but was {}".format(field, value))
+                deserialized = clazz.build(value)
+            elif issubclass(clazz, SerializableProperty):
+                # deserialize handles type checking already
+                deserialized = clazz(clazz).deserialize(value)
+            else:
+                raise NotImplementedError("No deserialization strategy reported for client "
+                                          "field type {} for field {}.".format(clazz, field))
+            setattr(obj, "_{}".format(field), deserialized)
+        return obj
+
+    @classmethod
+    def build(cls, data: dict):
+        """
+        Build a data concepts object from a dictionary or from a GEMD object.
+
+        This is an internal method, and should not be called directly by users.
+
+        Parameters
+        ----------
+        data: dict
+            A representation of the object. It must be possible to put this dictionary through
+            the loads/dumps cycle of the GMED
+            :py:mod:`JSON encoder <gemd.json>`. The ensuing dictionary must
+            have a `type` field that corresponds to the response key of this class or of
+            :py:class:`LinkByUID <gemd.entity.link_by_uid.LinkByUID>`.
+
+        Returns
+        -------
+        DataConcepts
+            An object corresponding to a data concepts resource.
+
+        """
+        return cls.get_json_support().copy(data)
+
+    @classmethod
     def get_type(cls, data) -> Type[Serializable]:
         """
         Determine the class of a serialized object.
 
         The data dictionary must have a 'type' key whose value corresponds to the response key
         of one of the classes that extends :class:`DataConcepts`.
 
@@ -116,17 +176,21 @@
 
         Returns
         -------
         class
             The class corresponding to data.
 
         """
+        if len(DataConcepts.class_dict) == 0:
+            # This line is only reached if get_type is called before build,
+            # which is hard to reproduce, hence the no cover.
+            DataConcepts._make_class_dict()  # pragma: no cover
         if isinstance(data, DictSerializable):
             data = data.as_dict()
-        return DictSerializable.class_mapping[data['type']]
+        return DataConcepts.class_dict[data['type']]
 
     @classmethod
     def get_collection_type(cls, data) -> "Type[DataConceptsCollection]":
         """
         Determine the associated collection type for a serialized data object.
 
         The data dictionary must have a 'type' key whose value corresponds to the individual key
@@ -148,14 +212,39 @@
             # This branch is intended to populate collection dict on first call
             DataConcepts._make_collection_dict()
         if isinstance(data, DictSerializable):
             data = data.as_dict()
         return DataConcepts.collection_dict[data['type']]
 
     @staticmethod
+    def _make_class_dict():
+        """Construct a dictionary from each type key to the class."""
+        from citrine.resources.condition_template import ConditionTemplate
+        from citrine.resources.parameter_template import ParameterTemplate
+        from citrine.resources.property_template import PropertyTemplate
+        from citrine.resources.material_template import MaterialTemplate
+        from citrine.resources.measurement_template import MeasurementTemplate
+        from citrine.resources.process_template import ProcessTemplate
+        from citrine.resources.ingredient_spec import IngredientSpec
+        from citrine.resources.material_spec import MaterialSpec
+        from citrine.resources.measurement_spec import MeasurementSpec
+        from citrine.resources.process_spec import ProcessSpec
+        from citrine.resources.ingredient_run import IngredientRun
+        from citrine.resources.material_run import MaterialRun
+        from citrine.resources.measurement_run import MeasurementRun
+        from citrine.resources.process_run import ProcessRun
+        _clazz_list = [ConditionTemplate, ParameterTemplate, PropertyTemplate,
+                       MaterialTemplate, MeasurementTemplate, ProcessTemplate,
+                       IngredientSpec, MaterialSpec, MeasurementSpec, ProcessSpec,
+                       IngredientRun, MaterialRun, MeasurementRun, ProcessRun]
+        for clazz in _clazz_list:
+            DataConcepts.class_dict[clazz._response_key] = clazz
+        DataConcepts.class_dict['link_by_uid'] = LinkByUID
+
+    @staticmethod
     def _make_collection_dict():
         """Construct a dictionary from each type key to the associated collection."""
         from citrine.resources.condition_template import ConditionTemplateCollection
         from citrine.resources.parameter_template import ParameterTemplateCollection
         from citrine.resources.property_template import PropertyTemplateCollection
         from citrine.resources.material_template import MaterialTemplateCollection
         from citrine.resources.measurement_template import MeasurementTemplateCollection
@@ -174,14 +263,69 @@
             IngredientSpecCollection, MaterialSpecCollection, MeasurementSpecCollection,
             ProcessSpecCollection, IngredientRunCollection, MaterialRunCollection,
             MeasurementRunCollection, ProcessRunCollection
         ]
         for collection in _collection_list:
             DataConcepts.collection_dict[collection._individual_key] = collection
 
+    @classmethod
+    def get_json_support(cls):
+        """Get a DataConcepts-compatible json serializer/deserializer."""
+        if cls.json_support is None:
+            DataConcepts._make_class_dict()
+            cls.json_support = GEMDJson(scope=CITRINE_SCOPE)
+            cls.json_support.register_classes(
+                {k: v for k, v in DataConcepts.class_dict.items() if k != "link_by_uid"}
+            )
+        return cls.json_support
+
+    def dump(self) -> dict:
+        """Overload dump to include the client-specific fields."""
+        result = super().dump()
+        for field, clazz in self.client_specific_fields.items():
+            value = getattr(self, f"_{field}", None)
+            if value is None:
+                serialized = None
+            elif isinstance(value, DictSerializable):
+                serialized = value.as_dict()
+            elif issubclass(clazz, SerializableProperty):
+                # deserialize handles type checking already
+                serialized = clazz(clazz).serialize(value)
+            else:  # pragma: no cover
+                raise NotImplementedError("No serialization strategy reported for client "
+                                          "field type {} for field {}.".format(clazz, field))
+            if serialized is not None:
+                result[field] = serialized
+        return result
+
+    def as_dict(self) -> dict:
+        """
+        Dump to a dictionary (useful for interoperability with gemd).
+
+        Note that something in the serialization stack changes the result df __dict__ dramatically
+        between gemd.entity.dict_serializable and this class.  This means we can't just use gemd's
+        as_dict, and so we'll trust citrine._serialization.properties to get us the list.
+        """
+        from citrine._serialization import properties as serial_properties
+
+        result = dict()
+        for property_name in serial_properties.Object(type(self)).fields:
+            result[property_name] = getattr(self, property_name, None)
+        result["type"] = result.pop("typ")
+        return result
+
+    def _dict_for_compare(self):
+        """Which fields should be ignored in equality comparison."""
+        base = super()._dict_for_compare()
+        for field in base:
+            base[field] = getattr(self, field, base[field])
+        base.pop("audit_info", None)
+        base.pop("dataset", None)
+        return base
+
 
 def _make_link_by_uid(gemd_object_rep: Union[str, UUID, BaseEntity, LinkByUID]) -> LinkByUID:
     if isinstance(gemd_object_rep, BaseEntity):
         return gemd_object_rep.to_link(CITRINE_SCOPE, allow_fallback=True)
     elif isinstance(gemd_object_rep, LinkByUID):
         return gemd_object_rep
     elif isinstance(gemd_object_rep, (str, UUID)):
@@ -472,15 +616,17 @@
 
         scope = CITRINE_SCOPE
         id = dumped_data['uids'][scope]
         if self.dataset_id is None:
             raise RuntimeError("Must specify a dataset in order to update "
                                "a data model object with data validation.")
 
-        url = self._get_path(action=[scope, id, "async"])
+        url = self._get_path() + \
+            "/" + scope + "/" + id + "/async"
+
         response_json = self.session.put_resource(url, dumped_data, params={'dry_run': dry_run})
 
         job_id = response_json["job_id"]
 
         if wait_for_response:
             self.poll_async_update_job(job_id, timeout=timeout,
                                        polling_delay=polling_delay)
@@ -543,15 +689,16 @@
         Returns
         -------
         ResourceType
             An object with specified scope and uid
 
         """
         link = _make_link_by_uid(uid)
-        path = self._get_path(ignore_dataset=self.dataset_id is None, action=[link.scope, link.id])
+        path = self._get_path(ignore_dataset=self.dataset_id is None) \
+            + format_escaped_url("/{}/{}", link.scope, link.id)
         data = self.session.get_resource(path)
         return self.build(data)
 
     def list_by_name(self, name: str, *, exact: bool = False,
                      forward: bool = True, per_page: int = 100) -> Iterator[ResourceType]:
         """
         Get all objects with specified name in this dataset.
@@ -578,15 +725,15 @@
         """
         if self.dataset_id is None:
             raise RuntimeError("Must specify a dataset to filter by name.")
         params = {'dataset_id': str(self.dataset_id), 'name': name, 'exact': exact}
         raw_objects = self.session.cursor_paged_resource(
             self.session.get_resource,
             # "Ignoring" dataset because it is in the query params (and required)
-            self._get_path(ignore_dataset=True, action="filter-by-name"),
+            self._get_path(ignore_dataset=True) + "/filter-by-name",
             forward=forward,
             per_page=per_page,
             params=params)
         return (self.build(raw) for raw in raw_objects)
 
     def list_by_tag(self, tag: str, *, per_page: int = 100) -> Iterator[ResourceType]:
         """
@@ -634,15 +781,15 @@
             A representation of the object (Citrine id, LinkByUID, or the object itself)
         dry_run: bool
             Whether to actually delete the item or run a dry run of the delete operation.
             Dry run is intended to be used for validation. Default: false
 
         """
         link = _make_link_by_uid(uid)
-        path = self._get_path(action=[link.scope, link.id])
+        path = self._get_path() + format_escaped_url("/{}/{}", link.scope, link.id)
         params = {'dry_run': dry_run}
         self.session.delete_resource(path, params=params)
         return Response(status_code=200)  # delete succeeded
 
     def _get_relation(self, relation: str, uid: Union[UUID, str, LinkByUID, BaseEntity],
                       forward: bool = True, per_page: int = 100) -> Iterator[ResourceType]:
         """
```

### Comparing `citrine-2.24.1/src/citrine/resources/data_objects.py` & `citrine-2.8.0/src/citrine/resources/data_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,39 +3,31 @@
 from typing import Dict, Union, Optional, Iterator, List, TypeVar
 from uuid import uuid4
 
 from gemd.json import GEMDJson
 from gemd.util import recursive_foreach
 
 from citrine._utils.functions import get_object_id, replace_objects_with_links, scrub_none
-from citrine._serialization.properties import List as PropertyList
-from citrine._serialization.properties import String, Object
-from citrine._serialization.properties import Optional as PropertyOptional
-from gemd.entity.file_link import FileLink
 from citrine.exceptions import BadRequest
 from citrine.resources.api_error import ValidationError
 from citrine.resources.data_concepts import DataConcepts, DataConceptsCollection
 from citrine.resources.object_templates import ObjectTemplateResourceType
 from citrine.resources.process_template import ProcessTemplate
-from gemd.entity.object.base_object import BaseObject
 from gemd.entity.bounds.base_bounds import BaseBounds
 from gemd.entity.link_by_uid import LinkByUID
 from gemd.entity.template.attribute_template import AttributeTemplate
 
 
-class DataObject(DataConcepts, BaseObject, ABC):
+class DataObject(DataConcepts, ABC):
     """
     An abstract data object object.
 
     DataObject must be extended along with `Resource`
     """
 
-    notes = PropertyOptional(String(), 'notes')
-    file_links = PropertyOptional(PropertyList(Object(FileLink)), 'file_links', override=True)
-
 
 DataObjectResourceType = TypeVar("DataObjectResourceType", bound="DataObject")
 
 
 class DataObjectCollection(DataConceptsCollection[DataObjectResourceType], ABC):
     """A collection of one kind of data object object."""
 
@@ -80,15 +72,15 @@
         body = self._get_attribute_bounds_search_body(attribute_bounds)
         params = {}
         if self.dataset_id is not None:
             params['dataset_id'] = str(self.dataset_id)
         raw_objects = self.session.cursor_paged_resource(
             self.session.post_resource,
             # "Ignoring" dataset because it is in the query params (and required)
-            self._get_path(ignore_dataset=True, action="filter-by-attribute-bounds"),
+            self._get_path(ignore_dataset=True) + "/filter-by-attribute-bounds",
             json=body,
             forward=forward,
             per_page=per_page,
             params=params)
         return (self.build(raw) for raw in raw_objects)
 
     @staticmethod
@@ -120,15 +112,15 @@
 
         :param model: the data object to validate
         :param object_template: optional object template to validate against
         :param ingredient_process_template: optional process template to validate ingredient
          against. Ignored unless data object is an IngredientSpec or IngredientRun.
         :return: List[ValidationError] of validation errors encountered. Empty if successful.
         """
-        path = self._get_path(ignore_dataset=True, action="validate-templates")
+        path = self._get_path(ignore_dataset=True) + "/validate-templates"
 
         temp_scope = str(uuid4())
         GEMDJson(scope=temp_scope).dumps(model)  # This apparent no-op populates uids
         dumped_data = replace_objects_with_links(scrub_none(model.dump()))
         recursive_foreach(model, lambda x: x.uids.pop(temp_scope, None))  # Strip temp uids
 
         request_data = {"dataObject": dumped_data}
```

### Comparing `citrine-2.24.1/src/citrine/resources/data_version_update.py` & `citrine-2.8.0/src/citrine/resources/data_version_update.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/resources/dataset.py` & `citrine-2.8.0/src/citrine/resources/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from citrine._utils.functions import scrub_none
 from citrine.exceptions import NotFound
 from citrine.resources.api_error import ApiError
 from citrine.resources.condition_template import ConditionTemplateCollection
 from citrine.resources.data_concepts import DataConcepts
 from citrine.resources.delete import _poll_for_async_batch_delete_result
 from citrine.resources.file_link import FileCollection
-from citrine.resources.ingestion import IngestionCollection
 from citrine.resources.gemd_resource import GEMDResourceCollection
 from citrine.resources.ingredient_run import IngredientRunCollection
 from citrine.resources.ingredient_spec import IngredientSpecCollection
 from citrine.resources.material_run import MaterialRunCollection
 from citrine.resources.material_spec import MaterialSpecCollection
 from citrine.resources.material_template import MaterialTemplateCollection
 from citrine.resources.measurement_run import MeasurementRunCollection
@@ -88,18 +87,14 @@
     created_by = properties.Optional(properties.UUID(), 'created_by')
     updated_by = properties.Optional(properties.UUID(), 'updated_by')
     deleted_by = properties.Optional(properties.UUID(), 'deleted_by')
     create_time = properties.Optional(properties.Datetime(), 'create_time')
     update_time = properties.Optional(properties.Datetime(), 'update_time')
     delete_time = properties.Optional(properties.Datetime(), 'delete_time')
     public = properties.Optional(properties.Boolean(), 'public')
-    project_id = properties.Optional(properties.UUID(), 'project_id',
-                                     serializable=False, deserializable=False)
-    session = properties.Optional(properties.Object(Session), 'session',
-                                  serializable=False, deserializable=False)
 
     def __init__(self, name: str, *, summary: str,
                  description: str, unique_name: Optional[str] = None):
         self.name: str = name
         self.summary: str = summary
         self.description: str = description
         self.unique_name = unique_name
@@ -111,16 +106,14 @@
         self.created_by = None
         self.updated_by = None
         self.deleted_by = None
         self.create_time = None
         self.update_time = None
         self.delete_time = None
         self.public = None
-        self.project_id = None
-        self.session = None
 
     def __str__(self):
         return '<Dataset {!r}>'.format(self.name)
 
     @property
     def property_templates(self) -> PropertyTemplateCollection:
         """Return a resource representing all property templates in this dataset."""
@@ -197,19 +190,14 @@
         return GEMDResourceCollection(self.project_id, self.uid, self.session)
 
     @property
     def files(self) -> FileCollection:
         """Return a resource representing all files in the dataset."""
         return FileCollection(self.project_id, self.uid, self.session)
 
-    @property
-    def ingestions(self) -> IngestionCollection:
-        """Return a resource representing all files in the dataset."""
-        return IngestionCollection(self.project_id, self.uid, self.session)
-
     def register(self, model: DataConcepts, *, dry_run=False) -> DataConcepts:
         """Register a data model object to the appropriate collection."""
         return self.gemd._collection_for(model).register(model, dry_run=dry_run)
 
     def register_all(self,
                      models: Iterable[DataConcepts],
                      *,
@@ -281,32 +269,25 @@
         else:
             collection = self.gemd
         return collection.delete(uid, dry_run=dry_run)
 
     def delete_contents(
             self,
             *,
-            prompt_to_confirm: bool = True,
-            remove_templates: bool = True,
+            prompt_to_confirm: bool,
             timeout: float = 2 * 60,
             polling_delay: float = 1.0
     ):
         """
         Delete all the GEMD objects from within a single Dataset.
 
         Parameters
         ----------
         prompt_to_confirm: bool
-            If True, prompt for user confirmation before triggering delete.  Included
-            so that a script can skip confirmation if desired, but a user will not
-            accidentally stumble in a notebook or other REPL environment.  Default: True
-        remove_templates: bool
-            If False, templates will not be deleted along with other contents of the
-            dataset.  If true, all GEMD entities including templates will be deleted.
-            Default: True
+            If True, prompt for user confirmation before triggering delete.
         timeout: float
             Amount of time to wait on the job (in seconds) before giving up.
             Note that this number has no effect on the underlying job itself,
             which can also time out server-side.
         polling_delay: float
             How long to delay between each polling retry attempt.
         Returns
@@ -329,16 +310,15 @@
             if user_response.lower() in {'y', 'yes'}:
                 break  # return to main flow
             elif user_response.lower() in {'n', 'no'}:
                 raise RuntimeError("delete_contents was invoked unintentionally")
             else:
                 print(f'"{user_response}" is not a valid response')
 
-        params = {"remove_templates": remove_templates}
-        response = self.session.delete_resource(path, params=params)
+        response = self.session.delete_resource(path)
         job_id = response["job_id"]
 
         return _poll_for_async_batch_delete_result(self.project_id, self.session, job_id, timeout,
                                                    polling_delay)
 
     def gemd_batch_delete(
             self,
@@ -369,22 +349,14 @@
         ----------
         id_list: List[Union[LinkByUID, UUID, str, BaseEntity]]
             A list of the IDs of data objects to be removed. They can be passed
             as a LinkByUID tuple, a UUID, a string, or the object itself. A UUID
             or string is assumed to be a Citrine ID, whereas a LinkByUID or
             BaseEntity can also be used to provide an external ID.
 
-        timeout: float
-            Amount of time to wait on the job (in seconds) before giving up. Defaults
-            to 2 minutes. Note that this number has no effect on the underlying job
-            itself, which can also time out server-side.
-
-        polling_delay: float
-            How long to delay between each polling retry attempt.
-
         Returns
         -------
         List[Tuple[LinkByUID, ApiError]]
             A list of (LinkByUID, api_error) for each failure to delete an object.
             Note that this method doesn't raise an exception if an object fails to be
             deleted.
 
@@ -503,15 +475,15 @@
         """
         return super().list(per_page=per_page)
 
     def get_by_unique_name(self, unique_name: str) -> Dataset:
         """Get a Dataset with the given unique name."""
         if unique_name is None:
             raise ValueError("You must supply a unique_name")
-        path = self._get_path(query_terms={"unique_name": unique_name})
+        path = self._get_path() + "?unique_name=" + unique_name
         data = self.session.get_resource(path)
 
         if len(data) == 1:
             return self.build(data[0])
         elif len(data) > 1:
             raise RuntimeError("Received multiple results when requesting a unique dataset")
         else:
```

### Comparing `citrine-2.24.1/src/citrine/resources/delete.py` & `citrine-2.8.0/src/citrine/resources/delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,9 +118,9 @@
         Note that this method doesn't raise an exception if an object fails to be
         deleted.
 
     """
     response = _poll_for_job_completion(session, project_id, job_id, timeout=timeout,
                                         polling_delay=polling_delay)
 
-    return [(LinkByUID(f['id']['scope'], f['id']['id']), ApiError.build(f['cause']))
+    return [(LinkByUID(f['id']['scope'], f['id']['id']), ApiError.from_dict(f['cause']))
             for f in json.loads(response.output.get('failures', '[]'))]
```

### Comparing `citrine-2.24.1/src/citrine/resources/descriptors.py` & `citrine-2.8.0/src/citrine/resources/descriptors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,49 @@
-from typing import List, Union
+from typing import List
 from uuid import UUID
 
 from citrine._session import Session
 from citrine._utils.functions import format_escaped_url
 from citrine.informatics.data_sources import DataSource
 from citrine.informatics.descriptors import Descriptor
-from citrine.informatics.predictors import PredictorNode, GraphPredictor
+from citrine.informatics.predictors import Predictor
 
 
 # Not a full Collection since CRUD operations are not valid for Descriptors
 class DescriptorMethods:
     """A set of methods returning descriptors which require connection to the backend."""
 
     def __init__(self, project_id: UUID, session: Session):
         self.project_id = project_id
         self.session: Session = session
 
-    def from_predictor_responses(self, *, predictor: Union[GraphPredictor, PredictorNode],
+    def from_predictor_responses(self, *, predictor: Predictor,
                                  inputs: List[Descriptor]) -> List[Descriptor]:
         """
         Get responses for a predictor, given an input space.
 
         Parameters
         ----------
-        predictor : Union[Predictor, PredictorNode]
-            Either a single predictor node or full predictor
-             whose available responses are to be computed.
+        predictor : Predictor
+            The predictor whose available responses are to be computed.
         inputs : List[Descriptor]
             The input space to the predictor.
 
         Returns
         -------
         List[Descriptor]
             The computable responses of the predictor given the provided input space (as
             descriptors).
 
         """
-        if isinstance(predictor, GraphPredictor):
-            predictor_data = predictor.dump()["instance"]
-        else:
-            predictor_data = predictor.dump()
-
         response = self.session.post_resource(
             path=format_escaped_url('/projects/{}/material-descriptors/predictor-responses',
                                     self.project_id),
             json={
-                'predictor': predictor_data,
+                'predictor': predictor.dump()['instance'],
                 'inputs': [i.dump() for i in inputs]
             }
         )
         return [Descriptor.build(r) for r in response['responses']]
 
     def descriptors_from_data_source(self, *, data_source: DataSource) -> List[Descriptor]:
         """
```

### Comparing `citrine-2.24.1/src/citrine/resources/design_execution.py` & `citrine-2.8.0/src/citrine/resources/design_execution.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,68 +1,59 @@
 """Resources that represent both individual and collections of design workflow executions."""
+import sys
 from typing import Optional, Union, Iterator
 from uuid import UUID
 
 from citrine._rest.collection import Collection
-from citrine._utils.functions import MigratedClassMeta
+from citrine._utils.functions import shadow_classes_in_module
 from citrine._session import Session
-from citrine.informatics import executions
+import citrine.informatics.executions.design_execution
+from citrine.informatics.executions import DesignExecution
 from citrine.informatics.scores import Score
 from citrine.resources.response import Response
 
 
-class DesignExecution(executions.DesignExecution,
-                      deprecated_in="2.22.1",
-                      removed_in="3.0.0",
-                      metaclass=MigratedClassMeta):
-    """The execution of a DesignWorkflow.
-
-    Possible statuses are INPROGRESS, SUCCEEDED, and FAILED.
-    Design executions also have a ``status_description`` field with more information.
-
-    DesignExecution should be imported from citrine.informatics.executions.
-
-    """
+shadow_classes_in_module(citrine.informatics.executions.design_execution, sys.modules[__name__])
 
 
 class DesignExecutionCollection(Collection["DesignExecution"]):
     """A collection of DesignExecutions."""
 
     _path_template = '/projects/{project_id}/design-workflows/{workflow_id}/executions'  # noqa
     _individual_key = None
     _collection_key = 'response'
-    _resource = executions.DesignExecution
+    _resource = DesignExecution
 
     def __init__(self,
                  project_id: UUID,
                  session: Session,
                  workflow_id: Optional[UUID] = None):
         self.project_id: UUID = project_id
         self.session: Session = session
         self.workflow_id: UUID = workflow_id
 
-    def build(self, data: dict) -> executions.DesignExecution:
+    def build(self, data: dict) -> DesignExecution:
         """Build an individual DesignWorkflowExecution."""
-        execution = executions.DesignExecution.build(data)
+        execution = DesignExecution.build(data)
         execution._session = self.session
         execution.project_id = self.project_id
         return execution
 
     def trigger(self, execution_input: Score, *, max_candidates: Optional[int] = None):
         """Trigger a Design Workflow execution given a score and a maximum number of candidates."""
         path = self._get_path()
         json = {'score': execution_input.dump(), "max_candidates": max_candidates}
         data = self.session.post_resource(path, json)
         return self.build(data)
 
-    def register(self, model: executions.DesignExecution) -> executions.DesignExecution:
+    def register(self, model: DesignExecution) -> DesignExecution:
         """Cannot register an execution."""
         raise NotImplementedError("Cannot register a DesignExecution.")
 
-    def update(self, model: executions.DesignExecution) -> executions.DesignExecution:
+    def update(self, model: DesignExecution) -> DesignExecution:
         """Cannot update an execution."""
         raise NotImplementedError("Cannot update a DesignExecution.")
 
     def archive(self, uid: Union[UUID, str]):
         """Archive a Design Workflow execution.
 
         Parameters
@@ -82,15 +73,15 @@
         uid: UUID
             Unique identifier of the execution to restore
 
         """
         raise NotImplementedError(
             "Design Executions cannot be restored")
 
-    def list(self, *, per_page: int = 100) -> Iterator[executions.DesignExecution]:
+    def list(self, *, per_page: int = 100) -> Iterator[DesignExecution]:
         """
         Paginate over the elements of the collection.
 
         Leaving page and per_page as default values will yield all elements in the
         collection, paginating over all available pages.
 
         Parameters
```

### Comparing `citrine-2.24.1/src/citrine/resources/design_space.py` & `citrine-2.8.0/src/citrine/resources/design_space.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Resources that represent collections of design spaces."""
-import warnings
-from typing import List, Optional, TypeVar, Union
+from typing import Optional, TypeVar, Union
 from uuid import UUID
 
 from citrine._session import Session
 from citrine.resources.module import AbstractModuleCollection
 from citrine.informatics.design_spaces import DesignSpace, EnumeratedDesignSpace
 
 CreationType = TypeVar('CreationType', bound=DesignSpace)
@@ -51,41 +50,23 @@
             if width * length > self._enumerated_cell_limit:
                 msg = "EnumeratedDesignSpace only supports up to {} descriptor-values, " \
                       "but {} were given. Please reduce the number of descriptors or candidates " \
                       "in this EnumeratedDesignSpace"
                 raise ValueError(msg.format(self._enumerated_cell_limit, width * length))
         return
 
-    def _hydrate_design_space(self, model: DesignSpace) -> List[DesignSpace]:
-        if model.typ != "ProductDesignSpace":
-            return model
-
-        subspaces = []
-        for subspace in model.subspaces:
-            if isinstance(subspace, (str, UUID)):
-                warnings.warn("Support for UUIDs in subspaces is deprecated as of 2.16.0, and "
-                              "will be dropped in 3.0. Please use DesignSpace objects instead.",
-                              DeprecationWarning)
-                subspaces.append(self.get(subspace))
-            else:
-                subspaces.append(subspace)
-        model.subspaces = subspaces
-        return model
-
     def register(self, model: DesignSpace) -> DesignSpace:
         """Create a new design space."""
         self._validate_write_request(model)
-        hydrated_model = self._hydrate_design_space(model)
-        return AbstractModuleCollection.register(self, hydrated_model)
+        return AbstractModuleCollection.register(self, model)
 
     def update(self, model: DesignSpace) -> DesignSpace:
         """Update an existing design space by uid."""
         self._validate_write_request(model)
-        hydrated_model = self._hydrate_design_space(model)
-        return AbstractModuleCollection.update(self, hydrated_model)
+        return AbstractModuleCollection.update(self, model)
 
     def create_default(self,
                        *,
                        predictor_id: UUID,
                        predictor_version: Optional[Union[int, str]] = None,
                        include_ingredient_fraction_constraints: bool = False,
                        include_label_fraction_constraints: bool = False,
```

### Comparing `citrine-2.24.1/src/citrine/resources/experiment_datasource.py` & `citrine-2.8.0/src/citrine/resources/experiment_datasource.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/resources/file_link.py` & `citrine-2.8.0/src/citrine/resources/file_link.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """A collection of FileLink objects."""
 from deprecation import deprecated
 import mimetypes
 import os
 from pathlib import Path
+from enum import Enum
 from logging import getLogger
-from tempfile import TemporaryDirectory
-from typing import Optional, Tuple, Union, List, Dict, Iterable, Sequence
-from urllib.parse import urlparse, unquote_plus
+from typing import Optional, Tuple, Union, List, Dict
+from urllib.parse import urlparse, quote
 from uuid import UUID
 
 import requests
 from boto3 import client as boto3_client
 from boto3.session import Config
 from botocore.exceptions import ClientError
 from citrine._rest.collection import Collection
-from citrine._rest.resource import GEMDResource
+from citrine._rest.resource import Resource
 from citrine._serialization import properties
 from citrine._serialization.serializable import Serializable
 from citrine._session import Session
 from citrine._utils.functions import rewrite_s3_links_locally
-from citrine._utils.functions import write_file_locally
+from citrine._utils.functions import write_file_locally, format_escaped_url
 
 from citrine.jobs.job import JobSubmissionResponse, _poll_for_job_completion
 from citrine.resources.response import Response
-from gemd.entity.dict_serializable import DictSerializableMeta
 from gemd.entity.bounds.base_bounds import BaseBounds
 from gemd.entity.file_link import FileLink as GEMDFileLink
 from gemd.enumeration.base_enumeration import BaseEnumeration
 
 logger = getLogger(__name__)
 
 
@@ -63,15 +62,15 @@
         self.aws_session_token = ''
         self.s3_version = ''
         self.s3_endpoint_url = None
         self.s3_use_ssl = True
         self.s3_addressing_style = 'auto'
 
 
-class FileProcessingType(BaseEnumeration):
+class FileProcessingType(Enum):
     """The supported File Processing Types."""
 
     VALIDATE_CSV = "VALIDATE_CSV"
 
 
 class FileProcessingData:
     """The base class of all File Processing related data implementations."""
@@ -96,15 +95,15 @@
         self.exact_range_bounds = exact_range_bounds
 
 
 class CsvValidationData(FileProcessingData, Serializable):
     """The resulting data from the processed CSV file."""
 
     columns = properties.Optional(properties.List(properties.Object(CsvColumnInfo)),
-                                  'columns')
+                                  'columns', override=True)
     """:Optional[List[CsvColumnInfo]]: all of the columns in the CSV"""
     record_count = properties.Integer('record_count')
     """:int: the number of rows in the CSV"""
 
     def __init__(self, columns: List[CsvColumnInfo],
                  record_count: int):  # pragma: no cover
         self.columns = columns
@@ -114,141 +113,64 @@
 class FileProcessingResult:
     """
     The results of a successful file processing operation.
 
     The type of the actual data depends on the specific processing type.
     """
 
-    def __init__(self,
-                 processing_type: FileProcessingType,
-                 data: Union[Dict, FileProcessingData]):
+    def __init__(self, processing_type: FileProcessingType, data: Union[Dict,
+                                                                        FileProcessingData]):
         self.processing_type = processing_type
         self.data = data
 
 
-class FileLinkMeta(DictSerializableMeta):
-    """Metaclass for FileLink deserialization."""
-
-    def __init__(cls, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        cls.typ = properties.String('type', default="file_link", deserializable=False)
-
-
-def _get_ids_from_url(url: str) -> Tuple[Optional[UUID], Optional[UUID]]:
-    """Attempt to extract file_id and version_id from a URL."""
-    parsed = urlparse(url)
-    if len(parsed.query) > 0 or len(parsed.fragment) > 0:
-        # Illegal modifiers
-        return None, None
-    split_path = urlparse(url).path.split('/')
-    if len(split_path) >= 4 and split_path[-4] == 'files' and split_path[-2] == 'versions':
-        file_id = split_path[-3]
-        version_id = split_path[-1]
-    elif len(split_path) >= 2 and split_path[-2] == 'files':
-        file_id = split_path[-1]
-        version_id = None
-    else:
-        file_id, version_id = None, None
-
-    if file_id is not None:
-        try:
-            file_id = UUID(file_id)
-            if version_id is not None:
-                version_id = UUID(version_id)
-        except ValueError:
-            return None, None
-    return file_id, version_id
-
-
-class FileLink(
-    GEMDResource['FileLink'],
-    GEMDFileLink,
-    metaclass=FileLinkMeta,
-    typ=GEMDFileLink.typ
-):
+class FileLink(Resource['FileLink'], GEMDFileLink):
     """
     Resource that stores the name and url of an external file.
 
     Parameters
     ----------
     filename: str
         The name of the file.
     url: str
         URL that can be used to access the file.
 
-    Attributes
-    ----------
-    uid: UUID
-        Unique uuid4 identifier of this file; consistent across versions.
-    version: UUID
-        Unique uuid4 identifier of this version of this file
-    version_number: Integer
-        How many times this file has been uploaded;
-        files are the "same" if the share a filename and dataset
-    created_time: Datetime
-        Time the file was created on platform.
-    created_by: UUID
-        Unique uuid4 identifier of this User who loaded this file
-    mime_type: String
-        Encoded string representing the type of the file (IETF RFC 2045)
-    size: Integer
-        Size in bytes of the file
-    description: String
-        A human-readable description of the file
-
     """
 
     # NOTE: skipping the "metadata" field since it appears to be unused
     # NOTE: skipping the "versioned_url" field since it is redundant
     # NOTE: skipping the "unversioned_url" field since it is redundant
-    filename = properties.String('filename')
-    url = properties.String('url')
+    filename = properties.String('filename', override=True)
+    url = properties.String('url', override=True)
     uid = properties.Optional(properties.UUID, 'id', serializable=False)
     version = properties.Optional(properties.UUID, 'version', serializable=False)
     created_time = properties.Optional(properties.Datetime, 'created_time', serializable=False)
     created_by = properties.Optional(properties.UUID, 'created_by', serializable=False)
     mime_type = properties.Optional(properties.String, 'mime_type', serializable=False)
     size = properties.Optional(properties.Integer, 'size', serializable=False)
     description = properties.Optional(properties.String, 'description', serializable=False)
     version_number = properties.Optional(properties.Integer, 'version_number', serializable=False)
+    typ = properties.String('type', default="file_link", deserializable=False)
 
     def __init__(self, filename: str, url: str):
         GEMDFileLink.__init__(self, filename, url)
-        uid, version = _get_ids_from_url(url)
-        if uid is not None:
-            self.uid = uid
-        if version is not None:
-            self.version = version
-        self.typ = FileLink.typ
-
-    @staticmethod
-    def from_path(path: Union[str, Path]) -> "FileLink":
-        """Construct a FileLink from a local Path."""
-        path = Path(path)  # In case it was a string
-        return FileLink(filename=path.name, url=path.expanduser().absolute().as_uri())
+        self.typ = GEMDFileLink.typ
 
     @property
     def name(self):
         """Attribute name is an alias for filename."""
         return self.filename
 
-    @classmethod
-    def _pre_build(cls, data: dict) -> dict:
-        """Run data modification before building."""
-        if 'url' in data and 'id' not in data:
-            uid, version = _get_ids_from_url(data['url'])
-            if uid is not None:
-                data['id'] = str(uid)
-            if version is not None:
-                data['version'] = str(version)
-        return data
-
     def __str__(self):
         return f'<File link {self.filename!r}>'
 
+    def as_dict(self) -> dict:
+        """Dump to a dictionary (useful for interoperability with gemd)."""
+        return self.dump()
+
 
 class FileCollection(Collection[FileLink]):
     """Represents the collection of all file links associated with a dataset."""
 
     _path_template = 'projects/{project_id}/datasets/{dataset_id}/files'
     _collection_key = 'files'
     _resource = FileLink
@@ -256,46 +178,81 @@
     def __init__(self, project_id: UUID, dataset_id: UUID, session: Session):
         self.project_id = project_id
         self.dataset_id = dataset_id
         self.session = session
 
     def _get_path(self,
                   uid: Optional[Union[UUID, str]] = None,
-                  *,
                   ignore_dataset: Optional[bool] = False,
+                  *,
                   version: Union[str, UUID] = None,
-                  action: Union[str, Sequence[str]] = [],
-                  query_terms: Dict[str, str] = {},) -> str:
+                  action: str = None) -> str:
         """Build the path for taking an action with a particular file version."""
+        base = urlparse(super()._get_path(uid=uid, ignore_dataset=ignore_dataset))
+        new_path = base.path.split('/')
         if version is not None:
-            action = ['versions', version] + ([action] if isinstance(action, str) else action)
-        return super()._get_path(uid=uid, ignore_dataset=ignore_dataset, action=action)
+            new_path.extend([quote(x) for x in ('versions', str(version))])
+        if action is not None:
+            new_path.append(quote(action))
+
+        return base._replace(path='/'.join(new_path)).geturl()
+
+    @staticmethod
+    def _get_ids_from_url(url: str) -> Tuple[Optional[UUID], Optional[UUID]]:
+        """Attempt to extract file_id and version_id from a URL."""
+        parsed = urlparse(url)
+        if len(parsed.query) > 0 or len(parsed.fragment) > 0:
+            # Illegal modifiers
+            return None, None
+        split_path = urlparse(url).path.split('/')
+        if len(split_path) >= 4 and split_path[-4] == 'files' and split_path[-2] == 'versions':
+            file_id = split_path[-3]
+            version_id = split_path[-1]
+        elif len(split_path) >= 2 and split_path[-2] == 'files':
+            file_id = split_path[-1]
+            version_id = None
+        else:
+            file_id, version_id = None, None
+
+        if file_id is not None:
+            try:
+                file_id = UUID(file_id)
+                if version_id is not None:
+                    version_id = UUID(version_id)
+            except ValueError:
+                return None, None
+        return file_id, version_id
 
     def _get_path_from_file_link(self, file_link: FileLink,
                                  *,
                                  action: str = None) -> str:
         """Build the platform path for taking an action with a particular file link."""
-        if not self._is_on_platform_url(file_link.url) or file_link.uid is None:
-            raise ValueError("FileLink did not contain a Citrine platform file URL.")
-        return self._get_path(uid=file_link.uid, version=file_link.version, action=action)
+        # Use this session's project/dataset credentials and the URLs file / version
+        if file_link.uid is not None:
+            file_id = file_link.uid
+            version_id = file_link.version
+        else:
+            file_id, version_id = self._get_ids_from_url(file_link.url)
+            if file_id is None:
+                raise ValueError("FileLink did not contain a Citrine platform file URL.")
+        return self._get_path(uid=file_id, version=version_id, action=action)
 
     def build(self, data: dict) -> FileLink:
         """Build an instance of FileLink."""
         # Use this chance to construct a URL from platform metadata
         if 'url' not in data:
-            data['url'] = self._get_path(uid=data['id'], version=data['version'])
-
+            data['url'] = self._get_path(uid=data["id"], version=data["version"])
         return FileLink.build(data)
 
     def get(self,
             uid: Union[UUID, str],
             *,
             version: Optional[Union[UUID, str, int]] = None) -> FileLink:
         """
-        Retrieve an on-platform FileLink from its filename or file uuid.
+        Get an element of the collection by its id.
 
         Parameters
         ----------
         uid: Union[UUID, str]
             A representation of the FileLink (Citrine id or file name)
         version: Optional[UUID, str, int]
             The version, as a UUID or str(UUID) of the version_id or an int or
@@ -398,15 +355,15 @@
         -------
         _Uploader
             Holds the parameters returned by the upload request, for later use.
             These must include region_name, aws_access_key_id, aws_secret_access_key,
             aws_session_token, bucket, object_key, & upload_id.
 
         """
-        path = self._get_path(action="uploads")
+        path = self._get_path() + "/uploads"
         mime_type = self._mime_type(file_path)
         file_size = file_path.stat().st_size
         assert isinstance(file_size, int)
         upload_json = {
             'files': [
                 {
                     'file_name': dest_name,
@@ -462,15 +419,15 @@
 
         Returns
         -------
         FileLink
             All the data needed for a file.
 
         """
-        path = self._get_path(action="search")
+        path = self._get_path() + "/search"
 
         search_json = {
             'fileSearchFilter':
                 {
                     'type': SearchFileFilterTypeEnum.NAME_SEARCH.value,
                     'datasetId': str(dset_id),
                     'fileName': file_name,
@@ -495,15 +452,15 @@
 
         Returns
         -------
         FileLink
             All the data needed for a file.
 
         """
-        path = self._get_path(action="search")
+        path = self._get_path() + "/search"
 
         search_json = {
             'fileSearchFilter': {
                 'type': SearchFileFilterTypeEnum.VERSION_ID_SEARCH.value,
                 'fileVersionUuid': str(file_version_id)
             }
         }
@@ -534,15 +491,15 @@
 
         Returns
         -------
         FileLink
             All the data needed for a file.
 
         """
-        path = self._get_path(action="search")
+        path = self._get_path() + "/search"
 
         search_json = {
             'fileSearchFilter': {
                 'type': SearchFileFilterTypeEnum.DATASET_FILE_ID_SEARCH.value,
                 'datasetId': str(dset_id),
                 'datasetFileId': str(dataset_file_id),
                 'fileVersionNumber': file_version_number
@@ -551,15 +508,15 @@
 
         data = self.session.post_resource(path=path, json=search_json)
 
         return self.build(data['files'][0])
 
     @staticmethod
     def _mime_type(file_path: Path):
-        # This string coercion is for supporting pathlib.Path objects in python < 3.8
+        # This string coercion is for supporting pathlib.Path objects in python 3.6
         mime_type = mimetypes.guess_type(str(file_path))[0]
         if mime_type is None:
             mime_type = "application/octet-stream"
         return mime_type
 
     @staticmethod
     def _upload_file(file_path: Path, uploader: _Uploader):
@@ -622,16 +579,16 @@
 
         Returns
         -------
         FileLink
             The filename and url of the uploaded object.
 
         """
-        url = self._get_path(action=["uploads", uploader.upload_id, "complete"])
-        complete_response = self.session.put_resource(path=url,
+        path = self._get_path() + format_escaped_url("/uploads/{}/complete", uploader.upload_id)
+        complete_response = self.session.put_resource(path=path,
                                                       json={'s3_version': uploader.s3_version})
 
         try:
             file_id = complete_response['file_info']['file_id']
             version_id = complete_response['file_info']['version']
         except KeyError:
             raise RuntimeError("Upload completion response is missing some "
@@ -664,15 +621,15 @@
             final_path = local_path / file_link.filename
         else:
             final_path = local_path
 
         response_content = self.read(file_link=file_link)
         write_file_locally(response_content, final_path)
 
-    def read(self, *, file_link: Union[str, UUID, FileLink]) -> bytes:
+    def read(self, *, file_link: Union[str, UUID, FileLink]):
         """
         Read the file associated with a given FileLink.
 
         Parameters
         ----------
         file_link: FileLink, str, UUID
             Resource referencing the file.
@@ -681,34 +638,32 @@
         -------
         I/O stream
             The contents of the file.
 
         """
         file_link = self._resolve_file_link(file_link)
 
-        if self._is_local_url(file_link.url):  # Read the local file
-            path = Path(unquote_plus(urlparse(file_link.url).path))
-            return path.read_bytes()
-
         if self._is_external_url(file_link.url):  # Pull it from where ever it lives
             final_url = file_link.url
-        else:
+        elif self._validate_local_url(file_link.url):
             # The "/content-link" route returns a pre-signed url to download the file.
             content_link = self._get_path_from_file_link(file_link, action='content-link')
             content_link_response = self.session.get_resource(content_link)
             pre_signed_url = content_link_response['pre_signed_read_link']
             final_url = rewrite_s3_links_locally(pre_signed_url, self.session.s3_endpoint_url)
+        else:  # Unrecognized
+            raise ValueError(f"URL was malformed for a local file resource ({file_link.url}).")
 
         download_response = requests.get(final_url)
         return download_response.content
 
     @deprecated(deprecated_in="2.4.0",
                 removed_in="3.0.0",
                 details="The process file protocol is deprecated "
-                        "in favor of ingest()")
+                        "in favor of GUI-based ingest routes")
     def process(self, *, file_link: Union[FileLink, str, UUID],
                 processing_type: FileProcessingType,
                 wait_for_response: bool = True,
                 timeout: float = 2 * 60,
                 polling_delay: float = 1.0) -> Union[JobSubmissionResponse,
                                                      Dict[FileProcessingType,
                                                           FileProcessingResult]]:
@@ -731,18 +686,18 @@
 
         Returns
         -------
         JobSubmissionResponse
             A JobSubmissionResponse which can be used to poll for the result.
 
         """
-        if self._is_external_url(file_link.url):
+        file_link = self._resolve_file_link(file_link)
+        if not self._validate_local_url(file_link.url):
             raise ValueError(f"Only on-platform resources can be processed. "
                              f"Passed URL {file_link.url}.")
-        file_link = self._resolve_file_link(file_link)
 
         params = {"processing_type": processing_type.value}
         response = self.session.put_resource(
             self._get_path_from_file_link(file_link, action="processed"),
             json={},
             params=params
         )
@@ -756,15 +711,15 @@
                                                  polling_delay=polling_delay)
         else:
             return job
 
     @deprecated(deprecated_in="2.4.0",
                 removed_in="3.0.0",
                 details="The process file protocol is deprecated "
-                        "in favor of ingest()")
+                        "in favor of GUI-based ingest routes")
     def poll_file_processing_job(self, *, file_link: FileLink,
                                  processing_type: FileProcessingType,
                                  job_id: UUID,
                                  timeout: float = 2 * 60,
                                  polling_delay: float = 1.0) -> Dict[FileProcessingType,
                                                                      FileProcessingResult]:
         """
@@ -796,15 +751,15 @@
                                  polling_delay=polling_delay)
 
         return self.file_processing_result(file_link=file_link, processing_types=[processing_type])
 
     @deprecated(deprecated_in="2.4.0",
                 removed_in="3.0.0",
                 details="The process file protocol is deprecated "
-                        "in favor of ingest()")
+                        "in favor of GUI-based ingest routes")
     def file_processing_result(self, *,
                                file_link: FileLink,
                                processing_types: List[FileProcessingType]) -> \
             Dict[FileProcessingType, FileProcessingResult]:
         """
         Return the file processing result for the given file link and processing type.
 
@@ -838,124 +793,51 @@
                 data = CsvValidationData.build(data)
 
             result = FileProcessingResult(processing_type, data)
             results[processing_type] = result
 
         return results
 
-    def ingest(self,
-               files: Iterable[FileLink],
-               *,
-               upload: bool = False,
-               raise_errors: bool = True,
-               build_table: bool = False,
-               delete_dataset_contents: bool = False,
-               delete_templates: bool = True,
-               ) -> "IngestionStatus":  # noqa: F821
-        """
-        [ALPHA] Ingest a set of CSVs and/or Excel Workbooks formatted per the gemd-ingest protocol.
-
-        Parameters
-        ----------
-        files: List[FileLink]
-            A list of files from which GEMD objects should be built
-        upload: bool
-            If the files are off-platform references, upload them first.  Defaults to False,
-            in which case an off-platform resource raises an error.
-        raise_errors: bool
-            Whether ingestion errors raise exceptions (vs. simply reported in the results).
-            Default: True
-        build_table: bool
-            Whether to trigger a regeneration of the table config and building the table
-            after ingestion.  Default: False
-        delete_dataset_contents: bool
-            Whether to delete old objects prior to creating new ones.  Default: False
-        delete_templates: bool
-            Whether to delete old templates if deleting old objects.  Default: True
-
-        Returns
-        ----------
-        IngestionStatus
-            The result of the ingestion operation.
-
-        """
-        from citrine.resources.ingestion import IngestionCollection
-
-        targets = [self._resolve_file_link(f) for f in files]
-        offplatform = [f for f in targets if not self._is_on_platform_url(f.url)]
-        if upload:
-            with TemporaryDirectory() as downloads:
-                paths = [Path(downloads) / f.filename for f in offplatform]
-                for file_link, path in zip(offplatform, paths):
-                    self.download(file_link=file_link, local_path=path)
-                onplatform = [self.upload(file_path=p) for p in paths]
-            targets = [f for f in targets if self._is_on_platform_url(f.url)] + onplatform
-        elif len(offplatform) > 0:
-            raise ValueError(f"All files must be on-platform to load them.  "
-                             f"The following are not: {offplatform}")
-
-        ingestion_collection = IngestionCollection(project_id=self.project_id,
-                                                   dataset_id=self.dataset_id,
-                                                   session=self.session)
-        ingestion = ingestion_collection.build_from_file_links(targets)
-        return ingestion.build_objects(
-            raise_errors=raise_errors,
-            build_table=build_table,
-            delete_dataset_contents=delete_dataset_contents,
-            delete_templates=delete_templates
-        )
-
     def delete(self, file_link: FileLink):
         """
         Delete the file associated with a given FileLink from the database.
 
         Parameters
         ----------
         file_link: FileLink
             Resource referencing the external file.
 
         """
-        if not self._is_on_platform_url(file_link.url):
-            raise ValueError(f"Only platform resources can be deleted; passed URL {file_link.url}")
-        file_id = _get_ids_from_url(file_link.url)[0]
+        if self._is_external_url(file_link.url):
+            raise ValueError(f"Only local resources can be deleted; passed URL {file_link.url}")
+        file_id = self._get_ids_from_url(file_link.url)[0]
         if file_id is None:
             raise ValueError(f"URL was malformed for local resources; passed URL {file_link.url}")
         data = self.session.delete_resource(self._get_path(file_id))
         return Response(body=data)
 
     def _resolve_file_link(self, identifier: Union[str, UUID, FileLink]) -> FileLink:
         """Generate the FileLink object referenced by the passed argument."""
-        if isinstance(identifier, GEMDFileLink):
-            if not isinstance(identifier, FileLink):  # Up-convert type with existing info
-                update = FileLink(filename=identifier.filename, url=identifier.url)
-
-                if self._is_on_platform_url(update.url):
-                    if update.uid is None:
-                        raise ValueError(f"URL was malformed for platform resources; "
-                                         f"passed URL {update.url}")
-                    else:  # Validate that it's a real record
-                        update = self.get(uid=update.uid, version=update.version)
-                        if update.filename != identifier.filename:
-                            raise ValueError(
-                                f"Name mismatch between link ({identifier.filename}) "
-                                f"and platform ({update.filename})"
-                            )
-                    identifier = update
-
-            return identifier  # Passthrough since it's as full as it can get
-        elif isinstance(identifier, str):
-            if self._is_on_platform_url(identifier):  # It's either a filename or URL
-                file_id, version_id = _get_ids_from_url(identifier)
-                if file_id is None:  # Try it as a name or a stand-alone UID
-                    return self.get(identifier)
-                else:  # We got a file UID (and possibly a version UID) from a URL
-                    return self.get(uid=file_id, version=version_id)
-            else:  # Assume it's an absolute URL
-                filename = urlparse(identifier).path.split('/')[-1]
-                return FileLink(filename=filename, url=identifier)
+        if isinstance(identifier, FileLink):  # Passthrough for convenience
+            return identifier
+        elif isinstance(identifier, str) and self._is_external_url(identifier):
+            # Assume it's an absolute URL
+            filename = urlparse(identifier).path.split('/')[-1]
+            file_dict = {
+                'url': identifier,
+                'filename': filename,
+                'type': GEMDFileLink.typ
+            }
+            return FileLink.build(file_dict)
+        elif isinstance(identifier, str):  # It's either a filename or URL
+            file_id, version_id = self._get_ids_from_url(identifier)
+            if file_id is None:  # Try it as a name or a stand-alone UID
+                return self.get(identifier)
+            else:  # We got a file UID (and possibly a version UID) from a URL
+                return self.get(uid=file_id, version=version_id)
         elif isinstance(identifier, UUID):  # File UID
             return self.get(uid=identifier)
         else:
             raise TypeError(f"File Link can only be resolved from str, or UUID."
                             f"Instead got {type(identifier)} {identifier}.")
 
     def _is_external_url(self, url: str):
@@ -963,16 +845,13 @@
         parsed = urlparse(url)
         if len(parsed.scheme) == 0 or len(parsed.netloc) == 0:
             # Relative
             return False
 
         return urlparse(self._get_path()).netloc != parsed.netloc
 
-    @staticmethod
-    def _is_local_url(url: str):
-        """Check if the URL is for a local file."""
-        parsed = urlparse(url)
-        return parsed.scheme == "file"
+    def _validate_local_url(self, url):
+        """Verify link is well formed."""
+        if self._is_external_url(url):
+            return False
 
-    def _is_on_platform_url(self, url: str):
-        """Check if the URL is for an on-platform record."""
-        return not self._is_external_url(url) and not self._is_local_url(url)
+        return self._get_ids_from_url(url)[1] is not None  # Implies file_id is None, too
```

### Comparing `citrine-2.24.1/src/citrine/resources/gemd_resource.py` & `citrine-2.8.0/src/citrine/resources/gemd_resource.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/resources/gemtables.py` & `citrine-2.8.0/src/citrine/resources/gemtables.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     def __init__(self, project_id: UUID, session: Session):
         self.project_id = project_id
         self.session: Session = session
 
     def get(self, uid: Union[UUID, str], *, version: Optional[int] = None) -> GemTable:
         """Get a Table's metadata. If no version is specified, get the most recent version."""
         if version is not None:
-            path = self._get_path(uid, action=["versions", version])
+            path = self._get_path(uid) + format_escaped_url("/versions/{}", version)
             data = self.session.get_resource(path)
             return self.build(data)
         else:
             tables = self.list_versions(uid)
             newest_table = max(tables, key=lambda x: x.version or 0)
             return newest_table
```

### Comparing `citrine-2.24.1/src/citrine/resources/generative_design_execution.py` & `citrine-2.8.0/src/citrine/resources/generative_design_execution.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/resources/ingredient_run.py` & `citrine-2.8.0/src/citrine/resources/ingredient_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 """Resources that represent ingredient run data objects."""
 from typing import List, Dict, Optional, Type, Iterator, Union
 from uuid import UUID
 
-from citrine._rest.resource import GEMDResource
+from citrine._rest.resource import Resource
 from citrine._serialization.properties import List as PropertyList
-from citrine._serialization.properties import String, LinkOrElse, Object
+from citrine._serialization.properties import Mapping, String, LinkOrElse, Object
 from citrine._serialization.properties import Optional as PropertyOptional
+from citrine.resources.data_concepts import DataConcepts, _make_link_by_uid
 from citrine.resources.object_runs import ObjectRun, ObjectRunCollection
 from gemd.entity.file_link import FileLink
 from gemd.entity.link_by_uid import LinkByUID
 from gemd.entity.object.ingredient_run import IngredientRun as GEMDIngredientRun
 from gemd.entity.object.ingredient_spec import IngredientSpec as GEMDIngredientSpec
 from gemd.entity.object.material_run import MaterialRun as GEMDMaterialRun
 from gemd.entity.object.process_run import ProcessRun as GEMDProcessRun
 from gemd.entity.value.continuous_value import ContinuousValue
 
 
-class IngredientRun(
-    GEMDResource['IngredientRun'],
-    ObjectRun,
-    GEMDIngredientRun,
-    typ=GEMDIngredientRun.typ
-):
+class IngredientRun(ObjectRun, Resource['IngredientRun'], GEMDIngredientRun):
     """
     An ingredient run.
 
     Ingredients annotate a material with information about its usage in a process.
 
     Parameters
     ----------
@@ -60,31 +56,29 @@
     file_links: List[FileLink], optional
         Links to associated files, with resource paths into the files API.
 
     """
 
     _response_key = GEMDIngredientRun.typ  # 'ingredient_run'
 
-    material = PropertyOptional(LinkOrElse(GEMDMaterialRun), 'material', override=True)
-    process = PropertyOptional(LinkOrElse(GEMDProcessRun),
-                               'process',
-                               override=True,
-                               use_init=True,
-                               )
-    mass_fraction = PropertyOptional(Object(ContinuousValue), 'mass_fraction')
-    volume_fraction = PropertyOptional(Object(ContinuousValue), 'volume_fraction')
-    number_fraction = PropertyOptional(Object(ContinuousValue), 'number_fraction')
-    absolute_quantity = PropertyOptional(Object(ContinuousValue), 'absolute_quantity')
-    spec = PropertyOptional(LinkOrElse(GEMDIngredientSpec), 'spec', override=True, use_init=True)
-
-    """
-    Intentionally private because they have some unusual dynamics
-    """
-    _name = PropertyOptional(String(), 'name')
-    _labels = PropertyOptional(PropertyList(String()), 'labels')
+    uids = Mapping(String('scope'), String('id'), 'uids', override=True)
+    tags = PropertyOptional(PropertyList(String()), 'tags', override=True)
+    notes = PropertyOptional(String(), 'notes', override=True)
+    material = PropertyOptional(LinkOrElse(), 'material', override=True)
+    process = PropertyOptional(LinkOrElse(), 'process', override=True)
+    mass_fraction = PropertyOptional(Object(ContinuousValue), 'mass_fraction', override=True)
+    volume_fraction = PropertyOptional(Object(ContinuousValue), 'volume_fraction', override=True)
+    number_fraction = PropertyOptional(Object(ContinuousValue), 'number_fraction', override=True)
+    absolute_quantity = PropertyOptional(
+        Object(ContinuousValue), 'absolute_quantity', override=True)
+    name = PropertyOptional(String(), 'name', override=True)
+    labels = PropertyOptional(PropertyList(String()), 'labels', override=True)
+    spec = PropertyOptional(LinkOrElse(), 'spec', override=True)
+    file_links = PropertyOptional(PropertyList(Object(FileLink)), 'file_links', override=True)
+    typ = String('type')
 
     def __init__(self,
                  *,
                  uids: Optional[Dict[str, str]] = None,
                  tags: Optional[List[str]] = None,
                  notes: Optional[str] = None,
                  material: Optional[GEMDMaterialRun] = None,
@@ -93,15 +87,15 @@
                  volume_fraction: Optional[ContinuousValue] = None,
                  number_fraction: Optional[ContinuousValue] = None,
                  absolute_quantity: Optional[ContinuousValue] = None,
                  spec: Optional[GEMDIngredientSpec] = None,
                  file_links: Optional[List[FileLink]] = None):
         if uids is None:
             uids = dict()
-        super(ObjectRun, self).__init__()
+        DataConcepts.__init__(self, GEMDIngredientRun.typ)
         GEMDIngredientRun.__init__(self, uids=uids, tags=tags, notes=notes,
                                    material=material, process=process,
                                    mass_fraction=mass_fraction, volume_fraction=volume_fraction,
                                    number_fraction=number_fraction,
                                    absolute_quantity=absolute_quantity,
                                    spec=spec, file_links=file_links)
 
@@ -136,15 +130,16 @@
 
         Returns
         -------
         Iterator[IngredientRun]
             The ingredient runs using the specified ingredient spec.
 
         """
-        return self._get_relation(relation='ingredient-specs', uid=uid)
+        link = _make_link_by_uid(uid)
+        return self._get_relation(relation='ingredient-specs', uid=link)
 
     def list_by_process(self,
                         uid: Union[UUID, str, LinkByUID, GEMDProcessRun]
                         ) -> Iterator[IngredientRun]:
         """
         Get ingredients to a process.
 
@@ -155,15 +150,16 @@
 
         Returns
         -------
         Iterator[IngredientRun]
             The ingredients to the specified process.
 
         """
-        return self._get_relation(relation='process-runs', uid=uid)
+        link = _make_link_by_uid(uid)
+        return self._get_relation(relation='process-runs', uid=link)
 
     def list_by_material(self,
                          uid: Union[UUID, str, LinkByUID, GEMDMaterialRun]
                          ) -> Iterator[IngredientRun]:
         """
         Get ingredients using the specified material.
 
@@ -174,8 +170,9 @@
 
         Returns
         -------
         Iterator[IngredientRun]
             The ingredients using the specified material
 
         """
-        return self._get_relation(relation='material-runs', uid=uid)
+        link = _make_link_by_uid(uid)
+        return self._get_relation(relation='material-runs', uid=link)
```

### Comparing `citrine-2.24.1/src/citrine/resources/ingredient_spec.py` & `citrine-2.8.0/src/citrine/resources/ingredient_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 """Resources that represent ingredient spec data objects."""
 from typing import List, Dict, Optional, Type, Iterator, Union
 from uuid import UUID
 
-from citrine._rest.resource import GEMDResource
+from citrine._rest.resource import Resource
 from citrine._serialization.properties import List as PropertyList
-from citrine._serialization.properties import String, LinkOrElse, Object
+from citrine._serialization.properties import Mapping, String, LinkOrElse, Object
 from citrine._serialization.properties import Optional as PropertyOptional
+from citrine.resources.data_concepts import DataConcepts, _make_link_by_uid
 from citrine.resources.object_specs import ObjectSpec, ObjectSpecCollection
 from gemd.entity.file_link import FileLink
 from gemd.entity.link_by_uid import LinkByUID
 from gemd.entity.object.ingredient_spec import IngredientSpec as GEMDIngredientSpec
 from gemd.entity.object.material_spec import MaterialSpec as GEMDMaterialSpec
 from gemd.entity.object.process_spec import ProcessSpec as GEMDProcessSpec
 from gemd.entity.value.continuous_value import ContinuousValue
 
 
-class IngredientSpec(
-    GEMDResource['IngredientSpec'],
-    ObjectSpec,
-    GEMDIngredientSpec,
-    typ=GEMDIngredientSpec.typ
-):
+class IngredientSpec(ObjectSpec, Resource['IngredientSpec'], GEMDIngredientSpec):
     """
     An ingredient specification.
 
     Ingredients annotate a material with information about its usage in a process.
 
     Parameters
     ----------
@@ -61,27 +57,28 @@
     file_links: List[FileLink], optional
         Links to associated files, with resource paths into the files API.
 
     """
 
     _response_key = GEMDIngredientSpec.typ  # 'ingredient_spec'
 
-    material = PropertyOptional(LinkOrElse(GEMDMaterialSpec), 'material', override=True)
-    process = PropertyOptional(LinkOrElse(GEMDProcessSpec),
-                               'process',
-                               override=True,
-                               use_init=True)
+    uids = Mapping(String('scope'), String('id'), 'uids', override=True)
+    tags = PropertyOptional(PropertyList(String()), 'tags', override=True)
+    notes = PropertyOptional(String(), 'notes', override=True)
+    material = PropertyOptional(LinkOrElse(), 'material', override=True)
+    process = PropertyOptional(LinkOrElse(), 'process', override=True)
     mass_fraction = PropertyOptional(Object(ContinuousValue), 'mass_fraction', override=True)
     volume_fraction = PropertyOptional(Object(ContinuousValue), 'volume_fraction', override=True)
     number_fraction = PropertyOptional(Object(ContinuousValue), 'number_fraction', override=True)
-    absolute_quantity = PropertyOptional(Object(ContinuousValue),
-                                         'absolute_quantity',
-                                         override=True)
-    name = String('name', override=True, use_init=True)
-    labels = PropertyOptional(PropertyList(String()), 'labels', override=True, use_init=True)
+    absolute_quantity = PropertyOptional(
+        Object(ContinuousValue), 'absolute_quantity', override=True)
+    name = String('name', override=True)
+    labels = PropertyOptional(PropertyList(String()), 'labels', override=True)
+    file_links = PropertyOptional(PropertyList(Object(FileLink)), 'file_links', override=True)
+    typ = String('type')
 
     def __init__(self,
                  name: str,
                  *,
                  uids: Optional[Dict[str, str]] = None,
                  tags: Optional[List[str]] = None,
                  notes: Optional[str] = None,
@@ -92,15 +89,15 @@
                  number_fraction: Optional[ContinuousValue] = None,
                  absolute_quantity: Optional[ContinuousValue] = None,
                  labels: Optional[List[str]] = None,
                  file_links: Optional[List[FileLink]] = None):
         if uids is None:
             uids = dict()
 
-        super(ObjectSpec, self).__init__()
+        DataConcepts.__init__(self, GEMDIngredientSpec.typ)
         GEMDIngredientSpec.__init__(self, uids=uids, tags=tags, notes=notes,
                                     material=material, process=process,
                                     mass_fraction=mass_fraction, volume_fraction=volume_fraction,
                                     number_fraction=number_fraction,
                                     absolute_quantity=absolute_quantity, labels=labels,
                                     name=name, file_links=file_links)
 
@@ -135,15 +132,16 @@
 
         Returns
         -------
         Iterator[IngredientSpec]
             The ingredients to the specified process.
 
         """
-        return self._get_relation(relation='process-specs', uid=uid)
+        link = _make_link_by_uid(uid)
+        return self._get_relation(relation='process-specs', uid=link)
 
     def list_by_material(self,
                          uid: Union[UUID, str, LinkByUID, GEMDMaterialSpec]
                          ) -> Iterator[IngredientSpec]:
         """
         Get ingredients using the specified material.
 
@@ -154,8 +152,9 @@
 
         Returns
         -------
         Iterator[IngredientSpec]
             The ingredients using the specified material
 
         """
-        return self._get_relation(relation='material-specs', uid=uid)
+        link = _make_link_by_uid(uid)
+        return self._get_relation(relation='material-specs', uid=link)
```

### Comparing `citrine-2.24.1/src/citrine/resources/material_run.py` & `citrine-2.8.0/src/citrine/resources/material_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """Resources that represent material run data objects."""
+import json
+import os
+from logging import getLogger
 from typing import List, Dict, Optional, Type, Iterator, Union
 from uuid import UUID
 
-from citrine._rest.resource import GEMDResource
+from citrine._rest.resource import Resource
+from citrine._serialization.properties import List as PropertyList
 from citrine._serialization.properties import Optional as PropertyOptional
-from citrine._serialization.properties import String, LinkOrElse
+from citrine._serialization.properties import String, LinkOrElse, Mapping, Object
 from citrine._utils.functions import format_escaped_url
-from citrine.resources.data_concepts import _make_link_by_uid
+from citrine.resources.data_concepts import DataConcepts, _make_link_by_uid
 from citrine.resources.material_spec import MaterialSpecCollection
 from citrine.resources.object_runs import ObjectRun, ObjectRunCollection
 from gemd.entity.file_link import FileLink
 from gemd.entity.link_by_uid import LinkByUID
 from gemd.entity.object.material_run import MaterialRun as GEMDMaterialRun
 from gemd.entity.object.material_spec import MaterialSpec as GEMDMaterialSpec
 from gemd.entity.template.material_template import MaterialTemplate as GEMDMaterialTemplate
 from gemd.entity.object.process_run import ProcessRun as GEMDProcessRun
+from gemd.json import GEMDEncoder
+from gemd.util import writable_sort_order
 
+logger = getLogger(__name__)
 
-class MaterialRun(
-    GEMDResource['MaterialRun'],
-    ObjectRun,
-    GEMDMaterialRun,
-    typ=GEMDMaterialRun.typ
-):
+
+class MaterialRun(ObjectRun, Resource['MaterialRun'], GEMDMaterialRun):
     """
     A material run.
 
     Parameters
     ----------
     name: str
         Name of the material run.
@@ -56,38 +59,37 @@
         Measurements performed on this material. The link is established by creating the
         measurement run and settings its `material` field to this material run.
 
     """
 
     _response_key = GEMDMaterialRun.typ  # 'material_run'
 
-    name = String('name', override=True, use_init=True)
-    process = PropertyOptional(LinkOrElse(GEMDProcessRun),
-                               'process',
-                               override=True,
-                               use_init=True,)
-    sample_type = PropertyOptional(String, 'sample_type', override=True)
-    spec = PropertyOptional(LinkOrElse(GEMDMaterialSpec),
-                            'spec',
-                            override=True,
-                            use_init=True,)
+    name = String('name', override=True)
+    uids = Mapping(String('scope'), String('id'), 'uids', override=True)
+    tags = PropertyOptional(PropertyList(String()), 'tags', override=True)
+    notes = PropertyOptional(String(), 'notes', override=True)
+    process = PropertyOptional(LinkOrElse(), 'process', override=True)
+    sample_type = String('sample_type', override=True)
+    spec = PropertyOptional(LinkOrElse(), 'spec', override=True)
+    file_links = PropertyOptional(PropertyList(Object(FileLink)), 'file_links', override=True)
+    typ = String('type')
 
     def __init__(self,
                  name: str,
                  *,
                  uids: Optional[Dict[str, str]] = None,
                  tags: Optional[List[str]] = None,
                  notes: Optional[str] = None,
                  process: Optional[GEMDProcessRun] = None,
                  sample_type: Optional[str] = "unknown",
                  spec: Optional[GEMDMaterialSpec] = None,
                  file_links: Optional[List[FileLink]] = None):
         if uids is None:
             uids = dict()
-        super(ObjectRun, self).__init__()
+        DataConcepts.__init__(self, GEMDMaterialRun.typ)
         GEMDMaterialRun.__init__(self, name=name, uids=uids,
                                  tags=tags, process=process,
                                  sample_type=sample_type, spec=spec,
                                  file_links=file_links, notes=notes)
 
     def __str__(self):
         return '<Material run {!r}>'.format(self.name)
@@ -103,15 +105,15 @@
     _resource = MaterialRun
 
     @classmethod
     def get_type(cls) -> Type[MaterialRun]:
         """Return the resource type in the collection."""
         return MaterialRun
 
-    def get_history(self, id: Union[str, UUID, LinkByUID, MaterialRun]) -> MaterialRun:
+    def get_history(self, id: Union[str, UUID, LinkByUID, MaterialRun]) -> Type[MaterialRun]:
         """
         Get the history associated with a terminal material.
 
         The history contains every single every process, ingredient and material that went into
         the terminal material as well as the measurements that were performed on all of those
         materials. The returned object is a material run with all of its fields fully populated.
 
@@ -125,22 +127,32 @@
         MaterialRun
             A material run that has all of its fields fully populated with the processes,
             ingredients, measurements, and other materials that were involved in the history
             of the object.
 
         """
         link = _make_link_by_uid(id)
-        path = format_escaped_url("projects/{}/material-history/{}/{}",
-                                  self.project_id,
-                                  link.scope,
-                                  link.id
-                                  )
+        base_path = os.path.dirname(self._get_path(ignore_dataset=True))
+        path = base_path + format_escaped_url("/material-history/{}/{}", link.scope, link.id)
         data = self.session.get_resource(path)
 
-        return MaterialRun.build(data)
+        # Add the root to the context and sort by writable order
+        blob = dict()
+        blob["context"] = sorted(
+            data['context'] + [data['root']],
+            key=lambda x: writable_sort_order(x["type"])
+        )
+        terminal_scope, terminal_id = next(iter(data['root']['uids'].items()))
+        # Add a link to the root as the "object"
+        blob["object"] = LinkByUID(scope=terminal_scope, id=terminal_id)
+
+        # Serialize using normal json (with the GEMDEncoder) and then deserialize with the
+        # GEMDEncoder encoder in order to rebuild the material history
+        return MaterialRun.get_json_support().loads(
+            json.dumps(blob, cls=GEMDEncoder, sort_keys=True))
 
     def get_by_process(self,
                        uid: Union[UUID, str, LinkByUID, GEMDProcessRun]
                        ) -> Optional[MaterialRun]:
         """
         Get output material of a process.
 
@@ -151,16 +163,17 @@
 
         Returns
         -------
         MaterialRun
             The output material of the specified process, or None if no such material exists.
 
         """
+        link = _make_link_by_uid(uid)
         return next(
-            self._get_relation(relation='process-runs', uid=uid, per_page=1),
+            self._get_relation(relation='process-runs', uid=link, per_page=1),
             None
         )
 
     def list_by_spec(self,
                      uid: Union[UUID, str, LinkByUID, GEMDMaterialSpec]
                      ) -> Iterator[MaterialRun]:
         """
@@ -173,15 +186,16 @@
 
         Returns
         -------
         Iterator[MaterialRun]
             The material runs using the specified material spec.
 
         """
-        return self._get_relation('material-specs', uid=uid)
+        link = _make_link_by_uid(uid)
+        return self._get_relation('material-specs', uid=link)
 
     def list_by_template(self,
                          uid: Union[UUID, str, LinkByUID, GEMDMaterialTemplate]
                          ) -> Iterator[MaterialRun]:
         """
         Get the material runs using the specified material template.
```

### Comparing `citrine-2.24.1/src/citrine/resources/material_spec.py` & `citrine-2.8.0/src/citrine/resources/material_spec.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 """Resources that represent material spec data objects."""
 from logging import getLogger
 from typing import List, Dict, Optional, Type, Iterator, Union
 from uuid import UUID
 
-from citrine._rest.resource import GEMDResource
+from citrine._rest.resource import Resource
 from citrine._serialization.properties import List as PropertyList
 from citrine._serialization.properties import Optional as PropertyOptional
-from citrine._serialization.properties import String, LinkOrElse, Object
+from citrine._serialization.properties import String, LinkOrElse, Mapping, Object
+from citrine.resources.data_concepts import DataConcepts, _make_link_by_uid
 from citrine.resources.object_specs import ObjectSpec, ObjectSpecCollection
 from gemd.entity.attribute.property_and_conditions import PropertyAndConditions
 from gemd.entity.file_link import FileLink
 from gemd.entity.link_by_uid import LinkByUID
 from gemd.entity.object.material_spec import MaterialSpec as GEMDMaterialSpec
 from gemd.entity.object.process_spec import ProcessSpec as GEMDProcessSpec
 from gemd.entity.template.material_template import MaterialTemplate as GEMDMaterialTemplate
 
 logger = getLogger(__name__)
 
 
-class MaterialSpec(
-    GEMDResource['MaterialSpec'],
-    ObjectSpec,
-    GEMDMaterialSpec,
-    typ=GEMDMaterialSpec.typ
-):
+class MaterialSpec(ObjectSpec, Resource['MaterialSpec'], GEMDMaterialSpec):
     """
     A material specification.
 
     Parameters
     ----------
     name: str
         Name of the material spec.
@@ -51,41 +47,38 @@
     file_links: List[FileLink], optional
         Links to associated files, with resource paths into the files API.
 
     """
 
     _response_key = GEMDMaterialSpec.typ  # 'material_spec'
 
-    name = String('name', override=True, use_init=True)
-    process = PropertyOptional(LinkOrElse(GEMDProcessSpec),
-                               'process',
-                               override=True,
-                               use_init=True,
-                               )
-    properties = PropertyOptional(PropertyList(Object(PropertyAndConditions)),
-                                  'properties',
-                                  override=True)
-    template = PropertyOptional(LinkOrElse(GEMDMaterialTemplate),
-                                'template',
-                                override=True,
-                                use_init=True,)
+    name = String('name', override=True)
+    uids = Mapping(String('scope'), String('id'), 'uids', override=True)
+    tags = PropertyOptional(PropertyList(String()), 'tags', override=True)
+    notes = PropertyOptional(String(), 'notes', override=True)
+    process = PropertyOptional(LinkOrElse(), 'process', override=True)
+    properties = PropertyOptional(
+        PropertyList(Object(PropertyAndConditions)), 'properties', override=True)
+    template = PropertyOptional(LinkOrElse(), 'template', override=True)
+    file_links = PropertyOptional(PropertyList(Object(FileLink)), 'file_links', override=True)
+    typ = String('type')
 
     def __init__(self,
                  name: str,
                  *,
                  uids: Optional[Dict[str, str]] = None,
                  tags: Optional[List[str]] = None,
                  notes: Optional[str] = None,
                  process: Optional[GEMDProcessSpec] = None,
                  properties: Optional[List[PropertyAndConditions]] = None,
                  template: Optional[GEMDMaterialTemplate] = None,
                  file_links: Optional[List[FileLink]] = None):
         if uids is None:
             uids = dict()
-        super(ObjectSpec, self).__init__()
+        DataConcepts.__init__(self, GEMDMaterialSpec.typ)
         GEMDMaterialSpec.__init__(self, name=name, uids=uids,
                                   tags=tags, process=process, properties=properties,
                                   template=template, file_links=file_links, notes=notes)
 
     def __str__(self):
         return '<Material spec {!r}>'.format(self.name)
 
@@ -117,15 +110,16 @@
 
         Returns
         -------
         Iterator[MaterialSpec]
             The material specs using the specified material template.
 
         """
-        return self._get_relation('material-templates', uid=uid)
+        link = _make_link_by_uid(uid)
+        return self._get_relation('material-templates', uid=link)
 
     def get_by_process(self,
                        uid: Union[UUID, str, LinkByUID, GEMDProcessSpec]
                        ) -> Optional[MaterialSpec]:
         """
         Get output material of a process.
 
@@ -136,15 +130,16 @@
 
         Returns
         -------
         MaterialSpec
             The output material of the specified process, or None if no such material exists.
 
         """
+        link = _make_link_by_uid(uid)
         return next(
             self._get_relation(
                 relation='process-specs',
-                uid=uid,
+                uid=link,
                 per_page=1
             ),
             None
         )
```

### Comparing `citrine-2.24.1/src/citrine/resources/measurement_run.py` & `citrine-2.8.0/src/citrine/resources/measurement_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 """Resources that represent measurement run data objects."""
 from typing import List, Dict, Optional, Type, Iterator, Union
 from uuid import UUID
 
-from citrine._rest.resource import GEMDResource
+from citrine._rest.resource import Resource
 from citrine._serialization.properties import List as PropertyList
 from citrine._serialization.properties import Optional as PropertyOptional
-from citrine._serialization.properties import String, Object, LinkOrElse
+from citrine._serialization.properties import String, Object, Mapping, LinkOrElse
+from citrine.resources.data_concepts import DataConcepts, _make_link_by_uid
 from citrine.resources.object_runs import ObjectRun, ObjectRunCollection
 from gemd.entity.attribute.condition import Condition
 from gemd.entity.attribute.parameter import Parameter
 from gemd.entity.attribute.property import Property
 from gemd.entity.file_link import FileLink
 from gemd.entity.link_by_uid import LinkByUID
 from gemd.entity.object.material_run import MaterialRun as GEMDMaterialRun
 from gemd.entity.object.measurement_run import MeasurementRun as GEMDMeasurementRun
 from gemd.entity.object.measurement_spec import MeasurementSpec as GEMDMeasurementSpec
 from gemd.entity.source.performed_source import PerformedSource
 
 
-class MeasurementRun(
-    GEMDResource['MeasurementRun'],
-    ObjectRun,
-    GEMDMeasurementRun,
-    typ=GEMDMeasurementRun.typ
-):
+class MeasurementRun(ObjectRun, Resource['MeasurementRun'], GEMDMeasurementRun):
     """
     A measurement run.
 
     Parameters
     ----------
     name: str
         Name of the measurement run.
@@ -58,25 +54,26 @@
     source: PerformedSource, optional
         Information about the person who performed the run and when.
 
     """
 
     _response_key = GEMDMeasurementRun.typ  # 'measurement_run'
 
-    name = String('name', override=True, use_init=True)
+    name = String('name', override=True)
+    uids = Mapping(String('scope'), String('id'), 'uids', override=True)
+    tags = PropertyOptional(PropertyList(String()), 'tags', override=True)
+    notes = PropertyOptional(String(), 'notes', override=True)
     conditions = PropertyOptional(PropertyList(Object(Condition)), 'conditions', override=True)
     parameters = PropertyOptional(PropertyList(Object(Parameter)), 'parameters', override=True)
     properties = PropertyOptional(PropertyList(Object(Property)), 'properties', override=True)
-    spec = PropertyOptional(LinkOrElse(GEMDMeasurementSpec), 'spec', override=True, use_init=True,)
-    material = PropertyOptional(LinkOrElse(GEMDMaterialRun),
-                                "material",
-                                override=True,
-                                use_init=True,
-                                )
+    spec = PropertyOptional(LinkOrElse(), 'spec', override=True)
+    material = PropertyOptional(LinkOrElse(), "material", override=True)
+    file_links = PropertyOptional(PropertyList(Object(FileLink)), 'file_links', override=True)
     source = PropertyOptional(Object(PerformedSource), "source", override=True)
+    typ = String('type')
 
     def __init__(self,
                  name: str,
                  *,
                  uids: Optional[Dict[str, str]] = None,
                  tags: Optional[List[str]] = None,
                  notes: Optional[str] = None,
@@ -85,15 +82,15 @@
                  parameters: Optional[List[Parameter]] = None,
                  spec: Optional[GEMDMeasurementSpec] = None,
                  material: Optional[GEMDMaterialRun] = None,
                  file_links: Optional[List[FileLink]] = None,
                  source: Optional[PerformedSource] = None):
         if uids is None:
             uids = dict()
-        super(ObjectRun, self).__init__()
+        DataConcepts.__init__(self, GEMDMeasurementRun.typ)
         GEMDMeasurementRun.__init__(self, name=name, uids=uids,
                                     material=material,
                                     tags=tags, conditions=conditions, properties=properties,
                                     parameters=parameters, spec=spec,
                                     file_links=file_links, notes=notes, source=source)
 
     def __str__(self):
@@ -127,15 +124,16 @@
 
         Returns
         -------
         Iterator[MeasurementRun]
             The measurement runs using the specified measurement spec.
 
         """
-        return self._get_relation('measurement-specs', uid=uid)
+        link = _make_link_by_uid(uid)
+        return self._get_relation('measurement-specs', uid=link)
 
     def list_by_material(self,
                          uid: Union[UUID, str, LinkByUID, GEMDMaterialRun]
                          ) -> Iterator[MeasurementRun]:
         """
         Get measurements of the specified material.
 
@@ -146,8 +144,9 @@
 
         Returns
         -------
         Iterator[MeasurementRun]
             The measurements of the specified material
 
         """
-        return self._get_relation(relation='material-runs', uid=uid)
+        link = _make_link_by_uid(uid)
+        return self._get_relation(relation='material-runs', uid=link)
```

### Comparing `citrine-2.24.1/src/citrine/resources/measurement_spec.py` & `citrine-2.8.0/src/citrine/resources/measurement_spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 """Resources that represent measurement spec data objects."""
 from typing import List, Dict, Optional, Type, Union, Iterator
 from uuid import UUID
 
-from citrine._rest.resource import GEMDResource
+from citrine._rest.resource import Resource
 from citrine._serialization.properties import List as PropertyList
 from citrine._serialization.properties import Optional as PropertyOptional
-from citrine._serialization.properties import String, Object, LinkOrElse
+from citrine._serialization.properties import String, Object, Mapping, LinkOrElse
+from citrine.resources.data_concepts import DataConcepts, _make_link_by_uid
 from citrine.resources.object_specs import ObjectSpec, ObjectSpecCollection
 from gemd.entity.attribute.condition import Condition
 from gemd.entity.attribute.parameter import Parameter
 from gemd.entity.file_link import FileLink
 from gemd.entity.link_by_uid import LinkByUID
 from gemd.entity.object.measurement_spec import MeasurementSpec as GEMDMeasurementSpec
 from gemd.entity.template.measurement_template import \
     MeasurementTemplate as GEMDMeasurementTemplate
 
 
-class MeasurementSpec(
-    GEMDResource['MeasurementSpec'],
-    ObjectSpec,
-    GEMDMeasurementSpec,
-    typ=GEMDMeasurementSpec.typ
-):
+class MeasurementSpec(ObjectSpec, Resource['MeasurementSpec'], GEMDMeasurementSpec):
     """
     A measurement specification.
 
     Parameters
     ----------
     name: str
         Name of the measurement spec.
@@ -49,36 +45,37 @@
     file_links: List[FileLink], optional
         Links to associated files, with resource paths into the files API.
 
     """
 
     _response_key = GEMDMeasurementSpec.typ  # 'measurement_spec'
 
-    name = String('name', override=True, use_init=True)
+    name = String('name', override=True)
+    uids = Mapping(String('scope'), String('id'), 'uids', override=True)
+    tags = PropertyOptional(PropertyList(String()), 'tags', override=True)
+    notes = PropertyOptional(String(), 'notes', override=True)
     conditions = PropertyOptional(PropertyList(Object(Condition)), 'conditions', override=True)
     parameters = PropertyOptional(PropertyList(Object(Parameter)), 'parameters', override=True)
-    template = PropertyOptional(LinkOrElse(GEMDMeasurementTemplate),
-                                'template',
-                                override=True,
-                                use_init=True,
-                                )
+    template = PropertyOptional(LinkOrElse(), 'template', override=True)
+    file_links = PropertyOptional(PropertyList(Object(FileLink)), 'file_links', override=True)
+    typ = String('type')
 
     def __init__(self,
                  name: str,
                  *,
                  uids: Optional[Dict[str, str]] = None,
                  tags: Optional[List[str]] = None,
                  notes: Optional[str] = None,
                  conditions: Optional[List[Condition]] = None,
                  parameters: Optional[List[Parameter]] = None,
                  template: Optional[GEMDMeasurementTemplate] = None,
                  file_links: Optional[List[FileLink]] = None):
         if uids is None:
             uids = dict()
-        super(ObjectSpec, self).__init__()
+        DataConcepts.__init__(self, GEMDMeasurementSpec.typ)
         GEMDMeasurementSpec.__init__(self, name=name, uids=uids,
                                      tags=tags, conditions=conditions, parameters=parameters,
                                      template=template, file_links=file_links, notes=notes)
 
     def __str__(self):
         return '<Measurement spec {!r}>'.format(self.name)
 
@@ -111,8 +108,9 @@
 
         Returns
         -------
         Iterator[MeasurementSpec]
             The measurement specs using the specified measurement template.
 
         """
-        return self._get_relation('measurement-templates', uid=uid)
+        link = _make_link_by_uid(uid)
+        return self._get_relation('measurement-templates', uid=link)
```

### Comparing `citrine-2.24.1/src/citrine/resources/module.py` & `citrine-2.8.0/src/citrine/resources/module.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/resources/object_runs.py` & `citrine-2.8.0/src/citrine/resources/object_runs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Top-level class for all object run objects and collections thereof."""
 from abc import ABC
 from typing import TypeVar
 
 from citrine.resources.data_objects import DataObject, DataObjectCollection
-from gemd.entity.object.has_spec import HasSpec
 
 
-class ObjectRun(DataObject, HasSpec, ABC):
+class ObjectRun(DataObject, ABC):
     """
     An abstract object run object.
 
     ObjectRun must be extended along with `Resource`
     """
```

### Comparing `citrine-2.24.1/src/citrine/resources/object_specs.py` & `citrine-2.8.0/src/citrine/resources/object_specs.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/resources/object_templates.py` & `citrine-2.8.0/src/citrine/resources/object_templates.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 """Top-level class for all object template objects and collections thereof."""
 from abc import ABC
 from typing import TypeVar
 
-from citrine._serialization.properties import Optional as PropertyOptional
-from citrine._serialization.properties import String
 from citrine.resources.templates import Template, TemplateCollection
-from gemd.entity.template.base_template import BaseTemplate as GEMDTemplate
 
 
-class ObjectTemplate(Template, GEMDTemplate, ABC):
+class ObjectTemplate(Template, ABC):
     """
     An abstract object template object.
 
     ObjectTemplate must be extended along with `Resource`
     """
 
-    name = String('name')
-    description = PropertyOptional(String(), 'description')
-
 
 ObjectTemplateResourceType = TypeVar("ObjectTemplateResourceType", bound="ObjectTemplate")
 
 
 class ObjectTemplateCollection(TemplateCollection[ObjectTemplateResourceType], ABC):
     """A collection of one kind of object template object."""
```

### Comparing `citrine-2.24.1/src/citrine/resources/parameter_template.py` & `citrine-2.8.0/src/citrine/resources/parameter_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Resources that represent parameter templates."""
 from typing import List, Dict, Optional, Type
 
-from citrine._rest.resource import GEMDResource
+from citrine._rest.resource import Resource
+from citrine._serialization.properties import List as PropertyList
+from citrine._serialization.properties import Optional as PropertyOptional
+from citrine._serialization.properties import String, Mapping, Object
 from citrine.resources.attribute_templates import AttributeTemplate, AttributeTemplateCollection
+from citrine.resources.data_concepts import DataConcepts
 from gemd.entity.bounds.base_bounds import BaseBounds
 from gemd.entity.template.parameter_template import ParameterTemplate as GEMDParameterTemplate
 
 
-class ParameterTemplate(
-    GEMDResource['ParameterTemplate'],
-    AttributeTemplate,
-    GEMDParameterTemplate,
-    typ=GEMDParameterTemplate.typ
-):
+class ParameterTemplate(AttributeTemplate, Resource['ParameterTemplate'], GEMDParameterTemplate):
     """
     A parameter template.
 
     Parameters
     ----------
     name: str
         The name of the parameter template.
@@ -33,24 +32,31 @@
         are hierarchical strings that store information about an entity. They can be used
         for filtering and discoverability.
 
     """
 
     _response_key = GEMDParameterTemplate.typ  # 'parameter_template'
 
+    name = String('name', override=True)
+    description = PropertyOptional(String(), 'description', override=True)
+    uids = Mapping(String('scope'), String('id'), 'uids', override=True)
+    tags = PropertyOptional(PropertyList(String()), 'tags', override=True)
+    bounds = Object(BaseBounds, 'bounds', override=True)
+    typ = String('type')
+
     def __init__(self,
                  name: str,
                  *,
                  bounds: BaseBounds,
                  uids: Optional[Dict[str, str]] = None,
                  description: Optional[str] = None,
                  tags: Optional[List[str]] = None):
         if uids is None:
             uids = dict()
-        super(AttributeTemplate, self).__init__()
+        DataConcepts.__init__(self, GEMDParameterTemplate.typ)
         GEMDParameterTemplate.__init__(self, name=name, bounds=bounds, tags=tags,
                                        uids=uids, description=description)
 
     def __str__(self):
         return '<Parameter template {!r}>'.format(self.name)
```

### Comparing `citrine-2.24.1/src/citrine/resources/predictor_evaluation_execution.py` & `citrine-2.8.0/src/citrine/resources/predictor_evaluation_execution.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 """Resources that represent both individual and collections of predictor evaluation executions."""
 from functools import partial
+import sys
 from typing import Optional, Union, Iterator
 from uuid import UUID
 
 from citrine._rest.collection import Collection
 from citrine._rest.resource import PredictorRef
 from citrine._session import Session
-from citrine._utils.functions import MigratedClassMeta, format_escaped_url
-from citrine.informatics.executions import predictor_evaluation_execution
+from citrine._utils.functions import shadow_classes_in_module, \
+    format_escaped_url
+from citrine.informatics.executions import PredictorEvaluationExecution
+import citrine.informatics.executions.predictor_evaluation_execution
 from citrine.resources.response import Response
 
 
-class PredictorEvaluationExecution(predictor_evaluation_execution.PredictorEvaluationExecution,
-                                   deprecated_in="2.22.1",
-                                   removed_in="3.0.0",
-                                   metaclass=MigratedClassMeta):
-    """The execution of a PredictorEvaluationWorkflow.
-
-    Possible statuses are INPROGRESS, SUCCEEDED, and FAILED.
-    Predictor evaluation executions also have a ``status_description`` field with more information.
-
-    """
+shadow_classes_in_module(citrine.informatics.executions.predictor_evaluation_execution,
+                         sys.modules[__name__])
 
 
 class PredictorEvaluationExecutionCollection(Collection["PredictorEvaluationExecution"]):
     """A collection of PredictorEvaluationExecutions."""
 
     _path_template = '/projects/{project_id}/predictor-evaluation-executions'  # noqa
     _individual_key = None
     _collection_key = 'response'
-    _resource = predictor_evaluation_execution.PredictorEvaluationExecution
+    _resource = PredictorEvaluationExecution
 
     def __init__(self,
                  project_id: UUID,
                  session: Session,
                  workflow_id: Optional[UUID] = None):
         self.project_id: UUID = project_id
         self.session: Session = session
         self.workflow_id: Optional[UUID] = workflow_id
 
-    def build(self, data: dict) -> predictor_evaluation_execution.PredictorEvaluationExecution:
+    def build(self, data: dict) -> PredictorEvaluationExecution:
         """Build an individual PredictorEvaluationExecution."""
-        execution = predictor_evaluation_execution.PredictorEvaluationExecution.build(data)
+        execution = PredictorEvaluationExecution.build(data)
         execution._session = self.session
         execution.project_id = self.project_id
         return execution
 
     def trigger(self,
                 predictor_id: UUID,
                 *,
@@ -79,23 +74,19 @@
             params["random_state"] = random_state
 
         payload = PredictorRef(predictor_id, predictor_version).dump()
         data = self.session.post_resource(path, payload, params=params, version='v2')
 
         return self.build(data)
 
-    def register(self,
-                 model: predictor_evaluation_execution.PredictorEvaluationExecution
-                 ) -> predictor_evaluation_execution.PredictorEvaluationExecution:
+    def register(self, model: PredictorEvaluationExecution) -> PredictorEvaluationExecution:
         """Cannot register an execution."""
         raise NotImplementedError("Cannot register a PredictorEvaluationExecution.")
 
-    def update(self,
-               model: predictor_evaluation_execution.PredictorEvaluationExecution
-               ) -> predictor_evaluation_execution.PredictorEvaluationExecution:
+    def update(self, model: PredictorEvaluationExecution) -> PredictorEvaluationExecution:
         """Cannot update an execution."""
         raise NotImplementedError("Cannot update a PredictorEvaluationExecution.")
 
     def archive(self, uid: Union[UUID, str]):
         """Archive a predictor evaluation execution.
 
         Parameters
@@ -118,15 +109,15 @@
         self._put_resource_ref('restore', uid)
 
     def list(self,
              *,
              per_page: int = 100,
              predictor_id: Optional[UUID] = None,
              predictor_version: Optional[Union[int, str]] = None
-             ) -> Iterator[predictor_evaluation_execution.PredictorEvaluationExecution]:
+             ) -> Iterator[PredictorEvaluationExecution]:
         """
         Paginate over the elements of the collection.
 
         Parameters
         ---------
         per_page: int, optional
             Max number of results to return per page. Default is 100.  This parameter
```

### Comparing `citrine-2.24.1/src/citrine/resources/predictor_evaluation_workflow.py` & `citrine-2.8.0/src/citrine/resources/predictor_evaluation_workflow.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/resources/process_run.py` & `citrine-2.8.0/src/citrine/resources/process_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Resources that represent process run data objects."""
 from typing import List, Dict, Optional, Type, Union, Iterator
 from uuid import UUID
 
-from citrine._rest.resource import GEMDResource
+from citrine._rest.resource import Resource
 from citrine._serialization.properties import List as PropertyList
 from citrine._serialization.properties import Optional as PropertyOptional
-from citrine._serialization.properties import String, Object, LinkOrElse
+from citrine._serialization.properties import String, Mapping, Object, LinkOrElse
+from citrine.resources.data_concepts import DataConcepts, _make_link_by_uid
 from citrine.resources.object_runs import ObjectRun, ObjectRunCollection
 from gemd.entity.attribute.condition import Condition
 from gemd.entity.attribute.parameter import Parameter
 from gemd.entity.file_link import FileLink
 from gemd.entity.link_by_uid import LinkByUID
 from gemd.entity.object.process_run import ProcessRun as GEMDProcessRun
 from gemd.entity.object.process_spec import ProcessSpec as GEMDProcessSpec
 from gemd.entity.source.performed_source import PerformedSource
 
 
-class ProcessRun(GEMDResource['ProcessRun'], ObjectRun, GEMDProcessRun, typ=GEMDProcessRun.typ):
+class ProcessRun(ObjectRun, Resource['ProcessRun'], GEMDProcessRun):
     """
     A process run.
 
     Processes transform zero or more input materials into exactly one output material.
 
     Parameters
     ----------
@@ -57,34 +58,39 @@
         Ingredient runs that act as inputs to this process run. The link is established by
         creating each ingredient run and setting its `process` field to this process run.
 
     """
 
     _response_key = GEMDProcessRun.typ  # 'process_run'
 
-    name = String('name', override=True, use_init=True)
+    name = String('name', override=True)
+    uids = Mapping(String('scope'), String('id'), 'uids', override=True)
+    tags = PropertyOptional(PropertyList(String()), 'tags', override=True)
+    notes = PropertyOptional(String(), 'notes', override=True)
     conditions = PropertyOptional(PropertyList(Object(Condition)), 'conditions', override=True)
     parameters = PropertyOptional(PropertyList(Object(Parameter)), 'parameters', override=True)
-    spec = PropertyOptional(LinkOrElse(GEMDProcessSpec), 'spec', override=True, use_init=True,)
+    spec = PropertyOptional(LinkOrElse(), 'spec', override=True)
+    file_links = PropertyOptional(PropertyList(Object(FileLink)), 'file_links', override=True)
     source = PropertyOptional(Object(PerformedSource), "source", override=True)
+    typ = String('type')
 
     def __init__(self,
                  name: str,
                  *,
                  uids: Optional[Dict[str, str]] = None,
                  tags: Optional[List[str]] = None,
                  notes: Optional[str] = None,
                  conditions: Optional[List[Condition]] = None,
                  parameters: Optional[List[Parameter]] = None,
                  spec: Optional[GEMDProcessSpec] = None,
                  file_links: Optional[List[FileLink]] = None,
                  source: Optional[PerformedSource] = None):
         if uids is None:
             uids = dict()
-        super(ObjectRun, self).__init__()
+        DataConcepts.__init__(self, GEMDProcessRun.typ)
         GEMDProcessRun.__init__(self, name=name, uids=uids,
                                 tags=tags, conditions=conditions, parameters=parameters,
                                 spec=spec, file_links=file_links, notes=notes, source=source)
 
     def __str__(self):
         return '<Process run {!r}>'.format(self.name)
 
@@ -116,8 +122,9 @@
 
         Returns
         -------
         Iterator[ProcessRun]
             The process runs using the specified process spec.
 
         """
-        return self._get_relation('process-specs', uid=uid)
+        link = _make_link_by_uid(uid)
+        return self._get_relation('process-specs', uid=link)
```

### Comparing `citrine-2.24.1/src/citrine/resources/process_spec.py` & `citrine-2.8.0/src/citrine/resources/process_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 """Resources that represent process spec objects."""
 from typing import Optional, Dict, List, Type, Union, Iterator
 from uuid import UUID
 
-from citrine._rest.resource import GEMDResource
+from citrine._rest.resource import Resource
 from citrine._serialization.properties import List as PropertyList
 from citrine._serialization.properties import Optional as PropertyOptional
-from citrine._serialization.properties import String, Object, LinkOrElse
+from citrine._serialization.properties import String, Mapping, Object, LinkOrElse
+from citrine.resources.data_concepts import DataConcepts, _make_link_by_uid
 from citrine.resources.object_specs import ObjectSpec, ObjectSpecCollection
 from gemd.entity.attribute.condition import Condition
 from gemd.entity.attribute.parameter import Parameter
 from gemd.entity.file_link import FileLink
 from gemd.entity.link_by_uid import LinkByUID
 from gemd.entity.object.process_spec import ProcessSpec as GEMDProcessSpec
 from gemd.entity.template.process_template import ProcessTemplate as GEMDProcessTemplate
 
 
-class ProcessSpec(
-    GEMDResource['ProcessSpec'],
-    ObjectSpec,
-    GEMDProcessSpec,
-    typ=GEMDProcessSpec.typ
-):
+class ProcessSpec(ObjectSpec, Resource['ProcessSpec'], GEMDProcessSpec):
     """
     A process specification.
 
     Processes transform zero or more input materials into exactly one output material.
 
     Parameters
     ----------
@@ -59,36 +55,38 @@
         Ingredient specs that act as inputs to this process spec. The link is established by
         creating each ingredient spec and setting its `process` field to this process spec.
 
     """
 
     _response_key = GEMDProcessSpec.typ  # 'process_spec'
 
-    name = String('name', override=True, use_init=True)
+    name = String('name', override=True)
+    uids = Mapping(String('scope'), String('id'), 'uids', override=True)
+    tags = PropertyOptional(PropertyList(String()), 'tags', override=True)
+    notes = PropertyOptional(String(), 'notes', override=True)
     conditions = PropertyOptional(PropertyList(Object(Condition)), 'conditions', override=True)
     parameters = PropertyOptional(PropertyList(Object(Parameter)), 'parameters', override=True)
-    template = PropertyOptional(LinkOrElse(GEMDProcessTemplate),
-                                'template', override=True,
-                                use_init=True,
-                                )
+    template = PropertyOptional(LinkOrElse(), 'template', override=True)
+    file_links = PropertyOptional(PropertyList(Object(FileLink)), 'file_links', override=True)
+    typ = String('type')
 
     def __init__(self,
                  name: str,
                  *,
                  uids: Optional[Dict[str, str]] = None,
                  tags: Optional[List[str]] = None,
                  notes: Optional[str] = None,
                  conditions: Optional[List[Condition]] = None,
                  parameters: Optional[List[Parameter]] = None,
                  template: Optional[GEMDProcessTemplate] = None,
                  file_links: Optional[List[FileLink]] = None
                  ):
         if uids is None:
             uids = dict()
-        super(ObjectSpec, self).__init__()
+        DataConcepts.__init__(self, GEMDProcessSpec.typ)
         GEMDProcessSpec.__init__(self, name=name, uids=uids,
                                  tags=tags, conditions=conditions, parameters=parameters,
                                  template=template, file_links=file_links, notes=notes)
 
     def __str__(self):
         return '<Process spec {!r}>'.format(self.name)
 
@@ -120,8 +118,9 @@
 
         Returns
         -------
         Iterator[ProcessSpec]
             The process specs using the specified process template
 
         """
-        return self._get_relation('process-templates', uid=uid)
+        link = _make_link_by_uid(uid)
+        return self._get_relation('process-templates', uid=link)
```

### Comparing `citrine-2.24.1/src/citrine/resources/process_template.py` & `citrine-2.8.0/src/citrine/resources/process_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 """Resources that represent process templates."""
 from typing import List, Dict, Optional, Union, Sequence, Type
 
-from citrine._rest.resource import GEMDResource
+from citrine._rest.resource import Resource
 from citrine._serialization.properties import List as PropertyList
 from citrine._serialization.properties import Optional as PropertyOptional
 from citrine._serialization.properties import Union as PropertyUnion
-from citrine._serialization.properties import String, Object, SpecifiedMixedList, \
+from citrine._serialization.properties import String, Mapping, Object, SpecifiedMixedList, \
     LinkOrElse
 from citrine.resources.condition_template import ConditionTemplate
+from citrine.resources.data_concepts import DataConcepts
 from citrine.resources.object_templates import ObjectTemplate, ObjectTemplateCollection
 from citrine.resources.parameter_template import ParameterTemplate
 from gemd.entity.bounds.base_bounds import BaseBounds
 from gemd.entity.link_by_uid import LinkByUID
 from gemd.entity.template.process_template import ProcessTemplate as GEMDProcessTemplate
-from gemd.entity.template.condition_template import ConditionTemplate as GEMDConditionTemplate
-from gemd.entity.template.parameter_template import ParameterTemplate as GEMDParameterTemplate
 
 
-class ProcessTemplate(
-    GEMDResource['ProcessTemplate'],
-    ObjectTemplate,
-    GEMDProcessTemplate,
-    typ=GEMDProcessTemplate.typ
-):
+class ProcessTemplate(ObjectTemplate, Resource['ProcessTemplate'], GEMDProcessTemplate):
     """
     A process template.
 
     Process templates are collections of condition and parameter templates that constrain the
     values of a measurement's condition and parameter attributes, and provide a common structure
     for describing similar measurements.
 
@@ -55,36 +49,25 @@
         with the second entry being a separate, *more restrictive* Bounds object that defines
         the limits of the value for this parameter.
 
     """
 
     _response_key = GEMDProcessTemplate.typ  # 'process_template'
 
-    conditions = PropertyOptional(
-        PropertyList(
-            PropertyUnion([LinkOrElse(GEMDConditionTemplate),
-                           SpecifiedMixedList([LinkOrElse(GEMDConditionTemplate),
-                                               PropertyOptional(Object(BaseBounds))])]
-                          )
-        ),
-        'conditions',
-        override=True
-    )
-    parameters = PropertyOptional(
-        PropertyList(
-            PropertyUnion([LinkOrElse(GEMDParameterTemplate),
-                           SpecifiedMixedList([LinkOrElse(GEMDParameterTemplate),
-                                               PropertyOptional(Object(BaseBounds))])]
-                          )
-        ),
-        'parameters',
-        override=True
-    )
+    name = String('name', override=True)
+    description = PropertyOptional(String(), 'description', override=True)
+    uids = Mapping(String('scope'), String('id'), 'uids', override=True)
+    tags = PropertyOptional(PropertyList(String()), 'tags', override=True)
+    conditions = PropertyOptional(PropertyList(PropertyUnion([LinkOrElse, SpecifiedMixedList(
+        [LinkOrElse, PropertyOptional(Object(BaseBounds))])])), 'conditions', override=True)
+    parameters = PropertyOptional(PropertyList(PropertyUnion([LinkOrElse, SpecifiedMixedList(
+        [LinkOrElse, PropertyOptional(Object(BaseBounds))])])), 'parameters', override=True)
     allowed_labels = PropertyOptional(PropertyList(String()), 'allowed_labels', override=True)
     allowed_names = PropertyOptional(PropertyList(String()), 'allowed_names', override=True)
+    typ = String('type')
 
     def __init__(self,
                  name: str,
                  *,
                  uids: Optional[Dict[str, str]] = None,
                  conditions: Optional[Sequence[Union[ConditionTemplate,
                                                      LinkByUID,
@@ -98,15 +81,15 @@
                                                      ]]] = None,
                  allowed_labels: Optional[List[str]] = None,
                  allowed_names: Optional[List[str]] = None,
                  description: Optional[str] = None,
                  tags: Optional[List[str]] = None):
         if uids is None:
             uids = dict()
-        super(ObjectTemplate, self).__init__()
+        DataConcepts.__init__(self, GEMDProcessTemplate.typ)
         GEMDProcessTemplate.__init__(self, name=name, uids=uids,
                                      conditions=conditions, parameters=parameters, tags=tags,
                                      description=description, allowed_labels=allowed_labels,
                                      allowed_names=allowed_names)
 
     def __str__(self):
         return '<Process template {!r}>'.format(self.name)
```

### Comparing `citrine-2.24.1/src/citrine/resources/project.py` & `citrine-2.8.0/src/citrine/resources/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,15 +522,15 @@
         Returns
         -------
         Iterable[Dict]
             Projects in this collection.
 
         """
         collections = []
-        path = self._get_path(action="search")
+        path = self._get_path() + '/search'
         query_params = {'userId': ""}
 
         json = {} if search_params is None else {'search_params': search_params}
 
         data = self.session.post_resource(path,
                                           params=query_params,
                                           json=json,
```

### Comparing `citrine-2.24.1/src/citrine/resources/project_member.py` & `citrine-2.8.0/src/citrine/resources/project_member.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/resources/report.py` & `citrine-2.8.0/src/citrine/resources/report.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/resources/response.py` & `citrine-2.8.0/src/citrine/resources/response.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/resources/status_detail.py` & `citrine-2.8.0/src/citrine/resources/status_detail.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,12 +21,15 @@
 class StatusDetail(Serializable[StatusDetailType]):
     """A status message and its level."""
 
     msg = properties.String("msg")
     level = properties.String("level")
 
     def __init__(self, *, msg: str, level: Union[str, StatusLevelEnum]):
+        if not isinstance(level, StatusLevelEnum):
+            level = StatusLevelEnum.get_enum(level)
+
         self.msg = msg
-        self.level = StatusLevelEnum.from_str(level, exception=True)
+        self.level = level.value
 
     def __str__(self):
         return f"[{self.level.upper()}] {self.msg}"  # pragma: no cover
```

### Comparing `citrine-2.24.1/src/citrine/resources/table_config.py` & `citrine-2.8.0/src/citrine/resources/table_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 
         If no version is specified, then the most recent version is returned.
 
         """
         if uid is None:
             raise ValueError("Cannot get when uid=None.  Are you using a registered resource?")
         if version is not None:
-            path = self._get_path(uid, action=["versions", version])
+            path = self._get_path(uid) + format_escaped_url("/versions/{}", version)
             data = self.session.get_resource(path)
         else:
             path = self._get_path(uid)
             data = self.session.get_resource(path)
             version_numbers = [version_data['version_number'] for version_data in data['versions']]
             index = version_numbers.index(max(version_numbers))
             data['version'] = data['versions'][index]
@@ -498,15 +498,15 @@
         ----------
         table_config: TableConfig
             Table Config to preview
         preview_materials: List[LinkByUID]
             List of links to the material runs to use as terminal materials in the preview
 
         """
-        path = self._get_path(action="preview")
+        path = self._get_path() + "/preview"
         body = {
             "definition": table_config.dump(),
             "rows": [x.as_dict() for x in preview_materials]
         }
         return self.session.post_resource(path, body)
 
     def register(self, table_config: TableConfig) -> TableConfig:
```

### Comparing `citrine-2.24.1/src/citrine/resources/team.py` & `citrine-2.8.0/src/citrine/resources/team.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from uuid import UUID
 
 from citrine._rest.collection import Collection
 from citrine._rest.resource import Resource, ResourceTypeEnum
 from citrine._serialization import properties
 from citrine._session import Session
 from citrine._utils.functions import format_escaped_url
-from citrine.resources.project import ProjectCollection
+from citrine.resources import ProjectCollection
 from citrine.resources.user import User, UserCollection
 
 WRITE = "WRITE"
 READ = "READ"
 SHARE = "SHARE"
 TEAM_ACTIONS = Union[WRITE, READ, SHARE]
```

### Comparing `citrine-2.24.1/src/citrine/resources/templates.py` & `citrine-2.8.0/src/citrine/resources/templates.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/resources/user.py` & `citrine-2.8.0/src/citrine/_rest/resource.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,103 +1,70 @@
-"""Resources that represent both individual and collections of users."""
-from typing import Optional
+from typing import TypeVar, Optional, Union
+from uuid import UUID
 
-from citrine._rest.collection import Collection
-from citrine._rest.resource import Resource, ResourceTypeEnum
+from citrine._serialization.serializable import Serializable
 from citrine._serialization import properties
-from citrine._session import Session
+from gemd.enumeration.base_enumeration import BaseEnumeration
 
 
-class User(Resource['User']):
-    """
-    A Citrine User.
+class ResourceTypeEnum(BaseEnumeration):
+    """The type of the resource; used for modifying access controls.
 
-    Parameters
-    ----------
-    screen_name: str
-        Screen name of the user.
-    email: str
-        Email address of the user.
-    position: str
-        Position of the user.
-    is_admin: bool
-        Whether or not the user is an administrator.
-    session: Session, optional
-        Citrine session used to connect to the database.
+    * TEAM is a Team
+    * PROJECT is a Project
+    * DATASET is a Dataset
+    * MODULE is a Module: a Predictor or Design Space
+    * USER is a user
+    * TABLE is a GemTable
+    * TABLE_DEFINITION is a TableConfig
 
     """
 
-    _resource_type = ResourceTypeEnum.USER
-    _session: Optional[Session] = None
+    TEAM = "TEAM"
+    PROJECT = "PROJECT"
+    DATASET = "DATASET"
+    MODULE = "MODULE"
+    USER = "USER"
+    TABLE = "TABLE"
+    TABLE_DEFINITION = "TABLE_DEFINITION"
+
+
+Self = TypeVar('Self', bound='Resource')
+
+
+class Resource(Serializable[Self]):
+    """Abstract class for representing individual REST resource."""
+
+    _path_template: str = NotImplemented
+    _response_key: Optional[str] = None
+    _resource_type: ResourceTypeEnum = NotImplemented
+
+    def access_control_dict(self) -> dict:
+        """Return an access control entity representation of this resource. Internal use only."""
+        return {
+            "type": self._resource_type.value,
+            "id": str(self.uid)
+        }
+
+
+class ResourceRef(Serializable['ResourceRef']):
+    """A reference to a resource by UID."""
+
+    # json key 'module_uid' is a legacy of when this object was only used for modules
+    uid = properties.UUID('module_uid')
+
+    def __init__(self, uid: Union[UUID, str]):
+        self.uid = uid
+
+
+class PredictorRef(Serializable['PredictorRef']):
+    """A reference to a resource by UID."""
+
+    uid = properties.UUID('predictor_id')
+    version = properties.Optional(
+        properties.Union([properties.Integer(), properties.String()]),
+        'predictor_version'
+    )
 
-    uid = properties.Optional(properties.UUID, 'id')
-    screen_name = properties.String('screen_name')
-    position = properties.Optional(properties.String(), 'position')
-    email = properties.String('email')
-    is_admin = properties.Boolean('is_admin')
-
-    def __init__(self,
-                 *,
-                 screen_name: str,
-                 email: str,
-                 position: Optional[str],
-                 is_admin: bool):
-        self.email: str = email
-        self.position: Optional[str] = position
-        self.screen_name: str = screen_name
-        self.is_admin: bool = is_admin
-
-    def __str__(self):
-        return '<User {!r}>'.format(self.screen_name)
-
-    def get(self):
-        """Retrieve a specific user from the database."""
-        raise NotImplementedError("Get Not Implemented in Citrine Platform")
-
-
-class UserCollection(Collection[User]):
-    """Represents the collection of all users."""
-
-    _path_template = '/users'
-    _collection_key = 'users'
-    _individual_key = 'user'
-    _resource = User
-
-    def __init__(self, session: Session):
-        self.session: Session = session
-
-    def me(self):
-        """Get information about the current user."""
-        data = self.session.get_resource(self._path_template + '/me')
-        return self.build(data)
-
-    def build(self, data):
-        """
-        Build an individual user from a dictionary.
-
-        Parameters
-        ----------
-        data: dict
-          A dictionary representing the user.
-
-        Returns
-        -------
-        User
-          The user created from data.
-
-        """
-        user = User.build(data)
-        user._session = self.session
-        return user
-
-    def register(self,
-                 *,
-                 screen_name: str,
-                 email: str,
-                 position: str,
-                 is_admin: bool) -> User:
-        """Register a User."""
-        return super().register(User(
-            screen_name=screen_name,
-            email=email,
-            position=position,
-            is_admin=is_admin))
+    def __init__(self, uid: Union[UUID, str], version: Optional[Union[int, str]] = None):
+        self.uid = uid
+        self.version = version
```

### Comparing `citrine-2.24.1/src/citrine/seeding/find_or_create.py` & `citrine-2.8.0/src/citrine/seeding/find_or_create.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine/seeding/sort_gems.py` & `citrine-2.8.0/src/citrine/seeding/sort_gems.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/src/citrine.egg-info/PKG-INFO` & `citrine-2.8.0/src/citrine.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: citrine
-Version: 2.24.1
+Version: 2.8.0
 Summary: Python library for the Citrine Platform
 Home-page: http://github.com/CitrineInformatics/citrine-python
 Author: Citrine Informatics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: builders
 Provides-Extra: ../tests
 License-File: LICENSE
 
 # Getting Started
 `citrine-python` is the Python library for the Citrine Platform. To get started, install `citrine-python`:
```

### Comparing `citrine-2.24.1/src/citrine.egg-info/SOURCES.txt` & `citrine-2.8.0/src/citrine.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -63,32 +63,28 @@
 src/citrine/informatics/constraints/scalar_range_constraint.py
 src/citrine/informatics/design_spaces/__init__.py
 src/citrine/informatics/design_spaces/data_source_design_space.py
 src/citrine/informatics/design_spaces/design_space.py
 src/citrine/informatics/design_spaces/enumerated_design_space.py
 src/citrine/informatics/design_spaces/formulation_design_space.py
 src/citrine/informatics/design_spaces/product_design_space.py
-src/citrine/informatics/design_spaces/sample_design_space.py
 src/citrine/informatics/executions/__init__.py
 src/citrine/informatics/executions/design_execution.py
-src/citrine/informatics/executions/execution.py
 src/citrine/informatics/executions/generative_design_execution.py
 src/citrine/informatics/executions/predictor_evaluation_execution.py
-src/citrine/informatics/executions/sample_design_space_execution.py
 src/citrine/informatics/predictors/__init__.py
 src/citrine/informatics/predictors/auto_ml_predictor.py
 src/citrine/informatics/predictors/chemical_formula_featurizer.py
 src/citrine/informatics/predictors/expression_predictor.py
 src/citrine/informatics/predictors/graph_predictor.py
 src/citrine/informatics/predictors/ingredient_fractions_predictor.py
 src/citrine/informatics/predictors/ingredients_to_formulation_predictor.py
 src/citrine/informatics/predictors/label_fractions_predictor.py
 src/citrine/informatics/predictors/mean_property_predictor.py
 src/citrine/informatics/predictors/molecular_structure_featurizer.py
-src/citrine/informatics/predictors/node.py
 src/citrine/informatics/predictors/predictor.py
 src/citrine/informatics/predictors/simple_mixture_predictor.py
 src/citrine/informatics/predictors/single_predict_request.py
 src/citrine/informatics/predictors/single_prediction.py
 src/citrine/informatics/workflows/__init__.py
 src/citrine/informatics/workflows/design_workflow.py
 src/citrine/informatics/workflows/predictor_evaluation_workflow.py
@@ -112,15 +108,14 @@
 src/citrine/resources/design_space.py
 src/citrine/resources/design_workflow.py
 src/citrine/resources/experiment_datasource.py
 src/citrine/resources/file_link.py
 src/citrine/resources/gemd_resource.py
 src/citrine/resources/gemtables.py
 src/citrine/resources/generative_design_execution.py
-src/citrine/resources/ingestion.py
 src/citrine/resources/ingredient_run.py
 src/citrine/resources/ingredient_spec.py
 src/citrine/resources/job.py
 src/citrine/resources/material_run.py
 src/citrine/resources/material_spec.py
 src/citrine/resources/material_template.py
 src/citrine/resources/measurement_run.py
@@ -139,15 +134,14 @@
 src/citrine/resources/process_template.py
 src/citrine/resources/project.py
 src/citrine/resources/project_member.py
 src/citrine/resources/project_roles.py
 src/citrine/resources/property_template.py
 src/citrine/resources/report.py
 src/citrine/resources/response.py
-src/citrine/resources/sample_design_space_execution.py
 src/citrine/resources/status_detail.py
 src/citrine/resources/table_config.py
 src/citrine/resources/team.py
 src/citrine/resources/templates.py
 src/citrine/resources/user.py
 src/citrine/seeding/__init__.py
 src/citrine/seeding/find_or_create.py
```

### Comparing `citrine-2.24.1/tests/test_citrine.py` & `citrine-2.8.0/tests/test_citrine.py`

 * *Files identical despite different names*

### Comparing `citrine-2.24.1/tests/test_session.py` & `citrine-2.8.0/tests/test_session.py`

 * *Files identical despite different names*

