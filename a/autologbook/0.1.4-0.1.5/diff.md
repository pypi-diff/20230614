# Comparing `tmp/autologbook-0.1.4.tar.gz` & `tmp/autologbook-0.1.5.tar.gz`

## Comparing `autologbook-0.1.4.tar` & `autologbook-0.1.5.tar`

### file list

```diff
@@ -1,252 +1,252 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 autologbook-0.1.4/.flake8
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 autologbook-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 autologbook-0.1.4/pyqt5ac-config.yml
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 autologbook-0.1.4/requirements-dev.txt
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 autologbook-0.1.4/requirements.txt
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/__init__.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/__main__.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/about_dialog_ui.py
--rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/attachment.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autocli.py
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autoconfig.py
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autoerror.py
--rw-r--r--   0        0        0    83315 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autogui.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autologbook_app.py
--rw-r--r--   0        0        0    45270 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autoprotocol.py
--rw-r--r--   0        0        0    61480 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autotools.py
--rw-r--r--   0        0        0    84283 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autowatchdog.py
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/change_sample_dialog_ui.py
--rw-r--r--   0        0        0    60429 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/configuration_editor_ui.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/containers.py
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/context_menu.py
--rw-r--r--   0        0        0    24576 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/dialog_windows.py
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/edit_lock_dialog_ui.py
--rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/elog_interface.py
--rw-r--r--   0        0        0    29594 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/elog_post_splitter.py
--rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/file_system_command.py
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/file_type_guesser.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/html_helpers.py
--rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/jinja_integration.py
--rw-r--r--   0        0        0    33823 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/main_window_ui.py
--rw-r--r--   0        0        0    80159 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/microscope_picture.py
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/model_test_ui.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/navigation_image.py
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/object_factoy.py
--rw-r--r--   0        0        0    17906 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/optical_image.py
--rw-r--r--   0        0        0   157866 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/protocol_editor.py
--rw-r--r--   0        0        0    22485 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/protocol_editor_models.py
--rw-r--r--   0        0        0    27651 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/protocol_editor_ui.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/qt_signal_dispatcher.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/rename_dialog_ui.py
--rw-r--r--   0        0        0   464489 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/resource_rc.py
--rw-r--r--   0        0        0    39102 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/resource_rc.rcc
--rw-r--r--   0        0        0    14444 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/restore_element.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/restore_element_dialog_ui.py
--rw-r--r--   0        0        0    16776 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/sample.py
--rw-r--r--   0        0        0    14839 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/thread_worker.py
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/user_editor_ui.py
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/video.py
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/conf/type_guesser_regexp.yaml
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/attachment_base_template.yammy
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/digital_camera_optical_image_gps_template.yammy
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/digital_camera_optical_image_template.yammy
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/empty_page_template.yammy
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/fei_microscope_picture_template.yammy
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/footer_base_template.yammy
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/general_attachment_base_template.yammy
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/general_optical_images_base_template.yammy
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/keyence_optical_image_template.yammy
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/macros.yammy
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/microscope_list_post_base_template.yammy
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/microscope_list_post_url_only_template.yammy
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/microscope_picture_base_template.yammy
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/multi_microscope_protocol_template.yammy
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/navigation_base_template.yammy
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/navigation_image_template.yammy
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/optical_image_base_template.yammy
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/protocol_base_template.yammy
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/quattro_protocol_template.yammy
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/sample_attachment_base_template.yammy
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/sample_base_template.yammy
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/sample_list_base_template.yammy
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/sample_microscope_picture_base_template.yammy
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/sample_optical_image_base_template.yammy
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/sample_video_base_template.yammy
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/scripts.yammy
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/title_base_template.yammy
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/vega_microscope_picture_base_template.yammy
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/vega_microscope_picture_jpeg_full_template.yammy
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/vega_microscope_picture_jpeg_simple_template.yammy
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/vega_microscope_picture_jpeg_template.yammy
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/video_base_template.yammy
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/xl40_microscope_picture_base_template.yammy
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/xl40_microscope_picture_multi_template.yammy
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/xl40_microscope_picture_single_template.yammy
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/about_dialog.ui
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/change_sample_dialog.ui
--rw-r--r--   0        0        0    58393 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/configuration_editor.ui
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/edit_lock_dialog.ui
--rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/main_window.ui
--rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/model_test.ui
--rw-r--r--   0        0        0    36028 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/protocol_editor.ui
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/rename_dialog.ui
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resource.qrc
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/restore_element_dialog.ui
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/user_editor.ui
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-attach-48.png
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-bold-48.png
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-bulleted-list-48.png
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-cancel-32.png
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-cancel-48.png
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-choose-font-48.png
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-close-30.png
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-code-48.png
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-collapse-arrow-48.png
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-compact-camera-32.png
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-compact-camera-64.png
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-48.png
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-all-48.png
--rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-caption-48.png
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-description-48.png
--rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-extra-48.png
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-link-48.png
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-pair-48.png
--rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-single-48.png
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-design-48.png
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-edit-30.png
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-edit-user-30.png
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-expand-arrow-48.png
--rw-r--r--   0        0        0    29688 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-expand-arrow.gif
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-expand-arrows-48.png
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-folder-48.png
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-fullscreen-48.png
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-green-circle-48.png
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-high-importance-30.png
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-home-48.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-hyperlink-48.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-ice-48.png
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-image-48.png
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-internet-folder-30.png
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-italic-48.png
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-link-folder-48.png
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-logbook-64.png
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-map-marker-48.png
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-markdown-48.png
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-move-up-row-48.png
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-numbered-list-48.png
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-ok-30.png
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-open-envelope-30.png
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-opened-folder-30.png
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-opened-folder-48.png
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-optical-microscope-64.png
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-paste-all-48.png
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-paste-caption-48.png
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-paste-description-48.png
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-paste-extra-48.png
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-paste-special-48.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-pause-48.png
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-pencil-48.png
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-picture-48.png
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-pictures-folder-30.png
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-pictures-folder-48.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-play-48.png
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-recycle-48.png
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-red-circle-48.png
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-rename-48.png
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-save-30.png
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-save-as-48.png
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-search-48.png
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-section-48.png
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-select-all-48.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-sniper-48.png
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-start-30.png
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-start-48.png
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-stop-sign-30.png
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-stop-sign-48.png
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-strikethrough-48.png
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-subscript-48.png
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-superscript-48.png
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-support-48.png
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-sync-48.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-text-48.png
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-tools-48.png
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-trash-can-48.png
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-trash-restore-48.png
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-underline-48.png
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-update-left-rotation-48.png
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-upload-to-cloud-48.png
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-user-secured-48.png
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-video-clip-48.png
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-website-48.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/__init__.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/constants.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/dialog_compare_experiment_file.py
--rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/dialog_compare_experiment_file_ui.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/dialog_select_experiment_file.py
--rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/dialog_select_experiment_file_ui.py
--rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/experiment_wizard.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/experiment_wizard_app.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ini_syntax_highlighter.py
--rw-r--r--   0        0        0   153977 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/resources_rc.py
--rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/search_results_model.py
--rw-r--r--   0        0        0    10242 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_commit_new_experiment_page.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_commit_new_experiment_page_ui.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_conclusion_page.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_conclusion_page_ui.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_introduction_page.py
--rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_introduction_page_ui.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_new_experiment_page.py
--rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_new_experiment_page_ui.py
--rw-r--r--   0        0        0    14027 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_review_configuration_page.py
--rw-r--r--   0        0        0    29347 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_review_configuration_page_ui.py
--rw-r--r--   0        0        0    20948 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_search_experiment_page.py
--rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_search_experiment_page_ui.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/conf/unit_list.yaml
--rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/dialog_compare_experiment_file.ui
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/dialog_select_experiment_file.ui
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/wizard_commit_new_experiment_page.ui
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/wizard_conclusion_page.ui
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/wizard_introduction_page.ui
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/wizard_new_experiment_page.ui
--rw-r--r--   0        0        0    31336 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/wizard_review_configuration_page.ui
--rw-r--r--   0        0        0    11031 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/wizard_search_experiment_page.ui
--rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/ec-logo.jpg
--rw-r--r--   0        0        0    20260 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/glossy-microscope.png
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-done-48.png
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-error-48.png
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-fantasy-48.png
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-folder-48.png
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-new-48.png
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-new-96.png
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-question-mark-48.png
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-website-48.png
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/resources.qrc
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/__init__.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/about_image_converter_ui.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/event_logger.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/fei_image_manipulator.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/image_converter.py
--rw-r--r--   0        0        0    18975 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/image_converter_gui.py
--rw-r--r--   0        0        0    13209 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/main_window_image_converter_ui.py
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/metadata_dumper.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/mirror_maker.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/qt_exception_handler.py
--rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/resource_rc.py
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/util.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/ui/about_image_converter.ui
--rw-r--r--   0        0        0    14399 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/ui/main_window_image_converter.ui
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/ui/resource.qrc
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/ui/resources/icons8-picture-64.png
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/__init__.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_autotools.py
--rw-r--r--   0        0        0    28142 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_element_type_guesser.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_enums.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_file_utils.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_picture_resolution.py
--rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_protocol_elements.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_url_guessing.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 autologbook-0.1.4/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autologbook-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0    19134 2020-02-02 00:00:00.000000 autologbook-0.1.4/README.md
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 autologbook-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    21337 2020-02-02 00:00:00.000000 autologbook-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 autologbook-0.1.5/.flake8
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 autologbook-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 autologbook-0.1.5/pyqt5ac-config.yml
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 autologbook-0.1.5/requirements-dev.txt
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 autologbook-0.1.5/requirements.txt
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/__init__.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/__main__.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/about_dialog_ui.py
+-rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/attachment.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/autocli.py
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/autoconfig.py
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/autoerror.py
+-rw-r--r--   0        0        0    83315 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/autogui.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/autologbook_app.py
+-rw-r--r--   0        0        0    45270 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/autoprotocol.py
+-rw-r--r--   0        0        0    61495 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/autotools.py
+-rw-r--r--   0        0        0    84283 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/autowatchdog.py
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/change_sample_dialog_ui.py
+-rw-r--r--   0        0        0    60597 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/configuration_editor_ui.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/containers.py
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/context_menu.py
+-rw-r--r--   0        0        0    24576 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/dialog_windows.py
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/edit_lock_dialog_ui.py
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/elog_interface.py
+-rw-r--r--   0        0        0    29594 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/elog_post_splitter.py
+-rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/file_system_command.py
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/file_type_guesser.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/html_helpers.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/jinja_integration.py
+-rw-r--r--   0        0        0    33600 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/main_window_ui.py
+-rw-r--r--   0        0        0    80201 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/microscope_picture.py
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/model_test_ui.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/navigation_image.py
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/object_factoy.py
+-rw-r--r--   0        0        0    17906 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/optical_image.py
+-rw-r--r--   0        0        0   157866 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/protocol_editor.py
+-rw-r--r--   0        0        0    22485 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/protocol_editor_models.py
+-rw-r--r--   0        0        0    27651 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/protocol_editor_ui.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/qt_signal_dispatcher.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/rename_dialog_ui.py
+-rw-r--r--   0        0        0   464489 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/resource_rc.py
+-rw-r--r--   0        0        0    39102 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/resource_rc.rcc
+-rw-r--r--   0        0        0    14444 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/restore_element.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/restore_element_dialog_ui.py
+-rw-r--r--   0        0        0    16776 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/sample.py
+-rw-r--r--   0        0        0    14839 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/thread_worker.py
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/user_editor_ui.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/video.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/conf/type_guesser_regexp.yaml
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/attachment_base_template.yammy
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/digital_camera_optical_image_gps_template.yammy
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/digital_camera_optical_image_template.yammy
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/empty_page_template.yammy
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/fei_microscope_picture_template.yammy
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/footer_base_template.yammy
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/general_attachment_base_template.yammy
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/general_optical_images_base_template.yammy
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/keyence_optical_image_template.yammy
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/macros.yammy
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/microscope_list_post_base_template.yammy
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/microscope_list_post_url_only_template.yammy
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/microscope_picture_base_template.yammy
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/multi_microscope_protocol_template.yammy
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/navigation_base_template.yammy
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/navigation_image_template.yammy
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/optical_image_base_template.yammy
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/protocol_base_template.yammy
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/quattro_protocol_template.yammy
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/sample_attachment_base_template.yammy
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/sample_base_template.yammy
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/sample_list_base_template.yammy
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/sample_microscope_picture_base_template.yammy
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/sample_optical_image_base_template.yammy
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/sample_video_base_template.yammy
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/scripts.yammy
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/title_base_template.yammy
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/vega_microscope_picture_base_template.yammy
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/vega_microscope_picture_jpeg_full_template.yammy
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/vega_microscope_picture_jpeg_simple_template.yammy
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/vega_microscope_picture_jpeg_template.yammy
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/video_base_template.yammy
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/xl40_microscope_picture_base_template.yammy
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/xl40_microscope_picture_multi_template.yammy
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/templates/xl40_microscope_picture_single_template.yammy
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/about_dialog.ui
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/change_sample_dialog.ui
+-rw-r--r--   0        0        0    58513 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/configuration_editor.ui
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/edit_lock_dialog.ui
+-rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/main_window.ui
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/model_test.ui
+-rw-r--r--   0        0        0    36028 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/protocol_editor.ui
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/rename_dialog.ui
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resource.qrc
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/restore_element_dialog.ui
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/user_editor.ui
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-attach-48.png
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-bold-48.png
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-bulleted-list-48.png
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-cancel-32.png
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-cancel-48.png
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-choose-font-48.png
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-close-30.png
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-code-48.png
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-collapse-arrow-48.png
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-compact-camera-32.png
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-compact-camera-64.png
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-copy-48.png
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-copy-all-48.png
+-rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-copy-caption-48.png
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-copy-description-48.png
+-rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-copy-extra-48.png
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-copy-link-48.png
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-copy-pair-48.png
+-rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-copy-single-48.png
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-design-48.png
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-edit-30.png
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-edit-user-30.png
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-expand-arrow-48.png
+-rw-r--r--   0        0        0    29688 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-expand-arrow.gif
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-expand-arrows-48.png
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-folder-48.png
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-fullscreen-48.png
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-green-circle-48.png
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-high-importance-30.png
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-home-48.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-hyperlink-48.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-ice-48.png
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-image-48.png
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-internet-folder-30.png
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-italic-48.png
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-link-folder-48.png
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-logbook-64.png
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-map-marker-48.png
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-markdown-48.png
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-move-up-row-48.png
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-numbered-list-48.png
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-ok-30.png
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-open-envelope-30.png
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-opened-folder-30.png
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-opened-folder-48.png
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-optical-microscope-64.png
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-paste-all-48.png
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-paste-caption-48.png
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-paste-description-48.png
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-paste-extra-48.png
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-paste-special-48.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-pause-48.png
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-pencil-48.png
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-picture-48.png
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-pictures-folder-30.png
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-pictures-folder-48.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-play-48.png
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-recycle-48.png
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-red-circle-48.png
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-rename-48.png
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-save-30.png
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-save-as-48.png
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-search-48.png
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-section-48.png
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-select-all-48.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-sniper-48.png
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-start-30.png
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-start-48.png
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-stop-sign-30.png
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-stop-sign-48.png
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-strikethrough-48.png
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-subscript-48.png
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-superscript-48.png
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-support-48.png
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-sync-48.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-text-48.png
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-tools-48.png
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-trash-can-48.png
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-trash-restore-48.png
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-underline-48.png
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-update-left-rotation-48.png
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-upload-to-cloud-48.png
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-user-secured-48.png
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-video-clip-48.png
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 autologbook-0.1.5/autologbook/ui/resources/icons8-website-48.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/__init__.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/constants.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/dialog_compare_experiment_file.py
+-rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/dialog_compare_experiment_file_ui.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/dialog_select_experiment_file.py
+-rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/dialog_select_experiment_file_ui.py
+-rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/experiment_wizard.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/experiment_wizard_app.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ini_syntax_highlighter.py
+-rw-r--r--   0        0        0   153977 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/resources_rc.py
+-rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/search_results_model.py
+-rw-r--r--   0        0        0    10242 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/wizard_commit_new_experiment_page.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/wizard_commit_new_experiment_page_ui.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/wizard_conclusion_page.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/wizard_conclusion_page_ui.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/wizard_introduction_page.py
+-rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/wizard_introduction_page_ui.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/wizard_new_experiment_page.py
+-rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/wizard_new_experiment_page_ui.py
+-rw-r--r--   0        0        0    14027 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/wizard_review_configuration_page.py
+-rw-r--r--   0        0        0    29347 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/wizard_review_configuration_page_ui.py
+-rw-r--r--   0        0        0    20948 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/wizard_search_experiment_page.py
+-rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/wizard_search_experiment_page_ui.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/conf/unit_list.yaml
+-rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/dialog_compare_experiment_file.ui
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/dialog_select_experiment_file.ui
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/wizard_commit_new_experiment_page.ui
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/wizard_conclusion_page.ui
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/wizard_introduction_page.ui
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/wizard_new_experiment_page.ui
+-rw-r--r--   0        0        0    31336 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/wizard_review_configuration_page.ui
+-rw-r--r--   0        0        0    11031 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/wizard_search_experiment_page.ui
+-rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/resources/ec-logo.jpg
+-rw-r--r--   0        0        0    20260 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/resources/glossy-microscope.png
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/resources/icons8-done-48.png
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/resources/icons8-error-48.png
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/resources/icons8-fantasy-48.png
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/resources/icons8-folder-48.png
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/resources/icons8-new-48.png
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/resources/icons8-new-96.png
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/resources/icons8-question-mark-48.png
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/resources/icons8-website-48.png
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 autologbook-0.1.5/expwizard/ui/resources/resources.qrc
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/__init__.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/about_image_converter_ui.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/event_logger.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/fei_image_manipulator.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/image_converter.py
+-rw-r--r--   0        0        0    18975 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/image_converter_gui.py
+-rw-r--r--   0        0        0    13209 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/main_window_image_converter_ui.py
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/metadata_dumper.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/mirror_maker.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/qt_exception_handler.py
+-rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/resource_rc.py
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/util.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/ui/about_image_converter.ui
+-rw-r--r--   0        0        0    14399 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/ui/main_window_image_converter.ui
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/ui/resource.qrc
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 autologbook-0.1.5/labtools/ui/resources/icons8-picture-64.png
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 autologbook-0.1.5/test/__init__.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 autologbook-0.1.5/test/test_autotools.py
+-rw-r--r--   0        0        0    28142 2020-02-02 00:00:00.000000 autologbook-0.1.5/test/test_element_type_guesser.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 autologbook-0.1.5/test/test_enums.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 autologbook-0.1.5/test/test_file_utils.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 autologbook-0.1.5/test/test_picture_resolution.py
+-rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 autologbook-0.1.5/test/test_protocol_elements.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 autologbook-0.1.5/test/test_url_guessing.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 autologbook-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autologbook-0.1.5/LICENSE.txt
+-rw-r--r--   0        0        0    19134 2020-02-02 00:00:00.000000 autologbook-0.1.5/README.md
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 autologbook-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    21337 2020-02-02 00:00:00.000000 autologbook-0.1.5/PKG-INFO
```

### Comparing `autologbook-0.1.4/.pre-commit-config.yaml` & `autologbook-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/requirements-dev.txt` & `autologbook-0.1.5/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/__init__.py` & `autologbook-0.1.5/autologbook/__init__.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/__main__.py` & `autologbook-0.1.5/autologbook/__main__.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/about_dialog_ui.py` & `autologbook-0.1.5/autologbook/about_dialog_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'S:\software-dev\autologbook-dev\autologbook\ui\about_dialog.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.4
+# Created by: PyQt5 UI code generator 5.15.7
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
@@ -28,15 +28,15 @@
         self.retranslateUi(About)
         QtCore.QMetaObject.connectSlotsByName(About)
 
     def retranslateUi(self, About):
         _translate = QtCore.QCoreApplication.translate
         About.setWindowTitle(_translate("About", "About Autologbook"))
         self.label.setText(_translate("About", "<html><head/><body><p align=\"center\"><img src=\":/resources/icons8-logbook-64.png\"/></p><p\n"
-"       align=\"center\"><br/></p><p align=\"center\">AUTOLOGBOOK v0.1.4</p><p\n"
+"       align=\"center\"><br/></p><p align=\"center\">AUTOLOGBOOK v0.1.5</p><p\n"
 "       align=\"center\">A script for automatic logbook generation in microscopy</p><p align=\"center\">GitHub\n"
 "       <a href=\"https://github.com/abulgher/autologbook\"><span style=\" text-decoration:\n"
 "       underline; color:#0000ff;\">Source Code</span></a></p><p align=\"center\">(C)\n"
 "       Antonio Bulgheroni - 2022</p><p align=\"center\"><br/><a href=\"https://icons8.com/icon/pNYOTp5DinZ3/copy\"><span\n"
 "       style=\" text-decoration: underline; color:#0000ff;\">Copy</span></a> icon by <a href=\"https://icons8.com\"><span\n"
 "       style=\" text-decoration: underline; color:#0000ff;\">Icons8</span></a></p></body></html>\n"
 "      "))
```

### Comparing `autologbook-0.1.4/autologbook/attachment.py` & `autologbook-0.1.5/autologbook/attachment.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/autocli.py` & `autologbook-0.1.5/autologbook/autocli.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/autoconfig.py` & `autologbook-0.1.5/autologbook/autoconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 #
 # GENERAL
 #
 CUSTOMID_START = 1000
 CUSTOMID_TIFFCODE = 37510
 VEGA_TIFFCODE = 50431
 VEGA_JPEG_ID_CODE = piexif.ExifIFD.UserComment
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 THREAD_STATUS_UPDATE = 1000  # in ms
 AUTO_SAVE_INTERVAL = 300000  # in ms
 MAX_ATTACHMENTS = 50  # it is a limitation of elog
 ELOG_PAGE_SIZE_LIMIT = 240000  # the real max is 250000, I kept a 10k as a safety margin.
 #
 # ELOG PARAMETERS
 #
```

### Comparing `autologbook-0.1.4/autologbook/autoerror.py` & `autologbook-0.1.5/autologbook/autoerror.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/autogui.py` & `autologbook-0.1.5/autologbook/autogui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/autologbook_app.py` & `autologbook-0.1.5/autologbook/autologbook_app.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/autoprotocol.py` & `autologbook-0.1.5/autologbook/autoprotocol.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/autotools.py` & `autologbook-0.1.5/autologbook/autotools.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
     }
 
     config['Autologbook watchdog'] = {
         'max_attempts': '5',
         'wait_min': '1',
         'wait_max': '5',
         'wait_increment': '1',
-        'minimum delay between ELOG post': '45',
+        'minimum delay between ELOG post': '600',
         'observer_timeout': 0.5
     }
     config['Mirroring watchdog'] = {
         'max_attempts': '2',
         'wait': '0.5',
         'observer_timeout': 0.2
     }
@@ -836,15 +836,15 @@
                                        ResolutionUnit(tiffinfo.get(ures_code, 0)))
         if desired_um is not None:
             resolution.convert_to_unit(desired_um)
 
     elif source == ResolutionSource.FEI_TAG:
 
         fei_tag_code = 34682
-        fei_metadata = configparser.ConfigParser(allow_no_value=True)
+        fei_metadata = configparser.ConfigParser(allow_no_value=True, strict=False)
         fei_metadata.read_string(tiffinfo[fei_tag_code])
 
         pixel_width = fei_metadata.getfloat('Scan', 'PixelWidth')
         pixel_height = fei_metadata.getfloat('Scan', 'PixelHeight')
 
         xres = 1 / (pixel_width * 100)
         yres = 1 / (pixel_height * 100)
```

### Comparing `autologbook-0.1.4/autologbook/autowatchdog.py` & `autologbook-0.1.5/autologbook/autowatchdog.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/change_sample_dialog_ui.py` & `autologbook-0.1.5/autologbook/change_sample_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/configuration_editor_ui.py` & `autologbook-0.1.5/autologbook/configuration_editor_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'S:\software-dev\autologbook-dev\autologbook\ui\configuration_editor.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.4
+# Created by: PyQt5 UI code generator 5.15.7
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
@@ -300,16 +300,17 @@
         self.autologbook_max_attempts_spinbox.setProperty("value", 5)
         self.autologbook_max_attempts_spinbox.setObjectName("autologbook_max_attempts_spinbox")
         self.gridLayout_4.addWidget(self.autologbook_max_attempts_spinbox, 0, 1, 1, 1)
         self.autologbook_wait_max_label = QtWidgets.QLabel(self.autologbook_watchdog_group_box)
         self.autologbook_wait_max_label.setObjectName("autologbook_wait_max_label")
         self.gridLayout_4.addWidget(self.autologbook_wait_max_label, 2, 0, 1, 1)
         self.autologbook_min_delay_spinbox = QtWidgets.QDoubleSpinBox(self.autologbook_watchdog_group_box)
-        self.autologbook_min_delay_spinbox.setDecimals(1)
-        self.autologbook_min_delay_spinbox.setProperty("value", 45.0)
+        self.autologbook_min_delay_spinbox.setDecimals(0)
+        self.autologbook_min_delay_spinbox.setMaximum(3600.0)
+        self.autologbook_min_delay_spinbox.setProperty("value", 600.0)
         self.autologbook_min_delay_spinbox.setObjectName("autologbook_min_delay_spinbox")
         self.gridLayout_4.addWidget(self.autologbook_min_delay_spinbox, 4, 1, 1, 1)
         self.autologbook_wait_min_spinbox = QtWidgets.QDoubleSpinBox(self.autologbook_watchdog_group_box)
         self.autologbook_wait_min_spinbox.setDecimals(1)
         self.autologbook_wait_min_spinbox.setProperty("value", 1.0)
         self.autologbook_wait_min_spinbox.setObjectName("autologbook_wait_min_spinbox")
         self.gridLayout_4.addWidget(self.autologbook_wait_min_spinbox, 1, 1, 1, 1)
@@ -569,21 +570,21 @@
         self.versa_elog_logbook_label.setBuddy(self.versa_elog_logbook_field)
         self.label_10.setBuddy(self.default_microscope_combo)
         self.label_11.setBuddy(self.default_protocol_folder)
         self.label_12.setBuddy(self.default_mirroring_folder)
 
         self.retranslateUi(configurationDialog)
         self.microscope_tabs.setCurrentIndex(0)
-        self.search_basepath_button.clicked.connect(configurationDialog.search_basepath)
-        self.load_conf_button.clicked.connect(configurationDialog.load_conf_file)
-        self.save_conf_button.clicked.connect(configurationDialog.save_conf_file)
-        self.elog_password_field.textEdited['QString'].connect(configurationDialog.password_edited)
-        self.buttonBox.accepted.connect(configurationDialog.accept)
-        self.reset_conf_button.clicked.connect(configurationDialog.reset_conf)
-        self.buttonBox.rejected.connect(configurationDialog.reject)
+        self.search_basepath_button.clicked.connect(configurationDialog.search_basepath) # type: ignore
+        self.load_conf_button.clicked.connect(configurationDialog.load_conf_file) # type: ignore
+        self.save_conf_button.clicked.connect(configurationDialog.save_conf_file) # type: ignore
+        self.elog_password_field.textEdited['QString'].connect(configurationDialog.password_edited) # type: ignore
+        self.buttonBox.accepted.connect(configurationDialog.accept) # type: ignore
+        self.reset_conf_button.clicked.connect(configurationDialog.reset_conf) # type: ignore
+        self.buttonBox.rejected.connect(configurationDialog.reject) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(configurationDialog)
         configurationDialog.setTabOrder(self.elog_user_field, self.elog_password_field)
         configurationDialog.setTabOrder(self.elog_password_field, self.elog_max_auth_error_field)
         configurationDialog.setTabOrder(self.elog_max_auth_error_field, self.elog_hostname_field)
         configurationDialog.setTabOrder(self.elog_hostname_field, self.elog_port_field)
         configurationDialog.setTabOrder(self.elog_port_field, self.elog_ssl_check_box)
         configurationDialog.setTabOrder(self.elog_ssl_check_box, self.elog_timeout_spinbox)
```

### Comparing `autologbook-0.1.4/autologbook/containers.py` & `autologbook-0.1.5/autologbook/containers.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/context_menu.py` & `autologbook-0.1.5/autologbook/context_menu.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/dialog_windows.py` & `autologbook-0.1.5/autologbook/dialog_windows.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/edit_lock_dialog_ui.py` & `autologbook-0.1.5/autologbook/edit_lock_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/elog_interface.py` & `autologbook-0.1.5/autologbook/elog_interface.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/elog_post_splitter.py` & `autologbook-0.1.5/autologbook/elog_post_splitter.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/file_system_command.py` & `autologbook-0.1.5/autologbook/file_system_command.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/file_type_guesser.py` & `autologbook-0.1.5/autologbook/file_type_guesser.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/html_helpers.py` & `autologbook-0.1.5/autologbook/html_helpers.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/jinja_integration.py` & `autologbook-0.1.5/autologbook/jinja_integration.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/main_window_ui.py` & `autologbook-0.1.5/autologbook/main_window_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file 'C:\Users\Antonio\Documents\pyenv\devenv\autologbook\autologbook\ui\main_window.ui'
+# Form implementation generated from reading ui file 'S:\software-dev\autologbook-dev\autologbook\ui\main_window.ui'
 #
 # Created by: PyQt5 UI code generator 5.15.7
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
-from . import resource_rc
-
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
         MainWindow.resize(862, 675)
         MainWindow.setAcceptDrops(True)
         icon = QtGui.QIcon()
@@ -39,16 +37,15 @@
         sizePolicy.setHeightForWidth(self.protocol_folder_text.sizePolicy().hasHeightForWidth())
         self.protocol_folder_text.setSizePolicy(sizePolicy)
         self.protocol_folder_text.setMinimumSize(QtCore.QSize(400, 0))
         self.protocol_folder_text.setObjectName("protocol_folder_text")
         self.gridLayout.addWidget(self.protocol_folder_text, 0, 2, 1, 1)
         self.select_protocol_folder = QtWidgets.QPushButton(self.centralwidget)
         icon1 = QtGui.QIcon()
-        icon1.addPixmap(QtGui.QPixmap(":/resources/icons8-pictures-folder-48.png"),
-                        QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon1.addPixmap(QtGui.QPixmap(":/resources/icons8-pictures-folder-48.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.select_protocol_folder.setIcon(icon1)
         self.select_protocol_folder.setObjectName("select_protocol_folder")
         self.gridLayout.addWidget(self.select_protocol_folder, 0, 3, 1, 4)
         self.mirror_checkBox = QtWidgets.QCheckBox(self.centralwidget)
         self.mirror_checkBox.setLayoutDirection(QtCore.Qt.LeftToRight)
         self.mirror_checkBox.setObjectName("mirror_checkBox")
         self.gridLayout.addWidget(self.mirror_checkBox, 1, 0, 1, 1)
@@ -345,37 +342,36 @@
         self.label_3.setBuddy(self.select_microscope_comboBox)
         self.label_5.setBuddy(self.projectID_field)
         self.label_6.setBuddy(self.project_name_field)
         self.label_7.setBuddy(self.responsible_field)
         self.label_4.setBuddy(self.log_message_box)
 
         self.retranslateUi(MainWindow)
-        self.mirror_checkBox.toggled['bool'].connect(self.mirroring_folder_text.setEnabled)  # type: ignore
-        self.mirror_checkBox.toggled['bool'].connect(self.select_mirroring_folder.setEnabled)  # type: ignore
-        self.watchdog_pushbutton.clicked['bool'].connect(MainWindow.toggled_watchdog)  # type: ignore
-        self.open_explorer_pushbuttom.clicked.connect(MainWindow.open_browser)  # type: ignore
-        self.edit_custom_html_file_pushbutton.clicked.connect(MainWindow.open_yaml_editor)  # type: ignore
-        self.select_protocol_folder.clicked.connect(MainWindow.open_protocol_folder)  # type: ignore
-        self.select_mirroring_folder.clicked.connect(MainWindow.open_mirroring_folder)  # type: ignore
-        self.watchdog_pushbutton.toggled['bool'].connect(self.open_explorer_pushbuttom.setEnabled)  # type: ignore
-        self.select_microscope_comboBox.currentIndexChanged['QString'].connect(
-            MainWindow.changed_microscope)  # type: ignore
-        self.mirror_checkBox.toggled['bool'].connect(MainWindow.toggled_mirroring)  # type: ignore
-        self.protocol_folder_text.editingFinished.connect(MainWindow.validate_inputs)  # type: ignore
-        self.mirroring_folder_text.editingFinished.connect(MainWindow.validate_inputs)  # type: ignore
-        self.clean_logger_pushbutton.clicked.connect(MainWindow.clear_logger)  # type: ignore
-        self.save_logger_pushbutton.clicked.connect(MainWindow.save_logger)  # type: ignore
-        self.custom_ownership_checkbox.toggled['bool'].connect(self.projectID_field.setEnabled)  # type: ignore
-        self.custom_ownership_checkbox.toggled['bool'].connect(self.project_name_field.setEnabled)  # type: ignore
-        self.custom_ownership_checkbox.toggled['bool'].connect(self.responsible_field.setEnabled)  # type: ignore
-        self.custom_ownership_checkbox.toggled['bool'].connect(MainWindow.toggled_custom_ownership)  # type: ignore
-        self.projectID_field.editingFinished.connect(MainWindow.validate_inputs)  # type: ignore
-        self.project_name_field.editingFinished.connect(MainWindow.validate_inputs)  # type: ignore
-        self.responsible_field.editingFinished.connect(MainWindow.validate_inputs)  # type: ignore
-        self.open_browser_button.clicked.connect(MainWindow.open_protocol_webpage)  # type: ignore
+        self.mirror_checkBox.toggled['bool'].connect(self.mirroring_folder_text.setEnabled) # type: ignore
+        self.mirror_checkBox.toggled['bool'].connect(self.select_mirroring_folder.setEnabled) # type: ignore
+        self.watchdog_pushbutton.clicked['bool'].connect(MainWindow.toggled_watchdog) # type: ignore
+        self.open_explorer_pushbuttom.clicked.connect(MainWindow.open_browser) # type: ignore
+        self.edit_custom_html_file_pushbutton.clicked.connect(MainWindow.open_yaml_editor) # type: ignore
+        self.select_protocol_folder.clicked.connect(MainWindow.open_protocol_folder) # type: ignore
+        self.select_mirroring_folder.clicked.connect(MainWindow.open_mirroring_folder) # type: ignore
+        self.watchdog_pushbutton.toggled['bool'].connect(self.open_explorer_pushbuttom.setEnabled) # type: ignore
+        self.select_microscope_comboBox.currentIndexChanged['QString'].connect(MainWindow.changed_microscope) # type: ignore
+        self.mirror_checkBox.toggled['bool'].connect(MainWindow.toggled_mirroring) # type: ignore
+        self.protocol_folder_text.editingFinished.connect(MainWindow.validate_inputs) # type: ignore
+        self.mirroring_folder_text.editingFinished.connect(MainWindow.validate_inputs) # type: ignore
+        self.clean_logger_pushbutton.clicked.connect(MainWindow.clear_logger) # type: ignore
+        self.save_logger_pushbutton.clicked.connect(MainWindow.save_logger) # type: ignore
+        self.custom_ownership_checkbox.toggled['bool'].connect(self.projectID_field.setEnabled) # type: ignore
+        self.custom_ownership_checkbox.toggled['bool'].connect(self.project_name_field.setEnabled) # type: ignore
+        self.custom_ownership_checkbox.toggled['bool'].connect(self.responsible_field.setEnabled) # type: ignore
+        self.custom_ownership_checkbox.toggled['bool'].connect(MainWindow.toggled_custom_ownership) # type: ignore
+        self.projectID_field.editingFinished.connect(MainWindow.validate_inputs) # type: ignore
+        self.project_name_field.editingFinished.connect(MainWindow.validate_inputs) # type: ignore
+        self.responsible_field.editingFinished.connect(MainWindow.validate_inputs) # type: ignore
+        self.open_browser_button.clicked.connect(MainWindow.open_protocol_webpage) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
         MainWindow.setTabOrder(self.protocol_folder_text, self.select_protocol_folder)
         MainWindow.setTabOrder(self.select_protocol_folder, self.mirror_checkBox)
         MainWindow.setTabOrder(self.mirror_checkBox, self.mirroring_folder_text)
         MainWindow.setTabOrder(self.mirroring_folder_text, self.select_mirroring_folder)
         MainWindow.setTabOrder(self.select_mirroring_folder, self.select_microscope_comboBox)
         MainWindow.setTabOrder(self.select_microscope_comboBox, self.custom_ownership_checkbox)
@@ -390,62 +386,51 @@
         MainWindow.setTabOrder(self.clean_logger_pushbutton, self.save_logger_pushbutton)
 
     def retranslateUi(self, MainWindow):
         _translate = QtCore.QCoreApplication.translate
         MainWindow.setWindowTitle(_translate("MainWindow", "Autologbook GUI"))
         self.label.setText(_translate("MainWindow", "Protocol folder"))
         self.select_protocol_folder.setToolTip(_translate("MainWindow", "Select the protocol folder"))
-        self.select_protocol_folder.setWhatsThis(_translate(
-            "MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Click here to select a folder to be monitored. </span></p><p>It is recommended to name this folder as ProtocolID-Project-Responsible as, for example, 2204123-RADCAS-Bulgheroni</p></body></html>"))
+        self.select_protocol_folder.setWhatsThis(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Click here to select a folder to be monitored. </span></p><p>It is recommended to name this folder as ProtocolID-Project-Responsible as, for example, 2204123-RADCAS-Bulgheroni</p></body></html>"))
         self.select_protocol_folder.setText(_translate("MainWindow", "Select folder"))
-        self.mirror_checkBox.setToolTip(_translate(
-            "MainWindow", "<html><head/><body><p>Activate mirroring</p></body></html>"))
-        self.mirror_checkBox.setWhatsThis(_translate(
-            "MainWindow", "<html><head/><body><p>Activating the mirroring will start the automatic copy of all files present in the protocol folder to the mirroring folder.</p></body></html>"))
+        self.mirror_checkBox.setToolTip(_translate("MainWindow", "<html><head/><body><p>Activate mirroring</p></body></html>"))
+        self.mirror_checkBox.setWhatsThis(_translate("MainWindow", "<html><head/><body><p>Activating the mirroring will start the automatic copy of all files present in the protocol folder to the mirroring folder.</p></body></html>"))
         self.mirror_checkBox.setText(_translate("MainWindow", "Activate mirroring"))
         self.label_2.setText(_translate("MainWindow", "Mirroring folder"))
-        self.select_mirroring_folder.setToolTip(_translate(
-            "MainWindow", "<html><head/><body><p>Select a mirroring folder</p></body></html>"))
-        self.select_mirroring_folder.setWhatsThis(_translate(
-            "MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Select a mirroring folder</span></p><p>This folder <span style=\" font-weight:600;\">must </span>have be named as ProtocolID-Project-Responsible and must be on R:\\A226\\Results. If not, the watchdog won\'t be able to start.</p></body></html>"))
+        self.select_mirroring_folder.setToolTip(_translate("MainWindow", "<html><head/><body><p>Select a mirroring folder</p></body></html>"))
+        self.select_mirroring_folder.setWhatsThis(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Select a mirroring folder</span></p><p>This folder <span style=\" font-weight:600;\">must </span>have be named as ProtocolID-Project-Responsible and must be on R:\\A226\\Results. If not, the watchdog won\'t be able to start.</p></body></html>"))
         self.select_mirroring_folder.setText(_translate("MainWindow", "Select folder"))
         self.label_3.setText(_translate("MainWindow", "Select microscope "))
-        self.select_microscope_comboBox.setToolTip(_translate(
-            "MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Select the microscope as appropriate.</span></p></body></html>"))
+        self.select_microscope_comboBox.setToolTip(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Select the microscope as appropriate.</span></p></body></html>"))
         self.select_microscope_comboBox.setItemText(0, _translate("MainWindow", "Quattro"))
         self.select_microscope_comboBox.setItemText(1, _translate("MainWindow", "Versa"))
         self.select_microscope_comboBox.setItemText(2, _translate("MainWindow", "XL40-GB"))
         self.select_microscope_comboBox.setItemText(3, _translate("MainWindow", "XL40-Cold"))
         self.select_microscope_comboBox.setItemText(4, _translate("MainWindow", "Vega"))
         self.select_microscope_comboBox.setItemText(5, _translate("MainWindow", "TEM"))
         self.GUIThreadLabel.setText(_translate("MainWindow", "G:"))
         self.gui_thread_status.setToolTip(_translate("MainWindow", "Status of the GUI thread"))
-        self.custom_ownership_checkbox.setToolTip(_translate(
-            "MainWindow", "<html><head/><body><p>Activate custom protocol parameters (ID / Projet name / Project responsible)</p></body></html>"))
+        self.custom_ownership_checkbox.setToolTip(_translate("MainWindow", "<html><head/><body><p>Activate custom protocol parameters (ID / Projet name / Project responsible)</p></body></html>"))
         self.custom_ownership_checkbox.setText(_translate("MainWindow", "Use custom parameters"))
         self.label_5.setText(_translate("MainWindow", "Protocol ID"))
         self.label_6.setText(_translate("MainWindow", "Project name"))
         self.label_7.setText(_translate("MainWindow", "Responsible"))
         self.AutoThreadLabel.setText(_translate("MainWindow", "A:"))
         self.auto_thread_status.setToolTip(_translate("MainWindow", "Status of the autologbook watchdog thread"))
         self.auto_obs_status.setToolTip(_translate("MainWindow", "Status of the autologbook watchdog observer thread"))
         self.auto_emi_status.setToolTip(_translate("MainWindow", "Status of the autologbook watchdog emitter thread"))
-        self.watchdog_pushbutton.setToolTip(_translate(
-            "MainWindow", "<html><head/><body><p>Start the watchog</p></body></html>"))
+        self.watchdog_pushbutton.setToolTip(_translate("MainWindow", "<html><head/><body><p>Start the watchog</p></body></html>"))
         self.watchdog_pushbutton.setWhatsThis(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Start the watchdog</span></p><p><br/></p><p>The watchdog will monitor the protocol or the mirroring  folder for interesting new file and add them to eLOG entry automatically.</p><p><br/></p><p>At least one between the protocol and the mirroring folder must be rooted in R:\\A226\\Results, otherwise the watchdog won\'t be started.</p></body></html>"))
         self.watchdog_pushbutton.setText(_translate("MainWindow", "Start watchdog"))
         self.open_explorer_pushbuttom.setToolTip(_translate("MainWindow", "Open the protocol folder"))
-        self.open_explorer_pushbuttom.setWhatsThis(_translate(
-            "MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Open protocol folder</span></p><p>Click this button to open a file explorer pointing to either the protocol folder or the mirroring one if the mirroing option is activated.</p></body></html>"))
+        self.open_explorer_pushbuttom.setWhatsThis(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Open protocol folder</span></p><p>Click this button to open a file explorer pointing to either the protocol folder or the mirroring one if the mirroing option is activated.</p></body></html>"))
         self.open_explorer_pushbuttom.setText(_translate("MainWindow", "Open protocol folder"))
-        self.open_browser_button.setToolTip(_translate(
-            "MainWindow", "<html><head/><body><p>Open the protocol webpage</p></body></html>"))
+        self.open_browser_button.setToolTip(_translate("MainWindow", "<html><head/><body><p>Open the protocol webpage</p></body></html>"))
         self.open_browser_button.setText(_translate("MainWindow", "Open protocol webpage"))
-        self.edit_custom_html_file_pushbutton.setToolTip(_translate(
-            "MainWindow", "<html><head/><body><p>Open the interactive protocol editor</p></body></html>"))
+        self.edit_custom_html_file_pushbutton.setToolTip(_translate("MainWindow", "<html><head/><body><p>Open the interactive protocol editor</p></body></html>"))
         self.edit_custom_html_file_pushbutton.setText(_translate("MainWindow", "Open protocol editor"))
         self.label_4.setText(_translate("MainWindow", "Logging messages"))
         self.clean_logger_pushbutton.setText(_translate("MainWindow", "Clear logger"))
         self.save_logger_pushbutton.setText(_translate("MainWindow", "Save logger..."))
         self.menu_File.setTitle(_translate("MainWindow", "&File"))
         self.menuLoad_recent.setTitle(_translate("MainWindow", "Load recent"))
         self.menuRun.setTitle(_translate("MainWindow", "Run"))
@@ -468,7 +453,8 @@
         self.action_toggle_watchdog.setText(_translate("MainWindow", "Toggle watchdog"))
         self.action_toggle_watchdog.setToolTip(_translate("MainWindow", "Start / stop the watchdog"))
         self.action_toggle_watchdog.setShortcut(_translate("MainWindow", "Ctrl+G"))
         self.actionRecent1.setText(_translate("MainWindow", "Recent1"))
         self.actionRecent2.setText(_translate("MainWindow", "Recent2"))
         self.actionRecent3.setText(_translate("MainWindow", "Recent3"))
         self.actionRecent4.setText(_translate("MainWindow", "Recent4"))
+from . import resource_rc
```

### Comparing `autologbook-0.1.4/autologbook/microscope_picture.py` & `autologbook-0.1.5/autologbook/microscope_picture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1626,15 +1626,15 @@
 
     def _remove_databar(self, input_file, output_file):
 
         with Image.open(input_file) as full_img:
             tiffinfo = full_img.tag_v2
             image_xsize, image_ysize = full_img.size
 
-            fei_metadata = configparser.ConfigParser(allow_no_value=True)
+            fei_metadata = configparser.ConfigParser(allow_no_value=True, strict=False)
             fei_metadata.read_string(tiffinfo[self.params['fei_tag_code']])
 
             scan_width = fei_metadata.getint('Image', 'ResolutionX')
             scan_height = fei_metadata.getint('Image', 'ResolutionY')
 
             if (image_xsize, image_ysize) != (scan_width, scan_height):
                 crop_img = full_img.crop((0, 0, scan_width, scan_height))
@@ -1679,15 +1679,15 @@
                     good_fei_tag_code = fei_tag_code
                     break
             if good_fei_tag_code is None:
                 raise autoerror.NotFEIMicroscopePicture
             else:
                 self.params['fei_tag_code'] = good_fei_tag_code
 
-            fei_metadata = configparser.ConfigParser(allow_no_value=True)
+            fei_metadata = configparser.ConfigParser(allow_no_value=True, strict=False)
             fei_metadata.read_string(tiff_tags[good_fei_tag_code])
 
             # for HV add kV if > 1000
             self.params['hv'] = (
                 fei_metadata.get('Beam', 'HV') + 'V',
                 str(round(fei_metadata.getfloat('Beam', 'HV') / 1000)) + 'kV'
             )[fei_metadata.getfloat('Beam', 'HV') > 1000]
@@ -1757,15 +1757,15 @@
         for fei_tag_code in autotools.FEITagCodes:
             if fei_tag_code in tiff_tags:
                 good_fei_tag_code = fei_tag_code
                 break
         if good_fei_tag_code is None:
             return None
 
-        fei_metadata = configparser.ConfigParser(allow_no_value=True)
+        fei_metadata = configparser.ConfigParser(allow_no_value=True, strict=False)
         fei_metadata.read_string(tiff_tags[good_fei_tag_code])
 
         return fei_metadata.get('System', 'SystemType', fallback=None)
 
     def update(self):
         """
         Update the parameters of an FEI Microscope picture.
```

### Comparing `autologbook-0.1.4/autologbook/model_test_ui.py` & `autologbook-0.1.5/autologbook/model_test_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/navigation_image.py` & `autologbook-0.1.5/autologbook/navigation_image.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/object_factoy.py` & `autologbook-0.1.5/autologbook/object_factoy.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/optical_image.py` & `autologbook-0.1.5/autologbook/optical_image.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/protocol_editor.py` & `autologbook-0.1.5/autologbook/protocol_editor.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/protocol_editor_models.py` & `autologbook-0.1.5/autologbook/protocol_editor_models.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/protocol_editor_ui.py` & `autologbook-0.1.5/autologbook/protocol_editor_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/qt_signal_dispatcher.py` & `autologbook-0.1.5/autologbook/qt_signal_dispatcher.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/rename_dialog_ui.py` & `autologbook-0.1.5/autologbook/rename_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/resource_rc.py` & `autologbook-0.1.5/autologbook/resource_rc.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/resource_rc.rcc` & `autologbook-0.1.5/autologbook/resource_rc.rcc`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/restore_element.py` & `autologbook-0.1.5/autologbook/restore_element.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/restore_element_dialog_ui.py` & `autologbook-0.1.5/autologbook/restore_element_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/sample.py` & `autologbook-0.1.5/autologbook/sample.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/thread_worker.py` & `autologbook-0.1.5/autologbook/thread_worker.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/user_editor_ui.py` & `autologbook-0.1.5/autologbook/user_editor_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/video.py` & `autologbook-0.1.5/autologbook/video.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/conf/type_guesser_regexp.yaml` & `autologbook-0.1.5/autologbook/conf/type_guesser_regexp.yaml`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/attachment_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/attachment_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/digital_camera_optical_image_gps_template.yammy` & `autologbook-0.1.5/autologbook/templates/digital_camera_optical_image_gps_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/digital_camera_optical_image_template.yammy` & `autologbook-0.1.5/autologbook/templates/digital_camera_optical_image_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/fei_microscope_picture_template.yammy` & `autologbook-0.1.5/autologbook/templates/fei_microscope_picture_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/general_optical_images_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/general_optical_images_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/macros.yammy` & `autologbook-0.1.5/autologbook/templates/macros.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/microscope_picture_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/microscope_picture_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/navigation_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/navigation_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/navigation_image_template.yammy` & `autologbook-0.1.5/autologbook/templates/navigation_image_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/optical_image_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/optical_image_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/protocol_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/protocol_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/quattro_protocol_template.yammy` & `autologbook-0.1.5/autologbook/templates/quattro_protocol_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/sample_attachment_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/sample_attachment_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/sample_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/sample_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/sample_list_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/sample_list_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/sample_microscope_picture_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/sample_microscope_picture_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/sample_optical_image_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/sample_optical_image_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/sample_video_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/sample_video_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/scripts.yammy` & `autologbook-0.1.5/autologbook/templates/scripts.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/title_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/title_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/vega_microscope_picture_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/vega_microscope_picture_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/vega_microscope_picture_jpeg_simple_template.yammy` & `autologbook-0.1.5/autologbook/templates/vega_microscope_picture_jpeg_simple_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/vega_microscope_picture_jpeg_template.yammy` & `autologbook-0.1.5/autologbook/templates/vega_microscope_picture_jpeg_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/video_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/video_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/xl40_microscope_picture_base_template.yammy` & `autologbook-0.1.5/autologbook/templates/xl40_microscope_picture_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/templates/xl40_microscope_picture_multi_template.yammy` & `autologbook-0.1.5/autologbook/templates/xl40_microscope_picture_multi_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/about_dialog.ui` & `autologbook-0.1.5/autologbook/ui/about_dialog.ui`

 * *Files 8% similar despite different names*

#### Comparing `autologbook-0.1.4/autologbook/ui/about_dialog.ui` & `autologbook-0.1.5/autologbook/ui/about_dialog.ui`

```diff
@@ -23,15 +23,15 @@
       </iconset>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
         <widget class="QLabel" name="label">
           <property name="text">
             <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;center&quot;&gt;&lt;img src=&quot;:/resources/icons8-logbook-64.png&quot;/&gt;&lt;/p&gt;&lt;p
-       align=&quot;center&quot;&gt;&lt;br/&gt;&lt;/p&gt;&lt;p align=&quot;center&quot;&gt;AUTOLOGBOOK v0.1.4&lt;/p&gt;&lt;p
+       align=&quot;center&quot;&gt;&lt;br/&gt;&lt;/p&gt;&lt;p align=&quot;center&quot;&gt;AUTOLOGBOOK v0.1.5&lt;/p&gt;&lt;p
        align=&quot;center&quot;&gt;A script for automatic logbook generation in microscopy&lt;/p&gt;&lt;p align=&quot;center&quot;&gt;GitHub
        &lt;a href=&quot;https://github.com/abulgher/autologbook&quot;&gt;&lt;span style=&quot; text-decoration:
        underline; color:#0000ff;&quot;&gt;Source Code&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;&lt;p align=&quot;center&quot;&gt;(C)
        Antonio Bulgheroni - 2022&lt;/p&gt;&lt;p align=&quot;center&quot;&gt;&lt;br/&gt;&lt;a href=&quot;https://icons8.com/icon/pNYOTp5DinZ3/copy&quot;&gt;&lt;span
        style=&quot; text-decoration: underline; color:#0000ff;&quot;&gt;Copy&lt;/span&gt;&lt;/a&gt; icon by &lt;a href=&quot;https://icons8.com&quot;&gt;&lt;span
        style=&quot; text-decoration: underline; color:#0000ff;&quot;&gt;Icons8&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
           </property>
```

### Comparing `autologbook-0.1.4/autologbook/ui/change_sample_dialog.ui` & `autologbook-0.1.5/autologbook/ui/change_sample_dialog.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/configuration_editor.ui` & `autologbook-0.1.5/autologbook/ui/configuration_editor.ui`

 * *Files 1% similar despite different names*

#### Comparing `autologbook-0.1.4/autologbook/ui/configuration_editor.ui` & `autologbook-0.1.5/autologbook/ui/configuration_editor.ui`

```diff
@@ -635,18 +635,21 @@
                         </item>
                         <item row="4" column="1">
                           <widget class="QDoubleSpinBox" name="autologbook_min_delay_spinbox">
                             <property name="whatsThis">
                               <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;&lt;span style=&quot; font-size:14pt; font-weight:600;&quot;&gt;Delay between ELOG posts&lt;/span&gt;&lt;/p&gt;&lt;p&gt;&lt;br/&gt;&lt;/p&gt;&lt;p&gt;If many filesystem events are detected by the autologbook watchdog, there could be a high number of almost identical ELOG message posted in a short period of time. All these posts are not only saturating the band and riskying to kill the ELOG server, but they are also useless. &lt;/p&gt;&lt;p&gt;&lt;br/&gt;&lt;/p&gt;&lt;p&gt;For this reason, two ELOG posts must be separated at least by the number of seconds specified by this parameter.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                             </property>
                             <property name="decimals">
-                              <number>1</number>
+                              <number>0</number>
+                            </property>
+                            <property name="maximum">
+                              <double>3600.000000000000000</double>
                             </property>
                             <property name="value">
-                              <double>45.000000000000000</double>
+                              <double>600.000000000000000</double>
                             </property>
                           </widget>
                         </item>
                         <item row="1" column="1">
                           <widget class="QDoubleSpinBox" name="autologbook_wait_min_spinbox">
                             <property name="whatsThis">
                               <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;&lt;span style=&quot; font-size:14pt;&quot;&gt;Autologobook watchdog minimum waiting time&lt;/span&gt;&lt;/p&gt;&lt;p&gt;While the autologbook watchdog is monitoring the protocol folder and try to operate on a file, it could be that for several reasons the process is failing.&lt;/p&gt;&lt;p&gt;In this case the same process will be attempted up to a maximum number of trials with an increasing waiting time in between from minimum waiting time (this parameter) to maximum waititng time with a waiting time increment.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
```

### Comparing `autologbook-0.1.4/autologbook/ui/edit_lock_dialog.ui` & `autologbook-0.1.5/autologbook/ui/edit_lock_dialog.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/main_window.ui` & `autologbook-0.1.5/autologbook/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/model_test.ui` & `autologbook-0.1.5/autologbook/ui/model_test.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/protocol_editor.ui` & `autologbook-0.1.5/autologbook/ui/protocol_editor.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/rename_dialog.ui` & `autologbook-0.1.5/autologbook/ui/rename_dialog.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resource.qrc` & `autologbook-0.1.5/autologbook/ui/resource.qrc`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/restore_element_dialog.ui` & `autologbook-0.1.5/autologbook/ui/restore_element_dialog.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/user_editor.ui` & `autologbook-0.1.5/autologbook/ui/user_editor.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-attach-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-attach-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-bold-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-bold-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-cancel-32.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-cancel-32.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-cancel-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-cancel-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-choose-font-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-choose-font-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-close-30.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-close-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-code-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-code-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-compact-camera-64.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-compact-camera-64.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-all-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-copy-all-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-caption-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-copy-caption-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-description-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-copy-description-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-extra-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-copy-extra-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-link-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-copy-link-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-pair-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-copy-pair-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-single-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-copy-single-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-design-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-design-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-edit-30.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-edit-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-edit-user-30.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-edit-user-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-expand-arrow.gif` & `autologbook-0.1.5/autologbook/ui/resources/icons8-expand-arrow.gif`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-green-circle-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-green-circle-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-high-importance-30.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-high-importance-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-home-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-home-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-hyperlink-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-hyperlink-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-ice-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-ice-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-image-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-image-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-internet-folder-30.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-internet-folder-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-link-folder-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-link-folder-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-logbook-64.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-logbook-64.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-map-marker-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-map-marker-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-markdown-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-markdown-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-move-up-row-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-move-up-row-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-numbered-list-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-numbered-list-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-ok-30.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-ok-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-open-envelope-30.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-open-envelope-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-opened-folder-30.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-opened-folder-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-opened-folder-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-opened-folder-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-optical-microscope-64.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-optical-microscope-64.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-paste-all-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-paste-all-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-paste-caption-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-paste-caption-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-paste-description-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-paste-description-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-paste-extra-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-paste-extra-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-paste-special-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-paste-special-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-pencil-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-pencil-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-picture-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-picture-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-pictures-folder-30.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-pictures-folder-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-pictures-folder-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-pictures-folder-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-play-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-play-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-recycle-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-recycle-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-red-circle-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-red-circle-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-save-as-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-save-as-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-search-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-search-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-section-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-section-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-sniper-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-sniper-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-start-30.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-start-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-start-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-start-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-stop-sign-30.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-stop-sign-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-stop-sign-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-stop-sign-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-strikethrough-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-strikethrough-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-support-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-support-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-sync-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-sync-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-tools-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-tools-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-trash-restore-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-trash-restore-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-underline-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-underline-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-update-left-rotation-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-update-left-rotation-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-upload-to-cloud-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-upload-to-cloud-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-user-secured-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-user-secured-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/autologbook/ui/resources/icons8-website-48.png` & `autologbook-0.1.5/autologbook/ui/resources/icons8-website-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/constants.py` & `autologbook-0.1.5/expwizard/constants.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/dialog_compare_experiment_file.py` & `autologbook-0.1.5/expwizard/dialog_compare_experiment_file.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/dialog_compare_experiment_file_ui.py` & `autologbook-0.1.5/expwizard/dialog_compare_experiment_file_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/dialog_select_experiment_file.py` & `autologbook-0.1.5/expwizard/dialog_select_experiment_file.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/dialog_select_experiment_file_ui.py` & `autologbook-0.1.5/expwizard/dialog_select_experiment_file_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/experiment_wizard.py` & `autologbook-0.1.5/expwizard/experiment_wizard.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/experiment_wizard_app.py` & `autologbook-0.1.5/expwizard/experiment_wizard_app.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ini_syntax_highlighter.py` & `autologbook-0.1.5/expwizard/ini_syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/resources_rc.py` & `autologbook-0.1.5/expwizard/resources_rc.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/search_results_model.py` & `autologbook-0.1.5/expwizard/search_results_model.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/wizard_commit_new_experiment_page.py` & `autologbook-0.1.5/expwizard/wizard_commit_new_experiment_page.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/wizard_commit_new_experiment_page_ui.py` & `autologbook-0.1.5/expwizard/wizard_commit_new_experiment_page_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/wizard_conclusion_page.py` & `autologbook-0.1.5/expwizard/wizard_conclusion_page.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/wizard_conclusion_page_ui.py` & `autologbook-0.1.5/expwizard/wizard_conclusion_page_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/wizard_introduction_page.py` & `autologbook-0.1.5/expwizard/wizard_introduction_page.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/wizard_introduction_page_ui.py` & `autologbook-0.1.5/expwizard/wizard_introduction_page_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/wizard_new_experiment_page.py` & `autologbook-0.1.5/expwizard/wizard_new_experiment_page.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/wizard_new_experiment_page_ui.py` & `autologbook-0.1.5/expwizard/wizard_new_experiment_page_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/wizard_review_configuration_page.py` & `autologbook-0.1.5/expwizard/wizard_review_configuration_page.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/wizard_review_configuration_page_ui.py` & `autologbook-0.1.5/expwizard/wizard_review_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/wizard_search_experiment_page.py` & `autologbook-0.1.5/expwizard/wizard_search_experiment_page.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/wizard_search_experiment_page_ui.py` & `autologbook-0.1.5/expwizard/wizard_search_experiment_page_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/conf/unit_list.yaml` & `autologbook-0.1.5/expwizard/conf/unit_list.yaml`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/dialog_compare_experiment_file.ui` & `autologbook-0.1.5/expwizard/ui/dialog_compare_experiment_file.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/dialog_select_experiment_file.ui` & `autologbook-0.1.5/expwizard/ui/dialog_select_experiment_file.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/wizard_commit_new_experiment_page.ui` & `autologbook-0.1.5/expwizard/ui/wizard_commit_new_experiment_page.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/wizard_conclusion_page.ui` & `autologbook-0.1.5/expwizard/ui/wizard_conclusion_page.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/wizard_introduction_page.ui` & `autologbook-0.1.5/expwizard/ui/wizard_introduction_page.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/wizard_new_experiment_page.ui` & `autologbook-0.1.5/expwizard/ui/wizard_new_experiment_page.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/wizard_review_configuration_page.ui` & `autologbook-0.1.5/expwizard/ui/wizard_review_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/wizard_search_experiment_page.ui` & `autologbook-0.1.5/expwizard/ui/wizard_search_experiment_page.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/resources/ec-logo.jpg` & `autologbook-0.1.5/expwizard/ui/resources/ec-logo.jpg`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/resources/glossy-microscope.png` & `autologbook-0.1.5/expwizard/ui/resources/glossy-microscope.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/resources/icons8-error-48.png` & `autologbook-0.1.5/expwizard/ui/resources/icons8-error-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/resources/icons8-fantasy-48.png` & `autologbook-0.1.5/expwizard/ui/resources/icons8-fantasy-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/resources/icons8-new-48.png` & `autologbook-0.1.5/expwizard/ui/resources/icons8-new-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/resources/icons8-new-96.png` & `autologbook-0.1.5/expwizard/ui/resources/icons8-new-96.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/resources/icons8-question-mark-48.png` & `autologbook-0.1.5/expwizard/ui/resources/icons8-question-mark-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/expwizard/ui/resources/icons8-website-48.png` & `autologbook-0.1.5/expwizard/ui/resources/icons8-website-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/__init__.py` & `autologbook-0.1.5/labtools/__init__.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/about_image_converter_ui.py` & `autologbook-0.1.5/labtools/about_image_converter_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/event_logger.py` & `autologbook-0.1.5/labtools/event_logger.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/fei_image_manipulator.py` & `autologbook-0.1.5/labtools/fei_image_manipulator.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/image_converter.py` & `autologbook-0.1.5/labtools/image_converter.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/image_converter_gui.py` & `autologbook-0.1.5/labtools/image_converter_gui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/main_window_image_converter_ui.py` & `autologbook-0.1.5/labtools/main_window_image_converter_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/metadata_dumper.py` & `autologbook-0.1.5/labtools/metadata_dumper.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/mirror_maker.py` & `autologbook-0.1.5/labtools/mirror_maker.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/qt_exception_handler.py` & `autologbook-0.1.5/labtools/qt_exception_handler.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/resource_rc.py` & `autologbook-0.1.5/labtools/resource_rc.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/util.py` & `autologbook-0.1.5/labtools/util.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/ui/about_image_converter.ui` & `autologbook-0.1.5/labtools/ui/about_image_converter.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/ui/main_window_image_converter.ui` & `autologbook-0.1.5/labtools/ui/main_window_image_converter.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/labtools/ui/resources/icons8-picture-64.png` & `autologbook-0.1.5/labtools/ui/resources/icons8-picture-64.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/test/__init__.py` & `autologbook-0.1.5/test/__init__.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/test/test_autotools.py` & `autologbook-0.1.5/test/test_autotools.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/test/test_element_type_guesser.py` & `autologbook-0.1.5/test/test_element_type_guesser.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/test/test_enums.py` & `autologbook-0.1.5/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/test/test_file_utils.py` & `autologbook-0.1.5/test/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/test/test_picture_resolution.py` & `autologbook-0.1.5/test/test_picture_resolution.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/test/test_protocol_elements.py` & `autologbook-0.1.5/test/test_protocol_elements.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/test/test_url_guessing.py` & `autologbook-0.1.5/test/test_url_guessing.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/.gitignore` & `autologbook-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/LICENSE.txt` & `autologbook-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/README.md` & `autologbook-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.4/pyproject.toml` & `autologbook-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 [tool.isort]
 line_length = 119
 multi_line_output = 3
 include_trailing_comma = true
 
 [project]
 name = "autologbook"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name = "Antonio Bulgheroni", email = "antonio.bulgheroni@gmail.com" },
 ]
 dependencies = [
   'py_elog >= 1.3.16',
   'Markdown ==3.4.1',
   'watchdog >= 2.1.9',
```

### Comparing `autologbook-0.1.4/PKG-INFO` & `autologbook-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autologbook
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python toolkit for the automatic generation of elog entries of SEM analysis.
 Project-URL: Homepage, https://github.com/abulgher/autologbook
 Author-email: Antonio Bulgheroni <antonio.bulgheroni@gmail.com>
 License: Copyright (c) 2022 Antonio Bulgheroni
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

