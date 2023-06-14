# Comparing `tmp/curia-4.2.0b8.tar.gz` & `tmp/curia-4.2.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curia-4.2.0b8.tar", max compression
+gzip compressed data, was "curia-4.2.0b9.tar", max compression
```

## Comparing `curia-4.2.0b8.tar` & `curia-4.2.0b9.tar`

### file list

```diff
@@ -1,1398 +1,1398 @@
--rw-r--r--   0        0        0     6541 2023-06-13 18:30:19.797963 curia-4.2.0b8/README.md
--rw-r--r--   0        0        0     3988 2023-06-13 18:31:39.940847 curia-4.2.0b8/pyproject.toml
--rw-r--r--   0        0        0       80 2023-06-13 18:31:39.904848 curia-4.2.0b8/src/curia/__init__.py
--rw-r--r--   0        0        0      786 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/.gitignore
--rw-r--r--   0        0        0        6 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/.swagger-codegen/VERSION
--rw-r--r--   0        0        0     1030 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/.swagger-codegen-ignore
--rw-r--r--   0        0        0      349 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/.travis.yml
--rw-r--r--   0        0        0   124667 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/README.md
--rw-r--r--   0        0        0        0 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/__init__.py
--rw-r--r--   0        0        0      292 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AggregationType.md
--rw-r--r--   0        0        0      293 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AllOfCohortModel.md
--rw-r--r--   0        0        0      300 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AllOfCohortOrganization.md
--rw-r--r--   0        0        0      299 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AllOfCohortTrainCohort.md
--rw-r--r--   0        0        0      298 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AllOfDataTableDataset.md
--rw-r--r--   0        0        0      294 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AllOfModelCohorts.md
--rw-r--r--   0        0        0      297 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AllOfModelJobDataset.md
--rw-r--r--   0        0        0      301 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AllOfModelJobEnvironment.md
--rw-r--r--   0        0        0      295 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AllOfModelJobModel.md
--rw-r--r--   0        0        0      297 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AllOfModelJobProject.md
--rw-r--r--   0        0        0      296 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AllOfModelModelJobs.md
--rw-r--r--   0        0        0      294 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AllOfModelProject.md
--rw-r--r--   0        0        0    18774 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AnalysesApi.md
--rw-r--r--   0        0        0     1042 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/Analysis.md
--rw-r--r--   0        0        0     1452 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AnalysisJob.md
--rw-r--r--   0        0        0      417 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobConfig.md
--rw-r--r--   0        0        0      818 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobJoinedProjectResponseDto.md
--rw-r--r--   0        0        0      682 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobOutput.md
--rw-r--r--   0        0        0      841 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobOutputJoinedAnalysisJobJoinedProjectResponseDto.md
--rw-r--r--   0        0        0     1114 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobOutputJoinedAnalysisJobResponseDto.md
--rw-r--r--   0        0        0      772 2023-06-13 18:30:19.797963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobOutputResponseDto.md
--rw-r--r--   0        0        0    20503 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobOutputsApi.md
--rw-r--r--   0        0        0     1045 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobResponseDto.md
--rw-r--r--   0        0        0     1034 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobStatus.md
--rw-r--r--   0        0        0      824 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobStatusJoinedProjectResponseDto.md
--rw-r--r--   0        0        0     1043 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobStatusResponseDto.md
--rw-r--r--   0        0        0    20538 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobStatusesApi.md
--rw-r--r--   0        0        0      292 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobType.md
--rw-r--r--   0        0        0    22862 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnalysisJobsApi.md
--rw-r--r--   0        0        0      815 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnalysisJoinedProjectResponseDto.md
--rw-r--r--   0        0        0      828 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnalysisResponseDto.md
--rw-r--r--   0        0        0      289 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnalysisType.md
--rw-r--r--   0        0        0      307 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnyOfArithmeticExpressionValue.md
--rw-r--r--   0        0        0      304 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnyOfBooleanExpressionValue.md
--rw-r--r--   0        0        0      325 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnyOfCohortDefinitionPatientMetadataFiltersItems.md
--rw-r--r--   0        0        0      296 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/AnyOfConditionValue.md
--rw-r--r--   0        0        0      473 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/ArithmeticExpression.md
--rw-r--r--   0        0        0      295 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/ArithmeticOperator.md
--rw-r--r--   0        0        0      317 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/Body.md
--rw-r--r--   0        0        0      357 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/Body1.md
--rw-r--r--   0        0        0      508 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/Body2.md
--rw-r--r--   0        0        0      361 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/Body3.md
--rw-r--r--   0        0        0      323 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/Body4.md
--rw-r--r--   0        0        0      322 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/Body5.md
--rw-r--r--   0        0        0      578 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/BooleanExpression.md
--rw-r--r--   0        0        0     1037 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/Code.md
--rw-r--r--   0        0        0     1251 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/Cohort.md
--rw-r--r--   0        0        0     1234 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CohortDefinition.md
--rw-r--r--   0        0        0      723 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CohortFilter.md
--rw-r--r--   0        0        0      408 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CohortFilterCondition.md
--rw-r--r--   0        0        0      887 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CohortJoinedCohortResponseDto.md
--rw-r--r--   0        0        0     1192 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CohortJoinedModelJobResponseDto.md
--rw-r--r--   0        0        0     1201 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CohortResponseDto.md
--rw-r--r--   0        0        0     1616 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CohortResults.md
--rw-r--r--   0        0        0      874 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CohortSet.md
--rw-r--r--   0        0        0     1646 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CohortWindow.md
--rw-r--r--   0        0        0    20143 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CohortsApi.md
--rw-r--r--   0        0        0      384 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/Condition.md
--rw-r--r--   0        0        0      294 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/ConditionOperator.md
--rw-r--r--   0        0        0      815 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/ContainerConfig.md
--rw-r--r--   0        0        0      413 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateAnalysisDto.md
--rw-r--r--   0        0        0      635 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateAnalysisJobDto.md
--rw-r--r--   0        0        0      392 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateAnalysisJobOutputDto.md
--rw-r--r--   0        0        0      610 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateAnalysisJobStatusDto.md
--rw-r--r--   0        0        0      531 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateCohortDto.md
--rw-r--r--   0        0        0      533 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateDataQueryDto.md
--rw-r--r--   0        0        0      415 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateDataStoreDto.md
--rw-r--r--   0        0        0      478 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateDataTableDto.md
--rw-r--r--   0        0        0      453 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateDatabaseDto.md
--rw-r--r--   0        0        0      420 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateDatasetColumnDto.md
--rw-r--r--   0        0        0      963 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateDatasetDto.md
--rw-r--r--   0        0        0      684 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateFeatureDto.md
--rw-r--r--   0        0        0      418 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateFeatureStoreDto.md
--rw-r--r--   0        0        0      349 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyAnalysisDto.md
--rw-r--r--   0        0        0      358 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyAnalysisJobDto.md
--rw-r--r--   0        0        0      376 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyAnalysisJobOutputDto.md
--rw-r--r--   0        0        0      376 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyAnalysisJobStatusDto.md
--rw-r--r--   0        0        0      337 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyCodeDto.md
--rw-r--r--   0        0        0      343 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyCohortDto.md
--rw-r--r--   0        0        0      352 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyDataQueryDto.md
--rw-r--r--   0        0        0      352 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyDataStoreDto.md
--rw-r--r--   0        0        0      364 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyDatasetColumnDto.md
--rw-r--r--   0        0        0      346 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyDatasetDto.md
--rw-r--r--   0        0        0      355 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyDatasetJobDto.md
--rw-r--r--   0        0        0      358 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyEnvironmentDto.md
--rw-r--r--   0        0        0      370 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyFeatureCategoryDto.md
--rw-r--r--   0        0        0      346 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyFeatureDto.md
--rw-r--r--   0        0        0      361 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyFeatureStoreDto.md
--rw-r--r--   0        0        0      379 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyFeatureSubCategoryDto.md
--rw-r--r--   0        0        0      355 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyModelBatchDto.md
--rw-r--r--   0        0        0      364 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyModelBatchJobDto.md
--rw-r--r--   0        0        0      361 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyModelDatasetDto.md
--rw-r--r--   0        0        0      340 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyModelDto.md
--rw-r--r--   0        0        0      364 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyModelEndpointDto.md
--rw-r--r--   0        0        0      349 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyModelJobDto.md
--rw-r--r--   0        0        0      367 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyModelJobOutputDto.md
--rw-r--r--   0        0        0      388 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyModelJobOutputFeatureDto.md
--rw-r--r--   0        0        0      370 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyModelPopulationDto.md
--rw-r--r--   0        0        0      361 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyOrganizationDto.md
--rw-r--r--   0        0        0      409 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyOrganizationFeatureExclusionDto.md
--rw-r--r--   0        0        0      382 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyOrganizationSettingDto.md
--rw-r--r--   0        0        0      370 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyPopulationStoreDto.md
--rw-r--r--   0        0        0      346 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyProcessDto.md
--rw-r--r--   0        0        0      355 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyProcessJobDto.md
--rw-r--r--   0        0        0      373 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyProcessJobOutputDto.md
--rw-r--r--   0        0        0      373 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyProcessJobStatusDto.md
--rw-r--r--   0        0        0      346 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyProjectDto.md
--rw-r--r--   0        0        0      364 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyProjectMemberDto.md
--rw-r--r--   0        0        0      352 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManySchedulerDto.md
--rw-r--r--   0        0        0      337 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyTaskDto.md
--rw-r--r--   0        0        0      364 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyTaskExecutionDto.md
--rw-r--r--   0        0        0      382 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyTaskExecutionStatusDto.md
--rw-r--r--   0        0        0      361 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyUserFavoriteDto.md
--rw-r--r--   0        0        0      349 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyWorkflowDto.md
--rw-r--r--   0        0        0      376 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyWorkflowExecutionDto.md
--rw-r--r--   0        0        0      388 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyWorkflowExecutionSpecDto.md
--rw-r--r--   0        0        0      373 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateManyWorkflowTemplateDto.md
--rw-r--r--   0        0        0      370 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateModelBatchDto.md
--rw-r--r--   0        0        0      616 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateModelBatchJobDto.md
--rw-r--r--   0        0        0      648 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateModelDto.md
--rw-r--r--   0        0        0      872 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateModelJobDto.md
--rw-r--r--   0        0        0      431 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateModelJobOutputDto.md
--rw-r--r--   0        0        0      626 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateModelJobStatusDto.md
--rw-r--r--   0        0        0     1131 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateModelPopulationDto.md
--rw-r--r--   0        0        0      405 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateOrganizationDto.md
--rw-r--r--   0        0        0      731 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateOrganizationSettingDto.md
--rw-r--r--   0        0        0      421 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreatePopulationStoreDto.md
--rw-r--r--   0        0        0      430 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateProcessDto.md
--rw-r--r--   0        0        0      620 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateProcessJobDto.md
--rw-r--r--   0        0        0      390 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateProcessJobOutputDto.md
--rw-r--r--   0        0        0      663 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateProcessJobStatusDto.md
--rw-r--r--   0        0        0      457 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateProjectDto.md
--rw-r--r--   0        0        0      433 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateProjectMemberDto.md
--rw-r--r--   0        0        0      647 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateSchedulerDto.md
--rw-r--r--   0        0        0      510 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateTaskDto.md
--rw-r--r--   0        0        0      754 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateTaskExecutionDto.md
--rw-r--r--   0        0        0      434 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateTaskExecutionStatusDto.md
--rw-r--r--   0        0        0      500 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateUserAuditTrailDto.md
--rw-r--r--   0        0        0      437 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateUserFavoriteDto.md
--rw-r--r--   0        0        0      394 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateWorkflowDto.md
--rw-r--r--   0        0        0      554 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateWorkflowExecutionDto.md
--rw-r--r--   0        0        0      525 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateWorkflowExecutionSpecDto.md
--rw-r--r--   0        0        0      438 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateWorkflowExecutionStatusDto.md
--rw-r--r--   0        0        0      555 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/CreateWorkflowTemplateDto.md
--rw-r--r--   0        0        0    19877 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DataQueriesApi.md
--rw-r--r--   0        0        0      947 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DataQuery.md
--rw-r--r--   0        0        0     1322 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DataQueryJoinedDatasetResponseDto.md
--rw-r--r--   0        0        0      938 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DataQueryResponseDto.md
--rw-r--r--   0        0        0      820 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DataStore.md
--rw-r--r--   0        0        0      759 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DataStoreResponseDto.md
--rw-r--r--   0        0        0    17872 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DataStoresApi.md
--rw-r--r--   0        0        0      898 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DataTable.md
--rw-r--r--   0        0        0      801 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DataTableJoinedDatabaseResponseDto.md
--rw-r--r--   0        0        0     1322 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DataTableJoinedDatasetResponseDto.md
--rw-r--r--   0        0        0      985 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DataTableResponseDto.md
--rw-r--r--   0        0        0     8627 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DataTablesApi.md
--rw-r--r--   0        0        0      913 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/Database.md
--rw-r--r--   0        0        0      778 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DatabaseJoinedDataTableResponseDto.md
--rw-r--r--   0        0        0      896 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DatabaseResponseDto.md
--rw-r--r--   0        0        0    11707 2023-06-13 18:30:19.801963 curia-4.2.0b8/src/curia/api/docs/DatabasesApi.md
--rw-r--r--   0        0        0     1788 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/Dataset.md
--rw-r--r--   0        0        0      774 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/DatasetColumn.md
--rw-r--r--   0        0        0     1326 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/DatasetColumnJoinedDatasetResponseDto.md
--rw-r--r--   0        0        0      845 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/DatasetColumnResponseDto.md
--rw-r--r--   0        0        0    18544 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/DatasetColumnsApi.md
--rw-r--r--   0        0        0      898 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/DatasetJob.md
--rw-r--r--   0        0        0      804 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/DatasetJobStatus.md
--rw-r--r--   0        0        0      842 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/DatasetJoinedDataQueryResponseDto.md
--rw-r--r--   0        0        0      741 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/DatasetJoinedDatasetColumnResponseDto.md
--rw-r--r--   0        0        0     1544 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/DatasetResponseDto.md
--rw-r--r--   0        0        0    33268 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/DatasetsApi.md
--rw-r--r--   0        0        0      391 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/DatasetsuploadlargecompleteParts.md
--rw-r--r--   0        0        0     1072 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/Environment.md
--rw-r--r--   0        0        0      674 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/EnvironmentActivity.md
--rw-r--r--   0        0        0     1291 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/Feature.md
--rw-r--r--   0        0        0      877 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/FeatureCategory.md
--rw-r--r--   0        0        0      671 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/FeatureJoinedFeatureSubCategoryJoinedFeatureCategoryResponseDto.md
--rw-r--r--   0        0        0      868 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/FeatureJoinedFeatureSubCategoryResponseDto.md
--rw-r--r--   0        0        0     1499 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/FeatureJoinedModelPopulationResponseDto.md
--rw-r--r--   0        0        0      691 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/FeatureJoinedOrganizationFeatureExclusionResponseDto.md
--rw-r--r--   0        0        0     1434 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/FeatureResponseDto.md
--rw-r--r--   0        0        0      823 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/FeatureStore.md
--rw-r--r--   0        0        0      762 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/FeatureStoreResponseDto.md
--rw-r--r--   0        0        0    18376 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/FeatureStoresApi.md
--rw-r--r--   0        0        0      812 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/FeatureSubCategory.md
--rw-r--r--   0        0        0      789 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/FeatureTable.md
--rw-r--r--   0        0        0    17445 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/FeaturesApi.md
--rw-r--r--   0        0        0      775 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GeographicCounts.md
--rw-r--r--   0        0        0      656 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GeographicQueries.md
--rw-r--r--   0        0        0      519 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyAnalysisJobOutputResponseDto.md
--rw-r--r--   0        0        0      501 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyAnalysisJobResponseDto.md
--rw-r--r--   0        0        0      519 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyAnalysisJobStatusResponseDto.md
--rw-r--r--   0        0        0      492 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyAnalysisResponseDto.md
--rw-r--r--   0        0        0      458 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyCodeResponseDto.md
--rw-r--r--   0        0        0      486 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyCohortResponseDto.md
--rw-r--r--   0        0        0      495 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyDataQueryResponseDto.md
--rw-r--r--   0        0        0      495 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyDataStoreResponseDto.md
--rw-r--r--   0        0        0      495 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyDataTableResponseDto.md
--rw-r--r--   0        0        0      492 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyDatabaseResponseDto.md
--rw-r--r--   0        0        0      507 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyDatasetColumnResponseDto.md
--rw-r--r--   0        0        0      476 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyDatasetJobResponseDto.md
--rw-r--r--   0        0        0      494 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyDatasetJobStatusResponseDto.md
--rw-r--r--   0        0        0      489 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyDatasetResponseDto.md
--rw-r--r--   0        0        0      479 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyEnvironmentResponseDto.md
--rw-r--r--   0        0        0      491 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyFeatureCategoryResponseDto.md
--rw-r--r--   0        0        0      489 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyFeatureResponseDto.md
--rw-r--r--   0        0        0      504 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyFeatureStoreResponseDto.md
--rw-r--r--   0        0        0      500 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyFeatureSubCategoryResponseDto.md
--rw-r--r--   0        0        0      507 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyModelBatchJobResponseDto.md
--rw-r--r--   0        0        0      498 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyModelBatchResponseDto.md
--rw-r--r--   0        0        0      482 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyModelDatasetResponseDto.md
--rw-r--r--   0        0        0      485 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyModelEndpointResponseDto.md
--rw-r--r--   0        0        0      485 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyModelJobEventResponseDto.md
--rw-r--r--   0        0        0      509 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyModelJobOutputFeatureResponseDto.md
--rw-r--r--   0        0        0      510 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyModelJobOutputResponseDto.md
--rw-r--r--   0        0        0      492 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyModelJobResponseDto.md
--rw-r--r--   0        0        0      510 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyModelJobStatusResponseDto.md
--rw-r--r--   0        0        0      513 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyModelPopulationResponseDto.md
--rw-r--r--   0        0        0      483 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyModelResponseDto.md
--rw-r--r--   0        0        0      530 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyOrganizationFeatureExclusionResponseDto.md
--rw-r--r--   0        0        0      504 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyOrganizationResponseDto.md
--rw-r--r--   0        0        0      525 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyOrganizationSettingResponseDto.md
--rw-r--r--   0        0        0      513 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyPopulationStoreResponseDto.md
--rw-r--r--   0        0        0      516 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyProcessJobOutputResponseDto.md
--rw-r--r--   0        0        0      498 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyProcessJobResponseDto.md
--rw-r--r--   0        0        0      516 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyProcessJobStatusResponseDto.md
--rw-r--r--   0        0        0      489 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyProcessResponseDto.md
--rw-r--r--   0        0        0      507 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyProjectMemberResponseDto.md
--rw-r--r--   0        0        0      489 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyProjectResponseDto.md
--rw-r--r--   0        0        0      495 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManySchedulerResponseDto.md
--rw-r--r--   0        0        0      507 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyTaskExecutionResponseDto.md
--rw-r--r--   0        0        0      525 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyTaskExecutionStatusResponseDto.md
--rw-r--r--   0        0        0      480 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyTaskResponseDto.md
--rw-r--r--   0        0        0      510 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyUserAuditTrailResponseDto.md
--rw-r--r--   0        0        0      504 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyUserFavoriteResponseDto.md
--rw-r--r--   0        0        0      519 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyWorkflowExecutionResponseDto.md
--rw-r--r--   0        0        0      531 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyWorkflowExecutionSpecResponseDto.md
--rw-r--r--   0        0        0      537 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyWorkflowExecutionStatusResponseDto.md
--rw-r--r--   0        0        0      492 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyWorkflowResponseDto.md
--rw-r--r--   0        0        0      516 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/GetManyWorkflowTemplateResponseDto.md
--rw-r--r--   0        0        0      615 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/InlineResponse200.md
--rw-r--r--   0        0        0      336 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/InlineResponse200Info.md
--rw-r--r--   0        0        0      615 2023-06-13 18:30:19.805963 curia-4.2.0b8/src/curia/api/docs/InlineResponse503.md
--rw-r--r--   0        0        0    21159 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/InternalApi.md
--rw-r--r--   0        0        0      968 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/InterventionDefinition.md
--rw-r--r--   0        0        0      281 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/Json.md
--rw-r--r--   0        0        0      292 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/LogicalOperator.md
--rw-r--r--   0        0        0     1303 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/Model.md
--rw-r--r--   0        0        0      914 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelBatch.md
--rw-r--r--   0        0        0     1319 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelBatchJob.md
--rw-r--r--   0        0        0      836 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelBatchJobJoinedModelBatchJoinedProjectResponseDto.md
--rw-r--r--   0        0        0      846 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelBatchJobJoinedModelBatchResponseDto.md
--rw-r--r--   0        0        0     1051 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelBatchJobResponseDto.md
--rw-r--r--   0        0        0    25416 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelBatchJobsApi.md
--rw-r--r--   0        0        0      817 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelBatchJoinedProjectResponseDto.md
--rw-r--r--   0        0        0      789 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelBatchResponseDto.md
--rw-r--r--   0        0        0    19271 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelBatchesApi.md
--rw-r--r--   0        0        0      760 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelDataset.md
--rw-r--r--   0        0        0      716 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelEndpoint.md
--rw-r--r--   0        0        0     1899 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJob.md
--rw-r--r--   0        0        0      698 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobConfig.md
--rw-r--r--   0        0        0      946 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobEvent.md
--rw-r--r--   0        0        0      889 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedCohortResponseDto.md
--rw-r--r--   0        0        0      843 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedDataQueryResponseDto.md
--rw-r--r--   0        0        0     1321 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedDatasetResponseDto.md
--rw-r--r--   0        0        0      691 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedFeatureSubCategoryResponseDto.md
--rw-r--r--   0        0        0      753 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelJobOutputResponseDto.md
--rw-r--r--   0        0        0      948 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelJobStatusResponseDto.md
--rw-r--r--   0        0        0      762 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedCohortDefinitionJoinedPeriodDefinitionResponseDto.md
--rw-r--r--   0        0        0     1116 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedCohortDefinitionResponseDto.md
--rw-r--r--   0        0        0     1357 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedDataQueryJoinedDatasetResponseDto.md
--rw-r--r--   0        0        0     1043 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedDataQueryResponseDto.md
--rw-r--r--   0        0        0      802 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedInterventionDefinitionResponseDto.md
--rw-r--r--   0        0        0      969 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedOutcomeDefinitionResponseDto.md
--rw-r--r--   0        0        0     2176 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationResponseDto.md
--rw-r--r--   0        0        0      970 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelResponseDto.md
--rw-r--r--   0        0        0      815 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedProjectResponseDto.md
--rw-r--r--   0        0        0      846 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobOutput.md
--rw-r--r--   0        0        0      738 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobOutputFeature.md
--rw-r--r--   0        0        0     1327 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobOutputJoinedDatasetResponseDto.md
--rw-r--r--   0        0        0      835 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobOutputJoinedModelJobJoinedProjectResponseDto.md
--rw-r--r--   0        0        0     1347 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobOutputJoinedModelJobResponseDto.md
--rw-r--r--   0        0        0      981 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobOutputResponseDto.md
--rw-r--r--   0        0        0    18734 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobOutputsApi.md
--rw-r--r--   0        0        0     2268 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobResponseDto.md
--rw-r--r--   0        0        0     1041 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobStatus.md
--rw-r--r--   0        0        0      835 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobStatusJoinedModelJobJoinedProjectResponseDto.md
--rw-r--r--   0        0        0     1347 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobStatusJoinedModelJobResponseDto.md
--rw-r--r--   0        0        0     1057 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobStatusResponseDto.md
--rw-r--r--   0        0        0    10815 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobStatusesApi.md
--rw-r--r--   0        0        0    24358 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJobsApi.md
--rw-r--r--   0        0        0     1203 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJoinedCohortJoinedModelJobResponseDto.md
--rw-r--r--   0        0        0     1016 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJoinedCohortResponseDto.md
--rw-r--r--   0        0        0      900 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJoinedModelJobJoinedCohortResponseDto.md
--rw-r--r--   0        0        0     1332 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJoinedModelJobJoinedDatasetResponseDto.md
--rw-r--r--   0        0        0      702 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJoinedModelJobJoinedFeatureSubCategoryResponseDto.md
--rw-r--r--   0        0        0     1612 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJoinedModelJobResponseDto.md
--rw-r--r--   0        0        0     1231 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJoinedModelOutputDetailsResponseDto.md
--rw-r--r--   0        0        0      812 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJoinedProjectResponseDto.md
--rw-r--r--   0        0        0      756 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelJoinedUserFavoriteResponseDto.md
--rw-r--r--   0        0        0     1260 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelOutputDetails.md
--rw-r--r--   0        0        0     2231 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelPopulation.md
--rw-r--r--   0        0        0      748 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedCohortDefinitionJoinedPeriodDefinitionResponseDto.md
--rw-r--r--   0        0        0     1074 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedCohortDefinitionResponseDto.md
--rw-r--r--   0        0        0     1038 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedCohortResultsResponseDto.md
--rw-r--r--   0        0        0     1343 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedDataQueryJoinedDatasetResponseDto.md
--rw-r--r--   0        0        0     1001 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedDataQueryResponseDto.md
--rw-r--r--   0        0        0     1013 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedFeatureResponseDto.md
--rw-r--r--   0        0        0      788 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedInterventionDefinitionResponseDto.md
--rw-r--r--   0        0        0      991 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedModelJobJoinedModelResponseDto.md
--rw-r--r--   0        0        0     1344 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedModelJobResponseDto.md
--rw-r--r--   0        0        0      955 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedOutcomeDefinitionResponseDto.md
--rw-r--r--   0        0        0     2592 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelPopulationResponseDto.md
--rw-r--r--   0        0        0    20616 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelPopulationsApi.md
--rw-r--r--   0        0        0     1516 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelResponseDto.md
--rw-r--r--   0        0        0    21791 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/ModelsApi.md
--rw-r--r--   0        0        0      283 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/Object.md
--rw-r--r--   0        0        0     2124 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/Organization.md
--rw-r--r--   0        0        0      807 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/OrganizationFeatureCategoryExclusion.md
--rw-r--r--   0        0        0      796 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/OrganizationFeatureExclusion.md
--rw-r--r--   0        0        0      713 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/OrganizationResponseDto.md
--rw-r--r--   0        0        0     1136 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/OrganizationSetting.md
--rw-r--r--   0        0        0     1075 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/OrganizationSettingResponseDto.md
--rw-r--r--   0        0        0    23020 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/OrganizationSettingsApi.md
--rw-r--r--   0        0        0    18327 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/OrganizationsApi.md
--rw-r--r--   0        0        0     1135 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/OutcomeDefinition.md
--rw-r--r--   0        0        0      388 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/PeriodDefinition.md
--rw-r--r--   0        0        0      287 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/PeriodType.md
--rw-r--r--   0        0        0      510 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/PersonSet.md
--rw-r--r--   0        0        0      381 2023-06-13 18:30:19.809963 curia-4.2.0b8/src/curia/api/docs/PipelineConfig.md
--rw-r--r--   0        0        0   600317 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/PlatformApi.md
--rw-r--r--   0        0        0     1268 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/Population.md
--rw-r--r--   0        0        0      899 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/PopulationStore.md
--rw-r--r--   0        0        0      765 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/PopulationStoreResponseDto.md
--rw-r--r--   0        0        0    18880 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/PopulationStoresApi.md
--rw-r--r--   0        0        0      918 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/Process.md
--rw-r--r--   0        0        0     1264 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJob.md
--rw-r--r--   0        0        0      386 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJobConfig.md
--rw-r--r--   0        0        0      817 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJobJoinedProjectResponseDto.md
--rw-r--r--   0        0        0      743 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJobOutput.md
--rw-r--r--   0        0        0      839 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJobOutputJoinedProcessJobJoinedProjectResponseDto.md
--rw-r--r--   0        0        0     1105 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJobOutputJoinedProcessJobResponseDto.md
--rw-r--r--   0        0        0      831 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJobOutputResponseDto.md
--rw-r--r--   0        0        0    20335 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJobOutputsApi.md
--rw-r--r--   0        0        0     1039 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJobResponseDto.md
--rw-r--r--   0        0        0     1084 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJobStatus.md
--rw-r--r--   0        0        0      823 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJobStatusJoinedProjectResponseDto.md
--rw-r--r--   0        0        0     1094 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJobStatusResponseDto.md
--rw-r--r--   0        0        0    20370 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJobStatusesApi.md
--rw-r--r--   0        0        0    22718 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJobsApi.md
--rw-r--r--   0        0        0      814 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessJoinedProjectResponseDto.md
--rw-r--r--   0        0        0      843 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessResponseDto.md
--rw-r--r--   0        0        0      288 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessType.md
--rw-r--r--   0        0        0    18676 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProcessesApi.md
--rw-r--r--   0        0        0     1452 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/Project.md
--rw-r--r--   0        0        0      899 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProjectJoinedModelJoinedCohortResponseDto.md
--rw-r--r--   0        0        0     1094 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProjectJoinedModelResponseDto.md
--rw-r--r--   0        0        0      814 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProjectJoinedProjectResponseDto.md
--rw-r--r--   0        0        0      758 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProjectJoinedUserFavoriteResponseDto.md
--rw-r--r--   0        0        0      787 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProjectMember.md
--rw-r--r--   0        0        0      820 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProjectMemberJoinedProjectResponseDto.md
--rw-r--r--   0        0        0      858 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProjectMemberResponseDto.md
--rw-r--r--   0        0        0    18544 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProjectMembersApi.md
--rw-r--r--   0        0        0     1250 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProjectResponseDto.md
--rw-r--r--   0        0        0    22464 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/ProjectsApi.md
--rw-r--r--   0        0        0     1112 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/Scheduler.md
--rw-r--r--   0        0        0    17759 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/SchedulerApi.md
--rw-r--r--   0        0        0      753 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/SchedulerJoinedWorkflowResponseDto.md
--rw-r--r--   0        0        0     1103 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/SchedulerResponseDto.md
--rw-r--r--   0        0        0      500 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/SelectExpression.md
--rw-r--r--   0        0        0      288 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/SetOperator.md
--rw-r--r--   0        0        0      425 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/StateData.md
--rw-r--r--   0        0        0      993 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/Task.md
--rw-r--r--   0        0        0     1275 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/TaskExecution.md
--rw-r--r--   0        0        0      873 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/TaskExecutionJoinedTaskResponseDto.md
--rw-r--r--   0        0        0      917 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/TaskExecutionJoinedWorkflowExecutionResponseDto.md
--rw-r--r--   0        0        0     1318 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/TaskExecutionResponseDto.md
--rw-r--r--   0        0        0      802 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/TaskExecutionStatus.md
--rw-r--r--   0        0        0      942 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/TaskExecutionStatusJoinedTaskExecutionJoinedWorkflowExecutionResponseDto.md
--rw-r--r--   0        0        0     1285 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/TaskExecutionStatusJoinedTaskExecutionResponseDto.md
--rw-r--r--   0        0        0      885 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/TaskExecutionStatusResponseDto.md
--rw-r--r--   0        0        0      287 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/TaskInputs.md
--rw-r--r--   0        0        0      288 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/TaskOutputs.md
--rw-r--r--   0        0        0      854 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/TaskResponseDto.md
--rw-r--r--   0        0        0    21547 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/TasksApi.md
--rw-r--r--   0        0        0      446 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/UpdateAnalysisDto.md
--rw-r--r--   0        0        0      668 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/UpdateAnalysisJobDto.md
--rw-r--r--   0        0        0      425 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/UpdateAnalysisJobOutputDto.md
--rw-r--r--   0        0        0      665 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/UpdateAnalysisJobStatusDto.md
--rw-r--r--   0        0        0      542 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/UpdateCohortDto.md
--rw-r--r--   0        0        0      544 2023-06-13 18:30:19.813963 curia-4.2.0b8/src/curia/api/docs/UpdateDataQueryDto.md
--rw-r--r--   0        0        0      415 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateDataStoreDto.md
--rw-r--r--   0        0        0      500 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateDataTableDto.md
--rw-r--r--   0        0        0      464 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateDatabaseDto.md
--rw-r--r--   0        0        0      453 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateDatasetColumnDto.md
--rw-r--r--   0        0        0      985 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateDatasetDto.md
--rw-r--r--   0        0        0      794 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateFeatureDto.md
--rw-r--r--   0        0        0      418 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateFeatureStoreDto.md
--rw-r--r--   0        0        0      381 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateModelBatchDto.md
--rw-r--r--   0        0        0      649 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateModelBatchJobDto.md
--rw-r--r--   0        0        0      692 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateModelDto.md
--rw-r--r--   0        0        0      905 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateModelJobDto.md
--rw-r--r--   0        0        0      464 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateModelJobOutputDto.md
--rw-r--r--   0        0        0      659 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateModelJobStatusDto.md
--rw-r--r--   0        0        0     1131 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateModelPopulationDto.md
--rw-r--r--   0        0        0      416 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateOrganizationDto.md
--rw-r--r--   0        0        0      742 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateOrganizationSettingDto.md
--rw-r--r--   0        0        0      421 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdatePopulationStoreDto.md
--rw-r--r--   0        0        0      452 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateProcessDto.md
--rw-r--r--   0        0        0      642 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateProcessJobDto.md
--rw-r--r--   0        0        0      423 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateProcessJobOutputDto.md
--rw-r--r--   0        0        0      663 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateProcessJobStatusDto.md
--rw-r--r--   0        0        0      468 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateProjectDto.md
--rw-r--r--   0        0        0      466 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateProjectMemberDto.md
--rw-r--r--   0        0        0      691 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateSchedulerDto.md
--rw-r--r--   0        0        0      532 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateTaskDto.md
--rw-r--r--   0        0        0      776 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateTaskExecutionDto.md
--rw-r--r--   0        0        0      467 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateTaskExecutionStatusDto.md
--rw-r--r--   0        0        0      555 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateUserAuditTrailDto.md
--rw-r--r--   0        0        0      736 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateUserDto.md
--rw-r--r--   0        0        0      437 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateUserFavoriteDto.md
--rw-r--r--   0        0        0      416 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateWorkflowDto.md
--rw-r--r--   0        0        0      565 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateWorkflowExecutionDto.md
--rw-r--r--   0        0        0      547 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateWorkflowExecutionSpecDto.md
--rw-r--r--   0        0        0      471 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateWorkflowExecutionStatusDto.md
--rw-r--r--   0        0        0      577 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UpdateWorkflowTemplateDto.md
--rw-r--r--   0        0        0      708 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UserAuditTrail.md
--rw-r--r--   0        0        0     8869 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UserAuditTrailApi.md
--rw-r--r--   0        0        0      686 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UserAuditTrailResponseDto.md
--rw-r--r--   0        0        0      842 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UserFavorite.md
--rw-r--r--   0        0        0      830 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UserFavoriteJoinedModelJoinedProjectResponseDto.md
--rw-r--r--   0        0        0     1111 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UserFavoriteJoinedModelResponseDto.md
--rw-r--r--   0        0        0      854 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UserFavoriteResponseDto.md
--rw-r--r--   0        0        0    18376 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UserFavoritesApi.md
--rw-r--r--   0        0        0    29151 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/UserManagementApi.md
--rw-r--r--   0        0        0     1031 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/Workflow.md
--rw-r--r--   0        0        0     1197 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowExecution.md
--rw-r--r--   0        0        0      898 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionResponseDto.md
--rw-r--r--   0        0        0      901 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionSpec.md
--rw-r--r--   0        0        0      925 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionSpecJoinedWorkflowExecutionResponseDto.md
--rw-r--r--   0        0        0      988 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionSpecResponseDto.md
--rw-r--r--   0        0        0      814 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionStatus.md
--rw-r--r--   0        0        0      927 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionStatusJoinedWorkflowExecutionResponseDto.md
--rw-r--r--   0        0        0      905 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionStatusResponseDto.md
--rw-r--r--   0        0        0     1005 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowJoinedSchedulerResponseDto.md
--rw-r--r--   0        0        0      912 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowJoinedWorkflowExecutionResponseDto.md
--rw-r--r--   0        0        0      913 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowJoinedWorkflowTemplateResponseDto.md
--rw-r--r--   0        0        0     1108 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowResponseDto.md
--rw-r--r--   0        0        0     1020 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowTemplate.md
--rw-r--r--   0        0        0      511 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowTemplateDefinition.md
--rw-r--r--   0        0        0      303 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowTemplateParameters.md
--rw-r--r--   0        0        0      899 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowTemplateResponseDto.md
--rw-r--r--   0        0        0    39666 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/WorkflowsApi.md
--rw-r--r--   0        0        0      421 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/docs/ZipData.md
--rw-r--r--   0        0        0     1663 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/git_push.sh
--rw-r--r--   0        0        0       96 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/requirements.txt
--rw-r--r--   0        0        0     1004 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/setup.py
--rw-r--r--   0        0        0    31428 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/swagger_client/__init__.py
--rw-r--r--   0        0        0     2061 2023-06-13 18:30:19.817963 curia-4.2.0b8/src/curia/api/swagger_client/api/__init__.py
--rw-r--r--   0        0        0    33328 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/analyses_api.py
--rw-r--r--   0        0        0    35040 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/analysis_job_outputs_api.py
--rw-r--r--   0        0        0    35052 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/analysis_job_statuses_api.py
--rw-r--r--   0        0        0    40946 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/analysis_jobs_api.py
--rw-r--r--   0        0        0    39722 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/cohorts_api.py
--rw-r--r--   0        0        0    37585 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/data_queries_api.py
--rw-r--r--   0        0        0    33603 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/data_stores_api.py
--rw-r--r--   0        0        0    13421 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/data_tables_api.py
--rw-r--r--   0        0        0    19439 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/databases_api.py
--rw-r--r--   0        0        0    34251 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/dataset_columns_api.py
--rw-r--r--   0        0        0    67869 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/datasets_api.py
--rw-r--r--   0        0        0    34089 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/feature_stores_api.py
--rw-r--r--   0        0        0    33158 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/features_api.py
--rw-r--r--   0        0        0    40513 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/internal_api.py
--rw-r--r--   0        0        0    45647 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/model_batch_jobs_api.py
--rw-r--r--   0        0        0    33797 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/model_batches_api.py
--rw-r--r--   0        0        0    34483 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/model_job_outputs_api.py
--rw-r--r--   0        0        0    17685 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/model_job_statuses_api.py
--rw-r--r--   0        0        0    48185 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/model_jobs_api.py
--rw-r--r--   0        0        0    38516 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/model_populations_api.py
--rw-r--r--   0        0        0    43120 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/models_api.py
--rw-r--r--   0        0        0    41842 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/organization_settings_api.py
--rw-r--r--   0        0        0    34025 2023-06-13 18:30:19.821963 curia-4.2.0b8/src/curia/api/swagger_client/api/organizations_api.py
--rw-r--r--   0        0        0  1122558 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/platform_api.py
--rw-r--r--   0        0        0    34575 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/population_stores_api.py
--rw-r--r--   0        0        0    34878 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/process_job_outputs_api.py
--rw-r--r--   0        0        0    34890 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/process_job_statuses_api.py
--rw-r--r--   0        0        0    40786 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/process_jobs_api.py
--rw-r--r--   0        0        0    33190 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/processes_api.py
--rw-r--r--   0        0        0    34251 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/project_members_api.py
--rw-r--r--   0        0        0    43631 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/projects_api.py
--rw-r--r--   0        0        0    33481 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/scheduler_api.py
--rw-r--r--   0        0        0    42423 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/tasks_api.py
--rw-r--r--   0        0        0    13665 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/user_audit_trail_api.py
--rw-r--r--   0        0        0    34089 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/user_favorites_api.py
--rw-r--r--   0        0        0    60855 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/user_management_api.py
--rw-r--r--   0        0        0    74957 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api/workflows_api.py
--rw-r--r--   0        0        0    24824 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/api_client.py
--rw-r--r--   0        0        0     8257 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/configuration.py
--rw-r--r--   0        0        0    29282 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     2579 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/models/aggregation_type.py
--rw-r--r--   0        0        0     2804 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_cohort_model.py
--rw-r--r--   0        0        0     2888 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_cohort_organization.py
--rw-r--r--   0        0        0     2836 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_cohort_train_cohort.py
--rw-r--r--   0        0        0     2820 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_data_table_dataset.py
--rw-r--r--   0        0        0     2816 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_cohorts.py
--rw-r--r--   0        0        0     2836 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_job_dataset.py
--rw-r--r--   0        0        0     2884 2023-06-13 18:30:19.825963 curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_job_environment.py
--rw-r--r--   0        0        0     2812 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_job_model.py
--rw-r--r--   0        0        0     2836 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_job_project.py
--rw-r--r--   0        0        0     2841 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_model_jobs.py
--rw-r--r--   0        0        0     2824 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_project.py
--rw-r--r--   0        0        0    13573 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis.py
--rw-r--r--   0        0        0    18641 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job.py
--rw-r--r--   0        0        0     5946 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_config.py
--rw-r--r--   0        0        0    12323 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_joined_project_response_dto.py
--rw-r--r--   0        0        0    11100 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_output.py
--rw-r--r--   0        0        0    13519 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_joined_project_response_dto.py
--rw-r--r--   0        0        0    16307 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_response_dto.py
--rw-r--r--   0        0        0    11639 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_output_response_dto.py
--rw-r--r--   0        0        0    14674 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_response_dto.py
--rw-r--r--   0        0        0    15317 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_status.py
--rw-r--r--   0        0        0    12635 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_status_joined_project_response_dto.py
--rw-r--r--   0        0        0    15431 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_status_response_dto.py
--rw-r--r--   0        0        0     2549 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_type.py
--rw-r--r--   0        0        0    12167 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_joined_project_response_dto.py
--rw-r--r--   0        0        0    11343 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_response_dto.py
--rw-r--r--   0        0        0     2521 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_type.py
--rw-r--r--   0        0        0     2514 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/any_of_arithmetic_expression_value.py
--rw-r--r--   0        0        0     2502 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/any_of_boolean_expression_value.py
--rw-r--r--   0        0        0     2586 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/any_of_cohort_definition_patient_metadata_filters_items.py
--rw-r--r--   0        0        0     2470 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/any_of_condition_value.py
--rw-r--r--   0        0        0     4635 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/arithmetic_expression.py
--rw-r--r--   0        0        0     2685 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/arithmetic_operator.py
--rw-r--r--   0        0        0     2962 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/body.py
--rw-r--r--   0        0        0     3545 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/body1.py
--rw-r--r--   0        0        0     4880 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/body2.py
--rw-r--r--   0        0        0     3657 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/body3.py
--rw-r--r--   0        0        0     3069 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/body4.py
--rw-r--r--   0        0        0     3015 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/body5.py
--rw-r--r--   0        0        0     6747 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/boolean_expression.py
--rw-r--r--   0        0        0    15654 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/code.py
--rw-r--r--   0        0        0    15747 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/cohort.py
--rw-r--r--   0        0        0    15751 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_definition.py
--rw-r--r--   0        0        0    10333 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_filter.py
--rw-r--r--   0        0        0     5722 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_filter_condition.py
--rw-r--r--   0        0        0    12768 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_joined_cohort_response_dto.py
--rw-r--r--   0        0        0    19274 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_joined_model_job_response_dto.py
--rw-r--r--   0        0        0    14684 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_response_dto.py
--rw-r--r--   0        0        0    22225 2023-06-13 18:30:19.829963 curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_results.py
--rw-r--r--   0        0        0    10728 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_set.py
--rw-r--r--   0        0        0    24287 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_window.py
--rw-r--r--   0        0        0     4438 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/condition.py
--rw-r--r--   0        0        0     2702 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/condition_operator.py
--rw-r--r--   0        0        0    11475 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/container_config.py
--rw-r--r--   0        0        0     5531 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_analysis_dto.py
--rw-r--r--   0        0        0     8644 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_analysis_job_dto.py
--rw-r--r--   0        0        0     4881 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_analysis_job_output_dto.py
--rw-r--r--   0        0        0     9264 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_analysis_job_status_dto.py
--rw-r--r--   0        0        0     6174 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_cohort_dto.py
--rw-r--r--   0        0        0     6672 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_data_query_dto.py
--rw-r--r--   0        0        0     4465 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_data_store_dto.py
--rw-r--r--   0        0        0     6098 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_data_table_dto.py
--rw-r--r--   0        0        0     5373 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_database_dto.py
--rw-r--r--   0        0        0     5411 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_dataset_column_dto.py
--rw-r--r--   0        0        0    14417 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_dataset_dto.py
--rw-r--r--   0        0        0    12449 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_feature_dto.py
--rw-r--r--   0        0        0     4513 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_feature_store_dto.py
--rw-r--r--   0        0        0     3204 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_analysis_dto.py
--rw-r--r--   0        0        0     3237 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_analysis_job_dto.py
--rw-r--r--   0        0        0     3303 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_analysis_job_output_dto.py
--rw-r--r--   0        0        0     3303 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_analysis_job_status_dto.py
--rw-r--r--   0        0        0     3161 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_code_dto.py
--rw-r--r--   0        0        0     3192 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_cohort_dto.py
--rw-r--r--   0        0        0     3225 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_data_query_dto.py
--rw-r--r--   0        0        0     3225 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_data_store_dto.py
--rw-r--r--   0        0        0     3269 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_dataset_column_dto.py
--rw-r--r--   0        0        0     3203 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_dataset_dto.py
--rw-r--r--   0        0        0     3226 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_dataset_job_dto.py
--rw-r--r--   0        0        0     3237 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_environment_dto.py
--rw-r--r--   0        0        0     3282 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_feature_category_dto.py
--rw-r--r--   0        0        0     3203 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_feature_dto.py
--rw-r--r--   0        0        0     3258 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_feature_store_dto.py
--rw-r--r--   0        0        0     3315 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_feature_sub_category_dto.py
--rw-r--r--   0        0        0     3226 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_batch_dto.py
--rw-r--r--   0        0        0     3259 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_batch_job_dto.py
--rw-r--r--   0        0        0     3248 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_dataset_dto.py
--rw-r--r--   0        0        0     3181 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_dto.py
--rw-r--r--   0        0        0     3259 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_endpoint_dto.py
--rw-r--r--   0        0        0     3214 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_job_dto.py
--rw-r--r--   0        0        0     3280 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_job_output_dto.py
--rw-r--r--   0        0        0     3348 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_job_output_feature_dto.py
--rw-r--r--   0        0        0     3291 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_population_dto.py
--rw-r--r--   0        0        0     3258 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_organization_dto.py
--rw-r--r--   0        0        0     3425 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_organization_feature_exclusion_dto.py
--rw-r--r--   0        0        0     3335 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_organization_setting_dto.py
--rw-r--r--   0        0        0     3291 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_population_store_dto.py
--rw-r--r--   0        0        0     3193 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_process_dto.py
--rw-r--r--   0        0        0     3226 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_process_job_dto.py
--rw-r--r--   0        0        0     3292 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_process_job_output_dto.py
--rw-r--r--   0        0        0     3292 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_process_job_status_dto.py
--rw-r--r--   0        0        0     3203 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_project_dto.py
--rw-r--r--   0        0        0     3269 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_project_member_dto.py
--rw-r--r--   0        0        0     3225 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_scheduler_dto.py
--rw-r--r--   0        0        0     3170 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_task_dto.py
--rw-r--r--   0        0        0     3269 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_task_execution_dto.py
--rw-r--r--   0        0        0     3335 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_task_execution_status_dto.py
--rw-r--r--   0        0        0     3258 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_user_favorite_dto.py
--rw-r--r--   0        0        0     3214 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_workflow_dto.py
--rw-r--r--   0        0        0     3313 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_workflow_execution_dto.py
--rw-r--r--   0        0        0     3357 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_workflow_execution_spec_dto.py
--rw-r--r--   0        0        0     3302 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_workflow_template_dto.py
--rw-r--r--   0        0        0     4024 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_batch_dto.py
--rw-r--r--   0        0        0     9127 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_batch_job_dto.py
--rw-r--r--   0        0        0    10402 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_dto.py
--rw-r--r--   0        0        0    13134 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_job_dto.py
--rw-r--r--   0        0        0     5529 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_job_output_dto.py
--rw-r--r--   0        0        0     8923 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_job_status_dto.py
--rw-r--r--   0        0        0    17030 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_population_dto.py
--rw-r--r--   0        0        0     4606 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_organization_dto.py
--rw-r--r--   0        0        0    10373 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_organization_setting_dto.py
--rw-r--r--   0        0        0     4561 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_population_store_dto.py
--rw-r--r--   0        0        0     5717 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_process_dto.py
--rw-r--r--   0        0        0     8417 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_process_job_dto.py
--rw-r--r--   0        0        0     4844 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_process_job_output_dto.py
--rw-r--r--   0        0        0     8770 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_process_job_status_dto.py
--rw-r--r--   0        0        0     5503 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_project_dto.py
--rw-r--r--   0        0        0     5654 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_project_member_dto.py
--rw-r--r--   0        0        0     8781 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_scheduler_dto.py
--rw-r--r--   0        0        0     6113 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_task_dto.py
--rw-r--r--   0        0        0     9916 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_task_execution_dto.py
--rw-r--r--   0        0        0     5645 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_task_execution_status_dto.py
--rw-r--r--   0        0        0     7646 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_user_audit_trail_dto.py
--rw-r--r--   0        0        0     4939 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_user_favorite_dto.py
--rw-r--r--   0        0        0     4712 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_workflow_dto.py
--rw-r--r--   0        0        0     6968 2023-06-13 18:30:19.833963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_workflow_execution_dto.py
--rw-r--r--   0        0        0     5185 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_workflow_execution_spec_dto.py
--rw-r--r--   0        0        0     5725 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_workflow_execution_status_dto.py
--rw-r--r--   0        0        0     5707 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/create_workflow_template_dto.py
--rw-r--r--   0        0        0    12708 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/data_query.py
--rw-r--r--   0        0        0    21959 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/data_query_joined_dataset_response_dto.py
--rw-r--r--   0        0        0    12694 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/data_query_response_dto.py
--rw-r--r--   0        0        0    10691 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/data_store.py
--rw-r--r--   0        0        0    10467 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/data_store_response_dto.py
--rw-r--r--   0        0        0    12128 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/data_table.py
--rw-r--r--   0        0        0    12212 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/data_table_joined_database_response_dto.py
--rw-r--r--   0        0        0    21959 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/data_table_joined_dataset_response_dto.py
--rw-r--r--   0        0        0    12902 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/data_table_response_dto.py
--rw-r--r--   0        0        0    12245 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/database.py
--rw-r--r--   0        0        0    12089 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/database_joined_data_table_response_dto.py
--rw-r--r--   0        0        0    12170 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/database_response_dto.py
--rw-r--r--   0        0        0    24496 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/dataset.py
--rw-r--r--   0        0        0    10736 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_column.py
--rw-r--r--   0        0        0    22359 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_column_joined_dataset_response_dto.py
--rw-r--r--   0        0        0    11398 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_column_response_dto.py
--rw-r--r--   0        0        0    11516 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_job.py
--rw-r--r--   0        0        0    11875 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_job_status.py
--rw-r--r--   0        0        0    12663 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_joined_data_query_response_dto.py
--rw-r--r--   0        0        0    11235 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_joined_dataset_column_response_dto.py
--rw-r--r--   0        0        0    22191 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_response_dto.py
--rw-r--r--   0        0        0     4007 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/datasetsuploadlargecomplete_parts.py
--rw-r--r--   0        0        0    14049 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/environment.py
--rw-r--r--   0        0        0     9848 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/environment_activity.py
--rw-r--r--   0        0        0    19679 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/feature.py
--rw-r--r--   0        0        0    10474 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/feature_category.py
--rw-r--r--   0        0        0     9769 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_joined_feature_category_response_dto.py
--rw-r--r--   0        0        0    11222 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_response_dto.py
--rw-r--r--   0        0        0    24534 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/feature_joined_model_population_response_dto.py
--rw-r--r--   0        0        0    10642 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/feature_joined_organization_feature_exclusion_response_dto.py
--rw-r--r--   0        0        0    20827 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/feature_response_dto.py
--rw-r--r--   0        0        0    10847 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/feature_store.py
--rw-r--r--   0        0        0    10611 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/feature_store_response_dto.py
--rw-r--r--   0        0        0    10733 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/feature_sub_category.py
--rw-r--r--   0        0        0    12122 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/feature_table.py
--rw-r--r--   0        0        0     8403 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/geographic_counts.py
--rw-r--r--   0        0        0     8947 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/geographic_queries.py
--rw-r--r--   0        0        0     6575 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_analysis_job_output_response_dto.py
--rw-r--r--   0        0        0     6413 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_analysis_job_response_dto.py
--rw-r--r--   0        0        0     6575 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_analysis_job_status_response_dto.py
--rw-r--r--   0        0        0     6332 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_analysis_response_dto.py
--rw-r--r--   0        0        0     6192 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_code_response_dto.py
--rw-r--r--   0        0        0     6288 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_cohort_response_dto.py
--rw-r--r--   0        0        0     6369 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_data_query_response_dto.py
--rw-r--r--   0        0        0     6369 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_data_store_response_dto.py
--rw-r--r--   0        0        0     6369 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_data_table_response_dto.py
--rw-r--r--   0        0        0     6342 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_database_response_dto.py
--rw-r--r--   0        0        0     6477 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_dataset_column_response_dto.py
--rw-r--r--   0        0        0     6353 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_dataset_job_response_dto.py
--rw-r--r--   0        0        0     6515 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_dataset_job_status_response_dto.py
--rw-r--r--   0        0        0     6315 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_dataset_response_dto.py
--rw-r--r--   0        0        0     6380 2023-06-13 18:30:19.837963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_environment_response_dto.py
--rw-r--r--   0        0        0     6489 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_feature_category_response_dto.py
--rw-r--r--   0        0        0     6315 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_feature_response_dto.py
--rw-r--r--   0        0        0     6450 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_feature_store_response_dto.py
--rw-r--r--   0        0        0     6570 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_feature_sub_category_response_dto.py
--rw-r--r--   0        0        0     6467 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_batch_job_response_dto.py
--rw-r--r--   0        0        0     6386 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_batch_response_dto.py
--rw-r--r--   0        0        0     6407 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_dataset_response_dto.py
--rw-r--r--   0        0        0     6434 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_endpoint_response_dto.py
--rw-r--r--   0        0        0     6434 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_job_event_response_dto.py
--rw-r--r--   0        0        0     6651 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_job_output_feature_response_dto.py
--rw-r--r--   0        0        0     6504 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_job_output_response_dto.py
--rw-r--r--   0        0        0     6342 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_job_response_dto.py
--rw-r--r--   0        0        0     6504 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_job_status_response_dto.py
--rw-r--r--   0        0        0     6531 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_population_response_dto.py
--rw-r--r--   0        0        0     6261 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_response_dto.py
--rw-r--r--   0        0        0     6840 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_organization_feature_exclusion_response_dto.py
--rw-r--r--   0        0        0     6450 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_organization_response_dto.py
--rw-r--r--   0        0        0     6639 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_organization_setting_response_dto.py
--rw-r--r--   0        0        0     6531 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_population_store_response_dto.py
--rw-r--r--   0        0        0     6548 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_process_job_output_response_dto.py
--rw-r--r--   0        0        0     6386 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_process_job_response_dto.py
--rw-r--r--   0        0        0     6548 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_process_job_status_response_dto.py
--rw-r--r--   0        0        0     6305 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_process_response_dto.py
--rw-r--r--   0        0        0     6477 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_project_member_response_dto.py
--rw-r--r--   0        0        0     6315 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_project_response_dto.py
--rw-r--r--   0        0        0     6369 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_scheduler_response_dto.py
--rw-r--r--   0        0        0     6477 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_task_execution_response_dto.py
--rw-r--r--   0        0        0     6639 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_task_execution_status_response_dto.py
--rw-r--r--   0        0        0     6234 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_task_response_dto.py
--rw-r--r--   0        0        0     6504 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_user_audit_trail_response_dto.py
--rw-r--r--   0        0        0     6450 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_user_favorite_response_dto.py
--rw-r--r--   0        0        0     6585 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_workflow_execution_response_dto.py
--rw-r--r--   0        0        0     6693 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_workflow_execution_spec_response_dto.py
--rw-r--r--   0        0        0     6747 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_workflow_execution_status_response_dto.py
--rw-r--r--   0        0        0     6342 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_workflow_response_dto.py
--rw-r--r--   0        0        0     6558 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_workflow_template_response_dto.py
--rw-r--r--   0        0        0     5229 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/inline_response200.py
--rw-r--r--   0        0        0     3129 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/inline_response200_info.py
--rw-r--r--   0        0        0     5229 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/inline_response503.py
--rw-r--r--   0        0        0    12256 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/intervention_definition.py
--rw-r--r--   0        0        0     2419 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/json.py
--rw-r--r--   0        0        0     2541 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/logical_operator.py
--rw-r--r--   0        0        0    18333 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model.py
--rw-r--r--   0        0        0    11239 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch.py
--rw-r--r--   0        0        0    18191 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch_job.py
--rw-r--r--   0        0        0    13259 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_joined_project_response_dto.py
--rw-r--r--   0        0        0    10783 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_response_dto.py
--rw-r--r--   0        0        0    15234 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch_job_response_dto.py
--rw-r--r--   0        0        0    12271 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch_joined_project_response_dto.py
--rw-r--r--   0        0        0     9890 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch_response_dto.py
--rw-r--r--   0        0        0    10328 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_dataset.py
--rw-r--r--   0        0        0    10092 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_endpoint.py
--rw-r--r--   0        0        0    25050 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job.py
--rw-r--r--   0        0        0     9956 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_config.py
--rw-r--r--   0        0        0    12596 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_event.py
--rw-r--r--   0        0        0    12880 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_cohort_response_dto.py
--rw-r--r--   0        0        0    12719 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_data_query_response_dto.py
--rw-r--r--   0        0        0    21859 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_dataset_response_dto.py
--rw-r--r--   0        0        0    10146 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_feature_sub_category_response_dto.py
--rw-r--r--   0        0        0    11429 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_job_output_response_dto.py
--rw-r--r--   0        0        0    15143 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_job_status_response_dto.py
--rw-r--r--   0        0        0    13077 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py
--rw-r--r--   0        0        0    15368 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_response_dto.py
--rw-r--r--   0        0        0    25459 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py
--rw-r--r--   0        0        0    14899 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_response_dto.py
--rw-r--r--   0        0        0    11903 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_intervention_definition_response_dto.py
--rw-r--r--   0        0        0    14948 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_outcome_definition_response_dto.py
--rw-r--r--   0        0        0    28497 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_response_dto.py
--rw-r--r--   0        0        0    16370 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_response_dto.py
--rw-r--r--   0        0        0    12177 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_project_response_dto.py
--rw-r--r--   0        0        0    11585 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_output.py
--rw-r--r--   0        0        0     9880 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_output_feature.py
--rw-r--r--   0        0        0    22459 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_output_joined_dataset_response_dto.py
--rw-r--r--   0        0        0    13217 2023-06-13 18:30:19.841963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_output_joined_model_job_joined_project_response_dto.py
--rw-r--r--   0        0        0    20838 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_output_joined_model_job_response_dto.py
--rw-r--r--   0        0        0    12387 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_output_response_dto.py
--rw-r--r--   0        0        0    26342 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_response_dto.py
--rw-r--r--   0        0        0    14799 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_status.py
--rw-r--r--   0        0        0    13217 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_status_joined_model_job_joined_project_response_dto.py
--rw-r--r--   0        0        0    20838 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_status_joined_model_job_response_dto.py
--rw-r--r--   0        0        0    15027 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_status_response_dto.py
--rw-r--r--   0        0        0    20198 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_cohort_joined_model_job_response_dto.py
--rw-r--r--   0        0        0    13589 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_cohort_response_dto.py
--rw-r--r--   0        0        0    13496 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_model_job_joined_cohort_response_dto.py
--rw-r--r--   0        0        0    22959 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_model_job_joined_dataset_response_dto.py
--rw-r--r--   0        0        0    10586 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_model_job_joined_feature_sub_category_response_dto.py
--rw-r--r--   0        0        0    21985 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_model_job_response_dto.py
--rw-r--r--   0        0        0    27656 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_model_output_details_response_dto.py
--rw-r--r--   0        0        0    12021 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_project_response_dto.py
--rw-r--r--   0        0        0    10587 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_user_favorite_response_dto.py
--rw-r--r--   0        0        0    25995 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_output_details.py
--rw-r--r--   0        0        0    30089 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_population.py
--rw-r--r--   0        0        0    12461 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_joined_period_definition_response_dto.py
--rw-r--r--   0        0        0    14542 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_response_dto.py
--rw-r--r--   0        0        0    17056 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_cohort_results_response_dto.py
--rw-r--r--   0        0        0    24059 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_data_query_joined_dataset_response_dto.py
--rw-r--r--   0        0        0    14017 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_data_query_response_dto.py
--rw-r--r--   0        0        0    19133 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_feature_response_dto.py
--rw-r--r--   0        0        0    11287 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_intervention_definition_response_dto.py
--rw-r--r--   0        0        0    17798 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_model_job_joined_model_response_dto.py
--rw-r--r--   0        0        0    20883 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_model_job_response_dto.py
--rw-r--r--   0        0        0    14164 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_outcome_definition_response_dto.py
--rw-r--r--   0        0        0    30731 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_response_dto.py
--rw-r--r--   0        0        0    19577 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/model_response_dto.py
--rw-r--r--   0        0        0     2427 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/object.py
--rw-r--r--   0        0        0    23664 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/organization.py
--rw-r--r--   0        0        0    11112 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/organization_feature_category_exclusion.py
--rw-r--r--   0        0        0    11223 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/organization_feature_exclusion.py
--rw-r--r--   0        0        0     9770 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/organization_response_dto.py
--rw-r--r--   0        0        0    16743 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/organization_setting.py
--rw-r--r--   0        0        0    16743 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/organization_setting_response_dto.py
--rw-r--r--   0        0        0    14689 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/outcome_definition.py
--rw-r--r--   0        0        0     5149 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/period_definition.py
--rw-r--r--   0        0        0     2751 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/period_type.py
--rw-r--r--   0        0        0     5332 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/person_set.py
--rw-r--r--   0        0        0     3987 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/pipeline_config.py
--rw-r--r--   0        0        0    15191 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/population.py
--rw-r--r--   0        0        0    11771 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/population_store.py
--rw-r--r--   0        0        0    10755 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/population_store_response_dto.py
--rw-r--r--   0        0        0    12257 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process.py
--rw-r--r--   0        0        0    16287 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_job.py
--rw-r--r--   0        0        0     4858 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_config.py
--rw-r--r--   0        0        0    12271 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_joined_project_response_dto.py
--rw-r--r--   0        0        0    10479 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_output.py
--rw-r--r--   0        0        0    13415 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_output_joined_process_job_joined_project_response_dto.py
--rw-r--r--   0        0        0    15893 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_output_joined_process_job_response_dto.py
--rw-r--r--   0        0        0    11016 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_output_response_dto.py
--rw-r--r--   0        0        0    14331 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_response_dto.py
--rw-r--r--   0        0        0    14764 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_status.py
--rw-r--r--   0        0        0    12583 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_status_joined_project_response_dto.py
--rw-r--r--   0        0        0    14902 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_status_response_dto.py
--rw-r--r--   0        0        0    12115 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_joined_project_response_dto.py
--rw-r--r--   0        0        0    11494 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_response_dto.py
--rw-r--r--   0        0        0     2837 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/process_type.py
--rw-r--r--   0        0        0    17760 2023-06-13 18:30:19.845963 curia-4.2.0b8/src/curia/api/swagger_client/models/project.py
--rw-r--r--   0        0        0    13440 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/project_joined_model_joined_cohort_response_dto.py
--rw-r--r--   0        0        0    17121 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/project_joined_model_response_dto.py
--rw-r--r--   0        0        0    12125 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/project_joined_project_response_dto.py
--rw-r--r--   0        0        0    10675 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/project_joined_user_favorite_response_dto.py
--rw-r--r--   0        0        0    10979 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/project_member.py
--rw-r--r--   0        0        0    12437 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/project_member_joined_project_response_dto.py
--rw-r--r--   0        0        0    11641 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/project_member_response_dto.py
--rw-r--r--   0        0        0    14895 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/project_response_dto.py
--rw-r--r--   0        0        0    15487 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/scheduler.py
--rw-r--r--   0        0        0    11402 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/scheduler_joined_workflow_response_dto.py
--rw-r--r--   0        0        0    15605 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/scheduler_response_dto.py
--rw-r--r--   0        0        0     5775 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/select_expression.py
--rw-r--r--   0        0        0     2567 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/set_operator.py
--rw-r--r--   0        0        0     5737 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/state_data.py
--rw-r--r--   0        0        0    12800 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/task.py
--rw-r--r--   0        0        0    16585 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution.py
--rw-r--r--   0        0        0    13035 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_joined_task_response_dto.py
--rw-r--r--   0        0        0    14390 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_joined_workflow_execution_response_dto.py
--rw-r--r--   0        0        0    16918 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_response_dto.py
--rw-r--r--   0        0        0    11220 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_status.py
--rw-r--r--   0        0        0    15890 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py
--rw-r--r--   0        0        0    18175 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_response_dto.py
--rw-r--r--   0        0        0    11900 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_status_response_dto.py
--rw-r--r--   0        0        0     2443 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/task_inputs.py
--rw-r--r--   0        0        0     2447 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/task_outputs.py
--rw-r--r--   0        0        0    11971 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/task_response_dto.py
--rw-r--r--   0        0        0     5276 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_analysis_dto.py
--rw-r--r--   0        0        0     8382 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_analysis_job_dto.py
--rw-r--r--   0        0        0     4621 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_analysis_job_output_dto.py
--rw-r--r--   0        0        0     8830 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_analysis_job_status_dto.py
--rw-r--r--   0        0        0     6081 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_cohort_dto.py
--rw-r--r--   0        0        0     6584 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_data_query_dto.py
--rw-r--r--   0        0        0     4465 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_data_store_dto.py
--rw-r--r--   0        0        0     5925 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_data_table_dto.py
--rw-r--r--   0        0        0     5290 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_database_dto.py
--rw-r--r--   0        0        0     5156 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_dataset_column_dto.py
--rw-r--r--   0        0        0    14251 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_dataset_dto.py
--rw-r--r--   0        0        0    11532 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_feature_dto.py
--rw-r--r--   0        0        0     4513 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_feature_store_dto.py
--rw-r--r--   0        0        0     3935 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_batch_dto.py
--rw-r--r--   0        0        0     8867 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_batch_job_dto.py
--rw-r--r--   0        0        0    10055 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_dto.py
--rw-r--r--   0        0        0    12875 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_job_dto.py
--rw-r--r--   0        0        0     5272 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_job_output_dto.py
--rw-r--r--   0        0        0     8660 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_job_status_dto.py
--rw-r--r--   0        0        0    17030 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_population_dto.py
--rw-r--r--   0        0        0     4523 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_organization_dto.py
--rw-r--r--   0        0        0    10276 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_organization_setting_dto.py
--rw-r--r--   0        0        0     4561 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_population_store_dto.py
--rw-r--r--   0        0        0     5545 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_process_dto.py
--rw-r--r--   0        0        0     8239 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_process_job_dto.py
--rw-r--r--   0        0        0     4585 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_process_job_output_dto.py
--rw-r--r--   0        0        0     8770 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_process_job_status_dto.py
--rw-r--r--   0        0        0     5420 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_project_dto.py
--rw-r--r--   0        0        0     5396 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_project_member_dto.py
--rw-r--r--   0        0        0     8433 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_scheduler_dto.py
--rw-r--r--   0        0        0     5947 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_task_dto.py
--rw-r--r--   0        0        0     9730 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_task_execution_dto.py
--rw-r--r--   0        0        0     5385 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_task_execution_status_dto.py
--rw-r--r--   0        0        0     7200 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_user_audit_trail_dto.py
--rw-r--r--   0        0        0     9810 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_user_dto.py
--rw-r--r--   0        0        0     4939 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_user_favorite_dto.py
--rw-r--r--   0        0        0     4539 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_workflow_dto.py
--rw-r--r--   0        0        0     6878 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_workflow_execution_dto.py
--rw-r--r--   0        0        0     5005 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_workflow_execution_spec_dto.py
--rw-r--r--   0        0        0     5465 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_workflow_execution_status_dto.py
--rw-r--r--   0        0        0     5535 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/update_workflow_template_dto.py
--rw-r--r--   0        0        0    10477 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/user_audit_trail.py
--rw-r--r--   0        0        0    11559 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/user_audit_trail_response_dto.py
--rw-r--r--   0        0        0    10871 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/user_favorite.py
--rw-r--r--   0        0        0    12957 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/user_favorite_joined_model_joined_project_response_dto.py
--rw-r--r--   0        0        0    17499 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/user_favorite_joined_model_response_dto.py
--rw-r--r--   0        0        0    10837 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/user_favorite_response_dto.py
--rw-r--r--   0        0        0    13040 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow.py
--rw-r--r--   0        0        0    15472 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution.py
--rw-r--r--   0        0        0    13250 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_response_dto.py
--rw-r--r--   0        0        0    10872 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_spec.py
--rw-r--r--   0        0        0    14870 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_spec_joined_workflow_execution_response_dto.py
--rw-r--r--   0        0        0    11514 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_spec_response_dto.py
--rw-r--r--   0        0        0    11440 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_status.py
--rw-r--r--   0        0        0    14990 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_status_joined_workflow_execution_response_dto.py
--rw-r--r--   0        0        0    12132 2023-06-13 18:30:19.849963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_status_response_dto.py
--rw-r--r--   0        0        0    15775 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_joined_scheduler_response_dto.py
--rw-r--r--   0        0        0    14090 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_joined_workflow_execution_response_dto.py
--rw-r--r--   0        0        0    12669 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_joined_workflow_template_response_dto.py
--rw-r--r--   0        0        0    13141 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_response_dto.py
--rw-r--r--   0        0        0    12837 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_template.py
--rw-r--r--   0        0        0     5367 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_template_definition.py
--rw-r--r--   0        0        0     2507 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_template_parameters.py
--rw-r--r--   0        0        0    11941 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_template_response_dto.py
--rw-r--r--   0        0        0     5655 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/swagger_client/models/zip_data.py
--rw-r--r--   0        0        0    13208 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/swagger_client/rest.py
--rw-r--r--   0        0        0        0 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/__init__.py
--rw-r--r--   0        0        0     1091 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_aggregation_type.py
--rw-r--r--   0        0        0     1102 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_all_of_cohort_model.py
--rw-r--r--   0        0        0     1158 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_all_of_cohort_organization.py
--rw-r--r--   0        0        0     1152 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_all_of_cohort_train_cohort.py
--rw-r--r--   0        0        0     1158 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_all_of_data_table_dataset.py
--rw-r--r--   0        0        0     1110 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_all_of_model_cohorts.py
--rw-r--r--   0        0        0     1136 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_all_of_model_job_dataset.py
--rw-r--r--   0        0        0     1168 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_all_of_model_job_environment.py
--rw-r--r--   0        0        0     1120 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_all_of_model_job_model.py
--rw-r--r--   0        0        0     1136 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_all_of_model_job_project.py
--rw-r--r--   0        0        0     1128 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_all_of_model_model_jobs.py
--rw-r--r--   0        0        0     1110 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_all_of_model_project.py
--rw-r--r--   0        0        0     2252 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analyses_api.py
--rw-r--r--   0        0        0     1033 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis.py
--rw-r--r--   0        0        0     1059 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job.py
--rw-r--r--   0        0        0     1109 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job_config.py
--rw-r--r--   0        0        0     1272 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job_joined_project_response_dto.py
--rw-r--r--   0        0        0     1109 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job_output.py
--rw-r--r--   0        0        0     1464 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job_output_joined_analysis_job_joined_project_response_dto.py
--rw-r--r--   0        0        0     1356 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job_output_joined_analysis_job_response_dto.py
--rw-r--r--   0        0        0     1214 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job_output_response_dto.py
--rw-r--r--   0        0        0     2675 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job_outputs_api.py
--rw-r--r--   0        0        0     1164 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job_response_dto.py
--rw-r--r--   0        0        0     1109 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job_status.py
--rw-r--r--   0        0        0     1322 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job_status_joined_project_response_dto.py
--rw-r--r--   0        0        0     1214 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job_status_response_dto.py
--rw-r--r--   0        0        0     2680 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job_statuses_api.py
--rw-r--r--   0        0        0     1093 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_job_type.py
--rw-r--r--   0        0        0     2749 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_jobs_api.py
--rw-r--r--   0        0        0     1246 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_joined_project_response_dto.py
--rw-r--r--   0        0        0     1138 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_response_dto.py
--rw-r--r--   0        0        0     1067 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_analysis_type.py
--rw-r--r--   0        0        0     1217 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_any_of_arithmetic_expression_value.py
--rw-r--r--   0        0        0     1193 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_any_of_boolean_expression_value.py
--rw-r--r--   0        0        0     1367 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_any_of_cohort_definition_patient_metadata_filters_items.py
--rw-r--r--   0        0        0     1127 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_any_of_condition_value.py
--rw-r--r--   0        0        0     1131 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_arithmetic_expression.py
--rw-r--r--   0        0        0     1115 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_arithmetic_operator.py
--rw-r--r--   0        0        0     1000 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_body.py
--rw-r--r--   0        0        0     1009 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_body1.py
--rw-r--r--   0        0        0     1008 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_body2.py
--rw-r--r--   0        0        0     1008 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_body3.py
--rw-r--r--   0        0        0      978 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_body4.py
--rw-r--r--   0        0        0      978 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_body5.py
--rw-r--r--   0        0        0     1107 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_boolean_expression.py
--rw-r--r--   0        0        0     1000 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_code.py
--rw-r--r--   0        0        0     1016 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_cohort.py
--rw-r--r--   0        0        0     1099 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_cohort_definition.py
--rw-r--r--   0        0        0     1066 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_cohort_filter.py
--rw-r--r--   0        0        0     1140 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_cohort_filter_condition.py
--rw-r--r--   0        0        0     1222 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_cohort_joined_cohort_response_dto.py
--rw-r--r--   0        0        0     1240 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_cohort_joined_model_job_response_dto.py
--rw-r--r--   0        0        0     1122 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_cohort_response_dto.py
--rw-r--r--   0        0        0     1075 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_cohort_results.py
--rw-r--r--   0        0        0     1043 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_cohort_set.py
--rw-r--r--   0        0        0     1066 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_cohort_window.py
--rw-r--r--   0        0        0     2511 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_cohorts_api.py
--rw-r--r--   0        0        0     1041 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_condition.py
--rw-r--r--   0        0        0     1107 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_condition_operator.py
--rw-r--r--   0        0        0     1090 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_container_config.py
--rw-r--r--   0        0        0     1122 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_analysis_dto.py
--rw-r--r--   0        0        0     1148 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_analysis_job_dto.py
--rw-r--r--   0        0        0     1198 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_analysis_job_output_dto.py
--rw-r--r--   0        0        0     1198 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_analysis_job_status_dto.py
--rw-r--r--   0        0        0     1106 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_cohort_dto.py
--rw-r--r--   0        0        0     1132 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_data_query_dto.py
--rw-r--r--   0        0        0     1118 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_data_store_dto.py
--rw-r--r--   0        0        0     1132 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_data_table_dto.py
--rw-r--r--   0        0        0     1122 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_database_dto.py
--rw-r--r--   0        0        0     1164 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_dataset_column_dto.py
--rw-r--r--   0        0        0     1114 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_dataset_dto.py
--rw-r--r--   0        0        0     1114 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_feature_dto.py
--rw-r--r--   0        0        0     1142 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_feature_store_dto.py
--rw-r--r--   0        0        0     1143 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_analysis_dto.py
--rw-r--r--   0        0        0     1169 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_analysis_job_dto.py
--rw-r--r--   0        0        0     1219 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_analysis_job_output_dto.py
--rw-r--r--   0        0        0     1219 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_analysis_job_status_dto.py
--rw-r--r--   0        0        0     1110 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_code_dto.py
--rw-r--r--   0        0        0     1126 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_cohort_dto.py
--rw-r--r--   0        0        0     1153 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_data_query_dto.py
--rw-r--r--   0        0        0     1152 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_data_store_dto.py
--rw-r--r--   0        0        0     1184 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_dataset_column_dto.py
--rw-r--r--   0        0        0     1134 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_dataset_dto.py
--rw-r--r--   0        0        0     1160 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_dataset_job_dto.py
--rw-r--r--   0        0        0     1166 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_environment_dto.py
--rw-r--r--   0        0        0     1200 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_feature_category_dto.py
--rw-r--r--   0        0        0     1134 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_feature_dto.py
--rw-r--r--   0        0        0     1176 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_feature_store_dto.py
--rw-r--r--   0        0        0     1226 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_feature_sub_category_dto.py
--rw-r--r--   0        0        0     1161 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_model_batch_dto.py
--rw-r--r--   0        0        0     1187 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_model_batch_job_dto.py
--rw-r--r--   0        0        0     1176 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_model_dataset_dto.py
--rw-r--r--   0        0        0     1118 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_model_dto.py
--rw-r--r--   0        0        0     1184 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_model_endpoint_dto.py
--rw-r--r--   0        0        0     1144 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_model_job_dto.py
--rw-r--r--   0        0        0     1194 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_model_job_output_dto.py
--rw-r--r--   0        0        0     1253 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_model_job_output_feature_dto.py
--rw-r--r--   0        0        0     1201 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_model_population_dto.py
--rw-r--r--   0        0        0     1174 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_organization_dto.py
--rw-r--r--   0        0        0     1306 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_organization_feature_exclusion_dto.py
--rw-r--r--   0        0        0     1232 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_organization_setting_dto.py
--rw-r--r--   0        0        0     1200 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_population_store_dto.py
--rw-r--r--   0        0        0     1135 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_process_dto.py
--rw-r--r--   0        0        0     1161 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_process_job_dto.py
--rw-r--r--   0        0        0     1211 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_process_job_output_dto.py
--rw-r--r--   0        0        0     1211 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_process_job_status_dto.py
--rw-r--r--   0        0        0     1134 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_project_dto.py
--rw-r--r--   0        0        0     1184 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_project_member_dto.py
--rw-r--r--   0        0        0     1161 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_scheduler_dto.py
--rw-r--r--   0        0        0     1121 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_task_dto.py
--rw-r--r--   0        0        0     1195 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_task_execution_dto.py
--rw-r--r--   0        0        0     1245 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_task_execution_status_dto.py
--rw-r--r--   0        0        0     1176 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_user_favorite_dto.py
--rw-r--r--   0        0        0     1153 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_workflow_dto.py
--rw-r--r--   0        0        0     1227 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_workflow_execution_dto.py
--rw-r--r--   0        0        0     1250 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_workflow_execution_spec_dto.py
--rw-r--r--   0        0        0     1219 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_many_workflow_template_dto.py
--rw-r--r--   0        0        0     1140 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_model_batch_dto.py
--rw-r--r--   0        0        0     1166 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_model_batch_job_dto.py
--rw-r--r--   0        0        0     1098 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_model_dto.py
--rw-r--r--   0        0        0     1124 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_model_job_dto.py
--rw-r--r--   0        0        0     1174 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_model_job_output_dto.py
--rw-r--r--   0        0        0     1174 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_model_job_status_dto.py
--rw-r--r--   0        0        0     1180 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_model_population_dto.py
--rw-r--r--   0        0        0     1154 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_organization_dto.py
--rw-r--r--   0        0        0     1212 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_organization_setting_dto.py
--rw-r--r--   0        0        0     1166 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_population_store_dto.py
--rw-r--r--   0        0        0     1114 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_process_dto.py
--rw-r--r--   0        0        0     1140 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_process_job_dto.py
--rw-r--r--   0        0        0     1190 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_process_job_output_dto.py
--rw-r--r--   0        0        0     1190 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_process_job_status_dto.py
--rw-r--r--   0        0        0     1114 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_project_dto.py
--rw-r--r--   0        0        0     1164 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_project_member_dto.py
--rw-r--r--   0        0        0     1130 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_scheduler_dto.py
--rw-r--r--   0        0        0     1090 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_task_dto.py
--rw-r--r--   0        0        0     1164 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_task_execution_dto.py
--rw-r--r--   0        0        0     1214 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_task_execution_status_dto.py
--rw-r--r--   0        0        0     1174 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_user_audit_trail_dto.py
--rw-r--r--   0        0        0     1156 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_user_favorite_dto.py
--rw-r--r--   0        0        0     1122 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_workflow_dto.py
--rw-r--r--   0        0        0     1196 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_workflow_execution_dto.py
--rw-r--r--   0        0        0     1216 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_workflow_execution_spec_dto.py
--rw-r--r--   0        0        0     1246 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test/test_create_workflow_execution_status_dto.py
--rw-r--r--   0        0        0     1188 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_create_workflow_template_dto.py
--rw-r--r--   0        0        0     2504 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_data_queries_api.py
--rw-r--r--   0        0        0     1043 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_data_query.py
--rw-r--r--   0        0        0     1256 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_data_query_joined_dataset_response_dto.py
--rw-r--r--   0        0        0     1148 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_data_query_response_dto.py
--rw-r--r--   0        0        0     1042 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_data_store.py
--rw-r--r--   0        0        0     1134 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_data_store_response_dto.py
--rw-r--r--   0        0        0     2360 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_data_stores_api.py
--rw-r--r--   0        0        0     1043 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_data_table.py
--rw-r--r--   0        0        0     1264 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_data_table_joined_database_response_dto.py
--rw-r--r--   0        0        0     1256 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_data_table_joined_dataset_response_dto.py
--rw-r--r--   0        0        0     1148 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_data_table_response_dto.py
--rw-r--r--   0        0        0     1255 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_data_tables_api.py
--rw-r--r--   0        0        0     1033 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_database.py
--rw-r--r--   0        0        0     1264 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_database_joined_data_table_response_dto.py
--rw-r--r--   0        0        0     1138 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_database_response_dto.py
--rw-r--r--   0        0        0     1588 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_databases_api.py
--rw-r--r--   0        0        0     1024 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_dataset.py
--rw-r--r--   0        0        0     1074 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_dataset_column.py
--rw-r--r--   0        0        0     1288 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_dataset_column_joined_dataset_response_dto.py
--rw-r--r--   0        0        0     1180 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_dataset_column_response_dto.py
--rw-r--r--   0        0        0     2486 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_dataset_columns_api.py
--rw-r--r--   0        0        0     1050 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_dataset_job.py
--rw-r--r--   0        0        0     1100 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_dataset_job_status.py
--rw-r--r--   0        0        0     1256 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_dataset_joined_data_query_response_dto.py
--rw-r--r--   0        0        0     1288 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_dataset_joined_dataset_column_response_dto.py
--rw-r--r--   0        0        0     1130 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_dataset_response_dto.py
--rw-r--r--   0        0        0     3799 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_datasets_api.py
--rw-r--r--   0        0        0     1226 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_datasetsuploadlargecomplete_parts.py
--rw-r--r--   0        0        0     1056 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_environment.py
--rw-r--r--   0        0        0     1122 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_environment_activity.py
--rw-r--r--   0        0        0     1024 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_feature.py
--rw-r--r--   0        0        0     1090 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_feature_category.py
--rw-r--r--   0        0        0     1504 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_feature_joined_feature_sub_category_joined_feature_category_response_dto.py
--rw-r--r--   0        0        0     1330 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_feature_joined_feature_sub_category_response_dto.py
--rw-r--r--   0        0        0     1304 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_feature_joined_model_population_response_dto.py
--rw-r--r--   0        0        0     1410 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_feature_joined_organization_feature_exclusion_response_dto.py
--rw-r--r--   0        0        0     1130 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_feature_response_dto.py
--rw-r--r--   0        0        0     1066 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_feature_store.py
--rw-r--r--   0        0        0     1158 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_feature_store_response_dto.py
--rw-r--r--   0        0        0     2480 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_feature_stores_api.py
--rw-r--r--   0        0        0     1116 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_feature_sub_category.py
--rw-r--r--   0        0        0     1066 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_feature_table.py
--rw-r--r--   0        0        0     2217 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_features_api.py
--rw-r--r--   0        0        0     1098 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_geographic_counts.py
--rw-r--r--   0        0        0     1106 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_geographic_queries.py
--rw-r--r--   0        0        0     1261 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_analysis_job_output_response_dto.py
--rw-r--r--   0        0        0     1211 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_analysis_job_response_dto.py
--rw-r--r--   0        0        0     1261 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_analysis_job_status_response_dto.py
--rw-r--r--   0        0        0     1185 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_analysis_response_dto.py
--rw-r--r--   0        0        0     1152 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_code_response_dto.py
--rw-r--r--   0        0        0     1168 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_cohort_response_dto.py
--rw-r--r--   0        0        0     1195 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_data_query_response_dto.py
--rw-r--r--   0        0        0     1194 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_data_store_response_dto.py
--rw-r--r--   0        0        0     1195 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_data_table_response_dto.py
--rw-r--r--   0        0        0     1185 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_database_response_dto.py
--rw-r--r--   0        0        0     1226 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_dataset_column_response_dto.py
--rw-r--r--   0        0        0     1202 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_dataset_job_response_dto.py
--rw-r--r--   0        0        0     1252 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_dataset_job_status_response_dto.py
--rw-r--r--   0        0        0     1176 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_dataset_response_dto.py
--rw-r--r--   0        0        0     1208 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_environment_response_dto.py
--rw-r--r--   0        0        0     1242 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_feature_category_response_dto.py
--rw-r--r--   0        0        0     1176 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_feature_response_dto.py
--rw-r--r--   0        0        0     1218 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_feature_store_response_dto.py
--rw-r--r--   0        0        0     1268 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_feature_sub_category_response_dto.py
--rw-r--r--   0        0        0     1229 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_model_batch_job_response_dto.py
--rw-r--r--   0        0        0     1203 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_model_batch_response_dto.py
--rw-r--r--   0        0        0     1218 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_model_dataset_response_dto.py
--rw-r--r--   0        0        0     1226 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_model_endpoint_response_dto.py
--rw-r--r--   0        0        0     1228 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_model_job_event_response_dto.py
--rw-r--r--   0        0        0     1295 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_model_job_output_feature_response_dto.py
--rw-r--r--   0        0        0     1236 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_model_job_output_response_dto.py
--rw-r--r--   0        0        0     1186 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_model_job_response_dto.py
--rw-r--r--   0        0        0     1236 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_model_job_status_response_dto.py
--rw-r--r--   0        0        0     1243 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_model_population_response_dto.py
--rw-r--r--   0        0        0     1160 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_model_response_dto.py
--rw-r--r--   0        0        0     1348 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_organization_feature_exclusion_response_dto.py
--rw-r--r--   0        0        0     1216 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_organization_response_dto.py
--rw-r--r--   0        0        0     1274 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_organization_setting_response_dto.py
--rw-r--r--   0        0        0     1242 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_population_store_response_dto.py
--rw-r--r--   0        0        0     1253 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_process_job_output_response_dto.py
--rw-r--r--   0        0        0     1203 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_process_job_response_dto.py
--rw-r--r--   0        0        0     1253 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_process_job_status_response_dto.py
--rw-r--r--   0        0        0     1177 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_process_response_dto.py
--rw-r--r--   0        0        0     1226 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_project_member_response_dto.py
--rw-r--r--   0        0        0     1176 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_project_response_dto.py
--rw-r--r--   0        0        0     1203 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_scheduler_response_dto.py
--rw-r--r--   0        0        0     1237 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_task_execution_response_dto.py
--rw-r--r--   0        0        0     1287 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_task_execution_status_response_dto.py
--rw-r--r--   0        0        0     1163 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_task_response_dto.py
--rw-r--r--   0        0        0     1237 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_user_audit_trail_response_dto.py
--rw-r--r--   0        0        0     1218 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_user_favorite_response_dto.py
--rw-r--r--   0        0        0     1269 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_workflow_execution_response_dto.py
--rw-r--r--   0        0        0     1292 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_workflow_execution_spec_response_dto.py
--rw-r--r--   0        0        0     1319 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_workflow_execution_status_response_dto.py
--rw-r--r--   0        0        0     1195 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_workflow_response_dto.py
--rw-r--r--   0        0        0     1261 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_get_many_workflow_template_response_dto.py
--rw-r--r--   0        0        0     1107 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_inline_response200.py
--rw-r--r--   0        0        0     1141 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_inline_response200_info.py
--rw-r--r--   0        0        0     1107 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_inline_response503.py
--rw-r--r--   0        0        0     7598 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_internal_api.py
--rw-r--r--   0        0        0     1147 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_intervention_definition.py
--rw-r--r--   0        0        0     1001 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_json.py
--rw-r--r--   0        0        0     1091 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_logical_operator.py
--rw-r--r--   0        0        0     1008 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model.py
--rw-r--r--   0        0        0     1051 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_batch.py
--rw-r--r--   0        0        0     1077 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_batch_job.py
--rw-r--r--   0        0        0     1424 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_batch_job_joined_model_batch_joined_project_response_dto.py
--rw-r--r--   0        0        0     1316 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_batch_job_joined_model_batch_response_dto.py
--rw-r--r--   0        0        0     1182 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_batch_job_response_dto.py
--rw-r--r--   0        0        0     3070 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_batch_jobs_api.py
--rw-r--r--   0        0        0     1264 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_batch_joined_project_response_dto.py
--rw-r--r--   0        0        0     1156 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_batch_response_dto.py
--rw-r--r--   0        0        0     2371 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_batches_api.py
--rw-r--r--   0        0        0     1066 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_dataset.py
--rw-r--r--   0        0        0     1074 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_endpoint.py
--rw-r--r--   0        0        0     1034 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job.py
--rw-r--r--   0        0        0     1084 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_config.py
--rw-r--r--   0        0        0     1076 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_event.py
--rw-r--r--   0        0        0     1240 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_cohort_response_dto.py
--rw-r--r--   0        0        0     1252 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_data_query_response_dto.py
--rw-r--r--   0        0        0     1248 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_dataset_response_dto.py
--rw-r--r--   0        0        0     1340 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_feature_sub_category_response_dto.py
--rw-r--r--   0        0        0     1308 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_job_output_response_dto.py
--rw-r--r--   0        0        0     1308 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_job_status_response_dto.py
--rw-r--r--   0        0        0     1678 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py
--rw-r--r--   0        0        0     1496 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_response_dto.py
--rw-r--r--   0        0        0     1548 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py
--rw-r--r--   0        0        0     1440 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_response_dto.py
--rw-r--r--   0        0        0     1544 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_joined_intervention_definition_response_dto.py
--rw-r--r--   0        0        0     1504 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_joined_outcome_definition_response_dto.py
--rw-r--r--   0        0        0     1314 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_response_dto.py
--rw-r--r--   0        0        0     1232 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_response_dto.py
--rw-r--r--   0        0        0     1248 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_joined_project_response_dto.py
--rw-r--r--   0        0        0     1084 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_output.py
--rw-r--r--   0        0        0     1142 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_output_feature.py
--rw-r--r--   0        0        0     1298 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_output_joined_dataset_response_dto.py
--rw-r--r--   0        0        0     1416 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_output_joined_model_job_joined_project_response_dto.py
--rw-r--r--   0        0        0     1308 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_output_joined_model_job_response_dto.py
--rw-r--r--   0        0        0     1190 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_output_response_dto.py
--rw-r--r--   0        0        0     2555 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_outputs_api.py
--rw-r--r--   0        0        0     1140 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_response_dto.py
--rw-r--r--   0        0        0     1084 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_status.py
--rw-r--r--   0        0        0     1416 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_status_joined_model_job_joined_project_response_dto.py
--rw-r--r--   0        0        0     1308 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_status_joined_model_job_response_dto.py
--rw-r--r--   0        0        0     1190 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_status_response_dto.py
--rw-r--r--   0        0        0     1586 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_job_statuses_api.py
--rw-r--r--   0        0        0     2820 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_jobs_api.py
--rw-r--r--   0        0        0     1332 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_joined_cohort_joined_model_job_response_dto.py
--rw-r--r--   0        0        0     1214 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_joined_cohort_response_dto.py
--rw-r--r--   0        0        0     1332 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_joined_model_job_joined_cohort_response_dto.py
--rw-r--r--   0        0        0     1340 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_joined_model_job_joined_dataset_response_dto.py
--rw-r--r--   0        0        0     1432 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_joined_model_job_joined_feature_sub_category_response_dto.py
--rw-r--r--   0        0        0     1232 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_joined_model_job_response_dto.py
--rw-r--r--   0        0        0     1300 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_joined_model_output_details_response_dto.py
--rw-r--r--   0        0        0     1222 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_joined_project_response_dto.py
--rw-r--r--   0        0        0     1264 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_joined_user_favorite_response_dto.py
--rw-r--r--   0        0        0     1116 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_output_details.py
--rw-r--r--   0        0        0     1091 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_population.py
--rw-r--r--   0        0        0     1560 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_population_joined_cohort_definition_joined_period_definition_response_dto.py
--rw-r--r--   0        0        0     1378 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_population_joined_cohort_definition_response_dto.py
--rw-r--r--   0        0        0     1354 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_population_joined_cohort_results_response_dto.py
--rw-r--r--   0        0        0     1430 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_population_joined_data_query_joined_dataset_response_dto.py
--rw-r--r--   0        0        0     1322 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_population_joined_data_query_response_dto.py
--rw-r--r--   0        0        0     1304 2023-06-13 18:30:19.857963 curia-4.2.0b8/src/curia/api/test/test_model_population_joined_feature_response_dto.py
--rw-r--r--   0        0        0     1426 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_model_population_joined_intervention_definition_response_dto.py
--rw-r--r--   0        0        0     1406 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_model_population_joined_model_job_joined_model_response_dto.py
--rw-r--r--   0        0        0     1314 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_model_population_joined_model_job_response_dto.py
--rw-r--r--   0        0        0     1386 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_model_population_joined_outcome_definition_response_dto.py
--rw-r--r--   0        0        0     1196 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_model_population_response_dto.py
--rw-r--r--   0        0        0     2769 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_model_populations_api.py
--rw-r--r--   0        0        0     1114 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_model_response_dto.py
--rw-r--r--   0        0        0     2895 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_models_api.py
--rw-r--r--   0        0        0     1016 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_object.py
--rw-r--r--   0        0        0     1064 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_organization.py
--rw-r--r--   0        0        0     1276 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_organization_feature_category_exclusion.py
--rw-r--r--   0        0        0     1196 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_organization_feature_exclusion.py
--rw-r--r--   0        0        0     1170 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_organization_response_dto.py
--rw-r--r--   0        0        0     1122 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_organization_setting.py
--rw-r--r--   0        0        0     1228 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_organization_setting_response_dto.py
--rw-r--r--   0        0        0     3201 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_organization_settings_api.py
--rw-r--r--   0        0        0     2431 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_organizations_api.py
--rw-r--r--   0        0        0     1107 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_outcome_definition.py
--rw-r--r--   0        0        0     1098 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_period_definition.py
--rw-r--r--   0        0        0     1051 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_period_type.py
--rw-r--r--   0        0        0     1043 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_person_set.py
--rw-r--r--   0        0        0     1082 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_pipeline_config.py
--rw-r--r--   0        0        0    26607 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_platform_api.py
--rw-r--r--   0        0        0     1048 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_population.py
--rw-r--r--   0        0        0     1090 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_population_store.py
--rw-r--r--   0        0        0     1182 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_population_store_response_dto.py
--rw-r--r--   0        0        0     2600 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_population_stores_api.py
--rw-r--r--   0        0        0     1025 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process.py
--rw-r--r--   0        0        0     1051 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_job.py
--rw-r--r--   0        0        0     1114 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_job_config.py
--rw-r--r--   0        0        0     1264 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_job_joined_project_response_dto.py
--rw-r--r--   0        0        0     1101 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_job_output.py
--rw-r--r--   0        0        0     1448 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_job_output_joined_process_job_joined_project_response_dto.py
--rw-r--r--   0        0        0     1340 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_job_output_joined_process_job_response_dto.py
--rw-r--r--   0        0        0     1206 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_job_output_response_dto.py
--rw-r--r--   0        0        0     2635 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_job_outputs_api.py
--rw-r--r--   0        0        0     1156 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_job_response_dto.py
--rw-r--r--   0        0        0     1101 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_job_status.py
--rw-r--r--   0        0        0     1314 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_job_status_joined_project_response_dto.py
--rw-r--r--   0        0        0     1206 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_job_status_response_dto.py
--rw-r--r--   0        0        0     2640 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_job_statuses_api.py
--rw-r--r--   0        0        0     2703 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_jobs_api.py
--rw-r--r--   0        0        0     1238 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_joined_project_response_dto.py
--rw-r--r--   0        0        0     1130 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_response_dto.py
--rw-r--r--   0        0        0     1059 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_process_type.py
--rw-r--r--   0        0        0     2222 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_processes_api.py
--rw-r--r--   0        0        0     1024 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_project.py
--rw-r--r--   0        0        0     1322 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_project_joined_model_joined_cohort_response_dto.py
--rw-r--r--   0        0        0     1222 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_project_joined_model_response_dto.py
--rw-r--r--   0        0        0     1238 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_project_joined_project_response_dto.py
--rw-r--r--   0        0        0     1280 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_project_joined_user_favorite_response_dto.py
--rw-r--r--   0        0        0     1074 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_project_member.py
--rw-r--r--   0        0        0     1288 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_project_member_joined_project_response_dto.py
--rw-r--r--   0        0        0     1180 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_project_member_response_dto.py
--rw-r--r--   0        0        0     2486 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_project_members_api.py
--rw-r--r--   0        0        0     1130 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_project_response_dto.py
--rw-r--r--   0        0        0     2858 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_projects_api.py
--rw-r--r--   0        0        0     1051 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_scheduler.py
--rw-r--r--   0        0        0     2340 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_scheduler_api.py
--rw-r--r--   0        0        0     1248 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_scheduler_joined_workflow_response_dto.py
--rw-r--r--   0        0        0     1146 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_scheduler_response_dto.py
--rw-r--r--   0        0        0     1099 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_select_expression.py
--rw-r--r--   0        0        0     1059 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_set_operator.py
--rw-r--r--   0        0        0     1056 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_state_data.py
--rw-r--r--   0        0        0     1011 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_task.py
--rw-r--r--   0        0        0     1085 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_task_execution.py
--rw-r--r--   0        0        0     1250 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_task_execution_joined_task_response_dto.py
--rw-r--r--   0        0        0     1356 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_task_execution_joined_workflow_execution_response_dto.py
--rw-r--r--   0        0        0     1180 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_task_execution_response_dto.py
--rw-r--r--   0        0        0     1135 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_task_execution_status.py
--rw-r--r--   0        0        0     1564 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py
--rw-r--r--   0        0        0     1374 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_task_execution_status_joined_task_execution_response_dto.py
--rw-r--r--   0        0        0     1230 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_task_execution_status_response_dto.py
--rw-r--r--   0        0        0     1061 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_task_inputs.py
--rw-r--r--   0        0        0     1069 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_task_outputs.py
--rw-r--r--   0        0        0     1106 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_task_response_dto.py
--rw-r--r--   0        0        0     2687 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_tasks_api.py
--rw-r--r--   0        0        0     1122 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_analysis_dto.py
--rw-r--r--   0        0        0     1148 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_analysis_job_dto.py
--rw-r--r--   0        0        0     1198 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_analysis_job_output_dto.py
--rw-r--r--   0        0        0     1198 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_analysis_job_status_dto.py
--rw-r--r--   0        0        0     1106 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_cohort_dto.py
--rw-r--r--   0        0        0     1132 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_data_query_dto.py
--rw-r--r--   0        0        0     1118 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_data_store_dto.py
--rw-r--r--   0        0        0     1132 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_data_table_dto.py
--rw-r--r--   0        0        0     1122 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_database_dto.py
--rw-r--r--   0        0        0     1164 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_dataset_column_dto.py
--rw-r--r--   0        0        0     1114 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_dataset_dto.py
--rw-r--r--   0        0        0     1114 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_feature_dto.py
--rw-r--r--   0        0        0     1142 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_feature_store_dto.py
--rw-r--r--   0        0        0     1140 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_model_batch_dto.py
--rw-r--r--   0        0        0     1166 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_model_batch_job_dto.py
--rw-r--r--   0        0        0     1098 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_model_dto.py
--rw-r--r--   0        0        0     1124 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_model_job_dto.py
--rw-r--r--   0        0        0     1174 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_model_job_output_dto.py
--rw-r--r--   0        0        0     1174 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_model_job_status_dto.py
--rw-r--r--   0        0        0     1180 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_model_population_dto.py
--rw-r--r--   0        0        0     1154 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_organization_dto.py
--rw-r--r--   0        0        0     1212 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_organization_setting_dto.py
--rw-r--r--   0        0        0     1166 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_population_store_dto.py
--rw-r--r--   0        0        0     1114 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_process_dto.py
--rw-r--r--   0        0        0     1140 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_process_job_dto.py
--rw-r--r--   0        0        0     1190 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_process_job_output_dto.py
--rw-r--r--   0        0        0     1190 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_process_job_status_dto.py
--rw-r--r--   0        0        0     1114 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_project_dto.py
--rw-r--r--   0        0        0     1164 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_project_member_dto.py
--rw-r--r--   0        0        0     1130 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_scheduler_dto.py
--rw-r--r--   0        0        0     1090 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_task_dto.py
--rw-r--r--   0        0        0     1164 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_task_execution_dto.py
--rw-r--r--   0        0        0     1214 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_task_execution_status_dto.py
--rw-r--r--   0        0        0     1174 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_user_audit_trail_dto.py
--rw-r--r--   0        0        0     1076 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_user_dto.py
--rw-r--r--   0        0        0     1156 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_user_favorite_dto.py
--rw-r--r--   0        0        0     1122 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_workflow_dto.py
--rw-r--r--   0        0        0     1196 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_workflow_execution_dto.py
--rw-r--r--   0        0        0     1216 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_workflow_execution_spec_dto.py
--rw-r--r--   0        0        0     1246 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_workflow_execution_status_dto.py
--rw-r--r--   0        0        0     1188 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_update_workflow_template_dto.py
--rw-r--r--   0        0        0     1085 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_user_audit_trail.py
--rw-r--r--   0        0        0     1334 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_user_audit_trail_api.py
--rw-r--r--   0        0        0     1190 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_user_audit_trail_response_dto.py
--rw-r--r--   0        0        0     1066 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_user_favorite.py
--rw-r--r--   0        0        0     1372 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_user_favorite_joined_model_joined_project_response_dto.py
--rw-r--r--   0        0        0     1264 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_user_favorite_joined_model_response_dto.py
--rw-r--r--   0        0        0     1172 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_user_favorite_response_dto.py
--rw-r--r--   0        0        0     2446 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_user_favorites_api.py
--rw-r--r--   0        0        0     4472 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_user_management_api.py
--rw-r--r--   0        0        0     1043 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow.py
--rw-r--r--   0        0        0     1117 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_execution.py
--rw-r--r--   0        0        0     1212 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_execution_response_dto.py
--rw-r--r--   0        0        0     1140 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_execution_spec.py
--rw-r--r--   0        0        0     1422 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_execution_spec_joined_workflow_execution_response_dto.py
--rw-r--r--   0        0        0     1232 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_execution_spec_response_dto.py
--rw-r--r--   0        0        0     1167 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_execution_status.py
--rw-r--r--   0        0        0     1438 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_execution_status_joined_workflow_execution_response_dto.py
--rw-r--r--   0        0        0     1262 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_execution_status_response_dto.py
--rw-r--r--   0        0        0     1262 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_joined_scheduler_response_dto.py
--rw-r--r--   0        0        0     1328 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_joined_workflow_execution_response_dto.py
--rw-r--r--   0        0        0     1320 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_joined_workflow_template_response_dto.py
--rw-r--r--   0        0        0     1138 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_response_dto.py
--rw-r--r--   0        0        0     1109 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_template.py
--rw-r--r--   0        0        0     1191 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_template_definition.py
--rw-r--r--   0        0        0     1180 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_template_parameters.py
--rw-r--r--   0        0        0     1204 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflow_template_response_dto.py
--rw-r--r--   0        0        0     2575 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_workflows_api.py
--rw-r--r--   0        0        0     1040 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/test/test_zip_data.py
--rw-r--r--   0        0        0       69 2023-06-13 18:30:19.853963 curia-4.2.0b8/src/curia/api/test-requirements.txt
--rw-r--r--   0        0        0      143 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/api/tox.ini
--rw-r--r--   0        0        0        0 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/mock/__init__.py
--rw-r--r--   0        0        0    22897 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/mock/api.py
--rw-r--r--   0        0        0    17122 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/mock/api_server.py
--rw-r--r--   0        0        0     4287 2023-06-13 18:30:19.861963 curia-4.2.0b8/src/curia/mock/moto.py
--rw-r--r--   0        0        0     1565 2023-06-13 18:30:19.865963 curia-4.2.0b8/src/curia/mock/s3.py
--rw-r--r--   0        0        0    14281 2023-06-13 18:30:19.865963 curia-4.2.0b8/src/curia/mock/server.py
--rw-r--r--   0        0        0      284 2023-06-13 18:30:19.865963 curia-4.2.0b8/src/curia/mock/session.py
--rw-r--r--   0        0        0      992 2023-06-13 18:30:19.865963 curia-4.2.0b8/src/curia/session.py
--rw-r--r--   0        0        0        0 2023-06-13 18:30:19.865963 curia-4.2.0b8/src/curia/utils/__init__.py
--rw-r--r--   0        0        0     1276 2023-06-13 18:30:19.865963 curia-4.2.0b8/src/curia/utils/dataset.py
--rw-r--r--   0        0        0     3727 2023-06-13 18:30:19.865963 curia-4.2.0b8/src/curia/utils/job.py
--rw-r--r--   0        0        0     1125 2023-06-13 18:30:19.865963 curia-4.2.0b8/src/curia/utils/python.py
--rw-r--r--   0        0        0     7824 2023-06-13 18:30:19.865963 curia-4.2.0b8/src/curia/utils/s3.py
--rw-r--r--   0        0        0     1165 2023-06-13 18:30:19.865963 curia-4.2.0b8/src/curia/utils/string.py
--rw-r--r--   0        0        0     7531 1970-01-01 00:00:00.000000 curia-4.2.0b8/PKG-INFO
+-rw-r--r--   0        0        0     6541 2023-06-14 19:39:44.860363 curia-4.2.0b9/README.md
+-rw-r--r--   0        0        0     3986 2023-06-14 19:41:00.464019 curia-4.2.0b9/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-06-14 19:41:00.428019 curia-4.2.0b9/src/curia/__init__.py
+-rw-r--r--   0        0        0      786 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/.gitignore
+-rw-r--r--   0        0        0        6 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0     1030 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/.swagger-codegen-ignore
+-rw-r--r--   0        0        0      349 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/.travis.yml
+-rw-r--r--   0        0        0   124667 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/__init__.py
+-rw-r--r--   0        0        0      292 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AggregationType.md
+-rw-r--r--   0        0        0      293 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AllOfCohortModel.md
+-rw-r--r--   0        0        0      300 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AllOfCohortOrganization.md
+-rw-r--r--   0        0        0      299 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AllOfCohortTrainCohort.md
+-rw-r--r--   0        0        0      298 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AllOfDataTableDataset.md
+-rw-r--r--   0        0        0      294 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AllOfModelCohorts.md
+-rw-r--r--   0        0        0      297 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AllOfModelJobDataset.md
+-rw-r--r--   0        0        0      301 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AllOfModelJobEnvironment.md
+-rw-r--r--   0        0        0      295 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AllOfModelJobModel.md
+-rw-r--r--   0        0        0      297 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AllOfModelJobProject.md
+-rw-r--r--   0        0        0      296 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AllOfModelModelJobs.md
+-rw-r--r--   0        0        0      294 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AllOfModelProject.md
+-rw-r--r--   0        0        0    18774 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysesApi.md
+-rw-r--r--   0        0        0     1042 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/Analysis.md
+-rw-r--r--   0        0        0     1452 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJob.md
+-rw-r--r--   0        0        0      417 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobConfig.md
+-rw-r--r--   0        0        0      818 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0      682 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobOutput.md
+-rw-r--r--   0        0        0      841 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobOutputJoinedAnalysisJobJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0     1114 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobOutputJoinedAnalysisJobResponseDto.md
+-rw-r--r--   0        0        0      772 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobOutputResponseDto.md
+-rw-r--r--   0        0        0    20503 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobOutputsApi.md
+-rw-r--r--   0        0        0     1045 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobResponseDto.md
+-rw-r--r--   0        0        0     1034 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobStatus.md
+-rw-r--r--   0        0        0      824 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobStatusJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0     1043 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobStatusResponseDto.md
+-rw-r--r--   0        0        0    20538 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobStatusesApi.md
+-rw-r--r--   0        0        0      292 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobType.md
+-rw-r--r--   0        0        0    22862 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJobsApi.md
+-rw-r--r--   0        0        0      815 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0      828 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisResponseDto.md
+-rw-r--r--   0        0        0      289 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnalysisType.md
+-rw-r--r--   0        0        0      307 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnyOfArithmeticExpressionValue.md
+-rw-r--r--   0        0        0      304 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnyOfBooleanExpressionValue.md
+-rw-r--r--   0        0        0      325 2023-06-14 19:39:44.860363 curia-4.2.0b9/src/curia/api/docs/AnyOfCohortDefinitionPatientMetadataFiltersItems.md
+-rw-r--r--   0        0        0      296 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/AnyOfConditionValue.md
+-rw-r--r--   0        0        0      473 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/ArithmeticExpression.md
+-rw-r--r--   0        0        0      295 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/ArithmeticOperator.md
+-rw-r--r--   0        0        0      317 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/Body.md
+-rw-r--r--   0        0        0      357 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/Body1.md
+-rw-r--r--   0        0        0      508 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/Body2.md
+-rw-r--r--   0        0        0      361 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/Body3.md
+-rw-r--r--   0        0        0      323 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/Body4.md
+-rw-r--r--   0        0        0      322 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/Body5.md
+-rw-r--r--   0        0        0      578 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/BooleanExpression.md
+-rw-r--r--   0        0        0     1037 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/Code.md
+-rw-r--r--   0        0        0     1251 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/Cohort.md
+-rw-r--r--   0        0        0     1234 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CohortDefinition.md
+-rw-r--r--   0        0        0      723 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CohortFilter.md
+-rw-r--r--   0        0        0      408 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CohortFilterCondition.md
+-rw-r--r--   0        0        0      887 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CohortJoinedCohortResponseDto.md
+-rw-r--r--   0        0        0     1192 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CohortJoinedModelJobResponseDto.md
+-rw-r--r--   0        0        0     1201 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CohortResponseDto.md
+-rw-r--r--   0        0        0     1616 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CohortResults.md
+-rw-r--r--   0        0        0      874 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CohortSet.md
+-rw-r--r--   0        0        0     1646 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CohortWindow.md
+-rw-r--r--   0        0        0    20143 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CohortsApi.md
+-rw-r--r--   0        0        0      384 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/Condition.md
+-rw-r--r--   0        0        0      294 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/ConditionOperator.md
+-rw-r--r--   0        0        0      815 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/ContainerConfig.md
+-rw-r--r--   0        0        0      413 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateAnalysisDto.md
+-rw-r--r--   0        0        0      635 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateAnalysisJobDto.md
+-rw-r--r--   0        0        0      392 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateAnalysisJobOutputDto.md
+-rw-r--r--   0        0        0      610 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateAnalysisJobStatusDto.md
+-rw-r--r--   0        0        0      531 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateCohortDto.md
+-rw-r--r--   0        0        0      533 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateDataQueryDto.md
+-rw-r--r--   0        0        0      415 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateDataStoreDto.md
+-rw-r--r--   0        0        0      478 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateDataTableDto.md
+-rw-r--r--   0        0        0      453 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateDatabaseDto.md
+-rw-r--r--   0        0        0      420 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateDatasetColumnDto.md
+-rw-r--r--   0        0        0      963 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateDatasetDto.md
+-rw-r--r--   0        0        0      684 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateFeatureDto.md
+-rw-r--r--   0        0        0      418 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateFeatureStoreDto.md
+-rw-r--r--   0        0        0      349 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyAnalysisDto.md
+-rw-r--r--   0        0        0      358 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyAnalysisJobDto.md
+-rw-r--r--   0        0        0      376 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyAnalysisJobOutputDto.md
+-rw-r--r--   0        0        0      376 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyAnalysisJobStatusDto.md
+-rw-r--r--   0        0        0      337 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyCodeDto.md
+-rw-r--r--   0        0        0      343 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyCohortDto.md
+-rw-r--r--   0        0        0      352 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyDataQueryDto.md
+-rw-r--r--   0        0        0      352 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyDataStoreDto.md
+-rw-r--r--   0        0        0      364 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyDatasetColumnDto.md
+-rw-r--r--   0        0        0      346 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyDatasetDto.md
+-rw-r--r--   0        0        0      355 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyDatasetJobDto.md
+-rw-r--r--   0        0        0      358 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyEnvironmentDto.md
+-rw-r--r--   0        0        0      370 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyFeatureCategoryDto.md
+-rw-r--r--   0        0        0      346 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyFeatureDto.md
+-rw-r--r--   0        0        0      361 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyFeatureStoreDto.md
+-rw-r--r--   0        0        0      379 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyFeatureSubCategoryDto.md
+-rw-r--r--   0        0        0      355 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyModelBatchDto.md
+-rw-r--r--   0        0        0      364 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyModelBatchJobDto.md
+-rw-r--r--   0        0        0      361 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyModelDatasetDto.md
+-rw-r--r--   0        0        0      340 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyModelDto.md
+-rw-r--r--   0        0        0      364 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyModelEndpointDto.md
+-rw-r--r--   0        0        0      349 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyModelJobDto.md
+-rw-r--r--   0        0        0      367 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyModelJobOutputDto.md
+-rw-r--r--   0        0        0      388 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyModelJobOutputFeatureDto.md
+-rw-r--r--   0        0        0      370 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyModelPopulationDto.md
+-rw-r--r--   0        0        0      361 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyOrganizationDto.md
+-rw-r--r--   0        0        0      409 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyOrganizationFeatureExclusionDto.md
+-rw-r--r--   0        0        0      382 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyOrganizationSettingDto.md
+-rw-r--r--   0        0        0      370 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyPopulationStoreDto.md
+-rw-r--r--   0        0        0      346 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyProcessDto.md
+-rw-r--r--   0        0        0      355 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyProcessJobDto.md
+-rw-r--r--   0        0        0      373 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyProcessJobOutputDto.md
+-rw-r--r--   0        0        0      373 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyProcessJobStatusDto.md
+-rw-r--r--   0        0        0      346 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyProjectDto.md
+-rw-r--r--   0        0        0      364 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyProjectMemberDto.md
+-rw-r--r--   0        0        0      352 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManySchedulerDto.md
+-rw-r--r--   0        0        0      337 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyTaskDto.md
+-rw-r--r--   0        0        0      364 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyTaskExecutionDto.md
+-rw-r--r--   0        0        0      382 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyTaskExecutionStatusDto.md
+-rw-r--r--   0        0        0      361 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyUserFavoriteDto.md
+-rw-r--r--   0        0        0      349 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyWorkflowDto.md
+-rw-r--r--   0        0        0      376 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyWorkflowExecutionDto.md
+-rw-r--r--   0        0        0      388 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyWorkflowExecutionSpecDto.md
+-rw-r--r--   0        0        0      373 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateManyWorkflowTemplateDto.md
+-rw-r--r--   0        0        0      370 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateModelBatchDto.md
+-rw-r--r--   0        0        0      616 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateModelBatchJobDto.md
+-rw-r--r--   0        0        0      648 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateModelDto.md
+-rw-r--r--   0        0        0      872 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateModelJobDto.md
+-rw-r--r--   0        0        0      431 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateModelJobOutputDto.md
+-rw-r--r--   0        0        0      626 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateModelJobStatusDto.md
+-rw-r--r--   0        0        0     1131 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateModelPopulationDto.md
+-rw-r--r--   0        0        0      405 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateOrganizationDto.md
+-rw-r--r--   0        0        0      731 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateOrganizationSettingDto.md
+-rw-r--r--   0        0        0      421 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreatePopulationStoreDto.md
+-rw-r--r--   0        0        0      430 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateProcessDto.md
+-rw-r--r--   0        0        0      620 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateProcessJobDto.md
+-rw-r--r--   0        0        0      390 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateProcessJobOutputDto.md
+-rw-r--r--   0        0        0      663 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateProcessJobStatusDto.md
+-rw-r--r--   0        0        0      457 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateProjectDto.md
+-rw-r--r--   0        0        0      433 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateProjectMemberDto.md
+-rw-r--r--   0        0        0      647 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateSchedulerDto.md
+-rw-r--r--   0        0        0      510 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateTaskDto.md
+-rw-r--r--   0        0        0      754 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateTaskExecutionDto.md
+-rw-r--r--   0        0        0      434 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateTaskExecutionStatusDto.md
+-rw-r--r--   0        0        0      500 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateUserAuditTrailDto.md
+-rw-r--r--   0        0        0      437 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateUserFavoriteDto.md
+-rw-r--r--   0        0        0      394 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateWorkflowDto.md
+-rw-r--r--   0        0        0      554 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateWorkflowExecutionDto.md
+-rw-r--r--   0        0        0      525 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateWorkflowExecutionSpecDto.md
+-rw-r--r--   0        0        0      438 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateWorkflowExecutionStatusDto.md
+-rw-r--r--   0        0        0      555 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/CreateWorkflowTemplateDto.md
+-rw-r--r--   0        0        0    19877 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DataQueriesApi.md
+-rw-r--r--   0        0        0      947 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DataQuery.md
+-rw-r--r--   0        0        0     1322 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DataQueryJoinedDatasetResponseDto.md
+-rw-r--r--   0        0        0      938 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DataQueryResponseDto.md
+-rw-r--r--   0        0        0      820 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DataStore.md
+-rw-r--r--   0        0        0      759 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DataStoreResponseDto.md
+-rw-r--r--   0        0        0    17872 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DataStoresApi.md
+-rw-r--r--   0        0        0      898 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DataTable.md
+-rw-r--r--   0        0        0      801 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DataTableJoinedDatabaseResponseDto.md
+-rw-r--r--   0        0        0     1322 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DataTableJoinedDatasetResponseDto.md
+-rw-r--r--   0        0        0      985 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DataTableResponseDto.md
+-rw-r--r--   0        0        0     8627 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DataTablesApi.md
+-rw-r--r--   0        0        0      913 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/Database.md
+-rw-r--r--   0        0        0      778 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DatabaseJoinedDataTableResponseDto.md
+-rw-r--r--   0        0        0      896 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DatabaseResponseDto.md
+-rw-r--r--   0        0        0    11707 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DatabasesApi.md
+-rw-r--r--   0        0        0     1788 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/Dataset.md
+-rw-r--r--   0        0        0      774 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DatasetColumn.md
+-rw-r--r--   0        0        0     1326 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DatasetColumnJoinedDatasetResponseDto.md
+-rw-r--r--   0        0        0      845 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DatasetColumnResponseDto.md
+-rw-r--r--   0        0        0    18544 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DatasetColumnsApi.md
+-rw-r--r--   0        0        0      898 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DatasetJob.md
+-rw-r--r--   0        0        0      804 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DatasetJobStatus.md
+-rw-r--r--   0        0        0      842 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DatasetJoinedDataQueryResponseDto.md
+-rw-r--r--   0        0        0      741 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DatasetJoinedDatasetColumnResponseDto.md
+-rw-r--r--   0        0        0     1544 2023-06-14 19:39:44.864363 curia-4.2.0b9/src/curia/api/docs/DatasetResponseDto.md
+-rw-r--r--   0        0        0    33268 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/DatasetsApi.md
+-rw-r--r--   0        0        0      391 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/DatasetsuploadlargecompleteParts.md
+-rw-r--r--   0        0        0     1072 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/Environment.md
+-rw-r--r--   0        0        0      674 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/EnvironmentActivity.md
+-rw-r--r--   0        0        0     1291 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/Feature.md
+-rw-r--r--   0        0        0      877 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/FeatureCategory.md
+-rw-r--r--   0        0        0      671 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/FeatureJoinedFeatureSubCategoryJoinedFeatureCategoryResponseDto.md
+-rw-r--r--   0        0        0      868 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/FeatureJoinedFeatureSubCategoryResponseDto.md
+-rw-r--r--   0        0        0     1499 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/FeatureJoinedModelPopulationResponseDto.md
+-rw-r--r--   0        0        0      691 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/FeatureJoinedOrganizationFeatureExclusionResponseDto.md
+-rw-r--r--   0        0        0     1434 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/FeatureResponseDto.md
+-rw-r--r--   0        0        0      823 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/FeatureStore.md
+-rw-r--r--   0        0        0      762 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/FeatureStoreResponseDto.md
+-rw-r--r--   0        0        0    18376 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/FeatureStoresApi.md
+-rw-r--r--   0        0        0      812 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/FeatureSubCategory.md
+-rw-r--r--   0        0        0      789 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/FeatureTable.md
+-rw-r--r--   0        0        0    17445 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/FeaturesApi.md
+-rw-r--r--   0        0        0      775 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GeographicCounts.md
+-rw-r--r--   0        0        0      656 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GeographicQueries.md
+-rw-r--r--   0        0        0      519 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyAnalysisJobOutputResponseDto.md
+-rw-r--r--   0        0        0      501 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyAnalysisJobResponseDto.md
+-rw-r--r--   0        0        0      519 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyAnalysisJobStatusResponseDto.md
+-rw-r--r--   0        0        0      492 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyAnalysisResponseDto.md
+-rw-r--r--   0        0        0      458 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyCodeResponseDto.md
+-rw-r--r--   0        0        0      486 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyCohortResponseDto.md
+-rw-r--r--   0        0        0      495 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyDataQueryResponseDto.md
+-rw-r--r--   0        0        0      495 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyDataStoreResponseDto.md
+-rw-r--r--   0        0        0      495 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyDataTableResponseDto.md
+-rw-r--r--   0        0        0      492 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyDatabaseResponseDto.md
+-rw-r--r--   0        0        0      507 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyDatasetColumnResponseDto.md
+-rw-r--r--   0        0        0      476 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyDatasetJobResponseDto.md
+-rw-r--r--   0        0        0      494 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyDatasetJobStatusResponseDto.md
+-rw-r--r--   0        0        0      489 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyDatasetResponseDto.md
+-rw-r--r--   0        0        0      479 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyEnvironmentResponseDto.md
+-rw-r--r--   0        0        0      491 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyFeatureCategoryResponseDto.md
+-rw-r--r--   0        0        0      489 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyFeatureResponseDto.md
+-rw-r--r--   0        0        0      504 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyFeatureStoreResponseDto.md
+-rw-r--r--   0        0        0      500 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyFeatureSubCategoryResponseDto.md
+-rw-r--r--   0        0        0      507 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyModelBatchJobResponseDto.md
+-rw-r--r--   0        0        0      498 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyModelBatchResponseDto.md
+-rw-r--r--   0        0        0      482 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyModelDatasetResponseDto.md
+-rw-r--r--   0        0        0      485 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyModelEndpointResponseDto.md
+-rw-r--r--   0        0        0      485 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyModelJobEventResponseDto.md
+-rw-r--r--   0        0        0      509 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyModelJobOutputFeatureResponseDto.md
+-rw-r--r--   0        0        0      510 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyModelJobOutputResponseDto.md
+-rw-r--r--   0        0        0      492 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyModelJobResponseDto.md
+-rw-r--r--   0        0        0      510 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyModelJobStatusResponseDto.md
+-rw-r--r--   0        0        0      513 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyModelPopulationResponseDto.md
+-rw-r--r--   0        0        0      483 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyModelResponseDto.md
+-rw-r--r--   0        0        0      530 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyOrganizationFeatureExclusionResponseDto.md
+-rw-r--r--   0        0        0      504 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyOrganizationResponseDto.md
+-rw-r--r--   0        0        0      525 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyOrganizationSettingResponseDto.md
+-rw-r--r--   0        0        0      513 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyPopulationStoreResponseDto.md
+-rw-r--r--   0        0        0      516 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyProcessJobOutputResponseDto.md
+-rw-r--r--   0        0        0      498 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyProcessJobResponseDto.md
+-rw-r--r--   0        0        0      516 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyProcessJobStatusResponseDto.md
+-rw-r--r--   0        0        0      489 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyProcessResponseDto.md
+-rw-r--r--   0        0        0      507 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyProjectMemberResponseDto.md
+-rw-r--r--   0        0        0      489 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyProjectResponseDto.md
+-rw-r--r--   0        0        0      495 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManySchedulerResponseDto.md
+-rw-r--r--   0        0        0      507 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyTaskExecutionResponseDto.md
+-rw-r--r--   0        0        0      525 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyTaskExecutionStatusResponseDto.md
+-rw-r--r--   0        0        0      480 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyTaskResponseDto.md
+-rw-r--r--   0        0        0      510 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyUserAuditTrailResponseDto.md
+-rw-r--r--   0        0        0      504 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyUserFavoriteResponseDto.md
+-rw-r--r--   0        0        0      519 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyWorkflowExecutionResponseDto.md
+-rw-r--r--   0        0        0      531 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyWorkflowExecutionSpecResponseDto.md
+-rw-r--r--   0        0        0      537 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyWorkflowExecutionStatusResponseDto.md
+-rw-r--r--   0        0        0      492 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyWorkflowResponseDto.md
+-rw-r--r--   0        0        0      516 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/GetManyWorkflowTemplateResponseDto.md
+-rw-r--r--   0        0        0      615 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/InlineResponse200.md
+-rw-r--r--   0        0        0      336 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/InlineResponse200Info.md
+-rw-r--r--   0        0        0      615 2023-06-14 19:39:44.868363 curia-4.2.0b9/src/curia/api/docs/InlineResponse503.md
+-rw-r--r--   0        0        0    21159 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/InternalApi.md
+-rw-r--r--   0        0        0      968 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/InterventionDefinition.md
+-rw-r--r--   0        0        0      281 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/Json.md
+-rw-r--r--   0        0        0      292 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/LogicalOperator.md
+-rw-r--r--   0        0        0     1303 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/Model.md
+-rw-r--r--   0        0        0      914 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelBatch.md
+-rw-r--r--   0        0        0     1319 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelBatchJob.md
+-rw-r--r--   0        0        0      836 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelBatchJobJoinedModelBatchJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0      846 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelBatchJobJoinedModelBatchResponseDto.md
+-rw-r--r--   0        0        0     1051 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelBatchJobResponseDto.md
+-rw-r--r--   0        0        0    25416 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelBatchJobsApi.md
+-rw-r--r--   0        0        0      817 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelBatchJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0      789 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelBatchResponseDto.md
+-rw-r--r--   0        0        0    19271 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelBatchesApi.md
+-rw-r--r--   0        0        0      760 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelDataset.md
+-rw-r--r--   0        0        0      716 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelEndpoint.md
+-rw-r--r--   0        0        0     1899 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJob.md
+-rw-r--r--   0        0        0      698 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobConfig.md
+-rw-r--r--   0        0        0      946 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobEvent.md
+-rw-r--r--   0        0        0      889 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedCohortResponseDto.md
+-rw-r--r--   0        0        0      843 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedDataQueryResponseDto.md
+-rw-r--r--   0        0        0     1321 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedDatasetResponseDto.md
+-rw-r--r--   0        0        0      691 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedFeatureSubCategoryResponseDto.md
+-rw-r--r--   0        0        0      753 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelJobOutputResponseDto.md
+-rw-r--r--   0        0        0      948 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelJobStatusResponseDto.md
+-rw-r--r--   0        0        0      762 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedCohortDefinitionJoinedPeriodDefinitionResponseDto.md
+-rw-r--r--   0        0        0     1116 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedCohortDefinitionResponseDto.md
+-rw-r--r--   0        0        0     1357 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedDataQueryJoinedDatasetResponseDto.md
+-rw-r--r--   0        0        0     1043 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedDataQueryResponseDto.md
+-rw-r--r--   0        0        0      802 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedInterventionDefinitionResponseDto.md
+-rw-r--r--   0        0        0      969 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedOutcomeDefinitionResponseDto.md
+-rw-r--r--   0        0        0     2176 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationResponseDto.md
+-rw-r--r--   0        0        0      970 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelResponseDto.md
+-rw-r--r--   0        0        0      815 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0      846 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobOutput.md
+-rw-r--r--   0        0        0      738 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobOutputFeature.md
+-rw-r--r--   0        0        0     1327 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobOutputJoinedDatasetResponseDto.md
+-rw-r--r--   0        0        0      835 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobOutputJoinedModelJobJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0     1347 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobOutputJoinedModelJobResponseDto.md
+-rw-r--r--   0        0        0      981 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobOutputResponseDto.md
+-rw-r--r--   0        0        0    18734 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobOutputsApi.md
+-rw-r--r--   0        0        0     2268 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobResponseDto.md
+-rw-r--r--   0        0        0     1041 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobStatus.md
+-rw-r--r--   0        0        0      835 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobStatusJoinedModelJobJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0     1347 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobStatusJoinedModelJobResponseDto.md
+-rw-r--r--   0        0        0     1057 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobStatusResponseDto.md
+-rw-r--r--   0        0        0    10815 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobStatusesApi.md
+-rw-r--r--   0        0        0    24358 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJobsApi.md
+-rw-r--r--   0        0        0     1203 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJoinedCohortJoinedModelJobResponseDto.md
+-rw-r--r--   0        0        0     1016 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJoinedCohortResponseDto.md
+-rw-r--r--   0        0        0      900 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJoinedModelJobJoinedCohortResponseDto.md
+-rw-r--r--   0        0        0     1332 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJoinedModelJobJoinedDatasetResponseDto.md
+-rw-r--r--   0        0        0      702 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJoinedModelJobJoinedFeatureSubCategoryResponseDto.md
+-rw-r--r--   0        0        0     1612 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJoinedModelJobResponseDto.md
+-rw-r--r--   0        0        0     1231 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJoinedModelOutputDetailsResponseDto.md
+-rw-r--r--   0        0        0      812 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0      756 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelJoinedUserFavoriteResponseDto.md
+-rw-r--r--   0        0        0     1260 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelOutputDetails.md
+-rw-r--r--   0        0        0     2231 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelPopulation.md
+-rw-r--r--   0        0        0      748 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedCohortDefinitionJoinedPeriodDefinitionResponseDto.md
+-rw-r--r--   0        0        0     1074 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedCohortDefinitionResponseDto.md
+-rw-r--r--   0        0        0     1038 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedCohortResultsResponseDto.md
+-rw-r--r--   0        0        0     1343 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedDataQueryJoinedDatasetResponseDto.md
+-rw-r--r--   0        0        0     1001 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedDataQueryResponseDto.md
+-rw-r--r--   0        0        0     1013 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedFeatureResponseDto.md
+-rw-r--r--   0        0        0      788 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedInterventionDefinitionResponseDto.md
+-rw-r--r--   0        0        0      991 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedModelJobJoinedModelResponseDto.md
+-rw-r--r--   0        0        0     1344 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedModelJobResponseDto.md
+-rw-r--r--   0        0        0      955 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedOutcomeDefinitionResponseDto.md
+-rw-r--r--   0        0        0     2592 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelPopulationResponseDto.md
+-rw-r--r--   0        0        0    20616 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelPopulationsApi.md
+-rw-r--r--   0        0        0     1516 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelResponseDto.md
+-rw-r--r--   0        0        0    21791 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/ModelsApi.md
+-rw-r--r--   0        0        0      283 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/Object.md
+-rw-r--r--   0        0        0     2124 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/Organization.md
+-rw-r--r--   0        0        0      807 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/OrganizationFeatureCategoryExclusion.md
+-rw-r--r--   0        0        0      796 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/OrganizationFeatureExclusion.md
+-rw-r--r--   0        0        0      713 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/OrganizationResponseDto.md
+-rw-r--r--   0        0        0     1136 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/OrganizationSetting.md
+-rw-r--r--   0        0        0     1075 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/OrganizationSettingResponseDto.md
+-rw-r--r--   0        0        0    23020 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/OrganizationSettingsApi.md
+-rw-r--r--   0        0        0    18327 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/OrganizationsApi.md
+-rw-r--r--   0        0        0     1135 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/OutcomeDefinition.md
+-rw-r--r--   0        0        0      388 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/PeriodDefinition.md
+-rw-r--r--   0        0        0      287 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/PeriodType.md
+-rw-r--r--   0        0        0      510 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/PersonSet.md
+-rw-r--r--   0        0        0      381 2023-06-14 19:39:44.872363 curia-4.2.0b9/src/curia/api/docs/PipelineConfig.md
+-rw-r--r--   0        0        0   600317 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/PlatformApi.md
+-rw-r--r--   0        0        0     1268 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/Population.md
+-rw-r--r--   0        0        0      899 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/PopulationStore.md
+-rw-r--r--   0        0        0      765 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/PopulationStoreResponseDto.md
+-rw-r--r--   0        0        0    18880 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/PopulationStoresApi.md
+-rw-r--r--   0        0        0      918 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/Process.md
+-rw-r--r--   0        0        0     1264 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJob.md
+-rw-r--r--   0        0        0      386 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJobConfig.md
+-rw-r--r--   0        0        0      817 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJobJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0      743 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJobOutput.md
+-rw-r--r--   0        0        0      839 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJobOutputJoinedProcessJobJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0     1105 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJobOutputJoinedProcessJobResponseDto.md
+-rw-r--r--   0        0        0      831 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJobOutputResponseDto.md
+-rw-r--r--   0        0        0    20335 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJobOutputsApi.md
+-rw-r--r--   0        0        0     1039 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJobResponseDto.md
+-rw-r--r--   0        0        0     1084 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJobStatus.md
+-rw-r--r--   0        0        0      823 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJobStatusJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0     1094 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJobStatusResponseDto.md
+-rw-r--r--   0        0        0    20370 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJobStatusesApi.md
+-rw-r--r--   0        0        0    22718 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJobsApi.md
+-rw-r--r--   0        0        0      814 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0      843 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessResponseDto.md
+-rw-r--r--   0        0        0      288 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessType.md
+-rw-r--r--   0        0        0    18676 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProcessesApi.md
+-rw-r--r--   0        0        0     1452 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/Project.md
+-rw-r--r--   0        0        0      899 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProjectJoinedModelJoinedCohortResponseDto.md
+-rw-r--r--   0        0        0     1094 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProjectJoinedModelResponseDto.md
+-rw-r--r--   0        0        0      814 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProjectJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0      758 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProjectJoinedUserFavoriteResponseDto.md
+-rw-r--r--   0        0        0      787 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProjectMember.md
+-rw-r--r--   0        0        0      820 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProjectMemberJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0      858 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProjectMemberResponseDto.md
+-rw-r--r--   0        0        0    18544 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProjectMembersApi.md
+-rw-r--r--   0        0        0     1250 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProjectResponseDto.md
+-rw-r--r--   0        0        0    22464 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/ProjectsApi.md
+-rw-r--r--   0        0        0     1112 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/Scheduler.md
+-rw-r--r--   0        0        0    17759 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/SchedulerApi.md
+-rw-r--r--   0        0        0      753 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/SchedulerJoinedWorkflowResponseDto.md
+-rw-r--r--   0        0        0     1103 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/SchedulerResponseDto.md
+-rw-r--r--   0        0        0      500 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/SelectExpression.md
+-rw-r--r--   0        0        0      288 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/SetOperator.md
+-rw-r--r--   0        0        0      425 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/StateData.md
+-rw-r--r--   0        0        0      993 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/Task.md
+-rw-r--r--   0        0        0     1275 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/TaskExecution.md
+-rw-r--r--   0        0        0      873 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/TaskExecutionJoinedTaskResponseDto.md
+-rw-r--r--   0        0        0      917 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/TaskExecutionJoinedWorkflowExecutionResponseDto.md
+-rw-r--r--   0        0        0     1318 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/TaskExecutionResponseDto.md
+-rw-r--r--   0        0        0      802 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/TaskExecutionStatus.md
+-rw-r--r--   0        0        0      942 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/TaskExecutionStatusJoinedTaskExecutionJoinedWorkflowExecutionResponseDto.md
+-rw-r--r--   0        0        0     1285 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/TaskExecutionStatusJoinedTaskExecutionResponseDto.md
+-rw-r--r--   0        0        0      885 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/TaskExecutionStatusResponseDto.md
+-rw-r--r--   0        0        0      287 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/TaskInputs.md
+-rw-r--r--   0        0        0      288 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/TaskOutputs.md
+-rw-r--r--   0        0        0      854 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/TaskResponseDto.md
+-rw-r--r--   0        0        0    21547 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/TasksApi.md
+-rw-r--r--   0        0        0      446 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateAnalysisDto.md
+-rw-r--r--   0        0        0      668 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateAnalysisJobDto.md
+-rw-r--r--   0        0        0      425 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateAnalysisJobOutputDto.md
+-rw-r--r--   0        0        0      665 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateAnalysisJobStatusDto.md
+-rw-r--r--   0        0        0      542 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateCohortDto.md
+-rw-r--r--   0        0        0      544 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateDataQueryDto.md
+-rw-r--r--   0        0        0      415 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateDataStoreDto.md
+-rw-r--r--   0        0        0      500 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateDataTableDto.md
+-rw-r--r--   0        0        0      464 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateDatabaseDto.md
+-rw-r--r--   0        0        0      453 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateDatasetColumnDto.md
+-rw-r--r--   0        0        0      985 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateDatasetDto.md
+-rw-r--r--   0        0        0      794 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateFeatureDto.md
+-rw-r--r--   0        0        0      418 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateFeatureStoreDto.md
+-rw-r--r--   0        0        0      381 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateModelBatchDto.md
+-rw-r--r--   0        0        0      649 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateModelBatchJobDto.md
+-rw-r--r--   0        0        0      692 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateModelDto.md
+-rw-r--r--   0        0        0      905 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateModelJobDto.md
+-rw-r--r--   0        0        0      464 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateModelJobOutputDto.md
+-rw-r--r--   0        0        0      659 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateModelJobStatusDto.md
+-rw-r--r--   0        0        0     1131 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateModelPopulationDto.md
+-rw-r--r--   0        0        0      416 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateOrganizationDto.md
+-rw-r--r--   0        0        0      742 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateOrganizationSettingDto.md
+-rw-r--r--   0        0        0      421 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdatePopulationStoreDto.md
+-rw-r--r--   0        0        0      452 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateProcessDto.md
+-rw-r--r--   0        0        0      642 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateProcessJobDto.md
+-rw-r--r--   0        0        0      423 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateProcessJobOutputDto.md
+-rw-r--r--   0        0        0      663 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateProcessJobStatusDto.md
+-rw-r--r--   0        0        0      468 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateProjectDto.md
+-rw-r--r--   0        0        0      466 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateProjectMemberDto.md
+-rw-r--r--   0        0        0      691 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateSchedulerDto.md
+-rw-r--r--   0        0        0      532 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateTaskDto.md
+-rw-r--r--   0        0        0      776 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateTaskExecutionDto.md
+-rw-r--r--   0        0        0      467 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateTaskExecutionStatusDto.md
+-rw-r--r--   0        0        0      555 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateUserAuditTrailDto.md
+-rw-r--r--   0        0        0      736 2023-06-14 19:39:44.876363 curia-4.2.0b9/src/curia/api/docs/UpdateUserDto.md
+-rw-r--r--   0        0        0      437 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UpdateUserFavoriteDto.md
+-rw-r--r--   0        0        0      416 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UpdateWorkflowDto.md
+-rw-r--r--   0        0        0      565 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UpdateWorkflowExecutionDto.md
+-rw-r--r--   0        0        0      547 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UpdateWorkflowExecutionSpecDto.md
+-rw-r--r--   0        0        0      471 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UpdateWorkflowExecutionStatusDto.md
+-rw-r--r--   0        0        0      577 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UpdateWorkflowTemplateDto.md
+-rw-r--r--   0        0        0      708 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UserAuditTrail.md
+-rw-r--r--   0        0        0     8869 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UserAuditTrailApi.md
+-rw-r--r--   0        0        0      686 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UserAuditTrailResponseDto.md
+-rw-r--r--   0        0        0      842 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UserFavorite.md
+-rw-r--r--   0        0        0      830 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UserFavoriteJoinedModelJoinedProjectResponseDto.md
+-rw-r--r--   0        0        0     1111 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UserFavoriteJoinedModelResponseDto.md
+-rw-r--r--   0        0        0      854 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UserFavoriteResponseDto.md
+-rw-r--r--   0        0        0    18376 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UserFavoritesApi.md
+-rw-r--r--   0        0        0    29151 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/UserManagementApi.md
+-rw-r--r--   0        0        0     1031 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/Workflow.md
+-rw-r--r--   0        0        0     1197 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowExecution.md
+-rw-r--r--   0        0        0      898 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionResponseDto.md
+-rw-r--r--   0        0        0      901 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionSpec.md
+-rw-r--r--   0        0        0      925 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionSpecJoinedWorkflowExecutionResponseDto.md
+-rw-r--r--   0        0        0      988 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionSpecResponseDto.md
+-rw-r--r--   0        0        0      814 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionStatus.md
+-rw-r--r--   0        0        0      927 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionStatusJoinedWorkflowExecutionResponseDto.md
+-rw-r--r--   0        0        0      905 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionStatusResponseDto.md
+-rw-r--r--   0        0        0     1005 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowJoinedSchedulerResponseDto.md
+-rw-r--r--   0        0        0      912 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowJoinedWorkflowExecutionResponseDto.md
+-rw-r--r--   0        0        0      913 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowJoinedWorkflowTemplateResponseDto.md
+-rw-r--r--   0        0        0     1108 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowResponseDto.md
+-rw-r--r--   0        0        0     1020 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowTemplate.md
+-rw-r--r--   0        0        0      511 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowTemplateDefinition.md
+-rw-r--r--   0        0        0      303 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowTemplateParameters.md
+-rw-r--r--   0        0        0      899 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowTemplateResponseDto.md
+-rw-r--r--   0        0        0    39666 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/WorkflowsApi.md
+-rw-r--r--   0        0        0      421 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/docs/ZipData.md
+-rw-r--r--   0        0        0     1663 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/git_push.sh
+-rw-r--r--   0        0        0       96 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/requirements.txt
+-rw-r--r--   0        0        0     1004 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/setup.py
+-rw-r--r--   0        0        0    31428 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/swagger_client/__init__.py
+-rw-r--r--   0        0        0     2061 2023-06-14 19:39:44.880363 curia-4.2.0b9/src/curia/api/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0    33328 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/analyses_api.py
+-rw-r--r--   0        0        0    35040 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/analysis_job_outputs_api.py
+-rw-r--r--   0        0        0    35052 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/analysis_job_statuses_api.py
+-rw-r--r--   0        0        0    40946 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/analysis_jobs_api.py
+-rw-r--r--   0        0        0    39722 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/cohorts_api.py
+-rw-r--r--   0        0        0    37585 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/data_queries_api.py
+-rw-r--r--   0        0        0    33603 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/data_stores_api.py
+-rw-r--r--   0        0        0    13421 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/data_tables_api.py
+-rw-r--r--   0        0        0    19439 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/databases_api.py
+-rw-r--r--   0        0        0    34251 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/dataset_columns_api.py
+-rw-r--r--   0        0        0    67869 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/datasets_api.py
+-rw-r--r--   0        0        0    34089 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/feature_stores_api.py
+-rw-r--r--   0        0        0    33158 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/features_api.py
+-rw-r--r--   0        0        0    40513 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/internal_api.py
+-rw-r--r--   0        0        0    45647 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/model_batch_jobs_api.py
+-rw-r--r--   0        0        0    33797 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/model_batches_api.py
+-rw-r--r--   0        0        0    34483 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/model_job_outputs_api.py
+-rw-r--r--   0        0        0    17685 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/model_job_statuses_api.py
+-rw-r--r--   0        0        0    48185 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/model_jobs_api.py
+-rw-r--r--   0        0        0    38516 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/model_populations_api.py
+-rw-r--r--   0        0        0    43120 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/models_api.py
+-rw-r--r--   0        0        0    41842 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/organization_settings_api.py
+-rw-r--r--   0        0        0    34025 2023-06-14 19:39:44.884363 curia-4.2.0b9/src/curia/api/swagger_client/api/organizations_api.py
+-rw-r--r--   0        0        0  1122558 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/platform_api.py
+-rw-r--r--   0        0        0    34575 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/population_stores_api.py
+-rw-r--r--   0        0        0    34878 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/process_job_outputs_api.py
+-rw-r--r--   0        0        0    34890 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/process_job_statuses_api.py
+-rw-r--r--   0        0        0    40786 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/process_jobs_api.py
+-rw-r--r--   0        0        0    33190 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/processes_api.py
+-rw-r--r--   0        0        0    34251 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/project_members_api.py
+-rw-r--r--   0        0        0    43631 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/projects_api.py
+-rw-r--r--   0        0        0    33481 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/scheduler_api.py
+-rw-r--r--   0        0        0    42423 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/tasks_api.py
+-rw-r--r--   0        0        0    13665 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/user_audit_trail_api.py
+-rw-r--r--   0        0        0    34089 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/user_favorites_api.py
+-rw-r--r--   0        0        0    60855 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/user_management_api.py
+-rw-r--r--   0        0        0    74957 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api/workflows_api.py
+-rw-r--r--   0        0        0    24824 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8257 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/configuration.py
+-rw-r--r--   0        0        0    29282 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     2579 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/aggregation_type.py
+-rw-r--r--   0        0        0     2804 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_cohort_model.py
+-rw-r--r--   0        0        0     2888 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_cohort_organization.py
+-rw-r--r--   0        0        0     2836 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_cohort_train_cohort.py
+-rw-r--r--   0        0        0     2820 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_data_table_dataset.py
+-rw-r--r--   0        0        0     2816 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_cohorts.py
+-rw-r--r--   0        0        0     2836 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_job_dataset.py
+-rw-r--r--   0        0        0     2884 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_job_environment.py
+-rw-r--r--   0        0        0     2812 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_job_model.py
+-rw-r--r--   0        0        0     2836 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_job_project.py
+-rw-r--r--   0        0        0     2841 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_model_jobs.py
+-rw-r--r--   0        0        0     2824 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_project.py
+-rw-r--r--   0        0        0    13573 2023-06-14 19:39:44.888363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis.py
+-rw-r--r--   0        0        0    18641 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job.py
+-rw-r--r--   0        0        0     5946 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_config.py
+-rw-r--r--   0        0        0    12323 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0    11100 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_output.py
+-rw-r--r--   0        0        0    13519 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0    16307 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_response_dto.py
+-rw-r--r--   0        0        0    11639 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_output_response_dto.py
+-rw-r--r--   0        0        0    14674 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_response_dto.py
+-rw-r--r--   0        0        0    15317 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_status.py
+-rw-r--r--   0        0        0    12635 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_status_joined_project_response_dto.py
+-rw-r--r--   0        0        0    15431 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_status_response_dto.py
+-rw-r--r--   0        0        0     2549 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_type.py
+-rw-r--r--   0        0        0    12167 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_joined_project_response_dto.py
+-rw-r--r--   0        0        0    11343 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_response_dto.py
+-rw-r--r--   0        0        0     2521 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_type.py
+-rw-r--r--   0        0        0     2514 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/any_of_arithmetic_expression_value.py
+-rw-r--r--   0        0        0     2502 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/any_of_boolean_expression_value.py
+-rw-r--r--   0        0        0     2586 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/any_of_cohort_definition_patient_metadata_filters_items.py
+-rw-r--r--   0        0        0     2470 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/any_of_condition_value.py
+-rw-r--r--   0        0        0     4635 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/arithmetic_expression.py
+-rw-r--r--   0        0        0     2685 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/arithmetic_operator.py
+-rw-r--r--   0        0        0     2962 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/body.py
+-rw-r--r--   0        0        0     3545 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/body1.py
+-rw-r--r--   0        0        0     4880 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/body2.py
+-rw-r--r--   0        0        0     3657 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/body3.py
+-rw-r--r--   0        0        0     3069 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/body4.py
+-rw-r--r--   0        0        0     3015 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/body5.py
+-rw-r--r--   0        0        0     6747 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/boolean_expression.py
+-rw-r--r--   0        0        0    15654 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/code.py
+-rw-r--r--   0        0        0    15747 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/cohort.py
+-rw-r--r--   0        0        0    15751 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_definition.py
+-rw-r--r--   0        0        0    10333 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_filter.py
+-rw-r--r--   0        0        0     5722 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_filter_condition.py
+-rw-r--r--   0        0        0    12768 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_joined_cohort_response_dto.py
+-rw-r--r--   0        0        0    19274 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_joined_model_job_response_dto.py
+-rw-r--r--   0        0        0    14684 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_response_dto.py
+-rw-r--r--   0        0        0    22225 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_results.py
+-rw-r--r--   0        0        0    10728 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_set.py
+-rw-r--r--   0        0        0    24287 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_window.py
+-rw-r--r--   0        0        0     4438 2023-06-14 19:39:44.892363 curia-4.2.0b9/src/curia/api/swagger_client/models/condition.py
+-rw-r--r--   0        0        0     2702 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/condition_operator.py
+-rw-r--r--   0        0        0    11475 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/container_config.py
+-rw-r--r--   0        0        0     5531 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_analysis_dto.py
+-rw-r--r--   0        0        0     8644 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_analysis_job_dto.py
+-rw-r--r--   0        0        0     4881 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_analysis_job_output_dto.py
+-rw-r--r--   0        0        0     9264 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_analysis_job_status_dto.py
+-rw-r--r--   0        0        0     6174 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_cohort_dto.py
+-rw-r--r--   0        0        0     6672 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_data_query_dto.py
+-rw-r--r--   0        0        0     4465 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_data_store_dto.py
+-rw-r--r--   0        0        0     6098 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_data_table_dto.py
+-rw-r--r--   0        0        0     5373 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_database_dto.py
+-rw-r--r--   0        0        0     5411 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_dataset_column_dto.py
+-rw-r--r--   0        0        0    14417 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_dataset_dto.py
+-rw-r--r--   0        0        0    12449 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_feature_dto.py
+-rw-r--r--   0        0        0     4513 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_feature_store_dto.py
+-rw-r--r--   0        0        0     3204 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_analysis_dto.py
+-rw-r--r--   0        0        0     3237 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_analysis_job_dto.py
+-rw-r--r--   0        0        0     3303 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_analysis_job_output_dto.py
+-rw-r--r--   0        0        0     3303 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_analysis_job_status_dto.py
+-rw-r--r--   0        0        0     3161 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_code_dto.py
+-rw-r--r--   0        0        0     3192 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_cohort_dto.py
+-rw-r--r--   0        0        0     3225 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_data_query_dto.py
+-rw-r--r--   0        0        0     3225 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_data_store_dto.py
+-rw-r--r--   0        0        0     3269 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_dataset_column_dto.py
+-rw-r--r--   0        0        0     3203 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_dataset_dto.py
+-rw-r--r--   0        0        0     3226 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_dataset_job_dto.py
+-rw-r--r--   0        0        0     3237 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_environment_dto.py
+-rw-r--r--   0        0        0     3282 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_feature_category_dto.py
+-rw-r--r--   0        0        0     3203 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_feature_dto.py
+-rw-r--r--   0        0        0     3258 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_feature_store_dto.py
+-rw-r--r--   0        0        0     3315 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_feature_sub_category_dto.py
+-rw-r--r--   0        0        0     3226 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_batch_dto.py
+-rw-r--r--   0        0        0     3259 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_batch_job_dto.py
+-rw-r--r--   0        0        0     3248 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_dataset_dto.py
+-rw-r--r--   0        0        0     3181 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_dto.py
+-rw-r--r--   0        0        0     3259 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_endpoint_dto.py
+-rw-r--r--   0        0        0     3214 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_job_dto.py
+-rw-r--r--   0        0        0     3280 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_job_output_dto.py
+-rw-r--r--   0        0        0     3348 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_job_output_feature_dto.py
+-rw-r--r--   0        0        0     3291 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_population_dto.py
+-rw-r--r--   0        0        0     3258 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_organization_dto.py
+-rw-r--r--   0        0        0     3425 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_organization_feature_exclusion_dto.py
+-rw-r--r--   0        0        0     3335 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_organization_setting_dto.py
+-rw-r--r--   0        0        0     3291 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_population_store_dto.py
+-rw-r--r--   0        0        0     3193 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_process_dto.py
+-rw-r--r--   0        0        0     3226 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_process_job_dto.py
+-rw-r--r--   0        0        0     3292 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_process_job_output_dto.py
+-rw-r--r--   0        0        0     3292 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_process_job_status_dto.py
+-rw-r--r--   0        0        0     3203 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_project_dto.py
+-rw-r--r--   0        0        0     3269 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_project_member_dto.py
+-rw-r--r--   0        0        0     3225 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_scheduler_dto.py
+-rw-r--r--   0        0        0     3170 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_task_dto.py
+-rw-r--r--   0        0        0     3269 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_task_execution_dto.py
+-rw-r--r--   0        0        0     3335 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_task_execution_status_dto.py
+-rw-r--r--   0        0        0     3258 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_user_favorite_dto.py
+-rw-r--r--   0        0        0     3214 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_workflow_dto.py
+-rw-r--r--   0        0        0     3313 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_workflow_execution_dto.py
+-rw-r--r--   0        0        0     3357 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_workflow_execution_spec_dto.py
+-rw-r--r--   0        0        0     3302 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_workflow_template_dto.py
+-rw-r--r--   0        0        0     4024 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_batch_dto.py
+-rw-r--r--   0        0        0     9127 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_batch_job_dto.py
+-rw-r--r--   0        0        0    10402 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_dto.py
+-rw-r--r--   0        0        0    13134 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_job_dto.py
+-rw-r--r--   0        0        0     5529 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_job_output_dto.py
+-rw-r--r--   0        0        0     8923 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_job_status_dto.py
+-rw-r--r--   0        0        0    17030 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_population_dto.py
+-rw-r--r--   0        0        0     4606 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_organization_dto.py
+-rw-r--r--   0        0        0    10373 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_organization_setting_dto.py
+-rw-r--r--   0        0        0     4561 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_population_store_dto.py
+-rw-r--r--   0        0        0     5717 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_process_dto.py
+-rw-r--r--   0        0        0     8417 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_process_job_dto.py
+-rw-r--r--   0        0        0     4844 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_process_job_output_dto.py
+-rw-r--r--   0        0        0     8770 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_process_job_status_dto.py
+-rw-r--r--   0        0        0     5503 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_project_dto.py
+-rw-r--r--   0        0        0     5654 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_project_member_dto.py
+-rw-r--r--   0        0        0     8781 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_scheduler_dto.py
+-rw-r--r--   0        0        0     6113 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_task_dto.py
+-rw-r--r--   0        0        0     9916 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_task_execution_dto.py
+-rw-r--r--   0        0        0     5645 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_task_execution_status_dto.py
+-rw-r--r--   0        0        0     7646 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_user_audit_trail_dto.py
+-rw-r--r--   0        0        0     4939 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_user_favorite_dto.py
+-rw-r--r--   0        0        0     4712 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_workflow_dto.py
+-rw-r--r--   0        0        0     6968 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_workflow_execution_dto.py
+-rw-r--r--   0        0        0     5185 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_workflow_execution_spec_dto.py
+-rw-r--r--   0        0        0     5725 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_workflow_execution_status_dto.py
+-rw-r--r--   0        0        0     5707 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/create_workflow_template_dto.py
+-rw-r--r--   0        0        0    12708 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/data_query.py
+-rw-r--r--   0        0        0    21959 2023-06-14 19:39:44.896363 curia-4.2.0b9/src/curia/api/swagger_client/models/data_query_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0    12694 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/data_query_response_dto.py
+-rw-r--r--   0        0        0    10691 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/data_store.py
+-rw-r--r--   0        0        0    10467 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/data_store_response_dto.py
+-rw-r--r--   0        0        0    12128 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/data_table.py
+-rw-r--r--   0        0        0    12212 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/data_table_joined_database_response_dto.py
+-rw-r--r--   0        0        0    21959 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/data_table_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0    12902 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/data_table_response_dto.py
+-rw-r--r--   0        0        0    12245 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/database.py
+-rw-r--r--   0        0        0    12089 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/database_joined_data_table_response_dto.py
+-rw-r--r--   0        0        0    12170 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/database_response_dto.py
+-rw-r--r--   0        0        0    24496 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/dataset.py
+-rw-r--r--   0        0        0    10736 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_column.py
+-rw-r--r--   0        0        0    22359 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_column_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0    11398 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_column_response_dto.py
+-rw-r--r--   0        0        0    11516 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_job.py
+-rw-r--r--   0        0        0    11875 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_job_status.py
+-rw-r--r--   0        0        0    12663 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_joined_data_query_response_dto.py
+-rw-r--r--   0        0        0    11235 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_joined_dataset_column_response_dto.py
+-rw-r--r--   0        0        0    22191 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_response_dto.py
+-rw-r--r--   0        0        0     4007 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/datasetsuploadlargecomplete_parts.py
+-rw-r--r--   0        0        0    14049 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/environment.py
+-rw-r--r--   0        0        0     9848 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/environment_activity.py
+-rw-r--r--   0        0        0    19679 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/feature.py
+-rw-r--r--   0        0        0    10474 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/feature_category.py
+-rw-r--r--   0        0        0     9769 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_joined_feature_category_response_dto.py
+-rw-r--r--   0        0        0    11222 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_response_dto.py
+-rw-r--r--   0        0        0    24534 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/feature_joined_model_population_response_dto.py
+-rw-r--r--   0        0        0    10642 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/feature_joined_organization_feature_exclusion_response_dto.py
+-rw-r--r--   0        0        0    20827 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/feature_response_dto.py
+-rw-r--r--   0        0        0    10847 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/feature_store.py
+-rw-r--r--   0        0        0    10611 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/feature_store_response_dto.py
+-rw-r--r--   0        0        0    10733 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/feature_sub_category.py
+-rw-r--r--   0        0        0    12122 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/feature_table.py
+-rw-r--r--   0        0        0     8403 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/geographic_counts.py
+-rw-r--r--   0        0        0     8947 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/geographic_queries.py
+-rw-r--r--   0        0        0     6575 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_analysis_job_output_response_dto.py
+-rw-r--r--   0        0        0     6413 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_analysis_job_response_dto.py
+-rw-r--r--   0        0        0     6575 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_analysis_job_status_response_dto.py
+-rw-r--r--   0        0        0     6332 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_analysis_response_dto.py
+-rw-r--r--   0        0        0     6192 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_code_response_dto.py
+-rw-r--r--   0        0        0     6288 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_cohort_response_dto.py
+-rw-r--r--   0        0        0     6369 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_data_query_response_dto.py
+-rw-r--r--   0        0        0     6369 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_data_store_response_dto.py
+-rw-r--r--   0        0        0     6369 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_data_table_response_dto.py
+-rw-r--r--   0        0        0     6342 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_database_response_dto.py
+-rw-r--r--   0        0        0     6477 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_dataset_column_response_dto.py
+-rw-r--r--   0        0        0     6353 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_dataset_job_response_dto.py
+-rw-r--r--   0        0        0     6515 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_dataset_job_status_response_dto.py
+-rw-r--r--   0        0        0     6315 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_dataset_response_dto.py
+-rw-r--r--   0        0        0     6380 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_environment_response_dto.py
+-rw-r--r--   0        0        0     6489 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_feature_category_response_dto.py
+-rw-r--r--   0        0        0     6315 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_feature_response_dto.py
+-rw-r--r--   0        0        0     6450 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_feature_store_response_dto.py
+-rw-r--r--   0        0        0     6570 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_feature_sub_category_response_dto.py
+-rw-r--r--   0        0        0     6467 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_batch_job_response_dto.py
+-rw-r--r--   0        0        0     6386 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_batch_response_dto.py
+-rw-r--r--   0        0        0     6407 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_dataset_response_dto.py
+-rw-r--r--   0        0        0     6434 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_endpoint_response_dto.py
+-rw-r--r--   0        0        0     6434 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_job_event_response_dto.py
+-rw-r--r--   0        0        0     6651 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_job_output_feature_response_dto.py
+-rw-r--r--   0        0        0     6504 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_job_output_response_dto.py
+-rw-r--r--   0        0        0     6342 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_job_response_dto.py
+-rw-r--r--   0        0        0     6504 2023-06-14 19:39:44.900363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_job_status_response_dto.py
+-rw-r--r--   0        0        0     6531 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_population_response_dto.py
+-rw-r--r--   0        0        0     6261 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_response_dto.py
+-rw-r--r--   0        0        0     6840 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_organization_feature_exclusion_response_dto.py
+-rw-r--r--   0        0        0     6450 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_organization_response_dto.py
+-rw-r--r--   0        0        0     6639 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_organization_setting_response_dto.py
+-rw-r--r--   0        0        0     6531 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_population_store_response_dto.py
+-rw-r--r--   0        0        0     6548 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_process_job_output_response_dto.py
+-rw-r--r--   0        0        0     6386 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_process_job_response_dto.py
+-rw-r--r--   0        0        0     6548 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_process_job_status_response_dto.py
+-rw-r--r--   0        0        0     6305 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_process_response_dto.py
+-rw-r--r--   0        0        0     6477 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_project_member_response_dto.py
+-rw-r--r--   0        0        0     6315 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_project_response_dto.py
+-rw-r--r--   0        0        0     6369 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_scheduler_response_dto.py
+-rw-r--r--   0        0        0     6477 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_task_execution_response_dto.py
+-rw-r--r--   0        0        0     6639 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_task_execution_status_response_dto.py
+-rw-r--r--   0        0        0     6234 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_task_response_dto.py
+-rw-r--r--   0        0        0     6504 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_user_audit_trail_response_dto.py
+-rw-r--r--   0        0        0     6450 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_user_favorite_response_dto.py
+-rw-r--r--   0        0        0     6585 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_workflow_execution_response_dto.py
+-rw-r--r--   0        0        0     6693 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_workflow_execution_spec_response_dto.py
+-rw-r--r--   0        0        0     6747 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_workflow_execution_status_response_dto.py
+-rw-r--r--   0        0        0     6342 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_workflow_response_dto.py
+-rw-r--r--   0        0        0     6558 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_workflow_template_response_dto.py
+-rw-r--r--   0        0        0     5229 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/inline_response200.py
+-rw-r--r--   0        0        0     3129 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/inline_response200_info.py
+-rw-r--r--   0        0        0     5229 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/inline_response503.py
+-rw-r--r--   0        0        0    12256 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/intervention_definition.py
+-rw-r--r--   0        0        0     2419 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/json.py
+-rw-r--r--   0        0        0     2541 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/logical_operator.py
+-rw-r--r--   0        0        0    18333 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model.py
+-rw-r--r--   0        0        0    11239 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch.py
+-rw-r--r--   0        0        0    18191 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch_job.py
+-rw-r--r--   0        0        0    13259 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_joined_project_response_dto.py
+-rw-r--r--   0        0        0    10783 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_response_dto.py
+-rw-r--r--   0        0        0    15234 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch_job_response_dto.py
+-rw-r--r--   0        0        0    12271 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch_joined_project_response_dto.py
+-rw-r--r--   0        0        0     9890 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch_response_dto.py
+-rw-r--r--   0        0        0    10328 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_dataset.py
+-rw-r--r--   0        0        0    10092 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_endpoint.py
+-rw-r--r--   0        0        0    25050 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job.py
+-rw-r--r--   0        0        0     9956 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_config.py
+-rw-r--r--   0        0        0    12596 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_event.py
+-rw-r--r--   0        0        0    12880 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_cohort_response_dto.py
+-rw-r--r--   0        0        0    12719 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_data_query_response_dto.py
+-rw-r--r--   0        0        0    21859 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0    10146 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_feature_sub_category_response_dto.py
+-rw-r--r--   0        0        0    11429 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_job_output_response_dto.py
+-rw-r--r--   0        0        0    15143 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_job_status_response_dto.py
+-rw-r--r--   0        0        0    13077 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py
+-rw-r--r--   0        0        0    15368 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_response_dto.py
+-rw-r--r--   0        0        0    25459 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0    14899 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_response_dto.py
+-rw-r--r--   0        0        0    11903 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_intervention_definition_response_dto.py
+-rw-r--r--   0        0        0    14948 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_outcome_definition_response_dto.py
+-rw-r--r--   0        0        0    28497 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_response_dto.py
+-rw-r--r--   0        0        0    16370 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_response_dto.py
+-rw-r--r--   0        0        0    12177 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0    11585 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_output.py
+-rw-r--r--   0        0        0     9880 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_output_feature.py
+-rw-r--r--   0        0        0    22459 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_output_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0    13217 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_output_joined_model_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0    20838 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_output_joined_model_job_response_dto.py
+-rw-r--r--   0        0        0    12387 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_output_response_dto.py
+-rw-r--r--   0        0        0    26342 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_response_dto.py
+-rw-r--r--   0        0        0    14799 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_status.py
+-rw-r--r--   0        0        0    13217 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_status_joined_model_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0    20838 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_status_joined_model_job_response_dto.py
+-rw-r--r--   0        0        0    15027 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_status_response_dto.py
+-rw-r--r--   0        0        0    20198 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_cohort_joined_model_job_response_dto.py
+-rw-r--r--   0        0        0    13589 2023-06-14 19:39:44.904363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_cohort_response_dto.py
+-rw-r--r--   0        0        0    13496 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_model_job_joined_cohort_response_dto.py
+-rw-r--r--   0        0        0    22959 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_model_job_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0    10586 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_model_job_joined_feature_sub_category_response_dto.py
+-rw-r--r--   0        0        0    21985 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_model_job_response_dto.py
+-rw-r--r--   0        0        0    27656 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_model_output_details_response_dto.py
+-rw-r--r--   0        0        0    12021 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_project_response_dto.py
+-rw-r--r--   0        0        0    10587 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_user_favorite_response_dto.py
+-rw-r--r--   0        0        0    25995 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_output_details.py
+-rw-r--r--   0        0        0    30089 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_population.py
+-rw-r--r--   0        0        0    12461 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_joined_period_definition_response_dto.py
+-rw-r--r--   0        0        0    14542 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_response_dto.py
+-rw-r--r--   0        0        0    17056 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_cohort_results_response_dto.py
+-rw-r--r--   0        0        0    24059 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_data_query_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0    14017 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_data_query_response_dto.py
+-rw-r--r--   0        0        0    19133 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_feature_response_dto.py
+-rw-r--r--   0        0        0    11287 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_intervention_definition_response_dto.py
+-rw-r--r--   0        0        0    17798 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_model_job_joined_model_response_dto.py
+-rw-r--r--   0        0        0    20883 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_model_job_response_dto.py
+-rw-r--r--   0        0        0    14164 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_outcome_definition_response_dto.py
+-rw-r--r--   0        0        0    30731 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_response_dto.py
+-rw-r--r--   0        0        0    19577 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/model_response_dto.py
+-rw-r--r--   0        0        0     2427 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/object.py
+-rw-r--r--   0        0        0    23664 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/organization.py
+-rw-r--r--   0        0        0    11112 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/organization_feature_category_exclusion.py
+-rw-r--r--   0        0        0    11223 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/organization_feature_exclusion.py
+-rw-r--r--   0        0        0     9770 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/organization_response_dto.py
+-rw-r--r--   0        0        0    16743 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/organization_setting.py
+-rw-r--r--   0        0        0    16743 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/organization_setting_response_dto.py
+-rw-r--r--   0        0        0    14689 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/outcome_definition.py
+-rw-r--r--   0        0        0     5149 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/period_definition.py
+-rw-r--r--   0        0        0     2751 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/period_type.py
+-rw-r--r--   0        0        0     5332 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/person_set.py
+-rw-r--r--   0        0        0     3987 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/pipeline_config.py
+-rw-r--r--   0        0        0    15191 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/population.py
+-rw-r--r--   0        0        0    11771 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/population_store.py
+-rw-r--r--   0        0        0    10755 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/population_store_response_dto.py
+-rw-r--r--   0        0        0    12257 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process.py
+-rw-r--r--   0        0        0    16287 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_job.py
+-rw-r--r--   0        0        0     4858 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_config.py
+-rw-r--r--   0        0        0    12271 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0    10479 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_output.py
+-rw-r--r--   0        0        0    13415 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_output_joined_process_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0    15893 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_output_joined_process_job_response_dto.py
+-rw-r--r--   0        0        0    11016 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_output_response_dto.py
+-rw-r--r--   0        0        0    14331 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_response_dto.py
+-rw-r--r--   0        0        0    14764 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_status.py
+-rw-r--r--   0        0        0    12583 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_status_joined_project_response_dto.py
+-rw-r--r--   0        0        0    14902 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_status_response_dto.py
+-rw-r--r--   0        0        0    12115 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_joined_project_response_dto.py
+-rw-r--r--   0        0        0    11494 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_response_dto.py
+-rw-r--r--   0        0        0     2837 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/process_type.py
+-rw-r--r--   0        0        0    17760 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/project.py
+-rw-r--r--   0        0        0    13440 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/project_joined_model_joined_cohort_response_dto.py
+-rw-r--r--   0        0        0    17121 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/project_joined_model_response_dto.py
+-rw-r--r--   0        0        0    12125 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/project_joined_project_response_dto.py
+-rw-r--r--   0        0        0    10675 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/project_joined_user_favorite_response_dto.py
+-rw-r--r--   0        0        0    10979 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/project_member.py
+-rw-r--r--   0        0        0    12437 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/project_member_joined_project_response_dto.py
+-rw-r--r--   0        0        0    11641 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/project_member_response_dto.py
+-rw-r--r--   0        0        0    14895 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/project_response_dto.py
+-rw-r--r--   0        0        0    15487 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/scheduler.py
+-rw-r--r--   0        0        0    11402 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/scheduler_joined_workflow_response_dto.py
+-rw-r--r--   0        0        0    15605 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/scheduler_response_dto.py
+-rw-r--r--   0        0        0     5775 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/select_expression.py
+-rw-r--r--   0        0        0     2567 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/set_operator.py
+-rw-r--r--   0        0        0     5737 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/state_data.py
+-rw-r--r--   0        0        0    12800 2023-06-14 19:39:44.908363 curia-4.2.0b9/src/curia/api/swagger_client/models/task.py
+-rw-r--r--   0        0        0    16585 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution.py
+-rw-r--r--   0        0        0    13035 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_joined_task_response_dto.py
+-rw-r--r--   0        0        0    14390 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_joined_workflow_execution_response_dto.py
+-rw-r--r--   0        0        0    16918 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_response_dto.py
+-rw-r--r--   0        0        0    11220 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_status.py
+-rw-r--r--   0        0        0    15890 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py
+-rw-r--r--   0        0        0    18175 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_response_dto.py
+-rw-r--r--   0        0        0    11900 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_status_response_dto.py
+-rw-r--r--   0        0        0     2443 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/task_inputs.py
+-rw-r--r--   0        0        0     2447 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/task_outputs.py
+-rw-r--r--   0        0        0    11971 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/task_response_dto.py
+-rw-r--r--   0        0        0     5276 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_analysis_dto.py
+-rw-r--r--   0        0        0     8382 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_analysis_job_dto.py
+-rw-r--r--   0        0        0     4621 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_analysis_job_output_dto.py
+-rw-r--r--   0        0        0     8830 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_analysis_job_status_dto.py
+-rw-r--r--   0        0        0     6081 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_cohort_dto.py
+-rw-r--r--   0        0        0     6584 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_data_query_dto.py
+-rw-r--r--   0        0        0     4465 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_data_store_dto.py
+-rw-r--r--   0        0        0     5925 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_data_table_dto.py
+-rw-r--r--   0        0        0     5290 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_database_dto.py
+-rw-r--r--   0        0        0     5156 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_dataset_column_dto.py
+-rw-r--r--   0        0        0    14251 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_dataset_dto.py
+-rw-r--r--   0        0        0    11532 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_feature_dto.py
+-rw-r--r--   0        0        0     4513 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_feature_store_dto.py
+-rw-r--r--   0        0        0     3935 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_batch_dto.py
+-rw-r--r--   0        0        0     8867 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_batch_job_dto.py
+-rw-r--r--   0        0        0    10055 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_dto.py
+-rw-r--r--   0        0        0    12875 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_job_dto.py
+-rw-r--r--   0        0        0     5272 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_job_output_dto.py
+-rw-r--r--   0        0        0     8660 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_job_status_dto.py
+-rw-r--r--   0        0        0    17030 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_population_dto.py
+-rw-r--r--   0        0        0     4523 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_organization_dto.py
+-rw-r--r--   0        0        0    10276 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_organization_setting_dto.py
+-rw-r--r--   0        0        0     4561 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_population_store_dto.py
+-rw-r--r--   0        0        0     5545 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_process_dto.py
+-rw-r--r--   0        0        0     8239 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_process_job_dto.py
+-rw-r--r--   0        0        0     4585 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_process_job_output_dto.py
+-rw-r--r--   0        0        0     8770 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_process_job_status_dto.py
+-rw-r--r--   0        0        0     5420 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_project_dto.py
+-rw-r--r--   0        0        0     5396 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_project_member_dto.py
+-rw-r--r--   0        0        0     8433 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_scheduler_dto.py
+-rw-r--r--   0        0        0     5947 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_task_dto.py
+-rw-r--r--   0        0        0     9730 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_task_execution_dto.py
+-rw-r--r--   0        0        0     5385 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_task_execution_status_dto.py
+-rw-r--r--   0        0        0     7200 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_user_audit_trail_dto.py
+-rw-r--r--   0        0        0     9810 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_user_dto.py
+-rw-r--r--   0        0        0     4939 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_user_favorite_dto.py
+-rw-r--r--   0        0        0     4539 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_workflow_dto.py
+-rw-r--r--   0        0        0     6878 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_workflow_execution_dto.py
+-rw-r--r--   0        0        0     5005 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_workflow_execution_spec_dto.py
+-rw-r--r--   0        0        0     5465 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_workflow_execution_status_dto.py
+-rw-r--r--   0        0        0     5535 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/update_workflow_template_dto.py
+-rw-r--r--   0        0        0    10477 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/user_audit_trail.py
+-rw-r--r--   0        0        0    11559 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/user_audit_trail_response_dto.py
+-rw-r--r--   0        0        0    10871 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/user_favorite.py
+-rw-r--r--   0        0        0    12957 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/user_favorite_joined_model_joined_project_response_dto.py
+-rw-r--r--   0        0        0    17499 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/user_favorite_joined_model_response_dto.py
+-rw-r--r--   0        0        0    10837 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/user_favorite_response_dto.py
+-rw-r--r--   0        0        0    13040 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow.py
+-rw-r--r--   0        0        0    15472 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution.py
+-rw-r--r--   0        0        0    13250 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_response_dto.py
+-rw-r--r--   0        0        0    10872 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_spec.py
+-rw-r--r--   0        0        0    14870 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_spec_joined_workflow_execution_response_dto.py
+-rw-r--r--   0        0        0    11514 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_spec_response_dto.py
+-rw-r--r--   0        0        0    11440 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_status.py
+-rw-r--r--   0        0        0    14990 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_status_joined_workflow_execution_response_dto.py
+-rw-r--r--   0        0        0    12132 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_status_response_dto.py
+-rw-r--r--   0        0        0    15775 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_joined_scheduler_response_dto.py
+-rw-r--r--   0        0        0    14090 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_joined_workflow_execution_response_dto.py
+-rw-r--r--   0        0        0    12669 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_joined_workflow_template_response_dto.py
+-rw-r--r--   0        0        0    13141 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_response_dto.py
+-rw-r--r--   0        0        0    12837 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_template.py
+-rw-r--r--   0        0        0     5367 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_template_definition.py
+-rw-r--r--   0        0        0     2507 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_template_parameters.py
+-rw-r--r--   0        0        0    11941 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_template_response_dto.py
+-rw-r--r--   0        0        0     5655 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/models/zip_data.py
+-rw-r--r--   0        0        0    13208 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/swagger_client/rest.py
+-rw-r--r--   0        0        0        0 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/__init__.py
+-rw-r--r--   0        0        0     1091 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_aggregation_type.py
+-rw-r--r--   0        0        0     1102 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_all_of_cohort_model.py
+-rw-r--r--   0        0        0     1158 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_all_of_cohort_organization.py
+-rw-r--r--   0        0        0     1152 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_all_of_cohort_train_cohort.py
+-rw-r--r--   0        0        0     1158 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_all_of_data_table_dataset.py
+-rw-r--r--   0        0        0     1110 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_all_of_model_cohorts.py
+-rw-r--r--   0        0        0     1136 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_all_of_model_job_dataset.py
+-rw-r--r--   0        0        0     1168 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_all_of_model_job_environment.py
+-rw-r--r--   0        0        0     1120 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_all_of_model_job_model.py
+-rw-r--r--   0        0        0     1136 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_all_of_model_job_project.py
+-rw-r--r--   0        0        0     1128 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_all_of_model_model_jobs.py
+-rw-r--r--   0        0        0     1110 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_all_of_model_project.py
+-rw-r--r--   0        0        0     2252 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_analyses_api.py
+-rw-r--r--   0        0        0     1033 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_analysis.py
+-rw-r--r--   0        0        0     1059 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_analysis_job.py
+-rw-r--r--   0        0        0     1109 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test/test_analysis_job_config.py
+-rw-r--r--   0        0        0     1272 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1109 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_job_output.py
+-rw-r--r--   0        0        0     1464 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_job_output_joined_analysis_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1356 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_job_output_joined_analysis_job_response_dto.py
+-rw-r--r--   0        0        0     1214 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_job_output_response_dto.py
+-rw-r--r--   0        0        0     2675 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_job_outputs_api.py
+-rw-r--r--   0        0        0     1164 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_job_response_dto.py
+-rw-r--r--   0        0        0     1109 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_job_status.py
+-rw-r--r--   0        0        0     1322 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_job_status_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1214 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_job_status_response_dto.py
+-rw-r--r--   0        0        0     2680 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_job_statuses_api.py
+-rw-r--r--   0        0        0     1093 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_job_type.py
+-rw-r--r--   0        0        0     2749 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_jobs_api.py
+-rw-r--r--   0        0        0     1246 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1138 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_response_dto.py
+-rw-r--r--   0        0        0     1067 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_analysis_type.py
+-rw-r--r--   0        0        0     1217 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_any_of_arithmetic_expression_value.py
+-rw-r--r--   0        0        0     1193 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_any_of_boolean_expression_value.py
+-rw-r--r--   0        0        0     1367 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_any_of_cohort_definition_patient_metadata_filters_items.py
+-rw-r--r--   0        0        0     1127 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_any_of_condition_value.py
+-rw-r--r--   0        0        0     1131 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_arithmetic_expression.py
+-rw-r--r--   0        0        0     1115 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_arithmetic_operator.py
+-rw-r--r--   0        0        0     1000 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_body.py
+-rw-r--r--   0        0        0     1009 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_body1.py
+-rw-r--r--   0        0        0     1008 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_body2.py
+-rw-r--r--   0        0        0     1008 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_body3.py
+-rw-r--r--   0        0        0      978 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_body4.py
+-rw-r--r--   0        0        0      978 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_body5.py
+-rw-r--r--   0        0        0     1107 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_boolean_expression.py
+-rw-r--r--   0        0        0     1000 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_code.py
+-rw-r--r--   0        0        0     1016 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_cohort.py
+-rw-r--r--   0        0        0     1099 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_cohort_definition.py
+-rw-r--r--   0        0        0     1066 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_cohort_filter.py
+-rw-r--r--   0        0        0     1140 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_cohort_filter_condition.py
+-rw-r--r--   0        0        0     1222 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_cohort_joined_cohort_response_dto.py
+-rw-r--r--   0        0        0     1240 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_cohort_joined_model_job_response_dto.py
+-rw-r--r--   0        0        0     1122 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_cohort_response_dto.py
+-rw-r--r--   0        0        0     1075 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_cohort_results.py
+-rw-r--r--   0        0        0     1043 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_cohort_set.py
+-rw-r--r--   0        0        0     1066 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_cohort_window.py
+-rw-r--r--   0        0        0     2511 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_cohorts_api.py
+-rw-r--r--   0        0        0     1041 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_condition.py
+-rw-r--r--   0        0        0     1107 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_condition_operator.py
+-rw-r--r--   0        0        0     1090 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_container_config.py
+-rw-r--r--   0        0        0     1122 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_analysis_dto.py
+-rw-r--r--   0        0        0     1148 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_analysis_job_dto.py
+-rw-r--r--   0        0        0     1198 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_analysis_job_output_dto.py
+-rw-r--r--   0        0        0     1198 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_analysis_job_status_dto.py
+-rw-r--r--   0        0        0     1106 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_cohort_dto.py
+-rw-r--r--   0        0        0     1132 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_data_query_dto.py
+-rw-r--r--   0        0        0     1118 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_data_store_dto.py
+-rw-r--r--   0        0        0     1132 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_data_table_dto.py
+-rw-r--r--   0        0        0     1122 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_database_dto.py
+-rw-r--r--   0        0        0     1164 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_dataset_column_dto.py
+-rw-r--r--   0        0        0     1114 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_dataset_dto.py
+-rw-r--r--   0        0        0     1114 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_feature_dto.py
+-rw-r--r--   0        0        0     1142 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_feature_store_dto.py
+-rw-r--r--   0        0        0     1143 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_analysis_dto.py
+-rw-r--r--   0        0        0     1169 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_analysis_job_dto.py
+-rw-r--r--   0        0        0     1219 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_analysis_job_output_dto.py
+-rw-r--r--   0        0        0     1219 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_analysis_job_status_dto.py
+-rw-r--r--   0        0        0     1110 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_code_dto.py
+-rw-r--r--   0        0        0     1126 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_cohort_dto.py
+-rw-r--r--   0        0        0     1153 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_data_query_dto.py
+-rw-r--r--   0        0        0     1152 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_data_store_dto.py
+-rw-r--r--   0        0        0     1184 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_dataset_column_dto.py
+-rw-r--r--   0        0        0     1134 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_dataset_dto.py
+-rw-r--r--   0        0        0     1160 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_dataset_job_dto.py
+-rw-r--r--   0        0        0     1166 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_environment_dto.py
+-rw-r--r--   0        0        0     1200 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_feature_category_dto.py
+-rw-r--r--   0        0        0     1134 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_feature_dto.py
+-rw-r--r--   0        0        0     1176 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_feature_store_dto.py
+-rw-r--r--   0        0        0     1226 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_feature_sub_category_dto.py
+-rw-r--r--   0        0        0     1161 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_model_batch_dto.py
+-rw-r--r--   0        0        0     1187 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_model_batch_job_dto.py
+-rw-r--r--   0        0        0     1176 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_model_dataset_dto.py
+-rw-r--r--   0        0        0     1118 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_model_dto.py
+-rw-r--r--   0        0        0     1184 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_model_endpoint_dto.py
+-rw-r--r--   0        0        0     1144 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_model_job_dto.py
+-rw-r--r--   0        0        0     1194 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_model_job_output_dto.py
+-rw-r--r--   0        0        0     1253 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_model_job_output_feature_dto.py
+-rw-r--r--   0        0        0     1201 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_model_population_dto.py
+-rw-r--r--   0        0        0     1174 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_organization_dto.py
+-rw-r--r--   0        0        0     1306 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_organization_feature_exclusion_dto.py
+-rw-r--r--   0        0        0     1232 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_organization_setting_dto.py
+-rw-r--r--   0        0        0     1200 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_population_store_dto.py
+-rw-r--r--   0        0        0     1135 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_process_dto.py
+-rw-r--r--   0        0        0     1161 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_process_job_dto.py
+-rw-r--r--   0        0        0     1211 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_process_job_output_dto.py
+-rw-r--r--   0        0        0     1211 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_process_job_status_dto.py
+-rw-r--r--   0        0        0     1134 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_project_dto.py
+-rw-r--r--   0        0        0     1184 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_project_member_dto.py
+-rw-r--r--   0        0        0     1161 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_scheduler_dto.py
+-rw-r--r--   0        0        0     1121 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_task_dto.py
+-rw-r--r--   0        0        0     1195 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_task_execution_dto.py
+-rw-r--r--   0        0        0     1245 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_task_execution_status_dto.py
+-rw-r--r--   0        0        0     1176 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_user_favorite_dto.py
+-rw-r--r--   0        0        0     1153 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_workflow_dto.py
+-rw-r--r--   0        0        0     1227 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_workflow_execution_dto.py
+-rw-r--r--   0        0        0     1250 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_workflow_execution_spec_dto.py
+-rw-r--r--   0        0        0     1219 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_many_workflow_template_dto.py
+-rw-r--r--   0        0        0     1140 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_model_batch_dto.py
+-rw-r--r--   0        0        0     1166 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_model_batch_job_dto.py
+-rw-r--r--   0        0        0     1098 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_model_dto.py
+-rw-r--r--   0        0        0     1124 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_model_job_dto.py
+-rw-r--r--   0        0        0     1174 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_model_job_output_dto.py
+-rw-r--r--   0        0        0     1174 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_model_job_status_dto.py
+-rw-r--r--   0        0        0     1180 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_model_population_dto.py
+-rw-r--r--   0        0        0     1154 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_organization_dto.py
+-rw-r--r--   0        0        0     1212 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_organization_setting_dto.py
+-rw-r--r--   0        0        0     1166 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_population_store_dto.py
+-rw-r--r--   0        0        0     1114 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_process_dto.py
+-rw-r--r--   0        0        0     1140 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_process_job_dto.py
+-rw-r--r--   0        0        0     1190 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_process_job_output_dto.py
+-rw-r--r--   0        0        0     1190 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_process_job_status_dto.py
+-rw-r--r--   0        0        0     1114 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_project_dto.py
+-rw-r--r--   0        0        0     1164 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_project_member_dto.py
+-rw-r--r--   0        0        0     1130 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_scheduler_dto.py
+-rw-r--r--   0        0        0     1090 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_task_dto.py
+-rw-r--r--   0        0        0     1164 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_task_execution_dto.py
+-rw-r--r--   0        0        0     1214 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_task_execution_status_dto.py
+-rw-r--r--   0        0        0     1174 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_user_audit_trail_dto.py
+-rw-r--r--   0        0        0     1156 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_user_favorite_dto.py
+-rw-r--r--   0        0        0     1122 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_workflow_dto.py
+-rw-r--r--   0        0        0     1196 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_workflow_execution_dto.py
+-rw-r--r--   0        0        0     1216 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_workflow_execution_spec_dto.py
+-rw-r--r--   0        0        0     1246 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_workflow_execution_status_dto.py
+-rw-r--r--   0        0        0     1188 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_create_workflow_template_dto.py
+-rw-r--r--   0        0        0     2504 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_data_queries_api.py
+-rw-r--r--   0        0        0     1043 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_data_query.py
+-rw-r--r--   0        0        0     1256 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_data_query_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0     1148 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_data_query_response_dto.py
+-rw-r--r--   0        0        0     1042 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_data_store.py
+-rw-r--r--   0        0        0     1134 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_data_store_response_dto.py
+-rw-r--r--   0        0        0     2360 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_data_stores_api.py
+-rw-r--r--   0        0        0     1043 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_data_table.py
+-rw-r--r--   0        0        0     1264 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_data_table_joined_database_response_dto.py
+-rw-r--r--   0        0        0     1256 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_data_table_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0     1148 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_data_table_response_dto.py
+-rw-r--r--   0        0        0     1255 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_data_tables_api.py
+-rw-r--r--   0        0        0     1033 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_database.py
+-rw-r--r--   0        0        0     1264 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_database_joined_data_table_response_dto.py
+-rw-r--r--   0        0        0     1138 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_database_response_dto.py
+-rw-r--r--   0        0        0     1588 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_databases_api.py
+-rw-r--r--   0        0        0     1024 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_dataset.py
+-rw-r--r--   0        0        0     1074 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_dataset_column.py
+-rw-r--r--   0        0        0     1288 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_dataset_column_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0     1180 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_dataset_column_response_dto.py
+-rw-r--r--   0        0        0     2486 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_dataset_columns_api.py
+-rw-r--r--   0        0        0     1050 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_dataset_job.py
+-rw-r--r--   0        0        0     1100 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_dataset_job_status.py
+-rw-r--r--   0        0        0     1256 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_dataset_joined_data_query_response_dto.py
+-rw-r--r--   0        0        0     1288 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_dataset_joined_dataset_column_response_dto.py
+-rw-r--r--   0        0        0     1130 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_dataset_response_dto.py
+-rw-r--r--   0        0        0     3799 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_datasets_api.py
+-rw-r--r--   0        0        0     1226 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_datasetsuploadlargecomplete_parts.py
+-rw-r--r--   0        0        0     1056 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_environment.py
+-rw-r--r--   0        0        0     1122 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_environment_activity.py
+-rw-r--r--   0        0        0     1024 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_feature.py
+-rw-r--r--   0        0        0     1090 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_feature_category.py
+-rw-r--r--   0        0        0     1504 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_feature_joined_feature_sub_category_joined_feature_category_response_dto.py
+-rw-r--r--   0        0        0     1330 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_feature_joined_feature_sub_category_response_dto.py
+-rw-r--r--   0        0        0     1304 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_feature_joined_model_population_response_dto.py
+-rw-r--r--   0        0        0     1410 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_feature_joined_organization_feature_exclusion_response_dto.py
+-rw-r--r--   0        0        0     1130 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_feature_response_dto.py
+-rw-r--r--   0        0        0     1066 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_feature_store.py
+-rw-r--r--   0        0        0     1158 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_feature_store_response_dto.py
+-rw-r--r--   0        0        0     2480 2023-06-14 19:39:44.916363 curia-4.2.0b9/src/curia/api/test/test_feature_stores_api.py
+-rw-r--r--   0        0        0     1116 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_feature_sub_category.py
+-rw-r--r--   0        0        0     1066 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_feature_table.py
+-rw-r--r--   0        0        0     2217 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_features_api.py
+-rw-r--r--   0        0        0     1098 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_geographic_counts.py
+-rw-r--r--   0        0        0     1106 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_geographic_queries.py
+-rw-r--r--   0        0        0     1261 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_analysis_job_output_response_dto.py
+-rw-r--r--   0        0        0     1211 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_analysis_job_response_dto.py
+-rw-r--r--   0        0        0     1261 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_analysis_job_status_response_dto.py
+-rw-r--r--   0        0        0     1185 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_analysis_response_dto.py
+-rw-r--r--   0        0        0     1152 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_code_response_dto.py
+-rw-r--r--   0        0        0     1168 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_cohort_response_dto.py
+-rw-r--r--   0        0        0     1195 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_data_query_response_dto.py
+-rw-r--r--   0        0        0     1194 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_data_store_response_dto.py
+-rw-r--r--   0        0        0     1195 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_data_table_response_dto.py
+-rw-r--r--   0        0        0     1185 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_database_response_dto.py
+-rw-r--r--   0        0        0     1226 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_dataset_column_response_dto.py
+-rw-r--r--   0        0        0     1202 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_dataset_job_response_dto.py
+-rw-r--r--   0        0        0     1252 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_dataset_job_status_response_dto.py
+-rw-r--r--   0        0        0     1176 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_dataset_response_dto.py
+-rw-r--r--   0        0        0     1208 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_environment_response_dto.py
+-rw-r--r--   0        0        0     1242 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_feature_category_response_dto.py
+-rw-r--r--   0        0        0     1176 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_feature_response_dto.py
+-rw-r--r--   0        0        0     1218 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_feature_store_response_dto.py
+-rw-r--r--   0        0        0     1268 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_feature_sub_category_response_dto.py
+-rw-r--r--   0        0        0     1229 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_model_batch_job_response_dto.py
+-rw-r--r--   0        0        0     1203 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_model_batch_response_dto.py
+-rw-r--r--   0        0        0     1218 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_model_dataset_response_dto.py
+-rw-r--r--   0        0        0     1226 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_model_endpoint_response_dto.py
+-rw-r--r--   0        0        0     1228 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_model_job_event_response_dto.py
+-rw-r--r--   0        0        0     1295 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_model_job_output_feature_response_dto.py
+-rw-r--r--   0        0        0     1236 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_model_job_output_response_dto.py
+-rw-r--r--   0        0        0     1186 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_model_job_response_dto.py
+-rw-r--r--   0        0        0     1236 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_model_job_status_response_dto.py
+-rw-r--r--   0        0        0     1243 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_model_population_response_dto.py
+-rw-r--r--   0        0        0     1160 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_model_response_dto.py
+-rw-r--r--   0        0        0     1348 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_organization_feature_exclusion_response_dto.py
+-rw-r--r--   0        0        0     1216 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_organization_response_dto.py
+-rw-r--r--   0        0        0     1274 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_organization_setting_response_dto.py
+-rw-r--r--   0        0        0     1242 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_population_store_response_dto.py
+-rw-r--r--   0        0        0     1253 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_process_job_output_response_dto.py
+-rw-r--r--   0        0        0     1203 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_process_job_response_dto.py
+-rw-r--r--   0        0        0     1253 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_process_job_status_response_dto.py
+-rw-r--r--   0        0        0     1177 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_process_response_dto.py
+-rw-r--r--   0        0        0     1226 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_project_member_response_dto.py
+-rw-r--r--   0        0        0     1176 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_project_response_dto.py
+-rw-r--r--   0        0        0     1203 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_scheduler_response_dto.py
+-rw-r--r--   0        0        0     1237 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_task_execution_response_dto.py
+-rw-r--r--   0        0        0     1287 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_task_execution_status_response_dto.py
+-rw-r--r--   0        0        0     1163 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_task_response_dto.py
+-rw-r--r--   0        0        0     1237 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_user_audit_trail_response_dto.py
+-rw-r--r--   0        0        0     1218 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_user_favorite_response_dto.py
+-rw-r--r--   0        0        0     1269 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_workflow_execution_response_dto.py
+-rw-r--r--   0        0        0     1292 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_workflow_execution_spec_response_dto.py
+-rw-r--r--   0        0        0     1319 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_workflow_execution_status_response_dto.py
+-rw-r--r--   0        0        0     1195 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_workflow_response_dto.py
+-rw-r--r--   0        0        0     1261 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_get_many_workflow_template_response_dto.py
+-rw-r--r--   0        0        0     1107 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_inline_response200.py
+-rw-r--r--   0        0        0     1141 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_inline_response200_info.py
+-rw-r--r--   0        0        0     1107 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_inline_response503.py
+-rw-r--r--   0        0        0     7598 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_internal_api.py
+-rw-r--r--   0        0        0     1147 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_intervention_definition.py
+-rw-r--r--   0        0        0     1001 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_json.py
+-rw-r--r--   0        0        0     1091 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_logical_operator.py
+-rw-r--r--   0        0        0     1008 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model.py
+-rw-r--r--   0        0        0     1051 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_batch.py
+-rw-r--r--   0        0        0     1077 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_batch_job.py
+-rw-r--r--   0        0        0     1424 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_batch_job_joined_model_batch_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1316 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_batch_job_joined_model_batch_response_dto.py
+-rw-r--r--   0        0        0     1182 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_batch_job_response_dto.py
+-rw-r--r--   0        0        0     3070 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_batch_jobs_api.py
+-rw-r--r--   0        0        0     1264 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_batch_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1156 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_batch_response_dto.py
+-rw-r--r--   0        0        0     2371 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_batches_api.py
+-rw-r--r--   0        0        0     1066 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_dataset.py
+-rw-r--r--   0        0        0     1074 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_endpoint.py
+-rw-r--r--   0        0        0     1034 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job.py
+-rw-r--r--   0        0        0     1084 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_config.py
+-rw-r--r--   0        0        0     1076 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_event.py
+-rw-r--r--   0        0        0     1240 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_cohort_response_dto.py
+-rw-r--r--   0        0        0     1252 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_data_query_response_dto.py
+-rw-r--r--   0        0        0     1248 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0     1340 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_feature_sub_category_response_dto.py
+-rw-r--r--   0        0        0     1308 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_job_output_response_dto.py
+-rw-r--r--   0        0        0     1308 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_job_status_response_dto.py
+-rw-r--r--   0        0        0     1678 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py
+-rw-r--r--   0        0        0     1496 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_response_dto.py
+-rw-r--r--   0        0        0     1548 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0     1440 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_response_dto.py
+-rw-r--r--   0        0        0     1544 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_joined_intervention_definition_response_dto.py
+-rw-r--r--   0        0        0     1504 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_joined_outcome_definition_response_dto.py
+-rw-r--r--   0        0        0     1314 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_response_dto.py
+-rw-r--r--   0        0        0     1232 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_response_dto.py
+-rw-r--r--   0        0        0     1248 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1084 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_output.py
+-rw-r--r--   0        0        0     1142 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_output_feature.py
+-rw-r--r--   0        0        0     1298 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_output_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0     1416 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_output_joined_model_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1308 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_output_joined_model_job_response_dto.py
+-rw-r--r--   0        0        0     1190 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_output_response_dto.py
+-rw-r--r--   0        0        0     2555 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_outputs_api.py
+-rw-r--r--   0        0        0     1140 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_response_dto.py
+-rw-r--r--   0        0        0     1084 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_status.py
+-rw-r--r--   0        0        0     1416 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_status_joined_model_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1308 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_status_joined_model_job_response_dto.py
+-rw-r--r--   0        0        0     1190 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_status_response_dto.py
+-rw-r--r--   0        0        0     1586 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_job_statuses_api.py
+-rw-r--r--   0        0        0     2820 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_jobs_api.py
+-rw-r--r--   0        0        0     1332 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_joined_cohort_joined_model_job_response_dto.py
+-rw-r--r--   0        0        0     1214 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_joined_cohort_response_dto.py
+-rw-r--r--   0        0        0     1332 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_joined_model_job_joined_cohort_response_dto.py
+-rw-r--r--   0        0        0     1340 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_joined_model_job_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0     1432 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_joined_model_job_joined_feature_sub_category_response_dto.py
+-rw-r--r--   0        0        0     1232 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_joined_model_job_response_dto.py
+-rw-r--r--   0        0        0     1300 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_joined_model_output_details_response_dto.py
+-rw-r--r--   0        0        0     1222 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1264 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_joined_user_favorite_response_dto.py
+-rw-r--r--   0        0        0     1116 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_output_details.py
+-rw-r--r--   0        0        0     1091 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_population.py
+-rw-r--r--   0        0        0     1560 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_population_joined_cohort_definition_joined_period_definition_response_dto.py
+-rw-r--r--   0        0        0     1378 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_population_joined_cohort_definition_response_dto.py
+-rw-r--r--   0        0        0     1354 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_population_joined_cohort_results_response_dto.py
+-rw-r--r--   0        0        0     1430 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_population_joined_data_query_joined_dataset_response_dto.py
+-rw-r--r--   0        0        0     1322 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_population_joined_data_query_response_dto.py
+-rw-r--r--   0        0        0     1304 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_population_joined_feature_response_dto.py
+-rw-r--r--   0        0        0     1426 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_population_joined_intervention_definition_response_dto.py
+-rw-r--r--   0        0        0     1406 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_population_joined_model_job_joined_model_response_dto.py
+-rw-r--r--   0        0        0     1314 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_population_joined_model_job_response_dto.py
+-rw-r--r--   0        0        0     1386 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_population_joined_outcome_definition_response_dto.py
+-rw-r--r--   0        0        0     1196 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_population_response_dto.py
+-rw-r--r--   0        0        0     2769 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_populations_api.py
+-rw-r--r--   0        0        0     1114 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_model_response_dto.py
+-rw-r--r--   0        0        0     2895 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_models_api.py
+-rw-r--r--   0        0        0     1016 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_object.py
+-rw-r--r--   0        0        0     1064 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_organization.py
+-rw-r--r--   0        0        0     1276 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_organization_feature_category_exclusion.py
+-rw-r--r--   0        0        0     1196 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_organization_feature_exclusion.py
+-rw-r--r--   0        0        0     1170 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_organization_response_dto.py
+-rw-r--r--   0        0        0     1122 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_organization_setting.py
+-rw-r--r--   0        0        0     1228 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_organization_setting_response_dto.py
+-rw-r--r--   0        0        0     3201 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_organization_settings_api.py
+-rw-r--r--   0        0        0     2431 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_organizations_api.py
+-rw-r--r--   0        0        0     1107 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_outcome_definition.py
+-rw-r--r--   0        0        0     1098 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_period_definition.py
+-rw-r--r--   0        0        0     1051 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_period_type.py
+-rw-r--r--   0        0        0     1043 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_person_set.py
+-rw-r--r--   0        0        0     1082 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_pipeline_config.py
+-rw-r--r--   0        0        0    26607 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_platform_api.py
+-rw-r--r--   0        0        0     1048 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_population.py
+-rw-r--r--   0        0        0     1090 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_population_store.py
+-rw-r--r--   0        0        0     1182 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_population_store_response_dto.py
+-rw-r--r--   0        0        0     2600 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_population_stores_api.py
+-rw-r--r--   0        0        0     1025 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_process.py
+-rw-r--r--   0        0        0     1051 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_process_job.py
+-rw-r--r--   0        0        0     1114 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_process_job_config.py
+-rw-r--r--   0        0        0     1264 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_process_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1101 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_process_job_output.py
+-rw-r--r--   0        0        0     1448 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_process_job_output_joined_process_job_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1340 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_process_job_output_joined_process_job_response_dto.py
+-rw-r--r--   0        0        0     1206 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_process_job_output_response_dto.py
+-rw-r--r--   0        0        0     2635 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_process_job_outputs_api.py
+-rw-r--r--   0        0        0     1156 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_process_job_response_dto.py
+-rw-r--r--   0        0        0     1101 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_process_job_status.py
+-rw-r--r--   0        0        0     1314 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_process_job_status_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1206 2023-06-14 19:39:44.920363 curia-4.2.0b9/src/curia/api/test/test_process_job_status_response_dto.py
+-rw-r--r--   0        0        0     2640 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_process_job_statuses_api.py
+-rw-r--r--   0        0        0     2703 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_process_jobs_api.py
+-rw-r--r--   0        0        0     1238 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_process_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1130 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_process_response_dto.py
+-rw-r--r--   0        0        0     1059 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_process_type.py
+-rw-r--r--   0        0        0     2222 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_processes_api.py
+-rw-r--r--   0        0        0     1024 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_project.py
+-rw-r--r--   0        0        0     1322 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_project_joined_model_joined_cohort_response_dto.py
+-rw-r--r--   0        0        0     1222 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_project_joined_model_response_dto.py
+-rw-r--r--   0        0        0     1238 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_project_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1280 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_project_joined_user_favorite_response_dto.py
+-rw-r--r--   0        0        0     1074 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_project_member.py
+-rw-r--r--   0        0        0     1288 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_project_member_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1180 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_project_member_response_dto.py
+-rw-r--r--   0        0        0     2486 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_project_members_api.py
+-rw-r--r--   0        0        0     1130 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_project_response_dto.py
+-rw-r--r--   0        0        0     2858 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_projects_api.py
+-rw-r--r--   0        0        0     1051 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_scheduler.py
+-rw-r--r--   0        0        0     2340 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_scheduler_api.py
+-rw-r--r--   0        0        0     1248 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_scheduler_joined_workflow_response_dto.py
+-rw-r--r--   0        0        0     1146 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_scheduler_response_dto.py
+-rw-r--r--   0        0        0     1099 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_select_expression.py
+-rw-r--r--   0        0        0     1059 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_set_operator.py
+-rw-r--r--   0        0        0     1056 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_state_data.py
+-rw-r--r--   0        0        0     1011 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_task.py
+-rw-r--r--   0        0        0     1085 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_task_execution.py
+-rw-r--r--   0        0        0     1250 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_task_execution_joined_task_response_dto.py
+-rw-r--r--   0        0        0     1356 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_task_execution_joined_workflow_execution_response_dto.py
+-rw-r--r--   0        0        0     1180 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_task_execution_response_dto.py
+-rw-r--r--   0        0        0     1135 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_task_execution_status.py
+-rw-r--r--   0        0        0     1564 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py
+-rw-r--r--   0        0        0     1374 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_task_execution_status_joined_task_execution_response_dto.py
+-rw-r--r--   0        0        0     1230 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_task_execution_status_response_dto.py
+-rw-r--r--   0        0        0     1061 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_task_inputs.py
+-rw-r--r--   0        0        0     1069 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_task_outputs.py
+-rw-r--r--   0        0        0     1106 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_task_response_dto.py
+-rw-r--r--   0        0        0     2687 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_tasks_api.py
+-rw-r--r--   0        0        0     1122 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_analysis_dto.py
+-rw-r--r--   0        0        0     1148 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_analysis_job_dto.py
+-rw-r--r--   0        0        0     1198 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_analysis_job_output_dto.py
+-rw-r--r--   0        0        0     1198 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_analysis_job_status_dto.py
+-rw-r--r--   0        0        0     1106 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_cohort_dto.py
+-rw-r--r--   0        0        0     1132 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_data_query_dto.py
+-rw-r--r--   0        0        0     1118 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_data_store_dto.py
+-rw-r--r--   0        0        0     1132 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_data_table_dto.py
+-rw-r--r--   0        0        0     1122 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_database_dto.py
+-rw-r--r--   0        0        0     1164 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_dataset_column_dto.py
+-rw-r--r--   0        0        0     1114 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_dataset_dto.py
+-rw-r--r--   0        0        0     1114 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_feature_dto.py
+-rw-r--r--   0        0        0     1142 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_feature_store_dto.py
+-rw-r--r--   0        0        0     1140 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_model_batch_dto.py
+-rw-r--r--   0        0        0     1166 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_model_batch_job_dto.py
+-rw-r--r--   0        0        0     1098 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_model_dto.py
+-rw-r--r--   0        0        0     1124 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_model_job_dto.py
+-rw-r--r--   0        0        0     1174 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_model_job_output_dto.py
+-rw-r--r--   0        0        0     1174 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_model_job_status_dto.py
+-rw-r--r--   0        0        0     1180 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_model_population_dto.py
+-rw-r--r--   0        0        0     1154 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_organization_dto.py
+-rw-r--r--   0        0        0     1212 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_organization_setting_dto.py
+-rw-r--r--   0        0        0     1166 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_population_store_dto.py
+-rw-r--r--   0        0        0     1114 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_process_dto.py
+-rw-r--r--   0        0        0     1140 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_process_job_dto.py
+-rw-r--r--   0        0        0     1190 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_process_job_output_dto.py
+-rw-r--r--   0        0        0     1190 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_process_job_status_dto.py
+-rw-r--r--   0        0        0     1114 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_project_dto.py
+-rw-r--r--   0        0        0     1164 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_project_member_dto.py
+-rw-r--r--   0        0        0     1130 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_scheduler_dto.py
+-rw-r--r--   0        0        0     1090 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_task_dto.py
+-rw-r--r--   0        0        0     1164 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_task_execution_dto.py
+-rw-r--r--   0        0        0     1214 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_task_execution_status_dto.py
+-rw-r--r--   0        0        0     1174 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_user_audit_trail_dto.py
+-rw-r--r--   0        0        0     1076 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_user_dto.py
+-rw-r--r--   0        0        0     1156 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_user_favorite_dto.py
+-rw-r--r--   0        0        0     1122 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_workflow_dto.py
+-rw-r--r--   0        0        0     1196 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_workflow_execution_dto.py
+-rw-r--r--   0        0        0     1216 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_workflow_execution_spec_dto.py
+-rw-r--r--   0        0        0     1246 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_workflow_execution_status_dto.py
+-rw-r--r--   0        0        0     1188 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_update_workflow_template_dto.py
+-rw-r--r--   0        0        0     1085 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_user_audit_trail.py
+-rw-r--r--   0        0        0     1334 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_user_audit_trail_api.py
+-rw-r--r--   0        0        0     1190 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_user_audit_trail_response_dto.py
+-rw-r--r--   0        0        0     1066 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_user_favorite.py
+-rw-r--r--   0        0        0     1372 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_user_favorite_joined_model_joined_project_response_dto.py
+-rw-r--r--   0        0        0     1264 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_user_favorite_joined_model_response_dto.py
+-rw-r--r--   0        0        0     1172 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_user_favorite_response_dto.py
+-rw-r--r--   0        0        0     2446 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_user_favorites_api.py
+-rw-r--r--   0        0        0     4472 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_user_management_api.py
+-rw-r--r--   0        0        0     1043 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow.py
+-rw-r--r--   0        0        0     1117 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_execution.py
+-rw-r--r--   0        0        0     1212 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_execution_response_dto.py
+-rw-r--r--   0        0        0     1140 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_execution_spec.py
+-rw-r--r--   0        0        0     1422 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_execution_spec_joined_workflow_execution_response_dto.py
+-rw-r--r--   0        0        0     1232 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_execution_spec_response_dto.py
+-rw-r--r--   0        0        0     1167 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_execution_status.py
+-rw-r--r--   0        0        0     1438 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_execution_status_joined_workflow_execution_response_dto.py
+-rw-r--r--   0        0        0     1262 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_execution_status_response_dto.py
+-rw-r--r--   0        0        0     1262 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_joined_scheduler_response_dto.py
+-rw-r--r--   0        0        0     1328 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_joined_workflow_execution_response_dto.py
+-rw-r--r--   0        0        0     1320 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_joined_workflow_template_response_dto.py
+-rw-r--r--   0        0        0     1138 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_response_dto.py
+-rw-r--r--   0        0        0     1109 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_template.py
+-rw-r--r--   0        0        0     1191 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_template_definition.py
+-rw-r--r--   0        0        0     1180 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_template_parameters.py
+-rw-r--r--   0        0        0     1204 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflow_template_response_dto.py
+-rw-r--r--   0        0        0     2575 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_workflows_api.py
+-rw-r--r--   0        0        0     1040 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/test/test_zip_data.py
+-rw-r--r--   0        0        0       69 2023-06-14 19:39:44.912363 curia-4.2.0b9/src/curia/api/test-requirements.txt
+-rw-r--r--   0        0        0      143 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/api/tox.ini
+-rw-r--r--   0        0        0        0 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/mock/__init__.py
+-rw-r--r--   0        0        0    22897 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/mock/api.py
+-rw-r--r--   0        0        0    17122 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/mock/api_server.py
+-rw-r--r--   0        0        0     4287 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/mock/moto.py
+-rw-r--r--   0        0        0     1565 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/mock/s3.py
+-rw-r--r--   0        0        0    14281 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/mock/server.py
+-rw-r--r--   0        0        0      284 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/mock/session.py
+-rw-r--r--   0        0        0      992 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/session.py
+-rw-r--r--   0        0        0        0 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/utils/__init__.py
+-rw-r--r--   0        0        0     1276 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/utils/dataset.py
+-rw-r--r--   0        0        0     3727 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/utils/job.py
+-rw-r--r--   0        0        0     1125 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/utils/python.py
+-rw-r--r--   0        0        0     7824 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/utils/s3.py
+-rw-r--r--   0        0        0     1165 2023-06-14 19:39:44.924363 curia-4.2.0b9/src/curia/utils/string.py
+-rw-r--r--   0        0        0     7529 1970-01-01 00:00:00.000000 curia-4.2.0b9/PKG-INFO
```

### Comparing `curia-4.2.0b8/README.md` & `curia-4.2.0b9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![PyPI version](https://badge.fury.io/py/curia.svg)](https://badge.fury.io/py/curia)
 
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
-[![Python 3.11](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3110/)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)
 
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Curia-ai_curia-python-sdk&metric=alert_status&token=e6d33fff8f3c9375c06d3b3deba711b1891c0b0b)](https://sonarcloud.io/dashboard?id=Curia-ai_curia-python-sdk)
 [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=Curia-ai_curia-python-sdk&metric=bugs&token=e6d33fff8f3c9375c06d3b3deba711b1891c0b0b)](https://sonarcloud.io/dashboard?id=Curia-ai_curia-python-sdk)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=Curia-ai_curia-python-sdk&metric=coverage&token=e6d33fff8f3c9375c06d3b3deba711b1891c0b0b)](https://sonarcloud.io/dashboard?id=Curia-ai_curia-python-sdk)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=Curia-ai_curia-python-sdk&metric=sqale_rating&token=e6d33fff8f3c9375c06d3b3deba711b1891c0b0b)](https://sonarcloud.io/dashboard?id=Curia-ai_curia-python-sdk)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=Curia-ai_curia-python-sdk&metric=reliability_rating&token=e6d33fff8f3c9375c06d3b3deba711b1891c0b0b)](https://sonarcloud.io/dashboard?id=Curia-ai_curia-python-sdk)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=Curia-ai_curia-python-sdk&metric=security_rating&token=e6d33fff8f3c9375c06d3b3deba711b1891c0b0b)](https://sonarcloud.io/dashboard?id=Curia-ai_curia-python-sdk)
```

### Comparing `curia-4.2.0b8/pyproject.toml` & `curia-4.2.0b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "curia"
-version = "4.2.0-beta.8"
+version = "4.2.0-beta.9"
 description = "A library for interfacing with the Curia API."
 authors = ["Aledade, Inc."]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-boto3 = "^1.26.150"
+boto3 = "^1.26.0"
 certifi = ">= 14.05.14"
 six = ">= 1.10"
 python-dateutil = ">= 2.5.3"
 urllib3 = ">= 1.15.1"
 pyarrow = "^12.0.0"
 pymaybe = "^0.1.6"
 requests = "^2.31.0"
```

### Comparing `curia-4.2.0b8/src/curia/api/.gitignore` & `curia-4.2.0b9/src/curia/api/.gitignore`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/.swagger-codegen-ignore` & `curia-4.2.0b9/src/curia/api/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/README.md` & `curia-4.2.0b9/src/curia/api/README.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysesApi.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysesApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Analysis.md` & `curia-4.2.0b9/src/curia/api/docs/Analysis.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJob.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJob.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJobJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJobJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJobOutput.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJobOutput.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJobOutputJoinedAnalysisJobJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJobOutputJoinedAnalysisJobJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJobOutputJoinedAnalysisJobResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJobOutputJoinedAnalysisJobResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJobOutputResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJobOutputResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJobOutputsApi.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJobOutputsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJobResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJobResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJobStatus.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJobStatus.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJobStatusJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJobStatusJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJobStatusResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJobStatusResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJobStatusesApi.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJobStatusesApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJobsApi.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJobsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/AnalysisResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/AnalysisResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/BooleanExpression.md` & `curia-4.2.0b9/src/curia/api/docs/BooleanExpression.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Code.md` & `curia-4.2.0b9/src/curia/api/docs/Code.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Cohort.md` & `curia-4.2.0b9/src/curia/api/docs/Cohort.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CohortDefinition.md` & `curia-4.2.0b9/src/curia/api/docs/CohortDefinition.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CohortFilter.md` & `curia-4.2.0b9/src/curia/api/docs/CohortFilter.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CohortJoinedCohortResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/CohortJoinedCohortResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CohortJoinedModelJobResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/CohortJoinedModelJobResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CohortResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/CohortResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CohortResults.md` & `curia-4.2.0b9/src/curia/api/docs/CohortResults.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CohortSet.md` & `curia-4.2.0b9/src/curia/api/docs/CohortSet.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CohortWindow.md` & `curia-4.2.0b9/src/curia/api/docs/CohortWindow.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CohortsApi.md` & `curia-4.2.0b9/src/curia/api/docs/CohortsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ContainerConfig.md` & `curia-4.2.0b9/src/curia/api/docs/ContainerConfig.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateAnalysisJobDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateAnalysisJobDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateAnalysisJobStatusDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateAnalysisJobStatusDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateCohortDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateCohortDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateDataQueryDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateDataQueryDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateDatasetDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateDatasetDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateFeatureDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateFeatureDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateModelBatchJobDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateModelBatchJobDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateModelDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateModelDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateModelJobDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateModelJobDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateModelJobStatusDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateModelJobStatusDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateModelPopulationDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateModelPopulationDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateOrganizationSettingDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateOrganizationSettingDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateProcessJobDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateProcessJobDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateProcessJobStatusDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateProcessJobStatusDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateSchedulerDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateSchedulerDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateTaskExecutionDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateTaskExecutionDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateWorkflowExecutionDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateWorkflowExecutionDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateWorkflowExecutionSpecDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateWorkflowExecutionSpecDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/CreateWorkflowTemplateDto.md` & `curia-4.2.0b9/src/curia/api/docs/CreateWorkflowTemplateDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DataQueriesApi.md` & `curia-4.2.0b9/src/curia/api/docs/DataQueriesApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DataQuery.md` & `curia-4.2.0b9/src/curia/api/docs/DataQuery.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DataQueryJoinedDatasetResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/DataQueryJoinedDatasetResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DataQueryResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/DataQueryResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DataStore.md` & `curia-4.2.0b9/src/curia/api/docs/DataStore.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DataStoreResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/DataStoreResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DataStoresApi.md` & `curia-4.2.0b9/src/curia/api/docs/DataStoresApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DataTable.md` & `curia-4.2.0b9/src/curia/api/docs/DataTable.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DataTableJoinedDatabaseResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/DataTableJoinedDatabaseResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DataTableJoinedDatasetResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/DataTableJoinedDatasetResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DataTableResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/DataTableResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DataTablesApi.md` & `curia-4.2.0b9/src/curia/api/docs/DataTablesApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Database.md` & `curia-4.2.0b9/src/curia/api/docs/Database.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DatabaseJoinedDataTableResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/DatabaseJoinedDataTableResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DatabaseResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/DatabaseResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DatabasesApi.md` & `curia-4.2.0b9/src/curia/api/docs/DatabasesApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Dataset.md` & `curia-4.2.0b9/src/curia/api/docs/Dataset.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DatasetColumn.md` & `curia-4.2.0b9/src/curia/api/docs/DatasetColumn.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DatasetColumnJoinedDatasetResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/DatasetColumnJoinedDatasetResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DatasetColumnResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/DatasetColumnResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DatasetColumnsApi.md` & `curia-4.2.0b9/src/curia/api/docs/DatasetColumnsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DatasetJob.md` & `curia-4.2.0b9/src/curia/api/docs/DatasetJob.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DatasetJobStatus.md` & `curia-4.2.0b9/src/curia/api/docs/DatasetJobStatus.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DatasetJoinedDataQueryResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/DatasetJoinedDataQueryResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DatasetJoinedDatasetColumnResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/DatasetJoinedDatasetColumnResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DatasetResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/DatasetResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/DatasetsApi.md` & `curia-4.2.0b9/src/curia/api/docs/DatasetsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Environment.md` & `curia-4.2.0b9/src/curia/api/docs/Environment.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/EnvironmentActivity.md` & `curia-4.2.0b9/src/curia/api/docs/EnvironmentActivity.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Feature.md` & `curia-4.2.0b9/src/curia/api/docs/Feature.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/FeatureCategory.md` & `curia-4.2.0b9/src/curia/api/docs/FeatureCategory.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/FeatureJoinedFeatureSubCategoryJoinedFeatureCategoryResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/FeatureJoinedFeatureSubCategoryJoinedFeatureCategoryResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/FeatureJoinedFeatureSubCategoryResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/FeatureJoinedFeatureSubCategoryResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/FeatureJoinedModelPopulationResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/FeatureJoinedModelPopulationResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/FeatureJoinedOrganizationFeatureExclusionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/FeatureJoinedOrganizationFeatureExclusionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/FeatureResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/FeatureResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/FeatureStore.md` & `curia-4.2.0b9/src/curia/api/docs/FeatureStore.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/FeatureStoreResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/FeatureStoreResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/FeatureStoresApi.md` & `curia-4.2.0b9/src/curia/api/docs/FeatureStoresApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/FeatureSubCategory.md` & `curia-4.2.0b9/src/curia/api/docs/FeatureSubCategory.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/FeatureTable.md` & `curia-4.2.0b9/src/curia/api/docs/FeatureTable.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/FeaturesApi.md` & `curia-4.2.0b9/src/curia/api/docs/FeaturesApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GeographicCounts.md` & `curia-4.2.0b9/src/curia/api/docs/GeographicCounts.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GeographicQueries.md` & `curia-4.2.0b9/src/curia/api/docs/GeographicQueries.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GetManyAnalysisJobOutputResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/GetManyAnalysisJobOutputResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GetManyAnalysisJobStatusResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/GetManyAnalysisJobStatusResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GetManyModelPopulationResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/GetManyModelPopulationResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GetManyOrganizationFeatureExclusionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/GetManyOrganizationFeatureExclusionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GetManyOrganizationSettingResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/GetManyOrganizationSettingResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GetManyPopulationStoreResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/GetManyPopulationStoreResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GetManyProcessJobOutputResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/GetManyProcessJobOutputResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GetManyProcessJobStatusResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/GetManyProcessJobStatusResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GetManyTaskExecutionStatusResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/GetManyTaskExecutionStatusResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GetManyWorkflowExecutionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/GetManyWorkflowExecutionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GetManyWorkflowExecutionSpecResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/GetManyWorkflowExecutionSpecResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GetManyWorkflowExecutionStatusResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/GetManyWorkflowExecutionStatusResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/GetManyWorkflowTemplateResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/GetManyWorkflowTemplateResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/InlineResponse200.md` & `curia-4.2.0b9/src/curia/api/docs/InlineResponse200.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/InlineResponse503.md` & `curia-4.2.0b9/src/curia/api/docs/InlineResponse503.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/InternalApi.md` & `curia-4.2.0b9/src/curia/api/docs/InternalApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/InterventionDefinition.md` & `curia-4.2.0b9/src/curia/api/docs/InterventionDefinition.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Model.md` & `curia-4.2.0b9/src/curia/api/docs/Model.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelBatch.md` & `curia-4.2.0b9/src/curia/api/docs/ModelBatch.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelBatchJob.md` & `curia-4.2.0b9/src/curia/api/docs/ModelBatchJob.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelBatchJobJoinedModelBatchJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelBatchJobJoinedModelBatchJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelBatchJobJoinedModelBatchResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelBatchJobJoinedModelBatchResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelBatchJobResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelBatchJobResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelBatchJobsApi.md` & `curia-4.2.0b9/src/curia/api/docs/ModelBatchJobsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelBatchJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelBatchJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelBatchResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelBatchResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelBatchesApi.md` & `curia-4.2.0b9/src/curia/api/docs/ModelBatchesApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelDataset.md` & `curia-4.2.0b9/src/curia/api/docs/ModelDataset.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelEndpoint.md` & `curia-4.2.0b9/src/curia/api/docs/ModelEndpoint.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJob.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJob.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobConfig.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobConfig.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobEvent.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobEvent.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedCohortResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedCohortResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedDataQueryResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedDataQueryResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedDatasetResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedDatasetResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedFeatureSubCategoryResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedFeatureSubCategoryResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelJobOutputResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelJobOutputResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelJobStatusResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelJobStatusResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedCohortDefinitionJoinedPeriodDefinitionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedCohortDefinitionJoinedPeriodDefinitionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedCohortDefinitionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedCohortDefinitionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedDataQueryJoinedDatasetResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedDataQueryJoinedDatasetResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedDataQueryResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedDataQueryResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedInterventionDefinitionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedInterventionDefinitionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedOutcomeDefinitionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationJoinedOutcomeDefinitionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelPopulationResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelPopulationResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedModelResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedModelResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobOutput.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobOutput.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobOutputFeature.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobOutputFeature.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobOutputJoinedDatasetResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobOutputJoinedDatasetResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobOutputJoinedModelJobJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobOutputJoinedModelJobJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobOutputJoinedModelJobResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobOutputJoinedModelJobResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobOutputResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobOutputResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobOutputsApi.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobOutputsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobStatus.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobStatus.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobStatusJoinedModelJobJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobStatusJoinedModelJobJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobStatusJoinedModelJobResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobStatusJoinedModelJobResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobStatusResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobStatusResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobStatusesApi.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobStatusesApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJobsApi.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJobsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJoinedCohortJoinedModelJobResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJoinedCohortJoinedModelJobResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJoinedCohortResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJoinedCohortResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJoinedModelJobJoinedCohortResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJoinedModelJobJoinedCohortResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJoinedModelJobJoinedDatasetResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJoinedModelJobJoinedDatasetResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJoinedModelJobJoinedFeatureSubCategoryResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJoinedModelJobJoinedFeatureSubCategoryResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJoinedModelJobResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJoinedModelJobResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJoinedModelOutputDetailsResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJoinedModelOutputDetailsResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelJoinedUserFavoriteResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelJoinedUserFavoriteResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelOutputDetails.md` & `curia-4.2.0b9/src/curia/api/docs/ModelOutputDetails.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelPopulation.md` & `curia-4.2.0b9/src/curia/api/docs/ModelPopulation.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedCohortDefinitionJoinedPeriodDefinitionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedCohortDefinitionJoinedPeriodDefinitionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedCohortDefinitionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedCohortDefinitionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedCohortResultsResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedCohortResultsResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedDataQueryJoinedDatasetResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedDataQueryJoinedDatasetResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedDataQueryResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedDataQueryResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedFeatureResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedFeatureResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedInterventionDefinitionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedInterventionDefinitionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedModelJobJoinedModelResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedModelJobJoinedModelResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedModelJobResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedModelJobResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelPopulationJoinedOutcomeDefinitionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelPopulationJoinedOutcomeDefinitionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelPopulationResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelPopulationResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelPopulationsApi.md` & `curia-4.2.0b9/src/curia/api/docs/ModelPopulationsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ModelResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ModelsApi.md` & `curia-4.2.0b9/src/curia/api/docs/ModelsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Organization.md` & `curia-4.2.0b9/src/curia/api/docs/Organization.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/OrganizationFeatureCategoryExclusion.md` & `curia-4.2.0b9/src/curia/api/docs/OrganizationFeatureCategoryExclusion.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/OrganizationFeatureExclusion.md` & `curia-4.2.0b9/src/curia/api/docs/OrganizationFeatureExclusion.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/OrganizationResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/OrganizationResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/OrganizationSetting.md` & `curia-4.2.0b9/src/curia/api/docs/OrganizationSetting.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/OrganizationSettingResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/OrganizationSettingResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/OrganizationSettingsApi.md` & `curia-4.2.0b9/src/curia/api/docs/OrganizationSettingsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/OrganizationsApi.md` & `curia-4.2.0b9/src/curia/api/docs/OrganizationsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/OutcomeDefinition.md` & `curia-4.2.0b9/src/curia/api/docs/OutcomeDefinition.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/PlatformApi.md` & `curia-4.2.0b9/src/curia/api/docs/PlatformApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Population.md` & `curia-4.2.0b9/src/curia/api/docs/Population.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/PopulationStore.md` & `curia-4.2.0b9/src/curia/api/docs/PopulationStore.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/PopulationStoreResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/PopulationStoreResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/PopulationStoresApi.md` & `curia-4.2.0b9/src/curia/api/docs/PopulationStoresApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Process.md` & `curia-4.2.0b9/src/curia/api/docs/Process.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJob.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJob.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJobJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJobJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJobOutput.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJobOutput.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJobOutputJoinedProcessJobJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJobOutputJoinedProcessJobJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJobOutputJoinedProcessJobResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJobOutputJoinedProcessJobResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJobOutputResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJobOutputResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJobOutputsApi.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJobOutputsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJobResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJobResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJobStatus.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJobStatus.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJobStatusJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJobStatusJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJobStatusResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJobStatusResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJobStatusesApi.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJobStatusesApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJobsApi.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJobsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProcessesApi.md` & `curia-4.2.0b9/src/curia/api/docs/ProcessesApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Project.md` & `curia-4.2.0b9/src/curia/api/docs/Project.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProjectJoinedModelJoinedCohortResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProjectJoinedModelJoinedCohortResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProjectJoinedModelResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProjectJoinedModelResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProjectJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProjectJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProjectJoinedUserFavoriteResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProjectJoinedUserFavoriteResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProjectMember.md` & `curia-4.2.0b9/src/curia/api/docs/ProjectMember.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProjectMemberJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProjectMemberJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProjectMemberResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProjectMemberResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProjectMembersApi.md` & `curia-4.2.0b9/src/curia/api/docs/ProjectMembersApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/ProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/ProjectsApi.md` & `curia-4.2.0b9/src/curia/api/docs/ProjectsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Scheduler.md` & `curia-4.2.0b9/src/curia/api/docs/Scheduler.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/SchedulerApi.md` & `curia-4.2.0b9/src/curia/api/docs/SchedulerApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/SchedulerJoinedWorkflowResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/SchedulerJoinedWorkflowResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/SchedulerResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/SchedulerResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Task.md` & `curia-4.2.0b9/src/curia/api/docs/Task.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/TaskExecution.md` & `curia-4.2.0b9/src/curia/api/docs/TaskExecution.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/TaskExecutionJoinedTaskResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/TaskExecutionJoinedTaskResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/TaskExecutionJoinedWorkflowExecutionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/TaskExecutionJoinedWorkflowExecutionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/TaskExecutionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/TaskExecutionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/TaskExecutionStatus.md` & `curia-4.2.0b9/src/curia/api/docs/TaskExecutionStatus.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/TaskExecutionStatusJoinedTaskExecutionJoinedWorkflowExecutionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/TaskExecutionStatusJoinedTaskExecutionJoinedWorkflowExecutionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/TaskExecutionStatusJoinedTaskExecutionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/TaskExecutionStatusJoinedTaskExecutionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/TaskExecutionStatusResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/TaskExecutionStatusResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/TaskResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/TaskResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/TasksApi.md` & `curia-4.2.0b9/src/curia/api/docs/TasksApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateAnalysisJobDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateAnalysisJobDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateAnalysisJobStatusDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateAnalysisJobStatusDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateCohortDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateCohortDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateDataQueryDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateDataQueryDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateDatasetDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateDatasetDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateFeatureDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateFeatureDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateModelBatchJobDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateModelBatchJobDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateModelDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateModelDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateModelJobDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateModelJobDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateModelJobStatusDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateModelJobStatusDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateModelPopulationDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateModelPopulationDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateOrganizationSettingDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateOrganizationSettingDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateProcessJobDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateProcessJobDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateProcessJobStatusDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateProcessJobStatusDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateSchedulerDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateSchedulerDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateTaskDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateTaskDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateTaskExecutionDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateTaskExecutionDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateUserAuditTrailDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateUserAuditTrailDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateUserDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateUserDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateWorkflowExecutionDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateWorkflowExecutionDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateWorkflowExecutionSpecDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateWorkflowExecutionSpecDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UpdateWorkflowTemplateDto.md` & `curia-4.2.0b9/src/curia/api/docs/UpdateWorkflowTemplateDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UserAuditTrail.md` & `curia-4.2.0b9/src/curia/api/docs/UserAuditTrail.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UserAuditTrailApi.md` & `curia-4.2.0b9/src/curia/api/docs/UserAuditTrailApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UserAuditTrailResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/UserAuditTrailResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UserFavorite.md` & `curia-4.2.0b9/src/curia/api/docs/UserFavorite.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UserFavoriteJoinedModelJoinedProjectResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/UserFavoriteJoinedModelJoinedProjectResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UserFavoriteJoinedModelResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/UserFavoriteJoinedModelResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UserFavoriteResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/UserFavoriteResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UserFavoritesApi.md` & `curia-4.2.0b9/src/curia/api/docs/UserFavoritesApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/UserManagementApi.md` & `curia-4.2.0b9/src/curia/api/docs/UserManagementApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/Workflow.md` & `curia-4.2.0b9/src/curia/api/docs/Workflow.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowExecution.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowExecution.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionSpec.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionSpec.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionSpecJoinedWorkflowExecutionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionSpecJoinedWorkflowExecutionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionSpecResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionSpecResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionStatus.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionStatus.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionStatusJoinedWorkflowExecutionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionStatusJoinedWorkflowExecutionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowExecutionStatusResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowExecutionStatusResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowJoinedSchedulerResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowJoinedSchedulerResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowJoinedWorkflowExecutionResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowJoinedWorkflowExecutionResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowJoinedWorkflowTemplateResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowJoinedWorkflowTemplateResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowTemplate.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowTemplate.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowTemplateResponseDto.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowTemplateResponseDto.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/docs/WorkflowsApi.md` & `curia-4.2.0b9/src/curia/api/docs/WorkflowsApi.md`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/git_push.sh` & `curia-4.2.0b9/src/curia/api/git_push.sh`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/setup.py` & `curia-4.2.0b9/src/curia/api/setup.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/__init__.py` & `curia-4.2.0b9/src/curia/api/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/__init__.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/analyses_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/analyses_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/analysis_job_outputs_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/analysis_job_outputs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/analysis_job_statuses_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/analysis_job_statuses_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/analysis_jobs_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/analysis_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/cohorts_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/cohorts_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/data_queries_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/data_queries_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/data_stores_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/data_stores_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/data_tables_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/data_tables_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/databases_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/databases_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/dataset_columns_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/dataset_columns_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/datasets_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/datasets_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/feature_stores_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/feature_stores_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/features_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/features_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/internal_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/internal_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/model_batch_jobs_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/model_batch_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/model_batches_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/model_batches_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/model_job_outputs_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/model_job_outputs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/model_job_statuses_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/model_job_statuses_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/model_jobs_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/model_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/model_populations_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/model_populations_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/models_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/models_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/organization_settings_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/organization_settings_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/organizations_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/platform_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/platform_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/population_stores_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/population_stores_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/process_job_outputs_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/process_job_outputs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/process_job_statuses_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/process_job_statuses_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/process_jobs_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/process_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/processes_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/processes_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/project_members_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/project_members_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/projects_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/scheduler_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/scheduler_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/tasks_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/user_audit_trail_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/user_audit_trail_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/user_favorites_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/user_favorites_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/user_management_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/user_management_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api/workflows_api.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api/workflows_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/api_client.py` & `curia-4.2.0b9/src/curia/api/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/configuration.py` & `curia-4.2.0b9/src/curia/api/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/__init__.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/aggregation_type.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/aggregation_type.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_cohort_model.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_cohort_model.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_cohort_organization.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_cohort_organization.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_cohort_train_cohort.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_cohort_train_cohort.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_data_table_dataset.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_data_table_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_cohorts.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_cohorts.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_job_dataset.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_job_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_job_environment.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_job_environment.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_job_model.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_job_model.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_job_project.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_job_project.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_model_jobs.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_model_jobs.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/all_of_model_project.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/all_of_model_project.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_config.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_config.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_output.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_output.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_status.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_status_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_status_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_job_type.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_job_type.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/analysis_type.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/analysis_type.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/any_of_arithmetic_expression_value.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/any_of_arithmetic_expression_value.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/any_of_boolean_expression_value.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/any_of_boolean_expression_value.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/any_of_cohort_definition_patient_metadata_filters_items.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/any_of_cohort_definition_patient_metadata_filters_items.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/any_of_condition_value.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/any_of_condition_value.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/arithmetic_expression.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/arithmetic_expression.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/arithmetic_operator.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/arithmetic_operator.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/body.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/body.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/body1.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/body1.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/body2.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/body2.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/body3.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/body3.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/body4.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/body4.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/body5.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/body5.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/boolean_expression.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/boolean_expression.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/code.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/code.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/cohort.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/cohort.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_definition.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_definition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_filter.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_filter.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_filter_condition.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_filter_condition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_joined_cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_joined_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_results.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_results.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_set.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_set.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/cohort_window.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/cohort_window.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/condition.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/condition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/condition_operator.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/condition_operator.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/container_config.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/container_config.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_analysis_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_analysis_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_analysis_job_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_analysis_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_analysis_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_analysis_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_analysis_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_analysis_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_cohort_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_cohort_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_data_query_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_data_query_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_data_store_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_data_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_data_table_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_data_table_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_database_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_database_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_dataset_column_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_dataset_column_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_dataset_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_feature_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_feature_store_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_feature_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_analysis_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_analysis_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_analysis_job_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_analysis_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_analysis_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_analysis_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_analysis_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_analysis_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_code_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_code_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_cohort_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_cohort_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_data_query_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_data_query_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_data_store_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_data_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_dataset_column_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_dataset_column_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_dataset_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_dataset_job_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_dataset_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_environment_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_environment_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_feature_category_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_feature_category_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_feature_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_feature_store_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_feature_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_feature_sub_category_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_feature_sub_category_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_batch_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_batch_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_batch_job_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_batch_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_dataset_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_endpoint_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_endpoint_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_job_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_job_output_feature_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_job_output_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_model_population_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_model_population_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_organization_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_organization_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_organization_feature_exclusion_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_organization_feature_exclusion_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_organization_setting_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_organization_setting_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_population_store_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_population_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_process_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_process_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_process_job_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_process_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_process_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_process_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_process_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_process_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_project_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_project_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_project_member_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_project_member_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_scheduler_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_scheduler_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_task_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_task_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_task_execution_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_task_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_task_execution_status_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_task_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_user_favorite_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_user_favorite_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_workflow_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_workflow_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_workflow_execution_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_workflow_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_workflow_execution_spec_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_workflow_execution_spec_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_many_workflow_template_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_many_workflow_template_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_batch_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_batch_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_batch_job_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_batch_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_job_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_model_population_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_model_population_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_organization_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_organization_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_organization_setting_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_organization_setting_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_population_store_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_population_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_process_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_process_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_process_job_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_process_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_process_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_process_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_process_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_process_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_project_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_project_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_project_member_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_project_member_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_scheduler_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_scheduler_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_task_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_task_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_task_execution_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_task_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_task_execution_status_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_task_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_user_audit_trail_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_user_audit_trail_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_user_favorite_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_user_favorite_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_workflow_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_workflow_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_workflow_execution_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_workflow_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_workflow_execution_spec_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_workflow_execution_spec_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_workflow_execution_status_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_workflow_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/create_workflow_template_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/create_workflow_template_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/data_query.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/data_query.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/data_query_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/data_query_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/data_query_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/data_store.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/data_store.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/data_store_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/data_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/data_table.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/data_table.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/data_table_joined_database_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/data_table_joined_database_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/data_table_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/data_table_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/data_table_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/data_table_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/database.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/database.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/database_joined_data_table_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/database_joined_data_table_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/database_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/database_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/dataset.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/dataset.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_column.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_column.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_column_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_column_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_column_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_column_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_job.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_job.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_job_status.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_joined_data_query_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_joined_dataset_column_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_joined_dataset_column_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/datasetsuploadlargecomplete_parts.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/datasetsuploadlargecomplete_parts.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/environment.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/environment.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/environment_activity.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/environment_activity.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/feature.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/feature.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/feature_category.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/feature_category.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_joined_feature_category_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_joined_feature_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/feature_joined_model_population_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/feature_joined_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/feature_joined_organization_feature_exclusion_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/feature_joined_organization_feature_exclusion_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/feature_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/feature_store.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/feature_store.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/feature_store_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/feature_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/feature_sub_category.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/feature_sub_category.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/feature_table.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/feature_table.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/geographic_counts.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/geographic_counts.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/geographic_queries.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/geographic_queries.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_analysis_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_analysis_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_analysis_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_analysis_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_analysis_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_analysis_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_analysis_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_analysis_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_code_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_code_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_data_query_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_data_store_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_data_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_data_table_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_data_table_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_database_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_database_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_dataset_column_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_dataset_column_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_dataset_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_dataset_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_dataset_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_dataset_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_environment_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_environment_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_feature_category_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_feature_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_feature_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_feature_store_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_feature_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_feature_sub_category_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_batch_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_batch_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_batch_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_batch_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_endpoint_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_endpoint_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_job_event_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_job_event_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_job_output_feature_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_job_output_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_population_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_model_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_organization_feature_exclusion_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_organization_feature_exclusion_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_organization_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_organization_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_organization_setting_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_organization_setting_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_population_store_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_population_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_process_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_process_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_process_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_process_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_process_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_process_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_process_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_process_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_project_member_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_project_member_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_scheduler_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_scheduler_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_task_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_task_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_task_execution_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_task_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_task_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_task_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_user_audit_trail_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_user_audit_trail_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_user_favorite_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_workflow_execution_spec_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_workflow_execution_spec_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_workflow_execution_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_workflow_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_workflow_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_workflow_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/get_many_workflow_template_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/get_many_workflow_template_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/inline_response200.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/inline_response200_info.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/inline_response200_info.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/inline_response503.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/inline_response503.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/intervention_definition.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/intervention_definition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/json.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/json.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/logical_operator.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/logical_operator.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch_job.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch_job.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_batch_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_batch_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_dataset.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_endpoint.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_endpoint.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_config.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_config.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_event.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_event.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_data_query_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_feature_sub_category_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_intervention_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_intervention_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_outcome_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_outcome_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_population_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_model_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_output.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_output.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_output_feature.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_output_feature.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_output_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_output_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_output_joined_model_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_output_joined_model_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_output_joined_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_output_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_status.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_status_joined_model_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_status_joined_model_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_status_joined_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_status_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_cohort_joined_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_cohort_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_model_job_joined_cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_model_job_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_model_job_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_model_job_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_model_job_joined_feature_sub_category_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_model_job_joined_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_model_output_details_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_model_output_details_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_joined_user_favorite_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_joined_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_output_details.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_output_details.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_population.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_population.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_joined_period_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_joined_period_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_cohort_results_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_cohort_results_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_data_query_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_data_query_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_data_query_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_feature_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_intervention_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_intervention_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_model_job_joined_model_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_model_job_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_joined_outcome_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_joined_outcome_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_population_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/model_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/object.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/object.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/organization.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/organization_feature_category_exclusion.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/organization_feature_category_exclusion.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/organization_feature_exclusion.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/organization_feature_exclusion.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/organization_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/organization_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/organization_setting.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/organization_setting.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/organization_setting_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/organization_setting_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/outcome_definition.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/outcome_definition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/period_definition.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/period_definition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/period_type.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/period_type.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/person_set.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/person_set.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/pipeline_config.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/population.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/population.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/population_store.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/population_store.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/population_store_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/population_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_job.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_job.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_config.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_config.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_output.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_output.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_output_joined_process_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_output_joined_process_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_output_joined_process_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_output_joined_process_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_status.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_status_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_status_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/process_type.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/process_type.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/project.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/project.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/project_joined_model_joined_cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/project_joined_model_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/project_joined_model_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/project_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/project_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/project_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/project_joined_user_favorite_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/project_joined_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/project_member.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/project_member.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/project_member_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/project_member_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/project_member_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/project_member_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/scheduler.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/scheduler.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/scheduler_joined_workflow_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/scheduler_joined_workflow_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/scheduler_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/scheduler_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/select_expression.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/select_expression.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/set_operator.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/set_operator.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/state_data.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/state_data.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/task.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/task.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_joined_task_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_joined_task_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_joined_workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_status.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_status.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/task_execution_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/task_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/task_inputs.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/task_inputs.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/task_outputs.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/task_outputs.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/task_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/task_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_analysis_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_analysis_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_analysis_job_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_analysis_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_analysis_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_analysis_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_analysis_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_analysis_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_cohort_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_cohort_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_data_query_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_data_query_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_data_store_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_data_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_data_table_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_data_table_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_database_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_database_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_dataset_column_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_dataset_column_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_dataset_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_feature_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_feature_store_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_feature_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_batch_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_batch_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_batch_job_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_batch_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_job_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_model_population_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_model_population_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_organization_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_organization_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_organization_setting_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_organization_setting_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_population_store_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_population_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_process_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_process_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_process_job_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_process_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_process_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_process_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_process_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_process_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_project_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_project_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_project_member_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_project_member_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_scheduler_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_scheduler_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_task_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_task_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_task_execution_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_task_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_task_execution_status_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_task_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_user_audit_trail_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_user_audit_trail_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_user_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_user_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_user_favorite_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_user_favorite_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_workflow_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_workflow_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_workflow_execution_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_workflow_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_workflow_execution_spec_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_workflow_execution_spec_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_workflow_execution_status_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_workflow_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/update_workflow_template_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/update_workflow_template_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/user_audit_trail.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/user_audit_trail.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/user_audit_trail_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/user_audit_trail_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/user_favorite.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/user_favorite.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/user_favorite_joined_model_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/user_favorite_joined_model_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/user_favorite_joined_model_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/user_favorite_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/user_favorite_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_spec.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_spec.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_spec_joined_workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_spec_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_spec_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_spec_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_status.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_status.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_status_joined_workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_status_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_execution_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_joined_scheduler_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_joined_scheduler_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_joined_workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_joined_workflow_template_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_joined_workflow_template_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_template.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_template.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_template_definition.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_template_definition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_template_parameters.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_template_parameters.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/workflow_template_response_dto.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/workflow_template_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/models/zip_data.py` & `curia-4.2.0b9/src/curia/api/swagger_client/models/zip_data.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/swagger_client/rest.py` & `curia-4.2.0b9/src/curia/api/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_aggregation_type.py` & `curia-4.2.0b9/src/curia/api/test/test_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_all_of_cohort_model.py` & `curia-4.2.0b9/src/curia/api/test/test_all_of_cohort_model.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_all_of_cohort_organization.py` & `curia-4.2.0b9/src/curia/api/test/test_all_of_cohort_organization.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_all_of_cohort_train_cohort.py` & `curia-4.2.0b9/src/curia/api/test/test_all_of_cohort_train_cohort.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_all_of_data_table_dataset.py` & `curia-4.2.0b9/src/curia/api/test/test_all_of_data_table_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_all_of_model_cohorts.py` & `curia-4.2.0b9/src/curia/api/test/test_all_of_model_cohorts.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_all_of_model_job_dataset.py` & `curia-4.2.0b9/src/curia/api/test/test_all_of_model_job_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_all_of_model_job_environment.py` & `curia-4.2.0b9/src/curia/api/test/test_all_of_model_job_environment.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_all_of_model_job_model.py` & `curia-4.2.0b9/src/curia/api/test/test_all_of_model_job_model.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_all_of_model_job_project.py` & `curia-4.2.0b9/src/curia/api/test/test_all_of_model_job_project.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_all_of_model_model_jobs.py` & `curia-4.2.0b9/src/curia/api/test/test_all_of_model_model_jobs.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_all_of_model_project.py` & `curia-4.2.0b9/src/curia/api/test/test_all_of_model_project.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analyses_api.py` & `curia-4.2.0b9/src/curia/api/test/test_analyses_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job_config.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job_config.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job_output.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job_output.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job_output_joined_analysis_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job_output_joined_analysis_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job_output_joined_analysis_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job_output_joined_analysis_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job_outputs_api.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job_outputs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job_status.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job_status_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job_status_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job_statuses_api.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job_statuses_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_job_type.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_job_type.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_jobs_api.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_analysis_type.py` & `curia-4.2.0b9/src/curia/api/test/test_analysis_type.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_any_of_arithmetic_expression_value.py` & `curia-4.2.0b9/src/curia/api/test/test_any_of_arithmetic_expression_value.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_any_of_boolean_expression_value.py` & `curia-4.2.0b9/src/curia/api/test/test_any_of_boolean_expression_value.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_any_of_cohort_definition_patient_metadata_filters_items.py` & `curia-4.2.0b9/src/curia/api/test/test_any_of_cohort_definition_patient_metadata_filters_items.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_any_of_condition_value.py` & `curia-4.2.0b9/src/curia/api/test/test_any_of_condition_value.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_arithmetic_expression.py` & `curia-4.2.0b9/src/curia/api/test/test_arithmetic_expression.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_arithmetic_operator.py` & `curia-4.2.0b9/src/curia/api/test/test_arithmetic_operator.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_body.py` & `curia-4.2.0b9/src/curia/api/test/test_body.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_body1.py` & `curia-4.2.0b9/src/curia/api/test/test_body1.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_body2.py` & `curia-4.2.0b9/src/curia/api/test/test_body2.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_body3.py` & `curia-4.2.0b9/src/curia/api/test/test_body3.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_body4.py` & `curia-4.2.0b9/src/curia/api/test/test_body4.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_body5.py` & `curia-4.2.0b9/src/curia/api/test/test_body5.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_boolean_expression.py` & `curia-4.2.0b9/src/curia/api/test/test_boolean_expression.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_code.py` & `curia-4.2.0b9/src/curia/api/test/test_code.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_cohort.py` & `curia-4.2.0b9/src/curia/api/test/test_cohort.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_cohort_definition.py` & `curia-4.2.0b9/src/curia/api/test/test_cohort_definition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_cohort_filter.py` & `curia-4.2.0b9/src/curia/api/test/test_cohort_filter.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_cohort_filter_condition.py` & `curia-4.2.0b9/src/curia/api/test/test_cohort_filter_condition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_cohort_joined_cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_cohort_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_cohort_joined_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_cohort_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_cohort_results.py` & `curia-4.2.0b9/src/curia/api/test/test_cohort_results.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_cohort_set.py` & `curia-4.2.0b9/src/curia/api/test/test_cohort_set.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_cohort_window.py` & `curia-4.2.0b9/src/curia/api/test/test_cohort_window.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_cohorts_api.py` & `curia-4.2.0b9/src/curia/api/test/test_cohorts_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_condition.py` & `curia-4.2.0b9/src/curia/api/test/test_condition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_condition_operator.py` & `curia-4.2.0b9/src/curia/api/test/test_condition_operator.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_container_config.py` & `curia-4.2.0b9/src/curia/api/test/test_container_config.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_analysis_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_analysis_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_analysis_job_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_analysis_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_analysis_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_analysis_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_analysis_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_analysis_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_cohort_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_cohort_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_data_query_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_data_query_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_data_store_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_data_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_data_table_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_data_table_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_database_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_database_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_dataset_column_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_dataset_column_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_dataset_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_feature_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_feature_store_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_feature_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_analysis_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_analysis_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_analysis_job_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_analysis_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_analysis_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_analysis_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_analysis_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_analysis_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_code_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_code_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_cohort_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_cohort_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_data_query_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_data_query_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_data_store_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_data_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_dataset_column_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_dataset_column_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_dataset_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_dataset_job_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_dataset_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_environment_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_environment_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_feature_category_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_feature_category_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_feature_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_feature_store_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_feature_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_feature_sub_category_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_feature_sub_category_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_model_batch_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_model_batch_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_model_batch_job_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_model_batch_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_model_dataset_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_model_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_model_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_model_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_model_endpoint_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_model_endpoint_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_model_job_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_model_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_model_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_model_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_model_job_output_feature_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_model_job_output_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_model_population_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_model_population_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_organization_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_organization_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_organization_feature_exclusion_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_organization_feature_exclusion_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_organization_setting_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_organization_setting_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_population_store_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_population_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_process_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_process_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_process_job_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_process_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_process_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_process_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_process_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_process_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_project_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_project_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_project_member_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_project_member_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_scheduler_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_scheduler_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_task_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_task_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_task_execution_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_task_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_task_execution_status_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_task_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_user_favorite_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_user_favorite_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_workflow_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_workflow_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_workflow_execution_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_workflow_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_workflow_execution_spec_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_workflow_execution_spec_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_many_workflow_template_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_many_workflow_template_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_model_batch_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_model_batch_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_model_batch_job_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_model_batch_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_model_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_model_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_model_job_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_model_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_model_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_model_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_model_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_model_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_model_population_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_model_population_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_organization_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_organization_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_organization_setting_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_organization_setting_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_population_store_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_population_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_process_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_process_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_process_job_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_process_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_process_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_process_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_process_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_process_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_project_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_project_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_project_member_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_project_member_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_scheduler_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_scheduler_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_task_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_task_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_task_execution_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_task_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_task_execution_status_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_task_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_user_audit_trail_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_user_audit_trail_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_user_favorite_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_user_favorite_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_workflow_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_workflow_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_workflow_execution_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_workflow_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_workflow_execution_spec_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_workflow_execution_spec_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_workflow_execution_status_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_workflow_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_create_workflow_template_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_create_workflow_template_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_data_queries_api.py` & `curia-4.2.0b9/src/curia/api/test/test_data_queries_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_data_query.py` & `curia-4.2.0b9/src/curia/api/test/test_data_query.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_data_query_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_data_query_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_data_query_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_data_store.py` & `curia-4.2.0b9/src/curia/api/test/test_data_store.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_data_store_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_data_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_data_stores_api.py` & `curia-4.2.0b9/src/curia/api/test/test_data_stores_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_data_table.py` & `curia-4.2.0b9/src/curia/api/test/test_data_table.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_data_table_joined_database_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_data_table_joined_database_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_data_table_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_data_table_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_data_table_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_data_table_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_data_tables_api.py` & `curia-4.2.0b9/src/curia/api/test/test_data_tables_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_database.py` & `curia-4.2.0b9/src/curia/api/test/test_database.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_database_joined_data_table_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_database_joined_data_table_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_database_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_database_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_databases_api.py` & `curia-4.2.0b9/src/curia/api/test/test_databases_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_dataset.py` & `curia-4.2.0b9/src/curia/api/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_dataset_column.py` & `curia-4.2.0b9/src/curia/api/test/test_dataset_column.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_dataset_column_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_dataset_column_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_dataset_column_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_dataset_column_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_dataset_columns_api.py` & `curia-4.2.0b9/src/curia/api/test/test_dataset_columns_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_dataset_job.py` & `curia-4.2.0b9/src/curia/api/test/test_dataset_job.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_dataset_job_status.py` & `curia-4.2.0b9/src/curia/api/test/test_dataset_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_dataset_joined_data_query_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_dataset_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_dataset_joined_dataset_column_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_dataset_joined_dataset_column_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_datasets_api.py` & `curia-4.2.0b9/src/curia/api/test/test_datasets_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_datasetsuploadlargecomplete_parts.py` & `curia-4.2.0b9/src/curia/api/test/test_datasetsuploadlargecomplete_parts.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_environment.py` & `curia-4.2.0b9/src/curia/api/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_environment_activity.py` & `curia-4.2.0b9/src/curia/api/test/test_environment_activity.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_feature.py` & `curia-4.2.0b9/src/curia/api/test/test_feature.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_feature_category.py` & `curia-4.2.0b9/src/curia/api/test/test_feature_category.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_feature_joined_feature_sub_category_joined_feature_category_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_feature_joined_feature_sub_category_joined_feature_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_feature_joined_feature_sub_category_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_feature_joined_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_feature_joined_model_population_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_feature_joined_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_feature_joined_organization_feature_exclusion_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_feature_joined_organization_feature_exclusion_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_feature_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_feature_store.py` & `curia-4.2.0b9/src/curia/api/test/test_feature_store.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_feature_store_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_feature_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_feature_stores_api.py` & `curia-4.2.0b9/src/curia/api/test/test_feature_stores_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_feature_sub_category.py` & `curia-4.2.0b9/src/curia/api/test/test_feature_sub_category.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_feature_table.py` & `curia-4.2.0b9/src/curia/api/test/test_feature_table.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_features_api.py` & `curia-4.2.0b9/src/curia/api/test/test_features_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_geographic_counts.py` & `curia-4.2.0b9/src/curia/api/test/test_geographic_counts.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_geographic_queries.py` & `curia-4.2.0b9/src/curia/api/test/test_geographic_queries.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_analysis_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_analysis_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_analysis_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_analysis_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_analysis_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_analysis_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_analysis_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_analysis_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_code_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_code_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_data_query_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_data_store_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_data_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_data_table_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_data_table_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_database_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_database_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_dataset_column_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_dataset_column_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_dataset_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_dataset_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_dataset_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_dataset_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_environment_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_environment_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_feature_category_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_feature_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_feature_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_feature_store_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_feature_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_feature_sub_category_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_model_batch_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_model_batch_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_model_batch_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_model_batch_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_model_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_model_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_model_endpoint_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_model_endpoint_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_model_job_event_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_model_job_event_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_model_job_output_feature_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_model_job_output_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_model_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_model_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_model_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_model_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_model_population_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_model_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_organization_feature_exclusion_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_organization_feature_exclusion_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_organization_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_organization_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_organization_setting_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_organization_setting_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_population_store_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_population_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_process_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_process_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_process_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_process_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_process_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_process_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_process_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_process_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_project_member_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_project_member_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_scheduler_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_scheduler_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_task_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_task_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_task_execution_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_task_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_task_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_task_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_user_audit_trail_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_user_audit_trail_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_user_favorite_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_workflow_execution_spec_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_workflow_execution_spec_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_workflow_execution_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_workflow_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_workflow_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_workflow_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_get_many_workflow_template_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_get_many_workflow_template_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_inline_response200.py` & `curia-4.2.0b9/src/curia/api/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_inline_response200_info.py` & `curia-4.2.0b9/src/curia/api/test/test_inline_response200_info.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_inline_response503.py` & `curia-4.2.0b9/src/curia/api/test/test_inline_response503.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_internal_api.py` & `curia-4.2.0b9/src/curia/api/test/test_internal_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_intervention_definition.py` & `curia-4.2.0b9/src/curia/api/test/test_intervention_definition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_json.py` & `curia-4.2.0b9/src/curia/api/test/test_json.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_logical_operator.py` & `curia-4.2.0b9/src/curia/api/test/test_logical_operator.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model.py` & `curia-4.2.0b9/src/curia/api/test/test_model.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_batch.py` & `curia-4.2.0b9/src/curia/api/test/test_model_batch.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_batch_job.py` & `curia-4.2.0b9/src/curia/api/test/test_model_batch_job.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_batch_job_joined_model_batch_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_batch_job_joined_model_batch_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_batch_job_joined_model_batch_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_batch_job_joined_model_batch_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_batch_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_batch_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_batch_jobs_api.py` & `curia-4.2.0b9/src/curia/api/test/test_model_batch_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_batch_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_batch_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_batch_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_batch_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_batches_api.py` & `curia-4.2.0b9/src/curia/api/test/test_model_batches_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_dataset.py` & `curia-4.2.0b9/src/curia/api/test/test_model_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_endpoint.py` & `curia-4.2.0b9/src/curia/api/test/test_model_endpoint.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_config.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_config.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_event.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_event.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_data_query_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_feature_sub_category_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_joined_intervention_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_joined_intervention_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_joined_outcome_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_joined_outcome_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_population_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_model_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_output.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_output.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_output_feature.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_output_feature.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_output_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_output_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_output_joined_model_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_output_joined_model_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_output_joined_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_output_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_outputs_api.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_outputs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_status.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_status_joined_model_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_status_joined_model_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_status_joined_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_status_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_job_statuses_api.py` & `curia-4.2.0b9/src/curia/api/test/test_model_job_statuses_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_jobs_api.py` & `curia-4.2.0b9/src/curia/api/test/test_model_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_joined_cohort_joined_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_joined_cohort_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_joined_cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_joined_model_job_joined_cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_joined_model_job_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_joined_model_job_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_joined_model_job_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_joined_model_job_joined_feature_sub_category_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_joined_model_job_joined_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_joined_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_joined_model_output_details_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_joined_model_output_details_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_joined_user_favorite_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_joined_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_output_details.py` & `curia-4.2.0b9/src/curia/api/test/test_model_output_details.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_population.py` & `curia-4.2.0b9/src/curia/api/test/test_model_population.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_population_joined_cohort_definition_joined_period_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_population_joined_cohort_definition_joined_period_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_population_joined_cohort_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_population_joined_cohort_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_population_joined_cohort_results_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_population_joined_cohort_results_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_population_joined_data_query_joined_dataset_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_population_joined_data_query_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_population_joined_data_query_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_population_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_population_joined_feature_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_population_joined_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_population_joined_intervention_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_population_joined_intervention_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_population_joined_model_job_joined_model_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_population_joined_model_job_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_population_joined_model_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_population_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_population_joined_outcome_definition_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_population_joined_outcome_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_population_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_populations_api.py` & `curia-4.2.0b9/src/curia/api/test/test_model_populations_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_model_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_models_api.py` & `curia-4.2.0b9/src/curia/api/test/test_models_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_object.py` & `curia-4.2.0b9/src/curia/api/test/test_object.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_organization.py` & `curia-4.2.0b9/src/curia/api/test/test_organization.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_organization_feature_category_exclusion.py` & `curia-4.2.0b9/src/curia/api/test/test_organization_feature_category_exclusion.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_organization_feature_exclusion.py` & `curia-4.2.0b9/src/curia/api/test/test_organization_feature_exclusion.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_organization_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_organization_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_organization_setting.py` & `curia-4.2.0b9/src/curia/api/test/test_organization_setting.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_organization_setting_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_organization_setting_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_organization_settings_api.py` & `curia-4.2.0b9/src/curia/api/test/test_organization_settings_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_organizations_api.py` & `curia-4.2.0b9/src/curia/api/test/test_organizations_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_outcome_definition.py` & `curia-4.2.0b9/src/curia/api/test/test_outcome_definition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_period_definition.py` & `curia-4.2.0b9/src/curia/api/test/test_period_definition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_period_type.py` & `curia-4.2.0b9/src/curia/api/test/test_period_type.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_person_set.py` & `curia-4.2.0b9/src/curia/api/test/test_person_set.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_pipeline_config.py` & `curia-4.2.0b9/src/curia/api/test/test_pipeline_config.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_platform_api.py` & `curia-4.2.0b9/src/curia/api/test/test_platform_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_population.py` & `curia-4.2.0b9/src/curia/api/test/test_population.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_population_store.py` & `curia-4.2.0b9/src/curia/api/test/test_population_store.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_population_store_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_population_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_population_stores_api.py` & `curia-4.2.0b9/src/curia/api/test/test_population_stores_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process.py` & `curia-4.2.0b9/src/curia/api/test/test_process.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_job.py` & `curia-4.2.0b9/src/curia/api/test/test_process_job.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_job_config.py` & `curia-4.2.0b9/src/curia/api/test/test_process_job_config.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_process_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_job_output.py` & `curia-4.2.0b9/src/curia/api/test/test_process_job_output.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_job_output_joined_process_job_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_process_job_output_joined_process_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_job_output_joined_process_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_process_job_output_joined_process_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_job_output_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_process_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_job_outputs_api.py` & `curia-4.2.0b9/src/curia/api/test/test_process_job_outputs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_job_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_process_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_job_status.py` & `curia-4.2.0b9/src/curia/api/test/test_process_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_job_status_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_process_job_status_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_job_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_process_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_job_statuses_api.py` & `curia-4.2.0b9/src/curia/api/test/test_process_job_statuses_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_jobs_api.py` & `curia-4.2.0b9/src/curia/api/test/test_process_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_process_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_process_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_process_type.py` & `curia-4.2.0b9/src/curia/api/test/test_process_type.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_processes_api.py` & `curia-4.2.0b9/src/curia/api/test/test_processes_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_project.py` & `curia-4.2.0b9/src/curia/api/test/test_project.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_project_joined_model_joined_cohort_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_project_joined_model_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_project_joined_model_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_project_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_project_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_project_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_project_joined_user_favorite_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_project_joined_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_project_member.py` & `curia-4.2.0b9/src/curia/api/test/test_project_member.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_project_member_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_project_member_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_project_member_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_project_member_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_project_members_api.py` & `curia-4.2.0b9/src/curia/api/test/test_project_members_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_projects_api.py` & `curia-4.2.0b9/src/curia/api/test/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_scheduler.py` & `curia-4.2.0b9/src/curia/api/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_scheduler_api.py` & `curia-4.2.0b9/src/curia/api/test/test_scheduler_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_scheduler_joined_workflow_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_scheduler_joined_workflow_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_scheduler_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_scheduler_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_select_expression.py` & `curia-4.2.0b9/src/curia/api/test/test_select_expression.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_set_operator.py` & `curia-4.2.0b9/src/curia/api/test/test_set_operator.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_state_data.py` & `curia-4.2.0b9/src/curia/api/test/test_state_data.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_task.py` & `curia-4.2.0b9/src/curia/api/test/test_task.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_task_execution.py` & `curia-4.2.0b9/src/curia/api/test/test_task_execution.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_task_execution_joined_task_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_task_execution_joined_task_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_task_execution_joined_workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_task_execution_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_task_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_task_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_task_execution_status.py` & `curia-4.2.0b9/src/curia/api/test/test_task_execution_status.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_task_execution_status_joined_task_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_task_execution_status_joined_task_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_task_execution_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_task_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_task_inputs.py` & `curia-4.2.0b9/src/curia/api/test/test_task_inputs.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_task_outputs.py` & `curia-4.2.0b9/src/curia/api/test/test_task_outputs.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_task_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_task_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_tasks_api.py` & `curia-4.2.0b9/src/curia/api/test/test_tasks_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_analysis_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_analysis_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_analysis_job_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_analysis_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_analysis_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_analysis_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_analysis_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_analysis_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_cohort_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_cohort_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_data_query_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_data_query_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_data_store_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_data_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_data_table_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_data_table_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_database_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_database_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_dataset_column_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_dataset_column_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_dataset_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_feature_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_feature_store_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_feature_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_model_batch_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_model_batch_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_model_batch_job_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_model_batch_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_model_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_model_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_model_job_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_model_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_model_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_model_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_model_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_model_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_model_population_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_model_population_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_organization_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_organization_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_organization_setting_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_organization_setting_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_population_store_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_population_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_process_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_process_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_process_job_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_process_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_process_job_output_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_process_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_process_job_status_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_process_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_project_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_project_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_project_member_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_project_member_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_scheduler_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_scheduler_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_task_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_task_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_task_execution_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_task_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_task_execution_status_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_task_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_user_audit_trail_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_user_audit_trail_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_user_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_user_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_user_favorite_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_user_favorite_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_workflow_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_workflow_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_workflow_execution_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_workflow_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_workflow_execution_spec_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_workflow_execution_spec_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_workflow_execution_status_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_workflow_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_update_workflow_template_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_update_workflow_template_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_user_audit_trail.py` & `curia-4.2.0b9/src/curia/api/test/test_user_audit_trail.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_user_audit_trail_api.py` & `curia-4.2.0b9/src/curia/api/test/test_user_audit_trail_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_user_audit_trail_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_user_audit_trail_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_user_favorite.py` & `curia-4.2.0b9/src/curia/api/test/test_user_favorite.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_user_favorite_joined_model_joined_project_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_user_favorite_joined_model_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_user_favorite_joined_model_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_user_favorite_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_user_favorite_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_user_favorites_api.py` & `curia-4.2.0b9/src/curia/api/test/test_user_favorites_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_user_management_api.py` & `curia-4.2.0b9/src/curia/api/test/test_user_management_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_execution.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_execution.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_execution_spec.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_execution_spec.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_execution_spec_joined_workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_execution_spec_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_execution_spec_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_execution_spec_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_execution_status.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_execution_status.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_execution_status_joined_workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_execution_status_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_execution_status_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_joined_scheduler_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_joined_scheduler_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_joined_workflow_execution_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_joined_workflow_template_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_joined_workflow_template_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_template.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_template.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_template_definition.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_template_definition.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_template_parameters.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_template_parameters.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflow_template_response_dto.py` & `curia-4.2.0b9/src/curia/api/test/test_workflow_template_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_workflows_api.py` & `curia-4.2.0b9/src/curia/api/test/test_workflows_api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/api/test/test_zip_data.py` & `curia-4.2.0b9/src/curia/api/test/test_zip_data.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/mock/api.py` & `curia-4.2.0b9/src/curia/mock/api.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/mock/api_server.py` & `curia-4.2.0b9/src/curia/mock/api_server.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/mock/moto.py` & `curia-4.2.0b9/src/curia/mock/moto.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/mock/s3.py` & `curia-4.2.0b9/src/curia/mock/s3.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/mock/server.py` & `curia-4.2.0b9/src/curia/mock/server.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/session.py` & `curia-4.2.0b9/src/curia/session.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/utils/dataset.py` & `curia-4.2.0b9/src/curia/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/utils/job.py` & `curia-4.2.0b9/src/curia/utils/job.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/utils/python.py` & `curia-4.2.0b9/src/curia/utils/python.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/utils/s3.py` & `curia-4.2.0b9/src/curia/utils/s3.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/src/curia/utils/string.py` & `curia-4.2.0b9/src/curia/utils/string.py`

 * *Files identical despite different names*

### Comparing `curia-4.2.0b8/PKG-INFO` & `curia-4.2.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: curia
-Version: 4.2.0b8
+Version: 4.2.0b9
 Summary: A library for interfacing with the Curia API.
 Author: Aledade, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: boto3 (>=1.26.150,<2.0.0)
+Requires-Dist: boto3 (>=1.26.0,<2.0.0)
 Requires-Dist: certifi (>=14.05.14)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: flask-cors (>=3.0.10,<4.0.0)
 Requires-Dist: logzero (>=1.7.0,<2.0.0)
 Requires-Dist: moto (>=4.1.11,<5.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/curia.svg)](https://badge.fury.io/py/curia)
 
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
-[![Python 3.11](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3110/)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)
 
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Curia-ai_curia-python-sdk&metric=alert_status&token=e6d33fff8f3c9375c06d3b3deba711b1891c0b0b)](https://sonarcloud.io/dashboard?id=Curia-ai_curia-python-sdk)
 [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=Curia-ai_curia-python-sdk&metric=bugs&token=e6d33fff8f3c9375c06d3b3deba711b1891c0b0b)](https://sonarcloud.io/dashboard?id=Curia-ai_curia-python-sdk)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=Curia-ai_curia-python-sdk&metric=coverage&token=e6d33fff8f3c9375c06d3b3deba711b1891c0b0b)](https://sonarcloud.io/dashboard?id=Curia-ai_curia-python-sdk)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=Curia-ai_curia-python-sdk&metric=sqale_rating&token=e6d33fff8f3c9375c06d3b3deba711b1891c0b0b)](https://sonarcloud.io/dashboard?id=Curia-ai_curia-python-sdk)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=Curia-ai_curia-python-sdk&metric=reliability_rating&token=e6d33fff8f3c9375c06d3b3deba711b1891c0b0b)](https://sonarcloud.io/dashboard?id=Curia-ai_curia-python-sdk)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=Curia-ai_curia-python-sdk&metric=security_rating&token=e6d33fff8f3c9375c06d3b3deba711b1891c0b0b)](https://sonarcloud.io/dashboard?id=Curia-ai_curia-python-sdk)
```

