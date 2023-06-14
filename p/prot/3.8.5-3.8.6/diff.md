# Comparing `tmp/prot-3.8.5.tar.gz` & `tmp/prot-3.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prot-3.8.5.tar", last modified: Wed Jun 14 19:45:20 2023, max compression
+gzip compressed data, was "prot-3.8.6.tar", last modified: Wed Jun 14 20:11:13 2023, max compression
```

## Comparing `prot-3.8.5.tar` & `prot-3.8.6.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.554239 prot-3.8.5/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1069 2023-06-14 19:42:21.000000 prot-3.8.5/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1761 2023-06-14 19:45:20.554239 prot-3.8.5/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-06-14 19:42:21.000000 prot-3.8.5/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-14 19:45:20.554239 prot-3.8.5/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      801 2023-06-14 19:42:21.000000 prot-3.8.5/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.438239 prot-3.8.5/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.450239 prot-3.8.5/src/prot/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    38776 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2998 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/__main__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/__version__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.454239 prot-3.8.5/src/prot/bs/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      177 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5526 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/bs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2182 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/bsMap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      764 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/bsPro.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1236 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/bsSpaz.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.494239 prot-3.8.5/src/prot/bs/stdLib/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      190 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2189 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/alwaysLandLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4352 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bigGDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1568 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bridgitLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2261 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37874 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsAchievement.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8330 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsAssault.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34286 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsBomb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18154 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsCaptureTheFlag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11373 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsChosenOne.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9234 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsConquest.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    96453 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsCoopGame.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5888 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsDeathMatch.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9248 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsEasterEggHunt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19687 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsElimination.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10709 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsFlag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27224 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsFootball.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   116735 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsGame.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12498 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsHockey.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      172 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsInternal.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7611 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsKeepAway.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsKingOfTheHill.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   155086 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageArabic.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   158524 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageBelarussian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   127437 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageChinese.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   118386 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageCroatian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   135541 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageCzech.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    94441 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageDanish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   141350 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageDutch.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   111226 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageEnglish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   105204 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageEsperanto.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   146287 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageFrench.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   148309 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageGerman.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   141903 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageGibberish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   187394 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageGreek.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   212586 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageHindi.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   137372 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageHungarian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   126188 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageIndonesian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   144849 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageItalian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   138448 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageKorean.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   162405 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguagePersian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   144892 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguagePolish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   145117 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguagePortuguese.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   121744 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageRomanian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   183660 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageRussian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   168786 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageSerbian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   142925 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageSpanish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   125252 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageSwedish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   129359 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageTurkish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   169058 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLanguageUkrainian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34599 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsLobby.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37628 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsMainMenu.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58253 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsMap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9381 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsMeteorShower.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6444 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsNinjaFight.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    48080 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsOnslaught.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11026 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsPowerup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24920 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsRace.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43185 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsRunaround.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12031 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsScoreBoard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12856 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsScoreSet.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18997 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsServerData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   141126 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsSpaz.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12571 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsTargetPractice.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58723 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsTeamGame.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10326 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsTheLastStand.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    63826 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsTutorial.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1093681 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsUI.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53124 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsUI2.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   188532 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsUtils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3224 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/bsVector.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3767 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/courtyardLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2120 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/cragCastleDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1635 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/doomShroomLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1513 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/footballStadiumDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1360 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/hockeyStadiumDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4179 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/lakeFrigidDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1674 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/monkeyFaceLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1448 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/rampageLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1491 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/roundaboutLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2377 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/stepRightUpLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1719 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/thePadLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2028 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/tipTopLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3284 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/towerDLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2234 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/bs/stdLib/zigZagLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12398 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/code.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.498239 prot-3.8.5/src/prot/color/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      239 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/color/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2524 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/color/ansi.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10462 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/color/ansitowin32.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1915 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/color/initialise.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5404 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/color/win32.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6438 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/color/winterm.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.498239 prot-3.8.5/src/prot/pip/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9136 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/pip/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1827 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/pip/__main__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      755 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/pip/extra.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  4056147 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/pip/packagesList.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.506239 prot-3.8.5/src/prot/progress/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4910 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/progress/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2854 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/progress/bar.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1372 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/progress/counter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1380 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/progress/spinner.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.510239 prot-3.8.5/src/prot/prompt/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      872 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.514239 prot-3.8.5/src/prot/prompt/application/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      519 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/application/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44248 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/application/application.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5051 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/application/current.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1349 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/application/dummy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3699 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/application/run_in_terminal.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5919 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/auto_suggest.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    70342 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/buffer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3768 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/cache.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.514239 prot-3.8.5/src/prot/prompt/clipboard/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      403 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/clipboard/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2489 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/clipboard/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1077 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/clipboard/in_memory.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1147 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/clipboard/pyperclip.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.518239 prot-3.8.5/src/prot/prompt/completion/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      810 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/completion/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11493 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/completion/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3832 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/completion/filesystem.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6945 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/completion/fuzzy_completer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3885 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/completion/nested.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2934 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/completion/word_completer.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.518239 prot-3.8.5/src/prot/prompt/contrib/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:42:40.000000 prot-3.8.5/src/prot/prompt/contrib/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.518239 prot-3.8.5/src/prot/prompt/contrib/completers/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       36 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/completers/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2012 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/completers/system.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.518239 prot-3.8.5/src/prot/prompt/contrib/regular_languages/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3220 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/regular_languages/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21889 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/regular_languages/compiler.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3239 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/regular_languages/completion.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3386 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/regular_languages/lexer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7827 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/regular_languages/regex_parser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/regular_languages/validation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.518239 prot-3.8.5/src/prot/prompt/contrib/ssh/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      138 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/ssh/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4365 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/ssh/server.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.522239 prot-3.8.5/src/prot/prompt/contrib/telnet/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       68 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/telnet/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      130 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/telnet/log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4974 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/telnet/protocol.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9518 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/contrib/telnet/server.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      187 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/data_structures.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    40593 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/document.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/enums.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.522239 prot-3.8.5/src/prot/prompt/eventloop/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      636 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4125 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/async_context_manager.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1711 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/async_generator.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1117 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/dummy_contextvars.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5514 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/inputhook.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3251 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2008 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/eventloop/win32.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.522239 prot-3.8.5/src/prot/prompt/filters/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1028 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/filters/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9276 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/filters/app.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5737 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/filters/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1830 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/filters/cli.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      848 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/filters/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.526239 prot-3.8.5/src/prot/prompt/formatted_text/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1378 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/formatted_text/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8089 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/formatted_text/ansi.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4881 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/formatted_text/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4328 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/formatted_text/html.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      756 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/formatted_text/pygments.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2747 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/formatted_text/utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7131 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/history.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.530239 prot-3.8.5/src/prot/prompt/input/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      209 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13116 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/ansi_escape_sequences.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3275 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1522 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/defaults.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1835 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/posix_pipe.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3897 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/posix_utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2538 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/typeahead.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10131 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/vt100.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8402 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/vt100_parser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22282 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/win32.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4111 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/input/win32_pipe.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.534239 prot-3.8.5/src/prot/prompt/key_binding/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      335 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.538239 prot-3.8.5/src/prot/prompt/key_binding/bindings/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:42:40.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1736 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/auto_suggest.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7105 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/basic.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6841 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/completion.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      744 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/cpr.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19627 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/emacs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      468 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/focus.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4946 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/mouse.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18371 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/named_commands.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1282 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/open_in_editor.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2303 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/page_navigation.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5573 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/scroll.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2583 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/search.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    75161 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/bindings/vi.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1917 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/defaults.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    32798 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/digraphs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      895 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/emacs_state.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19390 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/key_bindings.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17631 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/key_processor.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3316 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/key_binding/vi_state.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4885 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/keys.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.542239 prot-3.8.5/src/prot/prompt/layout/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3462 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97489 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/containers.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34955 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/controls.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6941 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/dimension.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1001 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/dummy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14088 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/layout.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10373 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/margins.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25365 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/menus.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1043 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/mouse_handlers.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34137 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/processors.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9745 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/screen.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2259 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/layout/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.542239 prot-3.8.5/src/prot/prompt/lexers/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      372 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/lexers/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2322 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/lexers/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11940 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/lexers/pygments.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      116 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1339 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/mouse_events.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.546239 prot-3.8.5/src/prot/prompt/output/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      244 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6324 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2199 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/color_depth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1487 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/conemu.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1886 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/defaults.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21317 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/vt100.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21140 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/win32.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2794 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/output/windows10.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5155 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/patch_stdout.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25735 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/renderer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6997 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/search.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1289 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/selection.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.546239 prot-3.8.5/src/prot/prompt/shortcuts/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      844 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8424 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/dialogs.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.546239 prot-3.8.5/src/prot/prompt/shortcuts/progress_bar/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      458 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/progress_bar/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14070 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/progress_bar/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11767 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/progress_bar/formatters.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57251 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/prompt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5707 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/shortcuts/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.550239 prot-3.8.5/src/prot/prompt/styles/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1603 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5062 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8363 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/defaults.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4355 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/named_colors.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1952 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/pygments.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13023 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/style.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12437 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/styles/style_transformation.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       85 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/token.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8119 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5837 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/validation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.550239 prot-3.8.5/src/prot/prompt/widgets/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1181 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/widgets/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    28404 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/widgets/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3349 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/widgets/dialogs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12736 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/widgets/menus.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12193 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/widgets/toolbars.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4138 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/prompt/win32_types.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.554239 prot-3.8.5/src/prot/wcwidth/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      140 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/wcwidth/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8004 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/wcwidth/table_wide.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24250 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/wcwidth/table_zero.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.554239 prot-3.8.5/src/prot/wcwidth/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/wcwidth/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3891 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/wcwidth/tests/test_core.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7831 2023-06-14 19:42:21.000000 prot-3.8.5/src/prot/wcwidth/wcwidth.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:45:20.450239 prot-3.8.5/src/prot.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1761 2023-06-14 19:45:20.000000 prot-3.8.5/src/prot.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9449 2023-06-14 19:45:20.000000 prot-3.8.5/src/prot.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-14 19:45:20.000000 prot-3.8.5/src/prot.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       59 2023-06-14 19:45:20.000000 prot-3.8.5/src/prot.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        5 2023-06-14 19:45:20.000000 prot-3.8.5/src/prot.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.394239 prot-3.8.6/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1069 2023-06-14 19:42:21.000000 prot-3.8.6/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2341 2023-06-14 20:11:13.394239 prot-3.8.6/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1444 2023-06-14 19:51:52.000000 prot-3.8.6/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-14 20:11:13.398239 prot-3.8.6/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1429 2023-06-14 20:08:19.000000 prot-3.8.6/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.170239 prot-3.8.6/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.190239 prot-3.8.6/src/prot/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    38776 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2998 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/__main__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-06-14 20:11:13.000000 prot-3.8.6/src/prot/__version__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.198239 prot-3.8.6/src/prot/bs/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      177 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5526 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/bs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2182 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/bsMap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      764 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/bsPro.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1236 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/bsSpaz.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.290239 prot-3.8.6/src/prot/bs/stdLib/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      190 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2189 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/alwaysLandLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4352 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bigGDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1568 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bridgitLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2261 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37874 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsAchievement.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8330 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsAssault.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34286 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsBomb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18154 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsCaptureTheFlag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11373 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsChosenOne.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9234 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsConquest.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    96453 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsCoopGame.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5888 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsDeathMatch.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9248 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsEasterEggHunt.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19687 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsElimination.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10709 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsFlag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27224 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsFootball.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   116735 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsGame.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12498 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsHockey.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      172 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsInternal.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7611 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsKeepAway.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsKingOfTheHill.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   155086 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageArabic.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   158524 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageBelarussian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   127437 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageChinese.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   118386 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageCroatian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   135541 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageCzech.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    94441 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageDanish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   141350 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageDutch.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   111226 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageEnglish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   105204 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageEsperanto.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   146287 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageFrench.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   148309 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageGerman.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   141903 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageGibberish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   187394 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageGreek.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   212586 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageHindi.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   137372 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageHungarian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   126188 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageIndonesian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   144849 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageItalian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   138448 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageKorean.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   162405 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguagePersian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   144892 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguagePolish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   145117 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguagePortuguese.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   121744 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageRomanian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   183660 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageRussian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   168786 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageSerbian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   142925 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageSpanish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   125252 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageSwedish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   129359 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageTurkish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   169058 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageUkrainian.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34599 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLobby.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37628 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsMainMenu.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58253 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsMap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9381 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsMeteorShower.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6444 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsNinjaFight.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    48080 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsOnslaught.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11026 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsPowerup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24920 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsRace.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43185 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsRunaround.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12031 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsScoreBoard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12856 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsScoreSet.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18997 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsServerData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   141126 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsSpaz.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12571 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsTargetPractice.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58723 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsTeamGame.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10326 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsTheLastStand.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    63826 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsTutorial.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1093681 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsUI.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53124 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsUI2.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   188532 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsUtils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3224 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsVector.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3767 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/courtyardLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2120 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/cragCastleDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1635 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/doomShroomLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1513 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/footballStadiumDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1360 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/hockeyStadiumDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4179 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/lakeFrigidDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1674 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/monkeyFaceLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1448 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/rampageLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1491 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/roundaboutLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2377 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/stepRightUpLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1719 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/thePadLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2028 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/tipTopLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3284 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/towerDLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2234 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/zigZagLevelDefs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12398 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/code.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.294239 prot-3.8.6/src/prot/color/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      239 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/color/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2524 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/color/ansi.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10462 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/color/ansitowin32.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1915 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/color/initialise.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5404 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/color/win32.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6438 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/color/winterm.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.294239 prot-3.8.6/src/prot/pip/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9136 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/pip/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1827 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/pip/__main__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      755 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/pip/extra.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)  4056147 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/pip/packagesList.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.302239 prot-3.8.6/src/prot/progress/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4910 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/progress/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2854 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/progress/bar.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1372 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/progress/counter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1380 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/progress/spinner.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.314239 prot-3.8.6/src/prot/prompt/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      872 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.318239 prot-3.8.6/src/prot/prompt/application/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      519 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/application/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44248 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/application/application.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5051 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/application/current.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1349 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/application/dummy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3699 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/application/run_in_terminal.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5919 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/auto_suggest.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    70342 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/buffer.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3768 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/cache.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.318239 prot-3.8.6/src/prot/prompt/clipboard/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      403 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/clipboard/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2489 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/clipboard/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1077 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/clipboard/in_memory.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1147 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/clipboard/pyperclip.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.322239 prot-3.8.6/src/prot/prompt/completion/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      810 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/completion/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11493 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/completion/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3832 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/completion/filesystem.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6945 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/completion/fuzzy_completer.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3885 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/completion/nested.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2934 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/completion/word_completer.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.322239 prot-3.8.6/src/prot/prompt/contrib/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:42:40.000000 prot-3.8.6/src/prot/prompt/contrib/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.326239 prot-3.8.6/src/prot/prompt/contrib/completers/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       36 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/completers/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2012 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/completers/system.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.330239 prot-3.8.6/src/prot/prompt/contrib/regular_languages/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3220 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/regular_languages/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21889 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/regular_languages/compiler.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3239 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/regular_languages/completion.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3386 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/regular_languages/lexer.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7827 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/regular_languages/regex_parser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/regular_languages/validation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.330239 prot-3.8.6/src/prot/prompt/contrib/ssh/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      138 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/ssh/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4365 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/ssh/server.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.334239 prot-3.8.6/src/prot/prompt/contrib/telnet/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       68 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/telnet/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      130 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/telnet/log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4974 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/telnet/protocol.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9518 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/telnet/server.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      187 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/data_structures.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    40593 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/document.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/enums.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.338239 prot-3.8.6/src/prot/prompt/eventloop/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      636 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4125 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/async_context_manager.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1711 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/async_generator.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1117 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/dummy_contextvars.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5514 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/inputhook.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3251 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/utils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2008 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/win32.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.342239 prot-3.8.6/src/prot/prompt/filters/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1028 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/filters/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9276 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/filters/app.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5737 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/filters/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1830 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/filters/cli.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      848 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/filters/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.346239 prot-3.8.6/src/prot/prompt/formatted_text/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1378 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/formatted_text/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8089 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/formatted_text/ansi.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4881 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/formatted_text/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4328 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/formatted_text/html.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      756 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/formatted_text/pygments.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2747 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/formatted_text/utils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7131 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/history.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.354239 prot-3.8.6/src/prot/prompt/input/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      209 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13116 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/ansi_escape_sequences.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3275 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1522 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/defaults.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1835 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/posix_pipe.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3897 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/posix_utils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2538 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/typeahead.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10131 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/vt100.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8402 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/vt100_parser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22282 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/win32.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4111 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/win32_pipe.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.358239 prot-3.8.6/src/prot/prompt/key_binding/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      335 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.366239 prot-3.8.6/src/prot/prompt/key_binding/bindings/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:42:40.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1736 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/auto_suggest.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7105 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/basic.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6841 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/completion.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      744 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/cpr.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19627 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/emacs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      468 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/focus.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4946 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/mouse.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18371 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/named_commands.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1282 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/open_in_editor.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2303 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/page_navigation.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5573 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/scroll.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2583 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/search.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    75161 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/vi.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1917 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/defaults.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    32798 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/digraphs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      895 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/emacs_state.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19390 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/key_bindings.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17631 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/key_processor.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3316 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/vi_state.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4885 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/keys.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.374239 prot-3.8.6/src/prot/prompt/layout/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3462 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97489 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/containers.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34955 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/controls.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6941 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/dimension.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1001 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/dummy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14088 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/layout.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10373 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/margins.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25365 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/menus.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1043 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/mouse_handlers.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34137 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/processors.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9745 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/screen.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2259 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.374239 prot-3.8.6/src/prot/prompt/lexers/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      372 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/lexers/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2322 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/lexers/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11940 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/lexers/pygments.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      116 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1339 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/mouse_events.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.378239 prot-3.8.6/src/prot/prompt/output/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      244 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6324 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2199 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/color_depth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1487 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/conemu.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1886 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/defaults.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21317 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/vt100.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21140 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/win32.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2794 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/windows10.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5155 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/patch_stdout.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25735 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/renderer.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6997 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/search.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1289 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/selection.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.382239 prot-3.8.6/src/prot/prompt/shortcuts/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      844 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8424 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/dialogs.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.386239 prot-3.8.6/src/prot/prompt/shortcuts/progress_bar/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      458 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/progress_bar/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14070 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/progress_bar/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11767 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/progress_bar/formatters.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57251 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/prompt.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5707 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.390239 prot-3.8.6/src/prot/prompt/styles/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1603 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5062 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8363 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/defaults.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4355 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/named_colors.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1952 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/pygments.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13023 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/style.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12437 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/style_transformation.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       85 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/token.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8119 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/utils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5837 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/validation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.390239 prot-3.8.6/src/prot/prompt/widgets/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1181 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/widgets/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    28404 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/widgets/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3349 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/widgets/dialogs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12736 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/widgets/menus.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12193 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/widgets/toolbars.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4138 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/win32_types.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.394239 prot-3.8.6/src/prot/wcwidth/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      140 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/wcwidth/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8004 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/wcwidth/table_wide.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24250 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/wcwidth/table_zero.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.394239 prot-3.8.6/src/prot/wcwidth/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/wcwidth/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3891 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/wcwidth/tests/test_core.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7831 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/wcwidth/wcwidth.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.194239 prot-3.8.6/src/prot.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2341 2023-06-14 20:11:13.000000 prot-3.8.6/src/prot.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9449 2023-06-14 20:11:13.000000 prot-3.8.6/src/prot.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-14 20:11:13.000000 prot-3.8.6/src/prot.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       59 2023-06-14 20:11:13.000000 prot-3.8.6/src/prot.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        5 2023-06-14 20:11:13.000000 prot-3.8.6/src/prot.egg-info/top_level.txt
```

### Comparing `prot-3.8.5/LICENSE` & `prot-3.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/README.md` & `prot-3.8.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 Prot - Pro Tools for Python 3
 
 [![Downloads](https://static.pepy.tech/badge/prot)](https://pepy.tech/project/prot)
 
-
-=============================
-
 Modules
 -------
 
  * **classes**
  * **functions**
  * **converters**
  * **settings**
```

### Comparing `prot-3.8.5/src/prot/__init__.py` & `prot-3.8.6/src/prot/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/__main__.py` & `prot-3.8.6/src/prot/__main__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/bs.py` & `prot-3.8.6/src/prot/bs/bs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/bsMap.py` & `prot-3.8.6/src/prot/bs/bsMap.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/bsPro.py` & `prot-3.8.6/src/prot/bs/bsPro.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/bsSpaz.py` & `prot-3.8.6/src/prot/bs/bsSpaz.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/alwaysLandLevelDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/alwaysLandLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bigGDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/bigGDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bridgitLevelDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/bridgitLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bs.py` & `prot-3.8.6/src/prot/bs/stdLib/bs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsAchievement.py` & `prot-3.8.6/src/prot/bs/stdLib/bsAchievement.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsAssault.py` & `prot-3.8.6/src/prot/bs/stdLib/bsAssault.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsBomb.py` & `prot-3.8.6/src/prot/bs/stdLib/bsBomb.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsCaptureTheFlag.py` & `prot-3.8.6/src/prot/bs/stdLib/bsCaptureTheFlag.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsChosenOne.py` & `prot-3.8.6/src/prot/bs/stdLib/bsChosenOne.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsConquest.py` & `prot-3.8.6/src/prot/bs/stdLib/bsConquest.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsCoopGame.py` & `prot-3.8.6/src/prot/bs/stdLib/bsCoopGame.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsDeathMatch.py` & `prot-3.8.6/src/prot/bs/stdLib/bsDeathMatch.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsEasterEggHunt.py` & `prot-3.8.6/src/prot/bs/stdLib/bsEasterEggHunt.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsElimination.py` & `prot-3.8.6/src/prot/bs/stdLib/bsElimination.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsFlag.py` & `prot-3.8.6/src/prot/bs/stdLib/bsFlag.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsFootball.py` & `prot-3.8.6/src/prot/bs/stdLib/bsFootball.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsGame.py` & `prot-3.8.6/src/prot/bs/stdLib/bsGame.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsHockey.py` & `prot-3.8.6/src/prot/bs/stdLib/bsHockey.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsKeepAway.py` & `prot-3.8.6/src/prot/bs/stdLib/bsKeepAway.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsKingOfTheHill.py` & `prot-3.8.6/src/prot/bs/stdLib/bsKingOfTheHill.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageArabic.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageArabic.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageBelarussian.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageBelarussian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageChinese.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageChinese.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageCroatian.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageCroatian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageCzech.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageCzech.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageDanish.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageDanish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageDutch.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageDutch.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageEnglish.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageEnglish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageEsperanto.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageEsperanto.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageFrench.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageFrench.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageGerman.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageGerman.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageGibberish.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageGibberish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageGreek.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageGreek.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageHindi.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageHindi.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageHungarian.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageHungarian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageIndonesian.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageIndonesian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageItalian.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageItalian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageKorean.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageKorean.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguagePersian.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguagePersian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguagePolish.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguagePolish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguagePortuguese.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguagePortuguese.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageRomanian.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageRomanian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageRussian.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageRussian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageSerbian.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageSerbian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageSpanish.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageSpanish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageSwedish.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageSwedish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageTurkish.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageTurkish.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLanguageUkrainian.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLanguageUkrainian.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsLobby.py` & `prot-3.8.6/src/prot/bs/stdLib/bsLobby.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsMainMenu.py` & `prot-3.8.6/src/prot/bs/stdLib/bsMainMenu.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsMap.py` & `prot-3.8.6/src/prot/bs/stdLib/bsMap.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsMeteorShower.py` & `prot-3.8.6/src/prot/bs/stdLib/bsMeteorShower.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsNinjaFight.py` & `prot-3.8.6/src/prot/bs/stdLib/bsNinjaFight.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsOnslaught.py` & `prot-3.8.6/src/prot/bs/stdLib/bsOnslaught.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsPowerup.py` & `prot-3.8.6/src/prot/bs/stdLib/bsPowerup.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsRace.py` & `prot-3.8.6/src/prot/bs/stdLib/bsRace.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsRunaround.py` & `prot-3.8.6/src/prot/bs/stdLib/bsRunaround.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsScoreBoard.py` & `prot-3.8.6/src/prot/bs/stdLib/bsScoreBoard.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsScoreSet.py` & `prot-3.8.6/src/prot/bs/stdLib/bsScoreSet.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsServerData.py` & `prot-3.8.6/src/prot/bs/stdLib/bsServerData.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsSpaz.py` & `prot-3.8.6/src/prot/bs/stdLib/bsSpaz.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsTargetPractice.py` & `prot-3.8.6/src/prot/bs/stdLib/bsTargetPractice.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsTeamGame.py` & `prot-3.8.6/src/prot/bs/stdLib/bsTeamGame.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsTheLastStand.py` & `prot-3.8.6/src/prot/bs/stdLib/bsTheLastStand.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsTutorial.py` & `prot-3.8.6/src/prot/bs/stdLib/bsTutorial.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsUI.py` & `prot-3.8.6/src/prot/bs/stdLib/bsUI.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsUI2.py` & `prot-3.8.6/src/prot/bs/stdLib/bsUI2.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsUtils.py` & `prot-3.8.6/src/prot/bs/stdLib/bsUtils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/bsVector.py` & `prot-3.8.6/src/prot/bs/stdLib/bsVector.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/courtyardLevelDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/courtyardLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/cragCastleDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/cragCastleDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/doomShroomLevelDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/doomShroomLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/footballStadiumDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/footballStadiumDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/hockeyStadiumDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/hockeyStadiumDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/lakeFrigidDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/lakeFrigidDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/monkeyFaceLevelDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/monkeyFaceLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/rampageLevelDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/rampageLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/roundaboutLevelDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/roundaboutLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/stepRightUpLevelDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/stepRightUpLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/thePadLevelDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/thePadLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/tipTopLevelDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/tipTopLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/towerDLevelDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/towerDLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/bs/stdLib/zigZagLevelDefs.py` & `prot-3.8.6/src/prot/bs/stdLib/zigZagLevelDefs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/code.py` & `prot-3.8.6/src/prot/code.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/color/ansi.py` & `prot-3.8.6/src/prot/color/ansi.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/color/ansitowin32.py` & `prot-3.8.6/src/prot/color/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/color/initialise.py` & `prot-3.8.6/src/prot/color/initialise.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/color/win32.py` & `prot-3.8.6/src/prot/color/win32.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/color/winterm.py` & `prot-3.8.6/src/prot/color/winterm.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/pip/__init__.py` & `prot-3.8.6/src/prot/pip/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/pip/__main__.py` & `prot-3.8.6/src/prot/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/pip/extra.py` & `prot-3.8.6/src/prot/pip/extra.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/pip/packagesList.py` & `prot-3.8.6/src/prot/pip/packagesList.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/progress/__init__.py` & `prot-3.8.6/src/prot/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/progress/bar.py` & `prot-3.8.6/src/prot/progress/bar.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/progress/counter.py` & `prot-3.8.6/src/prot/progress/counter.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/progress/spinner.py` & `prot-3.8.6/src/prot/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/__init__.py` & `prot-3.8.6/src/prot/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/application/__init__.py` & `prot-3.8.6/src/prot/prompt/application/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/application/application.py` & `prot-3.8.6/src/prot/prompt/application/application.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/application/current.py` & `prot-3.8.6/src/prot/prompt/application/current.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/application/dummy.py` & `prot-3.8.6/src/prot/prompt/application/dummy.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/application/run_in_terminal.py` & `prot-3.8.6/src/prot/prompt/application/run_in_terminal.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/auto_suggest.py` & `prot-3.8.6/src/prot/prompt/auto_suggest.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/buffer.py` & `prot-3.8.6/src/prot/prompt/buffer.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/cache.py` & `prot-3.8.6/src/prot/prompt/cache.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/clipboard/base.py` & `prot-3.8.6/src/prot/prompt/clipboard/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/clipboard/in_memory.py` & `prot-3.8.6/src/prot/prompt/clipboard/in_memory.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/clipboard/pyperclip.py` & `prot-3.8.6/src/prot/prompt/clipboard/pyperclip.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/completion/__init__.py` & `prot-3.8.6/src/prot/prompt/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/completion/base.py` & `prot-3.8.6/src/prot/prompt/completion/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/completion/filesystem.py` & `prot-3.8.6/src/prot/prompt/completion/filesystem.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/completion/fuzzy_completer.py` & `prot-3.8.6/src/prot/prompt/completion/fuzzy_completer.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/completion/nested.py` & `prot-3.8.6/src/prot/prompt/completion/nested.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/completion/word_completer.py` & `prot-3.8.6/src/prot/prompt/completion/word_completer.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/contrib/completers/system.py` & `prot-3.8.6/src/prot/prompt/contrib/completers/system.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/contrib/regular_languages/__init__.py` & `prot-3.8.6/src/prot/prompt/contrib/regular_languages/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/contrib/regular_languages/compiler.py` & `prot-3.8.6/src/prot/prompt/contrib/regular_languages/compiler.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/contrib/regular_languages/completion.py` & `prot-3.8.6/src/prot/prompt/contrib/regular_languages/completion.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/contrib/regular_languages/lexer.py` & `prot-3.8.6/src/prot/prompt/contrib/regular_languages/lexer.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/contrib/regular_languages/regex_parser.py` & `prot-3.8.6/src/prot/prompt/contrib/regular_languages/regex_parser.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/contrib/regular_languages/validation.py` & `prot-3.8.6/src/prot/prompt/contrib/regular_languages/validation.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/contrib/ssh/server.py` & `prot-3.8.6/src/prot/prompt/contrib/ssh/server.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/contrib/telnet/protocol.py` & `prot-3.8.6/src/prot/prompt/contrib/telnet/protocol.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/contrib/telnet/server.py` & `prot-3.8.6/src/prot/prompt/contrib/telnet/server.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/document.py` & `prot-3.8.6/src/prot/prompt/document.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/eventloop/__init__.py` & `prot-3.8.6/src/prot/prompt/eventloop/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/eventloop/async_context_manager.py` & `prot-3.8.6/src/prot/prompt/eventloop/async_context_manager.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/eventloop/async_generator.py` & `prot-3.8.6/src/prot/prompt/eventloop/async_generator.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/eventloop/dummy_contextvars.py` & `prot-3.8.6/src/prot/prompt/eventloop/dummy_contextvars.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/eventloop/inputhook.py` & `prot-3.8.6/src/prot/prompt/eventloop/inputhook.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/eventloop/utils.py` & `prot-3.8.6/src/prot/prompt/eventloop/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/eventloop/win32.py` & `prot-3.8.6/src/prot/prompt/eventloop/win32.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/filters/__init__.py` & `prot-3.8.6/src/prot/prompt/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/filters/app.py` & `prot-3.8.6/src/prot/prompt/filters/app.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/filters/base.py` & `prot-3.8.6/src/prot/prompt/filters/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/filters/cli.py` & `prot-3.8.6/src/prot/prompt/filters/cli.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/filters/utils.py` & `prot-3.8.6/src/prot/prompt/filters/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/formatted_text/__init__.py` & `prot-3.8.6/src/prot/prompt/formatted_text/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/formatted_text/ansi.py` & `prot-3.8.6/src/prot/prompt/formatted_text/ansi.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/formatted_text/base.py` & `prot-3.8.6/src/prot/prompt/formatted_text/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/formatted_text/html.py` & `prot-3.8.6/src/prot/prompt/formatted_text/html.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/formatted_text/pygments.py` & `prot-3.8.6/src/prot/prompt/formatted_text/pygments.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/formatted_text/utils.py` & `prot-3.8.6/src/prot/prompt/formatted_text/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/history.py` & `prot-3.8.6/src/prot/prompt/history.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/input/ansi_escape_sequences.py` & `prot-3.8.6/src/prot/prompt/input/ansi_escape_sequences.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/input/base.py` & `prot-3.8.6/src/prot/prompt/input/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/input/defaults.py` & `prot-3.8.6/src/prot/prompt/input/defaults.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/input/posix_pipe.py` & `prot-3.8.6/src/prot/prompt/input/posix_pipe.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/input/posix_utils.py` & `prot-3.8.6/src/prot/prompt/input/posix_utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/input/typeahead.py` & `prot-3.8.6/src/prot/prompt/input/typeahead.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/input/vt100.py` & `prot-3.8.6/src/prot/prompt/input/vt100.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/input/vt100_parser.py` & `prot-3.8.6/src/prot/prompt/input/vt100_parser.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/input/win32.py` & `prot-3.8.6/src/prot/prompt/input/win32.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/input/win32_pipe.py` & `prot-3.8.6/src/prot/prompt/input/win32_pipe.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/bindings/auto_suggest.py` & `prot-3.8.6/src/prot/prompt/key_binding/bindings/auto_suggest.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/bindings/basic.py` & `prot-3.8.6/src/prot/prompt/key_binding/bindings/basic.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/bindings/completion.py` & `prot-3.8.6/src/prot/prompt/key_binding/bindings/completion.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/bindings/cpr.py` & `prot-3.8.6/src/prot/prompt/key_binding/bindings/cpr.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/bindings/emacs.py` & `prot-3.8.6/src/prot/prompt/key_binding/bindings/emacs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/bindings/mouse.py` & `prot-3.8.6/src/prot/prompt/key_binding/bindings/mouse.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/bindings/named_commands.py` & `prot-3.8.6/src/prot/prompt/key_binding/bindings/named_commands.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/bindings/open_in_editor.py` & `prot-3.8.6/src/prot/prompt/key_binding/bindings/open_in_editor.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/bindings/page_navigation.py` & `prot-3.8.6/src/prot/prompt/key_binding/bindings/page_navigation.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/bindings/scroll.py` & `prot-3.8.6/src/prot/prompt/key_binding/bindings/scroll.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/bindings/search.py` & `prot-3.8.6/src/prot/prompt/key_binding/bindings/search.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/bindings/vi.py` & `prot-3.8.6/src/prot/prompt/key_binding/bindings/vi.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/defaults.py` & `prot-3.8.6/src/prot/prompt/key_binding/defaults.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/digraphs.py` & `prot-3.8.6/src/prot/prompt/key_binding/digraphs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/emacs_state.py` & `prot-3.8.6/src/prot/prompt/key_binding/emacs_state.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/key_bindings.py` & `prot-3.8.6/src/prot/prompt/key_binding/key_bindings.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/key_processor.py` & `prot-3.8.6/src/prot/prompt/key_binding/key_processor.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/key_binding/vi_state.py` & `prot-3.8.6/src/prot/prompt/key_binding/vi_state.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/keys.py` & `prot-3.8.6/src/prot/prompt/keys.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/layout/__init__.py` & `prot-3.8.6/src/prot/prompt/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/layout/containers.py` & `prot-3.8.6/src/prot/prompt/layout/containers.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/layout/controls.py` & `prot-3.8.6/src/prot/prompt/layout/controls.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/layout/dimension.py` & `prot-3.8.6/src/prot/prompt/layout/dimension.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/layout/dummy.py` & `prot-3.8.6/src/prot/prompt/layout/dummy.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/layout/layout.py` & `prot-3.8.6/src/prot/prompt/layout/layout.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/layout/margins.py` & `prot-3.8.6/src/prot/prompt/layout/margins.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/layout/menus.py` & `prot-3.8.6/src/prot/prompt/layout/menus.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/layout/mouse_handlers.py` & `prot-3.8.6/src/prot/prompt/layout/mouse_handlers.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/layout/processors.py` & `prot-3.8.6/src/prot/prompt/layout/processors.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/layout/screen.py` & `prot-3.8.6/src/prot/prompt/layout/screen.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/layout/utils.py` & `prot-3.8.6/src/prot/prompt/layout/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/lexers/base.py` & `prot-3.8.6/src/prot/prompt/lexers/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/lexers/pygments.py` & `prot-3.8.6/src/prot/prompt/lexers/pygments.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/mouse_events.py` & `prot-3.8.6/src/prot/prompt/mouse_events.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/output/base.py` & `prot-3.8.6/src/prot/prompt/output/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/output/color_depth.py` & `prot-3.8.6/src/prot/prompt/output/color_depth.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/output/conemu.py` & `prot-3.8.6/src/prot/prompt/output/conemu.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/output/defaults.py` & `prot-3.8.6/src/prot/prompt/output/defaults.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/output/vt100.py` & `prot-3.8.6/src/prot/prompt/output/vt100.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/output/win32.py` & `prot-3.8.6/src/prot/prompt/output/win32.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/output/windows10.py` & `prot-3.8.6/src/prot/prompt/output/windows10.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/patch_stdout.py` & `prot-3.8.6/src/prot/prompt/patch_stdout.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/renderer.py` & `prot-3.8.6/src/prot/prompt/renderer.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/search.py` & `prot-3.8.6/src/prot/prompt/search.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/selection.py` & `prot-3.8.6/src/prot/prompt/selection.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/shortcuts/__init__.py` & `prot-3.8.6/src/prot/prompt/shortcuts/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/shortcuts/dialogs.py` & `prot-3.8.6/src/prot/prompt/shortcuts/dialogs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/shortcuts/progress_bar/base.py` & `prot-3.8.6/src/prot/prompt/shortcuts/progress_bar/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/shortcuts/progress_bar/formatters.py` & `prot-3.8.6/src/prot/prompt/shortcuts/progress_bar/formatters.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/shortcuts/prompt.py` & `prot-3.8.6/src/prot/prompt/shortcuts/prompt.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/shortcuts/utils.py` & `prot-3.8.6/src/prot/prompt/shortcuts/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/styles/__init__.py` & `prot-3.8.6/src/prot/prompt/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/styles/base.py` & `prot-3.8.6/src/prot/prompt/styles/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/styles/defaults.py` & `prot-3.8.6/src/prot/prompt/styles/defaults.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/styles/named_colors.py` & `prot-3.8.6/src/prot/prompt/styles/named_colors.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/styles/pygments.py` & `prot-3.8.6/src/prot/prompt/styles/pygments.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/styles/style.py` & `prot-3.8.6/src/prot/prompt/styles/style.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/styles/style_transformation.py` & `prot-3.8.6/src/prot/prompt/styles/style_transformation.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/utils.py` & `prot-3.8.6/src/prot/prompt/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/validation.py` & `prot-3.8.6/src/prot/prompt/validation.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/widgets/__init__.py` & `prot-3.8.6/src/prot/prompt/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/widgets/base.py` & `prot-3.8.6/src/prot/prompt/widgets/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/widgets/dialogs.py` & `prot-3.8.6/src/prot/prompt/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/widgets/menus.py` & `prot-3.8.6/src/prot/prompt/widgets/menus.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/widgets/toolbars.py` & `prot-3.8.6/src/prot/prompt/widgets/toolbars.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/prompt/win32_types.py` & `prot-3.8.6/src/prot/prompt/win32_types.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/wcwidth/table_wide.py` & `prot-3.8.6/src/prot/wcwidth/table_wide.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/wcwidth/table_zero.py` & `prot-3.8.6/src/prot/wcwidth/table_zero.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/wcwidth/tests/test_core.py` & `prot-3.8.6/src/prot/wcwidth/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot/wcwidth/wcwidth.py` & `prot-3.8.6/src/prot/wcwidth/wcwidth.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.5/src/prot.egg-info/SOURCES.txt` & `prot-3.8.6/src/prot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

