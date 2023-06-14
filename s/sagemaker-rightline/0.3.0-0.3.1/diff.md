# Comparing `tmp/sagemaker-rightline-0.3.0.tar.gz` & `tmp/sagemaker-rightline-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-rightline-0.3.0.tar", last modified: Sat Jun 10 14:03:39 2023, max compression
+gzip compressed data, was "sagemaker-rightline-0.3.1.tar", last modified: Wed Jun 14 14:30:10 2023, max compression
```

## Comparing `sagemaker-rightline-0.3.0.tar` & `sagemaker-rightline-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:03:39.833795 sagemaker-rightline-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-06-10 14:03:39.833795 sagemaker-rightline-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:03:39.833795 sagemaker-rightline-0.3.0/sagemaker_rightline/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 14:03:32.000000 sagemaker-rightline-0.3.0/sagemaker_rightline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/sagemaker_rightline/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/sagemaker_rightline/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    24416 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/sagemaker_rightline/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:03:39.833795 sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-06-10 14:03:39.000000 sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-10 14:03:39.000000 sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:03:39.000000 sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-10 14:03:39.000000 sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-10 14:03:39.000000 sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 14:03:39.833795 sagemaker-rightline-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:03:39.833795 sagemaker-rightline-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:30:10.850690 sagemaker-rightline-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-06-14 14:30:10.850690 sagemaker-rightline-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:30:10.846690 sagemaker-rightline-0.3.1/sagemaker_rightline/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 14:30:00.000000 sagemaker-rightline-0.3.1/sagemaker_rightline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/sagemaker_rightline/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/sagemaker_rightline/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26341 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/sagemaker_rightline/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:30:10.850690 sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-06-14 14:30:10.000000 sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-14 14:30:10.000000 sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:30:10.000000 sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 14:30:10.000000 sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 14:30:10.000000 sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 14:30:10.850690 sagemaker-rightline-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:30:10.850690 sagemaker-rightline-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/tests/test_validations.py
```

### Comparing `sagemaker-rightline-0.3.0/LICENSE` & `sagemaker-rightline-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.0/PKG-INFO` & `sagemaker-rightline-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -83,14 +83,15 @@
   - `StepKmsKeyIdAsExpected`
   - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
   - `StepTagsAsExpected`
   - `StepInputsAsExpected`
+  - `StepOutputsAsExpected`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
 For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
@@ -108,28 +109,29 @@
 A `Report` is a class whose instance is returned by the `Configuration` class (optionally a pandas.DataFrame instead).
 It contains the results of the `Validations` that were run against the `Pipeline` object as well as additional information
 to allow for further analysis.
 
 ## Usage
 
 ```python
-from sagemaker.processing import NetworkConfig, ProcessingInput
+from sagemaker.processing import NetworkConfig, ProcessingInput, ProcessingOutput
 from sagemaker.workflow.parameters import ParameterString
 from sagemaker_rightline.model import Configuration
 from sagemaker_rightline.rules import Contains, Equals
 from sagemaker_rightline.validations import (
     PipelineParametersAsExpected,
     StepImagesExist,
     StepKmsKeyIdAsExpected,
     StepNetworkConfigAsExpected,
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
     StepTagsAsExpected,
     StepInputsAsExpected,
+    StepOutputsAsExpected,
 )
 
 # Import a dummy pipeline
 from tests.fixtures.pipeline import get_sagemaker_pipeline, DUMMY_BUCKET
 
 sm_pipeline = get_sagemaker_pipeline()
 
@@ -179,14 +181,25 @@
                 destination="/opt/ml/processing/input",
                 input_name="input-2",
             )
         ],
         step_type="Processing",  # either step_type or step_name must be set to filter
         rule=Contains(),
     ),
+    StepOutputsAsExpected(
+        outputs_expected=[
+            ProcessingOutput(
+                source="/opt/ml/processing/output",
+                destination=f"s3://{DUMMY_BUCKET}/output-1",
+                output_name="output-1",
+            )
+        ],
+        step_name="sm_processing_step_spark",  # optional
+        rule=Contains(),
+    ),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.3.0/README.md` & `sagemaker-rightline-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
   - `StepKmsKeyIdAsExpected`
   - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
   - `StepTagsAsExpected`
   - `StepInputsAsExpected`
+  - `StepOutputsAsExpected`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
 For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
@@ -63,28 +64,29 @@
 A `Report` is a class whose instance is returned by the `Configuration` class (optionally a pandas.DataFrame instead).
 It contains the results of the `Validations` that were run against the `Pipeline` object as well as additional information
 to allow for further analysis.
 
 ## Usage
 
 ```python
-from sagemaker.processing import NetworkConfig, ProcessingInput
+from sagemaker.processing import NetworkConfig, ProcessingInput, ProcessingOutput
 from sagemaker.workflow.parameters import ParameterString
 from sagemaker_rightline.model import Configuration
 from sagemaker_rightline.rules import Contains, Equals
 from sagemaker_rightline.validations import (
     PipelineParametersAsExpected,
     StepImagesExist,
     StepKmsKeyIdAsExpected,
     StepNetworkConfigAsExpected,
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
     StepTagsAsExpected,
     StepInputsAsExpected,
+    StepOutputsAsExpected,
 )
 
 # Import a dummy pipeline
 from tests.fixtures.pipeline import get_sagemaker_pipeline, DUMMY_BUCKET
 
 sm_pipeline = get_sagemaker_pipeline()
 
@@ -134,14 +136,25 @@
                 destination="/opt/ml/processing/input",
                 input_name="input-2",
             )
         ],
         step_type="Processing",  # either step_type or step_name must be set to filter
         rule=Contains(),
     ),
+    StepOutputsAsExpected(
+        outputs_expected=[
+            ProcessingOutput(
+                source="/opt/ml/processing/output",
+                destination=f"s3://{DUMMY_BUCKET}/output-1",
+                output_name="output-1",
+            )
+        ],
+        step_name="sm_processing_step_spark",  # optional
+        rule=Contains(),
+    ),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.3.0/pyproject.toml` & `sagemaker-rightline-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.0/sagemaker_rightline/model.py` & `sagemaker-rightline-0.3.1/sagemaker_rightline/model.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.0/sagemaker_rightline/rules.py` & `sagemaker-rightline-0.3.1/sagemaker_rightline/rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.0/sagemaker_rightline/validations.py` & `sagemaker-rightline-0.3.1/sagemaker_rightline/validations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Union
 
 import boto3
 from botocore.exceptions import ClientError
 from sagemaker.estimator import Estimator
 from sagemaker.inputs import FileSystemInput, TrainingInput
-from sagemaker.processing import NetworkConfig, ProcessingInput
+from sagemaker.processing import NetworkConfig, ProcessingInput, ProcessingOutput
 from sagemaker.workflow.entities import PipelineVariable
 from sagemaker.workflow.parameters import Parameter
 from sagemaker.workflow.pipeline import Pipeline
 
 from sagemaker_rightline.model import Rule, Validation, ValidationResult
 
 
@@ -619,15 +619,15 @@
                 )
         return formatted_inputs
 
     def run(
         self,
         sagemaker_pipeline: Pipeline,
     ) -> ValidationResult:
-        """Runs validation of Parameters on Pipeline.
+        """Runs validation of Step Inputs on Pipeline.
 
         :param sagemaker_pipeline: SageMaker Pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
         :return: validation result
         :rtype: ValidationResult
         """
         if self.step_filter:
@@ -646,7 +646,63 @@
             # TrainingStep has a dict with values potentially being TrainingInput or FileSystemInput
             inputs_observed_formatted = StepInputsAsExpected.format_training_inputs(inputs_observed)
             inputs_expected_formatted = StepInputsAsExpected.format_training_inputs(
                 self.inputs_expected
             )
         result = self.rule.run(inputs_observed_formatted, inputs_expected_formatted, self.name)
         return result
+
+
+class StepOutputsAsExpected(Validation):
+    """Validate Outputs of Pipeline Step.
+
+    Supported only for ProcessingStep. This validation is useful when
+    you want to ensure that the Outputs of a Pipeline Step are as
+    expected.
+    """
+
+    def __init__(
+        self,
+        outputs_expected: List[ProcessingOutput],
+        rule: Rule,
+        step_name: Optional[str] = None,
+    ) -> None:
+        """Initialize StepTagsAsExpected validation.
+
+        :param outputs_expected: Expected Inputs
+        :type outputs_expected: List[ProcessingOutput]
+        :param rule: Rule to use for validation
+        :type rule: Rule
+        :param step_name: Name of Step to validate, defaults to None
+        :type step_name: Optional[str], optional
+        :return: None
+        :rtype: None
+        """
+
+        self.step_filter: str = f"name=={step_name}" if step_name else ""
+
+        super().__init__(
+            name="StepOutputsAsExpected",
+            paths=[
+                f".steps[{self.step_filter} && step_type/value==Processing]].outputs",
+            ],
+            rule=rule,
+        )
+        self.outputs_expected: List[ProcessingOutput] = outputs_expected
+
+    def run(
+        self,
+        sagemaker_pipeline: Pipeline,
+    ) -> ValidationResult:
+        """Runs validation of StepOutputs on Pipeline.
+
+        :param sagemaker_pipeline: SageMaker Pipeline
+        :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
+        :return: validation result
+        :rtype: ValidationResult
+        """
+
+        outputs_observed = Validation.get_attribute(sagemaker_pipeline, self.paths)
+        outputs_observed_formatted = [x.__dict__ for y in outputs_observed for x in y]
+        outputs_expected_formatted = [x.__dict__ for x in self.outputs_expected]
+        result = self.rule.run(outputs_observed_formatted, outputs_expected_formatted, self.name)
+        return result
```

### Comparing `sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/PKG-INFO` & `sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -83,14 +83,15 @@
   - `StepKmsKeyIdAsExpected`
   - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
   - `StepTagsAsExpected`
   - `StepInputsAsExpected`
+  - `StepOutputsAsExpected`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
 For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
@@ -108,28 +109,29 @@
 A `Report` is a class whose instance is returned by the `Configuration` class (optionally a pandas.DataFrame instead).
 It contains the results of the `Validations` that were run against the `Pipeline` object as well as additional information
 to allow for further analysis.
 
 ## Usage
 
 ```python
-from sagemaker.processing import NetworkConfig, ProcessingInput
+from sagemaker.processing import NetworkConfig, ProcessingInput, ProcessingOutput
 from sagemaker.workflow.parameters import ParameterString
 from sagemaker_rightline.model import Configuration
 from sagemaker_rightline.rules import Contains, Equals
 from sagemaker_rightline.validations import (
     PipelineParametersAsExpected,
     StepImagesExist,
     StepKmsKeyIdAsExpected,
     StepNetworkConfigAsExpected,
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
     StepTagsAsExpected,
     StepInputsAsExpected,
+    StepOutputsAsExpected,
 )
 
 # Import a dummy pipeline
 from tests.fixtures.pipeline import get_sagemaker_pipeline, DUMMY_BUCKET
 
 sm_pipeline = get_sagemaker_pipeline()
 
@@ -179,14 +181,25 @@
                 destination="/opt/ml/processing/input",
                 input_name="input-2",
             )
         ],
         step_type="Processing",  # either step_type or step_name must be set to filter
         rule=Contains(),
     ),
+    StepOutputsAsExpected(
+        outputs_expected=[
+            ProcessingOutput(
+                source="/opt/ml/processing/output",
+                destination=f"s3://{DUMMY_BUCKET}/output-1",
+                output_name="output-1",
+            )
+        ],
+        step_name="sm_processing_step_spark",  # optional
+        rule=Contains(),
+    ),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.3.0/tests/test_model.py` & `sagemaker-rightline-0.3.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.0/tests/test_rules.py` & `sagemaker-rightline-0.3.1/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.0/tests/test_validations.py` & `sagemaker-rightline-0.3.1/tests/test_validations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import pytest
 from moto import mock_ecr, mock_iam, mock_lambda
 from sagemaker.inputs import FileSystemInput, TrainingInput
-from sagemaker.processing import NetworkConfig, ProcessingInput
+from sagemaker.processing import NetworkConfig, ProcessingInput, ProcessingOutput
 from sagemaker.workflow.parameters import ParameterString
 
 from sagemaker_rightline.model import Validation, ValidationResult
 from sagemaker_rightline.rules import Contains, Equals
 from sagemaker_rightline.validations import (
     ContainerImage,
     PipelineParametersAsExpected,
     StepImagesExist,
     StepInputsAsExpected,
     StepKmsKeyIdAsExpected,
     StepLambdaFunctionExists,
     StepNetworkConfigAsExpected,
+    StepOutputsAsExpected,
     StepRoleNameAsExpected,
     StepRoleNameExists,
     StepTagsAsExpected,
 )
 from tests.fixtures.constants import (
     TEST_ACCOUNT_ID,
     TEST_LAMBDA_FUNC_NAME,
@@ -691,7 +692,117 @@
 
 def test_step_inputs_as_expected_args_validation_neither() -> None:
     with pytest.raises(ValueError):
         StepInputsAsExpected(
             inputs_expected=[],
             rule=Equals(),
         )
+
+
+@pytest.mark.parametrize(
+    "rule,outputs_expected,success",
+    [
+        [
+            Contains,
+            [
+                ProcessingOutput(
+                    output_name="output-1",
+                    source="/opt/ml/processing/output/1",
+                    destination=f"s3://{DUMMY_BUCKET}/output-1",
+                ),
+                ProcessingOutput(
+                    output_name="output-2",
+                    source="/opt/ml/processing/output/2",
+                    destination=f"s3://{DUMMY_BUCKET}/output-2",
+                ),
+            ],
+            True,
+        ],
+        [
+            Contains,
+            [
+                ProcessingOutput(
+                    output_name="output-999",
+                    source="/opt/ml/processing/output/1",
+                    destination=f"s3://{DUMMY_BUCKET}/output-1",
+                ),
+                ProcessingOutput(
+                    output_name="output-2",
+                    source="/opt/ml/processing/output/2",
+                    destination=f"s3://{DUMMY_BUCKET}/output-2",
+                ),
+            ],
+            False,
+        ],
+        [
+            Equals,
+            [
+                ProcessingOutput(
+                    output_name="output-1",
+                    source="/opt/ml/processing/output/1",
+                    destination=f"s3://{DUMMY_BUCKET}/output-1",
+                ),
+                ProcessingOutput(
+                    output_name="output-2",
+                    source="/opt/ml/processing/output/2",
+                    destination=f"s3://{DUMMY_BUCKET}/output-2",
+                ),
+            ],
+            False,
+        ],
+    ],
+)
+def test_step_outputs_as_expected_no_filter(
+    rule, outputs_expected, success, sagemaker_pipeline
+) -> None:
+    step_outputs_validation = StepOutputsAsExpected(
+        outputs_expected=outputs_expected,
+        rule=rule(),
+    )
+    result = step_outputs_validation.run(sagemaker_pipeline)
+    assert result.success == success
+
+
+@pytest.mark.parametrize(
+    "rule,outputs_expected,step_name,success",
+    [
+        [
+            Equals,
+            [
+                ProcessingOutput(
+                    output_name="output-1",
+                    source="/opt/ml/processing/output/1",
+                    destination=f"s3://{DUMMY_BUCKET}/output-1",
+                ),
+                ProcessingOutput(
+                    output_name="output-2",
+                    source="/opt/ml/processing/output/2",
+                    destination=f"s3://{DUMMY_BUCKET}/output-2",
+                ),
+            ],
+            "sm_processing_step_sklearn",
+            True,
+        ],
+        [
+            Contains,
+            [
+                ProcessingOutput(
+                    output_name="output-2",
+                    source="/opt/ml/processing/output/2",
+                    destination=f"s3://{DUMMY_BUCKET}/output-2",
+                ),
+            ],
+            "sm_processing_step_sklearn",
+            True,
+        ],
+    ],
+)
+def test_step_outputs_as_expected_filter(
+    rule, outputs_expected, step_name, success, sagemaker_pipeline
+) -> None:
+    step_outputs_validation = StepOutputsAsExpected(
+        outputs_expected=outputs_expected,
+        step_name=step_name,
+        rule=rule(),
+    )
+    result = step_outputs_validation.run(sagemaker_pipeline)
+    assert result.success == success
```

