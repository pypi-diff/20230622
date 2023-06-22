# Comparing `tmp/ovos-gui-plugin-shell-companion-0.0.0a7.tar.gz` & `tmp/ovos-gui-plugin-shell-companion-0.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-gui-plugin-shell-companion-0.0.0a7.tar", last modified: Wed Jun 14 01:20:53 2023, max compression
+gzip compressed data, was "ovos-gui-plugin-shell-companion-0.0.0a8.tar", last modified: Wed Jun 21 14:59:01 2023, max compression
```

## Comparing `ovos-gui-plugin-shell-companion-0.0.0a7.tar` & `ovos-gui-plugin-shell-companion-0.0.0a8.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.894629 ovos-gui-plugin-shell-companion-0.0.0a7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-14 01:20:53.894629 ovos-gui-plugin-shell-companion-0.0.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.882629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/
--rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/color_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/cui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/descriptions.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.874629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.882629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_HtmlFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.886629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.886629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/code/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js
--rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.886629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.886629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/NameSelect.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    20289 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    10909 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.886629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3790 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    26178 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.886629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/snd/
--rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/snd/clicked.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.894629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts
--rwxr-xr-x   0 runner    (1001) docker     (123)     1969 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/wigets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:20:53.882629 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:20:53.894629 ovos-gui-plugin-shell-companion-0.0.0a7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2949 2023-06-14 01:20:53.000000 ovos-gui-plugin-shell-companion-0.0.0a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.140413 ovos-gui-plugin-shell-companion-0.0.0a8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-21 14:59:01.136413 ovos-gui-plugin-shell-companion-0.0.0a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.116413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/
+-rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/color_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/cui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/descriptions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.116413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.120413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_HtmlFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.124413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.124413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.124413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.124413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/NameSelect.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    20289 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    10909 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.128413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3790 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    26178 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.128413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/snd/
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/snd/clicked.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.136413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1969 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/wigets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.120413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:59:01.140413 ovos-gui-plugin-shell-companion-0.0.0a8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2949 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/setup.py
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/LICENSE` & `ovos-gui-plugin-shell-companion-0.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/PKG-INFO` & `ovos-gui-plugin-shell-companion-0.0.0a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-gui-plugin-shell-companion
-Version: 0.0.0a7
+Version: 0.0.0a8
 Summary: GUI plugin for ovos-shell
 Home-page: https://github.com/OpenVoiceOS/ovos-gui-plugin-shell-companion
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/README.md` & `ovos-gui-plugin-shell-companion-0.0.0a8/README.md`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/__init__.py` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/brightness.py` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/brightness.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/color_manager.py` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/color_manager.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/config.py` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/config.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/cui.py` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/cui.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/descriptions.json` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/descriptions.json`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright 2018 Aditya Mehra <aix.m@outlook.com>
+ * Copyright 2022 Aditya Mehra <aix.m@outlook.com>
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *    http://www.apache.org/licenses/LICENSE-2.0
  *
@@ -12,227 +12,237 @@
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
 import QtQuick.Layouts 1.4
-import QtQuick 2.4
-import QtQuick.Controls 2.0
-import org.kde.kirigami 2.5 as Kirigami
+import QtQuick 2.12
+import QtQuick.Controls 2.11
+import org.kde.kirigami 2.11 as Kirigami
 import Mycroft 1.0 as Mycroft
-import QtGraphicalEffects 1.12
+import OVOSPlugin 1.0 as OVOSPlugin
+import QtGraphicalEffects 1.0
 
 Item {
-    id: developerSettingsView
+    id: factorySettingsView
     anchors.fill: parent
-    property bool dashActive: sessionData.dashboard_enabled ? Boolean(sessionData.dashboard_enabled) : false
-    property bool busyVisible: false
-
-    onDashActiveChanged: {
-        developerSettingsView.busyVisible = false
-    }
+    property bool horizontalMode: width > height ? 1 :0
 
     Item {
         id: topArea
         anchors.left: parent.left
         anchors.right: parent.right
         anchors.top: parent.top
         height: Kirigami.Units.gridUnit * 2
 
         Kirigami.Heading {
-            id: brightnessSettingPageTextHeading
+            id: idleSettingPageTextHeading
             level: 1
             wrapMode: Text.WordWrap
             anchors.centerIn: parent
             font.bold: true
-            text: "Developer Settings"
+            text: qsTr("Factory Reset Settings")
             color: Kirigami.Theme.textColor
         }
     }
 
-    Item {
-        id: viewBusyOverlay
-        z: 300
-        anchors.top: topArea.bottom
-        anchors.left: parent.left
-        anchors.right: parent.right
-        anchors.bottom: bottomArea.top
-        visible: developerSettingsView.busyVisible
-        enabled: visible
-
-        BusyIndicator {
-            id: viewBusyIndicator
-            visible: viewBusyOverlay.visible
-            anchors.centerIn: parent
-            running: viewBusyOverlay.visible
-            enabled: viewBusyOverlay.visible
-        }
-    }
-
     Flickable {
         anchors.top: topArea.bottom
         anchors.topMargin: Kirigami.Units.largeSpacing
         anchors.left: parent.left
         anchors.right: parent.right
-        anchors.bottom: midBottomArea.top
+        anchors.bottom: bottomArea.top
         contentWidth: width
-        contentHeight: colMiddleContents.implicitHeight
+        contentHeight: factorySettingsLayout.implicitHeight
+        ScrollBar.vertical: ScrollBar {
+            width: Mycroft.Units.gridUnit
+            anchors.right: parent.right
+        }
         clip: true
 
-        ColumnLayout {
-            id: colMiddleContents
-            anchors.left: parent.left
-            anchors.right: parent.right
-            spacing: Kirigami.Units.smallSpacing
+        GridLayout {
+            id: factorySettingsLayout
+            width: parent.width - Mycroft.Units.gridUnit * 2
+            anchors.horizontalCenter: parent.horizontalCenter
+            columns: horizontalMode ? 2 : 1
+            columnSpacing: Mycroft.Units.gridUnit / 2
+            rowSpacing: Mycroft.Units.gridUnit / 2
 
-            Kirigami.Heading {
-                id: warnText
-                level: 3
+            Button {
+                text: qsTr("Wipe Cache")
+                Layout.alignment: Qt.AlignHCenter
                 Layout.fillWidth: true
-                wrapMode: Text.WordWrap
-                color: Kirigami.Theme.textColor
-                text: "Enabling OVOS Dashboard will provide you access to control various services on this device, the OVOS Dashboard can be accessed on any device located in your LAN network"
-            }
+                Layout.preferredHeight: Kirigami.Units.gridUnit * 4
+                
+                background: Rectangle {
+                    Kirigami.Theme.inherit: false
+                    Kirigami.Theme.colorSet: Kirigami.Theme.Button
+                    color: Kirigami.Theme.backgroundColor
+                    border.width: 1
+                    border.color: Qt.rgba(Kirigami.Theme.textColor.r, Kirigami.Theme.textColor.g, Kirigami.Theme.textColor.b, 0.5)
+                    radius: 6
+                }
 
-            Item {
-                Layout.fillWidth: true
-                Layout.preferredHeight: Kirigami.Units.largeSpacing
+                contentItem: Label {
+                    horizontalAlignment: Text.AlignHCenter
+                    verticalAlignment: Text.AlignVCenter
+                    text: qsTr("Wipe Cache")
+                    color: Kirigami.Theme.textColor
+                }
+                
+                onClicked: {
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
+                    Mycroft.MycroftController.sendRequest("system.factory.reset", {"wipe_cache": true, "wipe_data": false, "wipe_logs": false, "wipe_config": false, "reset_hardware": false})
+                }
+
+                onPressed: {
+                    opacity = 0.5
+                }
+                onReleased: {
+                    opacity = 1
+                }
             }
 
             Button {
+                Layout.alignment: Qt.AlignHCenter
                 Layout.fillWidth: true
-                Layout.preferredHeight: Kirigami.Units.gridUnit * 3
-                text: "Enable Dashboard"
-                visible: !dashActive
-                enabled: visible
+                Layout.preferredHeight: Kirigami.Units.gridUnit * 4
+
+                background: Rectangle {
+                    Kirigami.Theme.inherit: false
+                    Kirigami.Theme.colorSet: Kirigami.Theme.Button
+                    color: Kirigami.Theme.backgroundColor
+                    border.width: 1
+                    border.color: Qt.rgba(Kirigami.Theme.textColor.r, Kirigami.Theme.textColor.g, Kirigami.Theme.textColor.b, 0.5)
+                    radius: 6
+                }
+
+                contentItem: Label {
+                    horizontalAlignment: Text.AlignHCenter
+                    verticalAlignment: Text.AlignVCenter
+                    text: qsTr("Wipe Config")
+                    color: Kirigami.Theme.textColor
+                }
+
                 onClicked: {
                     Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
-                    triggerGuiEvent("mycroft.device.enable.dash", {})
-                    developerSettingsView.busyVisible = true
+                    Mycroft.MycroftController.sendRequest("system.factory.reset", {"wipe_cache": false, "wipe_data": false, "wipe_logs": false, "wipe_config": true, "reset_hardware": false})
+                }
+
+                onPressed: {
+                    opacity = 0.5
+                }
+                onReleased: {
+                    opacity = 1
                 }
             }
 
             Button {
+                Layout.alignment: Qt.AlignHCenter
                 Layout.fillWidth: true
-                Layout.preferredHeight: Kirigami.Units.gridUnit * 3
-                text: "Disable Dashboard"
-                visible: dashActive
-                enabled: visible
+                Layout.preferredHeight: Kirigami.Units.gridUnit * 4
+
+
+                background: Rectangle {
+                    Kirigami.Theme.inherit: false
+                    Kirigami.Theme.colorSet: Kirigami.Theme.Button
+                    color: Kirigami.Theme.backgroundColor
+                    border.width: 1
+                    border.color: Qt.rgba(Kirigami.Theme.textColor.r, Kirigami.Theme.textColor.g, Kirigami.Theme.textColor.b, 0.5)
+                    radius: 6
+                }
+
+                contentItem: Label {
+                    horizontalAlignment: Text.AlignHCenter
+                    verticalAlignment: Text.AlignVCenter
+                    text: qsTr("Wipe Data")
+                    color: Kirigami.Theme.textColor
+                }
+
                 onClicked: {
                     Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
-                    triggerGuiEvent("mycroft.device.disable.dash", {})
-                    developerSettingsView.busyVisible = true
+                    Mycroft.MycroftController.sendRequest("system.factory.reset", {"wipe_cache": false, "wipe_data": true, "wipe_logs": false, "wipe_config": false, "reset_hardware": false})
                 }
-            }
 
-            Kirigami.Separator {
-                Layout.fillWidth: true
-                Layout.preferredHeight: 1
-                visible: dashActive
-                enabled: visible
-            }
-
-            Kirigami.Heading {
-                Layout.fillWidth: true
-                wrapMode: Text.WordWrap
-                level: 3
-                color: Kirigami.Theme.textColor
-                text: "Dashboard Address: " +  sessionData.dashboard_url
-                visible: dashActive
-                enabled: visible
+                onPressed: {
+                    opacity = 0.5
+                }
+                onReleased: {
+                    opacity = 1
+                }
             }
 
-            Kirigami.Heading {
+            Button {
+                Layout.alignment: Qt.AlignHCenter
                 Layout.fillWidth: true
-                wrapMode: Text.WordWrap
-                level: 3
-                color: Kirigami.Theme.textColor
-                text: "Dashboard Username: " + sessionData.dashboard_user
-                visible: dashActive
-                enabled: visible
-            }
+                Layout.preferredHeight: Kirigami.Units.gridUnit * 4
 
-            Kirigami.Heading {
-                Layout.fillWidth: true
-                wrapMode: Text.WordWrap
-                level: 3
-                color: Kirigami.Theme.textColor
-                text: "Dashboard Password: " + sessionData.dashboard_password
-                visible: dashActive
-                enabled: visible
-            }
-        }
-    }
+                background: Rectangle {
+                    Kirigami.Theme.inherit: false
+                    Kirigami.Theme.colorSet: Kirigami.Theme.Button
+                    color: Kirigami.Theme.backgroundColor
+                    border.width: 1
+                    border.color: Qt.rgba(Kirigami.Theme.textColor.r, Kirigami.Theme.textColor.g, Kirigami.Theme.textColor.b, 0.5)
+                    radius: 6
+                }
 
-    Item {
-        id: midBottomArea
-        anchors.left: parent.left
-        anchors.right: parent.right
-        anchors.bottom: bottomArea.top
-        height: Math.max(Mycroft.Units.gridUnit * 5, Kirigami.Units.iconSizes.large)
+                contentItem: Label {
+                    horizontalAlignment: Text.AlignHCenter
+                    verticalAlignment: Text.AlignVCenter
+                    text: qsTr("Wipe Logs")
+                    color: Kirigami.Theme.textColor
+                }
 
-        Kirigami.Separator {
-            anchors.top: parent.top
-            anchors.left: parent.left
-            anchors.right: parent.right
-            height: 1
-        }
+                onClicked: {
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
+                    Mycroft.MycroftController.sendRequest("system.factory.reset", {"wipe_cache": false, "wipe_data": false, "wipe_logs": true, "wipe_config": false, "reset_hardware": false})
+                }
 
-        Button {
-            id: advancedSettingButton
-            width: parent.width
-            height: Math.max(Mycroft.Units.gridUnit * 5, Kirigami.Units.iconSizes.large)
-
-            background: Rectangle {
-                id: advancedSettingButtonBg
-                color: "transparent"
+                onPressed: {
+                    opacity = 0.5
+                }
+                onReleased: {
+                    opacity = 1
+                }
             }
 
-            contentItem: RowLayout {
-                Image {
-                    id: iconAdvancedSettingHolder
-                    Layout.alignment: Qt.AlignVCenter | Qt.AlignLeft
-                    Layout.preferredHeight: Kirigami.Units.iconSizes.medium
-                    Layout.preferredWidth: Kirigami.Units.iconSizes.medium
-                    source: "images/settings.png"
-
-                    ColorOverlay {
-                        anchors.fill: parent
-                        source: iconAdvancedSettingHolder
-                        color: Qt.rgba(Kirigami.Theme.textColor.r, Kirigami.Theme.textColor.g, Kirigami.Theme.textColor.b, 0.7)
-                    }
-                }
+            Button {
+                id: factoryResetButton
+                Layout.alignment: Qt.AlignHCenter
+                Layout.fillWidth: true
+                Layout.preferredHeight: Kirigami.Units.gridUnit * 4
 
+                background: Rectangle {
+                    Kirigami.Theme.inherit: false
+                    Kirigami.Theme.colorSet: Kirigami.Theme.Button
+                    color: Kirigami.Theme.backgroundColor
+                    border.width: 1
+                    border.color: Qt.rgba(Kirigami.Theme.textColor.r, Kirigami.Theme.textColor.g, Kirigami.Theme.textColor.b, 0.5)
+                    radius: 6
+                }
 
-                Kirigami.Heading {
-                    id: connectionNameLabel
-                    Layout.fillWidth: true
-                    Layout.alignment: Qt.AlignHCenter
+                contentItem: Label {
+                    horizontalAlignment: Text.AlignHCenter
                     verticalAlignment: Text.AlignVCenter
-                    height: paintedHeight
-                    elide: Text.ElideRight
-                    font.weight: Font.DemiBold
-                    text: "Advanced Settings"
-                    textFormat: Text.PlainText
+                    text: qsTr("Factory Reset")
                     color: Kirigami.Theme.textColor
-                    level: 2
                 }
-            }
 
-            onClicked: {
-                Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
-                Mycroft.MycroftController.sendRequest("ovos.phal.configuration.provider.list.groups", {})
-            }
+                onClicked: {
+                    Mycroft.SoundEffects.playClickedSound(Qt.resolvedUrl("../snd/clicked.wav"))
+                    Mycroft.MycroftController.sendRequest("system.factory.reset", {"wipe_cache": true, "wipe_data": true, "wipe_logs": true, "wipe_config": true, "reset_hardware": true})
+                }
 
-            onPressed: {
-                advancedSettingButtonBg.color = Qt.rgba(Kirigami.Theme.highlightColor.r, Kirigami.Theme.highlightColor.g, Kirigami.Theme.highlightColor.b, 0.4)
-            }
-            onReleased: {
-                advancedSettingButtonBg.color = "transparent"
+                onPressed: {
+                    opacity = 0.5
+                }
+                onReleased: {
+                    opacity = 1
+                }
             }
         }
     }
 
     Item {
         id: bottomArea
         anchors.left: parent.left
@@ -265,15 +275,15 @@
                 }
             }
 
             Kirigami.Heading {
                 level: 2
                 wrapMode: Text.WordWrap
                 font.bold: true
-                text: "Device Settings"
+                text: qsTr("Device Settings")
                 color: Kirigami.Theme.textColor
                 verticalAlignment: Text.AlignVCenter
                 Layout.fillWidth: true
                 Layout.preferredHeight: Kirigami.Units.gridUnit * 2
             }
         }
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/snd/clicked.wav` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/snd/clicked.wav`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts`

 * *Files 22% similar despite different names*

#### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts`

```diff
@@ -10,38 +10,13 @@
     </message>
     <message>
       <location filename="developer_settings.qml" line="117"/>
       <source>Advanced Settings</source>
       <translation>Erweiterte Einstellungen</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="152"/>
-      <source>Enable Dashboard</source>
-      <translation>Dashboard aktivieren</translation>
-    </message>
-    <message>
-      <location filename="developer_settings.qml" line="165"/>
-      <source>Disable Dashboard</source>
-      <translation>Dashboard deaktivieren</translation>
-    </message>
-    <message>
-      <location filename="developer_settings.qml" line="187"/>
-      <source>Dashboard Address</source>
-      <translation>Dashboard Adresse</translation>
-    </message>
-    <message>
-      <location filename="developer_settings.qml" line="197"/>
-      <source>Dashboard Username</source>
-      <translation>Dashboard Benutzername</translation>
-    </message>
-    <message>
-      <location filename="developer_settings.qml" line="207"/>
-      <source>Dashboard Password</source>
-      <translation>Dashboard Passwort</translation>
-    </message>
-    <message>
       <location filename="developer_settings.qml" line="250"/>
       <source>Device Settings</source>
       <translation>Geräteeinstellungen</translation>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts`

 * *Files 24% similar despite different names*

#### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts`

```diff
@@ -1,47 +1,32 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="es_ES">
+<TS version="2.1" language="fr_FR">
   <context>
-    <name>developer_settings</name>
+    <name>ssh_settings</name>
     <message>
-      <location filename="developer_settings.qml" line="48"/>
-      <source>Developer Settings</source>
-      <translation>Configuración del desarrollador</translation>
+      <location filename="ssh_settings.qml" line="44"/>
+      <source>SSH Settings</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="117"/>
-      <source>Advanced Settings</source>
-      <translation>Ajustes avanzados</translation>
+      <location filename="ssh_settings.qml" line="67"/>
+      <source>By enabling SSH Mode, anyone can access, change or delete anything on this device by connecting to it via another device.</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="152"/>
-      <source>Enable Dashboard</source>
-      <translation>Habilitar panel</translation>
+      <location filename="ssh_settings.qml" line="78"/>
+      <source>Enable SSH</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="165"/>
-      <source>Disable Dashboard</source>
-      <translation>Deshabilitar panel</translation>
+      <location filename="ssh_settings.qml" line="88"/>
+      <source>Disable SSH</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="187"/>
-      <source>Dashboard Address</source>
-      <translation>Dirección del tablero</translation>
-    </message>
-    <message>
-      <location filename="developer_settings.qml" line="197"/>
-      <source>Dashboard Username</source>
-      <translation>Nombre de usuario del panel</translation>
-    </message>
-    <message>
-      <location filename="developer_settings.qml" line="207"/>
-      <source>Dashboard Password</source>
-      <translation>Contraseña del panel</translation>
-    </message>
-    <message>
-      <location filename="developer_settings.qml" line="250"/>
+      <location filename="ssh_settings.qml" line="133"/>
       <source>Device Settings</source>
-      <translation>Configuración de dispositivo</translation>
+      <translation type="unfinished"/>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts`

 * *Files 15% similar despite different names*

#### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts`

```diff
@@ -1,47 +1,47 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="fr_FR">
+<TS version="2.1" language="pt_BR">
   <context>
-    <name>developer_settings</name>
+    <name>settingspage</name>
     <message>
-      <location filename="developer_settings.qml" line="48"/>
-      <source>Developer Settings</source>
-      <translation>Paramètres du développeur</translation>
+      <location filename="settingspage.qml" line="19"/>
+      <source>Homescreen Settings</source>
+      <translation>Configurações da tela inicial</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="117"/>
-      <source>Advanced Settings</source>
-      <translation>Réglages avancés</translation>
+      <location filename="settingspage.qml" line="25"/>
+      <source>Customize</source>
+      <translation>Customizar</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="152"/>
-      <source>Enable Dashboard</source>
-      <translation>Activer le tableau de bord</translation>
+      <location filename="settingspage.qml" line="31"/>
+      <source>Display</source>
+      <translation>Exibição</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="165"/>
-      <source>Disable Dashboard</source>
-      <translation>Désactiver le tableau de bord</translation>
+      <location filename="settingspage.qml" line="37"/>
+      <source>Enable SSH</source>
+      <translation>Ativar SSH</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="187"/>
-      <source>Dashboard Address</source>
-      <translation>Adresse du tableau de bord</translation>
+      <location filename="settingspage.qml" line="43"/>
+      <source>Developer Settings</source>
+      <translation>Configurações do desenvolvedor</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="197"/>
-      <source>Dashboard Username</source>
-      <translation>Nom d'utilisateur du tableau de bord</translation>
+      <location filename="settingspage.qml" line="49"/>
+      <source>About</source>
+      <translation>Sobre</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="207"/>
-      <source>Dashboard Password</source>
-      <translation>Mot de passe du tableau de bord</translation>
+      <location filename="settingspage.qml" line="68"/>
+      <source>Device Settings</source>
+      <translation>Configurações do dispositivo</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="250"/>
-      <source>Device Settings</source>
-      <translation>Réglages de l'appareil</translation>
+      <location filename="settingspage.qml" line="180"/>
+      <source>Home</source>
+      <translation>Casa</translation>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts`

 * *Files 24% similar despite different names*

#### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts`

```diff
@@ -1,47 +1,32 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="it_IT">
+<TS version="2.1" language="nl_NL">
   <context>
-    <name>developer_settings</name>
+    <name>ssh_settings</name>
     <message>
-      <location filename="developer_settings.qml" line="48"/>
-      <source>Developer Settings</source>
-      <translation>Paramètres du développeur</translation>
+      <location filename="ssh_settings.qml" line="44"/>
+      <source>SSH Settings</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="117"/>
-      <source>Advanced Settings</source>
-      <translation>Impostazioni avanzate</translation>
+      <location filename="ssh_settings.qml" line="67"/>
+      <source>By enabling SSH Mode, anyone can access, change or delete anything on this device by connecting to it via another device.</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="152"/>
-      <source>Enable Dashboard</source>
-      <translation>Abilita dashboard</translation>
+      <location filename="ssh_settings.qml" line="78"/>
+      <source>Enable SSH</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="165"/>
-      <source>Disable Dashboard</source>
-      <translation>Disabilita dashboard</translation>
+      <location filename="ssh_settings.qml" line="88"/>
+      <source>Disable SSH</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="187"/>
-      <source>Dashboard Address</source>
-      <translation>Indirizzo dashboard</translation>
-    </message>
-    <message>
-      <location filename="developer_settings.qml" line="197"/>
-      <source>Dashboard Username</source>
-      <translation>Nome utente dashboard</translation>
-    </message>
-    <message>
-      <location filename="developer_settings.qml" line="207"/>
-      <source>Dashboard Password</source>
-      <translation>Password dashboard</translation>
-    </message>
-    <message>
-      <location filename="developer_settings.qml" line="250"/>
+      <location filename="ssh_settings.qml" line="133"/>
       <source>Device Settings</source>
-      <translation>Impostazioni dispositivo</translation>
+      <translation type="unfinished"/>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts`

 * *Files 19% similar despite different names*

#### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts`

```diff
@@ -1,47 +1,32 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="nl_NL">
+<TS version="2.1" language="pt_BR">
   <context>
-    <name>developer_settings</name>
+    <name>ssh_settings</name>
     <message>
-      <location filename="developer_settings.qml" line="48"/>
-      <source>Developer Settings</source>
-      <translation>Ontwikkelaarsinstellingen</translation>
+      <location filename="ssh_settings.qml" line="44"/>
+      <source>SSH Settings</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="117"/>
-      <source>Advanced Settings</source>
-      <translation>Geavanceerde instellingen</translation>
+      <location filename="ssh_settings.qml" line="67"/>
+      <source>By enabling SSH Mode, anyone can access, change or delete anything on this device by connecting to it via another device.</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="152"/>
-      <source>Enable Dashboard</source>
-      <translation>Dashboard inschakelen</translation>
+      <location filename="ssh_settings.qml" line="78"/>
+      <source>Enable SSH</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="165"/>
-      <source>Disable Dashboard</source>
-      <translation>Dashboard uitschakelen</translation>
+      <location filename="ssh_settings.qml" line="88"/>
+      <source>Disable SSH</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="187"/>
-      <source>Dashboard Address</source>
-      <translation>Dashboardadres</translation>
-    </message>
-    <message>
-      <location filename="developer_settings.qml" line="197"/>
-      <source>Dashboard Username</source>
-      <translation>Dashboard-gebruikersnaam</translation>
-    </message>
-    <message>
-      <location filename="developer_settings.qml" line="207"/>
-      <source>Dashboard Password</source>
-      <translation>Dashboardwachtwoord</translation>
-    </message>
-    <message>
-      <location filename="developer_settings.qml" line="250"/>
+      <location filename="ssh_settings.qml" line="133"/>
       <source>Device Settings</source>
-      <translation>Apparaat instellingen</translation>
+      <translation type="unfinished"/>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts`

 * *Files 15% similar despite different names*

#### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts`

```diff
@@ -1,47 +1,47 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="pt_BR">
+<TS version="2.1" language="de_DE">
   <context>
-    <name>developer_settings</name>
+    <name>settingspage</name>
     <message>
-      <location filename="developer_settings.qml" line="48"/>
-      <source>Developer Settings</source>
-      <translation>Configurações do desenvolvedor</translation>
+      <location filename="settingspage.qml" line="19"/>
+      <source>Homescreen Settings</source>
+      <translation>Einstellungen Homescreen</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="117"/>
-      <source>Advanced Settings</source>
-      <translation>Configurações avançadas</translation>
+      <location filename="settingspage.qml" line="25"/>
+      <source>Customize</source>
+      <translation>Anpassen</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="152"/>
-      <source>Enable Dashboard</source>
-      <translation>Ativar painel</translation>
+      <location filename="settingspage.qml" line="31"/>
+      <source>Display</source>
+      <translation>Anzeige</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="165"/>
-      <source>Disable Dashboard</source>
-      <translation>Desativar painel</translation>
+      <location filename="settingspage.qml" line="37"/>
+      <source>Enable SSH</source>
+      <translation>SSH aktivieren</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="187"/>
-      <source>Dashboard Address</source>
-      <translation>Endereço do painel</translation>
+      <location filename="settingspage.qml" line="43"/>
+      <source>Developer Settings</source>
+      <translation>Entwicklereinstellungen</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="197"/>
-      <source>Dashboard Username</source>
-      <translation>Nome de usuário do painel</translation>
+      <location filename="settingspage.qml" line="49"/>
+      <source>About</source>
+      <translation>Über</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="207"/>
-      <source>Dashboard Password</source>
-      <translation>Senha do painel</translation>
+      <location filename="settingspage.qml" line="68"/>
+      <source>Device Settings</source>
+      <translation>Geräteeinstellungen</translation>
     </message>
     <message>
-      <location filename="developer_settings.qml" line="250"/>
-      <source>Device Settings</source>
-      <translation>Configurações do dispositivo</translation>
+      <location filename="settingspage.qml" line="180"/>
+      <source>Home</source>
+      <translation>Home</translation>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts`

 * *Files 9% similar despite different names*

#### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts`

```diff
@@ -1,47 +1,47 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="de_DE">
+<TS version="2.1" language="es_ES">
   <context>
     <name>settingspage</name>
     <message>
       <location filename="settingspage.qml" line="19"/>
       <source>Homescreen Settings</source>
-      <translation>Einstellungen Homescreen</translation>
+      <translation>Configuración de la pantalla de inicio</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="25"/>
       <source>Customize</source>
-      <translation>Anpassen</translation>
+      <translation>personalizar</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="31"/>
       <source>Display</source>
-      <translation>Anzeige</translation>
+      <translation>Monitor</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="37"/>
       <source>Enable SSH</source>
-      <translation>SSH aktivieren</translation>
+      <translation>Habilitar SSH</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="43"/>
       <source>Developer Settings</source>
-      <translation>Entwicklereinstellungen</translation>
+      <translation>Configuración del desarrollador</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="49"/>
       <source>About</source>
-      <translation>Über</translation>
+      <translation>Sobre</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="68"/>
       <source>Device Settings</source>
-      <translation>Geräteeinstellungen</translation>
+      <translation>Configuración de dispositivo</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="180"/>
       <source>Home</source>
-      <translation>Home</translation>
+      <translation>Hogar</translation>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts`

 * *Files 8% similar despite different names*

#### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts`

```diff
@@ -1,47 +1,47 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="es_ES">
+<TS version="2.1" language="fr_FR">
   <context>
     <name>settingspage</name>
     <message>
       <location filename="settingspage.qml" line="19"/>
       <source>Homescreen Settings</source>
-      <translation>Configuración de la pantalla de inicio</translation>
+      <translation>Paramètres de l'écran d'accueil</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="25"/>
       <source>Customize</source>
-      <translation>personalizar</translation>
+      <translation>Personnaliser</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="31"/>
       <source>Display</source>
-      <translation>Monitor</translation>
+      <translation>Affichage</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="37"/>
       <source>Enable SSH</source>
-      <translation>Habilitar SSH</translation>
+      <translation>Activer SSH</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="43"/>
       <source>Developer Settings</source>
-      <translation>Configuración del desarrollador</translation>
+      <translation>Paramètres du développeur</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="49"/>
       <source>About</source>
-      <translation>Sobre</translation>
+      <translation>À propos de</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="68"/>
       <source>Device Settings</source>
-      <translation>Configuración de dispositivo</translation>
+      <translation>Réglages de l'appareil</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="180"/>
       <source>Home</source>
-      <translation>Hogar</translation>
+      <translation>Maison</translation>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts`

 * *Files 14% similar despite different names*

#### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts`

```diff
@@ -1,47 +1,47 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="fr_FR">
+<TS version="2.1" language="nl_NL">
   <context>
     <name>settingspage</name>
     <message>
       <location filename="settingspage.qml" line="19"/>
       <source>Homescreen Settings</source>
-      <translation>Paramètres de l'écran d'accueil</translation>
+      <translation>Instellingen startscherm</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="25"/>
       <source>Customize</source>
-      <translation>Personnaliser</translation>
+      <translation>Aanpassen</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="31"/>
       <source>Display</source>
-      <translation>Affichage</translation>
+      <translation>Weergave</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="37"/>
       <source>Enable SSH</source>
-      <translation>Activer SSH</translation>
+      <translation>SSH inschakelen</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="43"/>
       <source>Developer Settings</source>
-      <translation>Paramètres du développeur</translation>
+      <translation>Ontwikkelaarsinstellingen</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="49"/>
       <source>About</source>
-      <translation>À propos de</translation>
+      <translation>Over</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="68"/>
       <source>Device Settings</source>
-      <translation>Réglages de l'appareil</translation>
+      <translation>Apparaat instellingen</translation>
     </message>
     <message>
       <location filename="settingspage.qml" line="180"/>
       <source>Home</source>
-      <translation>Maison</translation>
+      <translation>Huis</translation>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts`

 * *Files 24% similar despite different names*

#### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts`

```diff
@@ -1,47 +1,32 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="nl_NL">
+<TS version="2.1" language="it_IT">
   <context>
-    <name>settingspage</name>
+    <name>ssh_settings</name>
     <message>
-      <location filename="settingspage.qml" line="19"/>
-      <source>Homescreen Settings</source>
-      <translation>Instellingen startscherm</translation>
+      <location filename="ssh_settings.qml" line="44"/>
+      <source>SSH Settings</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="settingspage.qml" line="25"/>
-      <source>Customize</source>
-      <translation>Aanpassen</translation>
+      <location filename="ssh_settings.qml" line="67"/>
+      <source>By enabling SSH Mode, anyone can access, change or delete anything on this device by connecting to it via another device.</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="settingspage.qml" line="31"/>
-      <source>Display</source>
-      <translation>Weergave</translation>
-    </message>
-    <message>
-      <location filename="settingspage.qml" line="37"/>
+      <location filename="ssh_settings.qml" line="78"/>
       <source>Enable SSH</source>
-      <translation>SSH inschakelen</translation>
-    </message>
-    <message>
-      <location filename="settingspage.qml" line="43"/>
-      <source>Developer Settings</source>
-      <translation>Ontwikkelaarsinstellingen</translation>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="settingspage.qml" line="49"/>
-      <source>About</source>
-      <translation>Over</translation>
+      <location filename="ssh_settings.qml" line="88"/>
+      <source>Disable SSH</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="settingspage.qml" line="68"/>
+      <location filename="ssh_settings.qml" line="133"/>
       <source>Device Settings</source>
-      <translation>Apparaat instellingen</translation>
-    </message>
-    <message>
-      <location filename="settingspage.qml" line="180"/>
-      <source>Home</source>
-      <translation>Huis</translation>
+      <translation type="unfinished"/>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts`

 * *Files 20% similar despite different names*

#### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts`

```diff
@@ -1,47 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="pt_BR">
+<TS version="2.1" language="es_ES">
   <context>
-    <name>settingspage</name>
+    <name>developer_settings</name>
     <message>
-      <location filename="settingspage.qml" line="19"/>
-      <source>Homescreen Settings</source>
-      <translation>Configurações da tela inicial</translation>
-    </message>
-    <message>
-      <location filename="settingspage.qml" line="25"/>
-      <source>Customize</source>
-      <translation>Customizar</translation>
-    </message>
-    <message>
-      <location filename="settingspage.qml" line="31"/>
-      <source>Display</source>
-      <translation>Exibição</translation>
-    </message>
-    <message>
-      <location filename="settingspage.qml" line="37"/>
-      <source>Enable SSH</source>
-      <translation>Ativar SSH</translation>
-    </message>
-    <message>
-      <location filename="settingspage.qml" line="43"/>
+      <location filename="developer_settings.qml" line="48"/>
       <source>Developer Settings</source>
-      <translation>Configurações do desenvolvedor</translation>
+      <translation>Configuración del desarrollador</translation>
     </message>
     <message>
-      <location filename="settingspage.qml" line="49"/>
-      <source>About</source>
-      <translation>Sobre</translation>
+      <location filename="developer_settings.qml" line="117"/>
+      <source>Advanced Settings</source>
+      <translation>Ajustes avanzados</translation>
     </message>
     <message>
-      <location filename="settingspage.qml" line="68"/>
+      <location filename="developer_settings.qml" line="250"/>
       <source>Device Settings</source>
-      <translation>Configurações do dispositivo</translation>
-    </message>
-    <message>
-      <location filename="settingspage.qml" line="180"/>
-      <source>Home</source>
-      <translation>Casa</translation>
+      <translation>Configuración de dispositivo</translation>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts`

 * *Files 21% similar despite different names*

#### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts`

```diff
@@ -1,32 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="fr_FR">
+<TS version="2.1" language="nl_NL">
   <context>
-    <name>ssh_settings</name>
+    <name>developer_settings</name>
     <message>
-      <location filename="ssh_settings.qml" line="44"/>
-      <source>SSH Settings</source>
-      <translation type="unfinished"/>
+      <location filename="developer_settings.qml" line="48"/>
+      <source>Developer Settings</source>
+      <translation>Ontwikkelaarsinstellingen</translation>
     </message>
     <message>
-      <location filename="ssh_settings.qml" line="67"/>
-      <source>By enabling SSH Mode, anyone can access, change or delete anything on this device by connecting to it via another device.</source>
-      <translation type="unfinished"/>
+      <location filename="developer_settings.qml" line="117"/>
+      <source>Advanced Settings</source>
+      <translation>Geavanceerde instellingen</translation>
     </message>
     <message>
-      <location filename="ssh_settings.qml" line="78"/>
-      <source>Enable SSH</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="ssh_settings.qml" line="88"/>
-      <source>Disable SSH</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="ssh_settings.qml" line="133"/>
+      <location filename="developer_settings.qml" line="250"/>
       <source>Device Settings</source>
-      <translation type="unfinished"/>
+      <translation>Apparaat instellingen</translation>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts`

 * *Files 23% similar despite different names*

#### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts`

```diff
@@ -1,32 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="it_IT">
+<TS version="2.1" language="pt_BR">
   <context>
-    <name>ssh_settings</name>
+    <name>developer_settings</name>
     <message>
-      <location filename="ssh_settings.qml" line="44"/>
-      <source>SSH Settings</source>
-      <translation type="unfinished"/>
+      <location filename="developer_settings.qml" line="48"/>
+      <source>Developer Settings</source>
+      <translation>Configurações do desenvolvedor</translation>
     </message>
     <message>
-      <location filename="ssh_settings.qml" line="67"/>
-      <source>By enabling SSH Mode, anyone can access, change or delete anything on this device by connecting to it via another device.</source>
-      <translation type="unfinished"/>
+      <location filename="developer_settings.qml" line="117"/>
+      <source>Advanced Settings</source>
+      <translation>Configurações avançadas</translation>
     </message>
     <message>
-      <location filename="ssh_settings.qml" line="78"/>
-      <source>Enable SSH</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="ssh_settings.qml" line="88"/>
-      <source>Disable SSH</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="ssh_settings.qml" line="133"/>
+      <location filename="developer_settings.qml" line="250"/>
       <source>Device Settings</source>
-      <translation type="unfinished"/>
+      <translation>Configurações do dispositivo</translation>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion/wigets.py` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/wigets.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-gui-plugin-shell-companion
-Version: 0.0.0a7
+Version: 0.0.0a8
 Summary: GUI plugin for ovos-shell
 Home-page: https://github.com/OpenVoiceOS/ovos-gui-plugin-shell-companion
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt` & `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a7/setup.py` & `ovos-gui-plugin-shell-companion-0.0.0a8/setup.py`

 * *Files identical despite different names*

