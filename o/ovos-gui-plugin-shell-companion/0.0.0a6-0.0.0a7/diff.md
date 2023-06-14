# Comparing `tmp/ovos-gui-plugin-shell-companion-0.0.0a6.tar.gz` & `tmp/ovos-gui-plugin-shell-companion-0.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-gui-plugin-shell-companion-0.0.0a6.tar", last modified: Thu Jun  8 22:45:18 2023, max compression
+gzip compressed data, was "ovos-gui-plugin-shell-companion-0.0.0a7.tar", last modified: Wed Jun 14 01:20:53 2023, max compression
```

## Comparing `ovos-gui-plugin-shell-companion-0.0.0a6.tar` & `ovos-gui-plugin-shell-companion-0.0.0a7.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:45:18.801666 ovos-gui-plugin-shell-companion-0.0.0a6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-08 22:45:18.801666 ovos-gui-plugin-shell-companion-0.0.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:45:18.777666 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/color_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/cui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/descriptions.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:45:18.773666 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:45:18.777666 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/snd/
--rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/snd/clicked.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:45:18.781666 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_HtmlFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:45:18.785666 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:45:18.785666 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/code/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:45:18.785666 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    24264 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:45:18.785666 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/NameSelect.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    20307 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:45:18.789666 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3790 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    26181 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:45:18.801666 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts
--rwxr-xr-x   0 runner    (1001) docker     (123)     1969 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/wigets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:45:18.777666 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-08 22:45:18.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-06-08 22:45:18.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:45:18.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 22:45:18.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 22:45:18.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 22:45:18.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:45:18.000000 ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:45:18.801666 ovos-gui-plugin-shell-companion-0.0.0a6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2949 2023-06-08 22:45:17.000000 ovos-gui-plugin-shell-companion-0.0.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.894629 ovos-gui-plugin-shell-companion-0.0.0a7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-14 01:20:53.894629 ovos-gui-plugin-shell-companion-0.0.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.882629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/
+-rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/color_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/cui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/descriptions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.874629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.882629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_HtmlFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.886629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.886629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.886629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.886629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/NameSelect.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    20289 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    10909 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.886629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3790 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    26178 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.886629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/snd/
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/snd/clicked.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.894629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1969 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/wigets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.882629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:20:53.894629 ovos-gui-plugin-shell-companion-0.0.0a7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2949 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/setup.py
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/LICENSE` & `ovos-gui-plugin-shell-companion-0.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/PKG-INFO` & `ovos-gui-plugin-shell-companion-0.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-gui-plugin-shell-companion
-Version: 0.0.0a6
+Version: 0.0.0a7
 Summary: GUI plugin for ovos-shell
 Home-page: https://github.com/OpenVoiceOS/ovos-gui-plugin-shell-companion
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/README.md` & `ovos-gui-plugin-shell-companion-0.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/__init__.py` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,19 @@
     def __init__(self, config: dict, bus: MessageBusClient = None,
                  gui: GUIInterface = None,
                  preload_gui=False, permanent=True):
         config["homescreen_supported"] = True
         res_dir = join(dirname(__file__), "res")
         gui = gui or GUIInterface("ovos_gui_plugin_shell_companion",
                                   bus=bus, config=Configuration(),
-                                  resource_dir=res_dir)
-        if not gui.resource_dir:
-            LOG.info(f"Setting default GUI resource directory to: {res_dir}")
-            gui.resource_dir = res_dir
+                                  ui_directories={"qt5": join(res_dir, "ui"),
+                                                  "qt6": join(res_dir, "ui6")})
+        if not gui.ui_directories:
+            LOG.info(f"Setting default qt5 resource directory to: {res_dir}")
+            gui.ui_directories["qt5"] = res_dir
         LOG.info("OVOS Shell: Initializing")
         super().__init__(config=config, bus=bus, gui=gui,
                          preload_gui=preload_gui, permanent=permanent)
         self.local_display_config = get_ovos_shell_config()
         self.about_page_data = []
         self.build_initial_about_page_data()
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/brightness.py` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/brightness.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/color_manager.py` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/color_manager.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/config.py` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/config.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/cui.py` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/cui.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/descriptions.json` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/descriptions.json`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/snd/clicked.wav` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/snd/clicked.wav`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml`

 * *Files 0% similar despite different names*

```diff
@@ -174,14 +174,14 @@
             color: darkMode ? themeViewer.viewTextColor : themeViewer.viewPrimaryColor
             elide: Text.ElideRight
         }
     }
 
     onClicked: {
         if(clickEnabled){
-            Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+            Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
             styleViewPopUp.setTheme(modelDataStyle)
             styleViewPopUp.close()
             Mycroft.MycroftController.sendRequest("ovos.theme.get", {})
         }
     }
 }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
                     Layout.preferredHeight: Kirigami.Units.gridUnit * 2
                 }
             }
 
             MouseArea {
                 anchors.fill: parent
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     Mycroft.MycroftController.sendRequest("ovos.phal.configuration.provider.list.groups", {})
                 }
             }
         }
 
         Item {
             anchors.top: areaSep.bottom
@@ -327,15 +327,15 @@
                     }
                 }
             }
 
             MouseArea {
                 anchors.fill: parent
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     Mycroft.MycroftController.sendRequest("ovos.phal.configuration.provider.set", {"configuration": configurationLoaderView.updateFieldList, "group_name": configurationLoaderView.groupName})
                     Mycroft.MycroftController.sendRequest("ovos.phal.configuration.provider.list.groups", {})
                 }
             }
         }
     }
 }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
                             color: Kirigami.Theme.textColor
                             level: 2
                         }
                     }
                 }
 
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     Mycroft.MycroftController.sendRequest("ovos.phal.configuration.provider.get", {"group": modelData})
                 }
             }
         }
     }
 
     Item {
@@ -171,13 +171,13 @@
                 Layout.preferredHeight: Kirigami.Units.gridUnit * 2
             }
         }
 
         MouseArea {
             anchors.fill: parent
             onClicked: {
-                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                 triggerGuiEvent("mycroft.device.settings.developer", {})
             }
         }
     }
 }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
                         text: modelData.name
                         color: modelData.textColor
                         elide: Text.ElideRight
                     }
                 }
 
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     styleViewPopUp.showView(modelData.name, modelData.path, modelData.primaryColor, modelData.secondaryColor, modelData.textColor)
                 }
             }
         }
     }
 
     Item {
@@ -267,15 +267,15 @@
                     Layout.preferredHeight: Kirigami.Units.gridUnit * 2
                 }
             }
 
             MouseArea {
                 anchors.fill: parent
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     triggerGuiEvent("mycroft.device.settings", {})
                 }
             }
         }
 
         Item {
             anchors.top: areaSep.bottom
@@ -312,15 +312,15 @@
                     }
                 }
             }
 
             MouseArea {
                 anchors.fill: parent
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     triggerGuiEvent("mycroft.device.settings.create.theme", {})
                 }
             }
         }
     }
 
     ItemDelegate  {
@@ -477,15 +477,15 @@
                         Layout.preferredHeight: Kirigami.Units.gridUnit * 2
                     }
                 }
 
                 MouseArea {
                     anchors.fill: parent
                     onClicked: {
-                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                         styleViewPopUp.close()
                     }
                 }
             }
         }
     }
 }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                         wrapMode: Text.WordWrap
                         text: qsTr("Select Primary Color")
                     }
 
                     MouseArea {
                         anchors.fill: parent
                         onClicked: {
-                            Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                            Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                             primaryColorSelectorPopup.open()
                         }
                     }
                 }
                 Rectangle {
                     id: secondaryColorSelectButton
                     Layout.fillWidth: true
@@ -183,15 +183,15 @@
                         wrapMode: Text.WordWrap
                         text: qsTr("Select Secondary Color")
                     }
 
                     MouseArea {
                         anchors.fill: parent
                         onClicked: {
-                            Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                            Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                             secondaryColorSelectorPopup.open()
                         }
                     }
                 }
                 Rectangle {
                     id: autoTextColorButton
                     Layout.fillWidth: true
@@ -259,15 +259,15 @@
                         wrapMode: Text.WordWrap
                         text: qsTr("Set Name")
                     }
 
                     MouseArea {
                         anchors.fill: parent
                         onClicked: {
-                            Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                            Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                             setNameBoxPopup.open()
                         }
                     }
                 }
             }
 
             Kirigami.Separator {
@@ -325,15 +325,15 @@
                         Layout.preferredHeight: Kirigami.Units.gridUnit * 2
                     }
                 }
 
                 MouseArea {
                     anchors.fill: parent
                     onClicked: {
-                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                         previewPopUpBox.open()
                     }
                 }
             }
         }
         Item {
             id: themeButtonArea
@@ -381,15 +381,15 @@
                         Layout.preferredHeight: Kirigami.Units.gridUnit * 2
                     }
                 }
 
                 MouseArea {
                     anchors.fill: parent
                     onClicked: {
-                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                         Mycroft.MycroftController.sendRequest("ovos.shell.gui.color.scheme.generate", {"theme_name": createThemeView.selectedThemeName, "primaryColor": createThemeView.selectedPrimaryColor, "secondaryColor": createThemeView.selectedSecondaryColor, "textColor": createThemeView.selectedTextColor})
                         visualBusyIndicatorBox.visible = true
                         visualBusyIndicatorBox.enabled = true
                         timeoutMessageTimer.start()
                     }
                 }
             }
@@ -442,15 +442,15 @@
                 Layout.preferredHeight: Kirigami.Units.gridUnit * 2
             }
         }
 
         MouseArea {
             anchors.fill: parent
             onClicked: {
-                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                 triggerGuiEvent("mycroft.device.settings.customize", {})
             }
         }
     }
 
     ItemDelegate  {
         id: previewPopUpBox
@@ -589,15 +589,15 @@
                         Layout.preferredHeight: Kirigami.Units.gridUnit * 2
                     }
                 }
 
                 MouseArea {
                     anchors.fill: parent
                     onClicked: {
-                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                         previewPopUpBox.close()
                     }
                 }
             }
         }
     }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                     Layout.preferredHeight: Kirigami.Units.gridUnit * 2
                 }
             }
 
             MouseArea {
                 anchors.fill: parent
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
                     colorSelectPrimaryBox.close()
                 }
             }
         }
     }
 }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
                     Layout.preferredHeight: Kirigami.Units.gridUnit * 2
                 }
             }
 
             MouseArea {
                 anchors.fill: parent
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
                     colorSelectSecondaryBox.close()
                 }
             }
         }
     }
 }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     property color selected_border_color : Kirigami.Theme.highlightColor
     Layout.fillWidth: true
     Layout.fillHeight: true
     checkable: true
 
     onCheckedChanged: {
         if(checked) {
-            Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../../snd/clicked.wav"))
+            Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
         }
     }
 
     background: Rectangle {
         border.color: (checked ? selected_border_color : border_color)
         border.width: 4
         radius: 3
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
                     Layout.preferredHeight: Kirigami.Units.gridUnit * 2
                 }
             }
 
             MouseArea {
                 anchors.fill: parent
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
                     nameSelectBox.close()
                 }
             }
         }
     }
 }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml`

 * *Files 1% similar despite different names*

```diff
@@ -102,28 +102,28 @@
             Button {
                 Layout.fillWidth: true
                 Layout.preferredHeight: Kirigami.Units.gridUnit * 3
                 text: "Enable Dashboard"
                 visible: !dashActive
                 enabled: visible
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     triggerGuiEvent("mycroft.device.enable.dash", {})
                     developerSettingsView.busyVisible = true
                 }
             }
 
             Button {
                 Layout.fillWidth: true
                 Layout.preferredHeight: Kirigami.Units.gridUnit * 3
                 text: "Disable Dashboard"
                 visible: dashActive
                 enabled: visible
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     triggerGuiEvent("mycroft.device.disable.dash", {})
                     developerSettingsView.busyVisible = true
                 }
             }
 
             Kirigami.Separator {
                 Layout.fillWidth: true
@@ -216,15 +216,15 @@
                     textFormat: Text.PlainText
                     color: Kirigami.Theme.textColor
                     level: 2
                 }
             }
 
             onClicked: {
-                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                 Mycroft.MycroftController.sendRequest("ovos.phal.configuration.provider.list.groups", {})
             }
 
             onPressed: {
                 advancedSettingButtonBg.color = Qt.rgba(Kirigami.Theme.highlightColor.r, Kirigami.Theme.highlightColor.g, Kirigami.Theme.highlightColor.b, 0.4)
             }
             onReleased: {
@@ -276,13 +276,13 @@
                 Layout.preferredHeight: Kirigami.Units.gridUnit * 2
             }
         }
 
         MouseArea {
             anchors.fill: parent
             onClicked: {
-                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                 triggerGuiEvent("mycroft.device.settings", {})
             }
         }
     }
 }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
                         anchors.rightMargin: 8
                         height: Kirigami.Units.iconSizes.medium
                         width: Kirigami.Units.iconSizes.medium
                     }
 
                     onClicked: {
                         console.log(autoWallpaperRotationSwitch.checked)
-                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                         triggerGuiEvent("speaker.extension.display.set.wallpaper.rotation", {"wallpaper_rotation": autoWallpaperRotationSwitch.checked})
                     }
                 }
             }
 
             Rectangle {
                 Layout.fillWidth: true
@@ -224,15 +224,15 @@
                         anchors.rightMargin: 8
                         height: Kirigami.Units.iconSizes.medium
                         width: Kirigami.Units.iconSizes.medium
                     }
 
                     onClicked: {
                         console.log(autoDimSwitch.checked)
-                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                         triggerGuiEvent("speaker.extension.display.set.auto.dim", {"auto_dim": autoDimSwitch.checked})
                     }
                 }
             }
 
             Rectangle {
                 Layout.fillWidth: true
@@ -292,15 +292,15 @@
                         anchors.rightMargin: 8
                         height: Kirigami.Units.iconSizes.medium
                         width: Kirigami.Units.iconSizes.medium
                     }
 
                     onClicked: {
                         console.log(autoNightmodeSwitch.checked)
-                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                         triggerGuiEvent("speaker.extension.display.set.auto.nightmode", {"auto_nightmode": autoNightmodeSwitch.checked})
                     }
                 }
             }
 
             Rectangle {
                 Layout.fillWidth: true
@@ -360,15 +360,15 @@
                         anchors.rightMargin: 8
                         height: Kirigami.Units.iconSizes.medium
                         width: Kirigami.Units.iconSizes.medium
                     }
 
                     onClicked: {
                         console.log(displayMenuLabelsSwitch.checked)
-                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                        Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                         Mycroft.MycroftController.sendRequest("ovos.shell.set.menuLabels", {"enabled": displayMenuLabelsSwitch.checked})
                     }
                 }
             }
         }
     }
 
@@ -424,15 +424,15 @@
                     textFormat: Text.PlainText
                     color: Kirigami.Theme.textColor
                     level: 2
                 }
             }
 
             onClicked: {
-                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                 console.log("Sending Show Wallpaper Page Here")
                 triggerGuiEvent("mycroft.device.settings.wallpapers", {})
             }
 
             onPressed: {
                 wallpaperSettingButtonBg.color = Qt.rgba(Kirigami.Theme.highlightColor.r, Kirigami.Theme.highlightColor.g, Kirigami.Theme.highlightColor.b, 0.4)
             }
@@ -486,12 +486,12 @@
             }
         }
 
         MouseArea {
             anchors.fill: parent
             onClicked: {
                 triggerGuiEvent("mycroft.device.settings", {})
-                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
             }
         }
     }
 }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                     horizontalAlignment: Text.AlignHCenter
                     verticalAlignment: Text.AlignVCenter
                     text: qsTr("Wipe Cache")
                     color: Kirigami.Theme.textColor
                 }
                 
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     Mycroft.MycroftController.sendRequest("system.factory.reset", {"wipe_cache": true, "wipe_data": false, "wipe_logs": false, "wipe_config": false, "reset_hardware": false})
                 }
 
                 onPressed: {
                     opacity = 0.5
                 }
                 onReleased: {
@@ -121,15 +121,15 @@
                     horizontalAlignment: Text.AlignHCenter
                     verticalAlignment: Text.AlignVCenter
                     text: qsTr("Wipe Config")
                     color: Kirigami.Theme.textColor
                 }
 
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     Mycroft.MycroftController.sendRequest("system.factory.reset", {"wipe_cache": false, "wipe_data": false, "wipe_logs": false, "wipe_config": true, "reset_hardware": false})
                 }
 
                 onPressed: {
                     opacity = 0.5
                 }
                 onReleased: {
@@ -156,15 +156,15 @@
                     horizontalAlignment: Text.AlignHCenter
                     verticalAlignment: Text.AlignVCenter
                     text: qsTr("Wipe Data")
                     color: Kirigami.Theme.textColor
                 }
 
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     Mycroft.MycroftController.sendRequest("system.factory.reset", {"wipe_cache": false, "wipe_data": true, "wipe_logs": false, "wipe_config": false, "reset_hardware": false})
                 }
 
                 onPressed: {
                     opacity = 0.5
                 }
                 onReleased: {
@@ -190,15 +190,15 @@
                     horizontalAlignment: Text.AlignHCenter
                     verticalAlignment: Text.AlignVCenter
                     text: qsTr("Wipe Logs")
                     color: Kirigami.Theme.textColor
                 }
 
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     Mycroft.MycroftController.sendRequest("system.factory.reset", {"wipe_cache": false, "wipe_data": false, "wipe_logs": true, "wipe_config": false, "reset_hardware": false})
                 }
 
                 onPressed: {
                     opacity = 0.5
                 }
                 onReleased: {
@@ -225,15 +225,15 @@
                     horizontalAlignment: Text.AlignHCenter
                     verticalAlignment: Text.AlignVCenter
                     text: qsTr("Factory Reset")
                     color: Kirigami.Theme.textColor
                 }
 
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     Mycroft.MycroftController.sendRequest("system.factory.reset", {"wipe_cache": true, "wipe_data": true, "wipe_logs": true, "wipe_config": true, "reset_hardware": true})
                 }
 
                 onPressed: {
                     opacity = 0.5
                 }
                 onReleased: {
@@ -286,13 +286,13 @@
                 Layout.preferredHeight: Kirigami.Units.gridUnit * 2
             }
         }
 
         MouseArea {
             anchors.fill: parent
             onClicked: {
-                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                 triggerGuiEvent("mycroft.device.settings", {})
             }
         }
     }
 }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                                 source: "images/tick.svg"
                             }
                         }
                     }
                 }
 
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     triggerGuiEvent("mycroft.device.set.idle", {"selected": modelData.id})
                 }
             }
 
             Component.onCompleted: {
                 listIdleFaces.count
             }
@@ -173,13 +173,13 @@
                 Layout.preferredHeight: Kirigami.Units.gridUnit * 2
             }
         }
 
         MouseArea {
             anchors.fill: parent
             onClicked: {
-                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                 triggerGuiEvent("mycroft.device.settings", {})
             }
         }
     }
 }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                                 level: 2
                             }
                         }
                     }
                 }
 
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     triggerGuiEvent(model.settingEvent, {})
                 }
             }
         }
     }
 
     Item {
@@ -190,13 +190,13 @@
                 Layout.preferredHeight: Kirigami.Units.gridUnit * 2
             }
         }
 
         MouseArea {
             anchors.fill: parent
             onClicked: {
-                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                 triggerGuiEvent("mycroft.device.show.idle", {})
             }
         }
     }
 }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml`

 * *Files 1% similar despite different names*

```diff
@@ -73,25 +73,25 @@
             }
 
             Button {
                 Layout.fillWidth: true
                 Layout.preferredHeight: Kirigami.Units.gridUnit * 3
                 text: qsTr("Enable SSH")
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     Mycroft.MycroftController.sendRequest("system.ssh.enable", {"display": false})
                 }
             }
 
             Button {
                 Layout.fillWidth: true
                 Layout.preferredHeight: Kirigami.Units.gridUnit * 3
                 text: qsTr("Disable SSH")
                 onClicked: {
-                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                     Mycroft.MycroftController.sendRequest("system.ssh.disable", {"display": false})
                 }
             }
         }
     }
 
     Item {
@@ -137,13 +137,13 @@
                 Layout.preferredHeight: Kirigami.Units.gridUnit * 2
             }
         }
 
         MouseArea {
             anchors.fill: parent
             onClicked: {
-                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
                 triggerGuiEvent("mycroft.device.settings", {})
             }
         }
     }
 }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,15 @@
             }
         }
 
         MouseArea {
             anchors.fill: parent
             onClicked: {
                 triggerGuiEvent("mycroft.device.settings", {})
-                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../../snd/clicked.wav"))
+                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
             }
         }
     }
 
     ItemDelegate {
         id: setWallpaperPopupDialog
         width: wallpaperSettings.width
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion/wigets.py` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/wigets.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-gui-plugin-shell-companion
-Version: 0.0.0a6
+Version: 0.0.0a7
 Summary: GUI plugin for ovos-shell
 Home-page: https://github.com/OpenVoiceOS/ovos-gui-plugin-shell-companion
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt` & `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 ovos_gui_plugin_shell_companion.egg-info/PKG-INFO
 ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt
 ovos_gui_plugin_shell_companion.egg-info/dependency_links.txt
 ovos_gui_plugin_shell_companion.egg-info/entry_points.txt
 ovos_gui_plugin_shell_companion.egg-info/requires.txt
 ovos_gui_plugin_shell_companion.egg-info/top_level.txt
 ovos_gui_plugin_shell_companion.egg-info/zip-safe
-ovos_gui_plugin_shell_companion/res/snd/clicked.wav
 ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml
 ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml
 ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml
 ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml
 ovos_gui_plugin_shell_companion/res/ui/SYSTEM_HtmlFrame.qml
 ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml
 ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml
@@ -65,14 +64,15 @@
 ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg
 ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg
 ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png
 ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg
 ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg
 ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg
 ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg
+ovos_gui_plugin_shell_companion/res/ui/snd/clicked.wav
 ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm
 ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm
 ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm
 ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm
 ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm
 ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm
 ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a6/setup.py` & `ovos-gui-plugin-shell-companion-0.0.0a7/setup.py`

 * *Files identical despite different names*

