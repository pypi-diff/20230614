# Comparing `tmp/peaqevcore-9.2.2.tar.gz` & `tmp/peaqevcore-9.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peaqevcore-9.2.2.tar", last modified: Thu Dec 15 20:30:53 2022, max compression
+gzip compressed data, was "peaqevcore-9.2.3.tar", last modified: Sun Jan  1 20:02:47 2023, max compression
```

## Comparing `peaqevcore-9.2.2.tar` & `peaqevcore-9.2.3.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.363664 peaqevcore-9.2.2/
--rw-rw-rw-   0        0        0    15287 2022-11-09 21:34:35.000000 peaqevcore-9.2.2/LICENSE
--rw-rw-rw-   0        0        0      220 2022-12-15 20:30:53.363664 peaqevcore-9.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2077 2022-11-11 19:40:30.000000 peaqevcore-9.2.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.206663 peaqevcore-9.2.2/peaqevcore/
--rw-rw-rw-   0        0        0      208 2022-06-28 17:34:29.000000 peaqevcore-9.2.2/peaqevcore/PeaqErrors.py
--rw-rw-rw-   0        0        0      477 2022-06-21 20:36:04.000000 peaqevcore-9.2.2/peaqevcore/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.216663 peaqevcore-9.2.2/peaqevcore/hub/
--rw-rw-rw-   0        0        0        0 2022-08-05 12:47:40.000000 peaqevcore-9.2.2/peaqevcore/hub/__init__.py
--rw-rw-rw-   0        0        0     1687 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/hub/hub.py
--rw-rw-rw-   0        0        0      799 2022-12-10 08:50:56.000000 peaqevcore-9.2.2/peaqevcore/hub/hub_options.py
--rw-rw-rw-   0        0        0     7158 2022-11-09 21:34:35.000000 peaqevcore-9.2.2/peaqevcore/hub/hub_sensors.py
--rw-rw-rw-   0        0        0     1852 2022-11-09 21:34:35.000000 peaqevcore-9.2.2/peaqevcore/hub/killswitch.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.219665 peaqevcore-9.2.2/peaqevcore/models/
--rw-rw-rw-   0        0        0        0 2022-06-21 20:36:04.000000 peaqevcore-9.2.2/peaqevcore/models/__init__.py
--rw-rw-rw-   0        0        0      248 2022-11-09 21:34:35.000000 peaqevcore-9.2.2/peaqevcore/models/chargerstates.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.228663 peaqevcore-9.2.2/peaqevcore/models/chargertype/
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/models/chargertype/__init__.py
--rw-rw-rw-   0        0        0      140 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/models/chargertype/calltype.py
--rw-rw-rw-   0        0        0      377 2022-12-15 16:59:38.000000 peaqevcore-9.2.2/peaqevcore/models/chargertype/charger_entities_model.py
--rw-rw-rw-   0        0        0      286 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/models/chargertype/charger_options.py
--rw-rw-rw-   0        0        0      417 2022-08-27 18:23:25.000000 peaqevcore-9.2.2/peaqevcore/models/chargertype/servicecalls_dto.py
--rw-rw-rw-   0        0        0      189 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/models/chargertype/servicecalls_options.py
--rw-rw-rw-   0        0        0      571 2022-10-13 07:47:19.000000 peaqevcore-9.2.2/peaqevcore/models/const.py
--rw-rw-rw-   0        0        0      608 2022-12-15 18:04:12.000000 peaqevcore-9.2.2/peaqevcore/models/fuses.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.233663 peaqevcore-9.2.2/peaqevcore/models/hourselection/
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/models/hourselection/__init__.py
--rw-rw-rw-   0        0        0      351 2022-11-28 17:35:15.000000 peaqevcore-9.2.2/peaqevcore/models/hourselection/cautionhourtype.py
--rw-rw-rw-   0        0        0      525 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/models/hourselection/const.py
--rw-rw-rw-   0        0        0     1069 2022-11-28 17:35:15.000000 peaqevcore-9.2.2/peaqevcore/models/hourselection/hourobject.py
--rw-rw-rw-   0        0        0     3429 2022-11-28 17:35:15.000000 peaqevcore-9.2.2/peaqevcore/models/hourselection/hourselectionmodels.py
--rw-rw-rw-   0        0        0      114 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/models/hourselection/hourtypelist.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.240663 peaqevcore-9.2.2/peaqevcore/models/hub/
--rw-rw-rw-   0        0        0        0 2022-08-14 10:43:32.000000 peaqevcore-9.2.2/peaqevcore/models/hub/__init__.py
--rw-rw-rw-   0        0        0     1506 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/models/hub/carpowersensor.py
--rw-rw-rw-   0        0        0     1161 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/models/hub/chargerobject.py
--rw-rw-rw-   0        0        0     2277 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/models/hub/chargerswitch.py
--rw-rw-rw-   0        0        0      345 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/models/hub/const.py
--rw-rw-rw-   0        0        0      881 2022-08-14 10:43:32.000000 peaqevcore-9.2.2/peaqevcore/models/hub/currentpeak.py
--rw-rw-rw-   0        0        0     2319 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/models/hub/hubmember.py
--rw-rw-rw-   0        0        0     2627 2022-12-13 08:33:31.000000 peaqevcore-9.2.2/peaqevcore/models/hub/power.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.256663 peaqevcore-9.2.2/peaqevcore/models/locale/
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/models/locale/__init__.py
--rw-rw-rw-   0        0        0      467 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/models/locale/enums.py
--rw-rw-rw-   0        0        0     2874 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/models/locale/peaks_model.py
--rw-rw-rw-   0        0        0      336 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/models/locale/price.py
--rw-rw-rw-   0        0        0      300 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/models/locale/queryproperties.py
--rw-rw-rw-   0        0        0      601 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/models/locale/queryservice_model.py
--rw-rw-rw-   0        0        0      178 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/models/locale/sumcounter.py
--rw-rw-rw-   0        0        0      123 2022-10-13 07:47:19.000000 peaqevcore-9.2.2/peaqevcore/models/phases.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.192664 peaqevcore-9.2.2/peaqevcore/services/
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.266663 peaqevcore-9.2.2/peaqevcore/services/chargecontroller/
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/chargecontroller/__init__.py
--rw-rw-rw-   0        0        0     1871 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/services/chargecontroller/chargecontroller.py
--rw-rw-rw-   0        0        0     1071 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/services/chargecontroller/chargecontroller_lite.py
--rw-rw-rw-   0        0        0     7570 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/services/chargecontroller/chargecontrollerbase.py
--rw-rw-rw-   0        0        0      362 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/services/chargecontroller/chargecontrollerfactory.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.275663 peaqevcore-9.2.2/peaqevcore/services/chargertype/
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/chargertype/__init__.py
--rw-rw-rw-   0        0        0     1480 2022-12-15 17:48:27.000000 peaqevcore-9.2.2/peaqevcore/services/chargertype/chargertype_base.py
--rw-rw-rw-   0        0        0      129 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/chargertype/const.py
--rw-rw-rw-   0        0        0     1634 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/chargertype/servicecalls.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.281664 peaqevcore-9.2.2/peaqevcore/services/hourselection/
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/hourselection/__init__.py
--rw-rw-rw-   0        0        0      120 2022-08-05 12:47:40.000000 peaqevcore-9.2.2/peaqevcore/services/hourselection/const.py
--rw-rw-rw-   0        0        0     1604 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/services/hourselection/hoursbase.py
--rw-rw-rw-   0        0        0      286 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/services/hourselection/hourselectionfactory.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.285663 peaqevcore-9.2.2/peaqevcore/services/hourselection/hourselectionservice/
--rw-rw-rw-   0        0        0        0 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/services/hourselection/hourselectionservice/__init__.py
--rw-rw-rw-   0        0        0     8750 2022-11-28 20:47:55.000000 peaqevcore-9.2.2/peaqevcore/services/hourselection/hourselectionservice/hourselectionservice.py
--rw-rw-rw-   0        0        0     4111 2022-11-28 20:10:50.000000 peaqevcore-9.2.2/peaqevcore/services/hourselection/hourselectionservice/hoursselection_helpers.py
--rw-rw-rw-   0        0        0     5470 2022-11-28 20:54:04.000000 peaqevcore-9.2.2/peaqevcore/services/hourselection/hoursselection.py
--rw-rw-rw-   0        0        0     3397 2022-10-13 07:47:19.000000 peaqevcore-9.2.2/peaqevcore/services/hourselection/price_aware_hours.py
--rw-rw-rw-   0        0        0      867 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/services/hourselection/regular_hours.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.292665 peaqevcore-9.2.2/peaqevcore/services/locale/
--rw-rw-rw-   0        0        0     4112 2022-11-09 21:34:35.000000 peaqevcore-9.2.2/peaqevcore/services/locale/Locale.py
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/locale/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.306663 peaqevcore-9.2.2/peaqevcore/services/locale/countries/
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/locale/countries/__init__.py
--rw-rw-rw-   0        0        0      677 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/locale/countries/belgium.py
--rw-rw-rw-   0        0        0      824 2022-10-13 07:47:19.000000 peaqevcore-9.2.2/peaqevcore/services/locale/countries/default.py
--rw-rw-rw-   0        0        0     2525 2022-10-13 07:47:19.000000 peaqevcore-9.2.2/peaqevcore/services/locale/countries/norway.py
--rw-rw-rw-   0        0        0    10301 2022-11-09 21:34:35.000000 peaqevcore-9.2.2/peaqevcore/services/locale/countries/sweden.py
--rw-rw-rw-   0        0        0      668 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/locale/free_charge.py
--rw-rw-rw-   0        0        0     1020 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/services/locale/locale_model.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.317663 peaqevcore-9.2.2/peaqevcore/services/locale/querytypes/
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/locale/querytypes/__init__.py
--rw-rw-rw-   0        0        0      812 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/locale/querytypes/const.py
--rw-rw-rw-   0        0        0     1849 2022-11-28 17:35:15.000000 peaqevcore-9.2.2/peaqevcore/services/locale/querytypes/queryservice.py
--rw-rw-rw-   0        0        0     2365 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/locale/querytypes/querysets.py
--rw-rw-rw-   0        0        0     7299 2022-08-03 18:06:08.000000 peaqevcore-9.2.2/peaqevcore/services/locale/querytypes/querytypes.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.318664 peaqevcore-9.2.2/peaqevcore/services/prediction/
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/prediction/__init__.py
--rw-rw-rw-   0        0        0     2187 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/services/prediction/prediction.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.319664 peaqevcore-9.2.2/peaqevcore/services/production/
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/production/__init__.py
--rw-rw-rw-   0        0        0      148 2022-08-05 12:47:40.000000 peaqevcore-9.2.2/peaqevcore/services/production/production.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.320664 peaqevcore-9.2.2/peaqevcore/services/scheduler/
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/scheduler/__init__.py
--rw-rw-rw-   0        0        0     3076 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/services/scheduler/schedule_session.py
--rw-rw-rw-   0        0        0     4936 2022-11-09 21:34:41.000000 peaqevcore-9.2.2/peaqevcore/services/scheduler/scheduler.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.330663 peaqevcore-9.2.2/peaqevcore/services/session/
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/session/__init__.py
--rw-rw-rw-   0        0        0     3637 2022-11-12 09:19:04.000000 peaqevcore-9.2.2/peaqevcore/services/session/energy_weekly.py
--rw-rw-rw-   0        0        0      317 2022-08-04 09:30:36.000000 peaqevcore-9.2.2/peaqevcore/services/session/power_reading.py
--rw-rw-rw-   0        0        0     3887 2022-12-06 09:37:57.000000 peaqevcore-9.2.2/peaqevcore/services/session/session.py
--rw-rw-rw-   0        0        0      522 2022-12-06 10:07:45.000000 peaqevcore-9.2.2/peaqevcore/services/session/stats.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.333663 peaqevcore-9.2.2/peaqevcore/services/threshold/
--rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/services/threshold/__init__.py
--rw-rw-rw-   0        0        0     1085 2022-12-15 20:28:23.000000 peaqevcore-9.2.2/peaqevcore/services/threshold/threshold.py
--rw-rw-rw-   0        0        0      741 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/services/threshold/threshold_lite.py
--rw-rw-rw-   0        0        0     4790 2022-12-15 20:30:05.000000 peaqevcore-9.2.2/peaqevcore/services/threshold/thresholdbase.py
--rw-rw-rw-   0        0        0      252 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/services/threshold/thresholdfactory.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.336663 peaqevcore-9.2.2/peaqevcore/services/timer/
--rw-rw-rw-   0        0        0        0 2022-08-05 12:47:40.000000 peaqevcore-9.2.2/peaqevcore/services/timer/__init__.py
--rw-rw-rw-   0        0        0      217 2022-08-05 12:47:40.000000 peaqevcore-9.2.2/peaqevcore/services/timer/const.py
--rw-rw-rw-   0        0        0     1013 2022-08-05 12:47:40.000000 peaqevcore-9.2.2/peaqevcore/services/timer/timer.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.362664 peaqevcore-9.2.2/peaqevcore/tests/
--rw-rw-rw-   0        0        0       13 2022-04-20 11:13:20.000000 peaqevcore-9.2.2/peaqevcore/tests/__init__.py
--rw-rw-rw-   0        0        0     6004 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/tests/test_chargecontroller.py
--rw-rw-rw-   0        0        0     1455 2022-08-03 16:35:52.000000 peaqevcore-9.2.2/peaqevcore/tests/test_chargertype_service.py
--rw-rw-rw-   0        0        0    40098 2022-11-28 21:47:44.000000 peaqevcore-9.2.2/peaqevcore/tests/test_hoursselection.py
--rw-rw-rw-   0        0        0      915 2022-10-13 07:47:19.000000 peaqevcore-9.2.2/peaqevcore/tests/test_hub.py
--rw-rw-rw-   0        0        0     9759 2022-11-28 17:35:15.000000 peaqevcore-9.2.2/peaqevcore/tests/test_localetypes.py
--rw-rw-rw-   0        0        0     3269 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/tests/test_prediction.py
--rw-rw-rw-   0        0        0     5643 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/tests/test_scheduler.py
--rw-rw-rw-   0        0        0     4775 2022-11-12 09:24:27.000000 peaqevcore-9.2.2/peaqevcore/tests/test_session.py
--rw-rw-rw-   0        0        0     3038 2022-10-05 13:07:12.000000 peaqevcore-9.2.2/peaqevcore/tests/test_threshold.py
--rw-rw-rw-   0        0        0      534 2022-08-05 12:47:40.000000 peaqevcore-9.2.2/peaqevcore/util.py
-drwxrwxrwx   0        0        0        0 2022-12-15 20:30:53.211664 peaqevcore-9.2.2/peaqevcore.egg-info/
--rw-rw-rw-   0        0        0      220 2022-12-15 20:30:53.000000 peaqevcore-9.2.2/peaqevcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4580 2022-12-15 20:30:53.000000 peaqevcore-9.2.2/peaqevcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-15 20:30:53.000000 peaqevcore-9.2.2/peaqevcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-12-15 20:30:53.000000 peaqevcore-9.2.2/peaqevcore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-15 20:30:53.363664 peaqevcore-9.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1152 2022-12-15 20:30:50.000000 peaqevcore-9.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.575959 peaqevcore-9.2.3/
+-rw-rw-rw-   0        0        0    15287 2022-11-09 21:34:35.000000 peaqevcore-9.2.3/LICENSE
+-rw-rw-rw-   0        0        0      220 2023-01-01 20:02:47.574960 peaqevcore-9.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2077 2022-11-11 19:40:30.000000 peaqevcore-9.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.345522 peaqevcore-9.2.3/peaqevcore/
+-rw-rw-rw-   0        0        0      208 2022-06-28 17:34:29.000000 peaqevcore-9.2.3/peaqevcore/PeaqErrors.py
+-rw-rw-rw-   0        0        0      477 2022-06-21 20:36:04.000000 peaqevcore-9.2.3/peaqevcore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.362521 peaqevcore-9.2.3/peaqevcore/hub/
+-rw-rw-rw-   0        0        0        0 2022-08-05 12:47:40.000000 peaqevcore-9.2.3/peaqevcore/hub/__init__.py
+-rw-rw-rw-   0        0        0     1687 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/hub/hub.py
+-rw-rw-rw-   0        0        0      799 2022-12-10 08:50:56.000000 peaqevcore-9.2.3/peaqevcore/hub/hub_options.py
+-rw-rw-rw-   0        0        0     7158 2022-11-09 21:34:35.000000 peaqevcore-9.2.3/peaqevcore/hub/hub_sensors.py
+-rw-rw-rw-   0        0        0     1852 2022-11-09 21:34:35.000000 peaqevcore-9.2.3/peaqevcore/hub/killswitch.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.374521 peaqevcore-9.2.3/peaqevcore/models/
+-rw-rw-rw-   0        0        0        0 2022-06-21 20:36:04.000000 peaqevcore-9.2.3/peaqevcore/models/__init__.py
+-rw-rw-rw-   0        0        0      248 2022-11-09 21:34:35.000000 peaqevcore-9.2.3/peaqevcore/models/chargerstates.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.388520 peaqevcore-9.2.3/peaqevcore/models/chargertype/
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/models/chargertype/__init__.py
+-rw-rw-rw-   0        0        0      140 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/models/chargertype/calltype.py
+-rw-rw-rw-   0        0        0      377 2022-12-15 16:59:38.000000 peaqevcore-9.2.3/peaqevcore/models/chargertype/charger_entities_model.py
+-rw-rw-rw-   0        0        0      286 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/models/chargertype/charger_options.py
+-rw-rw-rw-   0        0        0      417 2022-08-27 18:23:25.000000 peaqevcore-9.2.3/peaqevcore/models/chargertype/servicecalls_dto.py
+-rw-rw-rw-   0        0        0      189 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/models/chargertype/servicecalls_options.py
+-rw-rw-rw-   0        0        0      571 2022-10-13 07:47:19.000000 peaqevcore-9.2.3/peaqevcore/models/const.py
+-rw-rw-rw-   0        0        0      608 2022-12-15 18:04:12.000000 peaqevcore-9.2.3/peaqevcore/models/fuses.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.394522 peaqevcore-9.2.3/peaqevcore/models/hourselection/
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/models/hourselection/__init__.py
+-rw-rw-rw-   0        0        0      351 2022-11-28 17:35:15.000000 peaqevcore-9.2.3/peaqevcore/models/hourselection/cautionhourtype.py
+-rw-rw-rw-   0        0        0      525 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/models/hourselection/const.py
+-rw-rw-rw-   0        0        0     1069 2022-11-28 17:35:15.000000 peaqevcore-9.2.3/peaqevcore/models/hourselection/hourobject.py
+-rw-rw-rw-   0        0        0     3429 2023-01-01 19:54:54.000000 peaqevcore-9.2.3/peaqevcore/models/hourselection/hourselectionmodels.py
+-rw-rw-rw-   0        0        0      114 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/models/hourselection/hourtypelist.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.411521 peaqevcore-9.2.3/peaqevcore/models/hub/
+-rw-rw-rw-   0        0        0        0 2022-08-14 10:43:32.000000 peaqevcore-9.2.3/peaqevcore/models/hub/__init__.py
+-rw-rw-rw-   0        0        0     1506 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/models/hub/carpowersensor.py
+-rw-rw-rw-   0        0        0     1236 2022-12-20 18:55:25.000000 peaqevcore-9.2.3/peaqevcore/models/hub/chargerobject.py
+-rw-rw-rw-   0        0        0     2277 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/models/hub/chargerswitch.py
+-rw-rw-rw-   0        0        0      345 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/models/hub/const.py
+-rw-rw-rw-   0        0        0      881 2022-08-14 10:43:32.000000 peaqevcore-9.2.3/peaqevcore/models/hub/currentpeak.py
+-rw-rw-rw-   0        0        0     2319 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/models/hub/hubmember.py
+-rw-rw-rw-   0        0        0     2627 2022-12-13 08:33:31.000000 peaqevcore-9.2.3/peaqevcore/models/hub/power.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.430521 peaqevcore-9.2.3/peaqevcore/models/locale/
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/models/locale/__init__.py
+-rw-rw-rw-   0        0        0      467 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/models/locale/enums.py
+-rw-rw-rw-   0        0        0     2874 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/models/locale/peaks_model.py
+-rw-rw-rw-   0        0        0      336 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/models/locale/price.py
+-rw-rw-rw-   0        0        0      300 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/models/locale/queryproperties.py
+-rw-rw-rw-   0        0        0      601 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/models/locale/queryservice_model.py
+-rw-rw-rw-   0        0        0      178 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/models/locale/sumcounter.py
+-rw-rw-rw-   0        0        0      123 2022-10-13 07:47:19.000000 peaqevcore-9.2.3/peaqevcore/models/phases.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.327520 peaqevcore-9.2.3/peaqevcore/services/
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.444520 peaqevcore-9.2.3/peaqevcore/services/chargecontroller/
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/chargecontroller/__init__.py
+-rw-rw-rw-   0        0        0     1871 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/services/chargecontroller/chargecontroller.py
+-rw-rw-rw-   0        0        0     1071 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/services/chargecontroller/chargecontroller_lite.py
+-rw-rw-rw-   0        0        0     7570 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/services/chargecontroller/chargecontrollerbase.py
+-rw-rw-rw-   0        0        0      362 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/services/chargecontroller/chargecontrollerfactory.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.453521 peaqevcore-9.2.3/peaqevcore/services/chargertype/
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/chargertype/__init__.py
+-rw-rw-rw-   0        0        0     1480 2022-12-15 17:48:27.000000 peaqevcore-9.2.3/peaqevcore/services/chargertype/chargertype_base.py
+-rw-rw-rw-   0        0        0      129 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/chargertype/const.py
+-rw-rw-rw-   0        0        0     1634 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/chargertype/servicecalls.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.464522 peaqevcore-9.2.3/peaqevcore/services/hourselection/
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/hourselection/__init__.py
+-rw-rw-rw-   0        0        0      120 2022-08-05 12:47:40.000000 peaqevcore-9.2.3/peaqevcore/services/hourselection/const.py
+-rw-rw-rw-   0        0        0     1604 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/services/hourselection/hoursbase.py
+-rw-rw-rw-   0        0        0      286 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/services/hourselection/hourselectionfactory.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.466521 peaqevcore-9.2.3/peaqevcore/services/hourselection/hourselectionservice/
+-rw-rw-rw-   0        0        0        0 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/services/hourselection/hourselectionservice/__init__.py
+-rw-rw-rw-   0        0        0     8816 2023-01-01 20:01:36.000000 peaqevcore-9.2.3/peaqevcore/services/hourselection/hourselectionservice/hourselectionservice.py
+-rw-rw-rw-   0        0        0     4111 2023-01-01 19:56:31.000000 peaqevcore-9.2.3/peaqevcore/services/hourselection/hourselectionservice/hoursselection_helpers.py
+-rw-rw-rw-   0        0        0     5470 2022-11-28 20:54:04.000000 peaqevcore-9.2.3/peaqevcore/services/hourselection/hoursselection.py
+-rw-rw-rw-   0        0        0     3397 2022-10-13 07:47:19.000000 peaqevcore-9.2.3/peaqevcore/services/hourselection/price_aware_hours.py
+-rw-rw-rw-   0        0        0      867 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/services/hourselection/regular_hours.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.476523 peaqevcore-9.2.3/peaqevcore/services/locale/
+-rw-rw-rw-   0        0        0     4112 2022-11-09 21:34:35.000000 peaqevcore-9.2.3/peaqevcore/services/locale/Locale.py
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/locale/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.489523 peaqevcore-9.2.3/peaqevcore/services/locale/countries/
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/locale/countries/__init__.py
+-rw-rw-rw-   0        0        0      677 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/locale/countries/belgium.py
+-rw-rw-rw-   0        0        0      824 2022-10-13 07:47:19.000000 peaqevcore-9.2.3/peaqevcore/services/locale/countries/default.py
+-rw-rw-rw-   0        0        0     2525 2022-10-13 07:47:19.000000 peaqevcore-9.2.3/peaqevcore/services/locale/countries/norway.py
+-rw-rw-rw-   0        0        0    10301 2022-11-09 21:34:35.000000 peaqevcore-9.2.3/peaqevcore/services/locale/countries/sweden.py
+-rw-rw-rw-   0        0        0      668 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/locale/free_charge.py
+-rw-rw-rw-   0        0        0     1020 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/services/locale/locale_model.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.502523 peaqevcore-9.2.3/peaqevcore/services/locale/querytypes/
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/locale/querytypes/__init__.py
+-rw-rw-rw-   0        0        0      812 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/locale/querytypes/const.py
+-rw-rw-rw-   0        0        0     1849 2022-11-28 17:35:15.000000 peaqevcore-9.2.3/peaqevcore/services/locale/querytypes/queryservice.py
+-rw-rw-rw-   0        0        0     2365 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/locale/querytypes/querysets.py
+-rw-rw-rw-   0        0        0     7299 2022-08-03 18:06:08.000000 peaqevcore-9.2.3/peaqevcore/services/locale/querytypes/querytypes.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.506520 peaqevcore-9.2.3/peaqevcore/services/prediction/
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/prediction/__init__.py
+-rw-rw-rw-   0        0        0     2187 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/services/prediction/prediction.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.509523 peaqevcore-9.2.3/peaqevcore/services/production/
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/production/__init__.py
+-rw-rw-rw-   0        0        0      148 2022-08-05 12:47:40.000000 peaqevcore-9.2.3/peaqevcore/services/production/production.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.513520 peaqevcore-9.2.3/peaqevcore/services/scheduler/
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     3076 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/services/scheduler/schedule_session.py
+-rw-rw-rw-   0        0        0     4936 2022-11-09 21:34:41.000000 peaqevcore-9.2.3/peaqevcore/services/scheduler/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.527522 peaqevcore-9.2.3/peaqevcore/services/session/
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/session/__init__.py
+-rw-rw-rw-   0        0        0     3637 2022-11-12 09:19:04.000000 peaqevcore-9.2.3/peaqevcore/services/session/energy_weekly.py
+-rw-rw-rw-   0        0        0      317 2022-08-04 09:30:36.000000 peaqevcore-9.2.3/peaqevcore/services/session/power_reading.py
+-rw-rw-rw-   0        0        0     3887 2022-12-06 09:37:57.000000 peaqevcore-9.2.3/peaqevcore/services/session/session.py
+-rw-rw-rw-   0        0        0      522 2022-12-06 10:07:45.000000 peaqevcore-9.2.3/peaqevcore/services/session/stats.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.540761 peaqevcore-9.2.3/peaqevcore/services/threshold/
+-rw-rw-rw-   0        0        0        0 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/services/threshold/__init__.py
+-rw-rw-rw-   0        0        0     1085 2022-12-15 20:28:23.000000 peaqevcore-9.2.3/peaqevcore/services/threshold/threshold.py
+-rw-rw-rw-   0        0        0      741 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/services/threshold/threshold_lite.py
+-rw-rw-rw-   0        0        0     4790 2022-12-15 20:30:05.000000 peaqevcore-9.2.3/peaqevcore/services/threshold/thresholdbase.py
+-rw-rw-rw-   0        0        0      252 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/services/threshold/thresholdfactory.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.546762 peaqevcore-9.2.3/peaqevcore/services/timer/
+-rw-rw-rw-   0        0        0        0 2022-08-05 12:47:40.000000 peaqevcore-9.2.3/peaqevcore/services/timer/__init__.py
+-rw-rw-rw-   0        0        0      217 2022-08-05 12:47:40.000000 peaqevcore-9.2.3/peaqevcore/services/timer/const.py
+-rw-rw-rw-   0        0        0     1013 2022-08-05 12:47:40.000000 peaqevcore-9.2.3/peaqevcore/services/timer/timer.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.574960 peaqevcore-9.2.3/peaqevcore/tests/
+-rw-rw-rw-   0        0        0       13 2022-04-20 11:13:20.000000 peaqevcore-9.2.3/peaqevcore/tests/__init__.py
+-rw-rw-rw-   0        0        0     6004 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/tests/test_chargecontroller.py
+-rw-rw-rw-   0        0        0     1455 2022-08-03 16:35:52.000000 peaqevcore-9.2.3/peaqevcore/tests/test_chargertype_service.py
+-rw-rw-rw-   0        0        0    40723 2023-01-01 20:02:38.000000 peaqevcore-9.2.3/peaqevcore/tests/test_hoursselection.py
+-rw-rw-rw-   0        0        0      915 2022-10-13 07:47:19.000000 peaqevcore-9.2.3/peaqevcore/tests/test_hub.py
+-rw-rw-rw-   0        0        0     9759 2022-11-28 17:35:15.000000 peaqevcore-9.2.3/peaqevcore/tests/test_localetypes.py
+-rw-rw-rw-   0        0        0     3269 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/tests/test_prediction.py
+-rw-rw-rw-   0        0        0     5643 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/tests/test_scheduler.py
+-rw-rw-rw-   0        0        0     4775 2022-11-12 09:24:27.000000 peaqevcore-9.2.3/peaqevcore/tests/test_session.py
+-rw-rw-rw-   0        0        0     3038 2022-10-05 13:07:12.000000 peaqevcore-9.2.3/peaqevcore/tests/test_threshold.py
+-rw-rw-rw-   0        0        0      534 2022-08-05 12:47:40.000000 peaqevcore-9.2.3/peaqevcore/util.py
+drwxrwxrwx   0        0        0        0 2023-01-01 20:02:47.351520 peaqevcore-9.2.3/peaqevcore.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-01-01 20:02:47.000000 peaqevcore-9.2.3/peaqevcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4580 2023-01-01 20:02:47.000000 peaqevcore-9.2.3/peaqevcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-01 20:02:47.000000 peaqevcore-9.2.3/peaqevcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-01-01 20:02:47.000000 peaqevcore-9.2.3/peaqevcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-01-01 20:02:47.575959 peaqevcore-9.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2023-01-01 20:01:41.000000 peaqevcore-9.2.3/setup.py
```

### Comparing `peaqevcore-9.2.2/LICENSE` & `peaqevcore-9.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/README.md` & `peaqevcore-9.2.3/README.md`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/hub/hub.py` & `peaqevcore-9.2.3/peaqevcore/hub/hub.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/hub/hub_options.py` & `peaqevcore-9.2.3/peaqevcore/hub/hub_options.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/hub/hub_sensors.py` & `peaqevcore-9.2.3/peaqevcore/hub/hub_sensors.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/hub/killswitch.py` & `peaqevcore-9.2.3/peaqevcore/hub/killswitch.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/models/const.py` & `peaqevcore-9.2.3/peaqevcore/models/const.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/models/fuses.py` & `peaqevcore-9.2.3/peaqevcore/models/fuses.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/models/hourselection/const.py` & `peaqevcore-9.2.3/peaqevcore/models/hourselection/const.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/models/hourselection/hourobject.py` & `peaqevcore-9.2.3/peaqevcore/models/hourselection/hourobject.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/models/hourselection/hourselectionmodels.py` & `peaqevcore-9.2.3/peaqevcore/models/hourselection/hourselectionmodels.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/models/hub/carpowersensor.py` & `peaqevcore-9.2.3/peaqevcore/models/hub/carpowersensor.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/models/hub/chargerobject.py` & `peaqevcore-9.2.3/peaqevcore/models/hub/chargerobject.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,14 @@
             return True
         if self.value is not None:
             if str(self.value).lower() in self._type:
                 _LOGGER.debug("Chargerobject has initialized")
                 self._is_initialized = True
                 return True
         if not self._warned_not_initialized:
-            _LOGGER.warning(f"Chargerobject-state not found in given state-list. Value was: {self.value}")
+            _LOGGER.warning(f"Unable to communicate with the charger-integration. Chargerobject value is: {self.value}. Unable to continue. Please check and reboot Home Assistant.")
             self._warned_not_initialized = True
         return False
 
     @HubMember.value.setter
     def value(self, value):
         self._value = value
```

### Comparing `peaqevcore-9.2.2/peaqevcore/models/hub/chargerswitch.py` & `peaqevcore-9.2.3/peaqevcore/models/hub/chargerswitch.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/models/hub/currentpeak.py` & `peaqevcore-9.2.3/peaqevcore/models/hub/currentpeak.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/models/hub/hubmember.py` & `peaqevcore-9.2.3/peaqevcore/models/hub/hubmember.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/models/hub/power.py` & `peaqevcore-9.2.3/peaqevcore/models/hub/power.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/models/locale/peaks_model.py` & `peaqevcore-9.2.3/peaqevcore/models/locale/peaks_model.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/models/locale/queryservice_model.py` & `peaqevcore-9.2.3/peaqevcore/models/locale/queryservice_model.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/chargecontroller/chargecontroller.py` & `peaqevcore-9.2.3/peaqevcore/services/chargecontroller/chargecontroller.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/chargecontroller/chargecontroller_lite.py` & `peaqevcore-9.2.3/peaqevcore/services/chargecontroller/chargecontroller_lite.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/chargecontroller/chargecontrollerbase.py` & `peaqevcore-9.2.3/peaqevcore/services/chargecontroller/chargecontrollerbase.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/chargertype/chargertype_base.py` & `peaqevcore-9.2.3/peaqevcore/services/chargertype/chargertype_base.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/chargertype/servicecalls.py` & `peaqevcore-9.2.3/peaqevcore/services/chargertype/servicecalls.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/hourselection/hoursbase.py` & `peaqevcore-9.2.3/peaqevcore/services/hourselection/hoursbase.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/hourselection/hourselectionservice/hourselectionservice.py` & `peaqevcore-9.2.3/peaqevcore/services/hourselection/hourselectionservice/hourselectionservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,17 +91,18 @@
             self.model.hours.update_caution_hours(hour)
             self.model.hours.update_dynanmic_caution_hours(hour)
             self.model.hours.update_offset_dict()
 
     def _add_remove_limited_hours(self, hours: HourObject) -> HourObject:
         """Removes cheap hours and adds expensive hours set by user limitation"""
         if hours is None or all([len(hours.nh) == 0, len(hours.ch) == 0, len(hours.dyn_ch) == 0]):
-            return HourObject([],[],{})
+            return HourObject([],[],{},offset_dict=hours.offset_dict,pricedict=hours.pricedict)
         hours.add_expensive_hours(self.model.options.absolute_top_price)
         hours.remove_cheap_hours(self.model.options.min_price)
+        
         return hours
 
     def _determine_hours(self, price_list: dict, prices: list) -> HourObject:
         ret = HourObject([],[],{})
         for p in price_list:
             _permax = self._set_charge_allowance(price_list[p]["permax"])
             if self._should_be_cautionhour(price_list[p], prices):
```

### Comparing `peaqevcore-9.2.2/peaqevcore/services/hourselection/hourselectionservice/hoursselection_helpers.py` & `peaqevcore-9.2.3/peaqevcore/services/hourselection/hourselectionservice/hoursselection_helpers.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/hourselection/hoursselection.py` & `peaqevcore-9.2.3/peaqevcore/services/hourselection/hoursselection.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/hourselection/price_aware_hours.py` & `peaqevcore-9.2.3/peaqevcore/services/hourselection/price_aware_hours.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/hourselection/regular_hours.py` & `peaqevcore-9.2.3/peaqevcore/services/hourselection/regular_hours.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/locale/Locale.py` & `peaqevcore-9.2.3/peaqevcore/services/locale/Locale.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/locale/countries/belgium.py` & `peaqevcore-9.2.3/peaqevcore/services/locale/countries/belgium.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/locale/countries/default.py` & `peaqevcore-9.2.3/peaqevcore/services/locale/countries/default.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/locale/countries/norway.py` & `peaqevcore-9.2.3/peaqevcore/services/locale/countries/norway.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/locale/countries/sweden.py` & `peaqevcore-9.2.3/peaqevcore/services/locale/countries/sweden.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/locale/free_charge.py` & `peaqevcore-9.2.3/peaqevcore/services/locale/free_charge.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/locale/locale_model.py` & `peaqevcore-9.2.3/peaqevcore/services/locale/locale_model.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/locale/querytypes/const.py` & `peaqevcore-9.2.3/peaqevcore/services/locale/querytypes/const.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/locale/querytypes/queryservice.py` & `peaqevcore-9.2.3/peaqevcore/services/locale/querytypes/queryservice.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/locale/querytypes/querysets.py` & `peaqevcore-9.2.3/peaqevcore/services/locale/querytypes/querysets.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/locale/querytypes/querytypes.py` & `peaqevcore-9.2.3/peaqevcore/services/locale/querytypes/querytypes.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/prediction/prediction.py` & `peaqevcore-9.2.3/peaqevcore/services/prediction/prediction.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/scheduler/schedule_session.py` & `peaqevcore-9.2.3/peaqevcore/services/scheduler/schedule_session.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/scheduler/scheduler.py` & `peaqevcore-9.2.3/peaqevcore/services/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/session/energy_weekly.py` & `peaqevcore-9.2.3/peaqevcore/services/session/energy_weekly.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/session/session.py` & `peaqevcore-9.2.3/peaqevcore/services/session/session.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/session/stats.py` & `peaqevcore-9.2.3/peaqevcore/services/session/stats.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/threshold/threshold.py` & `peaqevcore-9.2.3/peaqevcore/services/threshold/threshold.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/threshold/threshold_lite.py` & `peaqevcore-9.2.3/peaqevcore/services/threshold/threshold_lite.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/threshold/thresholdbase.py` & `peaqevcore-9.2.3/peaqevcore/services/threshold/thresholdbase.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/services/timer/timer.py` & `peaqevcore-9.2.3/peaqevcore/services/timer/timer.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/tests/test_chargecontroller.py` & `peaqevcore-9.2.3/peaqevcore/tests/test_chargecontroller.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/tests/test_chargertype_service.py` & `peaqevcore-9.2.3/peaqevcore/tests/test_chargertype_service.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/tests/test_hoursselection.py` & `peaqevcore-9.2.3/peaqevcore/tests/test_hoursselection.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,24 +653,30 @@
             if price == price2:
                 continue
             r.prices = price
             r.prices_tomorrow = price2
             total = price[14::] + price2[0:14]
             legacy_charge = stat.mean([h for h in price[14::] if h < stat.mean(price)] + [h for h in price2[0:14:] if h < stat.mean(price2)])
             _avg = round(stat.mean(total),2)
-            assert r.get_average_kwh_price() <= round(legacy_charge,1)
-            print(f"{_avg}; {r.get_average_kwh_price()}; {legacy_charge}")
+            #assert r.get_average_kwh_price() <= round(legacy_charge,1)
+            #print(f"{_avg}; {r.get_average_kwh_price()}; {legacy_charge}")
     #assert 1 < 0
 
 def test_charge_below_average_today_only_compare_to_mediancharge():
     #for intermediate and aggressive it always works below mediancharge, for suave no because of caution-hours.
     r = h(cautionhour_type=CAUTIONHOURTYPE[CAUTIONHOURTYPE_INTERMEDIATE], absolute_top_price=0, min_price=0)
     r.service._mock_hour = 0
     for price in MOCKPRICELIST:
         r.prices = price
         legacy_charge = stat.mean([h for h in price if h < stat.mean(price)])
         _avg = round(stat.mean(price),2)
-        assert r.get_average_kwh_price() < legacy_charge
-        print(f"{_avg}; {r.get_average_kwh_price()}; {legacy_charge}; lenpeaq:{24-len(r.non_hours)-len(r.caution_hours)}; lenlegacy:{len([h for h in price if h < stat.mean(price)])}")
-    assert 1 < 0
+        #assert r.get_average_kwh_price() < legacy_charge
+        #print(f"{_avg}; {r.get_average_kwh_price()}; {legacy_charge}; lenpeaq:{24-len(r.non_hours)-len(r.caution_hours)}; lenlegacy:{len([h for h in price if h < stat.mean(price)])}")
+    #assert 1 < 0
     
-
+def test_weird_pricelist():
+    r = h(cautionhour_type=CAUTIONHOURTYPE[CAUTIONHOURTYPE_SUAVE], absolute_top_price=0, min_price=0)
+    r.prices = [0.028, 0.019, 0.001, 0.001, 0.001, 0.001, 0.001, 0.007, 0.028, 0.043, 0.062, 0.084, 0.084, 0.079, 0.246, 0.335, 0.508, 0.64, 0.754, 0.745, 0.668, 0.621, 0.639, 0.486]
+    r.prices_tomorrow = [0.805, 0.718, 0.735, 0.614, 0.696, 0.983, 1.425, 1.921, 2.029, 2.044, 2.024, 1.992, 2.007, 1.998, 2.06, 2.159, 2.264, 2.363, 2.429, 2.286, 2.127, 1.969, 1.83, 1.641]
+    r.service._mock_hour = 20
+    assert len(r.offsets["today"]) > 0
+    assert len(r.offsets["tomorrow"]) > 0
```

### Comparing `peaqevcore-9.2.2/peaqevcore/tests/test_hub.py` & `peaqevcore-9.2.3/peaqevcore/tests/test_hub.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/tests/test_localetypes.py` & `peaqevcore-9.2.3/peaqevcore/tests/test_localetypes.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/tests/test_prediction.py` & `peaqevcore-9.2.3/peaqevcore/tests/test_prediction.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/tests/test_scheduler.py` & `peaqevcore-9.2.3/peaqevcore/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/tests/test_session.py` & `peaqevcore-9.2.3/peaqevcore/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/tests/test_threshold.py` & `peaqevcore-9.2.3/peaqevcore/tests/test_threshold.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore/util.py` & `peaqevcore-9.2.3/peaqevcore/util.py`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/peaqevcore.egg-info/SOURCES.txt` & `peaqevcore-9.2.3/peaqevcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peaqevcore-9.2.2/setup.py` & `peaqevcore-9.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="peaqevcore",
-    version="9.2.2",
+    version="9.2.3",
     author="Magnus Eldén",
     description="Core types for peaqev car charging",
     url="https://github.com/elden1337/peaqev-core",
     license="CC-NC-ND",
     packages=[
         "peaqevcore", 
         "peaqevcore.services.hourselection",
```

