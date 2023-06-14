# Comparing `tmp/steam-sdk-2023.6.8.tar.gz` & `tmp/steam-sdk-2023.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-sdk-2023.6.8.tar", last modified: Mon Jun  5 09:48:41 2023, max compression
+gzip compressed data, was "dist\steam-sdk-2023.6.9.tar", last modified: Mon Jun  5 15:06:57 2023, max compression
```

## Comparing `steam-sdk-2023.6.8.tar` & `steam-sdk-2023.6.9.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.359597 steam-sdk-2023.6.8/
--rw-rw-rw-   0        0        0      122 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1550 2023-06-05 09:48:41.356598 steam-sdk-2023.6.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-05 09:48:41.359597 steam-sdk-2023.6.8/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-06-05 09:44:36.000000 steam-sdk-2023.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.102840 steam-sdk-2023.6.8/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.111985 steam-sdk-2023.6.8/steam_sdk/analyses/
--rw-rw-rw-   0        0        0   125975 2023-06-05 09:01:13.000000 steam-sdk-2023.6.8/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.114149 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.118149 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23368 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.131271 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16757 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2800 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6828 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95412 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2652 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2341 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.133389 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22374 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.139389 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4527 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2921 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.141389 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29433 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.146735 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4704 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4852 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.149736 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.169253 steam-sdk-2023.6.8/steam_sdk/builders/
--rw-rw-rw-   0        0        0    12924 2023-05-12 15:08:26.000000 steam-sdk-2023.6.8/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   162736 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    35640 2023-06-05 07:40:24.000000 steam-sdk-2023.6.8/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    12076 2023-05-10 14:13:23.000000 steam-sdk-2023.6.8/steam_sdk/builders/BuilderSIGMA.py
--rw-rw-rw-   0        0        0    11689 2023-01-18 15:24:33.000000 steam-sdk-2023.6.8/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-19 08:13:58.000000 steam-sdk-2023.6.8/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.171252 steam-sdk-2023.6.8/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.172253 steam-sdk-2023.6.8/steam_sdk/configs/plotters/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/configs/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.174387 steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.176387 steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0    32991 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
--rw-rw-rw-   0        0        0     1426 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.178387 steam-sdk-2023.6.8/steam_sdk/cosims/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.218748 steam-sdk-2023.6.8/steam_sdk/data/
--rw-rw-rw-   0        0        0    10200 2023-05-12 13:31:31.000000 steam-sdk-2023.6.8/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0     7983 2023-05-22 11:27:05.000000 steam-sdk-2023.6.8/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0     3281 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2865 2023-04-24 12:48:33.000000 steam-sdk-2023.6.8/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     4193 2023-05-09 14:50:49.000000 steam-sdk-2023.6.8/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0    12762 2023-05-12 15:08:26.000000 steam-sdk-2023.6.8/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0    10823 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     4314 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5869 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    35376 2023-05-25 11:58:27.000000 steam-sdk-2023.6.8/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     2636 2023-05-09 14:50:49.000000 steam-sdk-2023.6.8/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataParsims.py
--rw-rw-rw-   0        0        0     1995 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2105 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     8068 2023-05-25 11:58:27.000000 steam-sdk-2023.6.8/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     6791 2023-05-09 14:51:04.000000 steam-sdk-2023.6.8/steam_sdk/data/DataSIGMA.py
--rw-rw-rw-   0        0        0     1650 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3204 2023-01-11 12:50:11.000000 steam-sdk-2023.6.8/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0    23052 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0    27819 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.235009 steam-sdk-2023.6.8/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3151 2022-12-19 08:13:58.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     2711 2022-12-19 08:13:58.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     1299 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3482 2022-12-19 08:13:58.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1924 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2062 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0     4959 2023-06-05 08:15:32.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverSIGMA.py
--rw-rw-rw-   0        0        0     1932 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.275081 steam-sdk-2023.6.8/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      317 2023-03-29 12:41:10.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0     2290 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1081 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6220 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     1650 2023-01-13 08:06:15.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     1030 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserDatToCsv.py
--rw-rw-rw-   0        0        0     8536 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2287 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0    48055 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    12436 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    10920 2023-05-12 13:31:31.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    63401 2023-06-01 14:44:35.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4780 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6838 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     2942 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserProtePyBBQ.py
--rw-rw-rw-   0        0        0   109575 2023-06-05 08:54:23.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0     1928 2023-05-09 14:51:03.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserSIGMA.py
--rw-rw-rw-   0        0        0    11707 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    55281 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     4088 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0      975 2023-06-02 08:04:34.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserYamlToRoxie.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0        2 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/dict_to_in.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.286223 steam-sdk-2023.6.8/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    61782 2023-05-23 14:30:59.000000 steam-sdk-2023.6.8/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0      916 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    72533 2023-05-17 07:23:09.000000 steam-sdk-2023.6.8/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    48206 2023-05-25 08:00:49.000000 steam-sdk-2023.6.8/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0     1972 2023-01-25 14:04:47.000000 steam-sdk-2023.6.8/steam_sdk/parsims/ParsimSweep.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.295355 steam-sdk-2023.6.8/steam_sdk/plotters/
--rw-rw-rw-   0        0        0     8053 2023-05-12 13:31:31.000000 steam-sdk-2023.6.8/steam_sdk/plotters/PlotterAnalysis.py
--rw-rw-rw-   0        0        0    20409 2023-06-05 09:18:18.000000 steam-sdk-2023.6.8/steam_sdk/plotters/PlotterMap2d.py
--rw-rw-rw-   0        0        0    39596 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2022-12-19 08:13:58.000000 steam-sdk-2023.6.8/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0     8863 2023-05-25 11:58:27.000000 steam-sdk-2023.6.8/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.297355 steam-sdk-2023.6.8/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0     5564 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.333167 steam-sdk-2023.6.8/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0    14942 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     4762 2023-06-02 08:04:34.000000 steam-sdk-2023.6.8/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2745 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0     3190 2023-06-05 08:54:23.000000 steam-sdk-2023.6.8/steam_sdk/utils/ParserRoxieHelpers.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0      686 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0     3837 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0      590 2023-05-09 14:50:57.000000 steam-sdk-2023.6.8/steam_sdk/utils/create_coordinate_file_SIGMA.py
--rw-rw-rw-   0        0        0     1279 2023-04-24 12:48:33.000000 steam-sdk-2023.6.8/steam_sdk/utils/get_attribute_type.py
--rw-rw-rw-   0        0        0      167 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0     4512 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0     1592 2023-04-24 12:48:33.000000 steam-sdk-2023.6.8/steam_sdk/utils/parse_str_to_list.py
--rw-rw-rw-   0        0        0      388 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-11 12:50:11.000000 steam-sdk-2023.6.8/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     7005 2023-05-11 09:21:50.000000 steam-sdk-2023.6.8/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.346467 steam-sdk-2023.6.8/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    35919 2023-03-23 12:53:02.000000 steam-sdk-2023.6.8/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0     6127 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/viewers/ViewerMeas.py
--rw-rw-rw-   0        0        0     1667 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/viewers/ViewerSim.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.350467 steam-sdk-2023.6.8/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.352467 steam-sdk-2023.6.8/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.353599 steam-sdk-2023.6.8/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.8/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.354599 steam-sdk-2023.6.8/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.8/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.8/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1834 2022-11-02 10:29:43.000000 steam-sdk-2023.6.8/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.108985 steam-sdk-2023.6.8/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     1550 2023-06-05 09:48:38.000000 steam-sdk-2023.6.8/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6763 2023-06-05 09:48:38.000000 steam-sdk-2023.6.8/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 09:48:38.000000 steam-sdk-2023.6.8/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1596 2023-06-05 09:48:38.000000 steam-sdk-2023.6.8/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-05 09:48:38.000000 steam-sdk-2023.6.8/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.804204 steam-sdk-2023.6.9/
+-rw-rw-rw-   0        0        0      122 2023-03-15 09:29:53.000000 steam-sdk-2023.6.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1550 2023-06-05 15:06:57.804204 steam-sdk-2023.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:06:57.804204 steam-sdk-2023.6.9/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-06-05 15:05:35.000000 steam-sdk-2023.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.585571 steam-sdk-2023.6.9/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.594720 steam-sdk-2023.6.9/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0   134224 2023-06-05 15:06:38.000000 steam-sdk-2023.6.9/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.595720 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.597863 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23368 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.609020 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16757 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2800 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6828 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95412 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2652 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2341 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.611020 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22374 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.618151 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4527 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2921 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.620151 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29433 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.625151 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4704 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4852 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.627257 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.641401 steam-sdk-2023.6.9/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    12924 2023-05-12 15:08:26.000000 steam-sdk-2023.6.9/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   162736 2023-05-25 11:58:42.000000 steam-sdk-2023.6.9/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    35640 2023-06-05 07:40:24.000000 steam-sdk-2023.6.9/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    12076 2023-05-10 14:13:23.000000 steam-sdk-2023.6.9/steam_sdk/builders/BuilderSIGMA.py
+-rw-rw-rw-   0        0        0    11689 2023-01-18 15:24:33.000000 steam-sdk-2023.6.9/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2022-12-19 08:13:58.000000 steam-sdk-2023.6.9/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2023-03-15 09:29:53.000000 steam-sdk-2023.6.9/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.642400 steam-sdk-2023.6.9/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.643400 steam-sdk-2023.6.9/steam_sdk/configs/plotters/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/configs/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.647522 steam-sdk-2023.6.9/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.649522 steam-sdk-2023.6.9/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0    32991 2023-05-25 11:58:42.000000 steam-sdk-2023.6.9/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
+-rw-rw-rw-   0        0        0     1426 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.651522 steam-sdk-2023.6.9/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.689010 steam-sdk-2023.6.9/steam_sdk/data/
+-rw-rw-rw-   0        0        0    10230 2023-06-05 15:06:38.000000 steam-sdk-2023.6.9/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0     7983 2023-05-22 11:27:05.000000 steam-sdk-2023.6.9/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0     3281 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2865 2023-04-24 12:48:33.000000 steam-sdk-2023.6.9/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     4193 2023-05-09 14:50:49.000000 steam-sdk-2023.6.9/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0    12762 2023-05-12 15:08:26.000000 steam-sdk-2023.6.9/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0    10823 2023-05-25 11:58:42.000000 steam-sdk-2023.6.9/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     4314 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5869 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    35376 2023-05-25 11:58:27.000000 steam-sdk-2023.6.9/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     2636 2023-05-09 14:50:49.000000 steam-sdk-2023.6.9/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/data/DataParsims.py
+-rw-rw-rw-   0        0        0     1995 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2105 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     8068 2023-05-25 11:58:27.000000 steam-sdk-2023.6.9/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     6791 2023-05-09 14:51:04.000000 steam-sdk-2023.6.9/steam_sdk/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0     1650 2023-03-15 09:29:53.000000 steam-sdk-2023.6.9/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3204 2023-01-11 12:50:11.000000 steam-sdk-2023.6.9/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0    23052 2023-05-25 11:58:42.000000 steam-sdk-2023.6.9/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0    27819 2023-05-25 11:58:42.000000 steam-sdk-2023.6.9/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.704131 steam-sdk-2023.6.9/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3151 2022-12-19 08:13:58.000000 steam-sdk-2023.6.9/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     2711 2022-12-19 08:13:58.000000 steam-sdk-2023.6.9/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     1299 2023-03-15 09:29:53.000000 steam-sdk-2023.6.9/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3482 2022-12-19 08:13:58.000000 steam-sdk-2023.6.9/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1924 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2062 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0     4916 2023-06-05 14:55:14.000000 steam-sdk-2023.6.9/steam_sdk/drivers/DriverSIGMA.py
+-rw-rw-rw-   0        0        0     1932 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.739807 steam-sdk-2023.6.9/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      317 2023-03-29 12:41:10.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0     2290 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1081 2023-05-25 11:58:42.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6220 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     1650 2023-01-13 08:06:15.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     1030 2023-03-15 09:29:53.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserDatToCsv.py
+-rw-rw-rw-   0        0        0     8536 2023-03-15 09:29:53.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2287 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0    48055 2023-05-25 11:58:42.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    12436 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    10920 2023-05-12 13:31:31.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    63813 2023-06-05 15:06:38.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4780 2023-03-15 09:29:53.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6838 2023-03-15 09:29:53.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     2942 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserProtePyBBQ.py
+-rw-rw-rw-   0        0        0   106285 2023-06-05 15:06:39.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0     1928 2023-05-09 14:51:03.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserSIGMA.py
+-rw-rw-rw-   0        0        0    11707 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    55281 2023-03-15 09:29:53.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     4088 2023-03-15 09:29:53.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0      975 2023-06-02 08:04:34.000000 steam-sdk-2023.6.9/steam_sdk/parsers/ParserYamlToRoxie.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0        2 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/parsers/dict_to_in.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.748926 steam-sdk-2023.6.9/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    61782 2023-05-23 14:30:59.000000 steam-sdk-2023.6.9/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0      916 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    82020 2023-06-05 15:06:38.000000 steam-sdk-2023.6.9/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    48206 2023-05-25 08:00:49.000000 steam-sdk-2023.6.9/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0     1972 2023-01-25 14:04:47.000000 steam-sdk-2023.6.9/steam_sdk/parsims/ParsimSweep.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.758064 steam-sdk-2023.6.9/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0     8053 2023-05-12 13:31:31.000000 steam-sdk-2023.6.9/steam_sdk/plotters/PlotterAnalysis.py
+-rw-rw-rw-   0        0        0    20409 2023-06-05 09:18:18.000000 steam-sdk-2023.6.9/steam_sdk/plotters/PlotterMap2d.py
+-rw-rw-rw-   0        0        0    39596 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2022-12-19 08:13:58.000000 steam-sdk-2023.6.9/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0     8863 2023-05-25 11:58:27.000000 steam-sdk-2023.6.9/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.760064 steam-sdk-2023.6.9/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0     5564 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.791012 steam-sdk-2023.6.9/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2023-03-15 09:29:53.000000 steam-sdk-2023.6.9/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0    14942 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     4762 2023-06-05 15:06:39.000000 steam-sdk-2023.6.9/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2745 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0     3037 2023-06-05 15:06:39.000000 steam-sdk-2023.6.9/steam_sdk/utils/ParserRoxieHelpers.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0      686 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0     3837 2023-03-15 09:29:53.000000 steam-sdk-2023.6.9/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0      590 2023-05-09 14:50:57.000000 steam-sdk-2023.6.9/steam_sdk/utils/create_coordinate_file_SIGMA.py
+-rw-rw-rw-   0        0        0     1279 2023-04-24 12:48:33.000000 steam-sdk-2023.6.9/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     1592 2023-04-24 12:48:33.000000 steam-sdk-2023.6.9/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0      388 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2023-01-11 12:50:11.000000 steam-sdk-2023.6.9/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     7005 2023-05-11 09:21:50.000000 steam-sdk-2023.6.9/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.796013 steam-sdk-2023.6.9/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    35919 2023-03-23 12:53:02.000000 steam-sdk-2023.6.9/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0     6127 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/viewers/ViewerMeas.py
+-rw-rw-rw-   0        0        0     1667 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/viewers/ViewerSim.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.799205 steam-sdk-2023.6.9/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.9/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.800205 steam-sdk-2023.6.9/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.801205 steam-sdk-2023.6.9/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.9/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.802204 steam-sdk-2023.6.9/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.9/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.9/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1834 2022-11-02 10:29:43.000000 steam-sdk-2023.6.9/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:06:57.591720 steam-sdk-2023.6.9/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1550 2023-06-05 15:06:55.000000 steam-sdk-2023.6.9/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6763 2023-06-05 15:06:55.000000 steam-sdk-2023.6.9/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:06:55.000000 steam-sdk-2023.6.9/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1596 2023-06-05 15:06:55.000000 steam-sdk-2023.6.9/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-05 15:06:55.000000 steam-sdk-2023.6.9/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam-sdk-2023.6.8/PKG-INFO` & `steam-sdk-2023.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.6.8
+Version: 2023.6.9
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: API,CERN,STEAM,SDK
+Keywords: CERN,STEAM,API,SDK
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.6.8/setup.py` & `steam-sdk-2023.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-sdk',
-    version="2023.6.8",
+    version="2023.6.9",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={'STEAM', 'API', 'SDK', 'CERN'},
```

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/AnalysisSTEAM.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 12% similar despite different names*

```diff
@@ -1435,26 +1435,31 @@
             # Read input file and run the ParsimEvent analysis
             pec = ParsimEventCircuit(ref_model=self.list_models[model_name], verbose=verbose)
             pec.read_from_input(path_input_file=input_file, flag_append=False)
             pec.write_event_file(simulation_name=simulation_name, simulation_numbers=simulation_numbers,
                                  path_outputfile_event_csv=path_output_event_csv)
 
             quenching_magnet_list = []  # required for families where multiple magnets can quench like RB
-
+            quenching_magnet_time = []
+            quenching_current_list = []
             for event_number in range(len(pec.list_events)):  # reading through each row of the event file
                 # get circuit specific information
                 circuit_name = pec.list_events[event_number].GeneralParameters.name
                 circuit_family_name = self.__get_circuit_family_name(circuit_name)
                 magnet_name = self.__get_magnet_name(circuit_name)
                 circuit_type = self.__get_circuit_type(circuit_name)
                 number_of_magnets = self.__get_number_of_magnets(circuit_name)
                 number_of_apertures = self.__get_number_of_apertures(circuit_name)
-                current_level = pec.list_events[event_number].PoweredCircuits[circuit_name].current_at_discharge
+                if circuit_family_name == "RB":
+                    current_level = pec.list_events[event_number].QuenchEvents[circuit_name].current_at_quench
+                    t_PC_off = pec.list_events[0].PoweredCircuits[circuit_name].delta_t_FGC_PIC
+                else:
+                    current_level = pec.list_events[event_number].PoweredCircuits[circuit_name].current_at_discharge
+                    t_PC_off = pec.list_events[event_number].PoweredCircuits[circuit_name].delta_t_FGC_PIC
                 magnets_list = self.__get_magnets_list(number_of_magnets)
-                t_PC_off = pec.list_events[event_number].PoweredCircuits[circuit_name].delta_t_FGC_PIC
                 magnet_types = self.__get_magnet_types_list(number_of_magnets)
 
                 # load circuit parameters step
                 if circuit_family_name == "RQ":
                     circuit_name_1 = circuit_name.replace(".", "D_")
                     circuit_name_2 = circuit_name.replace(".", "F_")
                     load_circuit_parameters_step_1 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_1)
@@ -1465,95 +1470,129 @@
                     modify_model_diode_step = ModifyModel(type='ModifyModel', model_name=model_name, variable_to_change=f'Netlist.x_D{quenching_magnet[0]}.value', variable_value=["RQ_Protection_Diode"], simulation_numbers=[], simulation_name=simulation_name, software=software)
                 elif circuit_type == "RCBX":
                     circuit_name_1 = circuit_name.replace("X", "XH")
                     circuit_name_2 = circuit_name.replace("X", "XV")
                     load_circuit_parameters_step_1 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_1)
                     load_circuit_parameters_step_2 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_2)
                 elif circuit_type in ["RCD", "RCO"]:
-                    parts = circuit_name.split("-")
-                    last_part = parts[-1]
-                    string1 = parts[0] + "." + last_part.split(".")[1]
-                    string2 = last_part
+                    if "-" in circuit_name:
+                        parts = circuit_name.split("-")
+                        last_part = parts[-1]
+                        string1 = parts[0] + "." + last_part.split(".")[1]
+                        string2 = last_part
+                    elif "." in circuit_name:
+                        string1 = circuit_name.replace(".", "D.", 1)
+                        string2 = circuit_name.replace(".", "O.", 1)
                     if circuit_type == "RCD":
                         load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=string1)
                     else:
                         load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=string2)
+                elif circuit_family_name == "RB":
+                    if event_number == len(pec.list_events) - 1:
+                        load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name)
                 else:
                     load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name)
 
                 # choosing stimulus output file location
                 if circuit_family_name == "IPD":
                     stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_family_name}', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
                 elif circuit_family_name == "RQ":
-                    stimulus_output_file_1 = os.path.join(default_keys.path_output, f'{circuit_type}_47magnets', f'{event_number + 1}', 'coil_resistances.stl')
-                    stimulus_output_file_2 = os.path.join(default_keys.path_output, f'{circuit_type}_47magnets',f'{event_number + 2}', 'coil_resistances.stl')
+                    stimulus_output_file_1 = os.path.join(default_keys.path_output, f'{circuit_type}', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
+                    stimulus_output_file_2 = os.path.join(default_keys.path_output, f'{circuit_type}', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[1]}", 'coil_resistances.stl')
                 elif circuit_type == "RCBX":
-                    stimulus_output_file_1 = os.path.join(default_keys.path_output, 'RCBX', f'{event_number + 1}', 'coil_resistances.stl')
-                    stimulus_output_file_2 = os.path.join(default_keys.path_output, 'RCBX', f'{event_number + 2}', 'coil_resistances.stl')
+                    stimulus_output_file_1 = os.path.join(default_keys.path_output, 'RCBX', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
+                    stimulus_output_file_2 = os.path.join(default_keys.path_output, 'RCBX', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[1]}", 'coil_resistances.stl')
                 elif simulation_name.startswith("IPQ"):
-                    stimulus_output_file = os.path.join(default_keys.path_output, f'{simulation_name}', f'{event_number + 1}', 'coil_resistances.stl')
+                    stimulus_output_file = os.path.join(default_keys.path_output, f'{simulation_name}', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
                 elif circuit_name.startswith("RCBY"):
                     stimulus_output_file = os.path.join(default_keys.path_output, 'RCBY', f'{event_number + 1}', 'coil_resistances.stl')
                 elif circuit_name.startswith(("RCBH", "RCBV")):
                     stimulus_output_file = os.path.join(default_keys.path_output, 'RCB', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
+                elif circuit_type == "RB":
+                    if event_number == len(pec.list_events) - 1:
+                        stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_type}', str(default_keys.file_counter), 'coil_resistances.stl')
+                elif circuit_name.startswith("RQS.A"):
+                    stimulus_output_file = os.path.join(default_keys.path_output, 'RQS_AxxBx', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
+                elif circuit_name.startswith(("RQS.R", "RQS.L")):
+                    stimulus_output_file = os.path.join(default_keys.path_output, 'RQS_R_LxBx', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
                 else:
                     stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_type}', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
 
                 # making appropriate directory if it doesn't exist for the stimulus output file
                 if circuit_family_name == "RQ" or circuit_type == "RCBX":
                     for file_path in [stimulus_output_file_1, stimulus_output_file_2]:
                         directory = os.path.dirname(file_path)
                         if not os.path.exists(directory):
                             os.makedirs(directory)
                 else:
-                    directory = os.path.dirname(stimulus_output_file)
-                    if not os.path.exists(directory):
-                        os.makedirs(directory)
+                    if circuit_family_name == "RB":
+                        if event_number == len(pec.list_events) - 1:
+                            directory = os.path.dirname(stimulus_output_file)
+                            if not os.path.exists(directory):
+                                os.makedirs(directory)
+                    else:
+                        directory = os.path.dirname(stimulus_output_file)
+                        if not os.path.exists(directory):
+                            os.makedirs(directory)
 
                 # write stimulus file step
                 if circuit_family_name == "RQ":
-                    write_stimuli_file_step_1 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_1, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=quenching_magnet, t_offset=[t_PC_off[0]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
-                    write_stimuli_file_step_2 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_2, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=quenching_magnet, t_offset=[t_PC_off[1]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step_1 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_1, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=quenching_magnet, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step_2 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_2, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=quenching_magnet, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_type == "RCBX":
-                    write_stimuli_file_step_1 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_1, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=magnets_list, t_offset=[t_PC_off[0]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
-                    write_stimuli_file_step_2 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_2, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=magnets_list, t_offset=[t_PC_off[1]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step_1 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_1, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level[0])], magnets=magnets_list, t_offset=[t_PC_off[0]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step_2 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_2, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level[1])], magnets=magnets_list, t_offset=[t_PC_off[1]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_family_name == "RQX":
                     current_level = [current_level[0]+current_level[1], current_level[0]+current_level[2], current_level[0]+current_level[2], current_level[0]]
                     write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=current_level, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_family_name == "IPQ" and number_of_magnets == 2:
                     write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=current_level, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_family_name == "IPQ" and number_of_magnets == 1:
                     write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
-                elif circuit_type in ["RCS", "ROD", "ROF", "RQ6", "RSD", "RSF", "RQTL9", "RQTD", "RQTF"]:
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                elif circuit_type in ["RCS", "RO_13magnets", "RO_8magnets", "RSD_12magnets", "RSD_11magnets", "RSF_10magnets", "RSF_9magnets", "RQTL9", "RQT"] or (circuit_type == "RQ6" and circuit_family_name == "600A") or circuit_name.startswith("RQS.A"):
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level)]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                elif circuit_name.startswith(("RQS.R", "RQS.L", "RSS")):
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level)]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_type == "RB":
                     position = pec.list_events[event_number].QuenchEvents[circuit_name].magnet_electrical_position
                     quenching_magnet = [self.__get_quenching_magnet_number(position, circuit_family_name)]
                     quenching_magnet_list.append(quenching_magnet[0])
-                    quenching_magnet_list.sort()
+                    quenching_magnet_time.append(pec.list_events[event_number].QuenchEvents[circuit_name].delta_t_iQPS_PIC)
+                    quenching_current_list.append(current_level)
                     # modify model diode step used to change diodes across the quenching magnets with heating
                     modify_model_diode_step = ModifyModel(type='ModifyModel', model_name=model_name, variable_to_change=f'Netlist.x_D{quenching_magnet[0]}.value', variable_value=["RB_Protection_Diode"], simulation_numbers=[], simulation_name=simulation_name, software=software)
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level]*(event_number + 1), magnets=quenching_magnet_list, t_offset=[t_PC_off]*(event_number + 1), interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    if event_number == len(pec.list_events) - 1:
+                        zipped_lists = zip(quenching_magnet_list, quenching_magnet_time, quenching_current_list)
+                        sorted_lists = sorted(zipped_lists, key=lambda x: x[0])
+                        quenching_magnet_list, quenching_magnet_time, quenching_current_list = zip(*sorted_lists)
+                        write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=quenching_current_list, magnets=quenching_magnet_list, t_offset=quenching_magnet_time, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_type == "RCD":
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[1]]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level[1])]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_type == "RCO":
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level[0])]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 else:
                     write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level)], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
 
                 # parsim sweep step with newly created event file
                 if circuit_family_name == "RQ" or circuit_type == "RCBX":
                     output_files = self.__split_csv(path_output_event_csv)
                     parsim_sweep_step_1 = ParametricSweep(type='ParametricSweep', input_sweep_file=output_files[0],
                                                         model_name=model_name, case_model=case_model, software=software, verbose=verbose)
                     parsim_sweep_step_2 = ParametricSweep(type='ParametricSweep', input_sweep_file=output_files[1],
                                                         model_name=model_name, case_model=case_model, software=software, verbose=verbose)
                 else:
-                    parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_event_csv,
-                                                        model_name=model_name, case_model=case_model, software=software, verbose=verbose)
+                    if circuit_family_name == "RB":
+                        if event_number == len(pec.list_events) - 1:
+                            parsim_sweep_step = ParametricSweep(type='ParametricSweep',
+                                                                input_sweep_file=path_output_event_csv,
+                                                                model_name=model_name, case_model=case_model,
+                                                                software=software, verbose=verbose)
+                    else:
+                        parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_event_csv,
+                                                            model_name=model_name, case_model=case_model, software=software, verbose=verbose)
 
                 # run all the steps together
                 if circuit_family_name == "RQ":
                     self.load_circuit_parameters(load_circuit_parameters_step_1, verbose=verbose)
                     self.write_stimuli_from_interpolation(write_stimuli_file_step_1, verbose=verbose)
                     self.step_modify_model(modify_model_diode_step, verbose=verbose)
                     self.run_parsim_sweep(parsim_sweep_step_1, verbose=verbose)
@@ -1813,17 +1852,17 @@
     def __get_circuit_family_name(self, circuit_name: str):
         if circuit_name.startswith("RCBH") or circuit_name.startswith("RCBV"):
             return "60A"
         elif circuit_name.startswith("RD"):
             return "IPD"
         elif circuit_name.startswith("RQX"):
             return "RQX"
-        elif circuit_name.startswith(("RQ4", "RQ5", "RQ6", "RQ7", "RQ8", "RQ9", "RQ10")):
+        elif circuit_name.startswith(("RQ4", "RQ5", "RQ7", "RQ8", "RQ9", "RQ10")) or (circuit_name.startswith("RQ6.") and len(circuit_name) == 6):
             return "IPQ"
-        elif circuit_name.startswith(("RQT12", "RQT13", "RQS", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RCBX", "RQSX3", "RCS", "ROD", "ROF", "RQ6", "RSD", "RSF", "RQTL9", "RQTD", "RQTF", "RCD", "RCO")):
+        elif circuit_name.startswith(("RQT12", "RQT13", "RQS", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RCBX", "RQSX3", "RCS", "ROD", "ROF", "RSD", "RSF", "RQTL9", "RQTD", "RQTF", "RCD", "RCO", "RC.")) or (circuit_name.startswith("RQ6.") and len(circuit_name) == 8):
             return "600A"
         elif circuit_name.startswith("RQ"):
             return "RQ"
         elif circuit_name.startswith(("RCBY", "RCBC", "RCTX")):
             return "80-120A"
         elif circuit_name.startswith("RB"):
             return "RB"
@@ -1834,49 +1873,75 @@
             return "MCBH"
         elif circuit_name.startswith("RD"):
             circuit_type = self.__get_circuit_type(circuit_name)
             magnet_dict = {"RD1": "MBX", "RD2": "MBRC", "RD3": "MBRS", "RD4": "MBRB"}
             return magnet_dict.get(circuit_type, "")
         elif circuit_name.startswith("RQX"):
             return ["MQXA", "MQXB"]
-        elif circuit_name.startswith(("RQ4", "RQ5", "RQ6", "RQ7", "RQ8", "RQ9", "RQ10")):
+        elif circuit_name.startswith(("RQ4", "RQ5", "RQ7", "RQ8", "RQ9", "RQ10")) or (circuit_name.startswith("RQ6.") and len(circuit_name) == 6):
             magnet_dict = {"IPQ_RQ4_2_2xRPHH_2xMQY": "MQY", "IPQ_RQ4_4_2xRPHH_4xMQY": ["MQY", "MQY"], "IPQ_RQ5_2_2xRPHGB_2xMQML": "MQML", "IPQ_RQ5_2_2xRPHH_2xMQY": "MQY", "IPQ_RQ5_4_2xRPHGB_4xMQM": ["MQM", "MQM"], "IPQ_RQ5_4_2xRPHH_4xMQY": ["MQY", "MQY"], "IPQ_RQ6_2_2xRPHGB_2xMQML": "MQML", "IPQ_RQ6_2_2xRPHGB_2xMQY": "MQY", "IPQ_RQ6_4_2xRPHGB_2xMQM_2xMQML": ["MQM", "MQML"], "IPQ_RQ7_2_2xRPHGA_2xMQM": "MQM", "IPQ_RQ7_4_2xRPHGA_4xMQM": ["MQM", "MQM"], "IPQ_RQ8_2_2xRPHGA_2xMQML": "MQML", "IPQ_RQ9_4_2xRPHGA_2xMQM_2xMQMC": ["MQM", "MQMC"], "IPQ_RQ10_2_2xRPHGA_2xMQML": "MQML"}
             return magnet_dict.get(self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name, "")
+        elif circuit_name.startswith("RQ6.") and len(circuit_name) == 8:
+            return ["MQTLH", "MQTLH_quenchback"]
+        elif circuit_name.startswith(("RQTL7", "RQTL8", "RQTL10", "RQTL11")):
+            return "MQTLI"
+        elif circuit_name.startswith("RQTL9"):
+            return ["MQTLI", "MQTLI_quenchback"]
+        elif circuit_name.startswith("RQSX3"):
+            return "MQSX"
+        elif circuit_name.startswith("RQS"):
+            return ["MQS", "MQS_quenchback"]
+        elif circuit_name.startswith(("RQT12", "RQT13")):
+            return "MQT"
+        elif circuit_name.startswith(("RQTD", "RQTF")):
+            return ["MQT", "MQT_quenchback"]
         elif circuit_name.startswith("RQ"):
             return "MQ"
         elif circuit_name.startswith("RCBY"):
             return "MCBYH"
         elif circuit_name.startswith("RCBC"):
             return "MCBCH"
-        elif circuit_name.startswith("RQT12"):
-            return "MQT"
         elif circuit_name.startswith("RCS"):
             return ["MCS", "MCS_quenchback"]
         elif circuit_name.startswith("RB"):
             return "MB"
         elif circuit_name.startswith("RCBX"):
             return ["MCBXH", "MCBXV"]
+        elif circuit_name.startswith("RSS"):
+            return ["MSS", "MSS_quenchback"]
+        elif circuit_name.startswith(("ROD", "ROF")):
+            return ["MO", "MO_quenchback"]
+        elif circuit_name.startswith(("RSD", "RSF")):
+            return ["MS", "MS_quenchback"]
         elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name == "RCD":
             return ["MCD", "MCD_quenchback"]
         elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name == "RCO":
             return ["MCO", "MCO_quenchback"]
 
     def __get_number_of_magnets(self, circuit_name: str):
         circuit_family_name = self.__get_circuit_family_name(circuit_name)
         circuit_type = self.__get_circuit_type(circuit_name)
         if circuit_type in ["RCS", "RB"]:
             return 154
         elif circuit_type in ["RCD", "RCO"]:
             return 77
+        elif circuit_name.startswith("RQ6.") and len(circuit_name) == 8:
+            return 6
+        elif circuit_name.startswith(("RQS.R", "RQS.L", "RQTL9")):
+            return 2
+        elif circuit_name.startswith(("RQS.A", "RSS", "RQX")):
+            return 4
+        elif circuit_name.startswith(("RQTD", "RQTF")):
+            return 8
         elif circuit_family_name in ["60A", "IPD", "80-120A", "600A"]:
             return 1
-        elif circuit_family_name == "RQ":
-            return 47  # deal with 51 later
-        elif circuit_family_name == "RQX":
-            return 4
+        elif circuit_type == "RQ_47magnets":
+            return 47
+        elif circuit_type == "RQ_51magnets":
+            return 51
         elif circuit_family_name == "IPQ":
             return int(int(re.search(r'_(\d+)_', self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name).group(1))/2)
 
     def __get_number_of_apertures(self, circuit_name: str):
         circuit_family_name = self.__get_circuit_family_name(circuit_name)
         if circuit_family_name in ["IPQ", "RB"]:
             return 2
@@ -1887,22 +1952,22 @@
         list = []
         for i in range(1, number_of_magnets+1):
             list.append(i)
         return list
 
     def __get_magnet_types_list(self, number_of_magnets: int):
         list = []
-        if number_of_magnets == 4: #to be improved
+        if number_of_magnets == 4 and self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name.startswith("RQX"): #to be improved
             list = [1, 2, 2, 1]
         elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name.startswith("IPQ") and number_of_magnets == 2:
             list = [1, 2]
         elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name.startswith("RB"):
             for i in range(1, number_of_magnets+1):
                 list.append(1)
-        elif number_of_magnets in [154, 13, 8, 77, 6, 12, 11, 10, 9]:
+        elif number_of_magnets in [154, 13, 8, 77, 6, 12, 11, 10, 9, 4, 2]:
             list = [1] + [2] * (number_of_magnets - 1)
         else:
             for i in range(1, number_of_magnets+1):
                 list.append(1)
         return list
 
     def __get_circuit_type(self, circuit_name: str):
@@ -1910,28 +1975,53 @@
             return "RCB"
         elif circuit_name.startswith(("RD1", "RD2", "RD3", "RD4")):
             return {"RD1": "RD1", "RD2": "RD2", "RD3": "RD3", "RD4": "RD4"}.get(circuit_name[:3], "No match found")
         elif circuit_name.startswith("RQX"):
             return "RQX"
         elif circuit_name.startswith(("RQ4", "RQ5", "RQ6", "RQ7", "RQ8", "RQ9", "RQ10")):
             return circuit_name.split(".")[0]
-        elif circuit_name.startswith("RQT12"):
-            return "RQT12"
-        elif circuit_name.startswith("RQ"):
-            return "RQ"
+        elif circuit_name.startswith(("RQT12", "RQT13")):
+            return "RQT_12_13"
+        elif circuit_name.startswith(("RQTL7", "RQTL8", "RQTL10", "RQTL11")):
+            return "RQTL_7_8_10_11"
+        elif circuit_name.startswith("RQTL9"):
+            return "RQTL9"
+        elif circuit_name.startswith(("RQTD", "RQTF")):
+            return "RQT"
+        elif circuit_name.startswith("RQSX3"):
+            return "RQSX3"
+        elif circuit_name.startswith("RQS"):
+            return "RQS"
+        elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name == "RQ_47magnets":
+            return "RQ_47magnets"
+        elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name == "RQ_51magnets":
+            return "RQ_51magnets"
         elif circuit_name.startswith("RCS"):
             return "RCS"
         elif circuit_name.startswith("RB"):
             return "RB"
         elif circuit_name.startswith("RCBX"):
             return "RCBX"
         elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name == "RCD":
             return "RCD"
         elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name == "RCO":
             return "RCO"
+        elif circuit_name.startswith("RCBC"):
+            return "RCBC"
+        elif circuit_name.startswith("RSS"):
+            return "RSS"
+        elif circuit_name.startswith(("RSD")):
+            magnet_number = self.__find_magnets(os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/600A_circuit_parameters.csv"), circuit_name)
+            return f"RSD_{magnet_number}magnets"
+        elif circuit_name.startswith(("RSF")):
+            magnet_number = self.__find_magnets(os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/600A_circuit_parameters.csv"), circuit_name)
+            return f"RSF_{magnet_number}magnets"
+        elif circuit_name.startswith(("RO")):
+            magnet_number = self.__find_magnets(os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/600A_circuit_parameters.csv"), circuit_name)
+            return f"RO_{magnet_number}magnets"
 
     def __get_quenching_magnet_number(self, position: str, circuit_family_name: str):
         df = pd.read_csv(os.path.join(f"../../tests/analyses/input/run_parsim_event_circuit/{circuit_family_name}_LayoutDetails.csv"))
         mask = df['Magnet'].str.split('.').str[1] == position
         result = df.loc[mask, '#Electric_circuit'].iloc[0]
         return result
 
@@ -1967,12 +2057,28 @@
             writer_even = csv.writer(output_even_file)
             writer_even.writerow(header)
             writer_even.writerows(even_rows)
 
         # Return a list of the output file names
         return [output_even_file_name, output_odd_file_name]
 
+    def __find_magnets(self, filename, key):
+        with open(filename, 'r') as file:
+            reader = csv.DictReader(file)
+            for row in reader:
+                if row['circuit'] == key:
+                    return row['NumberOfMagnets']
+            return None
+
+    def __find_circuit_model(self, filename, key):
+        with open(filename, 'r') as file:
+            reader = csv.DictReader(file)
+            for row in reader:
+                if row['circuit'] == key:
+                    return row['circuit_type']
+            return None
+
```

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam-sdk-2023.6.9/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/builders/BuilderFiQuS.py` & `steam-sdk-2023.6.9/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/builders/BuilderLEDET.py` & `steam-sdk-2023.6.9/steam_sdk/builders/BuilderLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/builders/BuilderModel.py` & `steam-sdk-2023.6.9/steam_sdk/builders/BuilderModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/builders/BuilderProteCCT.py` & `steam-sdk-2023.6.9/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/builders/BuilderPyBBQ.py` & `steam-sdk-2023.6.9/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/builders/BuilderSIGMA.py` & `steam-sdk-2023.6.9/steam_sdk/builders/BuilderSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam-sdk-2023.6.9/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/builders/Solenoids.py` & `steam-sdk-2023.6.9/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/builders/geometricFunctions.py` & `steam-sdk-2023.6.9/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx` & `steam-sdk-2023.6.9/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam-sdk-2023.6.9/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataAnalysis.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataAnalysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,14 +217,15 @@
     """
     local_LEDET_folder: str = None
     path_config_file: str = None
     default_configs: List[str] = []
     path_tdms_files: str = None
     path_output_measurement_files: str = None
     path_output: str = None
+    file_counter: int = None
 
 
 class ParsimEvent(BaseModel):
     """
         Level 2: Analysis step to write stimulus file from coil resistance csv file
     """
     type: Literal['ParsimEvent']
```

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataConductor.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataDakota.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataEventCircuit.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataEventMagnet.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataFiQuS.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataLEDET.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataModelCircuit.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataModelCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataModelConductor.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataModelMagnet.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataModelMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataParsimConductor.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataProteCCT.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataPyBBQ.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataRoxieParser.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataSIGMA.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataSettings.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataSettings.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DataSignal.py` & `steam-sdk-2023.6.9/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DictionaryLEDET.py` & `steam-sdk-2023.6.9/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DictionaryProteCCT.py` & `steam-sdk-2023.6.9/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/DictionaryPyBBQ.py` & `steam-sdk-2023.6.9/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/TemplateLEDET.py` & `steam-sdk-2023.6.9/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/data/TemplateProteCCT.py` & `steam-sdk-2023.6.9/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/drivers/DriverAnalysis.py` & `steam-sdk-2023.6.9/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/drivers/DriverDakota.py` & `steam-sdk-2023.6.9/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/drivers/DriverFiQuS.py` & `steam-sdk-2023.6.9/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/drivers/DriverLEDET.py` & `steam-sdk-2023.6.9/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/drivers/DriverPSPICE.py` & `steam-sdk-2023.6.9/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/drivers/DriverProteCCT.py` & `steam-sdk-2023.6.9/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/drivers/DriverPyBBQ.py` & `steam-sdk-2023.6.9/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/drivers/DriverSIGMA.py` & `steam-sdk-2023.6.9/steam_sdk/drivers/DriverSIGMA.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,44 +61,43 @@
         print(f"Using {bh_curve_database} as bh file path")
         print(f"Using {path_to_results} as path to results")
 
         # Call mainSIGMA which generates the Java files.
         self.MainSIGMA(input_file_path=input_file_path, model_folder=model_folder,
                        system_settings=self.system_settings, bh_curve_database=bh_curve_database,
                        input_coordinates_path=input_coordinates_path,path_to_results=path_to_results)
-        # Change folder to execute bat file
-        os.chdir(model_folder)
         batch_file_path = os.path.join(model_folder, f"{simulation_name}_Model_Compile_and_Open.bat")
         print(f'Running Comsol model via: {batch_file_path}')
 
         # This code is to run the process and logging the output. If you want to see the process real time in the
         # terminal you can comment out this code and run
         # subprocess.call(batch_file_path) instead.
         # -------------------------------------------------------------------------------------------------------------
         proc = subprocess.Popen([batch_file_path], stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                 universal_newlines=True)
         (stdout, stderr) = proc.communicate()
 
         log_file_path = os.path.join(path_to_results, "log_bat_file.txt")
-
+        error = False
         if proc.returncode != 0:
             print(stderr)
             raise ValueError(f"Batch file throws an error, COMSOL model could not be completed! Review error at {log_file_path}.")
         else:
             print(stdout)
             for line in stdout.split('\n'):
                 if "error" in line.lower():
-                    raise ValueError(
-                        f"Batch file throws an error, COMSOL model could not be completed! Review log at {log_file_path}.")
+                    error=True
 
-            print(f"Running batch file passes! See log file at {log_file_path}.")
 
         with open(log_file_path, 'w') as logfile:
             logfile.write(stdout)
-        # -------------------------------------------------------------------------------------------------------------
-
-        # Return to recovery path
         os.chdir(current_path)
+        if error:
+            raise ValueError(
+                f"Batch file throws an error, COMSOL model could not be completed! Review log at {log_file_path}.")
+        else:
+            print(f"Running batch file passes! See log file at {log_file_path}.")
 
+        # -------------------------------------------------------------------------------------------------------------
```

### Comparing `steam-sdk-2023.6.8/steam_sdk/drivers/DriverXYCE.py` & `steam-sdk-2023.6.9/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/CSD_Reader.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserCond2d.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserCsd.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserCsv.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserDakota.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserDatToCsv.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserDatToCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserExcel.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserFiQuS.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserLEDET.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserMap2d.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserMat.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserMat.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserPSPICE.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserPSPICE.py`

 * *Files 2% similar despite different names*

```diff
@@ -1047,19 +1047,27 @@
             for g in current_level_mag:
                 if n_apertures == 2:
                     [time, data_R1, data_R2] = InterpolateResistance(g, path_resources[magnet_type[k-1]-1], n_apertures=n_apertures, Type = InterpolationType)
                 else:
                     [time, data_R1] = InterpolateResistance(g, path_resources[magnet_type[k-1]-1], n_apertures=n_apertures, Type=InterpolationType)
                 if not R1.size > 0:
                     R1 = data_R1[np.newaxis, ...]
+                elif "IPQ" in Outputfile:
+                    if R1.size != data_R1.size:
+                        R1 = data_R1[np.newaxis, ...]
+                    R1 = np.vstack((R1, data_R1))
                 else:
                     R1 = np.vstack((R1, data_R1))
                 if n_apertures == 2:
                     if not R2.size > 0:
                         R2 = data_R2[np.newaxis, ...]
+                    elif "IPQ" in Outputfile:
+                        if R2.size != data_R2.size:
+                            R2 = data_R2[np.newaxis, ...]
+                        R2 = np.vstack((R2, data_R2))
                     else:
                         R2 = np.vstack((R2, data_R2))
 
             index = magnets.index(k)
             timeShift = tShift[index]
             if timeShift < 0: timeShift = 0
```

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserPdf.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserProteCCT.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserProtePyBBQ.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserProtePyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserRoxie.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserRoxie.py`

 * *Files 3% similar despite different names*

```diff
@@ -591,34 +591,36 @@
             elif keywords['trans']['key'] in row:
                 keywords['trans']['index'] = i
             elif keywords['block']['key'] in row:
                 keywords['block']['index'] = i
             else:
                 pass
 
+        self.symmetric_coil = True # Check if coil have symmetry
         for key in keywords:
             firstRow = fileContentByRow[keywords[key]['index']]
             nRowsParameters = int(firstRow[5:])
             if verbose:
                 print('{} definition parameters have {} row(s)'.format(key, nRowsParameters))
 
             # Separate part of the data with group definition information
             parameters = fileContentByRow[keywords[key]['index'] + 1:keywords[key]['index'] + 1 + nRowsParameters]
 
             if key == 'block':
                 self.layer_radius = list(set([float(row.split()[3]) for row in parameters]))
                 self.layer_radius.sort()
-
             # Assign parameters to a list of parameters objects
             for row in parameters:
                 rowSplitStr = row.split()
 
                 if key == 'group':
                     data.groups[rowSplitStr[0]] = pd.Group(symm=int(rowSplitStr[1]), typexy=int(rowSplitStr[2]),
                                                            blocks=list(map(int, rowSplitStr[3:-1])))
+                    if int(rowSplitStr[2]) == 0:
+                        self.symmetric_coil = False # If rows contains 0 then no symmetry - assumption but let's start from there
                 elif key == 'trans':
                     data.transs[rowSplitStr[0]] = pd.Trans(x=float(rowSplitStr[1]), y=float(rowSplitStr[2]),
                                                            alph=float(rowSplitStr[3]), bet=float(rowSplitStr[4]),
                                                            string=str(rowSplitStr[5]), act=int(rowSplitStr[6]),
                                                            bcs=list(map(int, rowSplitStr[7:-1])))
                     if data.transs[rowSplitStr[0]].string == 'SHIFT2':
                         self.shift_flag += 1
@@ -662,33 +664,38 @@
                                 raise Exception('The current block is not transformed or belongs to a group that is not'
                                                 'transformed: check "BCS" under "EULER" in the .data file.')
 
                     radius = float(rowSplitStr[3])
                     layer = self.layer_radius.index(radius) + 1
                     imag = int(rowSplitStr[10])
                     turn = float(rowSplitStr[11])
+                    current_sign = np.sign(float(rowSplitStr[6]))
                     if 'symm' in locals():
                         Avalue= turn * symm / 360 + 1
                         pole = floor(turn * symm / 360 + 1)
-                        # if imag==1 and turn ==0 or imag==0 and turn ==180:
-                        #     pole=2
-                        # else:
-                        #     pole = 1
+                        # How to fix this?
                     else:
                         pole = block_nr
 
+                    if self.symmetric_coil == False:
+                         if current_sign==-1:
+                            pole = 2
+                         else:
+                            pole = 1
+
                     data.blocks[rowSplitStr[0]] = pd.Block(type=int(rowSplitStr[1]), nco=int(rowSplitStr[2]),
                                                            radius=radius, phi=float(rowSplitStr[4]),
                                                            alpha=float(rowSplitStr[5]), current=float(rowSplitStr[6]),
                                                            condname=rowSplitStr[7], n1=int(rowSplitStr[8]),
                                                            n2=int(rowSplitStr[9]), imag=int(rowSplitStr[10]),
                                                            turn=turn, coil=coil, pole=pole, layer=layer,
                                                            winding=block_nr, shift2=pd.Coord(x=0., y=0.),
                                                            roll2=pd.Roll(coor=pd.Coord(x=0., y=0.), alph=0.))
-
+        if not self.symmetric_coil:
+            print("NO SYMMETRY")
         # Print each parameters object in the list
         if verbose:
             for no in data.groups:
                 arg = data.groups[no]  # group
                 print('Parameters of group {}: (symmetry type: {}, group type: {}, block list: {}).'
                       .format(int(no), arg.symm, arg.typexy, arg.blocks))
             for no in data.transs:
@@ -731,22 +738,23 @@
         # This index will increase with each added block
         nb = len(data)
 
         # Blocks to add to the attribute group.blocks
         blockToAddToGroup = []
 
         # Apply multipole geometry
+        self.windings=[]
         if self.group.typexy == 0:
             if verbose:
                 print('typexy = {}: No symmetry action.'.format(self.group.typexy)) ## Pull winding data from yaml files.
                 # here get the winding data from the yaml file. Overwrite the already defined windings in the data.
                 # Function is placed outside this file.
-            # path_model_data = "C:\\Users\\jlidholm\\cernbox\\Git-projects\\steam_sdk\\tests\\builders\\model_library\\magnets\\MED_C_COMB\\input\\modelData_MED_C_COMB.yaml"
-            # pyr = ParserYamlToRoxie(path_model_data)
-            # self.windings = pyr.read_model_data_yaml()
+            path_model_data = "C:\\Users\\jlidholm\\cernbox\\Git-projects\\steam_sdk\\tests\\builders\\model_library\\magnets\\MED_C_COMB\\input\\modelData_MED_C_COMB.yaml"
+            pyr = ParserYamlToRoxie(path_model_data)
+            self.windings = pyr.read_model_data_yaml()
         elif self.group.typexy == 1:
             if verbose:
                 print('typexy = {}: All.'.format(self.group.typexy))
 
             for additionalBlock in self.group.blocks:
                 nOriginalBlocks = nb
                 # idxBlock = additionalBlock - 1
@@ -1567,15 +1575,14 @@
             #     block.block_corners.iL = pd.Coord(x=sigDig(new_inner[0]), y=sigDig(new_inner[1]))
             #     block.block_corners.oL = pd.Coord(x=sigDig(new_outer[0]), y=sigDig(new_outer[1]))
             #     block.block_corners.iH = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))
             #     block.block_corners.oH = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))
 
         # ((block.pole % 2 == 0) * np.sign(-I[0]) +
         #  (block.pole % 2 != 0) * np.sign(I[0])) * block.radius / 1e3]
-
         return self.data.coil
 
     def getCablePositions(self, blocks: Dict[str, pd.Block] = None, cadata: pd.Cadata = None, verbose: bool = False):
         """
             **Returns insulated and bare conductor positions, and strand positions**
 
             Find insulated and bare conductor positions, and strand positions
@@ -1590,59 +1597,57 @@
             :return: list
         """
         blockTypes = {1: 'Cos-theta', 2: 'Block-coil'}
 
         if blocks:
             self.roxieData.coil.blocks = blocks
 
-        for no, blk in self.roxieData.coil.blocks.items():
-            self.data.coil.physical_order.append(pd.Order(coil=blk.coil, pole=blk.pole, layer=blk.layer,
-                                                          winding=blk.winding, block=int(no)))
+
 
         blk_layers = [[no, blk.layer] for no, blk in self.roxieData.coil.blocks.items()]
         blk_layers.sort(key=lambda x: x[1])
         # plt.figure(figsize=(10, 10))
         # self.ax = plt.axes()
         # self.ax.set_xlim(-0.2, 0.2)
         # self.ax.set_ylim(-0.2, 0.2)
         for pair in blk_layers:
             self.no = int(pair[0])
             self.block = self.roxieData.coil.blocks[pair[0]]
-            # # Double check that the winding is correct.
-            # index = None
-            # #self.block.pole = 1
-            #
-            # for i, sublist in enumerate(self.windings):
-            #     if self.no in sublist:
-            #         index = i
-            #         break
-            #
-            # if index is not None:
-            #     print(f"The block {self.no} is present at index {index+1}.")
-            #     self.block.winding = index + 1
-            #     self.roxieData.coil.blocks[str(self.no)].winding = self.block.winding
-            #
-            # else:
-            #     print(f"The block {self.no} is not present in the list.")
-            #
+            # Double check that the winding is correct.
+            index = None
+            #self.block.pole = 1
+
+            for i, sublist in enumerate(self.windings):
+                if self.no in sublist:
+                    index = i
+                    break
+
+            if index is not None:
+                print(f"The block {self.no} is present at index {index+1}.")
+                self.block.winding = index + 1
+                self.roxieData.coil.blocks[str(self.no)].winding = self.block.winding
+
+            else:
+                print(f"The block {self.no} is not present in the list.")
+
             # Get desired conductor data
             self.cond_name = self.block.condname
             self.getConductorFromCableDatabase(cadata=cadata)
 
             # Calculate x/y positions of the conductor corners and strands
             if verbose:
                 print('Block {} is of type {} --> {}.'.format(self.no, self.block.type, blockTypes[self.block.type]))
 
             self.findConductorPositions(verbose=verbose)
-        # for no, blk in self.roxieData.coil.blocks.items():
-        #     self.data.coil.physical_order.append(pd.Order(coil=blk.coil, pole=blk.pole, layer=blk.layer,
-        #                                                   winding=blk.winding, block=int(no)))
-        # # if verbose:
+        for no, blk in self.roxieData.coil.blocks.items():
+            self.data.coil.physical_order.append(pd.Order(coil=blk.coil, pole=blk.pole, layer=blk.layer,
+                                                          winding=blk.winding, block=int(no)))
+        # if verbose:
         #     print('Total number of conductors (half-turns): {}'.format(len(self.xPos)))
-        #plt.show()
+        # plt.show()
         return self.data.coil
 
     def getWedgePositions(self, coil: pd.CoilData = None, verbose: bool = False):
         """
             **Returns wedge positions**
 
             Find wedge positions
@@ -1654,74 +1659,74 @@
 
             :return: list
         """
         if coil:
             self.data = pd.RoxieData()
             self.data.coil = coil
 
-        # xPos = []
-        # yPos = []
-        # xBarePos = []
-        # yBarePos = []
-        # iPos = []
-        # xblockCorners = []
-        # yblockCorners = []
-        # colormap = cm.get_cmap('nipy_spectral')
-        # ht_coil = []
-        # block_coil = []
-
-        # for eo in self.data.coil.physical_order:
-        #     out = self.data.coil.coils[eo.coil].poles[eo.pole].layers[eo.layer].windings[eo.winding].blocks[eo.block]
-        #     winding = self.data.coil.coils[eo.coil].poles[eo.pole].layers[eo.layer].windings[eo.winding]
-        #     block = winding.blocks[eo.block]
-        #     xblockCorners.append([block.block_corners.iH.x, block.block_corners.oH.x, block.block_corners.oL.x,
-        #                           block.block_corners.iL.x])
-        #     yblockCorners.append([block.block_corners.iH.y, block.block_corners.oH.y, block.block_corners.oL.y,
-        #                           block.block_corners.iL.y])
-        #     block_coil.append(eo.coil)
-        #     # Save half turn corners
-        #     for halfTurn_nr, halfTurn in block.half_turns.items():
-        #         insu = halfTurn.corners.insulated
-        #         bare = halfTurn.corners.bare
-        #         xPos.append([insu.iH.x, insu.oH.x, insu.oL.x, insu.iL.x])
-        #         yPos.append([insu.iH.y, insu.oH.y, insu.oL.y, insu.iL.y])
-        #         xBarePos.append([bare.iH.x, bare.oH.x, bare.oL.x, bare.iL.x])
-        #         yBarePos.append([bare.iH.y, bare.oH.y, bare.oL.y, bare.iL.y])
-        #         iPos.append(block.current_sign)
+        xPos = []
+        yPos = []
+        xBarePos = []
+        yBarePos = []
+        iPos = []
+        xblockCorners = []
+        yblockCorners = []
+        colormap = cm.get_cmap('nipy_spectral')
+        ht_coil = []
+        block_coil = []
+
+        for eo in self.data.coil.physical_order:
+            out = self.data.coil.coils[eo.coil].poles[eo.pole].layers[eo.layer].windings[eo.winding].blocks[eo.block]
+            winding = self.data.coil.coils[eo.coil].poles[eo.pole].layers[eo.layer].windings[eo.winding]
+            block = winding.blocks[eo.block]
+            xblockCorners.append([block.block_corners.iH.x, block.block_corners.oH.x, block.block_corners.oL.x,
+                                  block.block_corners.iL.x])
+            yblockCorners.append([block.block_corners.iH.y, block.block_corners.oH.y, block.block_corners.oL.y,
+                                  block.block_corners.iL.y])
+            block_coil.append(eo.coil)
+            # Save half turn corners
+            for halfTurn_nr, halfTurn in block.half_turns.items():
+                insu = halfTurn.corners.insulated
+                bare = halfTurn.corners.bare
+                xPos.append([insu.iH.x, insu.oH.x, insu.oL.x, insu.iL.x])
+                yPos.append([insu.iH.y, insu.oH.y, insu.oL.y, insu.iL.y])
+                xBarePos.append([bare.iH.x, bare.oH.x, bare.oL.x, bare.iL.x])
+                yBarePos.append([bare.iH.y, bare.oH.y, bare.oL.y, bare.iL.y])
+                iPos.append(block.current_sign)
 
         # Create normalized scale between zero and number of half turns.
-        # normalize = Normalize(vmin=0, vmax=len(xPos))
-        #
-        # # Plot blocks and block number in coil
-        # max_size = max(max(xblockCorners, key=max))    # Plot bare half turns
-        # for c, (cXBarePos, cYBarePos) in enumerate(zip(xBarePos, yBarePos)):
-        #     pt1, pt2, pt3, pt4 = (cXBarePos[0], cYBarePos[0]), (cXBarePos[1], cYBarePos[1]), \
-        #                          (cXBarePos[2], cYBarePos[2]), (cXBarePos[3], cYBarePos[3])
-        #     if iPos[c] > 0:
-        #         line = plt.Polygon([pt1, pt2, pt3, pt4], closed=True, fill=True, facecolor='r', edgecolor='k',
-        #                            alpha=.25)
-        #     else:
-        #         line = plt.Polygon([pt1, pt2, pt3, pt4], closed=True, fill=True, facecolor='b', edgecolor='k',
-        #                            alpha=.25)
-        #     plt.gca().add_line(line)
-        # for c, (xblockCorners, yblockCorners) in enumerate(zip(xblockCorners, yblockCorners)):
-        #     pt1, pt2, pt3, pt4 = (xblockCorners[0], yblockCorners[0]), (xblockCorners[1], yblockCorners[1]), \
-        #                          (xblockCorners[2], yblockCorners[2]), (xblockCorners[3], yblockCorners[3])
-        #     line = Line2D([pt1[0], pt2[0]], [pt1[1], pt2[1]], color='b')
-        #     plt.gca().add_line(line)
-        #     line = Line2D([pt3[0], pt4[0]], [pt3[1], pt4[1]], color='Fb')
-        #     plt.gca().add_line(line)
-        #     bore_center_x, bore_center_y = (
-        #     self.data.coil.coils[block_coil[c]].bore_center.x, self.data.coil.coils[block_coil[c]].bore_center.y)
-        #     plot_arcs(pt4, pt1, (bore_center_x, bore_center_y), plt.gca())
-        #     plot_arcs(pt3, pt2, (bore_center_x, bore_center_y), plt.gca())
-        #     x_ave_cond, y_ave_cond = sum(xblockCorners) / len(xblockCorners), sum(yblockCorners) / len(yblockCorners)
-        #     plt.text(x_ave_cond, y_ave_cond, '{}'.format(c + 1), color='b', fontsize=14)
+        normalize = Normalize(vmin=0, vmax=len(xPos))
+
+        # Plot blocks and block number in coil
+        max_size = max(max(xblockCorners, key=max))    # Plot bare half turns
+        for c, (cXBarePos, cYBarePos) in enumerate(zip(xBarePos, yBarePos)):
+            pt1, pt2, pt3, pt4 = (cXBarePos[0], cYBarePos[0]), (cXBarePos[1], cYBarePos[1]), \
+                                 (cXBarePos[2], cYBarePos[2]), (cXBarePos[3], cYBarePos[3])
+            if iPos[c] > 0:
+                line = plt.Polygon([pt1, pt2, pt3, pt4], closed=True, fill=True, facecolor='r', edgecolor='k',
+                                   alpha=.25)
+            else:
+                line = plt.Polygon([pt1, pt2, pt3, pt4], closed=True, fill=True, facecolor='b', edgecolor='k',
+                                   alpha=.25)
+            plt.gca().add_line(line)
+        for c, (xblockCorners, yblockCorners) in enumerate(zip(xblockCorners, yblockCorners)):
+            pt1, pt2, pt3, pt4 = (xblockCorners[0], yblockCorners[0]), (xblockCorners[1], yblockCorners[1]), \
+                                 (xblockCorners[2], yblockCorners[2]), (xblockCorners[3], yblockCorners[3])
+            line = Line2D([pt1[0], pt2[0]], [pt1[1], pt2[1]], color='b')
+            plt.gca().add_line(line)
+            line = Line2D([pt3[0], pt4[0]], [pt3[1], pt4[1]], color='b')
+            plt.gca().add_line(line)
+            bore_center_x, bore_center_y = (
+            self.data.coil.coils[block_coil[c]].bore_center.x, self.data.coil.coils[block_coil[c]].bore_center.y)
+            plot_arcs(pt4, pt1, (bore_center_x, bore_center_y), plt.gca())
+            plot_arcs(pt3, pt2, (bore_center_x, bore_center_y), plt.gca())
+            x_ave_cond, y_ave_cond = sum(xblockCorners) / len(xblockCorners), sum(yblockCorners) / len(yblockCorners)
+            plt.text(x_ave_cond, y_ave_cond, '{}'.format(c + 1), color='b', fontsize=14)
 
-        # ax = plt.axes()
+        #ax = plt.axes()
 
         wedge_no = 0
         for coil_nr, coil in self.data.coil.coils.items():
             for pole_nr, pole in coil.poles.items():
                 for layer_nr, layer in pole.layers.items():
                     for winding_key, winding in layer.windings.items():
                         if winding_key < max(layer.windings.keys()) and winding_key + 1 in layer.windings.keys():
@@ -1731,65 +1736,41 @@
 
                             for block_key, block in winding.blocks.items():
                                 wedge_no += 1
                                 self.data.wedges[wedge_no] = pd.Wedge()
                                 wedge = self.data.wedges[wedge_no]
 
                                 if blocks.index(block_key) == 0:
-                                    # if block.block_corners.iH.y < 0 and block.block_corners.iH.x>0:
-                                    #     wedge.corners = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners.iH, iL=block.block_corners.iL,
-                                    #                               oH=adj_winding.blocks[adj_blocks[0]].block_corners.oH, oL=block.block_corners.oL)
-                                    #     wedge.corners_ins = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.iL, iL=block.block_corners_ins.iH,
-                                    #                                   oH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.oL, oL=block.block_corners_ins.oH)
-                                    #     wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
-                                    #     wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[0])
-                                    #
-                                    # elif block.block_corners.iH.y < 0 and block.block_corners.iH.x<0:
-                                    #     wedge.corners = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners.iL, iL=block.block_corners.iH,
-                                    #                               oH=adj_winding.blocks[adj_blocks[0]].block_corners.oL, oL=block.block_corners.oH)
-                                    #     wedge.corners_ins = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.iL, iL=block.block_corners_ins.iH,
-                                    #                                   oH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.oL, oL=block.block_corners_ins.oH)
-                                    #     wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
-                                    #     wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[0])
-                                    # else:
-                                        wedge.corners = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners.iL, iL=block.block_corners.iH,
-                                                                  oH=adj_winding.blocks[adj_blocks[0]].block_corners.oL, oL=block.block_corners.oH)
-                                        wedge.corners_ins = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.iL, iL=block.block_corners_ins.iH,
-                                                                      oH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.oL, oL=block.block_corners_ins.oH)
-                                        wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
-                                        wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[0])
+                                    wedge.corners = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners.iL, iL=block.block_corners.iH,
+                                                              oH=adj_winding.blocks[adj_blocks[0]].block_corners.oL, oL=block.block_corners.oH)
+                                    wedge.corners_ins = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.iL, iL=block.block_corners_ins.iH,
+                                                                  oH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.oL, oL=block.block_corners_ins.oH)
+                                    wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
+                                    wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[0])
                                 else:
-                                    # if block.block_corners.iH.y < 0 and block.block_corners.iH.x<0:
-                                    #     wedge.corners = pd.Corner(iH=adj_winding.blocks[adj_blocks[1]].block_corners.iL, iL=block.block_corners.iH,
-                                    #                               oH=adj_winding.blocks[adj_blocks[1]].block_corners.oL, oL=block.block_corners.oH)
-                                    #     wedge.corners_ins = pd.Corner(iH=adj_winding.blocks[adj_blocks[1]].block_corners_ins.iL, iL=block.block_corners_ins.iH,
-                                    #                                   oH=adj_winding.blocks[adj_blocks[1]].block_corners_ins.oL, oL=block.block_corners_ins.oH)
-                                    # wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
-                                    # wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[0])
-                                    # else:
                                     wedge.corners = pd.Corner(iH=block.block_corners.iL, iL=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners.iH,
                                                               oH=block.block_corners.oL, oL=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners.oH)
                                     wedge.corners_ins = pd.Corner(iH=block.block_corners_ins.iL, iL=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners_ins.iH,
                                                                   oH=block.block_corners_ins.oL, oL=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners_ins.oH)
                                     wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
                                     wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[blocks.index(block_key)])
 
-                                # color='k'
-                                # arg = [(wedge.corners.iH.x, wedge.corners.iH.y),
-                                #        (wedge.corners.iL.x, wedge.corners.iL.y),
-                                #        (wedge.corners.oH.x, wedge.corners.oH.y),
-                                #        (wedge.corners.oL.x, wedge.corners.oL.y)]
-                                # line = Line2D([arg[0][0], arg[1][0]], [arg[0][1], arg[1][1]], color=color)
-                                # plt.gca().add_line(line)
-                                # line = Line2D([arg[3][0], arg[2][0]], [arg[3][1], arg[2][1]], color=color)
-                                # plt.gca().add_line(line)
-                                # line = Line2D([arg[0][0], arg[2][0]], [arg[0][1], arg[2][1]], color=color)
-                                # plt.gca().add_line(line)
-                                # line = Line2D([arg[3][0], arg[1][0]], [arg[3][1], arg[1][1]], color=color)
-                                # plt.gca().add_line(line)
+                                color='k'
+                                arg = [(wedge.corners.iH.x, wedge.corners.iH.y),
+                                       (wedge.corners.iL.x, wedge.corners.iL.y),
+                                       (wedge.corners.oH.x, wedge.corners.oH.y),
+                                       (wedge.corners.oL.x, wedge.corners.oL.y)]
+                                line = Line2D([arg[0][0], arg[1][0]], [arg[0][1], arg[1][1]], color=color)
+                                plt.gca().add_line(line)
+                                line = Line2D([arg[3][0], arg[2][0]], [arg[3][1], arg[2][1]], color=color)
+                                plt.gca().add_line(line)
+                                line = Line2D([arg[0][0], arg[2][0]], [arg[0][1], arg[2][1]], color=color)
+                                plt.gca().add_line(line)
+                                line = Line2D([arg[3][0], arg[1][0]], [arg[3][1], arg[1][1]], color=color)
+                                plt.gca().add_line(line)
                                 # if block_key>5:
                                 #     break
 
                                 # ax.text(wedge.corners.iH.x, wedge.corners.iH.y, 'iH', style='italic', bbox={'facecolor': 'red', 'pad': 2})
                                 # ax.text(wedge.corners.oH.x, wedge.corners.oH.y, 'oH', style='italic', bbox={'facecolor': 'red', 'pad': 2})
                                 # ax.text(wedge.corners.iL.x, wedge.corners.iL.y, 'iL', style='italic', bbox={'facecolor': 'red', 'pad': 2})
                                 # ax.text(wedge.corners.oL.x, wedge.corners.oL.y, 'oL', style='italic', bbox={'facecolor': 'red', 'pad': 2})
@@ -1821,15 +1802,15 @@
                                                                      oH=wedge.corners_ins.oL, oL=wedge.corners_ins.oH)
                                 wedge.corrected_center.inner = pd.Coord(x=float(sigDig(inner[0])), y=float(sigDig(inner[1])))
                                 wedge.corrected_center.outer = pd.Coord(x=float(sigDig(outer[0])), y=float(sigDig(outer[1])))
                                 wedge.corrected_center_ins.inner = pd.Coord(x=float(sigDig(inner_ins[0])), y=float(sigDig(inner_ins[1])))
                                 wedge.corrected_center_ins.outer = pd.Coord(x=float(sigDig(outer_ins[0])), y=float(sigDig(outer_ins[1])))
                                 # ax.text(wedge.corrected_center.inner.x, wedge.corrected_center.inner.y, 'i' + str(wedge_no), style='italic', bbox={'facecolor': 'blue', 'pad': 2})
                                 # ax.text(wedge.corrected_center.outer.x, wedge.corrected_center.outer.y, 'o' + str(wedge_no), style='italic', bbox={'facecolor': 'blue', 'pad': 2})
-        #plt.show()
+        plt.show()
 
         return self.data if coil else self.data.wedges
 
     def getData(self, dir_iron: Path = None, dir_data: Path = None, dir_cadata: Path = None,
                 dump_yamls: bool = False, verbose: bool = False):
         """
             **Returns all data**
```

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserSIGMA.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserTdms.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserXYCE.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserYAML.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserYAML.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsers/ParserYamlToRoxie.py` & `steam-sdk-2023.6.9/steam_sdk/parsers/ParserYamlToRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsims/ParsimConductor.py` & `steam-sdk-2023.6.9/steam_sdk/parsims/ParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsims/ParsimDakota.py` & `steam-sdk-2023.6.9/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsims/ParsimEventCircuit.py` & `steam-sdk-2023.6.9/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,21 @@
         # Unpack arguments
         self.verbose: bool = verbose
         self.list_events: List[DataEventCircuit] = []
         # self.dict_AnalysisStepDefinition = {}
         # self.list_AnalysisStepSequence = []
         # # save local reference model, so that empty field in EventData.csv can be populated with default ones
         self.ref_model = ref_model
+        self.plateau_duration = 0
+        self.PC_switchoff_time = 0
+        self.schedule = {}
+        self.I_end_1 = 0
+        self.I_end_2 = 0
+        self.dI_dt = 0
+        self.dI_dt2 = 0
         # # TODO add a dictionary of default values?
 
     def read_from_input(self, path_input_file: str, flag_append: bool):
         '''
         Read a list of events from an input .csv file and assign its content to a list of DataEventCircuit() objects.
         This method is used to read and set the variables that can be expressed with one or a limited amount of values.
         More complex variables are covered by dedicated methods.
@@ -45,15 +52,15 @@
         # Read the input file
         if path_input_file.endswith('.csv'):
             df_events = pd.read_csv(path_input_file)
         elif path_input_file.endswith('.xlsx'):
             df_events = pd.read_excel(path_input_file)
         else:
             raise Exception(f'The extension of the file {path_input_file} is not supported.')
-        if df_events["Circuit Name"][0].startswith(("RCD-RCO", "RCBH", "RCBV")):
+        if df_events["Circuit Name"][0].startswith(("RCD-RCO", "RCBH", "RCBV", "RB", "RCBX", "RCBC", "RCBY", "RQS", "RC.", "RQ.", "RQ4", "RQ5", "RQ6", "RQ7", "RQ8", "RQ9", "RQ10")):
             df_events = pd.DataFrame([[0 if pd.isna(x) else x for x in row] for row in df_events.values], columns=df_events.columns)
         else:
             df_events = pd.DataFrame([[None if pd.isna(x) else x for x in row] for row in df_events.values], columns=df_events.columns)
         #df_events = df_events.dropna(axis=1, how='all')
 
         # validate dataframe - if csv file has a headline or empty rows on the top, skip row until there all columnnames have values
         skip_rows = 0
@@ -88,27 +95,27 @@
                 parsed_columns += self.__read_60A(event_info, new_event)
             elif circuit_type == "RQX":
                 parsed_columns += self.__read_RQX(event_info, new_event)
             elif circuit_type in ["RQ4", "RQ5", "RQ7", "RQ8", "RQ9", "RQ10"] or (circuit_name.startswith("RQ6.") and len(circuit_name) == 6):
                 parsed_columns += self.__read_IPQ(event_info, new_event)
             elif circuit_type in ["RD1", "RD2", "RD3", "RD4"]:
                 parsed_columns += self.__read_IPD(event_info, new_event)
-            elif circuit_type in ["RCS", "ROD", "ROF", "RSD", "RSF", "RQTL9", "RQTD", "RQTF"] or (circuit_name.startswith("RQ6.") and len(circuit_name) == 8):
+            elif circuit_type in ["RCS", "RQTL9", "RQTD", "RQTF"] or (circuit_name.startswith("RQ6.") and len(circuit_name) == 8) or circuit_name.startswith(("RQS.A", "ROD", "ROF", "RSD", "RSF")):
                 parsed_columns += self.__read_600A_with_EE(event_info, new_event)
-            elif circuit_type == "RCD":
+            elif circuit_type.startswith("RCD"):
                 parsed_columns += self.__read_RCD(event_info, new_event)
             elif circuit_type == "RCBX":
                 parsed_columns += self.__read_RCBX(event_info, new_event)
-            elif circuit_type in ["RCBCH", "RCBCV", "RCBYH", "RCBYV"]:
+            elif circuit_type.startswith(("RCBCH", "RCBCV", "RCBYH", "RCBYV")):
                 parsed_columns += self.__read_80_120A(event_info, new_event)
             elif circuit_type == "RQ":
                 parsed_columns += self.__read_RQ(event_info, new_event)
             elif circuit_type == "RB":
                 parsed_columns += self.__read_RB(event_info, new_event)
-            elif circuit_type in ["RQT12", "RQT13", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RQSX3"]: #RQS common to EE and no EE case
+            elif circuit_type in ["RQT12", "RQT13", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RQSX3"] or circuit_name.startswith(("RQS.R", "RQS.L")): #RQS common to EE and no EE case
                 parsed_columns += self.__read_600A_no_EE(event_info, new_event)
             else:
                 raise Exception(f"circuit type not supported {circuit_type}")
             list_events.append(new_event)
 
         # print out all the names of the ignored columns
         ignored_column_names = list(set(df_events.columns) - set(parsed_columns))
@@ -132,49 +139,56 @@
             path_outputfile_event_csv (str): Path to the output event CSV file.
 
         Raises:
             Exception: If the length of input simulation numbers differs from length of events found in the input file.
 
         """
         # check inputs
-        if simulation_name in ["RQ_47magnets", "RQ_51magnets", "RCBX"]:
+        if simulation_name in ["RCBX"]:
             if len(simulation_numbers) != 2 * len(self.list_events):
                 raise Exception(
                     f'length of input simulation numbers ({len(simulation_numbers)}) is not double of length of events found in the input file ({len(self.list_events)}) for RQ type circuit')
+        elif simulation_name in ["RB", "RQ_47magnets", "RQ_51magnets"]:
+            print("Case of multiple events possible")
         elif len(simulation_numbers) != len(self.list_events):
             raise Exception(
                 f'length of input simulation numbers ({len(simulation_numbers)}) differs from length of events found in the input file ({len(self.list_events)})')
 
         # Make target folder if it is missing
         make_folder_if_not_existing(os.path.dirname(path_outputfile_event_csv))
 
         # open file in writing mode
         all_rows = []
         list_paramerers = []
 
         # Loop trough each element of self.list_events and write parameters to csv
         for i, event in enumerate(self.list_events):
             print(i, event)
-            new_row = {'simulation_name': simulation_name, 'simulation_number': simulation_numbers[i]}
-            event_data = self.__write_event(event)
+            if simulation_name in ["RB", "RQ_47magnets", "RQ_51magnets"]:
+                new_row = {'simulation_name': simulation_name, 'simulation_number': simulation_numbers[0]}
+            else:
+                new_row = {'simulation_name': simulation_name, 'simulation_number': simulation_numbers[i]}
+            event_data = self.__write_event(event, event_counter=i)
             event_data_counter = 0
             if simulation_name == "RCD":
                 new_row = {'simulation_name': simulation_name, 'simulation_number': simulation_numbers[i]}
                 new_row.update(event_data[1][0])
                 all_rows.append(new_row)
                 list_paramerers = list(set(list_paramerers + list(new_row.keys())))
             elif simulation_name == "RCO":
                 new_row.update(event_data[0])
                 all_rows.append(new_row)
                 list_paramerers = list(set(list_paramerers + list(new_row.keys())))
             elif isinstance(event_data, list):
                 for data in event_data:
                     new_row.update(data)
-                    if simulation_name in ["RQ_47magnets", "RQ_51magnets", "RCBX"] and event_data_counter % 2 != 0:
-                        new_row['simulation_number'] = 2
+                    # if simulation_name in ["RQ_47magnets", "RQ_51magnets"] and event_data_counter % 2 != 0:
+                    #     new_row['simulation_number'] = 2
+                    if simulation_name in ["RCBX", "RQ_47magnets", "RQ_51magnets"] and event_data_counter % 2 != 0:
+                        new_row['simulation_number'] = simulation_numbers[1]
                     all_rows.append(new_row.copy())
                     list_paramerers = list(set(list_paramerers + list(new_row.keys())))
                     event_data_counter = event_data_counter + 1
             else:
                 new_row.update(event_data)
                 all_rows.append(new_row)
                 list_paramerers = list(set(list_paramerers + list(new_row.keys())))
@@ -887,32 +901,32 @@
                 for subkey in key:
                     return_list.append(subkey)
             else:
                 return_list.append(key)
 
         return return_list
 
-    def __write_event(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
+    def __write_event(self, event: DataEventCircuit, t_after_PC_off: float = 10.0, event_counter: int = 0):
         circuit_type = event.GeneralParameters.circuit_type
         circuit_name = event.GeneralParameters.name
-        if circuit_type in ["RQT12", "RQT13", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RQSX3", "RCBYV", "RCBYH", "RCBCH", "RCBCV", "RD1", "RD2", "RD3", "RD4"] or circuit_type.startswith(('RCBH', 'RCBV')):
+        if circuit_type in ["RQT12", "RQT13", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RQSX3", "RCBYV", "RCBYH", "RCBCH", "RCBCV", "RD1", "RD2", "RD3", "RD4"] or circuit_type.startswith(('RCBH', 'RCBV', 'RCBCH', 'RCBCV', 'RCBYH', 'RCBYV')) or circuit_name.startswith(("RQS.R", "RQS.L")):
             event_dict = self.__write_common_circuit_family(event, t_after_PC_off=t_after_PC_off)
         elif circuit_type == "RQ":
-            event_dict = self.__write_RQ(event, t_after_PC_off=t_after_PC_off)
+            event_dict = self.__write_RQ(event, t_after_PC_off=t_after_PC_off, event_counter=event_counter)
         elif circuit_type in ["RQ4", "RQ5", "RQ7", "RQ8", "RQ9", "RQ10"] or (circuit_name.startswith("RQ6.") and len(circuit_name) == 6):
             event_dict = self.__write_IPQ(event, t_after_PC_off=t_after_PC_off)
         elif circuit_type == "RQX":
             event_dict = self.__write_RQX(event, t_after_PC_off=t_after_PC_off)
-        elif circuit_type in ["RCS", "ROD", "ROF", "RSD", "RSF", "RQTL9", "RQTD", "RQTF"] or (circuit_name.startswith("RQ6.") and len(circuit_name) == 8):
+        elif circuit_type in ["RCS", "RQTL9", "RQTD", "RQTF"] or (circuit_name.startswith("RQ6.") and len(circuit_name) == 8) or circuit_name.startswith(("RQS.A", "ROD", "ROF", "RSD", "RSF")):
             event_dict = self.__write_600A_with_EE(event, t_after_PC_off=t_after_PC_off)
         elif circuit_type == "RB":
-            event_dict = self.__write_RB(event, t_after_PC_off=t_after_PC_off)
+            event_dict = self.__write_RB(event, t_after_PC_off=t_after_PC_off, event_counter=event_counter)
         elif circuit_type == "RCBX":
             event_dict = self.__write_RCBX(event, t_after_PC_off=t_after_PC_off)
-        elif circuit_name.startswith("RCD-RCO"):
+        elif circuit_name.startswith(("RCD-RCO", "RC.")):
             event_dict = self.__write_RCD_RCO(event, t_after_PC_off=t_after_PC_off)
         return event_dict
 
     def __write_common_circuit_family(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
         """
         Extract the information for an event of circuit type RCB.
 
@@ -924,15 +938,15 @@
 
         """
         circuit_name = event.GeneralParameters.name
         event_dict = dict()
         t_start = 0  # hard-coded
         I_start = 0.0  # hard-coded
         dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
-        if circuit_name.startswith("RCD-RCO"):
+        if circuit_name.startswith(("RCD-RCO", "RC.")):
             dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge[0]
             current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge[0]
         else:
             dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge
             current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge
         t_PC_off = self.__handle_ramp_rate_cases(event, circuit_name, t_after_PC_off, t_start, I_start, dI_dt, dI_dt2, current_at_discharge, event_dict)
         event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
@@ -969,15 +983,15 @@
         #     if rgetattr(event.PoweredCircuits[circuit_name], old_name) and not math.isnan(rgetattr(event.PoweredCircuits[circuit_name], old_name)):
         #         event_dict[new_name] = rgetattr(event.PoweredCircuits[circuit_name], old_name)
         #     if not new_name in event_dict:
         #         event_dict[new_name] = ''
 
         return event_dict
 
-    def __write_RQ(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
+    def __write_RQ(self, event: DataEventCircuit, t_after_PC_off: float = 10.0, event_counter: int = 0):
         """
         Extract the information for an event of circuit type RQ.
 
         Parameters:
             event (DataEventCircuit): The data event object to read the data.
 
         Returns:
@@ -988,67 +1002,88 @@
         list= []
         t_EE_list = []
         t_PC_off_list = []
         for i in range(2):
             event_dict = dict()
             t_start = 0  # hard-coded
             I_start = 0.0  # hard-coded
-            dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
+            self.dI_dt2 = dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
             dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge[i]
+            current_at_discharge = event.QuenchEvents[circuit_name].current_at_quench[i]
 
-            current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge[i]
             if dI_dt == 0:
                 I_end = current_at_discharge
                 dI_dt = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt'])
                 time_to_reach_I = self.__time_to_reach_I(I=I_end, dI_dt=dI_dt, dI_dt2=dI_dt2, I_start=I_start)
                 t_plateau = event.PoweredCircuits[circuit_name].plateau_duration[i]
                 t_PC_off = t_start + time_to_reach_I + t_plateau
-                #event_dict['GlobalParameters.global_parameters.t_plateau'] = t_plateau
-                event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end
-                event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
+                if event_counter == 0:
+                    self.I_end_1 = event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end
+                    self.I_end_2 = event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
+                    self.dI_dt = dI_dt
 
             elif np.sign(dI_dt) != np.sign(current_at_discharge):
                 I_end_1 = 1.2*current_at_discharge
                 I_end_2 = current_at_discharge
+                I_target = current_at_discharge + np.sign(current_at_discharge) * 100.0
                 t_plateau = 10  # hard-coded
-                t_PC_off = calculate_t_PC_off(t_start, I_start, [I_end_1, I_end_2], [-dI_dt, dI_dt], [dI_dt2, dI_dt2], [t_plateau, t_plateau], I_end_2)
-                event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end_1
-                event_dict['GlobalParameters.global_parameters.I_end_2'] = I_end_2
-                event_dict['GlobalParameters.global_parameters.dI_dt'] = -dI_dt  # setting dI_dt
-                event_dict['GlobalParameters.global_parameters.dI_dt2'] = dI_dt2  # setting dI_dt2
+                t_PC_off = calculate_t_PC_off(t_start, I_start, [I_end_1, I_target], [-dI_dt, dI_dt], [dI_dt2, dI_dt2], [t_plateau, t_plateau], I_end_2)
+                if event_counter == 0:
+                    self.I_end_1 = event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end_1
+                    self.I_end_2 = event_dict['GlobalParameters.global_parameters.I_end_2'] = I_end_2
+                    self.dI_dt = event_dict['GlobalParameters.global_parameters.dI_dt'] = -dI_dt  # setting dI_dt
 
             else:
                 I_end = str(current_at_discharge) + " + 100.0"
                 I_target = current_at_discharge + 100.0
                 t_plateau = t_start + 2 * dI_dt / dI_dt2 + (I_target - I_start - dI_dt ** 2 / dI_dt2) / dI_dt
                 t_PC_off = calculate_t_PC_off(t_start, I_start,  I_target, [dI_dt], [dI_dt2], [t_plateau], I_target - 100)
-                event_dict['GlobalParameters.global_parameters.dI_dt'] = dI_dt  #setting dI_dt
-                event_dict['GlobalParameters.global_parameters.I_end_1'] = I_target
-                event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
+                if event_counter == 0:
+                    self.dI_dt = event_dict['GlobalParameters.global_parameters.dI_dt'] = dI_dt  # setting dI_dt
+                    self.I_end_1 = event_dict['GlobalParameters.global_parameters.I_end_1'] = I_target
+                    self.I_end_2 = event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
 
             t_PC_off_list.append(t_PC_off)
-            dict_time_schedule = {
-                '0.0': '0.5',
-                f'{t_PC_off - 1.000}': '0.100',
-                f'{t_PC_off - 0.100}': '0.010',
-                f'{t_PC_off - 0.010}': '0.001',
-                f'{t_PC_off - 0.001}': '0.0001',
-                f'{t_PC_off + 0.020}': '0.001',
-                f'{t_PC_off + 1.000}': '0.010',
-                f'{t_PC_off + 3.000}': '0.500'
-            }
-            event_dict['GlobalParameters.global_parameters.I_start'] = I_start
-            event_dict['GlobalParameters.global_parameters.t_start'] = t_start
-            event_dict['GlobalParameters.global_parameters.t_plateau'] = t_plateau
-            event_dict['GlobalParameters.global_parameters.t_PC_off'] = t_PC_off
-            event_dict['GlobalParameters.global_parameters.t_EE'] = t_PC_off + 0.096
-            event_dict['Analysis.simulation_time.time_end'] = t_PC_off + t_after_PC_off
-            event_dict['Analysis.simulation_time.time_schedule'] = dict_time_schedule
-            event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off_list
-            event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC = t_EE_list.append(t_PC_off + 0.096)
+            if event_counter == 0:
+                dict_time_schedule = {
+                    '0.0': '0.5',
+                    f'{t_PC_off - 1.000}': '0.100',
+                    f'{t_PC_off - 0.100}': '0.010',
+                    f'{t_PC_off - 0.010}': '0.001',
+                    f'{t_PC_off - 0.001}': '0.0001',
+                    f'{t_PC_off + 0.020}': '0.001',
+                    f'{t_PC_off + 1.000}': '0.010',
+                    f'{t_PC_off + 3.000}': '0.500'
+                }
+
+                event_dict['GlobalParameters.global_parameters.I_start'] = I_start
+                event_dict['GlobalParameters.global_parameters.t_start'] = t_start
+                self.plateau_duration = event_dict['GlobalParameters.global_parameters.t_plateau'] = t_plateau
+                self.PC_switchoff_time = event_dict['GlobalParameters.global_parameters.t_PC_off'] = t_PC_off
+                event_dict['Analysis.simulation_time.time_end'] = t_PC_off + t_after_PC_off
+                self.schedule = event_dict['Analysis.simulation_time.time_schedule'] = dict_time_schedule
+                event_dict['GlobalParameters.global_parameters.t_EE'] = t_PC_off + event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC[i]*0.001 - event.PoweredCircuits[circuit_name].delta_t_FGC_PIC*0.001
+                #event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC = [event_dict['GlobalParameters.global_parameters.t_EE']]
+                event.QuenchEvents[circuit_name].delta_t_iQPS_PIC = t_PC_off + event.QuenchEvents[circuit_name].delta_t_iQPS_PIC * 0.001 - event.PoweredCircuits[circuit_name].delta_t_FGC_PIC * 0.001
+                event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
+            else:
+                event_dict['GlobalParameters.global_parameters.I_start'] = I_start
+                event_dict['GlobalParameters.global_parameters.t_start'] = t_start
+                event_dict['GlobalParameters.global_parameters.dI_dt'] = self.dI_dt
+                event_dict['GlobalParameters.global_parameters.I_end_1'] = self.I_end_1
+                event_dict['GlobalParameters.global_parameters.I_end_2'] = self.I_end_2
+                event_dict['GlobalParameters.global_parameters.dI_dt2'] = self.dI_dt2
+                event_dict['GlobalParameters.global_parameters.t_plateau'] = self.plateau_duration
+                event_dict['GlobalParameters.global_parameters.t_PC_off'] = self.PC_switchoff_time
+                event_dict['Analysis.simulation_time.time_end'] = self.PC_switchoff_time + t_after_PC_off + 100
+                event_dict['Analysis.simulation_time.time_schedule'] = self.schedule
+                event_dict['GlobalParameters.global_parameters.t_EE'] = self.PC_switchoff_time + event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC[i] * 0.001 - event.PoweredCircuits[circuit_name].delta_t_FGC_PIC * 0.001
+                #event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC = [event_dict['GlobalParameters.global_parameters.t_EE']]
+                event.QuenchEvents[circuit_name].delta_t_iQPS_PIC = self.PC_switchoff_time + event.QuenchEvents[circuit_name].delta_t_iQPS_PIC * 0.001 - event.PoweredCircuits[circuit_name].delta_t_FGC_PIC * 0.001
+                event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = self.PC_switchoff_time
 
             list.append(event_dict)
 
         return list
 
     def __write_RCBX(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
         """
@@ -1067,14 +1102,15 @@
         for i in range(2):
             event_dict = dict()
             t_start = 0  # hard-coded
             I_start = 0.0  # hard-coded
             dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
             dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge[i]
             current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge[i]
+            self.plateau_duration = event.PoweredCircuits[circuit_name].plateau_duration[i]
             t_PC_off = self.__handle_ramp_rate_cases(event, circuit_name, t_after_PC_off, t_start, I_start, dI_dt, dI_dt2, current_at_discharge, event_dict)
             t_PC_off_list.append(t_PC_off)
             event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off_list
             list.append(event_dict)
 
         return list
 
@@ -1312,31 +1348,31 @@
         list= []
         t_EE_list = []
         t_PC_off_list = []
         event_dict = dict()
         t_start = 0  # hard-coded
         I_start = 0.0  # hard-coded
         dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
-        if circuit_name.startswith("RCD-RCO"):
+        if circuit_name.startswith(("RCD-RCO", "RC.")):
             dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge[1]
             current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge[1]
         else:
             dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge
             current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge
         t_PC_off = self.__handle_ramp_rate_cases(event, circuit_name, t_after_PC_off, t_start, I_start, dI_dt, dI_dt2, current_at_discharge, event_dict)
         t_PC_off_list.append(t_PC_off)
-        event_dict['GlobalParameters.global_parameters.t_EE'] = t_PC_off + 0.008
+        event_dict['GlobalParameters.global_parameters.t_EE'] = t_PC_off + event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC * 0.001 - event.PoweredCircuits[circuit_name].delta_t_FGC_PIC * 0.001
         event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off_list
-        event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC = t_EE_list.append(t_PC_off + 0.008)
+        event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC = t_EE_list.append(event_dict['GlobalParameters.global_parameters.t_EE'])
 
         list.append(event_dict)
 
         return list
 
-    def __write_RB(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
+    def __write_RB(self, event: DataEventCircuit, t_after_PC_off: float = 10.0, event_counter: int = 0):
         """
         Extract the information for an event of circuit type RB.
 
         Parameters:
             event (DataEventCircuit): The data event object to read the data.
 
         Returns:
@@ -1344,35 +1380,107 @@
 
         """
         circuit_name = event.GeneralParameters.name
         list= []
         event_dict = dict()
         t_start = 0  # hard-coded
         I_start = 0.0  # hard-coded
-        dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
+        self.dI_dt2 = dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
         dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge
-        current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge
-        t_PC_off = self.__handle_ramp_rate_cases(event, circuit_name, t_after_PC_off, t_start, I_start, dI_dt, dI_dt2, current_at_discharge, event_dict)
-        event_dict['GlobalParameters.global_parameters.t_EE_1'] = t_PC_off + 0.005 # value to be confirmed for RB
-        event_dict['GlobalParameters.global_parameters.t_EE_2'] = t_PC_off + 0.005
-        event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
-        event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC = [t_PC_off + 0.005]*2
+        current_at_discharge = event.QuenchEvents[circuit_name].current_at_quench
+
+        if dI_dt == 0:
+            I_end = current_at_discharge
+            dI_dt = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt'])
+            time_to_reach_I = self.__time_to_reach_I(I=I_end, dI_dt=dI_dt, dI_dt2=dI_dt2, I_start=I_start)
+            t_plateau = event.PoweredCircuits[circuit_name].plateau_duration
+            if circuit_name.startswith(("RCD-RCO", "RC.")):
+                t_PC_off = t_start + time_to_reach_I + t_plateau[0]
+            else:
+                t_PC_off = t_start + time_to_reach_I + t_plateau
+            if event_counter == 0:
+                self.I_end_1 = event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end
+                self.I_end_2 = event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
+                self.dI_dt = dI_dt
+
+
+        elif np.sign(dI_dt) != np.sign(current_at_discharge):
+            I_end_1 = 1.2*current_at_discharge
+            I_end_2 = current_at_discharge
+            I_target = current_at_discharge + np.sign(current_at_discharge) * 100.0
+            t_plateau = 10  # hard-coded
+            t_PC_off = calculate_t_PC_off(t_start, I_start, [I_end_1, I_target], [-dI_dt, dI_dt], [dI_dt2, dI_dt2], [t_plateau, t_plateau], I_end_2)
+            if event_counter == 0:
+                self.I_end_1 = event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end_1
+                self.I_end_2 = event_dict['GlobalParameters.global_parameters.I_end_2'] = I_end_2
+                self.dI_dt = event_dict['GlobalParameters.global_parameters.dI_dt'] = -dI_dt  # setting dI_dt
+
+        else:
+            I_end = str(current_at_discharge) + " + 100.0"
+            I_target = current_at_discharge + 100.0
+            t_plateau = t_start + 2 * dI_dt / dI_dt2 + (I_target - I_start - dI_dt ** 2 / dI_dt2) / dI_dt
+            t_PC_off = calculate_t_PC_off(t_start, I_start,  I_target, [dI_dt], [dI_dt2], [t_plateau], I_target - 100)
+            if event_counter == 0:
+                self.dI_dt = event_dict['GlobalParameters.global_parameters.dI_dt'] = dI_dt  #setting dI_dt
+                self.I_end_1 = event_dict['GlobalParameters.global_parameters.I_end_1'] = I_target
+                self.I_end_2 = event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
+
+        if event_counter == 0:
+            dict_time_schedule = {
+                '0.0': '0.5',
+                f'{t_PC_off - 1.000}': '0.100',
+                f'{t_PC_off - 0.100}': '0.010',
+                f'{t_PC_off - 0.010}': '0.001',
+                f'{t_PC_off - 0.001}': '0.0001',
+                f'{t_PC_off + 0.020}': '0.001',
+                f'{t_PC_off + 1.000}': '0.010',
+                f'{t_PC_off + 3.000}': '0.500'
+            }
 
+            event_dict['GlobalParameters.global_parameters.I_start'] = I_start
+            event_dict['GlobalParameters.global_parameters.t_start'] = t_start
+            self.plateau_duration = event_dict['GlobalParameters.global_parameters.t_plateau'] = t_plateau
+            self.PC_switchoff_time = event_dict['GlobalParameters.global_parameters.t_PC_off'] = t_PC_off
+            event_dict['Analysis.simulation_time.time_end'] = t_PC_off + t_after_PC_off
+            self.schedule = event_dict['Analysis.simulation_time.time_schedule'] = dict_time_schedule
+            event_dict['GlobalParameters.global_parameters.t_EE_1'] = t_PC_off + event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC[1]*0.001 - event.PoweredCircuits[circuit_name].delta_t_FGC_PIC*0.001
+            event_dict['GlobalParameters.global_parameters.t_EE_2'] = t_PC_off + event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC[0]*0.001 - event.PoweredCircuits[circuit_name].delta_t_FGC_PIC*0.001
+            event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC = [event_dict['GlobalParameters.global_parameters.t_EE_1'], event_dict['GlobalParameters.global_parameters.t_EE_2']]
+            event.QuenchEvents[circuit_name].delta_t_iQPS_PIC = t_PC_off + event.QuenchEvents[circuit_name].delta_t_iQPS_PIC * 0.001 - event.PoweredCircuits[circuit_name].delta_t_FGC_PIC * 0.001
+            event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
+        else:
+            event_dict['GlobalParameters.global_parameters.I_start'] = I_start
+            event_dict['GlobalParameters.global_parameters.t_start'] = t_start
+            event_dict['GlobalParameters.global_parameters.dI_dt'] = self.dI_dt
+            event_dict['GlobalParameters.global_parameters.I_end_1'] = self.I_end_1
+            event_dict['GlobalParameters.global_parameters.I_end_2'] = self.I_end_2
+            event_dict['GlobalParameters.global_parameters.dI_dt2'] = self.dI_dt2
+            event_dict['GlobalParameters.global_parameters.t_plateau'] = self.plateau_duration
+            event_dict['GlobalParameters.global_parameters.t_PC_off'] = self.PC_switchoff_time
+            event_dict['Analysis.simulation_time.time_end'] = self.PC_switchoff_time + t_after_PC_off + 100
+            event_dict['Analysis.simulation_time.time_schedule'] = self.schedule
+            event_dict['GlobalParameters.global_parameters.t_EE_1'] = self.PC_switchoff_time + event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC[1]*0.001 - event.PoweredCircuits[circuit_name].delta_t_FGC_PIC*0.001
+            event_dict['GlobalParameters.global_parameters.t_EE_2'] = self.PC_switchoff_time + event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC[0]*0.001 - event.PoweredCircuits[circuit_name].delta_t_FGC_PIC*0.001
+            event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC = [event_dict['GlobalParameters.global_parameters.t_EE_1'], event_dict['GlobalParameters.global_parameters.t_EE_2']]
+            event.QuenchEvents[circuit_name].delta_t_iQPS_PIC = self.PC_switchoff_time + event.QuenchEvents[circuit_name].delta_t_iQPS_PIC*0.001 - event.PoweredCircuits[circuit_name].delta_t_FGC_PIC*0.001
+            event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = self.PC_switchoff_time
         list.append(event_dict)
 
         return list
 
     def __handle_ramp_rate_cases(self, event: DataEventCircuit, circuit_name: str, t_after_PC_off: float, t_start: float, I_start: float, dI_dt: float, dI_dt2: float, current_at_discharge: float, event_dict: dict ):
         if dI_dt == 0:
             I_end = current_at_discharge
             dI_dt = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt'])
             time_to_reach_I = self.__time_to_reach_I(I=I_end, dI_dt=dI_dt, dI_dt2=dI_dt2, I_start=I_start)
             t_plateau = event.PoweredCircuits[circuit_name].plateau_duration
-            if circuit_name.startswith("RCD-RCO"):
+            if circuit_name.startswith(("RCD-RCO", "RC.")):
                 t_PC_off = t_start + time_to_reach_I + t_plateau[0]
+            elif circuit_name.startswith("RCBX"):
+                t_PC_off = t_start + time_to_reach_I + self.plateau_duration
             else:
                 t_PC_off = t_start + time_to_reach_I + t_plateau
             event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end
             event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
 
         elif np.sign(dI_dt) != np.sign(current_at_discharge):
             I_end_1 = 1.2*current_at_discharge
@@ -1416,11 +1524,11 @@
 
     @staticmethod
     def __time_to_reach_I(I: float, dI_dt: float, dI_dt2: float, I_start: float):
         '''
         Calculate the time to reach a current assuming a parabolic, linear, and parabolic profile
         :return: time [s]
         '''
-        t_parabolic = dI_dt / dI_dt2
-        I_parabolic = 0.5 * dI_dt2 * t_parabolic**2
-        t_linear = (I - I_start - 2*I_parabolic) / dI_dt
+        t_parabolic = abs(dI_dt / dI_dt2)
+        I_parabolic = 0.5 * abs(dI_dt2) * t_parabolic**2
+        t_linear = (abs(I - I_start) - 2*I_parabolic) / abs(dI_dt)
         return t_parabolic*2 + t_linear
```

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsims/ParsimEventMagnet.py` & `steam-sdk-2023.6.9/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/parsims/ParsimSweep.py` & `steam-sdk-2023.6.9/steam_sdk/parsims/ParsimSweep.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/plotters/PlotterAnalysis.py` & `steam-sdk-2023.6.9/steam_sdk/plotters/PlotterAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/plotters/PlotterMap2d.py` & `steam-sdk-2023.6.9/steam_sdk/plotters/PlotterMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/plotters/PlotterModel.py` & `steam-sdk-2023.6.9/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/plotters/PlotterParametric.py` & `steam-sdk-2023.6.9/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/plotters/PlotterRoxie.py` & `steam-sdk-2023.6.9/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/postprocs/PostprocsMetrics.py` & `steam-sdk-2023.6.9/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/utils/MTF_reading_functions.py` & `steam-sdk-2023.6.9/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/utils/ModifyModelData.py` & `steam-sdk-2023.6.9/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam-sdk-2023.6.9/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/utils/ModifyModelDataconductor.py` & `steam-sdk-2023.6.9/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/utils/ParserRoxieHelpers.py` & `steam-sdk-2023.6.9/steam_sdk/utils/ParserRoxieHelpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,25 +64,23 @@
 
     else:
         point_iH = point_list[low_ind2]
         point_iL = point_list[low_ind1]
         point_number_iH = low_ind2
         point_number_iL = low_ind1
 
-    # color = 'k'
-    # arg = [(point_iH[0], point_iH[1]),
-    #        (point_iL[0], point_iL[1]),
-    #        (point_oH[0], point_oH[1]),
-    #        (point_oL[0], point_oL[1])]
-    #
-    # line = Line2D([arg[0][0], arg[1][0]], [arg[0][1], arg[1][1]], color=color)
-    # plt.scatter(arg[0][0],  arg[0][1], color='b')
-    # plt.text(arg[0][0], arg[0][1], str(point_number_iH), fontsize=12)
-    #
-    # plt.scatter(arg[1][0],  arg[1][1], color='r')
-    # plt.text(arg[1][0], arg[1][1], str(point_number_iL), fontsize=12)
-    #
-    # plt.scatter(arg[2][0],  arg[2][1], color='g')
-    # plt.scatter(arg[3][0],  arg[3][1], color='y')
+    color = 'k'
+    arg = [(point_iH[0], point_iH[1]),
+           (point_iL[0], point_iL[1]),
+           (point_oH[0], point_oH[1]),
+           (point_oL[0], point_oL[1])]
 
+    plt.scatter(arg[0][0],  arg[0][1], color='b')
+    plt.text(arg[0][0], arg[0][1], "iH", fontsize=12)
+
+    plt.scatter(arg[1][0],  arg[1][1], color='r')
+    plt.text(arg[1][0], arg[1][1], "iL", fontsize=12)
+
+    plt.scatter(arg[2][0],  arg[2][1], color='g')
+    plt.scatter(arg[3][0],  arg[3][1], color='y')
 
     return (point_oH, point_oL, point_iH, point_iL)
```

### Comparing `steam-sdk-2023.6.8/steam_sdk/utils/clean_NaN_from_signal.py` & `steam-sdk-2023.6.9/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/utils/compare_two_parameters.py` & `steam-sdk-2023.6.9/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/utils/create_coordinate_file_SIGMA.py` & `steam-sdk-2023.6.9/steam_sdk/utils/create_coordinate_file_SIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/utils/get_attribute_type.py` & `steam-sdk-2023.6.9/steam_sdk/utils/get_attribute_type.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/utils/misc.py` & `steam-sdk-2023.6.9/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/utils/parse_str_to_list.py` & `steam-sdk-2023.6.9/steam_sdk/utils/parse_str_to_list.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/utils/tic_toc.py` & `steam-sdk-2023.6.9/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/utils/utils_PC.py` & `steam-sdk-2023.6.9/steam_sdk/utils/utils_PC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/viewers/Viewer.py` & `steam-sdk-2023.6.9/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/viewers/ViewerMeas.py` & `steam-sdk-2023.6.9/steam_sdk/viewers/ViewerMeas.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/viewers/ViewerSim.py` & `steam-sdk-2023.6.9/steam_sdk/viewers/ViewerSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk/wrappers/wrapper_yaml.py` & `steam-sdk-2023.6.9/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk.egg-info/PKG-INFO` & `steam-sdk-2023.6.9/steam_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.6.8
+Version: 2023.6.9
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: API,CERN,STEAM,SDK
+Keywords: CERN,STEAM,API,SDK
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.6.8/steam_sdk.egg-info/SOURCES.txt` & `steam-sdk-2023.6.9/steam_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.8/steam_sdk.egg-info/requires.txt` & `steam-sdk-2023.6.9/steam_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

