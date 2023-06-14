# Comparing `tmp/prot-3.8.4.tar.gz` & `tmp/prot-3.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\prot-3.8.4.tar", last modified: Sat Jul 25 09:19:45 2020, max compression
+gzip compressed data, was "prot-3.8.5.tar", last modified: Wed Jun 14 19:45:20 2023, max compression
```

## Comparing `prot-3.8.4.tar` & `prot-3.8.5.tar`

### file list

```diff
@@ -1,309 +1,298 @@
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:45.149805 prot-3.8.4/
--rw-rw-rw-   0        0        0       31 2020-07-11 10:48:19.000000 prot-3.8.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2400 2020-07-25 09:19:45.147805 prot-3.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     1389 2020-04-02 21:20:31.000000 prot-3.8.4/README.md
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:40.215805 prot-3.8.4/protbuilder/
--rw-rw-rw-   0        0        0    46645 2020-07-11 09:57:36.000000 prot-3.8.4/protbuilder/__init__.pyc
--rw-rw-rw-   0        0        0      138 2020-07-11 09:57:36.000000 prot-3.8.4/protbuilder/__version__.pyc
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:40.349805 prot-3.8.4/protbuilder/color/
--rw-rw-rw-   0        0        0      371 2020-07-11 09:57:36.000000 prot-3.8.4/protbuilder/color/__init__.pyc
--rw-rw-rw-   0        0        0     3011 2020-07-11 09:57:36.000000 prot-3.8.4/protbuilder/color/ansi.pyc
--rw-rw-rw-   0        0        0     6729 2020-07-11 09:57:36.000000 prot-3.8.4/protbuilder/color/ansitowin32.pyc
--rw-rw-rw-   0        0        0     1632 2020-07-11 09:57:36.000000 prot-3.8.4/protbuilder/color/initialise.pyc
--rw-rw-rw-   0        0        0     3771 2020-07-11 09:57:36.000000 prot-3.8.4/protbuilder/color/win32.pyc
--rw-rw-rw-   0        0        0     4592 2020-07-11 09:57:36.000000 prot-3.8.4/protbuilder/color/winterm.pyc
--rw-rw-rw-   0        0        0       42 2020-07-25 09:19:45.152805 prot-3.8.4/setup.cfg
--rw-rw-rw-   0        0        0      789 2020-07-11 11:47:28.000000 prot-3.8.4/setup.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:40.036805 prot-3.8.4/src/
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:40.518805 prot-3.8.4/src/prot/
--rw-rw-rw-   0        0        0    40407 2020-07-23 19:30:41.000000 prot-3.8.4/src/prot/__init__.py
--rw-rw-rw-   0        0        0     3123 2020-07-06 15:37:28.000000 prot-3.8.4/src/prot/__main__.py
--rw-rw-rw-   0        0        0       21 2020-07-25 09:18:56.000000 prot-3.8.4/src/prot/__version__.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:40.629805 prot-3.8.4/src/prot/bs/
--rw-rw-rw-   0        0        0      185 2020-07-23 19:28:37.000000 prot-3.8.4/src/prot/bs/__init__.py
--rw-rw-rw-   0        0        0     5694 2020-07-23 20:43:51.000000 prot-3.8.4/src/prot/bs/bs.py
--rw-rw-rw-   0        0        0     2262 2020-07-23 19:40:18.000000 prot-3.8.4/src/prot/bs/bsMap.py
--rw-rw-rw-   0        0        0      801 2020-07-23 16:18:27.000000 prot-3.8.4/src/prot/bs/bsPro.py
--rw-rw-rw-   0        0        0     1281 2020-07-23 20:41:03.000000 prot-3.8.4/src/prot/bs/bsSpaz.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:42.609805 prot-3.8.4/src/prot/bs/stdLib/
--rw-rw-rw-   0        0        0      201 2020-07-25 09:12:28.000000 prot-3.8.4/src/prot/bs/stdLib/__init__.py
--rw-rw-rw-   0        0        0     2189 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/alwaysLandLevelDefs.py
--rw-rw-rw-   0        0        0     4352 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bigGDefs.py
--rw-rw-rw-   0        0        0     1568 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bridgitLevelDefs.py
--rw-rw-rw-   0        0        0     2261 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bs.py
--rw-rw-rw-   0        0        0    37874 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsAchievement.py
--rw-rw-rw-   0        0        0     8330 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsAssault.py
--rw-rw-rw-   0        0        0    34286 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsBomb.py
--rw-rw-rw-   0        0        0    18154 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsCaptureTheFlag.py
--rw-rw-rw-   0        0        0    11373 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsChosenOne.py
--rw-rw-rw-   0        0        0     9234 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsConquest.py
--rw-rw-rw-   0        0        0    96453 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsCoopGame.py
--rw-rw-rw-   0        0        0     5888 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsDeathMatch.py
--rw-rw-rw-   0        0        0     9248 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsEasterEggHunt.py
--rw-rw-rw-   0        0        0    19687 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsElimination.py
--rw-rw-rw-   0        0        0    10709 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsFlag.py
--rw-rw-rw-   0        0        0    27224 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsFootball.py
--rw-rw-rw-   0        0        0   116735 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsGame.py
--rw-rw-rw-   0        0        0    12498 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsHockey.py
--rw-rw-rw-   0        0        0      181 2020-07-24 16:28:41.000000 prot-3.8.4/src/prot/bs/stdLib/bsInternal.py
--rw-rw-rw-   0        0        0     7611 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsKeepAway.py
--rw-rw-rw-   0        0        0     8972 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsKingOfTheHill.py
--rw-rw-rw-   0        0        0   155086 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageArabic.py
--rw-rw-rw-   0        0        0   158524 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageBelarussian.py
--rw-rw-rw-   0        0        0   127437 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageChinese.py
--rw-rw-rw-   0        0        0   118386 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageCroatian.py
--rw-rw-rw-   0        0        0   135541 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageCzech.py
--rw-rw-rw-   0        0        0    94441 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageDanish.py
--rw-rw-rw-   0        0        0   141350 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageDutch.py
--rw-rw-rw-   0        0        0   111226 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageEnglish.py
--rw-rw-rw-   0        0        0   105204 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageEsperanto.py
--rw-rw-rw-   0        0        0   146287 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageFrench.py
--rw-rw-rw-   0        0        0   148309 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageGerman.py
--rw-rw-rw-   0        0        0   141903 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageGibberish.py
--rw-rw-rw-   0        0        0   187394 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageGreek.py
--rw-rw-rw-   0        0        0   212586 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageHindi.py
--rw-rw-rw-   0        0        0   137372 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageHungarian.py
--rw-rw-rw-   0        0        0   126188 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageIndonesian.py
--rw-rw-rw-   0        0        0   144849 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageItalian.py
--rw-rw-rw-   0        0        0   138448 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageKorean.py
--rw-rw-rw-   0        0        0   162405 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguagePersian.py
--rw-rw-rw-   0        0        0   144892 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguagePolish.py
--rw-rw-rw-   0        0        0   145117 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguagePortuguese.py
--rw-rw-rw-   0        0        0   121744 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageRomanian.py
--rw-rw-rw-   0        0        0   183660 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageRussian.py
--rw-rw-rw-   0        0        0   168786 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageSerbian.py
--rw-rw-rw-   0        0        0   142925 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageSpanish.py
--rw-rw-rw-   0        0        0   125252 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageSwedish.py
--rw-rw-rw-   0        0        0   129359 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageTurkish.py
--rw-rw-rw-   0        0        0   169058 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLanguageUkrainian.py
--rw-rw-rw-   0        0        0    34599 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsLobby.py
--rw-rw-rw-   0        0        0    37628 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsMainMenu.py
--rw-rw-rw-   0        0        0    58253 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsMap.py
--rw-rw-rw-   0        0        0     9381 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsMeteorShower.py
--rw-rw-rw-   0        0        0     6444 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsNinjaFight.py
--rw-rw-rw-   0        0        0    48080 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsOnslaught.py
--rw-rw-rw-   0        0        0    11026 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsPowerup.py
--rw-rw-rw-   0        0        0    24920 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsRace.py
--rw-rw-rw-   0        0        0    43185 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsRunaround.py
--rw-rw-rw-   0        0        0    12031 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsScoreBoard.py
--rw-rw-rw-   0        0        0    12856 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsScoreSet.py
--rw-rw-rw-   0        0        0    18997 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsServerData.py
--rw-rw-rw-   0        0        0   141126 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsSpaz.py
--rw-rw-rw-   0        0        0    12571 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsTargetPractice.py
--rw-rw-rw-   0        0        0    58723 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsTeamGame.py
--rw-rw-rw-   0        0        0    10326 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsTheLastStand.py
--rw-rw-rw-   0        0        0    63826 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsTutorial.py
--rw-rw-rw-   0        0        0  1093681 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsUI.py
--rw-rw-rw-   0        0        0    53124 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsUI2.py
--rw-rw-rw-   0        0        0   188532 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/bsUtils.py
--rw-rw-rw-   0        0        0     3224 2020-07-24 17:03:48.000000 prot-3.8.4/src/prot/bs/stdLib/bsVector.py
--rw-rw-rw-   0        0        0     3767 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/courtyardLevelDefs.py
--rw-rw-rw-   0        0        0     2120 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/cragCastleDefs.py
--rw-rw-rw-   0        0        0     1635 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/doomShroomLevelDefs.py
--rw-rw-rw-   0        0        0     1513 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/footballStadiumDefs.py
--rw-rw-rw-   0        0        0     1360 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/hockeyStadiumDefs.py
--rw-rw-rw-   0        0        0     4179 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/lakeFrigidDefs.py
--rw-rw-rw-   0        0        0     1674 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/monkeyFaceLevelDefs.py
--rw-rw-rw-   0        0        0     1448 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/rampageLevelDefs.py
--rw-rw-rw-   0        0        0     1491 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/roundaboutLevelDefs.py
--rw-rw-rw-   0        0        0     2377 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/stepRightUpLevelDefs.py
--rw-rw-rw-   0        0        0     1719 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/thePadLevelDefs.py
--rw-rw-rw-   0        0        0     2028 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/tipTopLevelDefs.py
--rw-rw-rw-   0        0        0     3284 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/towerDLevelDefs.py
--rw-rw-rw-   0        0        0     2234 2019-08-02 23:32:10.000000 prot-3.8.4/src/prot/bs/stdLib/zigZagLevelDefs.py
--rw-rw-rw-   0        0        0    12491 2020-04-23 20:02:06.000000 prot-3.8.4/src/prot/code.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:42.716805 prot-3.8.4/src/prot/color/
--rw-rw-rw-   0        0        0      239 2020-03-16 16:00:34.000000 prot-3.8.4/src/prot/color/__init__.py
--rw-rw-rw-   0        0        0     2524 2020-03-16 16:00:34.000000 prot-3.8.4/src/prot/color/ansi.py
--rw-rw-rw-   0        0        0    10462 2020-03-16 16:00:34.000000 prot-3.8.4/src/prot/color/ansitowin32.py
--rw-rw-rw-   0        0        0     1915 2020-03-16 16:00:34.000000 prot-3.8.4/src/prot/color/initialise.py
--rw-rw-rw-   0        0        0     5404 2020-03-16 16:00:34.000000 prot-3.8.4/src/prot/color/win32.py
--rw-rw-rw-   0        0        0     6438 2020-03-16 16:00:34.000000 prot-3.8.4/src/prot/color/winterm.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:42.762805 prot-3.8.4/src/prot/pip/
--rw-rw-rw-   0        0        0     9441 2020-04-05 08:16:08.000000 prot-3.8.4/src/prot/pip/__init__.py
--rw-rw-rw-   0        0        0     1901 2020-04-05 08:16:49.000000 prot-3.8.4/src/prot/pip/__main__.py
--rw-rw-rw-   0        0        0      755 2020-04-03 08:54:55.000000 prot-3.8.4/src/prot/pip/extra.py
--rw-rw-rw-   0        0        0  4056147 2020-07-11 10:09:51.000000 prot-3.8.4/src/prot/pip/packagesList.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:42.820805 prot-3.8.4/src/prot/progress/
--rw-rw-rw-   0        0        0     4910 2020-04-04 16:37:41.000000 prot-3.8.4/src/prot/progress/__init__.py
--rw-rw-rw-   0        0        0     2854 2020-03-21 18:35:45.000000 prot-3.8.4/src/prot/progress/bar.py
--rw-rw-rw-   0        0        0     1372 2020-03-21 18:35:45.000000 prot-3.8.4/src/prot/progress/counter.py
--rw-rw-rw-   0        0        0     1380 2020-03-21 18:35:45.000000 prot-3.8.4/src/prot/progress/spinner.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:43.114805 prot-3.8.4/src/prot/prompt/
--rw-rw-rw-   0        0        0      872 2020-03-06 02:24:16.000000 prot-3.8.4/src/prot/prompt/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:43.168805 prot-3.8.4/src/prot/prompt/application/
--rw-rw-rw-   0        0        0      519 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/application/__init__.py
--rw-rw-rw-   0        0        0    44248 2020-07-09 14:50:16.000000 prot-3.8.4/src/prot/prompt/application/application.py
--rw-rw-rw-   0        0        0     5051 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/application/current.py
--rw-rw-rw-   0        0        0     1349 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/application/dummy.py
--rw-rw-rw-   0        0        0     3699 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/application/run_in_terminal.py
--rw-rw-rw-   0        0        0     5919 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/auto_suggest.py
--rw-rw-rw-   0        0        0    70342 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/buffer.py
--rw-rw-rw-   0        0        0     3768 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/cache.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:43.193805 prot-3.8.4/src/prot/prompt/clipboard/
--rw-rw-rw-   0        0        0      403 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/clipboard/__init__.py
--rw-rw-rw-   0        0        0     2489 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/clipboard/base.py
--rw-rw-rw-   0        0        0     1077 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/clipboard/in_memory.py
--rw-rw-rw-   0        0        0     1147 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/clipboard/pyperclip.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:43.264805 prot-3.8.4/src/prot/prompt/completion/
--rw-rw-rw-   0        0        0      810 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/completion/__init__.py
--rw-rw-rw-   0        0        0    11493 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/completion/base.py
--rw-rw-rw-   0        0        0     3832 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/completion/filesystem.py
--rw-rw-rw-   0        0        0     6945 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/completion/fuzzy_completer.py
--rw-rw-rw-   0        0        0     3885 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/completion/nested.py
--rw-rw-rw-   0        0        0     2934 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/completion/word_completer.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:43.277805 prot-3.8.4/src/prot/prompt/contrib/
--rw-rw-rw-   0        0        0        0 2020-01-12 12:31:42.000000 prot-3.8.4/src/prot/prompt/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:43.280805 prot-3.8.4/src/prot/prompt/contrib/completers/
--rw-rw-rw-   0        0        0       36 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/contrib/completers/__init__.py
--rw-rw-rw-   0        0        0     2012 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/contrib/completers/system.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:43.338805 prot-3.8.4/src/prot/prompt/contrib/regular_languages/
--rw-rw-rw-   0        0        0     3220 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/contrib/regular_languages/__init__.py
--rw-rw-rw-   0        0        0    21889 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/contrib/regular_languages/compiler.py
--rw-rw-rw-   0        0        0     3239 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/contrib/regular_languages/completion.py
--rw-rw-rw-   0        0        0     3386 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/contrib/regular_languages/lexer.py
--rw-rw-rw-   0        0        0     7827 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/contrib/regular_languages/regex_parser.py
--rw-rw-rw-   0        0        0     2035 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/contrib/regular_languages/validation.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:43.356804 prot-3.8.4/src/prot/prompt/contrib/ssh/
--rw-rw-rw-   0        0        0      138 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/contrib/ssh/__init__.py
--rw-rw-rw-   0        0        0     4365 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/contrib/ssh/server.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:43.393804 prot-3.8.4/src/prot/prompt/contrib/telnet/
--rw-rw-rw-   0        0        0       68 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/contrib/telnet/__init__.py
--rw-rw-rw-   0        0        0      130 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/contrib/telnet/log.py
--rw-rw-rw-   0        0        0     4974 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/contrib/telnet/protocol.py
--rw-rw-rw-   0        0        0     9518 2020-03-31 14:52:56.000000 prot-3.8.4/src/prot/prompt/contrib/telnet/server.py
--rw-rw-rw-   0        0        0      187 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/data_structures.py
--rw-rw-rw-   0        0        0    40593 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/document.py
--rw-rw-rw-   0        0        0      322 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/enums.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:43.591805 prot-3.8.4/src/prot/prompt/eventloop/
--rw-rw-rw-   0        0        0      636 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/eventloop/__init__.py
--rw-rw-rw-   0        0        0     4125 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/eventloop/async_context_manager.py
--rw-rw-rw-   0        0        0     1711 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/eventloop/async_generator.py
--rw-rw-rw-   0        0        0     1117 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/eventloop/dummy_contextvars.py
--rw-rw-rw-   0        0        0     5514 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/eventloop/inputhook.py
--rw-rw-rw-   0        0        0     3251 2020-03-06 01:48:12.000000 prot-3.8.4/src/prot/prompt/eventloop/utils.py
--rw-rw-rw-   0        0        0     2008 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/eventloop/win32.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:43.624805 prot-3.8.4/src/prot/prompt/filters/
--rw-rw-rw-   0        0        0     1028 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/filters/__init__.py
--rw-rw-rw-   0        0        0     9276 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/filters/app.py
--rw-rw-rw-   0        0        0     5737 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/filters/base.py
--rw-rw-rw-   0        0        0     1830 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/filters/cli.py
--rw-rw-rw-   0        0        0      848 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/filters/utils.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:43.789804 prot-3.8.4/src/prot/prompt/formatted_text/
--rw-rw-rw-   0        0        0     1378 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/formatted_text/__init__.py
--rw-rw-rw-   0        0        0     8089 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/formatted_text/ansi.py
--rw-rw-rw-   0        0        0     4881 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/formatted_text/base.py
--rw-rw-rw-   0        0        0     4328 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/formatted_text/html.py
--rw-rw-rw-   0        0        0      756 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/formatted_text/pygments.py
--rw-rw-rw-   0        0        0     2747 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/formatted_text/utils.py
--rw-rw-rw-   0        0        0     7131 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/history.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:43.925805 prot-3.8.4/src/prot/prompt/input/
--rw-rw-rw-   0        0        0      209 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/input/__init__.py
--rw-rw-rw-   0        0        0    13116 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/input/ansi_escape_sequences.py
--rw-rw-rw-   0        0        0     3275 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/input/base.py
--rw-rw-rw-   0        0        0     1522 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/input/defaults.py
--rw-rw-rw-   0        0        0     1835 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/input/posix_pipe.py
--rw-rw-rw-   0        0        0     3897 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/input/posix_utils.py
--rw-rw-rw-   0        0        0     2538 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/input/typeahead.py
--rw-rw-rw-   0        0        0    10131 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/input/vt100.py
--rw-rw-rw-   0        0        0     8402 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/input/vt100_parser.py
--rw-rw-rw-   0        0        0    22282 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/input/win32.py
--rw-rw-rw-   0        0        0     4111 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/input/win32_pipe.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:44.092805 prot-3.8.4/src/prot/prompt/key_binding/
--rw-rw-rw-   0        0        0      335 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/key_binding/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:44.396805 prot-3.8.4/src/prot/prompt/key_binding/bindings/
--rw-rw-rw-   0        0        0        0 2020-01-12 12:31:42.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/__init__.py
--rw-rw-rw-   0        0        0     1736 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/auto_suggest.py
--rw-rw-rw-   0        0        0     7105 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/basic.py
--rw-rw-rw-   0        0        0     6841 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/completion.py
--rw-rw-rw-   0        0        0      744 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/cpr.py
--rw-rw-rw-   0        0        0    19627 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/emacs.py
--rw-rw-rw-   0        0        0      468 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/focus.py
--rw-rw-rw-   0        0        0     4946 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/mouse.py
--rw-rw-rw-   0        0        0    18371 2020-03-31 14:53:33.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/named_commands.py
--rw-rw-rw-   0        0        0     1282 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/open_in_editor.py
--rw-rw-rw-   0        0        0     2303 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/page_navigation.py
--rw-rw-rw-   0        0        0     5573 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/scroll.py
--rw-rw-rw-   0        0        0     2583 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/search.py
--rw-rw-rw-   0        0        0    75161 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/bindings/vi.py
--rw-rw-rw-   0        0        0     1917 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/defaults.py
--rw-rw-rw-   0        0        0    32798 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/key_binding/digraphs.py
--rw-rw-rw-   0        0        0      895 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/key_binding/emacs_state.py
--rw-rw-rw-   0        0        0    19390 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/key_bindings.py
--rw-rw-rw-   0        0        0    17631 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/key_binding/key_processor.py
--rw-rw-rw-   0        0        0     3316 2020-07-09 14:42:56.000000 prot-3.8.4/src/prot/prompt/key_binding/vi_state.py
--rw-rw-rw-   0        0        0     4885 2020-03-06 02:12:34.000000 prot-3.8.4/src/prot/prompt/keys.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:44.605805 prot-3.8.4/src/prot/prompt/layout/
--rw-rw-rw-   0        0        0     3462 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/layout/__init__.py
--rw-rw-rw-   0        0        0    97489 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/layout/containers.py
--rw-rw-rw-   0        0        0    34955 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/layout/controls.py
--rw-rw-rw-   0        0        0     6941 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/layout/dimension.py
--rw-rw-rw-   0        0        0     1001 2020-03-31 03:56:16.000000 prot-3.8.4/src/prot/prompt/layout/dummy.py
--rw-rw-rw-   0        0        0    14088 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/layout/layout.py
--rw-rw-rw-   0        0        0    10373 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/layout/margins.py
--rw-rw-rw-   0        0        0    25365 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/layout/menus.py
--rw-rw-rw-   0        0        0     1043 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/layout/mouse_handlers.py
--rw-rw-rw-   0        0        0    34137 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/layout/processors.py
--rw-rw-rw-   0        0        0     9745 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/layout/screen.py
--rw-rw-rw-   0        0        0     2259 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/layout/utils.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:44.617805 prot-3.8.4/src/prot/prompt/lexers/
--rw-rw-rw-   0        0        0      372 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/lexers/__init__.py
--rw-rw-rw-   0        0        0     2322 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/lexers/base.py
--rw-rw-rw-   0        0        0    11940 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/lexers/pygments.py
--rw-rw-rw-   0        0        0      116 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/log.py
--rw-rw-rw-   0        0        0     1339 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/mouse_events.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:44.713805 prot-3.8.4/src/prot/prompt/output/
--rw-rw-rw-   0        0        0      244 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/output/__init__.py
--rw-rw-rw-   0        0        0     6324 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/output/base.py
--rw-rw-rw-   0        0        0     2199 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/output/color_depth.py
--rw-rw-rw-   0        0        0     1487 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/output/conemu.py
--rw-rw-rw-   0        0        0     1886 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/output/defaults.py
--rw-rw-rw-   0        0        0    21317 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/output/vt100.py
--rw-rw-rw-   0        0        0    21140 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/output/win32.py
--rw-rw-rw-   0        0        0     2794 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/output/windows10.py
--rw-rw-rw-   0        0        0     5155 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/patch_stdout.py
--rw-rw-rw-   0        0        0    25735 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/renderer.py
--rw-rw-rw-   0        0        0     6997 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/search.py
--rw-rw-rw-   0        0        0     1289 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/selection.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:44.822804 prot-3.8.4/src/prot/prompt/shortcuts/
--rw-rw-rw-   0        0        0      844 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/shortcuts/__init__.py
--rw-rw-rw-   0        0        0     8424 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/shortcuts/dialogs.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:44.917805 prot-3.8.4/src/prot/prompt/shortcuts/progress_bar/
--rw-rw-rw-   0        0        0      458 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/shortcuts/progress_bar/__init__.py
--rw-rw-rw-   0        0        0    14070 2020-03-31 14:54:55.000000 prot-3.8.4/src/prot/prompt/shortcuts/progress_bar/base.py
--rw-rw-rw-   0        0        0    11767 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/shortcuts/progress_bar/formatters.py
--rw-rw-rw-   0        0        0    57251 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/shortcuts/prompt.py
--rw-rw-rw-   0        0        0     5707 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/shortcuts/utils.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:44.994806 prot-3.8.4/src/prot/prompt/styles/
--rw-rw-rw-   0        0        0     1603 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/styles/__init__.py
--rw-rw-rw-   0        0        0     5062 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/styles/base.py
--rw-rw-rw-   0        0        0     8363 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/styles/defaults.py
--rw-rw-rw-   0        0        0     4355 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/styles/named_colors.py
--rw-rw-rw-   0        0        0     1952 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/styles/pygments.py
--rw-rw-rw-   0        0        0    13023 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/styles/style.py
--rw-rw-rw-   0        0        0    12437 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/styles/style_transformation.py
--rw-rw-rw-   0        0        0       85 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/token.py
--rw-rw-rw-   0        0        0     8119 2020-03-31 09:45:47.000000 prot-3.8.4/src/prot/prompt/utils.py
--rw-rw-rw-   0        0        0     5837 2020-03-31 03:56:15.000000 prot-3.8.4/src/prot/prompt/validation.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:45.071805 prot-3.8.4/src/prot/prompt/widgets/
--rw-rw-rw-   0        0        0     1181 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/widgets/__init__.py
--rw-rw-rw-   0        0        0    28404 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/widgets/base.py
--rw-rw-rw-   0        0        0     3349 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/widgets/dialogs.py
--rw-rw-rw-   0        0        0    12736 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/widgets/menus.py
--rw-rw-rw-   0        0        0    12193 2020-03-31 03:56:17.000000 prot-3.8.4/src/prot/prompt/widgets/toolbars.py
--rw-rw-rw-   0        0        0     4138 2020-03-06 01:48:08.000000 prot-3.8.4/src/prot/prompt/win32_types.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:45.111805 prot-3.8.4/src/prot/wcwidth/
--rw-rw-rw-   0        0        0      140 2020-03-23 00:06:16.000000 prot-3.8.4/src/prot/wcwidth/__init__.py
--rw-rw-rw-   0        0        0     8004 2020-03-23 00:10:34.000000 prot-3.8.4/src/prot/wcwidth/table_wide.py
--rw-rw-rw-   0        0        0    24250 2020-03-23 00:10:34.000000 prot-3.8.4/src/prot/wcwidth/table_zero.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:45.143805 prot-3.8.4/src/prot/wcwidth/tests/
--rw-rw-rw-   0        0        0       42 2020-03-23 00:06:16.000000 prot-3.8.4/src/prot/wcwidth/tests/__init__.py
--rw-rw-rw-   0        0        0     3891 2020-03-31 09:47:57.000000 prot-3.8.4/src/prot/wcwidth/tests/test_core.py
--rw-rw-rw-   0        0        0     7831 2020-03-23 00:06:16.000000 prot-3.8.4/src/prot/wcwidth/wcwidth.py
-drwxrwxrwx   0        0        0        0 2020-07-25 09:19:40.585805 prot-3.8.4/src/prot.egg-info/
--rw-rw-rw-   0        0        0     2400 2020-07-25 09:19:02.000000 prot-3.8.4/src/prot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9720 2020-07-25 09:19:03.000000 prot-3.8.4/src/prot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-25 09:19:02.000000 prot-3.8.4/src/prot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2020-07-25 09:19:02.000000 prot-3.8.4/src/prot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-07-09 13:56:26.000000 prot-3.8.4/src/prot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        5 2020-07-25 09:19:02.000000 prot-3.8.4/src/prot.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.554239 prot-3.8.5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1069 2023-06-14 19:42:21.000000 prot-3.8.5/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1761 2023-06-14 19:45:20.554239 prot-3.8.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-06-14 19:42:21.000000 prot-3.8.5/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-14 19:45:20.554239 prot-3.8.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      801 2023-06-14 19:42:21.000000 prot-3.8.5/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.438239 prot-3.8.5/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.450239 prot-3.8.5/src/prot/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    38776 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2998 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/__main__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/__version__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.454239 prot-3.8.5/src/prot/bs/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      177 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5526 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/bs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2182 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/bsMap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      764 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/bsPro.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1236 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/bsSpaz.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.494239 prot-3.8.5/src/prot/bs/stdLib/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      190 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2189 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/alwaysLandLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4352 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bigGDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1568 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bridgitLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2261 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37874 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsAchievement.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8330 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsAssault.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34286 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsBomb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18154 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsCaptureTheFlag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11373 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsChosenOne.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9234 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsConquest.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    96453 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsCoopGame.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5888 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsDeathMatch.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9248 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsEasterEggHunt.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19687 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsElimination.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10709 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsFlag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27224 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsFootball.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   116735 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsGame.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12498 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsHockey.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      172 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsInternal.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7611 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsKeepAway.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsKingOfTheHill.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   155086 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageArabic.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   158524 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageBelarussian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   127437 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageChinese.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   118386 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageCroatian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   135541 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageCzech.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    94441 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageDanish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   141350 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageDutch.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   111226 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageEnglish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   105204 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageEsperanto.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   146287 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageFrench.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   148309 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageGerman.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   141903 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageGibberish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   187394 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageGreek.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   212586 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageHindi.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   137372 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageHungarian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   126188 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageIndonesian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   144849 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageItalian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   138448 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageKorean.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   162405 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguagePersian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   144892 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguagePolish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   145117 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguagePortuguese.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   121744 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageRomanian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   183660 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageRussian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   168786 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageSerbian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   142925 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageSpanish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   125252 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageSwedish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   129359 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageTurkish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   169058 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageUkrainian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34599 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLobby.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37628 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsMainMenu.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58253 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsMap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9381 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsMeteorShower.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6444 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsNinjaFight.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    48080 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsOnslaught.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11026 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsPowerup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24920 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsRace.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43185 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsRunaround.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12031 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsScoreBoard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12856 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsScoreSet.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18997 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsServerData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   141126 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsSpaz.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12571 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsTargetPractice.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58723 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsTeamGame.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10326 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsTheLastStand.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    63826 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsTutorial.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1093681 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsUI.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53124 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsUI2.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   188532 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsUtils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3224 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsVector.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3767 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/courtyardLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2120 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/cragCastleDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1635 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/doomShroomLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1513 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/footballStadiumDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1360 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/hockeyStadiumDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4179 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/lakeFrigidDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1674 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/monkeyFaceLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1448 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/rampageLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1491 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/roundaboutLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2377 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/stepRightUpLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1719 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/thePadLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2028 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/tipTopLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3284 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/towerDLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2234 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/zigZagLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12398 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/code.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.498239 prot-3.8.5/src/prot/color/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      239 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/color/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2524 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/color/ansi.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10462 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/color/ansitowin32.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1915 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/color/initialise.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5404 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/color/win32.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6438 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/color/winterm.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.498239 prot-3.8.5/src/prot/pip/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9136 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/pip/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1827 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/pip/__main__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      755 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/pip/extra.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)  4056147 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/pip/packagesList.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.506239 prot-3.8.5/src/prot/progress/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4910 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/progress/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2854 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/progress/bar.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1372 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/progress/counter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1380 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/progress/spinner.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.510239 prot-3.8.5/src/prot/prompt/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      872 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.514239 prot-3.8.5/src/prot/prompt/application/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      519 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/application/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44248 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/application/application.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5051 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/application/current.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1349 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/application/dummy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3699 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/application/run_in_terminal.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5919 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/auto_suggest.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    70342 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/buffer.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3768 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/cache.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.514239 prot-3.8.5/src/prot/prompt/clipboard/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      403 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/clipboard/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2489 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/clipboard/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1077 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/clipboard/in_memory.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1147 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/clipboard/pyperclip.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.518239 prot-3.8.5/src/prot/prompt/completion/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      810 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/completion/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11493 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/completion/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3832 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/completion/filesystem.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6945 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/completion/fuzzy_completer.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3885 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/completion/nested.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2934 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/completion/word_completer.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.518239 prot-3.8.5/src/prot/prompt/contrib/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:42:40.000000 prot-3.8.5/src/prot/prompt/contrib/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.518239 prot-3.8.5/src/prot/prompt/contrib/completers/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       36 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/completers/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2012 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/completers/system.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.518239 prot-3.8.5/src/prot/prompt/contrib/regular_languages/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3220 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/regular_languages/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21889 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/regular_languages/compiler.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3239 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/regular_languages/completion.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3386 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/regular_languages/lexer.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7827 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/regular_languages/regex_parser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/regular_languages/validation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.518239 prot-3.8.5/src/prot/prompt/contrib/ssh/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      138 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/ssh/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4365 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/ssh/server.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.522239 prot-3.8.5/src/prot/prompt/contrib/telnet/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       68 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/telnet/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      130 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/telnet/log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4974 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/telnet/protocol.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9518 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/telnet/server.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      187 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/data_structures.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    40593 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/document.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/enums.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.522239 prot-3.8.5/src/prot/prompt/eventloop/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      636 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4125 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/async_context_manager.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1711 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/async_generator.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1117 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/dummy_contextvars.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5514 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/inputhook.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3251 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/utils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2008 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/win32.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.522239 prot-3.8.5/src/prot/prompt/filters/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1028 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/filters/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9276 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/filters/app.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5737 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/filters/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1830 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/filters/cli.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      848 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/filters/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.526239 prot-3.8.5/src/prot/prompt/formatted_text/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1378 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/formatted_text/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8089 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/formatted_text/ansi.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4881 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/formatted_text/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4328 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/formatted_text/html.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      756 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/formatted_text/pygments.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2747 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/formatted_text/utils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7131 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/history.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.530239 prot-3.8.5/src/prot/prompt/input/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      209 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13116 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/ansi_escape_sequences.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3275 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1522 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/defaults.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1835 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/posix_pipe.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3897 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/posix_utils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2538 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/typeahead.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10131 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/vt100.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8402 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/vt100_parser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22282 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/win32.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4111 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/win32_pipe.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.534239 prot-3.8.5/src/prot/prompt/key_binding/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      335 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.538239 prot-3.8.5/src/prot/prompt/key_binding/bindings/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:42:40.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1736 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/auto_suggest.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7105 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/basic.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6841 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/completion.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      744 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/cpr.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19627 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/emacs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      468 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/focus.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4946 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/mouse.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18371 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/named_commands.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1282 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/open_in_editor.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2303 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/page_navigation.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5573 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/scroll.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2583 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/search.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    75161 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/vi.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1917 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/defaults.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    32798 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/digraphs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      895 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/emacs_state.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19390 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/key_bindings.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17631 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/key_processor.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3316 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/vi_state.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4885 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/keys.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.542239 prot-3.8.5/src/prot/prompt/layout/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3462 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97489 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/containers.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34955 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/controls.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6941 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/dimension.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1001 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/dummy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14088 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/layout.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10373 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/margins.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25365 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/menus.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1043 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/mouse_handlers.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34137 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/processors.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9745 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/screen.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2259 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.542239 prot-3.8.5/src/prot/prompt/lexers/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      372 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/lexers/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2322 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/lexers/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11940 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/lexers/pygments.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      116 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1339 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/mouse_events.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.546239 prot-3.8.5/src/prot/prompt/output/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      244 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6324 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2199 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/color_depth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1487 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/conemu.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1886 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/defaults.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21317 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/vt100.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21140 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/win32.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2794 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/windows10.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5155 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/patch_stdout.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25735 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/renderer.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6997 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/search.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1289 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/selection.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.546239 prot-3.8.5/src/prot/prompt/shortcuts/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      844 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8424 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/dialogs.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.546239 prot-3.8.5/src/prot/prompt/shortcuts/progress_bar/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      458 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/progress_bar/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14070 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/progress_bar/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11767 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/progress_bar/formatters.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57251 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/prompt.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5707 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.550239 prot-3.8.5/src/prot/prompt/styles/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1603 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5062 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8363 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/defaults.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4355 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/named_colors.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1952 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/pygments.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13023 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/style.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12437 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/style_transformation.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       85 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/token.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8119 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/utils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5837 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/validation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.550239 prot-3.8.5/src/prot/prompt/widgets/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1181 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/widgets/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    28404 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/widgets/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3349 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/widgets/dialogs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12736 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/widgets/menus.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12193 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/widgets/toolbars.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4138 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/win32_types.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.554239 prot-3.8.5/src/prot/wcwidth/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      140 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/wcwidth/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8004 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/wcwidth/table_wide.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24250 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/wcwidth/table_zero.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.554239 prot-3.8.5/src/prot/wcwidth/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/wcwidth/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3891 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/wcwidth/tests/test_core.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7831 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/wcwidth/wcwidth.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.450239 prot-3.8.5/src/prot.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1761 2023-06-14 19:45:20.000000 prot-3.8.5/src/prot.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9449 2023-06-14 19:45:20.000000 prot-3.8.5/src/prot.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-14 19:45:20.000000 prot-3.8.5/src/prot.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       59 2023-06-14 19:45:20.000000 prot-3.8.5/src/prot.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        5 2023-06-14 19:45:20.000000 prot-3.8.5/src/prot.egg-info/top_level.txt
```

### Comparing `prot-3.8.4/README.md` & `prot-3.8.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 Prot - Pro Tools for Python 3
+
+[![Downloads](https://static.pepy.tech/badge/prot)](https://pepy.tech/project/prot)
+
+
 =============================
 
 Modules
 -------
 
  * **classes**
  * **functions**
```

### Comparing `prot-3.8.4/src/prot/__main__.py` & `prot-3.8.5/src/prot/__main__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-from . import *
-from . import __version__ as version
-import prot
-import sys
-
-exit = False
-if 'light' in status:
-	printErr('command line interface not available in light version')
-	exit = True
-
-if __name__ == '__main__' and not exit:
-	for a in sys.argv[1:]:
-		if a in ['version', 'v']:
-			printMsg(version)
-			break
-		if a in ['tools', 't']:
-			ea = sys.argv[2]
-			if ea in ['test', 't']:
-				try:
-					c = int(sys.argv[3])
-				except:
-					c = 1000
-				testSpeed(c)
-			elif ea in ['wait', 'w']:
-				try:
-					c = float(sys.argv[3])
-				except:
-					try:
-						c = str(sys.argv[3])
-					except:
-						c = 1.0
-				Timer(c, None, False, 'foreground')
-			else:
-				printErr('argument is invalid.')
-			break
-		elif a in ['set', 's']:
-			if len(sys.argv) == 2:
-				for s in settings._data:
-					printMsg(s + ' : ' + settings._data[s])
-			elif len(sys.argv) == 3:
-				res = getattr(settings, sys.argv[2])
-				if res:
-					printMsg(sys.argv[2] + ' : ' + res)
-			elif len(sys.argv) == 4:
-				setattr(settings, sys.argv[2], sys.argv[3])
-				try:
-					if getattr(settings, sys.argv[2]) == sys.argv[3]:
-						printMsg(sys.argv[2] + ' : ' + sys.argv[3])
-				except: pass
-			else:
-				printErr('argument is invalid.')
-			break
-		elif a in ['run', 'r']:
-			func = sys.argv[2]
-			try:
-				args = sys.argv[3:]
-			except:
-				args = []
-			cargs = []
-			for a in args:
-				try:
-					integer = int(a)
-				except:
-					integer = None
-				if a.startswith('!'):
-					try:
-						data = ProtString(a[1:]).extract()
-						if len(data.dict) > 0:
-							narg = data.dict
-						elif len(data.list) > 0:
-							narg = data.list
-						else:
-							narg = []
-						if narg:
-							if type(narg) == list and len(narg) == 1 and not narg[0]:
-								narg = []
-						else:
-							narg = []
-					except:
-						try:
-							integer = int(a[1:])
-						except:
-							integer = None
-						if integer:
-							narg = integer
-						else:
-							narg = str(a[1:])
-				elif integer:
-					narg = integer
-				elif a in ['True', 'False', 'None']:
-					narg = True if a == 'True' else False if a == 'False' else None
-				else:
-					narg = str(a)
-				cargs.append(narg)
-			res = getattr(prot, func)(*cargs)
-			if res:
-				printMsg(res)
-		elif a in ['update', 'u']:
-			printMsg('current version is '+version)
-			if 'unofficial' in status:
-				printErr("can't update an unofficial product")
-				break
-			printMsg('checking for updates...')
-			try:
-				from prot.pip.extra import packageReleases
-				ver = int(list2str(version.split('.')))
-				vers = packageReleases('prot')
-				updateAvail = False
-				for v in vers:
-					cver = int(list2str(v.split('.')))
-					if cver > ver:
-						updateAvail = True
-						insver = v
-						break
-				if updateAvail:
-					printMsg('new version found, Installing prot v'+insver)
-					try:
-						runAsMain('pip -q install --upgrade prot=='+insver)
-					except: pass
-				else:
-					printMsg('latest version already installed')
-			except:
-				printErr('update failed.')
-		else:
-			printErr('argument is invalid.')
+from . import *
+from . import __version__ as version
+import prot
+import sys
+
+exit = False
+if 'light' in status:
+	printErr('command line interface not available in light version')
+	exit = True
+
+if __name__ == '__main__' and not exit:
+	for a in sys.argv[1:]:
+		if a in ['version', 'v']:
+			printMsg(version)
+			break
+		if a in ['tools', 't']:
+			ea = sys.argv[2]
+			if ea in ['test', 't']:
+				try:
+					c = int(sys.argv[3])
+				except:
+					c = 1000
+				testSpeed(c)
+			elif ea in ['wait', 'w']:
+				try:
+					c = float(sys.argv[3])
+				except:
+					try:
+						c = str(sys.argv[3])
+					except:
+						c = 1.0
+				Timer(c, None, False, 'foreground')
+			else:
+				printErr('argument is invalid.')
+			break
+		elif a in ['set', 's']:
+			if len(sys.argv) == 2:
+				for s in settings._data:
+					printMsg(s + ' : ' + settings._data[s])
+			elif len(sys.argv) == 3:
+				res = getattr(settings, sys.argv[2])
+				if res:
+					printMsg(sys.argv[2] + ' : ' + res)
+			elif len(sys.argv) == 4:
+				setattr(settings, sys.argv[2], sys.argv[3])
+				try:
+					if getattr(settings, sys.argv[2]) == sys.argv[3]:
+						printMsg(sys.argv[2] + ' : ' + sys.argv[3])
+				except: pass
+			else:
+				printErr('argument is invalid.')
+			break
+		elif a in ['run', 'r']:
+			func = sys.argv[2]
+			try:
+				args = sys.argv[3:]
+			except:
+				args = []
+			cargs = []
+			for a in args:
+				try:
+					integer = int(a)
+				except:
+					integer = None
+				if a.startswith('!'):
+					try:
+						data = ProtString(a[1:]).extract()
+						if len(data.dict) > 0:
+							narg = data.dict
+						elif len(data.list) > 0:
+							narg = data.list
+						else:
+							narg = []
+						if narg:
+							if type(narg) == list and len(narg) == 1 and not narg[0]:
+								narg = []
+						else:
+							narg = []
+					except:
+						try:
+							integer = int(a[1:])
+						except:
+							integer = None
+						if integer:
+							narg = integer
+						else:
+							narg = str(a[1:])
+				elif integer:
+					narg = integer
+				elif a in ['True', 'False', 'None']:
+					narg = True if a == 'True' else False if a == 'False' else None
+				else:
+					narg = str(a)
+				cargs.append(narg)
+			res = getattr(prot, func)(*cargs)
+			if res:
+				printMsg(res)
+		elif a in ['update', 'u']:
+			printMsg('current version is '+version)
+			if 'unofficial' in status:
+				printErr("can't update an unofficial product")
+				break
+			printMsg('checking for updates...')
+			try:
+				from prot.pip.extra import packageReleases
+				ver = int(list2str(version.split('.')))
+				vers = packageReleases('prot')
+				updateAvail = False
+				for v in vers:
+					cver = int(list2str(v.split('.')))
+					if cver > ver:
+						updateAvail = True
+						insver = v
+						break
+				if updateAvail:
+					printMsg('new version found, Installing prot v'+insver)
+					try:
+						runAsMain('pip -q install --upgrade prot=='+insver)
+					except: pass
+				else:
+					printMsg('latest version already installed')
+			except:
+				printErr('update failed.')
+		else:
+			printErr('argument is invalid.')
 		break
```

### Comparing `prot-3.8.4/src/prot/bs/bs.py` & `prot-3.8.5/src/prot/bs/bs.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-from . import *
-
-import os
-import hashlib
-import shutil
-
-from base64 import b64encode
-from functools import partial
-
-treeCache = {}
-
-def getModel(file):
-    return file + '.bob'
-
-def getCollideModel(file):
-    return file + '.cob'
-
-def getTexture(file):
-    return file + '.texture'
-
-def getSound(file):
-    return file + '.ogg'
-
-class Material(LoopBack): pass
-
-class Factory(object):
-    def __setattr__(self, key, value):
-        if key in ['dict', 'getcontents'] or key.startswith('_'):
-            object.__setattr__(self, key, value)
-        if not hasattr(self, 'dict'):
-            self.dict = {}
-        self.dict[key] = value
-
-    def __getattribute__(self, key):
-        if key in ['dict', 'getcontents'] or key.startswith('_'):
-            return object.__getattribute__(self, key, value)
-        if not hasattr(self, 'dict'):
-            self.dict = {}
-        return self.dict[key]
-
-    def getcontents(self, path='.'):
-        files = []
-        data = {self.__class__.__name__: files}
-        for key, value in self.dict.items():
-            if type(value) == str:
-                values = [value]
-            elif type(value) in [list, tuple]:
-                values = list(value)
-            else:
-                continue
-            for fileName in values:
-                if fileName.endswith('.texture'):
-                    files += bs.getFiles(fileName.split('.')[0], path, ['ktx', 'dds'])
-                else:
-                    files.append(fileName)
-        return data
-
-def md5sum(filename):
-    with open(filename, mode='rb') as f:
-        d = hashlib.md5()
-        for buf in iter(partial(f.read, 128), b''):
-            d.update(buf)
-    return d.hexdigest()
-
-def genPayloadInfo():
-    files = []
-    for root, subdirs, files_in_dir in os.walk(".", topdown=True, followlinks=False):
-        for file in files_in_dir:
-            if file.startswith('.') or file == 'payload_info': continue
-            files.append(os.path.join(root, file))
-
-    payloadStr = "{}\n1\n".format(len(files))
-    for file in files:
-        payloadStr += "{} {}\n".format(file.strip("./"), md5sum(file))
-
-    with open('payload_info', 'w') as f:
-        f.write(payloadStr)
-        f.close()
-
-def getFiles(file, path='.', formats=['ogg', 'ktx', 'dds', 'bob', 'cob', 'py', 'pyc']):
-    tree = makeTree(path)
-    files = []
-    for format in formats:
-        if file + '.' + format in tree:
-            files.append(file + '.' + format)
-    return files
-
-def makeTree(source='.', ignoreCache=False):
-    if source in treeCache and not ignoreCache:
-        return treeCache[source]
-    tree = {}
-    for p in os.listdir(source):
-        if os.path.isdir(os.path.join(source, p)):
-            for name, path in makeTree(os.path.join(source, p)).items():
-                tree[name] = path
-        else:
-            tree[p] = os.path.join(source, p)
-    if not ignoreCache:
-        treeCache[source] = tree
-    return tree
-
-def encodeFile(source):
-    ff = open('coded-'+source,'wb')
-    ff.write('import base64;exec(base64.b64decode('+repr(b64encode(open(source).read()))+'))')
-    ff.flush()
-
-def processMedia(data, path='.', divide=False, silent=False):
-    tree = makeTree(path)
-    media = os.path.join(path, 'media')
-    if not os.path.isdir(media):
-        os.mkdir(media)
-    for name, files in data.items():
-        if divide:
-            media = os.path.join(media, name)
-            if not os.path.isdir(media):
-              os.mkdir(media)
-
-        audios = os.path.join(media, 'audios')
-        tex = os.path.join(media, 'textures')
-        texAndroid = os.path.join(tex, 'android')
-        texOther = os.path.join(tex, 'other')
-        models = os.path.join(media, 'models')
-        scripts = os.path.join(media, 'scripts')
-
-        if not os.path.isdir(audios):
-            os.mkdir(audios)
-        if not os.path.isdir(tex):
-            os.mkdir(tex)
-        if not os.path.isdir(texAndroid):
-            os.mkdir(texAndroid)
-        if not os.path.isdir(texOther):
-            os.mkdir(texOther)
-        if not os.path.isdir(models):
-            os.mkdir(models)
-        if not os.path.isdir(scripts):
-            os.mkdir(scripts)
-
-        audioFormats = ['ogg']
-        texFormats = ['dds', 'ktx']
-        modelFormats = ['bob', 'cob']
-        scriptFormats = ['py', 'pyc']
-
-        for file in files:
-            if file in tree:
-                if file.type in audioFormats:
-                    if not silent:
-                        print(file + ' -> ' + audios)
-                    shutil.copy(tree[file], audios)
-                elif file.type in texFormats:
-                    if file.type == 'ktx':
-                        if not silent:
-                            print(file + ' -> ' + texAndroid)
-                        shutil.copy(tree[file], texAndroid)
-                    else:
-                        if not silent:
-                            print(file + ' -> ' + texOther)
-                        shutil.copy(tree[file], texOther)
-                elif file.type in modelFormats:
-                    if not silent:
-                        print(file + ' -> ' + models)
-                    shutil.copy(tree[file], models)
-                elif file.type in scriptFormats:
-                    if not silent:
-                        print(file + ' -> ' + scripts)
-                    shutil.copy(tree[file], scripts)
-                else:
-                   printWarn('type of file ' + file + ' is not supported')
-            else:
+from . import *
+
+import os
+import hashlib
+import shutil
+
+from base64 import b64encode
+from functools import partial
+
+treeCache = {}
+
+def getModel(file):
+    return file + '.bob'
+
+def getCollideModel(file):
+    return file + '.cob'
+
+def getTexture(file):
+    return file + '.texture'
+
+def getSound(file):
+    return file + '.ogg'
+
+class Material(LoopBack): pass
+
+class Factory(object):
+    def __setattr__(self, key, value):
+        if key in ['dict', 'getcontents'] or key.startswith('_'):
+            object.__setattr__(self, key, value)
+        if not hasattr(self, 'dict'):
+            self.dict = {}
+        self.dict[key] = value
+
+    def __getattribute__(self, key):
+        if key in ['dict', 'getcontents'] or key.startswith('_'):
+            return object.__getattribute__(self, key, value)
+        if not hasattr(self, 'dict'):
+            self.dict = {}
+        return self.dict[key]
+
+    def getcontents(self, path='.'):
+        files = []
+        data = {self.__class__.__name__: files}
+        for key, value in self.dict.items():
+            if type(value) == str:
+                values = [value]
+            elif type(value) in [list, tuple]:
+                values = list(value)
+            else:
+                continue
+            for fileName in values:
+                if fileName.endswith('.texture'):
+                    files += bs.getFiles(fileName.split('.')[0], path, ['ktx', 'dds'])
+                else:
+                    files.append(fileName)
+        return data
+
+def md5sum(filename):
+    with open(filename, mode='rb') as f:
+        d = hashlib.md5()
+        for buf in iter(partial(f.read, 128), b''):
+            d.update(buf)
+    return d.hexdigest()
+
+def genPayloadInfo():
+    files = []
+    for root, subdirs, files_in_dir in os.walk(".", topdown=True, followlinks=False):
+        for file in files_in_dir:
+            if file.startswith('.') or file == 'payload_info': continue
+            files.append(os.path.join(root, file))
+
+    payloadStr = "{}\n1\n".format(len(files))
+    for file in files:
+        payloadStr += "{} {}\n".format(file.strip("./"), md5sum(file))
+
+    with open('payload_info', 'w') as f:
+        f.write(payloadStr)
+        f.close()
+
+def getFiles(file, path='.', formats=['ogg', 'ktx', 'dds', 'bob', 'cob', 'py', 'pyc']):
+    tree = makeTree(path)
+    files = []
+    for format in formats:
+        if file + '.' + format in tree:
+            files.append(file + '.' + format)
+    return files
+
+def makeTree(source='.', ignoreCache=False):
+    if source in treeCache and not ignoreCache:
+        return treeCache[source]
+    tree = {}
+    for p in os.listdir(source):
+        if os.path.isdir(os.path.join(source, p)):
+            for name, path in makeTree(os.path.join(source, p)).items():
+                tree[name] = path
+        else:
+            tree[p] = os.path.join(source, p)
+    if not ignoreCache:
+        treeCache[source] = tree
+    return tree
+
+def encodeFile(source):
+    ff = open('coded-'+source,'wb')
+    ff.write('import base64;exec(base64.b64decode('+repr(b64encode(open(source).read()))+'))')
+    ff.flush()
+
+def processMedia(data, path='.', divide=False, silent=False):
+    tree = makeTree(path)
+    media = os.path.join(path, 'media')
+    if not os.path.isdir(media):
+        os.mkdir(media)
+    for name, files in data.items():
+        if divide:
+            media = os.path.join(media, name)
+            if not os.path.isdir(media):
+              os.mkdir(media)
+
+        audios = os.path.join(media, 'audios')
+        tex = os.path.join(media, 'textures')
+        texAndroid = os.path.join(tex, 'android')
+        texOther = os.path.join(tex, 'other')
+        models = os.path.join(media, 'models')
+        scripts = os.path.join(media, 'scripts')
+
+        if not os.path.isdir(audios):
+            os.mkdir(audios)
+        if not os.path.isdir(tex):
+            os.mkdir(tex)
+        if not os.path.isdir(texAndroid):
+            os.mkdir(texAndroid)
+        if not os.path.isdir(texOther):
+            os.mkdir(texOther)
+        if not os.path.isdir(models):
+            os.mkdir(models)
+        if not os.path.isdir(scripts):
+            os.mkdir(scripts)
+
+        audioFormats = ['ogg']
+        texFormats = ['dds', 'ktx']
+        modelFormats = ['bob', 'cob']
+        scriptFormats = ['py', 'pyc']
+
+        for file in files:
+            if file in tree:
+                if file.type in audioFormats:
+                    if not silent:
+                        print(file + ' -> ' + audios)
+                    shutil.copy(tree[file], audios)
+                elif file.type in texFormats:
+                    if file.type == 'ktx':
+                        if not silent:
+                            print(file + ' -> ' + texAndroid)
+                        shutil.copy(tree[file], texAndroid)
+                    else:
+                        if not silent:
+                            print(file + ' -> ' + texOther)
+                        shutil.copy(tree[file], texOther)
+                elif file.type in modelFormats:
+                    if not silent:
+                        print(file + ' -> ' + models)
+                    shutil.copy(tree[file], models)
+                elif file.type in scriptFormats:
+                    if not silent:
+                        print(file + ' -> ' + scripts)
+                    shutil.copy(tree[file], scripts)
+                else:
+                   printWarn('type of file ' + file + ' is not supported')
+            else:
                 printWarn('file ' + file + ' not found')
```

### Comparing `prot-3.8.4/src/prot/bs/bsMap.py` & `prot-3.8.5/src/prot/bs/bsMap.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from . import *
-
-import builtins as _builtins
-
-maps = {}
-depends = []
-
-class Map(object):
-    name = "Map"
-
-    @classmethod
-    def getPreviewTextureName(cls):
-        """
-        Return the name of the preview texture for this map.
-        """
-        return None
-
-    @classmethod
-    def onPreload(cls):
-        """
-        Called when the map is being preloaded;
-        it should load any media it requires to
-        class attributes on itself.
-        """
-        return None
-
-def registerMap(map):
-    if not map.name in maps:
-        maps[map.name] = map
-    else:
-        raise Exception(repr(map.name) + 'already exists.')
-
-def _import(*args, **kwargs):
-    depends.append(args[0])
-    if _import.redirect:
-        return _builtins.__import(*args, **kwargs)
-
-def record(redirect=False):
-    if redirect:
-        _import.redirect = True
-    else:
-        _import.redirect = False
-    _builtins.__import = _builtins.__import__
-    _builtins.__import__ = _import
-
-def end():
-    _builtins.__import__ = _builtins.__import
-    del _builtins.__import
-    del _import.redirect
-
-def clear():
-    global maps
-    global depends
-    maps = {}
-    depends = []
-
-def getMedia(path='.', divide=False, silent=False):
-    tree = bs.makeTree(path)
-    data = {}
-    for name, obj in maps.items():
-        medias = []
-        preloads = []
-        if obj.getPreviewTextureName() is not None:
-            medias += bs.getFiles(obj.getPreviewTextureName(), path, ['ktx', 'dds'])
-        if obj.onPreload() is not None:
-            for key, value in obj.onPreload().items():
-                if type(value) == str:
-                    preloads.append(value)
-                elif type(value) in [list, tuple]:
-                    preloads += list(value)
-        for preload in preloads:
-            if preload.endswith('.texture'):
-                medias += bs.getFiles(preload.split('.')[0], path, ['ktx', 'dds'])
-            else:
-                medias.append(preload)
-        for depend in depends:
-            medias += bs.getFiles(depend, path, ['py', 'pyc'])
-        data[name] = [ProtString(media) for media in medias]
-
-    if data:
+from . import *
+
+import builtins as _builtins
+
+maps = {}
+depends = []
+
+class Map(object):
+    name = "Map"
+
+    @classmethod
+    def getPreviewTextureName(cls):
+        """
+        Return the name of the preview texture for this map.
+        """
+        return None
+
+    @classmethod
+    def onPreload(cls):
+        """
+        Called when the map is being preloaded;
+        it should load any media it requires to
+        class attributes on itself.
+        """
+        return None
+
+def registerMap(map):
+    if not map.name in maps:
+        maps[map.name] = map
+    else:
+        raise Exception(repr(map.name) + 'already exists.')
+
+def _import(*args, **kwargs):
+    depends.append(args[0])
+    if _import.redirect:
+        return _builtins.__import(*args, **kwargs)
+
+def record(redirect=False):
+    if redirect:
+        _import.redirect = True
+    else:
+        _import.redirect = False
+    _builtins.__import = _builtins.__import__
+    _builtins.__import__ = _import
+
+def end():
+    _builtins.__import__ = _builtins.__import
+    del _builtins.__import
+    del _import.redirect
+
+def clear():
+    global maps
+    global depends
+    maps = {}
+    depends = []
+
+def getMedia(path='.', divide=False, silent=False):
+    tree = bs.makeTree(path)
+    data = {}
+    for name, obj in maps.items():
+        medias = []
+        preloads = []
+        if obj.getPreviewTextureName() is not None:
+            medias += bs.getFiles(obj.getPreviewTextureName(), path, ['ktx', 'dds'])
+        if obj.onPreload() is not None:
+            for key, value in obj.onPreload().items():
+                if type(value) == str:
+                    preloads.append(value)
+                elif type(value) in [list, tuple]:
+                    preloads += list(value)
+        for preload in preloads:
+            if preload.endswith('.texture'):
+                medias += bs.getFiles(preload.split('.')[0], path, ['ktx', 'dds'])
+            else:
+                medias.append(preload)
+        for depend in depends:
+            medias += bs.getFiles(depend, path, ['py', 'pyc'])
+        data[name] = [ProtString(media) for media in medias]
+
+    if data:
         bs.processMedia(data, path, divide, silent)
```

### Comparing `prot-3.8.4/src/prot/bs/bsSpaz.py` & `prot-3.8.5/src/prot/bs/bsSpaz.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from . import *
-
-import os
-import shutil
-
-appearances = {}
-
-class Appearance(Database):
-    def __init__(self, name):
-        Database.__init__(self)
-        if not name in appearances:
-            appearances[name] = self
-        else:
-            raise Exception(repr(name) + 'already exists.')
-
-def clear():
-    global appearances
-    appearances = {}
-
-def getOutput(file):
-    string = ''
-    for a in appearances:
-        string += 'addCharacter(' + repr(a) + ', cfg=' +str(appearances[a].dict) + ')\n'
-    
-    with open(file, 'w') as f:
-        f.write(string)
-        f.flush()
-
-def getMedia(path='.', divide=False, silent=False):
-    tree = bs.makeTree(path)
-    data = {}
-    for name, obj in appearances.items():
-        medias = []
-        for key, value in obj.dict.items():
-            if type(value) == str:
-                values = [value]
-            elif type(value) in [list, tuple]:
-                values = list(value)
-            else:
-                continue
-            for fileName in values:
-                medias += bs.getFiles(fileName, path, ['ogg', 'ktx', 'dds', 'bob', 'cob'])
-        data[name] = [ProtString(media) for media in medias]
-
-    if data:
+from . import *
+
+import os
+import shutil
+
+appearances = {}
+
+class Appearance(Database):
+    def __init__(self, name):
+        Database.__init__(self)
+        if not name in appearances:
+            appearances[name] = self
+        else:
+            raise Exception(repr(name) + 'already exists.')
+
+def clear():
+    global appearances
+    appearances = {}
+
+def getOutput(file):
+    string = ''
+    for a in appearances:
+        string += 'addCharacter(' + repr(a) + ', cfg=' +str(appearances[a].dict) + ')\n'
+    
+    with open(file, 'w') as f:
+        f.write(string)
+        f.flush()
+
+def getMedia(path='.', divide=False, silent=False):
+    tree = bs.makeTree(path)
+    data = {}
+    for name, obj in appearances.items():
+        medias = []
+        for key, value in obj.dict.items():
+            if type(value) == str:
+                values = [value]
+            elif type(value) in [list, tuple]:
+                values = list(value)
+            else:
+                continue
+            for fileName in values:
+                medias += bs.getFiles(fileName, path, ['ogg', 'ktx', 'dds', 'bob', 'cob'])
+        data[name] = [ProtString(media) for media in medias]
+
+    if data:
         bs.processMedia(data, path, divide, silent)
```

### Comparing `prot-3.8.4/src/prot/bs/stdLib/alwaysLandLevelDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/alwaysLandLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bigGDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/bigGDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bridgitLevelDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/bridgitLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bs.py` & `prot-3.8.5/src/prot/bs/stdLib/bs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsAchievement.py` & `prot-3.8.5/src/prot/bs/stdLib/bsAchievement.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsAssault.py` & `prot-3.8.5/src/prot/bs/stdLib/bsAssault.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsBomb.py` & `prot-3.8.5/src/prot/bs/stdLib/bsBomb.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsCaptureTheFlag.py` & `prot-3.8.5/src/prot/bs/stdLib/bsCaptureTheFlag.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsChosenOne.py` & `prot-3.8.5/src/prot/bs/stdLib/bsChosenOne.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsConquest.py` & `prot-3.8.5/src/prot/bs/stdLib/bsConquest.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsCoopGame.py` & `prot-3.8.5/src/prot/bs/stdLib/bsCoopGame.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsDeathMatch.py` & `prot-3.8.5/src/prot/bs/stdLib/bsDeathMatch.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsEasterEggHunt.py` & `prot-3.8.5/src/prot/bs/stdLib/bsEasterEggHunt.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsElimination.py` & `prot-3.8.5/src/prot/bs/stdLib/bsElimination.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsFlag.py` & `prot-3.8.5/src/prot/bs/stdLib/bsFlag.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsFootball.py` & `prot-3.8.5/src/prot/bs/stdLib/bsFootball.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsGame.py` & `prot-3.8.5/src/prot/bs/stdLib/bsGame.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsHockey.py` & `prot-3.8.5/src/prot/bs/stdLib/bsHockey.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsKeepAway.py` & `prot-3.8.5/src/prot/bs/stdLib/bsKeepAway.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsKingOfTheHill.py` & `prot-3.8.5/src/prot/bs/stdLib/bsKingOfTheHill.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageArabic.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageArabic.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageBelarussian.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageBelarussian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageChinese.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageChinese.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageCroatian.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageCroatian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageCzech.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageCzech.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageDanish.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageDanish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageDutch.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageDutch.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageEnglish.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageEnglish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageEsperanto.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageEsperanto.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageFrench.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageFrench.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageGerman.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageGerman.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageGibberish.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageGibberish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageGreek.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageGreek.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageHindi.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageHindi.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageHungarian.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageHungarian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageIndonesian.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageIndonesian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageItalian.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageItalian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageKorean.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageKorean.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguagePersian.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguagePersian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguagePolish.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguagePolish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguagePortuguese.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguagePortuguese.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageRomanian.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageRomanian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageRussian.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageRussian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageSerbian.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageSerbian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageSpanish.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageSpanish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageSwedish.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageSwedish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageTurkish.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageTurkish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLanguageUkrainian.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLanguageUkrainian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsLobby.py` & `prot-3.8.5/src/prot/bs/stdLib/bsLobby.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsMainMenu.py` & `prot-3.8.5/src/prot/bs/stdLib/bsMainMenu.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsMap.py` & `prot-3.8.5/src/prot/bs/stdLib/bsMap.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsMeteorShower.py` & `prot-3.8.5/src/prot/bs/stdLib/bsMeteorShower.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsNinjaFight.py` & `prot-3.8.5/src/prot/bs/stdLib/bsNinjaFight.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsOnslaught.py` & `prot-3.8.5/src/prot/bs/stdLib/bsOnslaught.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsPowerup.py` & `prot-3.8.5/src/prot/bs/stdLib/bsPowerup.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsRace.py` & `prot-3.8.5/src/prot/bs/stdLib/bsRace.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsRunaround.py` & `prot-3.8.5/src/prot/bs/stdLib/bsRunaround.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsScoreBoard.py` & `prot-3.8.5/src/prot/bs/stdLib/bsScoreBoard.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsScoreSet.py` & `prot-3.8.5/src/prot/bs/stdLib/bsScoreSet.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsServerData.py` & `prot-3.8.5/src/prot/bs/stdLib/bsServerData.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsSpaz.py` & `prot-3.8.5/src/prot/bs/stdLib/bsSpaz.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsTargetPractice.py` & `prot-3.8.5/src/prot/bs/stdLib/bsTargetPractice.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsTeamGame.py` & `prot-3.8.5/src/prot/bs/stdLib/bsTeamGame.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsTheLastStand.py` & `prot-3.8.5/src/prot/bs/stdLib/bsTheLastStand.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsTutorial.py` & `prot-3.8.5/src/prot/bs/stdLib/bsTutorial.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsUI.py` & `prot-3.8.5/src/prot/bs/stdLib/bsUI.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsUI2.py` & `prot-3.8.5/src/prot/bs/stdLib/bsUI2.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsUtils.py` & `prot-3.8.5/src/prot/bs/stdLib/bsUtils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/bsVector.py` & `prot-3.8.5/src/prot/bs/stdLib/bsVector.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/courtyardLevelDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/courtyardLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/cragCastleDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/cragCastleDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/doomShroomLevelDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/doomShroomLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/footballStadiumDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/footballStadiumDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/hockeyStadiumDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/hockeyStadiumDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/lakeFrigidDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/lakeFrigidDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/monkeyFaceLevelDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/monkeyFaceLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/rampageLevelDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/rampageLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/roundaboutLevelDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/roundaboutLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/stepRightUpLevelDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/stepRightUpLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/thePadLevelDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/thePadLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/tipTopLevelDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/tipTopLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/towerDLevelDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/towerDLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/bs/stdLib/zigZagLevelDefs.py` & `prot-3.8.5/src/prot/bs/stdLib/zigZagLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/code.py` & `prot-3.8.5/src/prot/code.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-from . import printMsg, printErr, printWarn, Database, list2str
-import random, base64 as __cmethst__, os, sys
-
-__spec__.data = Database()
-__spec__.data.codeType = [
-						{
-							'codes':['D=u*JdO7&//+g7fsH33Xk*M*$7*u_.', '=ev1=5u?$?-W5gf0n%w#5_7$%h__kq', 'Uc20dMPeVFq/~_+#&&fXugV_i&iA3Y', 'S50&+z5Z46#=1-Vh6Qt9jA@J1#4=!2', '_4Jb&v22749_+Ei9&Oq1_!qcu*92r0', '%$/fe9/y8q-j0A02pd9kk*IDGu20%_', 'Lqd4_8_%PrIP9oZC&uc3?K-A~Bp34U', '6~8_nf=/xcQ01GiKKd@68MVWO$.9o7', 'h#sFad1l-Br497W654q7Ye95e.4I4k', '74&UJR@cq!_9YekY/h-n~a$/!E+Q5Z', '$2#B?@5AP2IEUjxpDC@*ZYl=8+e/Ab', '701a_!*E#I.778my0!z877kBxCp-z=', 'K*uVq-=Z*8iY59/2c+aX3_MV.@*#Z_', '?2~5kA!eXu_cT--N$?T-*.+9NY947Z', '.!Wjz5NVOX3j7P1.bpC79.v24ls*K9', '1pr&Ll0giv/lBA$B_18!i$1@232-%/', 'a-@99ii9&Z84zN.kh/!8-5f&rqvj98', 'jvS#5d6?Rt=u!NJ1!2UDX4?*=5R%8v', 'ENr.T+8i37*ZKMS*UM4=jq=56*12H1', 'j6D-SWshO/p4Yc87wr.Hq40j81_KG7', '?23g7IBa9U4/9Xc4!o%438l&/46ZuG', 'Z1uLv&@058Oi_$50b?ox#3N4$_t4k0', '0w?Q!Gs27JY#RbW6li4zS+9&T5j_##', '37UHI5Q4AFV=v0A4P!zn!e_JTc9S93', '72zH338x?7s3cAe/l@.W6J%WO#Z@/$', '35fy*zV5w@ACWO3=S5u#Gj5l6beN@2', 'RGt86&1926@69_u95=4wyXI?=kHLJ6', 'U1qE!OC21*r+W0nm7k.X48+6k+&$l#', 'MU07fwRm1HdK00UZ2Jiu$_=I5t-2$X', '!1k6*a_7SD/20~*/xCn#.*C8uu.X~D', 'v66A4U.a$?E8W_xXR$*=@90r6_9&Dp', 'u+G!#4WbG$h=4.p5._9OWZ6143h.8R', 'Wz77@!#yZ@5W27g23?6r@2~7l515X~', '3~_p9CTPrJ.H9*TG370u#3rY6~ar=@', '/=t+%p7hy&nkuhnsHiK#=oG~DuAX~4', 'w!!x?_U6X96QpKx937jb8DFNv1.lU0', '~~!Y#78T95@3fV#DrB9$@9i6I?p39%', '$f@CD$Y6Ov1+1#w9.*?8I2x?bafsu.', 'dzkRN=7w59dk9_#e&?4L#Nj@?+Tpl!', '0d6X5_81GF-+/~2?wb=0?RPXqP952q', '8s2z%5r5da4vm0J8dn@Km7y0dL!*te', '+b#fG7*oVs4rN*1&.G+=G1%zO?#i/2', 'MxKR#-6ep@#Q+29kH5883XK=AJ#.H7', '&1$z4$+44E79tn?2$@_.6.bU&8?RVw', '@JF+pT55ydzR_5?Y_l@6S8_a/108$#', 'mD3e#5~13Z6s+V_cx7nm1Y/M4U=e.0', 'L9_VTQ.s7U=VRbC-#J5$7CE5-*9@vm', '072#3n./b11eh-Q_*Q$G_r6?!&P0PY', 'kMkdLA=+h%C40D8uoC7/7_!X&Mb%=4', 'b68cXM25q6GJ4s5N#g$062+0.WrT9_', '_5=9@avDV~UKbDod9~gw1g7A_jRb5_', 'JI%!ln.FNWNbqmDbo8=se+dJvo.W96', 'gNJamX*B!l/l#p9ag9Xi3Y%dy?j!NM', 'e=1=1bHh&n6.Sm3J8~1zU-g&o0?2rO', '?uO50+d.9.j7H8HFw0aBP21$$1qt~i', '#O!6uIse=7__DL-m-h9e88HdLj2jzm', 'OS~+5TtfjP5-kQecPM5Q+22Vhu!kY0', 'DVFEX14?U~b@t476VK72O&@ap.aB@V', 'n5dh!H-/-0W-%8?Q3X+_=26bNt=4@D', '46KKmbX-R6N~-9l=&5f1k0#E4PIm71', '!b$E9Typ#p+rM?#yQB50C442*gNMUs', 'TomYNZ-d3&i_%ySFi72WhY3L@-d~19', 'B31aV2!%ASH#q=19#tF6@1~j$BO69*', '@.TF_*xhfzC!BggwP7N47/*_#dZekt', 'K.@B#*/A*Q8I-IG1qcRqD_4O%D1s?v', 'lfs58h2Mn_O!@8=4ip/393?=L!0@4g', 'pjTb*?f4*Xn1.B3ZLV3Y30r21M@L%L', 'XeUh/86@F.-7Gf6&WT2cCP%7%x@~a.', '-/y.W6@*+H0M~kY@s$W0YXn&$2rjoh', '1y82N28LC!6_7$9k49K4X5/1$1Kw63', 'pXYEJ09tu0cd#9#Lf/3w4u7R0c?i3p', '9l6O$4rJD9/O82*6+wwiV#sBS9EV8I', 'QcL&tYKh4Q$cG1tx8.uM?0hth%E8O2', '6$+Q@HZElj2csmX_OzGi5A-BR8i++_', 'Ie/a8ph=Y_1%l=DC!du~e61A8qMUu7', '_nj%KGoz9&q-5V1=~&MnfYns1E171/', 'hg98U6oT$3Mq==97Hk9RVu#HtM$F+i', 'K=N409AL8~67fpL1IcT*6-9f4B125N', '&AX4U3A0~hh%4%P11%y10$batOcf!~', 'UaKC$b$%uzk?0#-/0Zs18q6+1s8ImF', '~7e$d#7!#QSw229hdM!3xFwI1_%/.q', 'xE6D12326RlIxi63j$&901w--GE9.1', 'ZZe*?23102IhIg4U&4$48f8OJ0+03w', '_kT&!9*VZ1sE-OtZ71L?x4$@P272EC', 'uJ35g6gHiQky+gs60_h8+f=~t1-tF7', '3Lu2O7Z%ZL2#/*z9_pFY=_7e-#qGOx', 'I0%2Phdd~I?6/Lw#MO98Jl7A*Cbv2W', 'D@s0qyF$aFl8/$53GWqA=1.&av#@!1', 'MG4%ZmhIod-e.0eqGO#VkfER8T2ttN', '2q#f@8arUE8Uu?V56c&76jWR9#!2?0', '4O5MQGM&h04=cH?P1!80dt+4&!a3d/', '1oBK%s9/h2j!0+d08uAT9-_v_pMu=0', 'fC9ioP-I9/l2?wJH42W4#1+y5r-pe7', '*x3PF8!@9_Jf5NUk@u4Zp-t@Fl0d_k', 'M!8gu53l92*O-R0F6W9$7~H%1/-025', '0Dhm.%2~0R$/Db428x3YBv7ZB4/KYF', 'E=E&VuP&J$snh5D8kn1vz0.4mYsNh8', '974KTXO3D6xJRkV/x$4.8+Q/xBnu%.', '@78/cNGHf4i3i?2A~Q0p3RXUwI5!h1', '46F6u.D1K1VNlywu9A5%_!xr?1y&CU'],
-							'decoder':__cmethst__.b64decode,
-							'encoder':__cmethst__.b64encode
-						},
-						{
-							'codes':['3#$1/0?#a783BL0M.y?FIva06-MqOo', '7Kcx#x?.F77C+F3B*SSCa$$+M*l9T7', 'oUGl8D__QhM.6Z&FA7-a8??34&Bmwe', '7#U0+p#y4T4ke4&2*9vVDgp3OGn&+~', '41IUP7HO0ENnT78v9%oU=m9a7NYM42', 'Mo5B$Q3jlNEtnQL1!fx2j.tvbI2c?X', '#3z940+Z7%aqRy_3176@66B1m4?duK', '2*Y177k1XHT=u%o!cT$#7e=Nv9V_g!', 'bK%4?K1?nQCzT45!!Fi0j7/%Q3YzaP', 'RI$Sv*4$@D@+V7X9~DRtcP5_8=8=+1', 'UIj8$Tgi&@sRk$34H55TP5*lN2gd2O', '/&B&n8s011!26u@NL?XDZ*t5LtVP39', 'WtPT~r5D*#10o2-p4N_JvxxgD%@8FC', 'Nk2u4aljuFVm%+_P~W=L8969VDi_gj', 'W931W7Us#&B@2-@05oTJ9d&f66!JF8', '?1Q#Ue-5!CUUmB+-jes1N8NzRHtS.i', '%9G$Pq7UrN1.#!6&!W056=Z-70_Nu7', 'P0?l#3zh5BOB8pF2JVS*pF+d79cL0k', '=1%.=@/A9D-=*EX0/Y#V#d8~Tyx?7G', 'P?/q@An*c.%U~81_36f+~k.=-6=6I6', '5vf1@_=!&92-3X?=DWW.Xxk@JU56-0', '6P8h0v?+IK?4FV23n.6o8T8my!M4_?', 'xD~p2?Mc/zSg+EZnQ$vG338b0P.3+l', '6B_BVso6Z0l$TQ.q_wdkHs?lAE=TJ8', 'RsmMkc96SF_VG~=FN~UHWV1?8B7bGq', '89N/5C9R6!+D!C9*-!393/WS1%rSUC', '/76AEesbv-y7M#sRb/6d?U+65F$bh@', '=6l5d5lRK4DIF6g.!qc3MP+U8_SB8c', 'Qy#$&S.50TJ3X5Ht0%5CS6v!=Zjf5J', 'avS&8BzVQ66HLA=_UbZDs1d=O+Fj.&', '&Y!D43x8=N54S*M=?NF2o9_/2J=RRM', 'A0Ru9mq36&.z5z!5/zMD?j7PVW~sf.', '0#Acz*yNpw8aOW&72sN!lPlaZ~%%u1', 'Zsq61qL44!IYZ!+*/2O4/5JZ4=4T#$', '_&o_V~/+M&@3%04d9gKnb-81.XJQ@D', '6953~~fF?Sj7KS107-m8vc7ykeSM~0', '_M5s3LxmWO6.c$3?*IDHKjMpL?4nv9', 'S+3=0n14Oc+Yg?h31$7X/WF~jr8/4j', 'P~?3.-0-8O=9%xCt+Uyg$TfyX%5537', 'B%z-r!nS-z4DPIb4@11#c*fI=0?5+9', 'lTAUgd%fy+gNZ5Il9nFj?=98+~6Z!D', 'Wr9G_J=s?Yqkjs*G854?y$z_Z_=*AY', '-e_@qQT&#uKQY7@LSD~q%G26-!m_qA', 'x_UcRS85r-N/KF*Cqarr+34~5+DpGV', '0+C4#@TUxFv0qK@h513Qxo1nko6t2e', '&=eU/1RCy_u+r+_is9Gx~S#PmS8I=_', '9@8P5kWt73$Mq7WI/tc91!/4b9?+61', 'P20@_G02Vy4uZ8~.249&25ZMq-n&0g', 'd~#.23yZ%CR1OsS5ER3V&jp/!M13Hv', 'N-5Ae1f/0$6H872FU_7/o7iDY!5nn*', '-m0?/?RUx55.@BH$1v0-S84Y@P2~2v', 'uX2deXaWU2#j@2K.@$AJJl2xz2KH!4', '6eeK@@p7b/!L!#?u~F7+O5A1j7V?#e', 'G078b!4lQ3j79AK0=8~puE!0hDCFX7', 'E7k98P9Vq3L3yf?v.@qWGk&KBh-y8K', 'l8y%f3Lts3Ze*m4=R_!0Tiw/~r9%Ag', 'Slj&1Fs0.las22t2R=~N6Xhk7Md0Mt', 'GlB1dk*j8oGYJMhb*R1?m#lpsDhGQ+', '--VhH+8y#XlA@H.53o1+.X$hRcZ8_t', 'hnMK0=VJ-&5e6?j34D3?/8?$5$xg8~', 'xhz!x0wN0p47B6v4W#3UC4%4#&6Y@=', 'a%*vBP_&5+650R#IzR0ylQ/14$6ykY', '7KZ8YP68%dPm8S6FL3?A-f0eZ-8bPo', 'RF%g519j1R?84%*94tc87JfL$~Obpn', 'wd52IW87=&066MiW$#811ikXtHiB#Z', 'a6Wv~3rGn-u#4$133=dN$p5g9_?f48', '%0!gazTjbg/02lAj_6g!3u9*a=r%6.', '792Ha3@qHBKvdg#F@dlxDaw7L8*+!l', '-/zCQG-81@e9v7Z7288**+%874nK8.', '/9P=x5*&23~sB-mVNk%4?.T1d6Y.$c', '1hi?2I5ylhYkhwcb@&3AMb.~1_EkCe', 'i92eYR69wV06B&j2a.q/KEKQtKk?2c', 'X6wCs4s#MDF_99D1No$~O$J22A4/q2', '7m50Z7+~gHD_bT&X=vT@m32/D.q!%e', '846?&zK=FIQd3.~5T6O?775.bQ=IC%', 'ht!3yKP9/Jmbdz!ikT-Ea$gTY3t_Q5', 'GUTd5Qe@6/NKv5=I3_I_u$DNmaN!A~', 'HGJi9%wAt~CZ@5=NPe~=F.5B6vnm7o', '8r0+99-4.h8A3wG75vtvTlBJ18uXdV', 'B&*M74*@JdIMI.~L9f$d40r+s82o5b', 'NMH35$Ai0d_$==3%2#HySRuSE_.Q%Q', '2o!7T~e?*H0m32?5?nS2C0k01o4pG?', '=6_DM5EL68E*du%DrH6/261d7G9W0j', 'X~00jdxTeNnxA79nBKm9RCb1L5+L2=', 'h-*jAKP_2_cgkm3pKpg2~NFh2bNmFn', 'w~PXi_?4=9K648@=r814h$gYj=._/C', '~f+fh0xfH/Zcf7iVj4L!4654S0s!r9', '%e27TK7uj$7J$V*&?Y~5D3W7BA.n_3', 'NqclBn%q4t707110/@k40957o&438g', '03P/NvSP0~QUSf_/Wm/&I76zTi2Oqv', 'D6C72l8_997~@Gt9aK9x$74qL~xqk_', '5.-J2I6w22O4&n.4y3DzF3g#w~.*-4', '_4/ct4v@b231yR.ZP6~590NXh4z-iD', 'sUBb90-Y4EEMq469K*Kj/w5Z8GU4P_', 'U7o=z$0!6Ous4EE+K+3?Yh08H6+dm&', '7&OI6sTl7P8k$%U$0r+6RPw7la8A9V', 'z272?7XO1F@#kW7nPS&5r?+3--xG17', 'A5u+mXY_R.f0iz?7MwP1-4d$R#I_+X', '4oGa84&H5ap8HA.U983~DQ_?8QDUgh', '=U9V4Bs6z+t@BS74yHPl@8d490467o'],
-							'decoder':__cmethst__.b32decode,
-							'encoder':__cmethst__.b32encode
-						},
-						{
-							'codes':['&ABCRe05$nxlulY%UrX3@$1C5=~5H_', 'k2RyF9FfXXm5NKRM03_r4b*2N5..m&', 'B!vX7NATP6V@8F3%S7~hRm%P&+vH%2', 'l_1=jP6W8lk43vQZ4Ye3$Jzm1_ut$B', 'cmOp/*a@U*#86wSzULM++e2Us4jsZU', '3*nXuaxG2BklNE&uVPPw94AK4$oA5~', 'pv9Qe37_T_/K_xs*?ay6fWgy1-MKVW', 'BZf~d80Z2gFqX2K6ViG5yt4274R4Ob', '.ELB/7o!U#JSt7c%9.0*s747Agz~/7', 'ichai&GndO62QB449WgkD*2O0CouR~', '4#0F@@=S?R#-.780Jq1N885XNeVOAw', 'ic@$fBtCb+Ft5M~o%lR3~wBaVYgB&@', 'Ad4Mc4CeW/SR1q-$&izaC+!Q@043W9', '!*Mv*eTL*2R+$W7XT7@@@L+00JolBf', 'XK*B4#Pfu79LJ0Nlup9=$Vx3@@n!t6', 'hV*kcP&%j3K!b3=~E6I?gOP3=!$PqQ', '4%W.o@GaUO+Oj1Z3Py1#6A3%F2z5~7', 'eqU#&b0_=1dc-8@/89X7RK=CItn*6~', '91fqX2=tK3t9H!7&PvUg4V31JhrUrg', 'KX4m49q5NhZj/*8a#x&8#w8W#5MZ$+', 'N@B7pU2?ph$GC3JLHq/p3q!0jI%L+i', '$COEn+6f?=1tR7At!8I9#.NW-rO71u', '07xo/!lf*UFr33i$1?_@FH=PWwcE/#', '4qe5.%Cq5R6/EE_-h0=3c90xT&ZT3!', 'gKP4!Q.=S9jcgho8A&1uA53xk24Go8', '8@D6*-l7orPocT9_mhj84O1_i5-85!', '7MoFFl0k/t~cA%H8Tg0+ELJLa1.T12', 'f~#3!k2D#Q1M~zP&6H7~*$3w/A48N4', '.s=9_rA/*V?=Z19P1F65uiJSpl.@84', '@h7=j3hd+-oLHy$%8Zw?Ha+=u118F/', '.8WWn4xZd*VvU%TE5a%3OYb=_$%2Vz', 'U?@2VW87NE8jXf73M=~-67p#A%X?_5', '=T-EZ3nv#?7M9V2Y~0EsucV@KR0&/v', '63k537I35=1Qp~L_J2K1so+z.aG9Og', '1$Ch#F*OrHDnHR74#90K@9=8_6Z23m', 'J1&R4j1uV4b2F72Y=&l#Eizr3E-%-U', 'RD/+!vvxOg1VR~UDbz&CJ%f+9l5LVN', 'm23snf5p?g3ilf9LlB.32A3JM!6g!Y', '+kR8a+jF!s@pO#290qM/DZ5_hO3K4G', '~6D%~F&2t=*c+acg+l17y+sQp6q#P_', '96!sui9z1FG/Y9b+Z5G0zMO5CHCam=', '6?7036Z-!@F2yH1Y/4rTl-#VDy?~nI', 'Uci!*1XeT?0*p-&8m!m3LS!@!fXmx!', 'Rzz%o9WZ!=4kMDS1-_Od=9-s+09fk8', '&~Q6_!8T/_#67b4G.FkZ.8qaR9IS%m', '4o$=9n614UnT3nP3Q~x!@9F9W8$2_d', '2w/~+O*cd~dtqgC.Ma865475zo/T%Q', 'l9Oy16254TTb~Gd9k?irU#+8QR=7K0', '!J.Y730=5GPplJGh8e7&z0*8jJWO65', '@&$Y&@q#Y73z06pQ&4A.+jnx56%Tvc', '~jy=Wnp#_3LiuKNV5C5eB33V!M@lC!', 'c5=O#+#H6d48.$A2se4!2A7wm6Tlzs', '=48zt4+54TO1246r5yL!gb4Mb046W%', '00cVm6-$7Ow2.#B*1@&+M45_uf73_x', 'wjYy$5%TO.w68E7_6T*x1C~2CstuqG', '.?j5nUmd!J18t2y&467D9~3ju9~m_w', 'nRx/_qM//ADs4uBS32$S45Q-%nSiLH', 'M~FK6P2%tG$2V3hM7c6&4@$jszw@&V', '+DWwppWyUr/@/C=7fz7pa%4+@-6RT9', '.~38V0!SKv1LoSW67+vCC33n7%LWHZ', '%T&?4A*.j6JTHI=.+_423voK3xr$D.', 'Qqei6cbTHa0@408Zqn8_U8xm$GfX%=', '$3GkC-Z2.V_4#zs+_I6PVO&fvEc.Dw', '9z-k6EnE1g%*&_vpY!91/wO1h$30JC', 'N%2BOL_+#8J8-CFfB-_!~%7QM73?H9', 'pdq9i+be&YRhes8t%3y=i5R9%#C755', '8+_H9~Z--%?M3$wp323qWP*UsT7d.g', 'R%10jFaGS5BQTF_?Mq0_+E%gx6aJK3', '=.UrzP736$t.S7q5vO+r1uxf@G9bm4', 'acsQ.H&/e=~6QuN/j1130x*#w738SD', 'vW3e_*0Zblz2-4w2V+6P9ewZ*@+2~J', 'yae210jf8Wd945YH2qD9iHTHgJ4-?7', '5c69*-H!7$W0vh/f91@g687Kl$1Im0', '5#5QRB.5IW9h*7zzxMj@@L8o6s7=82', 'Mgkxsi=$k1PfWBQYSFcOCo8*$8/BMe', '7XvN+2v4Vo7ux9I3Ob584u7J99T8Mu', '28/3%-u5d?*KpK6SK%5.f?Ug!7yKT0', '!4zv3X8ElbSF8IK?69//_F+L*ZYyVl', '3.oax6YRKf&zJbyf@w-pX@#n?qMxZ1', 'dK!8n0_-S72xqyr26R6HL$N59~o97D', 'Sm6SeY~mGT%j1306z=hQ@7MPcr?k2v', '~A.*6Ln7am57&A/6sXJO~ih3no6J7x', 'X5hi7?=U35%D7j-@8wU4X9w7*z9soI', 'O5W/V!QO.wh6$DA92mM!+h*Wrr7Z8T', '5#?!04#e5W25EH2GS-?#5fED89J75g', 'RRg%WpcpHz%QVd6c331$/?3?@4v=e.', '1q8C&P088X7b7033gA4c-Ud&BF&ZJ/', 'Dr3X=sP=/L8K3G~6v?ulRVMtZ27NB5', 'Dj#dF/bEG*--9UR.4Me3fu262!f6*K', '&TZ+qA?7JaU&rtp?e0?54-+NY21x2.', 'QKN657uSAk4j601?wF*5/MQ1dHUQgI', '6fy?jTV+dN.Z6to_c.+8_Ds32e83QV', '7QFb?hE%fE6mb01~4*2D_Pw$po_741', 'Vw9.2PE_t687L$=47W5wQMxTcE487#', 'ClL%$i16iCi1F0073ki*2G1%Z3y$&&', '6Ot&/W?7fqg?65!XM433$7l4mh84x+', '8@Gf6O+ip&n?qzR@EjeN8ZgB.0SsDj', '~a_uwUo=+O!5tk49m96tQ/X%unFz??', '0KKlGz$7wR%.VF3086n_&@454_l_7O', 'K0r.44XK5@N~NF*9K2+5b+Hnml_A*3'],
-							'decoder':__cmethst__.b16decode,
-							'encoder':__cmethst__.b16encode
-						}
-					]
-
-__spec__.data.compilerData = {
-								'name':'protStringCompiler',
-								'version':'1.1',
-								'codeListID':'9611699982',
-								}
-
-__spec__.data.compileOptions = [
-									{
-									'name':'type',
-									'options':['py', 'data'],
-									'default':'py'
-									}
-								]
-
-def encode(input, type='file'):
-	if type == 'file':
-		pyFile = open(input)
-		pyData = pyFile.read()
-		pyFile.close()
-	elif type in ['string', 'str']:
-		pyData = input
-	else:
-		printErr('type is invalid')
-		return
-	encType = random.choice(__spec__.data.codeType)
-	encCode = random.choice(encType['codes'])
-	encFunc = encType['encoder']
-	encData = encCode + '\n' + str(encFunc(bytes(pyData, 'utf-8')))[2:-1]
-	return encData
-
-def encrypt(input, output):
-	encData = encode(input)
-	encFile = open(output, 'w')
-	encFile.write(encData)
-	encFile.flush()
-	encFile.close()
-
-def execute(input, type='file'):
-	output = 'exec'
-	if type.startswith('out$'):
-		output = 'return'
-		type = type[4:]
-	if type == 'file':
-		pyFile = open(input)
-		pyData = pyFile.read()
-		pyFile.close()
-	elif type in ['string', 'str']:
-		pyData = input
-	else:
-		printErr('type is invalid')
-		return
-	pyLines = pyData.splitlines()
-	encCode = pyLines[0]
-	encData = pyLines[-1]
-	encFunc = None
-	for t in __spec__.data.codeType:
-		for c in t['codes']:
-			if c == encCode:
-				encFunc = t['decoder']
-	decData = list2str(str(encFunc(bytes(encData, 'utf-8')))[2:-1].splitlines(), '\n')
-	if output == 'exec':
-		decFile = open('decodedfile.py', 'w')
-		decFile.write(decData)
-		decFile.flush()
-		decFile.close()
-		decMod = __import__('decodedfile')
-		del decMod
-		del sys.modules['decodedfile']
-		os.remove('decodedfile')
-	else:
-		return decData
+from . import printMsg, printErr, printWarn, Database, list2str
+import random, base64 as __cmethst__, os, sys
+
+__spec__.data = Database()
+__spec__.data.codeType = [
+						{
+							'codes':['D=u*JdO7&//+g7fsH33Xk*M*$7*u_.', '=ev1=5u?$?-W5gf0n%w#5_7$%h__kq', 'Uc20dMPeVFq/~_+#&&fXugV_i&iA3Y', 'S50&+z5Z46#=1-Vh6Qt9jA@J1#4=!2', '_4Jb&v22749_+Ei9&Oq1_!qcu*92r0', '%$/fe9/y8q-j0A02pd9kk*IDGu20%_', 'Lqd4_8_%PrIP9oZC&uc3?K-A~Bp34U', '6~8_nf=/xcQ01GiKKd@68MVWO$.9o7', 'h#sFad1l-Br497W654q7Ye95e.4I4k', '74&UJR@cq!_9YekY/h-n~a$/!E+Q5Z', '$2#B?@5AP2IEUjxpDC@*ZYl=8+e/Ab', '701a_!*E#I.778my0!z877kBxCp-z=', 'K*uVq-=Z*8iY59/2c+aX3_MV.@*#Z_', '?2~5kA!eXu_cT--N$?T-*.+9NY947Z', '.!Wjz5NVOX3j7P1.bpC79.v24ls*K9', '1pr&Ll0giv/lBA$B_18!i$1@232-%/', 'a-@99ii9&Z84zN.kh/!8-5f&rqvj98', 'jvS#5d6?Rt=u!NJ1!2UDX4?*=5R%8v', 'ENr.T+8i37*ZKMS*UM4=jq=56*12H1', 'j6D-SWshO/p4Yc87wr.Hq40j81_KG7', '?23g7IBa9U4/9Xc4!o%438l&/46ZuG', 'Z1uLv&@058Oi_$50b?ox#3N4$_t4k0', '0w?Q!Gs27JY#RbW6li4zS+9&T5j_##', '37UHI5Q4AFV=v0A4P!zn!e_JTc9S93', '72zH338x?7s3cAe/l@.W6J%WO#Z@/$', '35fy*zV5w@ACWO3=S5u#Gj5l6beN@2', 'RGt86&1926@69_u95=4wyXI?=kHLJ6', 'U1qE!OC21*r+W0nm7k.X48+6k+&$l#', 'MU07fwRm1HdK00UZ2Jiu$_=I5t-2$X', '!1k6*a_7SD/20~*/xCn#.*C8uu.X~D', 'v66A4U.a$?E8W_xXR$*=@90r6_9&Dp', 'u+G!#4WbG$h=4.p5._9OWZ6143h.8R', 'Wz77@!#yZ@5W27g23?6r@2~7l515X~', '3~_p9CTPrJ.H9*TG370u#3rY6~ar=@', '/=t+%p7hy&nkuhnsHiK#=oG~DuAX~4', 'w!!x?_U6X96QpKx937jb8DFNv1.lU0', '~~!Y#78T95@3fV#DrB9$@9i6I?p39%', '$f@CD$Y6Ov1+1#w9.*?8I2x?bafsu.', 'dzkRN=7w59dk9_#e&?4L#Nj@?+Tpl!', '0d6X5_81GF-+/~2?wb=0?RPXqP952q', '8s2z%5r5da4vm0J8dn@Km7y0dL!*te', '+b#fG7*oVs4rN*1&.G+=G1%zO?#i/2', 'MxKR#-6ep@#Q+29kH5883XK=AJ#.H7', '&1$z4$+44E79tn?2$@_.6.bU&8?RVw', '@JF+pT55ydzR_5?Y_l@6S8_a/108$#', 'mD3e#5~13Z6s+V_cx7nm1Y/M4U=e.0', 'L9_VTQ.s7U=VRbC-#J5$7CE5-*9@vm', '072#3n./b11eh-Q_*Q$G_r6?!&P0PY', 'kMkdLA=+h%C40D8uoC7/7_!X&Mb%=4', 'b68cXM25q6GJ4s5N#g$062+0.WrT9_', '_5=9@avDV~UKbDod9~gw1g7A_jRb5_', 'JI%!ln.FNWNbqmDbo8=se+dJvo.W96', 'gNJamX*B!l/l#p9ag9Xi3Y%dy?j!NM', 'e=1=1bHh&n6.Sm3J8~1zU-g&o0?2rO', '?uO50+d.9.j7H8HFw0aBP21$$1qt~i', '#O!6uIse=7__DL-m-h9e88HdLj2jzm', 'OS~+5TtfjP5-kQecPM5Q+22Vhu!kY0', 'DVFEX14?U~b@t476VK72O&@ap.aB@V', 'n5dh!H-/-0W-%8?Q3X+_=26bNt=4@D', '46KKmbX-R6N~-9l=&5f1k0#E4PIm71', '!b$E9Typ#p+rM?#yQB50C442*gNMUs', 'TomYNZ-d3&i_%ySFi72WhY3L@-d~19', 'B31aV2!%ASH#q=19#tF6@1~j$BO69*', '@.TF_*xhfzC!BggwP7N47/*_#dZekt', 'K.@B#*/A*Q8I-IG1qcRqD_4O%D1s?v', 'lfs58h2Mn_O!@8=4ip/393?=L!0@4g', 'pjTb*?f4*Xn1.B3ZLV3Y30r21M@L%L', 'XeUh/86@F.-7Gf6&WT2cCP%7%x@~a.', '-/y.W6@*+H0M~kY@s$W0YXn&$2rjoh', '1y82N28LC!6_7$9k49K4X5/1$1Kw63', 'pXYEJ09tu0cd#9#Lf/3w4u7R0c?i3p', '9l6O$4rJD9/O82*6+wwiV#sBS9EV8I', 'QcL&tYKh4Q$cG1tx8.uM?0hth%E8O2', '6$+Q@HZElj2csmX_OzGi5A-BR8i++_', 'Ie/a8ph=Y_1%l=DC!du~e61A8qMUu7', '_nj%KGoz9&q-5V1=~&MnfYns1E171/', 'hg98U6oT$3Mq==97Hk9RVu#HtM$F+i', 'K=N409AL8~67fpL1IcT*6-9f4B125N', '&AX4U3A0~hh%4%P11%y10$batOcf!~', 'UaKC$b$%uzk?0#-/0Zs18q6+1s8ImF', '~7e$d#7!#QSw229hdM!3xFwI1_%/.q', 'xE6D12326RlIxi63j$&901w--GE9.1', 'ZZe*?23102IhIg4U&4$48f8OJ0+03w', '_kT&!9*VZ1sE-OtZ71L?x4$@P272EC', 'uJ35g6gHiQky+gs60_h8+f=~t1-tF7', '3Lu2O7Z%ZL2#/*z9_pFY=_7e-#qGOx', 'I0%2Phdd~I?6/Lw#MO98Jl7A*Cbv2W', 'D@s0qyF$aFl8/$53GWqA=1.&av#@!1', 'MG4%ZmhIod-e.0eqGO#VkfER8T2ttN', '2q#f@8arUE8Uu?V56c&76jWR9#!2?0', '4O5MQGM&h04=cH?P1!80dt+4&!a3d/', '1oBK%s9/h2j!0+d08uAT9-_v_pMu=0', 'fC9ioP-I9/l2?wJH42W4#1+y5r-pe7', '*x3PF8!@9_Jf5NUk@u4Zp-t@Fl0d_k', 'M!8gu53l92*O-R0F6W9$7~H%1/-025', '0Dhm.%2~0R$/Db428x3YBv7ZB4/KYF', 'E=E&VuP&J$snh5D8kn1vz0.4mYsNh8', '974KTXO3D6xJRkV/x$4.8+Q/xBnu%.', '@78/cNGHf4i3i?2A~Q0p3RXUwI5!h1', '46F6u.D1K1VNlywu9A5%_!xr?1y&CU'],
+							'decoder':__cmethst__.b64decode,
+							'encoder':__cmethst__.b64encode
+						},
+						{
+							'codes':['3#$1/0?#a783BL0M.y?FIva06-MqOo', '7Kcx#x?.F77C+F3B*SSCa$$+M*l9T7', 'oUGl8D__QhM.6Z&FA7-a8??34&Bmwe', '7#U0+p#y4T4ke4&2*9vVDgp3OGn&+~', '41IUP7HO0ENnT78v9%oU=m9a7NYM42', 'Mo5B$Q3jlNEtnQL1!fx2j.tvbI2c?X', '#3z940+Z7%aqRy_3176@66B1m4?duK', '2*Y177k1XHT=u%o!cT$#7e=Nv9V_g!', 'bK%4?K1?nQCzT45!!Fi0j7/%Q3YzaP', 'RI$Sv*4$@D@+V7X9~DRtcP5_8=8=+1', 'UIj8$Tgi&@sRk$34H55TP5*lN2gd2O', '/&B&n8s011!26u@NL?XDZ*t5LtVP39', 'WtPT~r5D*#10o2-p4N_JvxxgD%@8FC', 'Nk2u4aljuFVm%+_P~W=L8969VDi_gj', 'W931W7Us#&B@2-@05oTJ9d&f66!JF8', '?1Q#Ue-5!CUUmB+-jes1N8NzRHtS.i', '%9G$Pq7UrN1.#!6&!W056=Z-70_Nu7', 'P0?l#3zh5BOB8pF2JVS*pF+d79cL0k', '=1%.=@/A9D-=*EX0/Y#V#d8~Tyx?7G', 'P?/q@An*c.%U~81_36f+~k.=-6=6I6', '5vf1@_=!&92-3X?=DWW.Xxk@JU56-0', '6P8h0v?+IK?4FV23n.6o8T8my!M4_?', 'xD~p2?Mc/zSg+EZnQ$vG338b0P.3+l', '6B_BVso6Z0l$TQ.q_wdkHs?lAE=TJ8', 'RsmMkc96SF_VG~=FN~UHWV1?8B7bGq', '89N/5C9R6!+D!C9*-!393/WS1%rSUC', '/76AEesbv-y7M#sRb/6d?U+65F$bh@', '=6l5d5lRK4DIF6g.!qc3MP+U8_SB8c', 'Qy#$&S.50TJ3X5Ht0%5CS6v!=Zjf5J', 'avS&8BzVQ66HLA=_UbZDs1d=O+Fj.&', '&Y!D43x8=N54S*M=?NF2o9_/2J=RRM', 'A0Ru9mq36&.z5z!5/zMD?j7PVW~sf.', '0#Acz*yNpw8aOW&72sN!lPlaZ~%%u1', 'Zsq61qL44!IYZ!+*/2O4/5JZ4=4T#$', '_&o_V~/+M&@3%04d9gKnb-81.XJQ@D', '6953~~fF?Sj7KS107-m8vc7ykeSM~0', '_M5s3LxmWO6.c$3?*IDHKjMpL?4nv9', 'S+3=0n14Oc+Yg?h31$7X/WF~jr8/4j', 'P~?3.-0-8O=9%xCt+Uyg$TfyX%5537', 'B%z-r!nS-z4DPIb4@11#c*fI=0?5+9', 'lTAUgd%fy+gNZ5Il9nFj?=98+~6Z!D', 'Wr9G_J=s?Yqkjs*G854?y$z_Z_=*AY', '-e_@qQT&#uKQY7@LSD~q%G26-!m_qA', 'x_UcRS85r-N/KF*Cqarr+34~5+DpGV', '0+C4#@TUxFv0qK@h513Qxo1nko6t2e', '&=eU/1RCy_u+r+_is9Gx~S#PmS8I=_', '9@8P5kWt73$Mq7WI/tc91!/4b9?+61', 'P20@_G02Vy4uZ8~.249&25ZMq-n&0g', 'd~#.23yZ%CR1OsS5ER3V&jp/!M13Hv', 'N-5Ae1f/0$6H872FU_7/o7iDY!5nn*', '-m0?/?RUx55.@BH$1v0-S84Y@P2~2v', 'uX2deXaWU2#j@2K.@$AJJl2xz2KH!4', '6eeK@@p7b/!L!#?u~F7+O5A1j7V?#e', 'G078b!4lQ3j79AK0=8~puE!0hDCFX7', 'E7k98P9Vq3L3yf?v.@qWGk&KBh-y8K', 'l8y%f3Lts3Ze*m4=R_!0Tiw/~r9%Ag', 'Slj&1Fs0.las22t2R=~N6Xhk7Md0Mt', 'GlB1dk*j8oGYJMhb*R1?m#lpsDhGQ+', '--VhH+8y#XlA@H.53o1+.X$hRcZ8_t', 'hnMK0=VJ-&5e6?j34D3?/8?$5$xg8~', 'xhz!x0wN0p47B6v4W#3UC4%4#&6Y@=', 'a%*vBP_&5+650R#IzR0ylQ/14$6ykY', '7KZ8YP68%dPm8S6FL3?A-f0eZ-8bPo', 'RF%g519j1R?84%*94tc87JfL$~Obpn', 'wd52IW87=&066MiW$#811ikXtHiB#Z', 'a6Wv~3rGn-u#4$133=dN$p5g9_?f48', '%0!gazTjbg/02lAj_6g!3u9*a=r%6.', '792Ha3@qHBKvdg#F@dlxDaw7L8*+!l', '-/zCQG-81@e9v7Z7288**+%874nK8.', '/9P=x5*&23~sB-mVNk%4?.T1d6Y.$c', '1hi?2I5ylhYkhwcb@&3AMb.~1_EkCe', 'i92eYR69wV06B&j2a.q/KEKQtKk?2c', 'X6wCs4s#MDF_99D1No$~O$J22A4/q2', '7m50Z7+~gHD_bT&X=vT@m32/D.q!%e', '846?&zK=FIQd3.~5T6O?775.bQ=IC%', 'ht!3yKP9/Jmbdz!ikT-Ea$gTY3t_Q5', 'GUTd5Qe@6/NKv5=I3_I_u$DNmaN!A~', 'HGJi9%wAt~CZ@5=NPe~=F.5B6vnm7o', '8r0+99-4.h8A3wG75vtvTlBJ18uXdV', 'B&*M74*@JdIMI.~L9f$d40r+s82o5b', 'NMH35$Ai0d_$==3%2#HySRuSE_.Q%Q', '2o!7T~e?*H0m32?5?nS2C0k01o4pG?', '=6_DM5EL68E*du%DrH6/261d7G9W0j', 'X~00jdxTeNnxA79nBKm9RCb1L5+L2=', 'h-*jAKP_2_cgkm3pKpg2~NFh2bNmFn', 'w~PXi_?4=9K648@=r814h$gYj=._/C', '~f+fh0xfH/Zcf7iVj4L!4654S0s!r9', '%e27TK7uj$7J$V*&?Y~5D3W7BA.n_3', 'NqclBn%q4t707110/@k40957o&438g', '03P/NvSP0~QUSf_/Wm/&I76zTi2Oqv', 'D6C72l8_997~@Gt9aK9x$74qL~xqk_', '5.-J2I6w22O4&n.4y3DzF3g#w~.*-4', '_4/ct4v@b231yR.ZP6~590NXh4z-iD', 'sUBb90-Y4EEMq469K*Kj/w5Z8GU4P_', 'U7o=z$0!6Ous4EE+K+3?Yh08H6+dm&', '7&OI6sTl7P8k$%U$0r+6RPw7la8A9V', 'z272?7XO1F@#kW7nPS&5r?+3--xG17', 'A5u+mXY_R.f0iz?7MwP1-4d$R#I_+X', '4oGa84&H5ap8HA.U983~DQ_?8QDUgh', '=U9V4Bs6z+t@BS74yHPl@8d490467o'],
+							'decoder':__cmethst__.b32decode,
+							'encoder':__cmethst__.b32encode
+						},
+						{
+							'codes':['&ABCRe05$nxlulY%UrX3@$1C5=~5H_', 'k2RyF9FfXXm5NKRM03_r4b*2N5..m&', 'B!vX7NATP6V@8F3%S7~hRm%P&+vH%2', 'l_1=jP6W8lk43vQZ4Ye3$Jzm1_ut$B', 'cmOp/*a@U*#86wSzULM++e2Us4jsZU', '3*nXuaxG2BklNE&uVPPw94AK4$oA5~', 'pv9Qe37_T_/K_xs*?ay6fWgy1-MKVW', 'BZf~d80Z2gFqX2K6ViG5yt4274R4Ob', '.ELB/7o!U#JSt7c%9.0*s747Agz~/7', 'ichai&GndO62QB449WgkD*2O0CouR~', '4#0F@@=S?R#-.780Jq1N885XNeVOAw', 'ic@$fBtCb+Ft5M~o%lR3~wBaVYgB&@', 'Ad4Mc4CeW/SR1q-$&izaC+!Q@043W9', '!*Mv*eTL*2R+$W7XT7@@@L+00JolBf', 'XK*B4#Pfu79LJ0Nlup9=$Vx3@@n!t6', 'hV*kcP&%j3K!b3=~E6I?gOP3=!$PqQ', '4%W.o@GaUO+Oj1Z3Py1#6A3%F2z5~7', 'eqU#&b0_=1dc-8@/89X7RK=CItn*6~', '91fqX2=tK3t9H!7&PvUg4V31JhrUrg', 'KX4m49q5NhZj/*8a#x&8#w8W#5MZ$+', 'N@B7pU2?ph$GC3JLHq/p3q!0jI%L+i', '$COEn+6f?=1tR7At!8I9#.NW-rO71u', '07xo/!lf*UFr33i$1?_@FH=PWwcE/#', '4qe5.%Cq5R6/EE_-h0=3c90xT&ZT3!', 'gKP4!Q.=S9jcgho8A&1uA53xk24Go8', '8@D6*-l7orPocT9_mhj84O1_i5-85!', '7MoFFl0k/t~cA%H8Tg0+ELJLa1.T12', 'f~#3!k2D#Q1M~zP&6H7~*$3w/A48N4', '.s=9_rA/*V?=Z19P1F65uiJSpl.@84', '@h7=j3hd+-oLHy$%8Zw?Ha+=u118F/', '.8WWn4xZd*VvU%TE5a%3OYb=_$%2Vz', 'U?@2VW87NE8jXf73M=~-67p#A%X?_5', '=T-EZ3nv#?7M9V2Y~0EsucV@KR0&/v', '63k537I35=1Qp~L_J2K1so+z.aG9Og', '1$Ch#F*OrHDnHR74#90K@9=8_6Z23m', 'J1&R4j1uV4b2F72Y=&l#Eizr3E-%-U', 'RD/+!vvxOg1VR~UDbz&CJ%f+9l5LVN', 'm23snf5p?g3ilf9LlB.32A3JM!6g!Y', '+kR8a+jF!s@pO#290qM/DZ5_hO3K4G', '~6D%~F&2t=*c+acg+l17y+sQp6q#P_', '96!sui9z1FG/Y9b+Z5G0zMO5CHCam=', '6?7036Z-!@F2yH1Y/4rTl-#VDy?~nI', 'Uci!*1XeT?0*p-&8m!m3LS!@!fXmx!', 'Rzz%o9WZ!=4kMDS1-_Od=9-s+09fk8', '&~Q6_!8T/_#67b4G.FkZ.8qaR9IS%m', '4o$=9n614UnT3nP3Q~x!@9F9W8$2_d', '2w/~+O*cd~dtqgC.Ma865475zo/T%Q', 'l9Oy16254TTb~Gd9k?irU#+8QR=7K0', '!J.Y730=5GPplJGh8e7&z0*8jJWO65', '@&$Y&@q#Y73z06pQ&4A.+jnx56%Tvc', '~jy=Wnp#_3LiuKNV5C5eB33V!M@lC!', 'c5=O#+#H6d48.$A2se4!2A7wm6Tlzs', '=48zt4+54TO1246r5yL!gb4Mb046W%', '00cVm6-$7Ow2.#B*1@&+M45_uf73_x', 'wjYy$5%TO.w68E7_6T*x1C~2CstuqG', '.?j5nUmd!J18t2y&467D9~3ju9~m_w', 'nRx/_qM//ADs4uBS32$S45Q-%nSiLH', 'M~FK6P2%tG$2V3hM7c6&4@$jszw@&V', '+DWwppWyUr/@/C=7fz7pa%4+@-6RT9', '.~38V0!SKv1LoSW67+vCC33n7%LWHZ', '%T&?4A*.j6JTHI=.+_423voK3xr$D.', 'Qqei6cbTHa0@408Zqn8_U8xm$GfX%=', '$3GkC-Z2.V_4#zs+_I6PVO&fvEc.Dw', '9z-k6EnE1g%*&_vpY!91/wO1h$30JC', 'N%2BOL_+#8J8-CFfB-_!~%7QM73?H9', 'pdq9i+be&YRhes8t%3y=i5R9%#C755', '8+_H9~Z--%?M3$wp323qWP*UsT7d.g', 'R%10jFaGS5BQTF_?Mq0_+E%gx6aJK3', '=.UrzP736$t.S7q5vO+r1uxf@G9bm4', 'acsQ.H&/e=~6QuN/j1130x*#w738SD', 'vW3e_*0Zblz2-4w2V+6P9ewZ*@+2~J', 'yae210jf8Wd945YH2qD9iHTHgJ4-?7', '5c69*-H!7$W0vh/f91@g687Kl$1Im0', '5#5QRB.5IW9h*7zzxMj@@L8o6s7=82', 'Mgkxsi=$k1PfWBQYSFcOCo8*$8/BMe', '7XvN+2v4Vo7ux9I3Ob584u7J99T8Mu', '28/3%-u5d?*KpK6SK%5.f?Ug!7yKT0', '!4zv3X8ElbSF8IK?69//_F+L*ZYyVl', '3.oax6YRKf&zJbyf@w-pX@#n?qMxZ1', 'dK!8n0_-S72xqyr26R6HL$N59~o97D', 'Sm6SeY~mGT%j1306z=hQ@7MPcr?k2v', '~A.*6Ln7am57&A/6sXJO~ih3no6J7x', 'X5hi7?=U35%D7j-@8wU4X9w7*z9soI', 'O5W/V!QO.wh6$DA92mM!+h*Wrr7Z8T', '5#?!04#e5W25EH2GS-?#5fED89J75g', 'RRg%WpcpHz%QVd6c331$/?3?@4v=e.', '1q8C&P088X7b7033gA4c-Ud&BF&ZJ/', 'Dr3X=sP=/L8K3G~6v?ulRVMtZ27NB5', 'Dj#dF/bEG*--9UR.4Me3fu262!f6*K', '&TZ+qA?7JaU&rtp?e0?54-+NY21x2.', 'QKN657uSAk4j601?wF*5/MQ1dHUQgI', '6fy?jTV+dN.Z6to_c.+8_Ds32e83QV', '7QFb?hE%fE6mb01~4*2D_Pw$po_741', 'Vw9.2PE_t687L$=47W5wQMxTcE487#', 'ClL%$i16iCi1F0073ki*2G1%Z3y$&&', '6Ot&/W?7fqg?65!XM433$7l4mh84x+', '8@Gf6O+ip&n?qzR@EjeN8ZgB.0SsDj', '~a_uwUo=+O!5tk49m96tQ/X%unFz??', '0KKlGz$7wR%.VF3086n_&@454_l_7O', 'K0r.44XK5@N~NF*9K2+5b+Hnml_A*3'],
+							'decoder':__cmethst__.b16decode,
+							'encoder':__cmethst__.b16encode
+						}
+					]
+
+__spec__.data.compilerData = {
+								'name':'protStringCompiler',
+								'version':'1.1',
+								'codeListID':'9611699982',
+								}
+
+__spec__.data.compileOptions = [
+									{
+									'name':'type',
+									'options':['py', 'data'],
+									'default':'py'
+									}
+								]
+
+def encode(input, type='file'):
+	if type == 'file':
+		pyFile = open(input)
+		pyData = pyFile.read()
+		pyFile.close()
+	elif type in ['string', 'str']:
+		pyData = input
+	else:
+		printErr('type is invalid')
+		return
+	encType = random.choice(__spec__.data.codeType)
+	encCode = random.choice(encType['codes'])
+	encFunc = encType['encoder']
+	encData = encCode + '\n' + str(encFunc(bytes(pyData, 'utf-8')))[2:-1]
+	return encData
+
+def encrypt(input, output):
+	encData = encode(input)
+	encFile = open(output, 'w')
+	encFile.write(encData)
+	encFile.flush()
+	encFile.close()
+
+def execute(input, type='file'):
+	output = 'exec'
+	if type.startswith('out$'):
+		output = 'return'
+		type = type[4:]
+	if type == 'file':
+		pyFile = open(input)
+		pyData = pyFile.read()
+		pyFile.close()
+	elif type in ['string', 'str']:
+		pyData = input
+	else:
+		printErr('type is invalid')
+		return
+	pyLines = pyData.splitlines()
+	encCode = pyLines[0]
+	encData = pyLines[-1]
+	encFunc = None
+	for t in __spec__.data.codeType:
+		for c in t['codes']:
+			if c == encCode:
+				encFunc = t['decoder']
+	decData = list2str(str(encFunc(bytes(encData, 'utf-8')))[2:-1].splitlines(), '\n')
+	if output == 'exec':
+		decFile = open('decodedfile.py', 'w')
+		decFile.write(decData)
+		decFile.flush()
+		decFile.close()
+		decMod = __import__('decodedfile')
+		del decMod
+		del sys.modules['decodedfile']
+		os.remove('decodedfile')
+	else:
+		return decData
```

### Comparing `prot-3.8.4/src/prot/color/ansi.py` & `prot-3.8.5/src/prot/color/ansi.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/color/ansitowin32.py` & `prot-3.8.5/src/prot/color/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/color/initialise.py` & `prot-3.8.5/src/prot/color/initialise.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/color/win32.py` & `prot-3.8.5/src/prot/color/win32.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/color/winterm.py` & `prot-3.8.5/src/prot/color/winterm.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/pip/__init__.py` & `prot-3.8.5/src/prot/pip/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,306 +1,306 @@
-import sys
-try:
-	from .packagesList import packagesList as _p
-except:
-	_p = []
-import os
-import runpy as _r
-from .. import *
-try:
-	import xmlrpc.client as xmlrpclib
-except:
-	xmlrpclib = None
-
-__version__ = str(len(_p))
-DEFAULT_REPOSITORY = 'Pypi'
-
-def decode(file, type='txt'):
-	if type == 'txt':
-		return open(file).read().splitlines()
-	else:
-		return getVarFromFile(file, 'packagesList')
-
-def encode(data, type='txt'):
-	if type == 'txt':
-		string = ''
-		for d in data:
-			string += d+'\n'
-		return string
-	else:
-		return 'packagesList = '+str(data)
-		
-
-def convertUpdatePackage(iFile=None, oFile=None, ofFile='txt'):
-	printMsg('converting file to '+ofFile+' format...')
-	ifFile = 'txt' if not ofFile == 'txt' else 'py'
-	if type(iFile) == bool:
-		iFile = 'PackagesList.'+ifFile
-	if type(oFile) == bool:
-		oFile = 'PackagesList.'+ofFile
-	if not os.path.exists(iFile):
-		printErr('import argument not entered.')
-		return
-	data = decode(iFile, ifFile)
-	try:
-		open(oFile, 'w').write(encode(data, ofFile))
-	except PermissionError:
-		printErr('permission denied.')
-		return
-	printMsg('converted '+iFile+' to '+oFile+'.')
-	
-def updateBuiltinList(export=False, pList=False, fList='txt'):
-	if export and pList:
-		convertUpdatePackage(pList, export, fList)
-		return
-	if xmlrpclib is None and not pList:
-		printErr('xmlrpc is required.')
-		return
-	global _p
-	if not export:
-		printMsg('current version is '+str(len(_p)))
-	printMsg('checking for updates...' if not export else 'getting list...')
-	try:
-		if pList:
-			if type(pList) == bool:
-				pList = 'PackagesList.txt' if fList == 'txt' else 'packagesList.py'
-			if fList == 'txt':
-				pl = open(pList).read().splitlines()
-			else:
-				pl = getVarFromFile(pList, 'packagesList')
-		else:
-			client = xmlrpclib.ServerProxy('https://pypi.python.org/pypi')
-			pl = client.list_packages()
-	except:
-		printErr('update failed.' if not export else 'error occured while getting list.')
-		return
-	if len(pl) <= len(_p) and not export:
-		printMsg('built in list already updated.')
-		return
-	if settings.orderedBuiltinList == 'on':
-		pl.sort()
-	try:
-		if export:
-			if type(export) == bool:
-					export = 'PackagesList.txt' if fList == 'txt' else 'packagesList.py'
-			f = open(export, 'w')
-			f.write(encode(pl, fList))
-			f.flush()
-			f.close()
-		else:
-			_p = pl
-			f = open(os.path.join(os.path.split(__file__)[0], 'packagesList.py'), 'w')
-			f.write('packagesList = '+str(_p))
-			f.flush()
-			f.close()
-	except PermissionError:
-		printErr('permission denied.')
-		return
-	printMsg('built in list updated to version '+str(len(_p))+'.' if not export else 'list exported to '+export+'.' if fList == 'txt' else 'list exported to '+export+' with python format.')
-
-def getLocalRepo():
-	if settings.repo == 'default':
-		return DEFAULT_REPOSITORY
-	else:
-		return settings.repo
-
-def pip(args=None):
-	if type(args) == list:
-		args = ['prot.pip'] + args
-	elif type(args) == str:
-		args = ['prot.pip'] + args.split(' ')
-	else:
-		args = sys.argv
-	if not args[0] == 'prot.pip':
-		args[0] = 'prot.pip'
-	sys.argv = args
-	_r._run_module_as_main(sys.argv[0])
-
-def parseValue(value):
-	args = []
-	vals = []
-	for v in value:
-		if v.startswith('-'):
-			args.append(v)
-		elif v.startswith('+'):
-			args[len(args) - 1] += ' ' + v.replace('+', '')
-		else:
-			vals.append(v)
-	return vals, args
-
-def main(action, **values):
-	rules = [
-			{'key':'local',
-			'default':False},
-			{'key':'smart',
-			'default':False},
-			{'key':'value',
-			'default':None},
-			{'key':'export',
-			'default':None},
-			{'key':'list',
-			'default':False},
-			{'key':'listContents',
-			'default':[]},
-			{'key':'builtinList',
-			'default':False},
-			{'key':'searchList',
-			'default':False},
-			{'key':'searchKey',
-			'default':None},
-			{'key':'cfgFile',
-			'default':None},
-			{'key':'cfgStr',
-			'default':''},
-			{'key':'cfgList',
-			'default':[]}
-			]
-	options = OptionsDatabase(values, rules)
-	if not options.value:
-		options.value = ''
-	options.value, options.extraArgs = parseValue(options.value.split(' '))
-	options.value, options.extraArgs = list2str(options.value, ' '), list2str(options.extraArgs, ' ')
-	if options.local and type(options.local) == bool:
-		options.local = getLocalRepo()
-	if options.list and ((type(options.list) == bool) or ('search-' in options.list or 's-' in options.list)):
-		options.list = 'bltin' if (type(options.list) == bool) else options.list
-		options.builtinList = True
-		options.searchList = True if ('search-' in options.list or 's-' in options.list) else False
-		if options.searchList:
-			options.searchKey = options.list.split('-')[1]
-	if options.smart and type(options.smart) == bool:
-		options.smart = 'PackagesList.txt'
-	if options.export and type(options.export) == bool:
-		options.export = 'PackagesList.txt'
-	if options.list and type(options.list) == str:
-		options.list = options.list.replace('local.', options.local+'/' if options.local else '')
-	if options.smart and type(options.smart) == str:
-		options.smart = options.smart.replace('local.', options.local+'/' if options.local else '')
-	if options.export and type(options.export) == str:
-		options.export = options.export.replace('local.', options.local+'/' if options.local else '')
-
-	if options.smart:
-		if os.path.exists(options.smart):
-			f = open(options.smart)
-			options.cfgList = f.read().splitlines()
-			f.close()
-		else:
-			options.cfgFile = open(options.smart, 'w')
-		if options.cfgFile is None:
-			options.cfgFile = open(options.smart, 'w')
-		options.cfgStr = ''
-		for package in options.cfgList:
-			options.cfgStr += package+'\n'
-		if options.cfgStr.splitlines():
-			options.cfgFile.write(options.cfgStr)
-			options.cfgFile.flush()
-
-	if options.list:
-		if options.builtinList:
-			options.listContents += _p
-		if options.searchList:
-			newListContents = []
-			for c in options.listContents:
-				if options.searchKey in c:
-					newListContents.append(c)
-			options.listContents = newListContents
-		if not options.builtinList:
-			if os.path.exists(options.list):
-				options.listContents += open(options.list).read().splitlines()
-			else:
-				options.listContents.append(options.value)
-	else:
-		options.listContents.append(options.value)
-
-	if not action:
-		printErr('argument is invalid.')
-		return
-	if action in ['install', 'download', 'wheel']:
-		VAL1 = ValueWidget(0)
-		VAL2 = ValueWidget(0)
-		form = '$1 ignored, $2 $MSG $BAR' if settings.ui in ['small', 'verysmall'] else '$TIME ($VAL/$MAX) $1 ignored, $2 $MSG $BAR $PERC% completed'
-		progress = Progress(maxVal=len(options.listContents),
-							msg=action+'ed', msgForm=form,
-							replaces=[['$TIME', TimeWidget(hour=False)], ['$BAR', BarWidget(fillPerPercent=10 if settings.ui == 'verysmall' else 5)], ['$1', VAL1], ['$2', VAL2]],
-							inline=True)
-		for c in range(len(options.listContents)):
-			value = options.listContents[c]
-			if value is None:
-				progress.newline()
-				printErr('name not entered.')
-				VAL1.value += 1
-				progress.update(c+1)
-				continue
-			if options.value and not ' ' in options.value and not options.value.startswith('-'):
-				if not options.value in value:
-					VAL1.value += 1
-					progress.update(c+1)
-					continue
-			elif options.value and ' ' in options.value:
-				for v in options.value.split(' '):
-					if not v.startswith('-'):
-						if not options.value in value:
-							VAL1.value += 1
-							progress.update(c+1)
-							continue
-			if options.smart:
-				if value in options.cfgList:
-					VAL1.value += 1
-					progress.update(c+1)
-					continue
-			progress.newline()
-			try:
-				if options.local:
-					runAsMain(str('pip '+action+'$VAL'+'$EX'+' --no-index -f '+options.local).replace('$VAL', (' '+value if value else '')).replace('$EX', (' '+options.extraArgs) if options.extraArgs else ''))
-				else:
-					runAsMain(str('pip '+action+'$VAL'+'$EX').replace('$VAL', (' '+value if value else '')).replace('$EX', (' '+options.extraArgs) if options.extraArgs else ''))
-			except:
-				pass
-			if options.smart:
-				options.cfgList.append(value)
-				options.cfgFile.write(value+'\n')
-				options.cfgFile.flush()
-			VAL2.value += 1
-			progress.update(c+1)
-		progress.newline()
-		if options.smart:
-			options.cfgFile.close()
-
-	elif action == 'search':
-		searchResult = []
-		if options.value in options.listContents:
-			options.listContents.remove(options.value)
-		if options.listContents:
-			for p in options.listContents:
-				if options.value:
-					if options.value in p:
-						searchResult.append(p)
-				else:
-					searchResult.append(p)
-		elif options.local:
-			for f in os.listdir(options.local):
-				if f.endswith('.tar.gz') or f.endswith('.whl') or f.endswith('.zip'):
-					if options.value:
-						if options.value in f:
-							searchResult.append(f)
-					else:
-						searchResult.append(f)
-		else:
-			try: runAsMain('pip '+action+' '+options.value)
-			except: pass
-		if options.export:
-			f = open(options.export, 'w')
-			ss = ''
-			for p in searchResult:
-				ss += p+'\n'
-			f.write(ss)
-			f.flush()
-			f.close()
-			printMsg('search result exported to '+options.export)
-		else:
-			for p in searchResult:
-				printMsg(p, colorize=False)
-	elif action == 'version':
-		printMsg(len(_p))
-	else:
-		printErr('argument is invalid.')
+import sys
+try:
+	from .packagesList import packagesList as _p
+except:
+	_p = []
+import os
+import runpy as _r
+from .. import *
+try:
+	import xmlrpc.client as xmlrpclib
+except:
+	xmlrpclib = None
+
+__version__ = str(len(_p))
+DEFAULT_REPOSITORY = 'Pypi'
+
+def decode(file, type='txt'):
+	if type == 'txt':
+		return open(file).read().splitlines()
+	else:
+		return getVarFromFile(file, 'packagesList')
+
+def encode(data, type='txt'):
+	if type == 'txt':
+		string = ''
+		for d in data:
+			string += d+'\n'
+		return string
+	else:
+		return 'packagesList = '+str(data)
+		
+
+def convertUpdatePackage(iFile=None, oFile=None, ofFile='txt'):
+	printMsg('converting file to '+ofFile+' format...')
+	ifFile = 'txt' if not ofFile == 'txt' else 'py'
+	if type(iFile) == bool:
+		iFile = 'PackagesList.'+ifFile
+	if type(oFile) == bool:
+		oFile = 'PackagesList.'+ofFile
+	if not os.path.exists(iFile):
+		printErr('import argument not entered.')
+		return
+	data = decode(iFile, ifFile)
+	try:
+		open(oFile, 'w').write(encode(data, ofFile))
+	except PermissionError:
+		printErr('permission denied.')
+		return
+	printMsg('converted '+iFile+' to '+oFile+'.')
+	
+def updateBuiltinList(export=False, pList=False, fList='txt'):
+	if export and pList:
+		convertUpdatePackage(pList, export, fList)
+		return
+	if xmlrpclib is None and not pList:
+		printErr('xmlrpc is required.')
+		return
+	global _p
+	if not export:
+		printMsg('current version is '+str(len(_p)))
+	printMsg('checking for updates...' if not export else 'getting list...')
+	try:
+		if pList:
+			if type(pList) == bool:
+				pList = 'PackagesList.txt' if fList == 'txt' else 'packagesList.py'
+			if fList == 'txt':
+				pl = open(pList).read().splitlines()
+			else:
+				pl = getVarFromFile(pList, 'packagesList')
+		else:
+			client = xmlrpclib.ServerProxy('https://pypi.python.org/pypi')
+			pl = client.list_packages()
+	except:
+		printErr('update failed.' if not export else 'error occured while getting list.')
+		return
+	if len(pl) <= len(_p) and not export:
+		printMsg('built in list already updated.')
+		return
+	if settings.orderedBuiltinList == 'on':
+		pl.sort()
+	try:
+		if export:
+			if type(export) == bool:
+					export = 'PackagesList.txt' if fList == 'txt' else 'packagesList.py'
+			f = open(export, 'w')
+			f.write(encode(pl, fList))
+			f.flush()
+			f.close()
+		else:
+			_p = pl
+			f = open(os.path.join(os.path.split(__file__)[0], 'packagesList.py'), 'w')
+			f.write('packagesList = '+str(_p))
+			f.flush()
+			f.close()
+	except PermissionError:
+		printErr('permission denied.')
+		return
+	printMsg('built in list updated to version '+str(len(_p))+'.' if not export else 'list exported to '+export+'.' if fList == 'txt' else 'list exported to '+export+' with python format.')
+
+def getLocalRepo():
+	if settings.repo == 'default':
+		return DEFAULT_REPOSITORY
+	else:
+		return settings.repo
+
+def pip(args=None):
+	if type(args) == list:
+		args = ['prot.pip'] + args
+	elif type(args) == str:
+		args = ['prot.pip'] + args.split(' ')
+	else:
+		args = sys.argv
+	if not args[0] == 'prot.pip':
+		args[0] = 'prot.pip'
+	sys.argv = args
+	_r._run_module_as_main(sys.argv[0])
+
+def parseValue(value):
+	args = []
+	vals = []
+	for v in value:
+		if v.startswith('-'):
+			args.append(v)
+		elif v.startswith('+'):
+			args[len(args) - 1] += ' ' + v.replace('+', '')
+		else:
+			vals.append(v)
+	return vals, args
+
+def main(action, **values):
+	rules = [
+			{'key':'local',
+			'default':False},
+			{'key':'smart',
+			'default':False},
+			{'key':'value',
+			'default':None},
+			{'key':'export',
+			'default':None},
+			{'key':'list',
+			'default':False},
+			{'key':'listContents',
+			'default':[]},
+			{'key':'builtinList',
+			'default':False},
+			{'key':'searchList',
+			'default':False},
+			{'key':'searchKey',
+			'default':None},
+			{'key':'cfgFile',
+			'default':None},
+			{'key':'cfgStr',
+			'default':''},
+			{'key':'cfgList',
+			'default':[]}
+			]
+	options = OptionsDatabase(values, rules)
+	if not options.value:
+		options.value = ''
+	options.value, options.extraArgs = parseValue(options.value.split(' '))
+	options.value, options.extraArgs = list2str(options.value, ' '), list2str(options.extraArgs, ' ')
+	if options.local and type(options.local) == bool:
+		options.local = getLocalRepo()
+	if options.list and ((type(options.list) == bool) or ('search-' in options.list or 's-' in options.list)):
+		options.list = 'bltin' if (type(options.list) == bool) else options.list
+		options.builtinList = True
+		options.searchList = True if ('search-' in options.list or 's-' in options.list) else False
+		if options.searchList:
+			options.searchKey = options.list.split('-')[1]
+	if options.smart and type(options.smart) == bool:
+		options.smart = 'PackagesList.txt'
+	if options.export and type(options.export) == bool:
+		options.export = 'PackagesList.txt'
+	if options.list and type(options.list) == str:
+		options.list = options.list.replace('local.', options.local+'/' if options.local else '')
+	if options.smart and type(options.smart) == str:
+		options.smart = options.smart.replace('local.', options.local+'/' if options.local else '')
+	if options.export and type(options.export) == str:
+		options.export = options.export.replace('local.', options.local+'/' if options.local else '')
+
+	if options.smart:
+		if os.path.exists(options.smart):
+			f = open(options.smart)
+			options.cfgList = f.read().splitlines()
+			f.close()
+		else:
+			options.cfgFile = open(options.smart, 'w')
+		if options.cfgFile is None:
+			options.cfgFile = open(options.smart, 'w')
+		options.cfgStr = ''
+		for package in options.cfgList:
+			options.cfgStr += package+'\n'
+		if options.cfgStr.splitlines():
+			options.cfgFile.write(options.cfgStr)
+			options.cfgFile.flush()
+
+	if options.list:
+		if options.builtinList:
+			options.listContents += _p
+		if options.searchList:
+			newListContents = []
+			for c in options.listContents:
+				if options.searchKey in c:
+					newListContents.append(c)
+			options.listContents = newListContents
+		if not options.builtinList:
+			if os.path.exists(options.list):
+				options.listContents += open(options.list).read().splitlines()
+			else:
+				options.listContents.append(options.value)
+	else:
+		options.listContents.append(options.value)
+
+	if not action:
+		printErr('argument is invalid.')
+		return
+	if action in ['install', 'download', 'wheel']:
+		VAL1 = ValueWidget(0)
+		VAL2 = ValueWidget(0)
+		form = '$1 ignored, $2 $MSG $BAR' if settings.ui in ['small', 'verysmall'] else '$TIME ($VAL/$MAX) $1 ignored, $2 $MSG $BAR $PERC% completed'
+		progress = Progress(maxVal=len(options.listContents),
+							msg=action+'ed', msgForm=form,
+							replaces=[['$TIME', TimeWidget(hour=False)], ['$BAR', BarWidget(fillPerPercent=10 if settings.ui == 'verysmall' else 5)], ['$1', VAL1], ['$2', VAL2]],
+							inline=True)
+		for c in range(len(options.listContents)):
+			value = options.listContents[c]
+			if value is None:
+				progress.newline()
+				printErr('name not entered.')
+				VAL1.value += 1
+				progress.update(c+1)
+				continue
+			if options.value and not ' ' in options.value and not options.value.startswith('-'):
+				if not options.value in value:
+					VAL1.value += 1
+					progress.update(c+1)
+					continue
+			elif options.value and ' ' in options.value:
+				for v in options.value.split(' '):
+					if not v.startswith('-'):
+						if not options.value in value:
+							VAL1.value += 1
+							progress.update(c+1)
+							continue
+			if options.smart:
+				if value in options.cfgList:
+					VAL1.value += 1
+					progress.update(c+1)
+					continue
+			progress.newline()
+			try:
+				if options.local:
+					runAsMain(str('pip '+action+'$VAL'+'$EX'+' --no-index -f '+options.local).replace('$VAL', (' '+value if value else '')).replace('$EX', (' '+options.extraArgs) if options.extraArgs else ''))
+				else:
+					runAsMain(str('pip '+action+'$VAL'+'$EX').replace('$VAL', (' '+value if value else '')).replace('$EX', (' '+options.extraArgs) if options.extraArgs else ''))
+			except:
+				pass
+			if options.smart:
+				options.cfgList.append(value)
+				options.cfgFile.write(value+'\n')
+				options.cfgFile.flush()
+			VAL2.value += 1
+			progress.update(c+1)
+		progress.newline()
+		if options.smart:
+			options.cfgFile.close()
+
+	elif action == 'search':
+		searchResult = []
+		if options.value in options.listContents:
+			options.listContents.remove(options.value)
+		if options.listContents:
+			for p in options.listContents:
+				if options.value:
+					if options.value in p:
+						searchResult.append(p)
+				else:
+					searchResult.append(p)
+		elif options.local:
+			for f in os.listdir(options.local):
+				if f.endswith('.tar.gz') or f.endswith('.whl') or f.endswith('.zip'):
+					if options.value:
+						if options.value in f:
+							searchResult.append(f)
+					else:
+						searchResult.append(f)
+		else:
+			try: runAsMain('pip '+action+' '+options.value)
+			except: pass
+		if options.export:
+			f = open(options.export, 'w')
+			ss = ''
+			for p in searchResult:
+				ss += p+'\n'
+			f.write(ss)
+			f.flush()
+			f.close()
+			printMsg('search result exported to '+options.export)
+		else:
+			for p in searchResult:
+				printMsg(p, colorize=False)
+	elif action == 'version':
+		printMsg(len(_p))
+	else:
+		printErr('argument is invalid.')
 		return
```

### Comparing `prot-3.8.4/src/prot/pip/__main__.py` & `prot-3.8.5/src/prot/pip/__main__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import sys
-from . import *
-from .. import *
-
-exit = False
-if 'light' in status:
-	printErr('command line interface not available in light version')
-	exit = True
-
-if __name__ == '__main__' and not exit:
-	localRepo = False
-	action = None
-	value = None
-	pList = False
-	iList = False
-	eList = False
-	fList = 'txt'
-	smart = False
-	export = False
-	for a in sys.argv[1:]:
-		if action == 'update' and ('--export' in a or '-e' in a):
-			if ':' in a:
-				eList = a.split(':')[1]
-			else:
-				eList = True
-		elif action == 'update' and ('--import' in a or '-i' in a):
-			if ':' in a:
-				iList = a.split(':')[1]
-			else:
-				iList = True
-		elif action == 'update' and ('--format' in a or '-f' in a):
-			fList = 'py'
-		elif '--list' in a and not pList:
-			if ':' in a:
-				pList = a.split(':')[1]
-			else:
-				pList = True
-		elif '--local' in a or '-l' in a and not localRepo:
-			if ':' in a:
-				localRepo = a.split(':')[1]
-			else:
-				localRepo = True
-		elif '--smart' in a or '-s' in a and not smart:
-			if ':' in a:
-				smart = a.split(':')[1]
-			else:
-				smart = True
-		elif '--export' in a or '-e' in a and not export:
-			if ':' in a:
-				export = a.split(':')[1]
-			else:
-				export = True
-		elif a in ['search', 's'] and not action:
-			action = 'search'
-		elif a in ['install', 'i'] and not action:
-			action = 'install'
-		elif a in ['download', 'd'] and not action:
-			action = 'download'
-		elif a in ['wheel', 'w'] and not action:
-			action = 'wheel'
-		elif a in ['update', 'u'] and not action:
-			action = 'update'
-		elif a in ['version', 'v'] and not action:
-			action = 'version'
-		else:
-			if value is None:
-				value = ''
-			if value:
-				value += ' '
-			value += a
-
-	if action == 'update':
-		updateBuiltinList(eList, iList, fList)
-	else:
+import sys
+from . import *
+from .. import *
+
+exit = False
+if 'light' in status:
+	printErr('command line interface not available in light version')
+	exit = True
+
+if __name__ == '__main__' and not exit:
+	localRepo = False
+	action = None
+	value = None
+	pList = False
+	iList = False
+	eList = False
+	fList = 'txt'
+	smart = False
+	export = False
+	for a in sys.argv[1:]:
+		if action == 'update' and ('--export' in a or '-e' in a):
+			if ':' in a:
+				eList = a.split(':')[1]
+			else:
+				eList = True
+		elif action == 'update' and ('--import' in a or '-i' in a):
+			if ':' in a:
+				iList = a.split(':')[1]
+			else:
+				iList = True
+		elif action == 'update' and ('--format' in a or '-f' in a):
+			fList = 'py'
+		elif '--list' in a and not pList:
+			if ':' in a:
+				pList = a.split(':')[1]
+			else:
+				pList = True
+		elif '--local' in a or '-l' in a and not localRepo:
+			if ':' in a:
+				localRepo = a.split(':')[1]
+			else:
+				localRepo = True
+		elif '--smart' in a or '-s' in a and not smart:
+			if ':' in a:
+				smart = a.split(':')[1]
+			else:
+				smart = True
+		elif '--export' in a or '-e' in a and not export:
+			if ':' in a:
+				export = a.split(':')[1]
+			else:
+				export = True
+		elif a in ['search', 's'] and not action:
+			action = 'search'
+		elif a in ['install', 'i'] and not action:
+			action = 'install'
+		elif a in ['download', 'd'] and not action:
+			action = 'download'
+		elif a in ['wheel', 'w'] and not action:
+			action = 'wheel'
+		elif a in ['update', 'u'] and not action:
+			action = 'update'
+		elif a in ['version', 'v'] and not action:
+			action = 'version'
+		else:
+			if value is None:
+				value = ''
+			if value:
+				value += ' '
+			value += a
+
+	if action == 'update':
+		updateBuiltinList(eList, iList, fList)
+	else:
 		main(action, value=value, local=localRepo, list=pList, smart=smart, export=export)
```

### Comparing `prot-3.8.4/src/prot/pip/extra.py` & `prot-3.8.5/src/prot/pip/extra.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/pip/packagesList.py` & `prot-3.8.5/src/prot/pip/packagesList.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/progress/__init__.py` & `prot-3.8.5/src/prot/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/progress/bar.py` & `prot-3.8.5/src/prot/progress/bar.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/progress/counter.py` & `prot-3.8.5/src/prot/progress/counter.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/progress/spinner.py` & `prot-3.8.5/src/prot/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/__init__.py` & `prot-3.8.5/src/prot/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/application/__init__.py` & `prot-3.8.5/src/prot/prompt/application/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/application/application.py` & `prot-3.8.5/src/prot/prompt/application/application.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/application/current.py` & `prot-3.8.5/src/prot/prompt/application/current.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/application/dummy.py` & `prot-3.8.5/src/prot/prompt/application/dummy.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/application/run_in_terminal.py` & `prot-3.8.5/src/prot/prompt/application/run_in_terminal.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/auto_suggest.py` & `prot-3.8.5/src/prot/prompt/auto_suggest.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/buffer.py` & `prot-3.8.5/src/prot/prompt/buffer.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/cache.py` & `prot-3.8.5/src/prot/prompt/cache.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/clipboard/base.py` & `prot-3.8.5/src/prot/prompt/clipboard/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/clipboard/in_memory.py` & `prot-3.8.5/src/prot/prompt/clipboard/in_memory.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/clipboard/pyperclip.py` & `prot-3.8.5/src/prot/prompt/clipboard/pyperclip.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/completion/__init__.py` & `prot-3.8.5/src/prot/prompt/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/completion/base.py` & `prot-3.8.5/src/prot/prompt/completion/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/completion/filesystem.py` & `prot-3.8.5/src/prot/prompt/completion/filesystem.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/completion/fuzzy_completer.py` & `prot-3.8.5/src/prot/prompt/completion/fuzzy_completer.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/completion/nested.py` & `prot-3.8.5/src/prot/prompt/completion/nested.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/completion/word_completer.py` & `prot-3.8.5/src/prot/prompt/completion/word_completer.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/contrib/completers/system.py` & `prot-3.8.5/src/prot/prompt/contrib/completers/system.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/contrib/regular_languages/__init__.py` & `prot-3.8.5/src/prot/prompt/contrib/regular_languages/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/contrib/regular_languages/compiler.py` & `prot-3.8.5/src/prot/prompt/contrib/regular_languages/compiler.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/contrib/regular_languages/completion.py` & `prot-3.8.5/src/prot/prompt/contrib/regular_languages/completion.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/contrib/regular_languages/lexer.py` & `prot-3.8.5/src/prot/prompt/contrib/regular_languages/lexer.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/contrib/regular_languages/regex_parser.py` & `prot-3.8.5/src/prot/prompt/contrib/regular_languages/regex_parser.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/contrib/regular_languages/validation.py` & `prot-3.8.5/src/prot/prompt/contrib/regular_languages/validation.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/contrib/ssh/server.py` & `prot-3.8.5/src/prot/prompt/contrib/ssh/server.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/contrib/telnet/protocol.py` & `prot-3.8.5/src/prot/prompt/contrib/telnet/protocol.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/contrib/telnet/server.py` & `prot-3.8.5/src/prot/prompt/contrib/telnet/server.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/document.py` & `prot-3.8.5/src/prot/prompt/document.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/eventloop/__init__.py` & `prot-3.8.5/src/prot/prompt/eventloop/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/eventloop/async_context_manager.py` & `prot-3.8.5/src/prot/prompt/eventloop/async_context_manager.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/eventloop/async_generator.py` & `prot-3.8.5/src/prot/prompt/eventloop/async_generator.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/eventloop/dummy_contextvars.py` & `prot-3.8.5/src/prot/prompt/eventloop/dummy_contextvars.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/eventloop/inputhook.py` & `prot-3.8.5/src/prot/prompt/eventloop/inputhook.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/eventloop/utils.py` & `prot-3.8.5/src/prot/prompt/eventloop/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/eventloop/win32.py` & `prot-3.8.5/src/prot/prompt/eventloop/win32.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/filters/__init__.py` & `prot-3.8.5/src/prot/prompt/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/filters/app.py` & `prot-3.8.5/src/prot/prompt/filters/app.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/filters/base.py` & `prot-3.8.5/src/prot/prompt/filters/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/filters/cli.py` & `prot-3.8.5/src/prot/prompt/filters/cli.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/filters/utils.py` & `prot-3.8.5/src/prot/prompt/filters/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/formatted_text/__init__.py` & `prot-3.8.5/src/prot/prompt/formatted_text/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/formatted_text/ansi.py` & `prot-3.8.5/src/prot/prompt/formatted_text/ansi.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/formatted_text/base.py` & `prot-3.8.5/src/prot/prompt/formatted_text/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/formatted_text/html.py` & `prot-3.8.5/src/prot/prompt/formatted_text/html.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/formatted_text/pygments.py` & `prot-3.8.5/src/prot/prompt/formatted_text/pygments.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/formatted_text/utils.py` & `prot-3.8.5/src/prot/prompt/formatted_text/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/history.py` & `prot-3.8.5/src/prot/prompt/history.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/input/ansi_escape_sequences.py` & `prot-3.8.5/src/prot/prompt/input/ansi_escape_sequences.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/input/base.py` & `prot-3.8.5/src/prot/prompt/input/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/input/defaults.py` & `prot-3.8.5/src/prot/prompt/input/defaults.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/input/posix_pipe.py` & `prot-3.8.5/src/prot/prompt/input/posix_pipe.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/input/posix_utils.py` & `prot-3.8.5/src/prot/prompt/input/posix_utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/input/typeahead.py` & `prot-3.8.5/src/prot/prompt/input/typeahead.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/input/vt100.py` & `prot-3.8.5/src/prot/prompt/input/vt100.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/input/vt100_parser.py` & `prot-3.8.5/src/prot/prompt/input/vt100_parser.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/input/win32.py` & `prot-3.8.5/src/prot/prompt/input/win32.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/input/win32_pipe.py` & `prot-3.8.5/src/prot/prompt/input/win32_pipe.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/bindings/auto_suggest.py` & `prot-3.8.5/src/prot/prompt/key_binding/bindings/auto_suggest.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/bindings/basic.py` & `prot-3.8.5/src/prot/prompt/key_binding/bindings/basic.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/bindings/completion.py` & `prot-3.8.5/src/prot/prompt/key_binding/bindings/completion.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/bindings/cpr.py` & `prot-3.8.5/src/prot/prompt/key_binding/bindings/cpr.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/bindings/emacs.py` & `prot-3.8.5/src/prot/prompt/key_binding/bindings/emacs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/bindings/mouse.py` & `prot-3.8.5/src/prot/prompt/key_binding/bindings/mouse.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/bindings/named_commands.py` & `prot-3.8.5/src/prot/prompt/key_binding/bindings/named_commands.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/bindings/open_in_editor.py` & `prot-3.8.5/src/prot/prompt/key_binding/bindings/open_in_editor.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/bindings/page_navigation.py` & `prot-3.8.5/src/prot/prompt/key_binding/bindings/page_navigation.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/bindings/scroll.py` & `prot-3.8.5/src/prot/prompt/key_binding/bindings/scroll.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/bindings/search.py` & `prot-3.8.5/src/prot/prompt/key_binding/bindings/search.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/bindings/vi.py` & `prot-3.8.5/src/prot/prompt/key_binding/bindings/vi.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/defaults.py` & `prot-3.8.5/src/prot/prompt/key_binding/defaults.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/digraphs.py` & `prot-3.8.5/src/prot/prompt/key_binding/digraphs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/emacs_state.py` & `prot-3.8.5/src/prot/prompt/key_binding/emacs_state.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/key_bindings.py` & `prot-3.8.5/src/prot/prompt/key_binding/key_bindings.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/key_processor.py` & `prot-3.8.5/src/prot/prompt/key_binding/key_processor.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/key_binding/vi_state.py` & `prot-3.8.5/src/prot/prompt/key_binding/vi_state.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/keys.py` & `prot-3.8.5/src/prot/prompt/keys.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/layout/__init__.py` & `prot-3.8.5/src/prot/prompt/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/layout/containers.py` & `prot-3.8.5/src/prot/prompt/layout/containers.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/layout/controls.py` & `prot-3.8.5/src/prot/prompt/layout/controls.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/layout/dimension.py` & `prot-3.8.5/src/prot/prompt/layout/dimension.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/layout/dummy.py` & `prot-3.8.5/src/prot/prompt/layout/dummy.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/layout/layout.py` & `prot-3.8.5/src/prot/prompt/layout/layout.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/layout/margins.py` & `prot-3.8.5/src/prot/prompt/layout/margins.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/layout/menus.py` & `prot-3.8.5/src/prot/prompt/layout/menus.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/layout/mouse_handlers.py` & `prot-3.8.5/src/prot/prompt/layout/mouse_handlers.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/layout/processors.py` & `prot-3.8.5/src/prot/prompt/layout/processors.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/layout/screen.py` & `prot-3.8.5/src/prot/prompt/layout/screen.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/layout/utils.py` & `prot-3.8.5/src/prot/prompt/layout/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/lexers/base.py` & `prot-3.8.5/src/prot/prompt/lexers/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/lexers/pygments.py` & `prot-3.8.5/src/prot/prompt/lexers/pygments.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/mouse_events.py` & `prot-3.8.5/src/prot/prompt/mouse_events.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/output/base.py` & `prot-3.8.5/src/prot/prompt/output/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/output/color_depth.py` & `prot-3.8.5/src/prot/prompt/output/color_depth.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/output/conemu.py` & `prot-3.8.5/src/prot/prompt/output/conemu.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/output/defaults.py` & `prot-3.8.5/src/prot/prompt/output/defaults.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/output/vt100.py` & `prot-3.8.5/src/prot/prompt/output/vt100.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/output/win32.py` & `prot-3.8.5/src/prot/prompt/output/win32.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/output/windows10.py` & `prot-3.8.5/src/prot/prompt/output/windows10.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/patch_stdout.py` & `prot-3.8.5/src/prot/prompt/patch_stdout.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/renderer.py` & `prot-3.8.5/src/prot/prompt/renderer.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/search.py` & `prot-3.8.5/src/prot/prompt/search.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/selection.py` & `prot-3.8.5/src/prot/prompt/selection.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/shortcuts/__init__.py` & `prot-3.8.5/src/prot/prompt/shortcuts/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/shortcuts/dialogs.py` & `prot-3.8.5/src/prot/prompt/shortcuts/dialogs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/shortcuts/progress_bar/base.py` & `prot-3.8.5/src/prot/prompt/shortcuts/progress_bar/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/shortcuts/progress_bar/formatters.py` & `prot-3.8.5/src/prot/prompt/shortcuts/progress_bar/formatters.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/shortcuts/prompt.py` & `prot-3.8.5/src/prot/prompt/shortcuts/prompt.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/shortcuts/utils.py` & `prot-3.8.5/src/prot/prompt/shortcuts/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/styles/__init__.py` & `prot-3.8.5/src/prot/prompt/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/styles/base.py` & `prot-3.8.5/src/prot/prompt/styles/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/styles/defaults.py` & `prot-3.8.5/src/prot/prompt/styles/defaults.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/styles/named_colors.py` & `prot-3.8.5/src/prot/prompt/styles/named_colors.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/styles/pygments.py` & `prot-3.8.5/src/prot/prompt/styles/pygments.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/styles/style.py` & `prot-3.8.5/src/prot/prompt/styles/style.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/styles/style_transformation.py` & `prot-3.8.5/src/prot/prompt/styles/style_transformation.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/utils.py` & `prot-3.8.5/src/prot/prompt/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/validation.py` & `prot-3.8.5/src/prot/prompt/validation.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/widgets/__init__.py` & `prot-3.8.5/src/prot/prompt/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/widgets/base.py` & `prot-3.8.5/src/prot/prompt/widgets/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/widgets/dialogs.py` & `prot-3.8.5/src/prot/prompt/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/widgets/menus.py` & `prot-3.8.5/src/prot/prompt/widgets/menus.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/widgets/toolbars.py` & `prot-3.8.5/src/prot/prompt/widgets/toolbars.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/prompt/win32_types.py` & `prot-3.8.5/src/prot/prompt/win32_types.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/wcwidth/table_wide.py` & `prot-3.8.5/src/prot/wcwidth/table_wide.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/wcwidth/table_zero.py` & `prot-3.8.5/src/prot/wcwidth/table_zero.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/wcwidth/tests/test_core.py` & `prot-3.8.5/src/prot/wcwidth/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot/wcwidth/wcwidth.py` & `prot-3.8.5/src/prot/wcwidth/wcwidth.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.4/src/prot.egg-info/SOURCES.txt` & `prot-3.8.5/src/prot.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-MANIFEST.in
+LICENSE
 README.md
 setup.py
-protbuilder/__init__.pyc
-protbuilder/__version__.pyc
-protbuilder/color/__init__.pyc
-protbuilder/color/ansi.pyc
-protbuilder/color/ansitowin32.pyc
-protbuilder/color/initialise.pyc
-protbuilder/color/win32.pyc
-protbuilder/color/winterm.pyc
 src/prot/__init__.py
 src/prot/__main__.py
 src/prot/__version__.py
 src/prot/code.py
 src/prot.egg-info/PKG-INFO
 src/prot.egg-info/SOURCES.txt
 src/prot.egg-info/dependency_links.txt
 src/prot.egg-info/entry_points.txt
-src/prot.egg-info/not-zip-safe
 src/prot.egg-info/top_level.txt
 src/prot/bs/__init__.py
 src/prot/bs/bs.py
 src/prot/bs/bsMap.py
 src/prot/bs/bsPro.py
 src/prot/bs/bsSpaz.py
 src/prot/bs/stdLib/__init__.py
```

