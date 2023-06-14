# Comparing `tmp/p360-export-1.5.5.tar.gz` & `tmp/p360-export-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p360-export-1.5.5.tar", max compression
+gzip compressed data, was "p360-export-1.5.6.tar", max compression
```

## Comparing `p360-export-1.5.5.tar` & `p360-export-1.5.6.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     2459 2022-06-27 08:14:06.215938 p360-export-1.5.5/LICENSE
--rw-r--r--   0        0        0     6809 2023-06-12 15:16:44.017553 p360-export-1.5.5/README.md
--rw-r--r--   0        0        0     1762 2023-06-13 07:17:42.702125 p360-export-1.5.5/pyproject.toml
--rw-r--r--   0        0        0     1396 2022-12-15 13:06:57.741031 p360-export-1.5.5/src/p360_export/ExportManager.py
--rw-r--r--   0        0        0      812 2022-12-16 09:36:34.652886 p360-export-1.5.5/src/p360_export/ExportRunner.py
--rw-r--r--   0        0        0      417 2022-12-15 13:06:57.741031 p360-export-1.5.5/src/p360_export/_config/config.yaml
--rw-r--r--   0        0        0      569 2022-06-27 08:14:06.219271 p360-export-1.5.5/src/p360_export/config/AzureStorageConfigGetter.py
--rw-r--r--   0        0        0      701 2022-12-16 09:36:34.652886 p360-export-1.5.5/src/p360_export/config/AzureStorageConfigGetterTest.py
--rw-r--r--   0        0        0      148 2022-06-27 08:14:06.219271 p360-export-1.5.5/src/p360_export/config/ConfigGetterInterface.py
--rw-r--r--   0        0        0      463 2022-06-27 08:14:06.219271 p360-export-1.5.5/src/p360_export/config/LocalFileConfigGetter.py
--rw-r--r--   0        0        0      607 2022-12-15 13:06:57.741031 p360-export-1.5.5/src/p360_export/config/LocalFileConfigGetterTest.py
--rw-r--r--   0        0        0     2594 2022-12-16 09:36:34.652886 p360-export-1.5.5/src/p360_export/config/SkeletonConfigGetter.py
--rw-r--r--   0        0        0     2579 2023-06-12 15:16:44.017553 p360-export-1.5.5/src/p360_export/containers/Container.py
--rw-r--r--   0        0        0      569 2023-06-12 15:00:47.187522 p360-export-1.5.5/src/p360_export/containers/ContainerTest.py
--rw-r--r--   0        0        0     2772 2022-12-16 09:36:34.652886 p360-export-1.5.5/src/p360_export/containers/Core.py
--rw-r--r--   0        0        0      576 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/containers/DataPlatformContainer.py
--rw-r--r--   0        0        0     1160 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/containers/FacebookContainer.py
--rw-r--r--   0        0        0     2041 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/containers/GoogleAdsContainer.py
--rw-r--r--   0        0        0     1297 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/containers/GoogleAnalytics4Container.py
--rw-r--r--   0        0        0     3183 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/containers/SFMCContainer.py
--rw-r--r--   0        0        0      497 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/data/ColumnMappingGetter.py
--rw-r--r--   0        0        0      384 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/data/ColumnMappingGetterTest.py
--rw-r--r--   0        0        0      334 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/data/DataPicker.py
--rw-r--r--   0        0        0      249 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/data/build/DataBuilderInterface.py
--rw-r--r--   0        0        0     2768 2022-12-16 09:53:01.479561 p360-export-1.5.5/src/p360_export/data/build/FeatureStoreDataBuilder.py
--rw-r--r--   0        0        0     1803 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/data/build/FeatureStoreDataBuilderTest.py
--rw-r--r--   0        0        0      462 2022-06-27 13:41:55.362162 p360-export-1.5.5/src/p360_export/data/extra/FacebookData.py
--rw-r--r--   0        0        0      183 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/data/fix/DataFixerInterface.py
--rw-r--r--   0        0        0     3327 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/data/fix/DataFixersTest.py
--rw-r--r--   0        0        0      221 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/data/fix/DataPlatformDataFixer.py
--rw-r--r--   0        0        0     1012 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/data/fix/FacebookDataFixer.py
--rw-r--r--   0        0        0      755 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/data/fix/GoogleAdsDataFixer.py
--rw-r--r--   0        0        0      770 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/data/fix/GoogleAnalytics4DataFixer.py
--rw-r--r--   0        0        0      495 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/data/fix/SFMCDataFixer.py
--rw-r--r--   0        0        0     1666 2022-12-15 13:28:40.720987 p360-export-1.5.5/src/p360_export/data/type/resolve/DataFrameTypeResolver.py
--rw-r--r--   0        0        0     2350 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/data/type/resolve/SFMCTypeResolver.py
--rw-r--r--   0        0        0      202 2022-08-08 07:07:32.309111 p360-export-1.5.5/src/p360_export/data/type/resolve/TypeResolverInterface.py
--rw-r--r--   0        0        0     4027 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/data/type/resolve/TypeResolversTest.py
--rw-r--r--   0        0        0      328 2022-12-15 13:20:42.677669 p360-export-1.5.5/src/p360_export/data/type/validate/EmailValidator.py
--rw-r--r--   0        0        0      810 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/data/type/validate/PhoneNumberValidator.py
--rw-r--r--   0        0        0      146 2022-08-08 07:07:32.309111 p360-export-1.5.5/src/p360_export/data/type/validate/ValidatorInterface.py
--rw-r--r--   0        0        0     1679 2022-10-11 08:38:43.679337 p360-export-1.5.5/src/p360_export/data/type/validate/ValidatorsTest.py
--rw-r--r--   0        0        0      111 2023-06-12 15:16:44.017553 p360-export-1.5.5/src/p360_export/exceptions/config.py
--rw-r--r--   0        0        0      324 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/exceptions/data_picker.py
--rw-r--r--   0        0        0      306 2022-08-04 09:01:17.894159 p360-export-1.5.5/src/p360_export/exceptions/exporter.py
--rw-r--r--   0        0        0      183 2022-08-11 06:11:41.159706 p360-export-1.5.5/src/p360_export/exceptions/manager.py
--rw-r--r--   0        0        0      120 2022-06-27 14:44:52.609942 p360-export-1.5.5/src/p360_export/exceptions/query_builder.py
--rw-r--r--   0        0        0      186 2022-08-08 07:07:32.309111 p360-export-1.5.5/src/p360_export/exceptions/type_resolver.py
--rw-r--r--   0        0        0       65 2022-10-18 07:42:31.982398 p360-export-1.5.5/src/p360_export/exceptions/utils.py
--rw-r--r--   0        0        0      448 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/export/AudienceNameGetter.py
--rw-r--r--   0        0        0      664 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/export/DataPlatformExporter.py
--rw-r--r--   0        0        0      172 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/export/ExporterInterface.py
--rw-r--r--   0        0        0     1592 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/export/facebook/CustomAudienceGetter.py
--rw-r--r--   0        0        0     2354 2022-12-15 13:06:57.744364 p360-export-1.5.5/src/p360_export/export/facebook/FacebookExporter.py
--rw-r--r--   0        0        0      737 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/export/facebook/FacebookParameters.py
--rw-r--r--   0        0        0      761 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/export/google/ads/GoogleAdsExporter.py
--rw-r--r--   0        0        0      809 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/export/google/ads/GoogleClient.py
--rw-r--r--   0        0        0      712 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/export/google/ads/UserDataJobCreator.py
--rw-r--r--   0        0        0     1037 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/export/google/ads/UserDataJobOperationGetter.py
--rw-r--r--   0        0        0     1074 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/export/google/ads/UserDataJobOperationRequestGetter.py
--rw-r--r--   0        0        0     1383 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/export/google/ads/UserDataSender.py
--rw-r--r--   0        0        0     1893 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/export/google/ads/UserListGetter.py
--rw-r--r--   0        0        0      819 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/export/google/ga4/GoogleAnalytics4Client.py
--rw-r--r--   0        0        0     1242 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/export/google/ga4/GoogleAnalytics4EventBuilder.py
--rw-r--r--   0        0        0     1583 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/export/google/ga4/GoogleAnalytics4EventsUploader.py
--rw-r--r--   0        0        0      461 2023-06-12 09:25:52.916853 p360-export-1.5.5/src/p360_export/export/google/ga4/GoogleAnalytics4Exporter.py
--rw-r--r--   0        0        0     2402 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/export/sfmc/DataExtensionCreator.py
--rw-r--r--   0        0        0     1803 2022-12-15 13:06:57.747697 p360-export-1.5.5/src/p360_export/export/sfmc/DataExtensionFieldCreator.py
--rw-r--r--   0        0        0     3100 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/export/sfmc/DataExtensionFieldUpdater.py
--rw-r--r--   0        0        0     1485 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/export/sfmc/DataExtensionGetter.py
--rw-r--r--   0        0        0      362 2022-12-15 13:06:57.747697 p360-export-1.5.5/src/p360_export/export/sfmc/FieldNameFixer.py
--rw-r--r--   0        0        0      624 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/export/sfmc/ImportDefinitionExecutor.py
--rw-r--r--   0        0        0     2091 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/export/sfmc/ImportDefinitionGetter.py
--rw-r--r--   0        0        0     2475 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/export/sfmc/SFMCData.py
--rw-r--r--   0        0        0     1245 2022-12-15 13:06:57.747697 p360-export-1.5.5/src/p360_export/export/sfmc/SFMCExporter.py
--rw-r--r--   0        0        0     1103 2022-12-15 13:06:57.747697 p360-export-1.5.5/src/p360_export/export/sfmc/SFTPUploader.py
--rw-r--r--   0        0        0     5157 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/query/QueryBuilder.py
--rw-r--r--   0        0        0     1877 2022-12-16 09:36:34.656220 p360-export-1.5.5/src/p360_export/query/QueryBuildersTest.py
--rw-r--r--   0        0        0     2683 2022-12-16 09:36:34.659553 p360-export-1.5.5/src/p360_export/test/PySparkTestCase.py
--rw-r--r--   0        0        0      817 2022-12-16 09:36:34.659553 p360-export-1.5.5/src/p360_export/utils/ColumnHasher.py
--rw-r--r--   0        0        0     1797 2022-12-16 09:36:34.659553 p360-export-1.5.5/src/p360_export/utils/ColumnHasherTest.py
--rw-r--r--   0        0        0      566 2022-12-16 09:36:34.659553 p360-export-1.5.5/src/p360_export/utils/ColumnSampleGetter.py
--rw-r--r--   0        0        0     1859 2022-12-16 09:36:34.659553 p360-export-1.5.5/src/p360_export/utils/ColumnSampleGetterTest.py
--rw-r--r--   0        0        0      402 2022-12-15 13:06:57.747697 p360-export-1.5.5/src/p360_export/utils/secret_getters/DbutilsSecretsSecretGetter.py
--rw-r--r--   0        0        0      712 2022-12-15 13:06:57.747697 p360-export-1.5.5/src/p360_export/utils/secret_getters/DbutilsSecretsSecretGetterTest.py
--rw-r--r--   0        0        0      228 2022-12-15 13:06:57.747697 p360-export-1.5.5/src/p360_export/utils/secret_getters/EnvVariableSecretGetter.py
--rw-r--r--   0        0        0      618 2022-12-15 13:06:57.747697 p360-export-1.5.5/src/p360_export/utils/secret_getters/EnvVariableSecretGetterTest.py
--rw-r--r--   0        0        0      141 2022-12-15 13:06:57.747697 p360-export-1.5.5/src/p360_export/utils/secret_getters/SecretGetterInterface.py
--rw-r--r--   0        0        0      708 2022-12-15 13:07:02.387697 p360-export-1.5.5/src/p360_export/utils/utils.py
--rw-r--r--   0        0        0     8342 2023-06-13 07:45:06.335890 p360-export-1.5.5/setup.py
--rw-r--r--   0        0        0     7711 2023-06-13 07:45:06.336388 p360-export-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0     2459 2022-06-27 08:14:06.215938 p360-export-1.5.6/LICENSE
+-rw-r--r--   0        0        0     7108 2023-06-14 09:44:37.465258 p360-export-1.5.6/README.md
+-rw-r--r--   0        0        0     1762 2023-06-14 09:44:37.465258 p360-export-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0     1396 2022-12-15 13:06:57.741031 p360-export-1.5.6/src/p360_export/ExportManager.py
+-rw-r--r--   0        0        0      812 2022-12-16 09:36:34.652886 p360-export-1.5.6/src/p360_export/ExportRunner.py
+-rw-r--r--   0        0        0      417 2022-12-15 13:06:57.741031 p360-export-1.5.6/src/p360_export/_config/config.yaml
+-rw-r--r--   0        0        0      569 2022-06-27 08:14:06.219271 p360-export-1.5.6/src/p360_export/config/AzureStorageConfigGetter.py
+-rw-r--r--   0        0        0      701 2022-12-16 09:36:34.652886 p360-export-1.5.6/src/p360_export/config/AzureStorageConfigGetterTest.py
+-rw-r--r--   0        0        0      148 2022-06-27 08:14:06.219271 p360-export-1.5.6/src/p360_export/config/ConfigGetterInterface.py
+-rw-r--r--   0        0        0      463 2022-06-27 08:14:06.219271 p360-export-1.5.6/src/p360_export/config/LocalFileConfigGetter.py
+-rw-r--r--   0        0        0      607 2022-12-15 13:06:57.741031 p360-export-1.5.6/src/p360_export/config/LocalFileConfigGetterTest.py
+-rw-r--r--   0        0        0     2594 2022-12-16 09:36:34.652886 p360-export-1.5.6/src/p360_export/config/SkeletonConfigGetter.py
+-rw-r--r--   0        0        0     2579 2023-06-12 15:16:44.017553 p360-export-1.5.6/src/p360_export/containers/Container.py
+-rw-r--r--   0        0        0      569 2023-06-12 15:00:47.187522 p360-export-1.5.6/src/p360_export/containers/ContainerTest.py
+-rw-r--r--   0        0        0     2772 2022-12-16 09:36:34.652886 p360-export-1.5.6/src/p360_export/containers/Core.py
+-rw-r--r--   0        0        0      576 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/containers/DataPlatformContainer.py
+-rw-r--r--   0        0        0     1160 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/containers/FacebookContainer.py
+-rw-r--r--   0        0        0     2041 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/containers/GoogleAdsContainer.py
+-rw-r--r--   0        0        0     1297 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/containers/GoogleAnalytics4Container.py
+-rw-r--r--   0        0        0     3183 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/containers/SFMCContainer.py
+-rw-r--r--   0        0        0      497 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/data/ColumnMappingGetter.py
+-rw-r--r--   0        0        0      384 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/data/ColumnMappingGetterTest.py
+-rw-r--r--   0        0        0      334 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/data/DataPicker.py
+-rw-r--r--   0        0        0      249 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/data/build/DataBuilderInterface.py
+-rw-r--r--   0        0        0     2768 2022-12-16 09:53:01.479561 p360-export-1.5.6/src/p360_export/data/build/FeatureStoreDataBuilder.py
+-rw-r--r--   0        0        0     1803 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/data/build/FeatureStoreDataBuilderTest.py
+-rw-r--r--   0        0        0      462 2022-06-27 13:41:55.362162 p360-export-1.5.6/src/p360_export/data/extra/FacebookData.py
+-rw-r--r--   0        0        0      183 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/data/fix/DataFixerInterface.py
+-rw-r--r--   0        0        0     3327 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/data/fix/DataFixersTest.py
+-rw-r--r--   0        0        0      221 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/data/fix/DataPlatformDataFixer.py
+-rw-r--r--   0        0        0     1012 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/data/fix/FacebookDataFixer.py
+-rw-r--r--   0        0        0      755 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/data/fix/GoogleAdsDataFixer.py
+-rw-r--r--   0        0        0      770 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/data/fix/GoogleAnalytics4DataFixer.py
+-rw-r--r--   0        0        0      495 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/data/fix/SFMCDataFixer.py
+-rw-r--r--   0        0        0     1666 2022-12-15 13:28:40.720987 p360-export-1.5.6/src/p360_export/data/type/resolve/DataFrameTypeResolver.py
+-rw-r--r--   0        0        0     2350 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/data/type/resolve/SFMCTypeResolver.py
+-rw-r--r--   0        0        0      202 2022-08-08 07:07:32.309111 p360-export-1.5.6/src/p360_export/data/type/resolve/TypeResolverInterface.py
+-rw-r--r--   0        0        0     4027 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/data/type/resolve/TypeResolversTest.py
+-rw-r--r--   0        0        0      328 2022-12-15 13:20:42.677669 p360-export-1.5.6/src/p360_export/data/type/validate/EmailValidator.py
+-rw-r--r--   0        0        0      810 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/data/type/validate/PhoneNumberValidator.py
+-rw-r--r--   0        0        0      146 2022-08-08 07:07:32.309111 p360-export-1.5.6/src/p360_export/data/type/validate/ValidatorInterface.py
+-rw-r--r--   0        0        0     1679 2022-10-11 08:38:43.679337 p360-export-1.5.6/src/p360_export/data/type/validate/ValidatorsTest.py
+-rw-r--r--   0        0        0      111 2023-06-12 15:16:44.017553 p360-export-1.5.6/src/p360_export/exceptions/config.py
+-rw-r--r--   0        0        0      324 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/exceptions/data_picker.py
+-rw-r--r--   0        0        0      306 2022-08-04 09:01:17.894159 p360-export-1.5.6/src/p360_export/exceptions/exporter.py
+-rw-r--r--   0        0        0      183 2022-08-11 06:11:41.159706 p360-export-1.5.6/src/p360_export/exceptions/manager.py
+-rw-r--r--   0        0        0      120 2022-06-27 14:44:52.609942 p360-export-1.5.6/src/p360_export/exceptions/query_builder.py
+-rw-r--r--   0        0        0      186 2022-08-08 07:07:32.309111 p360-export-1.5.6/src/p360_export/exceptions/type_resolver.py
+-rw-r--r--   0        0        0       65 2022-10-18 07:42:31.982398 p360-export-1.5.6/src/p360_export/exceptions/utils.py
+-rw-r--r--   0        0        0      448 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/export/AudienceNameGetter.py
+-rw-r--r--   0        0        0      664 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/export/DataPlatformExporter.py
+-rw-r--r--   0        0        0      172 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/export/ExporterInterface.py
+-rw-r--r--   0        0        0     1592 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/export/facebook/CustomAudienceGetter.py
+-rw-r--r--   0        0        0     2354 2022-12-15 13:06:57.744364 p360-export-1.5.6/src/p360_export/export/facebook/FacebookExporter.py
+-rw-r--r--   0        0        0      737 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/export/facebook/FacebookParameters.py
+-rw-r--r--   0        0        0      761 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/export/google/ads/GoogleAdsExporter.py
+-rw-r--r--   0        0        0      809 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/export/google/ads/GoogleClient.py
+-rw-r--r--   0        0        0      712 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/export/google/ads/UserDataJobCreator.py
+-rw-r--r--   0        0        0     1037 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/export/google/ads/UserDataJobOperationGetter.py
+-rw-r--r--   0        0        0     1074 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/export/google/ads/UserDataJobOperationRequestGetter.py
+-rw-r--r--   0        0        0     1383 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/export/google/ads/UserDataSender.py
+-rw-r--r--   0        0        0     1893 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/export/google/ads/UserListGetter.py
+-rw-r--r--   0        0        0      819 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/export/google/ga4/GoogleAnalytics4Client.py
+-rw-r--r--   0        0        0     1242 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/export/google/ga4/GoogleAnalytics4EventBuilder.py
+-rw-r--r--   0        0        0     1583 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/export/google/ga4/GoogleAnalytics4EventsUploader.py
+-rw-r--r--   0        0        0      461 2023-06-12 09:25:52.916853 p360-export-1.5.6/src/p360_export/export/google/ga4/GoogleAnalytics4Exporter.py
+-rw-r--r--   0        0        0     2402 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/export/sfmc/DataExtensionCreator.py
+-rw-r--r--   0        0        0     1803 2022-12-15 13:06:57.747697 p360-export-1.5.6/src/p360_export/export/sfmc/DataExtensionFieldCreator.py
+-rw-r--r--   0        0        0     3100 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/export/sfmc/DataExtensionFieldUpdater.py
+-rw-r--r--   0        0        0     1485 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/export/sfmc/DataExtensionGetter.py
+-rw-r--r--   0        0        0      362 2022-12-15 13:06:57.747697 p360-export-1.5.6/src/p360_export/export/sfmc/FieldNameFixer.py
+-rw-r--r--   0        0        0      624 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/export/sfmc/ImportDefinitionExecutor.py
+-rw-r--r--   0        0        0     2091 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/export/sfmc/ImportDefinitionGetter.py
+-rw-r--r--   0        0        0     2611 2023-06-14 09:36:14.245250 p360-export-1.5.6/src/p360_export/export/sfmc/SFMCData.py
+-rw-r--r--   0        0        0     1245 2022-12-15 13:06:57.747697 p360-export-1.5.6/src/p360_export/export/sfmc/SFMCExporter.py
+-rw-r--r--   0        0        0     1131 2023-06-14 09:36:14.245250 p360-export-1.5.6/src/p360_export/export/sfmc/SFTPUploader.py
+-rw-r--r--   0        0        0     5157 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/query/QueryBuilder.py
+-rw-r--r--   0        0        0     1877 2022-12-16 09:36:34.656220 p360-export-1.5.6/src/p360_export/query/QueryBuildersTest.py
+-rw-r--r--   0        0        0     2683 2022-12-16 09:36:34.659553 p360-export-1.5.6/src/p360_export/test/PySparkTestCase.py
+-rw-r--r--   0        0        0      817 2022-12-16 09:36:34.659553 p360-export-1.5.6/src/p360_export/utils/ColumnHasher.py
+-rw-r--r--   0        0        0     1797 2022-12-16 09:36:34.659553 p360-export-1.5.6/src/p360_export/utils/ColumnHasherTest.py
+-rw-r--r--   0        0        0      566 2022-12-16 09:36:34.659553 p360-export-1.5.6/src/p360_export/utils/ColumnSampleGetter.py
+-rw-r--r--   0        0        0     1859 2022-12-16 09:36:34.659553 p360-export-1.5.6/src/p360_export/utils/ColumnSampleGetterTest.py
+-rw-r--r--   0        0        0      402 2022-12-15 13:06:57.747697 p360-export-1.5.6/src/p360_export/utils/secret_getters/DbutilsSecretsSecretGetter.py
+-rw-r--r--   0        0        0      712 2022-12-15 13:06:57.747697 p360-export-1.5.6/src/p360_export/utils/secret_getters/DbutilsSecretsSecretGetterTest.py
+-rw-r--r--   0        0        0      228 2022-12-15 13:06:57.747697 p360-export-1.5.6/src/p360_export/utils/secret_getters/EnvVariableSecretGetter.py
+-rw-r--r--   0        0        0      618 2022-12-15 13:06:57.747697 p360-export-1.5.6/src/p360_export/utils/secret_getters/EnvVariableSecretGetterTest.py
+-rw-r--r--   0        0        0      141 2022-12-15 13:06:57.747697 p360-export-1.5.6/src/p360_export/utils/secret_getters/SecretGetterInterface.py
+-rw-r--r--   0        0        0      708 2022-12-15 13:07:02.387697 p360-export-1.5.6/src/p360_export/utils/utils.py
+-rw-r--r--   0        0        0     8644 2023-06-14 09:44:44.260273 p360-export-1.5.6/setup.py
+-rw-r--r--   0        0        0     8010 2023-06-14 09:44:44.260837 p360-export-1.5.6/PKG-INFO
```

### Comparing `p360-export-1.5.5/LICENSE` & `p360-export-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/README.md` & `p360-export-1.5.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # p360-export
 
 Persona360 exporters.
 
 ### Latest Changes
+
+* :bookmark: Bump version to 1.5.6. PR [#93](https://github.com/DataSentics/p360-export/pull/93) by [@Vinsho](https://github.com/Vinsho).
+* :sparkles: Added new SFMC credential ftp_relative_path. PR [#92](https://github.com/DataSentics/p360-export/pull/92) by [@Vinsho](https://github.com/Vinsho).
 * :sparkles: Added Google Analytics 4 exporter. PR [#82](https://github.com/DataSentics/p360-export/pull/82) by [@guderkar](https://github.com/guderkar).
 #### 1.4.0
 * :construction_worker: Fixed release workflow PR [#81](https://github.com/DataSentics/p360-export/pull/81) by [@Vinsho](https://github.com/Vinsho).
 * :recycle: Typo fix. PR [#79](https://github.com/DataSentics/p360-export/pull/79) by [@Vinsho](https://github.com/Vinsho).
 * :sparkles: Fixed backward compatibility. PR [#77](https://github.com/DataSentics/p360-export/pull/77) by [@Vinsho](https://github.com/Vinsho).
 * :sparkles: Added logic for loading env specific config. PR [#76](https://github.com/DataSentics/p360-export/pull/76) by [@Vinsho](https://github.com/Vinsho).
 * :recycle: Odap integration. PR [#75](https://github.com/DataSentics/p360-export/pull/75) by [@Vinsho](https://github.com/Vinsho).
```

### Comparing `p360-export-1.5.5/pyproject.toml` & `p360-export-1.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "p360-export"
-version = "1.5.5"
+version = "1.5.6"
 description = "Persona360 data export"
 readme = "README.md"
 
 license = "Proprietary"
 
 authors = [
     "Datasentics <jiri.koutny@datasentics.com>"
```

### Comparing `p360-export-1.5.5/src/p360_export/ExportManager.py` & `p360-export-1.5.6/src/p360_export/ExportManager.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/ExportRunner.py` & `p360-export-1.5.6/src/p360_export/ExportRunner.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/config/AzureStorageConfigGetter.py` & `p360-export-1.5.6/src/p360_export/config/AzureStorageConfigGetter.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/config/AzureStorageConfigGetterTest.py` & `p360-export-1.5.6/src/p360_export/config/AzureStorageConfigGetterTest.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/config/LocalFileConfigGetterTest.py` & `p360-export-1.5.6/src/p360_export/config/LocalFileConfigGetterTest.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/config/SkeletonConfigGetter.py` & `p360-export-1.5.6/src/p360_export/config/SkeletonConfigGetter.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/containers/Container.py` & `p360-export-1.5.6/src/p360_export/containers/Container.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/containers/ContainerTest.py` & `p360-export-1.5.6/src/p360_export/containers/ContainerTest.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/containers/Core.py` & `p360-export-1.5.6/src/p360_export/containers/Core.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/containers/DataPlatformContainer.py` & `p360-export-1.5.6/src/p360_export/containers/DataPlatformContainer.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/containers/FacebookContainer.py` & `p360-export-1.5.6/src/p360_export/containers/FacebookContainer.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/containers/GoogleAdsContainer.py` & `p360-export-1.5.6/src/p360_export/containers/GoogleAdsContainer.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/containers/GoogleAnalytics4Container.py` & `p360-export-1.5.6/src/p360_export/containers/GoogleAnalytics4Container.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/containers/SFMCContainer.py` & `p360-export-1.5.6/src/p360_export/containers/SFMCContainer.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/data/build/FeatureStoreDataBuilder.py` & `p360-export-1.5.6/src/p360_export/data/build/FeatureStoreDataBuilder.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/data/build/FeatureStoreDataBuilderTest.py` & `p360-export-1.5.6/src/p360_export/data/build/FeatureStoreDataBuilderTest.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/data/fix/DataFixersTest.py` & `p360-export-1.5.6/src/p360_export/data/fix/DataFixersTest.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/data/fix/FacebookDataFixer.py` & `p360-export-1.5.6/src/p360_export/data/fix/FacebookDataFixer.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/data/fix/GoogleAdsDataFixer.py` & `p360-export-1.5.6/src/p360_export/data/fix/GoogleAdsDataFixer.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/data/fix/GoogleAnalytics4DataFixer.py` & `p360-export-1.5.6/src/p360_export/data/fix/GoogleAnalytics4DataFixer.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/data/type/resolve/DataFrameTypeResolver.py` & `p360-export-1.5.6/src/p360_export/data/type/resolve/DataFrameTypeResolver.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/data/type/resolve/SFMCTypeResolver.py` & `p360-export-1.5.6/src/p360_export/data/type/resolve/SFMCTypeResolver.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/data/type/resolve/TypeResolversTest.py` & `p360-export-1.5.6/src/p360_export/data/type/resolve/TypeResolversTest.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/data/type/validate/PhoneNumberValidator.py` & `p360-export-1.5.6/src/p360_export/data/type/validate/PhoneNumberValidator.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/data/type/validate/ValidatorsTest.py` & `p360-export-1.5.6/src/p360_export/data/type/validate/ValidatorsTest.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/DataPlatformExporter.py` & `p360-export-1.5.6/src/p360_export/export/DataPlatformExporter.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/facebook/CustomAudienceGetter.py` & `p360-export-1.5.6/src/p360_export/export/facebook/CustomAudienceGetter.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/facebook/FacebookExporter.py` & `p360-export-1.5.6/src/p360_export/export/facebook/FacebookExporter.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/facebook/FacebookParameters.py` & `p360-export-1.5.6/src/p360_export/export/facebook/FacebookParameters.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/google/ads/GoogleAdsExporter.py` & `p360-export-1.5.6/src/p360_export/export/google/ads/GoogleAdsExporter.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/google/ads/GoogleClient.py` & `p360-export-1.5.6/src/p360_export/export/google/ads/GoogleClient.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/google/ads/UserDataJobCreator.py` & `p360-export-1.5.6/src/p360_export/export/google/ads/UserDataJobCreator.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/google/ads/UserDataJobOperationGetter.py` & `p360-export-1.5.6/src/p360_export/export/google/ads/UserDataJobOperationGetter.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/google/ads/UserDataJobOperationRequestGetter.py` & `p360-export-1.5.6/src/p360_export/export/google/ads/UserDataJobOperationRequestGetter.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/google/ads/UserDataSender.py` & `p360-export-1.5.6/src/p360_export/export/google/ads/UserDataSender.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/google/ads/UserListGetter.py` & `p360-export-1.5.6/src/p360_export/export/google/ads/UserListGetter.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/google/ga4/GoogleAnalytics4Client.py` & `p360-export-1.5.6/src/p360_export/export/google/ga4/GoogleAnalytics4Client.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/google/ga4/GoogleAnalytics4EventBuilder.py` & `p360-export-1.5.6/src/p360_export/export/google/ga4/GoogleAnalytics4EventBuilder.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/google/ga4/GoogleAnalytics4EventsUploader.py` & `p360-export-1.5.6/src/p360_export/export/google/ga4/GoogleAnalytics4EventsUploader.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/sfmc/DataExtensionCreator.py` & `p360-export-1.5.6/src/p360_export/export/sfmc/DataExtensionCreator.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/sfmc/DataExtensionFieldCreator.py` & `p360-export-1.5.6/src/p360_export/export/sfmc/DataExtensionFieldCreator.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/sfmc/DataExtensionFieldUpdater.py` & `p360-export-1.5.6/src/p360_export/export/sfmc/DataExtensionFieldUpdater.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/sfmc/DataExtensionGetter.py` & `p360-export-1.5.6/src/p360_export/export/sfmc/DataExtensionGetter.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/sfmc/ImportDefinitionExecutor.py` & `p360-export-1.5.6/src/p360_export/export/sfmc/ImportDefinitionExecutor.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/sfmc/ImportDefinitionGetter.py` & `p360-export-1.5.6/src/p360_export/export/sfmc/ImportDefinitionGetter.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/sfmc/SFMCData.py` & `p360-export-1.5.6/src/p360_export/export/sfmc/SFMCData.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,7 +66,11 @@
     @property
     def client_secret(self) -> str:
         return self.__secret_getter.get(key=self.__config["credentials"]["client_secret_key"])
 
     @property
     def ftp_password(self) -> str:
         return self.__secret_getter.get(key=self.__config["credentials"]["ftp_password_key"])
+
+    @property
+    def ftp_relative_path(self) -> str:
+        return self.__config["credentials"].get("ftp_relative_path", "/Import/")
```

### Comparing `p360-export-1.5.5/src/p360_export/export/sfmc/SFMCExporter.py` & `p360-export-1.5.6/src/p360_export/export/sfmc/SFMCExporter.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/export/sfmc/SFTPUploader.py` & `p360-export-1.5.6/src/p360_export/export/sfmc/SFTPUploader.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,11 +26,11 @@
     def upload(self, df: DataFrame):
         connection = self.__get_connection()
 
         csv_path = self.__get_csv_path(self.__sfmc_data.export_id)
 
         df.toPandas().to_csv(csv_path)  # pyre-ignore[16]
 
-        connection.put(csv_path, f"/Import/{self.__sfmc_data.export_id}.csv")
+        connection.put(csv_path, f"{self.__sfmc_data.ftp_relative_path}{self.__sfmc_data.export_id}.csv")
         connection.close()
 
         os.remove(csv_path)
```

### Comparing `p360-export-1.5.5/src/p360_export/query/QueryBuilder.py` & `p360-export-1.5.6/src/p360_export/query/QueryBuilder.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/query/QueryBuildersTest.py` & `p360-export-1.5.6/src/p360_export/query/QueryBuildersTest.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/test/PySparkTestCase.py` & `p360-export-1.5.6/src/p360_export/test/PySparkTestCase.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/utils/ColumnHasher.py` & `p360-export-1.5.6/src/p360_export/utils/ColumnHasher.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/utils/ColumnHasherTest.py` & `p360-export-1.5.6/src/p360_export/utils/ColumnHasherTest.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/utils/ColumnSampleGetter.py` & `p360-export-1.5.6/src/p360_export/utils/ColumnSampleGetter.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/utils/ColumnSampleGetterTest.py` & `p360-export-1.5.6/src/p360_export/utils/ColumnSampleGetterTest.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/utils/secret_getters/DbutilsSecretsSecretGetterTest.py` & `p360-export-1.5.6/src/p360_export/utils/secret_getters/DbutilsSecretsSecretGetterTest.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/utils/secret_getters/EnvVariableSecretGetterTest.py` & `p360-export-1.5.6/src/p360_export/utils/secret_getters/EnvVariableSecretGetterTest.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/src/p360_export/utils/utils.py` & `p360-export-1.5.6/src/p360_export/utils/utils.py`

 * *Files identical despite different names*

### Comparing `p360-export-1.5.5/setup.py` & `p360-export-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
  'jsonschema>=4.4.0,<5.0.0',
  'pandas>=1.5.2,<2.0.0',
  'paramiko>=2.11.0,<3.0.0',
  'pyarrow>=10.0.1,<11.0.0']
 
 setup_kwargs = {
     'name': 'p360-export',
-    'version': '1.5.5',
+    'version': '1.5.6',
     'description': 'Persona360 data export',
-    'long_description': "# p360-export\n\nPersona360 exporters.\n\n### Latest Changes\n* :sparkles: Added Google Analytics 4 exporter. PR [#82](https://github.com/DataSentics/p360-export/pull/82) by [@guderkar](https://github.com/guderkar).\n#### 1.4.0\n* :construction_worker: Fixed release workflow PR [#81](https://github.com/DataSentics/p360-export/pull/81) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Typo fix. PR [#79](https://github.com/DataSentics/p360-export/pull/79) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Fixed backward compatibility. PR [#77](https://github.com/DataSentics/p360-export/pull/77) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Added logic for loading env specific config. PR [#76](https://github.com/DataSentics/p360-export/pull/76) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Odap integration. PR [#75](https://github.com/DataSentics/p360-export/pull/75) by [@Vinsho](https://github.com/Vinsho).\n* :art: Replaced pyfony with dependency-injector PR [#74](https://github.com/DataSentics/p360-export/pull/74) by [@Vinsho](https://github.com/Vinsho)\n#### 1.3.1\n* :bug: Don't fail on empty columns, don't send them to SFMC. PR [#72](https://github.com/DataSentics/p360-export/pull/72) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Added SFMC Field Name Fixer. PR [#71](https://github.com/DataSentics/p360-export/pull/71) by [@Vinsho](https://github.com/Vinsho).\n* :bug: Fixed missing _ in less than and greater than. PR [#70](https://github.com/DataSentics/p360-export/pull/70) by [@Vinsho](https://github.com/Vinsho).\n#### 1.3.0\n* :recycle: Target user_list by export_id. PR [#68](https://github.com/DataSentics/p360-export/pull/68) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Google ads export send User ID instead of email. PR [#67](https://github.com/DataSentics/p360-export/pull/67) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Target audience based on its id part. PR [#66](https://github.com/DataSentics/p360-export/pull/66) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Work with SFMC Customer Keys. PR [#65](https://github.com/DataSentics/p360-export/pull/65) by [@Vinsho](https://github.com/Vinsho).\n#### 1.2.1\n* :technologist: Replace asserts with native unittest assertions. PR [#63](https://github.com/DataSentics/p360-export/pull/63) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Added not_equals to QueryBuilder. PR [#62](https://github.com/DataSentics/p360-export/pull/62) by [@Vinsho](https://github.com/Vinsho).\n* :bug: Fixed query equals with multiple values. PR [#61](https://github.com/DataSentics/p360-export/pull/61) by [@Vinsho](https://github.com/Vinsho).\n* :bug: Fixed attributes only export. PR [#60](https://github.com/DataSentics/p360-export/pull/60) by [@Vinsho](https://github.com/Vinsho).\n#### 1.2.0\n* :arrow_up: Feature store bundle upgrade to 2.7.1. PR [#57](https://github.com/DataSentics/p360-export/pull/57) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Enabled export without segment. PR [#56](https://github.com/DataSentics/p360-export/pull/56) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Persona renamed to Segment. PR [#55](https://github.com/DataSentics/p360-export/pull/55) by [@Vinsho](https://github.com/Vinsho).\n* :boom: Config is recieved as argument in runner. PR [#53](https://github.com/DataSentics/p360-export/pull/53) by [@Vinsho](https://github.com/Vinsho).\n* :arrow_up: pyre-check-nightly replaced by pyre-check. PR [#54](https://github.com/DataSentics/p360-export/pull/54) by [@Vinsho](https://github.com/Vinsho).\n#### 1.1.0\n* :recycle: SFMC Exporter refactor. PR [#46](https://github.com/DataSentics/p360-export/pull/46) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: QueryBuilder and ExportManager refactor. PR [#49](https://github.com/DataSentics/p360-export/pull/49) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: ColumnSampleGetter turned to service. PR [#47](https://github.com/DataSentics/p360-export/pull/47) by [@Vinsho](https://github.com/Vinsho).\n* :arrow_up: Unpin the fixed feature-store-bundle version. PR [#48](https://github.com/DataSentics/p360-export/pull/48) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Google Ads Exporter Refactor. PR [#44](https://github.com/DataSentics/p360-export/pull/44) by [@Vinsho](https://github.com/Vinsho).\n* ♻️ TypeGuesser component refactor. PR [#35](https://github.com/DataSentics/p360-export/pull/35) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Facebook Exporter refactor. PR [#43](https://github.com/DataSentics/p360-export/pull/43) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Data Picker components refactor. PR [#40](https://github.com/DataSentics/p360-export/pull/40) by [@Vinsho](https://github.com/Vinsho).\n* :green_heart: Fixed failing pylint tests. PR [#42](https://github.com/DataSentics/p360-export/pull/42) by [@Vinsho](https://github.com/Vinsho).\n* :technologist: Alter pylint to pyfony coding style. PR [#41](https://github.com/DataSentics/p360-export/pull/41) by [@Vinsho](https://github.com/Vinsho).\n\n#### 1.0.2\n* :arrow_up: Feature store bundle update to 2.5.1. PR [#36](https://github.com/DataSentics/p360-export/pull/36) by [@matejoravec](https://github.com/matejoravec).\n* :construction_worker: Release pipeline customized. PR [#34](https://github.com/DataSentics/p360-export/pull/34) by [@matejoravec](https://github.com/matejoravec).\n\n#### 1.0.1\n* :memo: Missing emojis added to README. PR [#31](https://github.com/DataSentics/p360-export/pull/31) by [@matejoravec](https://github.com/matejoravec).\n* :arrow_up: feature-store-bundle 2.5.0b2 -> 2.5.0b3. PR [#30](https://github.com/DataSentics/p360-export/pull/30) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Make created Data Extension sendable. PR [#29](https://github.com/DataSentics/p360-export/pull/29) by [@Vinsho](https://github.com/Vinsho).\n* :bug: Fixed Type Guesser bugs. PR [#28](https://github.com/DataSentics/p360-export/pull/28) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Added Type Guesser. PR [#27](https://github.com/DataSentics/p360-export/pull/27) by [@Vinsho](https://github.com/Vinsho).\n* :building_construction: Retrieval of redundant attributes removed. PR [#26](https://github.com/DataSentics/p360-export/pull/26) by [@matejoravec](https://github.com/matejoravec).\n* :sparkles: SFMC Exporter: Enable field updating. PR [#23](https://github.com/DataSentics/p360-export/pull/23) by [@Vinsho](https://github.com/Vinsho).\n* :construction_worker: Build & Release Pipeline outsourced. PR [#25](https://github.com/DataSentics/p360-export/pull/25) by [@matejoravec](https://github.com/matejoravec).\n* :construction_worker: Latest changes action added. PR [#24](https://github.com/DataSentics/p360-export/pull/24) by [@matejoravec](https://github.com/matejoravec).\n",
+    'long_description': "# p360-export\n\nPersona360 exporters.\n\n### Latest Changes\n\n* :bookmark: Bump version to 1.5.6. PR [#93](https://github.com/DataSentics/p360-export/pull/93) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Added new SFMC credential ftp_relative_path. PR [#92](https://github.com/DataSentics/p360-export/pull/92) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Added Google Analytics 4 exporter. PR [#82](https://github.com/DataSentics/p360-export/pull/82) by [@guderkar](https://github.com/guderkar).\n#### 1.4.0\n* :construction_worker: Fixed release workflow PR [#81](https://github.com/DataSentics/p360-export/pull/81) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Typo fix. PR [#79](https://github.com/DataSentics/p360-export/pull/79) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Fixed backward compatibility. PR [#77](https://github.com/DataSentics/p360-export/pull/77) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Added logic for loading env specific config. PR [#76](https://github.com/DataSentics/p360-export/pull/76) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Odap integration. PR [#75](https://github.com/DataSentics/p360-export/pull/75) by [@Vinsho](https://github.com/Vinsho).\n* :art: Replaced pyfony with dependency-injector PR [#74](https://github.com/DataSentics/p360-export/pull/74) by [@Vinsho](https://github.com/Vinsho)\n#### 1.3.1\n* :bug: Don't fail on empty columns, don't send them to SFMC. PR [#72](https://github.com/DataSentics/p360-export/pull/72) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Added SFMC Field Name Fixer. PR [#71](https://github.com/DataSentics/p360-export/pull/71) by [@Vinsho](https://github.com/Vinsho).\n* :bug: Fixed missing _ in less than and greater than. PR [#70](https://github.com/DataSentics/p360-export/pull/70) by [@Vinsho](https://github.com/Vinsho).\n#### 1.3.0\n* :recycle: Target user_list by export_id. PR [#68](https://github.com/DataSentics/p360-export/pull/68) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Google ads export send User ID instead of email. PR [#67](https://github.com/DataSentics/p360-export/pull/67) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Target audience based on its id part. PR [#66](https://github.com/DataSentics/p360-export/pull/66) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Work with SFMC Customer Keys. PR [#65](https://github.com/DataSentics/p360-export/pull/65) by [@Vinsho](https://github.com/Vinsho).\n#### 1.2.1\n* :technologist: Replace asserts with native unittest assertions. PR [#63](https://github.com/DataSentics/p360-export/pull/63) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Added not_equals to QueryBuilder. PR [#62](https://github.com/DataSentics/p360-export/pull/62) by [@Vinsho](https://github.com/Vinsho).\n* :bug: Fixed query equals with multiple values. PR [#61](https://github.com/DataSentics/p360-export/pull/61) by [@Vinsho](https://github.com/Vinsho).\n* :bug: Fixed attributes only export. PR [#60](https://github.com/DataSentics/p360-export/pull/60) by [@Vinsho](https://github.com/Vinsho).\n#### 1.2.0\n* :arrow_up: Feature store bundle upgrade to 2.7.1. PR [#57](https://github.com/DataSentics/p360-export/pull/57) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Enabled export without segment. PR [#56](https://github.com/DataSentics/p360-export/pull/56) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Persona renamed to Segment. PR [#55](https://github.com/DataSentics/p360-export/pull/55) by [@Vinsho](https://github.com/Vinsho).\n* :boom: Config is recieved as argument in runner. PR [#53](https://github.com/DataSentics/p360-export/pull/53) by [@Vinsho](https://github.com/Vinsho).\n* :arrow_up: pyre-check-nightly replaced by pyre-check. PR [#54](https://github.com/DataSentics/p360-export/pull/54) by [@Vinsho](https://github.com/Vinsho).\n#### 1.1.0\n* :recycle: SFMC Exporter refactor. PR [#46](https://github.com/DataSentics/p360-export/pull/46) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: QueryBuilder and ExportManager refactor. PR [#49](https://github.com/DataSentics/p360-export/pull/49) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: ColumnSampleGetter turned to service. PR [#47](https://github.com/DataSentics/p360-export/pull/47) by [@Vinsho](https://github.com/Vinsho).\n* :arrow_up: Unpin the fixed feature-store-bundle version. PR [#48](https://github.com/DataSentics/p360-export/pull/48) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Google Ads Exporter Refactor. PR [#44](https://github.com/DataSentics/p360-export/pull/44) by [@Vinsho](https://github.com/Vinsho).\n* ♻️ TypeGuesser component refactor. PR [#35](https://github.com/DataSentics/p360-export/pull/35) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Facebook Exporter refactor. PR [#43](https://github.com/DataSentics/p360-export/pull/43) by [@Vinsho](https://github.com/Vinsho).\n* :recycle: Data Picker components refactor. PR [#40](https://github.com/DataSentics/p360-export/pull/40) by [@Vinsho](https://github.com/Vinsho).\n* :green_heart: Fixed failing pylint tests. PR [#42](https://github.com/DataSentics/p360-export/pull/42) by [@Vinsho](https://github.com/Vinsho).\n* :technologist: Alter pylint to pyfony coding style. PR [#41](https://github.com/DataSentics/p360-export/pull/41) by [@Vinsho](https://github.com/Vinsho).\n\n#### 1.0.2\n* :arrow_up: Feature store bundle update to 2.5.1. PR [#36](https://github.com/DataSentics/p360-export/pull/36) by [@matejoravec](https://github.com/matejoravec).\n* :construction_worker: Release pipeline customized. PR [#34](https://github.com/DataSentics/p360-export/pull/34) by [@matejoravec](https://github.com/matejoravec).\n\n#### 1.0.1\n* :memo: Missing emojis added to README. PR [#31](https://github.com/DataSentics/p360-export/pull/31) by [@matejoravec](https://github.com/matejoravec).\n* :arrow_up: feature-store-bundle 2.5.0b2 -> 2.5.0b3. PR [#30](https://github.com/DataSentics/p360-export/pull/30) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Make created Data Extension sendable. PR [#29](https://github.com/DataSentics/p360-export/pull/29) by [@Vinsho](https://github.com/Vinsho).\n* :bug: Fixed Type Guesser bugs. PR [#28](https://github.com/DataSentics/p360-export/pull/28) by [@Vinsho](https://github.com/Vinsho).\n* :sparkles: Added Type Guesser. PR [#27](https://github.com/DataSentics/p360-export/pull/27) by [@Vinsho](https://github.com/Vinsho).\n* :building_construction: Retrieval of redundant attributes removed. PR [#26](https://github.com/DataSentics/p360-export/pull/26) by [@matejoravec](https://github.com/matejoravec).\n* :sparkles: SFMC Exporter: Enable field updating. PR [#23](https://github.com/DataSentics/p360-export/pull/23) by [@Vinsho](https://github.com/Vinsho).\n* :construction_worker: Build & Release Pipeline outsourced. PR [#25](https://github.com/DataSentics/p360-export/pull/25) by [@matejoravec](https://github.com/matejoravec).\n* :construction_worker: Latest changes action added. PR [#24](https://github.com/DataSentics/p360-export/pull/24) by [@matejoravec](https://github.com/matejoravec).\n",
     'author': 'Datasentics',
     'author_email': 'jiri.koutny@datasentics.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `p360-export-1.5.5/PKG-INFO` & `p360-export-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p360-export
-Version: 1.5.5
+Version: 1.5.6
 Summary: Persona360 data export
 License: Proprietary
 Author: Datasentics
 Author-email: jiri.koutny@datasentics.com
 Requires-Python: >=3.8.10,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,17 @@
 Description-Content-Type: text/markdown
 
 # p360-export
 
 Persona360 exporters.
 
 ### Latest Changes
+
+* :bookmark: Bump version to 1.5.6. PR [#93](https://github.com/DataSentics/p360-export/pull/93) by [@Vinsho](https://github.com/Vinsho).
+* :sparkles: Added new SFMC credential ftp_relative_path. PR [#92](https://github.com/DataSentics/p360-export/pull/92) by [@Vinsho](https://github.com/Vinsho).
 * :sparkles: Added Google Analytics 4 exporter. PR [#82](https://github.com/DataSentics/p360-export/pull/82) by [@guderkar](https://github.com/guderkar).
 #### 1.4.0
 * :construction_worker: Fixed release workflow PR [#81](https://github.com/DataSentics/p360-export/pull/81) by [@Vinsho](https://github.com/Vinsho).
 * :recycle: Typo fix. PR [#79](https://github.com/DataSentics/p360-export/pull/79) by [@Vinsho](https://github.com/Vinsho).
 * :sparkles: Fixed backward compatibility. PR [#77](https://github.com/DataSentics/p360-export/pull/77) by [@Vinsho](https://github.com/Vinsho).
 * :sparkles: Added logic for loading env specific config. PR [#76](https://github.com/DataSentics/p360-export/pull/76) by [@Vinsho](https://github.com/Vinsho).
 * :recycle: Odap integration. PR [#75](https://github.com/DataSentics/p360-export/pull/75) by [@Vinsho](https://github.com/Vinsho).
```

