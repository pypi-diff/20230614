# Comparing `tmp/qiskit_metal-0.1.2.tar.gz` & `tmp/qiskit_metal-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qiskit_metal-0.1.2.tar", last modified: Sat Jul 23 14:33:08 2022, max compression
+gzip compressed data, was "qiskit_metal-0.1.5.tar", last modified: Wed Jun 14 21:57:03 2023, max compression
```

## Comparing `qiskit_metal-0.1.2.tar` & `qiskit_metal-0.1.5.tar`

### file list

```diff
@@ -1,307 +1,333 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    10531 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8437 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/
--rw-r--r--   0 runner    (1001) docker     (121)     6137 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4898 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/
--rw-r--r--   0 runner    (1001) docker     (121)     3688 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/
--rw-r--r--   0 runner    (1001) docker     (121)    19345 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/browser.png
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/build_history.png
--rw-r--r--   0 runner    (1001) docker     (121)    27784 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/build_history_small.png
--rw-r--r--   0 runner    (1001) docker     (121)    25779 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/cancel.png
--rw-r--r--   0 runner    (1001) docker     (121)    22800 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/delete.png
--rw-r--r--   0 runner    (1001) docker     (121)    42366 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/drawing.png
--rw-r--r--   0 runner    (1001) docker     (121)    39619 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/force_refresh.png
--rw-r--r--   0 runner    (1001) docker     (121)     9597 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/frequency.png
--rw-r--r--   0 runner    (1001) docker     (121)     3041 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/icon_attributions.txt
--rw-r--r--   0 runner    (1001) docker     (121)    40204 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/lightbulb.png
--rw-r--r--   0 runner    (1001) docker     (121)     9430 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/log copy.png
--rw-r--r--   0 runner    (1001) docker     (121)     9430 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/log.png
--rw-r--r--   0 runner    (1001) docker     (121)     9346 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/metal_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    34528 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/painting.png
--rw-r--r--   0 runner    (1001) docker     (121)    43501 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/pan.png
--rw-r--r--   0 runner    (1001) docker     (121)    33820 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/refresh.png
--rw-r--r--   0 runner    (1001) docker     (121)    11236 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (121)    40237 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/sos.png
--rw-r--r--   0 runner    (1001) docker     (121)    26094 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/stack.png
--rw-r--r--   0 runner    (1001) docker     (121)    38061 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/support.png
--rw-r--r--   0 runner    (1001) docker     (121)     7995 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/component_widget_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     6648 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/component_widget_ui.ui
--rw-r--r--   0 runner    (1001) docker     (121)     8800 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/elements_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     7204 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/elements_ui.ui
--rw-r--r--   0 runner    (1001) docker     (121)     8518 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/elements_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     6756 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/endcap_hfss_gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     2902 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/endcap_hfss_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/endcap_hfss_ui.ui
--rw-r--r--   0 runner    (1001) docker     (121)     5550 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/endcap_q3d_gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/endcap_q3d_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/endcap_q3d_ui.ui
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/list_model_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    28730 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (121)    21812 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/main_window_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3229 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/main_window_rc.qrc
--rw-r--r--   0 runner    (1001) docker     (121)  3369083 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/main_window_rc_rc.py
--rw-r--r--   0 runner    (1001) docker     (121)    58356 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/main_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)    50560 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/main_window_ui.ui
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/net_list_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/net_list_ui.ui
--rw-r--r--   0 runner    (1001) docker     (121)     7656 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/net_list_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     8652 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/plot_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     7537 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/plot_window_ui.ui
--rw-r--r--   0 runner    (1001) docker     (121)     4065 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_gds_gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_gds_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     8133 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_gds_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     7074 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_gds_ui.ui
--rw-r--r--   0 runner    (1001) docker     (121)     3585 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_hfss_gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_hfss_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     6842 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_hfss_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     5930 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_hfss_ui.ui
--rw-r--r--   0 runner    (1001) docker     (121)     3401 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_q3d_gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     1768 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_q3d_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5773 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_q3d_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     5126 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_q3d_ui.ui
--rw-r--r--   0 runner    (1001) docker     (121)     2048 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/tree_view_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/utility/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5264 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/utility/_handle_qt_messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     3011 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/utility/_toolbox_qt.py
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/utility/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/all_components/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/all_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8539 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/all_components/table_model_all_components.py
--rw-r--r--   0 runner    (1001) docker     (121)    10590 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/all_components/table_view_all_components.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/bases/
--rw-r--r--   0 runner    (1001) docker     (121)     2988 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/bases/QWidget_PlaceholderText.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19583 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/bases/dict_tree_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2627 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/bases/expanding_toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/build_history/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/build_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/build_history/build_history_scroll_area.py
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/build_history/build_history_scroll_area_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/build_history/build_history_scroll_area_ui.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/model_view/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/model_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/model_view/tree_delegate_param_entry.py
--rw-r--r--   0 runner    (1001) docker     (121)    29213 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/model_view/tree_model_param_entry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/model_view/tree_view_param_entry.py
--rw-r--r--   0 runner    (1001) docker     (121)    19437 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/parameter_entry_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     7675 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/parameter_entry_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     4304 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/parameter_entry_window_ui.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/edit_component/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/edit_component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10692 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/edit_component/component_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     9281 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/edit_component/table_model_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/edit_component/table_view_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     4706 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/edit_component/tree_model_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/edit_component/tree_view_options.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/log_widget/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/log_widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15493 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/log_widget/log_metal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/plot_widget/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/plot_widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4590 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/plot_widget/plot_window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/qlibrary_display/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/qlibrary_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5677 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/qlibrary_display/delegate_qlibrary.py
--rw-r--r--   0 runner    (1001) docker     (121)     4254 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/qlibrary_display/file_model_qlibrary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2755 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/qlibrary_display/proxy_model_qlibrary.py
--rw-r--r--   0 runner    (1001) docker     (121)     3575 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/qlibrary_display/tree_view_qlibrary.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/add_delete_table_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     4192 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/add_delete_table_ui.ui
--rw-r--r--   0 runner    (1001) docker     (121)     2836 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/dialog_popup_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/dialog_popup_ui.ui
--rw-r--r--   0 runner    (1001) docker     (121)     2756 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/prop_val_table_gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     7509 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/prop_val_table_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4207 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/right_click_table_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/_is_design.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/
--rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/core/
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9575 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/core/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8863 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/core/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/em/
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/em/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9402 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/em/cpw_calculations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/em/kappa_calculation.py
--rw-r--r--   0 runner    (1001) docker     (121)    14147 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/em/transmission_fitting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/hamiltonian/
--rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/hamiltonian/HO_wavefunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/hamiltonian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5276 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/hamiltonian/states_energies.py
--rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/hamiltonian/transmon_CPB_analytic.py
--rw-r--r--   0 runner    (1001) docker     (121)     4988 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/hamiltonian/transmon_analytics.py
--rw-r--r--   0 runner    (1001) docker     (121)    12420 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/hamiltonian/transmon_charge_basis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    11684 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/energy_participation_ratio.py
--rw-r--r--   0 runner    (1001) docker     (121)    59135 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/lom_core_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/lom_extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/lom_time_evolution_sim.py
--rw-r--r--   0 runner    (1001) docker     (121)    27660 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/lumped_capacitive.py
--rw-r--r--   0 runner    (1001) docker     (121)     8730 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/lumped_oscillator_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/simulation/
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11191 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/simulation/eigenmode.py
--rw-r--r--   0 runner    (1001) docker     (121)     9061 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/simulation/lumped_elements.py
--rw-r--r--   0 runner    (1001) docker     (121)    11109 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/simulation/scattering_impedance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/sweep_and_optimize/
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/sweep_and_optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10405 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/sweep_and_optimize/sweeper.py
--rw-r--r--   0 runner    (1001) docker     (121)    55932 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/analyses/sweep_and_optimize/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (121)     4461 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/designs/
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/designs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    42150 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/designs/design_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6104 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/designs/design_flipchip.py
--rw-r--r--   0 runner    (1001) docker     (121)     5135 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/designs/design_planar.py
--rw-r--r--   0 runner    (1001) docker     (121)    11898 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/designs/interface_components.py
--rw-r--r--   0 runner    (1001) docker     (121)     7022 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/designs/net_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/draw/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/draw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17576 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/draw/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/draw/mpl.py
--rw-r--r--   0 runner    (1001) docker     (121)    29283 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/draw/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/qgeometries/
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qgeometries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30784 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qgeometries/qgeometries_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/
--rw-r--r--   0 runner    (1001) docker     (121)     4646 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/_template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/core/
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8936 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/core/_parsed_dynamic_attrs.py
--rw-r--r--   0 runner    (1001) docker     (121)    50811 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/core/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    30073 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/core/qroute.py
--rw-r--r--   0 runner    (1001) docker     (121)     4333 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/core/qubit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/couplers/
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/couplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7966 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/couplers/cap_n_interdigital_tee.py
--rw-r--r--   0 runner    (1001) docker     (121)     6168 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/couplers/coupled_line_tee.py
--rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/couplers/line_tee.py
--rw-r--r--   0 runner    (1001) docker     (121)     8590 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/couplers/tunable_coupler_01.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/lumped/
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/lumped/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6521 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/lumped/cap_3_interdigital.py
--rw-r--r--   0 runner    (1001) docker     (121)     7486 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/lumped/cap_n_interdigital.py
--rw-r--r--   0 runner    (1001) docker     (121)     5103 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/lumped/resonator_coil_rect.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/
--rw-r--r--   0 runner    (1001) docker     (121)     5651 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/JJ_Dolan.py
--rw-r--r--   0 runner    (1001) docker     (121)     4423 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/JJ_Manhattan.py
--rw-r--r--   0 runner    (1001) docker     (121)     5954 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/SQUID_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)    14485 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/Transmon_Interdigitated.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18686 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/star_qubit.py
--rw-r--r--   0 runner    (1001) docker     (121)     8578 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_concentric.py
--rw-r--r--   0 runner    (1001) docker     (121)     9009 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_cross.py
--rw-r--r--   0 runner    (1001) docker     (121)     4807 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_cross_fl.py
--rw-r--r--   0 runner    (1001) docker     (121)    11922 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_pocket.py
--rw-r--r--   0 runner    (1001) docker     (121)    11599 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_pocket_6.py
--rw-r--r--   0 runner    (1001) docker     (121)     7726 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_pocket_cl.py
--rw-r--r--   0 runner    (1001) docker     (121)    15358 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_pocket_teeth.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3139 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/circle_caterpillar.py
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/circle_raster.py
--rw-r--r--   0 runner    (1001) docker     (121)     2546 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/n_gon.py
--rw-r--r--   0 runner    (1001) docker     (121)     3585 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/n_square_spiral.py
--rw-r--r--   0 runner    (1001) docker     (121)     2185 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2686 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/rectangle_hollow.py
--rw-r--r--   0 runner    (1001) docker     (121)     2416 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/smiley_face.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/terminations/
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/terminations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6164 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/terminations/launchpad_wb.py
--rw-r--r--   0 runner    (1001) docker     (121)     6956 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/terminations/launchpad_wb_coupled.py
--rw-r--r--   0 runner    (1001) docker     (121)     6500 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/terminations/launchpad_wb_driven.py
--rw-r--r--   0 runner    (1001) docker     (121)     2473 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/terminations/open_to_ground.py
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/terminations/short_to_ground.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19812 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/anchored_path.py
--rw-r--r--   0 runner    (1001) docker     (121)    18308 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/framed_path.py
--rw-r--r--   0 runner    (1001) docker     (121)    20969 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/meandered.py
--rw-r--r--   0 runner    (1001) docker     (121)     9141 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/mixed_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     8919 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/straight_path.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/user_components/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/user_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/qlibrary/user_components/my_qcomponent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/
--rw-r--r--   0 runner    (1001) docker     (121)     2261 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_ansys/
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_ansys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    78816 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_ansys/ansys_renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)    52147 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_ansys/hfss_renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_ansys/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)    23903 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_ansys/q3d_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_base/
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16903 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_base/renderer_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3462 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_base/renderer_gui_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4003 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_base/rndr_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_base/rndr_export.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_gds/
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_gds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   104962 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_gds/gds_renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)    20727 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_gds/make_cheese.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4008 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/extensions/animated_text.py
--rw-r--r--   0 runner    (1001) docker     (121)    30789 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/mpl_canvas.py
--rw-r--r--   0 runner    (1001) docker     (121)    23950 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/mpl_interaction.py
--rw-r--r--   0 runner    (1001) docker     (121)    19334 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/mpl_renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)    12559 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/mpl_toolbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     4334 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/patch.py
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/renderers/setup_default.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4030 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/assertions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/custom_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/run_all_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    10049 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_analyses_1_inst_options.py
--rw-r--r--   0 runner    (1001) docker     (121)    34848 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_analyses_2_functionality.py
--rw-r--r--   0 runner    (1001) docker     (121)     8910 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_default_options.py
--rw-r--r--   0 runner    (1001) docker     (121)    19695 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_designs.py
--rw-r--r--   0 runner    (1001) docker     (121)    34032 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_draw.py
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_gui_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)    13146 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_qgeometries.py
--rw-r--r--   0 runner    (1001) docker     (121)    32090 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_qlibrary_1_instantiate.py
--rw-r--r--   0 runner    (1001) docker     (121)    38546 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_qlibrary_2_options.py
--rw-r--r--   0 runner    (1001) docker     (121)    26333 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_qlibrary_3_functionality.py
--rw-r--r--   0 runner    (1001) docker     (121)    20319 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_renderers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_speed.py
--rw-r--r--   0 runner    (1001) docker     (121)    12488 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_toolbox_metal.py
--rw-r--r--   0 runner    (1001) docker     (121)     6572 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/tests/test_toolbox_python.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/toolbox_metal/
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/toolbox_metal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4743 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/toolbox_metal/about.py
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/toolbox_metal/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/toolbox_metal/import_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/toolbox_metal/math_and_overrides.py
--rw-r--r--   0 runner    (1001) docker     (121)    15252 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/toolbox_metal/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal/toolbox_python/
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/toolbox_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4990 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/toolbox_python/_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/toolbox_python/attr_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     7251 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/toolbox_python/display.py
--rw-r--r--   0 runner    (1001) docker     (121)    20350 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/qiskit_metal/toolbox_python/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10531 2022-07-23 14:33:07.000000 qiskit_metal-0.1.2/qiskit_metal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12007 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/qiskit_metal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-23 14:33:07.000000 qiskit_metal-0.1.2/qiskit_metal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-07-23 14:33:07.000000 qiskit_metal-0.1.2/qiskit_metal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-23 14:33:07.000000 qiskit_metal-0.1.2/qiskit_metal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-23 14:33:08.000000 qiskit_metal-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-07-23 14:32:59.000000 qiskit_metal-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.289991 qiskit_metal-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-14 21:56:54.000000 qiskit_metal-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 21:56:54.000000 qiskit_metal-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-06-14 21:57:03.289991 qiskit_metal-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-06-14 21:56:54.000000 qiskit_metal-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.253991 qiskit_metal-0.1.5/qiskit_metal/
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.261991 qiskit_metal-0.1.5/qiskit_metal/_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.265991 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)    19345 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/browser.png
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/build_history.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27784 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/build_history_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25779 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/cancel.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42366 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/drawing.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39619 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/force_refresh.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/frequency.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/icon_attributions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    40204 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/lightbulb.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/log copy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/log.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/metal_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34528 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/painting.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43501 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/pan.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33820 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/refresh.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40237 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/sos.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26094 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/stack.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38061 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/support.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/component_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/component_widget_ui.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/elements_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/elements_ui.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/elements_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/endcap_hfss_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/endcap_hfss_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/endcap_hfss_ui.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/endcap_q3d_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/endcap_q3d_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/endcap_q3d_ui.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/list_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31429 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21812 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/main_window_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/main_window_rc.qrc
+-rw-r--r--   0 runner    (1001) docker     (123)  3369083 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/main_window_rc_rc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58356 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/main_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50560 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/main_window_ui.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/net_list_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/net_list_ui.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/net_list_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/plot_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/plot_window_ui.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_gds_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_gds_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_gds_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_gds_ui.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_hfss_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_hfss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_hfss_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_hfss_ui.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_q3d_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_q3d_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_q3d_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_q3d_ui.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/tree_view_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.265991 qiskit_metal-0.1.5/qiskit_metal/_gui/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/utility/_handle_qt_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/utility/_toolbox_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/utility/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.265991 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.265991 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/all_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/all_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/all_components/table_model_all_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/all_components/table_view_all_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.265991 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/bases/QWidget_PlaceholderText.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19583 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/bases/dict_tree_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/bases/expanding_toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.269991 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/build_history/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/build_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/build_history/build_history_scroll_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/build_history/build_history_scroll_area_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/build_history/build_history_scroll_area_ui.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.269991 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.269991 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/model_view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/model_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/model_view/tree_delegate_param_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29213 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/model_view/tree_model_param_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/model_view/tree_view_param_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19437 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/parameter_entry_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/parameter_entry_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/parameter_entry_window_ui.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.269991 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/edit_component/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/edit_component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/edit_component/component_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/edit_component/table_model_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/edit_component/table_view_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/edit_component/tree_model_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/edit_component/tree_view_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.269991 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/log_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/log_widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/log_widget/log_metal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.269991 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/plot_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/plot_widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/plot_widget/plot_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.269991 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/qlibrary_display/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/qlibrary_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/qlibrary_display/delegate_qlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/qlibrary_display/file_model_qlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/qlibrary_display/proxy_model_qlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/qlibrary_display/tree_view_qlibrary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.273991 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/add_delete_table_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/add_delete_table_ui.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/dialog_popup_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/dialog_popup_ui.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/prop_val_table_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/prop_val_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/right_click_table_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/_is_design.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.273991 qiskit_metal-0.1.5/qiskit_metal/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.273991 qiskit_metal-0.1.5/qiskit_metal/analyses/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/core/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.273991 qiskit_metal-0.1.5/qiskit_metal/analyses/em/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/em/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/em/cpw_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/em/kappa_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/em/transmission_fitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.273991 qiskit_metal-0.1.5/qiskit_metal/analyses/hamiltonian/
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/hamiltonian/HO_wavefunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/hamiltonian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/hamiltonian/states_energies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/hamiltonian/transmon_CPB_analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/hamiltonian/transmon_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/hamiltonian/transmon_charge_basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.273991 qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/energy_participation_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59135 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/lom_core_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/lom_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/lom_time_evolution_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28064 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/lumped_capacitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/lumped_oscillator_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.273991 qiskit_metal-0.1.5/qiskit_metal/analyses/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/simulation/eigenmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/simulation/lumped_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/simulation/scattering_impedance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.273991 qiskit_metal-0.1.5/qiskit_metal/analyses/sweep_and_optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/sweep_and_optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/sweep_and_optimize/sweeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55932 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/analyses/sweep_and_optimize/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.277991 qiskit_metal-0.1.5/qiskit_metal/designs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/designs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42150 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/designs/design_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/designs/design_flipchip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/designs/design_multiplanar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/designs/design_planar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/designs/interface_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/designs/net_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.277991 qiskit_metal-0.1.5/qiskit_metal/draw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/draw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17576 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/draw/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/draw/mpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29799 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/draw/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.277991 qiskit_metal-0.1.5/qiskit_metal/qgeometries/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qgeometries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32209 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qgeometries/qgeometries_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.277991 qiskit_metal-0.1.5/qiskit_metal/qlibrary/
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.277991 qiskit_metal-0.1.5/qiskit_metal/qlibrary/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/core/_parsed_dynamic_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50837 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/core/design_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30073 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/core/qroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/core/qubit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.277991 qiskit_metal-0.1.5/qiskit_metal/qlibrary/couplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/couplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/couplers/cap_n_interdigital_tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/couplers/coupled_line_tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/couplers/line_tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/couplers/tunable_coupler_01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/couplers/tunable_coupler_02.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.277991 qiskit_metal-0.1.5/qiskit_metal/qlibrary/lumped/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/lumped/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/lumped/cap_3_interdigital.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/lumped/cap_n_interdigital.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/lumped/resonator_coil_rect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.277991 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/JJ_Dolan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/JJ_Manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/SQUID_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/Transmon_Interdigitated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/star_qubit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_concentric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_concentric_type_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_cross_fl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_pocket_6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_pocket_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_pocket_teeth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.281991 qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/circle_caterpillar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/circle_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/n_gon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/n_square_spiral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/rectangle_hollow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/smiley_face.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.281991 qiskit_metal-0.1.5/qiskit_metal/qlibrary/terminations/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/terminations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/terminations/launchpad_wb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/terminations/launchpad_wb_coupled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/terminations/launchpad_wb_driven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/terminations/open_to_ground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/terminations/short_to_ground.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.281991 qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19812 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/anchored_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18308 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/framed_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20969 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/meandered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/mixed_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/straight_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.281991 qiskit_metal-0.1.5/qiskit_metal/qlibrary/user_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/user_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/qlibrary/user_components/my_qcomponent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.281991 qiskit_metal-0.1.5/qiskit_metal/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.281991 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78869 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys/ansys_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52147 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys/hfss_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29919 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys/q3d_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.281991 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys_pyaedt/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys_pyaedt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41304 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys_pyaedt/hfss_renderer_aedt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30745 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys_pyaedt/hfss_renderer_drivenmodal_aedt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys_pyaedt/hfss_renderer_eigenmode_aedt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48351 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys_pyaedt/pyaedt_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23647 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys_pyaedt/q3d_renderer_aedt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.281991 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_base/renderer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_base/renderer_gui_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_base/rndr_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_base/rndr_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.281991 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_elmer/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_elmer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_elmer/elmer_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31382 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_elmer/elmer_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24351 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_elmer/elmer_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.285991 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_gds/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_gds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106259 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_gds/gds_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_gds/make_cheese.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.285991 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_gmsh/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_gmsh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59073 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_gmsh/gmsh_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13527 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_gmsh/gmsh_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.285991 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.285991 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/extensions/animated_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30789 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/mpl_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23966 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/mpl_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19334 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/mpl_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/mpl_toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/setup_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/renderers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.285991 qiskit_metal-0.1.5/qiskit_metal/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/custom_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/run_all_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_analyses_1_inst_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34848 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_analyses_2_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_default_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19820 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_designs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33961 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_gui_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_qgeometries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32090 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_qlibrary_1_instantiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38763 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_qlibrary_2_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26333 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_qlibrary_3_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42269 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_toolbox_metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/tests/test_toolbox_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.285991 qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/bounds_for_path_and_poly_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/import_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/layer_stack_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/math_and_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.289991 qiskit_metal-0.1.5/qiskit_metal/toolbox_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/toolbox_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/toolbox_python/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/toolbox_python/attr_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/toolbox_python/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/qiskit_metal/toolbox_python/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:57:03.257991 qiskit_metal-0.1.5/qiskit_metal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-06-14 21:57:03.000000 qiskit_metal-0.1.5/qiskit_metal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-06-14 21:57:03.000000 qiskit_metal-0.1.5/qiskit_metal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:57:03.000000 qiskit_metal-0.1.5/qiskit_metal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-14 21:57:03.000000 qiskit_metal-0.1.5/qiskit_metal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 21:57:03.000000 qiskit_metal-0.1.5/qiskit_metal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:57:03.289991 qiskit_metal-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-14 21:56:55.000000 qiskit_metal-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qiskit_metal-0.1.2/PKG-INFO` & `qiskit_metal-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,147 +1,146 @@
 Metadata-Version: 2.1
 Name: qiskit_metal
-Version: 0.1.2
+Version: 0.1.5
 Summary: Qiskit Metal | for quantum device design & analysis
 Home-page: https://github.com/Qiskit/qiskit-metal
 Author: Qiskit Metal Development Team
 Author-email: qiskit@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-metal/issues
 Project-URL: Documentation, https://qiskit.org/documentation/metal
 Project-URL: Source Code, https://github.com/Qiskit/qiskit-metal
-Description: # Qiskit Metal 
-        [![License](https://img.shields.io/github/license/Qiskit/qiskit-metal.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)<!--- long-description-skip-begin -->[![Release](https://img.shields.io/github/release/Qiskit/qiskit-metal.svg?style=popout-square)](https://github.com/Qiskit/qiskit-metal/releases)<!--- long-description-skip-begin -->[![join slack](https://img.shields.io/badge/slack-@qiskit-yellow.svg?logo=slack&style=popout-square)](https://ibm.co/joinqiskitslack)[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4618153.svg)](https://doi.org/10.5281/zenodo.4618153)
-         
-        >![Welcome to Qiskit Metal!](https://raw.githubusercontent.com/Qiskit/qiskit-metal/main/docs/images/zkm_banner.png 'Welcome to Qiskit Metal')
-        > Qiskit Metal is an open-source framework for engineers and scientists to design superconducting quantum devices with ease.
-        
-        ## Installation
-        If you are interested in customizing your experience, or if you are unable to install qiskit-metal using the `pip install` instructions below, consider installing directly the source code, following the instructions in the [documentation](https://qiskit.org/documentation/metal/installation.html) and/or the [installation instructions for developers](https://github.com/Qiskit/qiskit-metal/blob/main/README_developers.md).
-        
-        For normal use, please continue reading.
-        
-        ### The Qiskit Metal deployed package
-        You can install Qiskit Metal via the pip tool (a python package manager).
-        ```bash
-        pip install qiskit-metal
-        ```
-        PIP will handle most of the dependencies automatically and you will always install the latest (and well-tested) version of the package.
-        
-        Some of the dependencies, namely pyside2 and geopandas, might require manual installation, depending on your specific system compatibility. If you encounter installation or execution errors, please refer first to the [FAQ](https://qiskit.org/documentation/metal/faq.html).
-        
-        We recommend to install qiskit-metal in a conda environment or venv, to prevent version conflicts with pre-existing package versions.
-        
-        ### Jupyter Notebook
-        At this time, we recommend using Jupyter notebook/lab to be able to access all the Qiskit Metal features. Jupyter is not installed with the default dependencies, to accommodate those users intending to utilize a centralized or customized installation.
-        
-        If you require a fresh installation, please refer to either [anaconda.org](https://anaconda.org/) or [jupyter.org](https://jupyter.org/install).
-        
-        Unless you installed the entire `jupyter` package in your current environment, do not forget to create the appropriate kernel to make the environment (thus qiskit-metal) available to jupyter (instructions in the [FAQ](https://qiskit.org/documentation/metal/faq.html))
-        
-        ## Creating Your First Quantum Component in Qiskit Metal:
-        Now that Qiskit Metal is installed, it's time to begin working with it.
-        We are ready to try out a quantum chip example, which is simulated locally using
-        the Qiskit MetalGUI element. This is a simple example that makes a qubit.
-        ```
-        $ python
-        ```
-        ```python
-        >>> from qiskit_metal import designs, draw, MetalGUI, Dict, open_docs
-        >>> design = designs.DesignPlanar()
-        >>> design.overwrite_enabled = True
-        >>> design.chips.main
-        >>> design.chips.main.size.size_x = '11mm'
-        >>> design.chips.main.size.size_y = '9mm'
-        >>> gui = MetalGUI(design)
-        ```
-        #### Launch the Qiskit Metal GUI to interactively view, edit, and simulate a QDesign:
-        ```python
-        >>> gui = MetalGUI(design)
-        ```
-        #### Let's create a new qubit (a transmon) by creating an object of this class.
-        ```python
-        >>> from qiskit_metal.qlibrary.qubits.transmon_pocket import TransmonPocket
-        >>> q1 = TransmonPocket(design, 'Q1', options=dict(connection_pads=dict(a=dict())))
-        >>> gui.rebuild()
-        >>> gui.edit_component('Q1')
-        >>> gui.autoscale()
-        ```
-        #### Change options.
-        ```python
-        >>> q1.options.pos_x = '0.5 mm'
-        >>> q1.options.pos_y = '0.25 mm'
-        >>> q1.options.pad_height = '90um'
-        >>> q1.options.pad_width  = '455um'
-        >>> q1.options.pad_gap    = '30 um'
-        ```
-        #### Update the component geometry after changing the options.
-        ```python
-        >>> gui.rebuild()
-        ```
-        ![Example_Image!](https://raw.githubusercontent.com/Qiskit/qiskit-metal/main/docs/images/1_1_Birds_eye_view_of_Qiskit_Metal_example_image.jpg 'Example_Image') 
-        #### Get a list of all the qcomponents in QDesign and then zoom on them.
-        ```python
-        >>> all_component_names = design.components.keys()
-        >>> gui.zoom_on_components(all_component_names)
-        ```
-        #### Closing the Qiskit Metal GUI.
-        ```python
-        >>> gui.main_window.close()
-        ```
-        
-        A script is available [here](https://qiskit.org/documentation/metal/tut/overview/1.1%20High%20Level%20Demo%20of%20Qiskit%20Metal.html), where we also show the overview of Qiskit Metal.
-        
-        ## Community and Support
-        
-        #### Watch the recorded tutorials 
-        [![Video Tutorials](https://img.shields.io/badge/youtube-Video_Tutorials-red.svg?logo=youtube)](https://youtube.com/playlist?list=PLOFEBzvs-VvqHl5ZqVmhB_FcSqmLufsjb)
-        
-        The streaming will also be recorded and made available [here](https://www.youtube.com/playlist?list=PLOFEBzvs-VvqHl5ZqVmhB_FcSqmLufsjb) for offline review.
-        
-        #### Take part in the live tutorials and discussion
-        Through June 2021 we are offering live tutorials and Q&A. [Sign up](https://airtable.com/shrxQEgKqZCf319F3) to receive an invite to the upcoming sessions.  The streaming will also be recorded and made available for offline review.  Find [here](https://github.com/Qiskit/qiskit-metal/blob/main/README_Tutorials.md) more details on schedule and use the Slack channel to give us feedback and to request the most relevant content to you.
-        
-        #### Get help: Slack 
-        [![join slack](https://img.shields.io/badge/slack-blue.svg?logo=slack)](https://ibm.co/joinqiskitslack)
-        
-        Use the slack channel.  Join [qiskit slack](https://ibm.co/joinqiskitslack) and then join the `#metal` channel to communicate with the developers and other participants.  You may also use this channel to inquire about collaborations.
-        
-        ## Contribution Guidelines
-        If you'd like to contribute to Qiskit Metal, please take a look at our
-        [contribution guidelines](https://github.com/Qiskit/qiskit-metal/blob/main/CONTRIBUTING.md). This project adheres to Qiskit's [code of conduct](https://github.com/Qiskit/qiskit-metal/blob/main/CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.
-        We use [GitHub issues](https://github.com/Qiskit/qiskit-metal/issues) for tracking requests and bugs. Please
-        [join the Qiskit Slack community](https://ibm.co/joinqiskitslack)
-        and use our [Qiskit Slack channel](https://qiskit.slack.com) for discussion and simple questions.
-        For questions that are more suited for a forum we use the Qiskit tag in the [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
-        ## Next Steps
-        Now you're set up and ready to check out some of the other examples from our
-        [Qiskit Metal Tutorials](https://github.com/Qiskit/qiskit-metal/blob/main/tutorials/) repository or [Qiskit Metal Documentation](https://qiskit.org/documentation/metal/tut/).
-        ## Authors and Citation
-        Qiskit Metal is the work of [many people](https://github.com/Qiskit/qiskit-metal/pulse/monthly) who contribute to the project at different levels. Metal was conceived and developed by [Zlatko Minev](https://www.zlatko-minev.com) at IBM; then co-led with Thomas McConkey. If you use Qiskit Metal, please cite as per the included [BibTeX file](https://github.com/Qiskit/qiskit-metal/blob/main/Qiskit_Metal.bib). For icon attributions, see [here](https://github.com/Qiskit/qiskit-metal/blob/main/qiskit_metal/_gui/_imgs/icon_attributions.txt).
-        ## Changelog and Release Notes
-        The changelog provides a quick overview of notable changes for a given release.
-        
-        The changelog for a particular release can be found in the correspondent Github release page. For example, you can find the changelog for the `0.0.4` release [here](https://github.com/Qiskit/qiskit-metal/releases/tag/0.0.4)
-        
-        The changelog for all releases can be found in the release page: [![Releases](https://img.shields.io/github/release/Qiskit/qiskit-metal.svg?style=popout-square)](https://github.com/Qiskit/qiskit-metal/releases)
-        
-        Additionally, as part of each release detailed release notes are written to document in detail what has changed as part of a release. This includes any documentation on potential breaking changes on upgrade and new features.
-        
-        ## License
-        [Apache License 2.0](https://github.com/Qiskit/qiskit-metal/blob/main/LICENSE.txt)
-        
 Keywords: qiskit sdk quantum eda
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Qiskit Metal 
+[![License](https://img.shields.io/github/license/Qiskit/qiskit-metal.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)<!--- long-description-skip-begin -->[![Release](https://img.shields.io/github/release/Qiskit/qiskit-metal.svg?style=popout-square)](https://github.com/Qiskit/qiskit-metal/releases)<!--- long-description-skip-begin -->[![join slack](https://img.shields.io/badge/slack-@qiskit-yellow.svg?logo=slack&style=popout-square)](https://qisk.it/join-slack)[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4618153.svg)](https://doi.org/10.5281/zenodo.4618153)
+ 
+>![Welcome to Qiskit Metal!](https://raw.githubusercontent.com/Qiskit/qiskit-metal/main/docs/images/zkm_banner.png 'Welcome to Qiskit Metal')
+> Qiskit Metal is an open-source framework for engineers and scientists to design superconducting quantum devices with ease.
+
+## Installation
+If you are interested in customizing your experience, or if you are unable to install qiskit-metal using the `pip install` instructions below, consider installing directly the source code, following the instructions in the [documentation](https://qiskit.org/documentation/metal/installation.html) and/or the [installation instructions for developers](https://github.com/Qiskit/qiskit-metal/blob/main/README_developers.md).
+
+For normal use, please continue reading.
+
+### The Qiskit Metal deployed package
+You can install Qiskit Metal via the pip tool (a python package manager).
+```bash
+pip install qiskit-metal
+```
+PIP will handle most of the dependencies automatically and you will always install the latest (and well-tested) version of the package.
+
+Some of the dependencies, namely pyside2 and geopandas, might require manual installation, depending on your specific system compatibility. If you encounter installation or execution errors, please refer first to the [FAQ](https://qiskit.org/documentation/metal/faq.html).
+
+We recommend to install qiskit-metal in a conda environment or venv, to prevent version conflicts with pre-existing package versions.
+
+### Jupyter Notebook
+At this time, we recommend using Jupyter notebook/lab to be able to access all the Qiskit Metal features. Jupyter is not installed with the default dependencies, to accommodate those users intending to utilize a centralized or customized installation.
+
+If you require a fresh installation, please refer to either [anaconda.org](https://anaconda.org/) or [jupyter.org](https://jupyter.org/install).
+
+Unless you installed the entire `jupyter` package in your current environment, do not forget to create the appropriate kernel to make the environment (thus qiskit-metal) available to jupyter (instructions in the [FAQ](https://qiskit.org/documentation/metal/faq.html))
+
+## Creating Your First Quantum Component in Qiskit Metal:
+Now that Qiskit Metal is installed, it's time to begin working with it.
+We are ready to try out a quantum chip example, which is simulated locally using
+the Qiskit MetalGUI element. This is a simple example that makes a qubit.
+```
+$ python
+```
+```python
+>>> from qiskit_metal import designs, draw, MetalGUI, Dict, open_docs
+>>> design = designs.DesignPlanar()
+>>> design.overwrite_enabled = True
+>>> design.chips.main
+>>> design.chips.main.size.size_x = '11mm'
+>>> design.chips.main.size.size_y = '9mm'
+>>> gui = MetalGUI(design)
+```
+#### Launch the Qiskit Metal GUI to interactively view, edit, and simulate a QDesign:
+```python
+>>> gui = MetalGUI(design)
+```
+#### Let's create a new qubit (a transmon) by creating an object of this class.
+```python
+>>> from qiskit_metal.qlibrary.qubits.transmon_pocket import TransmonPocket
+>>> q1 = TransmonPocket(design, 'Q1', options=dict(connection_pads=dict(a=dict())))
+>>> gui.rebuild()
+>>> gui.edit_component('Q1')
+>>> gui.autoscale()
+```
+#### Change options.
+```python
+>>> q1.options.pos_x = '0.5 mm'
+>>> q1.options.pos_y = '0.25 mm'
+>>> q1.options.pad_height = '90um'
+>>> q1.options.pad_width  = '455um'
+>>> q1.options.pad_gap    = '30 um'
+```
+#### Update the component geometry after changing the options.
+```python
+>>> gui.rebuild()
+```
+![Example_Image!](https://raw.githubusercontent.com/Qiskit/qiskit-metal/main/docs/images/1_1_Birds_eye_view_of_Qiskit_Metal_example_image.jpg 'Example_Image') 
+#### Get a list of all the qcomponents in QDesign and then zoom on them.
+```python
+>>> all_component_names = design.components.keys()
+>>> gui.zoom_on_components(all_component_names)
+```
+#### Closing the Qiskit Metal GUI.
+```python
+>>> gui.main_window.close()
+```
+
+A script is available [here](https://qiskit.org/documentation/metal/tut/overview/1.1%20High%20Level%20Demo%20of%20Qiskit%20Metal.html), where we also show the overview of Qiskit Metal.
+
+## Community and Support
+
+#### Watch the recorded tutorials 
+[![Video Tutorials](https://img.shields.io/badge/youtube-Video_Tutorials-red.svg?logo=youtube)](https://youtube.com/playlist?list=PLOFEBzvs-VvqHl5ZqVmhB_FcSqmLufsjb)
+
+The streaming will also be recorded and made available [here](https://www.youtube.com/playlist?list=PLOFEBzvs-VvqHl5ZqVmhB_FcSqmLufsjb) for offline review.
+
+#### Take part in the live tutorials and discussion
+Through June 2021 we are offering live tutorials and Q&A. [Sign up](https://airtable.com/shrxQEgKqZCf319F3) to receive an invite to the upcoming sessions.  The streaming will also be recorded and made available for offline review.  Find [here](https://github.com/Qiskit/qiskit-metal/blob/main/README_Tutorials.md) more details on schedule and use the Slack channel to give us feedback and to request the most relevant content to you.
+
+#### Get help: Slack 
+[![join slack](https://img.shields.io/badge/slack-blue.svg?logo=slack)](https://qisk.it/join-slack)
+
+Use the slack channel.  Join [qiskit slack](https://qisk.it/join-slack) and then join the `#metal` channel to communicate with the developers and other participants.  You may also use this channel to inquire about collaborations.
+
+## Contribution Guidelines
+If you'd like to contribute to Qiskit Metal, please take a look at our
+[contribution guidelines](https://github.com/Qiskit/qiskit-metal/blob/main/CONTRIBUTING.md). This project adheres to Qiskit's [code of conduct](https://github.com/Qiskit/qiskit-metal/blob/main/CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.
+We use [GitHub issues](https://github.com/Qiskit/qiskit-metal/issues) for tracking requests and bugs. Please
+[join the Qiskit Slack community](https://qisk.it/join-slack)
+and use our [Qiskit Slack channel](https://qiskit.slack.com) for discussion and simple questions.
+For questions that are more suited for a forum we use the Qiskit tag in the [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
+## Next Steps
+Now you're set up and ready to check out some of the other examples from our
+[Qiskit Metal Tutorials](https://github.com/Qiskit/qiskit-metal/blob/main/tutorials/) repository or [Qiskit Metal Documentation](https://qiskit.org/documentation/metal/tut/).
+## Authors and Citation
+Qiskit Metal is the work of [many people](https://github.com/Qiskit/qiskit-metal/pulse/monthly) who contribute to the project at different levels. Metal was conceived and developed by [Zlatko Minev](https://www.zlatko-minev.com) at IBM; then co-led with Thomas McConkey. If you use Qiskit Metal, please cite as per the included [BibTeX file](https://github.com/Qiskit/qiskit-metal/blob/main/Qiskit_Metal.bib). For icon attributions, see [here](https://github.com/Qiskit/qiskit-metal/blob/main/qiskit_metal/_gui/_imgs/icon_attributions.txt).
+## Changelog and Release Notes
+The changelog provides a quick overview of notable changes for a given release.
+
+The changelog for a particular release can be found in the correspondent Github release page. For example, you can find the changelog for the `0.0.4` release [here](https://github.com/Qiskit/qiskit-metal/releases/tag/0.0.4)
+
+The changelog for all releases can be found in the release page: [![Releases](https://img.shields.io/github/release/Qiskit/qiskit-metal.svg?style=popout-square)](https://github.com/Qiskit/qiskit-metal/releases)
+
+Additionally, as part of each release detailed release notes are written to document in detail what has changed as part of a release. This includes any documentation on potential breaking changes on upgrade and new features.
+
+## License
+[Apache License 2.0](https://github.com/Qiskit/qiskit-metal/blob/main/LICENSE.txt)
```

### Comparing `qiskit_metal-0.1.2/README.md` & `qiskit_metal-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Qiskit Metal 
-[![License](https://img.shields.io/github/license/Qiskit/qiskit-metal.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)<!--- long-description-skip-begin -->[![Release](https://img.shields.io/github/release/Qiskit/qiskit-metal.svg?style=popout-square)](https://github.com/Qiskit/qiskit-metal/releases)<!--- long-description-skip-begin -->[![join slack](https://img.shields.io/badge/slack-@qiskit-yellow.svg?logo=slack&style=popout-square)](https://ibm.co/joinqiskitslack)[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4618153.svg)](https://doi.org/10.5281/zenodo.4618153)
+[![License](https://img.shields.io/github/license/Qiskit/qiskit-metal.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)<!--- long-description-skip-begin -->[![Release](https://img.shields.io/github/release/Qiskit/qiskit-metal.svg?style=popout-square)](https://github.com/Qiskit/qiskit-metal/releases)<!--- long-description-skip-begin -->[![join slack](https://img.shields.io/badge/slack-@qiskit-yellow.svg?logo=slack&style=popout-square)](https://qisk.it/join-slack)[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4618153.svg)](https://doi.org/10.5281/zenodo.4618153)
  
 >![Welcome to Qiskit Metal!](https://raw.githubusercontent.com/Qiskit/qiskit-metal/main/docs/images/zkm_banner.png 'Welcome to Qiskit Metal')
 > Qiskit Metal is an open-source framework for engineers and scientists to design superconducting quantum devices with ease.
 
 ## Installation
 If you are interested in customizing your experience, or if you are unable to install qiskit-metal using the `pip install` instructions below, consider installing directly the source code, following the instructions in the [documentation](https://qiskit.org/documentation/metal/installation.html) and/or the [installation instructions for developers](https://github.com/Qiskit/qiskit-metal/blob/main/README_developers.md).
 
@@ -87,23 +87,23 @@
 
 The streaming will also be recorded and made available [here](https://www.youtube.com/playlist?list=PLOFEBzvs-VvqHl5ZqVmhB_FcSqmLufsjb) for offline review.
 
 #### Take part in the live tutorials and discussion
 Through June 2021 we are offering live tutorials and Q&A. [Sign up](https://airtable.com/shrxQEgKqZCf319F3) to receive an invite to the upcoming sessions.  The streaming will also be recorded and made available for offline review.  Find [here](https://github.com/Qiskit/qiskit-metal/blob/main/README_Tutorials.md) more details on schedule and use the Slack channel to give us feedback and to request the most relevant content to you.
 
 #### Get help: Slack 
-[![join slack](https://img.shields.io/badge/slack-blue.svg?logo=slack)](https://ibm.co/joinqiskitslack)
+[![join slack](https://img.shields.io/badge/slack-blue.svg?logo=slack)](https://qisk.it/join-slack)
 
-Use the slack channel.  Join [qiskit slack](https://ibm.co/joinqiskitslack) and then join the `#metal` channel to communicate with the developers and other participants.  You may also use this channel to inquire about collaborations.
+Use the slack channel.  Join [qiskit slack](https://qisk.it/join-slack) and then join the `#metal` channel to communicate with the developers and other participants.  You may also use this channel to inquire about collaborations.
 
 ## Contribution Guidelines
 If you'd like to contribute to Qiskit Metal, please take a look at our
 [contribution guidelines](https://github.com/Qiskit/qiskit-metal/blob/main/CONTRIBUTING.md). This project adheres to Qiskit's [code of conduct](https://github.com/Qiskit/qiskit-metal/blob/main/CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.
 We use [GitHub issues](https://github.com/Qiskit/qiskit-metal/issues) for tracking requests and bugs. Please
-[join the Qiskit Slack community](https://ibm.co/joinqiskitslack)
+[join the Qiskit Slack community](https://qisk.it/join-slack)
 and use our [Qiskit Slack channel](https://qiskit.slack.com) for discussion and simple questions.
 For questions that are more suited for a forum we use the Qiskit tag in the [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
 ## Next Steps
 Now you're set up and ready to check out some of the other examples from our
 [Qiskit Metal Tutorials](https://github.com/Qiskit/qiskit-metal/blob/main/tutorials/) repository or [Qiskit Metal Documentation](https://qiskit.org/documentation/metal/tut/).
 ## Authors and Citation
 Qiskit Metal is the work of [many people](https://github.com/Qiskit/qiskit-metal/pulse/monthly) who contribute to the project at different levels. Metal was conceived and developed by [Zlatko Minev](https://www.zlatko-minev.com) at IBM; then co-led with Thomas McConkey. If you use Qiskit Metal, please cite as per the included [BibTeX file](https://github.com/Qiskit/qiskit-metal/blob/main/Qiskit_Metal.bib). For icon attributions, see [here](https://github.com/Qiskit/qiskit-metal/blob/main/qiskit_metal/_gui/_imgs/icon_attributions.txt).
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 # pylint: disable=wrong-import-order
 # pylint: disable=wrong-import-position
 """Qiskit Metal"""
-__version__ = '0.1.2'
+__version__ = '0.1.5'
 __license__ = "Apache 2.0"
 __copyright__ = 'Copyright IBM 2019-2020'
 __author__ = 'Zlatko Minev, Thomas McConkey, and them IBM Quantum Team'
 __status__ = "Development"
 
 ###########################################################################
 ### Windows OS catch for library geopandas not installed with setup.py
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_defaults.py` & `qiskit_metal-0.1.5/qiskit_metal/_defaults.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/browser.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/browser.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/build_history.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/build_history.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/build_history_small.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/build_history_small.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/cancel.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/cancel.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/delete.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/delete.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/drawing.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/drawing.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/force_refresh.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/force_refresh.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/frequency.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/frequency.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/icon_attributions.txt` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/icon_attributions.txt`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/lightbulb.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/lightbulb.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/log copy.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/log copy.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/log.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/log.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/metal_logo.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/metal_logo.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/painting.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/painting.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/pan.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/pan.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/refresh.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/refresh.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/screenshot.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/screenshot.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/sos.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/sos.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/stack.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/stack.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/_imgs/support.png` & `qiskit_metal-0.1.5/qiskit_metal/_gui/_imgs/support.png`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/component_widget_ui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/component_widget_ui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/component_widget_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/component_widget_ui.ui`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/elements_ui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/elements_ui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/elements_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/elements_ui.ui`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/elements_window.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/elements_window.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/endcap_hfss_gui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/endcap_hfss_gui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/endcap_hfss_ui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/endcap_hfss_ui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/endcap_hfss_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/endcap_hfss_ui.ui`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/endcap_q3d_gui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/endcap_q3d_gui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/endcap_q3d_ui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/endcap_q3d_ui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/endcap_q3d_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/endcap_q3d_ui.ui`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/list_model_base.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/list_model_base.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/main_window.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/main_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -556,24 +556,48 @@
         dock.show()
         dock.setMaximumHeight(99999)
 
     def _setup_elements_widget(self):
         """Create main Window Elements Widget."""
         self.elements_win = ElementsWindow(self, self.main_window)
 
+        # Component filter
         self.ui.tabQGeometry.sort_model = QSortFilterProxyModel()
         self.ui.tabQGeometry.sort_model.setSourceModel(self.elements_win.model)
+        self.ui.tabQGeometry.sort_model.setFilterKeyColumn(1)
 
         self.elements_win.ui.tableElements.setModel(
             self.ui.tabQGeometry.sort_model)
         self.elements_win.ui.tableElements.setSortingEnabled(True)
 
+        # Add a text changed event to the QGeometry/Component/Layer text boxes
+        self.elements_win.ui.lineEdit.textChanged.connect(
+            self.elements_lineEdit_onChanged)
+        self.elements_win.ui.lineEdit_2.textChanged.connect(
+            self.elements_lineEdit_2_onChanged)
+
         # Add to the tabbed main view
         self.ui.tabQGeometry.layout().addWidget(self.elements_win)
 
+    def elements_lineEdit_onChanged(self, text):
+        """ Text changed event for QGeometry/Component text box
+        Args:
+            text: Text typed in the filter box.
+        """
+        self.ui.tabQGeometry.sort_model.setFilterKeyColumn(1)
+        self.ui.tabQGeometry.sort_model.setFilterWildcard(text)
+
+    def elements_lineEdit_2_onChanged(self, text):
+        """ Text changed event for QGeometry/Layer text box
+        Args:
+            text: Text typed in the filter box.
+        """
+        self.ui.tabQGeometry.sort_model.setFilterKeyColumn(3)
+        self.ui.tabQGeometry.sort_model.setFilterWildcard(text)
+
     def _setup_net_list_widget(self):
         """Create main Window Elements Widget."""
         self.net_list_win = NetListWindow(self, self.main_window)
 
         self.ui.tabNetList.sort_model = QSortFilterProxyModel()
         self.ui.tabNetList.sort_model.setSourceModel(self.net_list_win.model)
 
@@ -589,15 +613,33 @@
 
         Table model that shows the summary of the components of a design
         in a table with their names, classes, and modules
         """
         model = QTableModel_AllComponents(self,
                                           logger=self.logger,
                                           tableView=self.ui.tableComponents)
-        self.ui.tableComponents.setModel(model)
+        # Add Sort/Filter logic to the components table
+        self.ui.proxyModel = QSortFilterProxyModel()
+        self.ui.proxyModel.setSourceModel(model)
+
+        # search all columns
+        self.ui.proxyModel.setFilterKeyColumn(-1)
+        self.ui.tableComponents.setSortingEnabled(True)
+        self.ui.tableComponents.setModel(self.ui.proxyModel)
+
+        # Add a text changed event to the filter text box
+        self.ui.filter_text_design.textChanged.connect(
+            self.filter_text_design_onChanged)
+
+    def filter_text_design_onChanged(self, text):
+        """ Text changed event for filter_text_design
+        Args:
+            text: Text typed in the filter box.
+        """
+        self.ui.proxyModel.setFilterWildcard(text)
 
     def _create_new_component_object_from_qlibrary(self, full_path: str):
         """
         Must be defined outside of _setup_library_widget to ensure self == MetalGUI and will retain opened ScrollArea
 
         Args:
             relative_index: QModelIndex of the desired QComponent file in the Qlibrary GUI display
@@ -635,14 +677,16 @@
 
         dock.library_model.setRootPath(self.QLIBRARY_ROOT)
 
         # QSortFilterProxyModel
         #QSortFilterProxyModel: sorting items, filtering out items, or both.  maps the original model indexes to new indexes, allows a given source model to be restructured as far as views are concerned without requiring any transformations on the underlying data, and without duplicating the data in memory.
         dock.proxy_library_model = LibraryFileProxyModel()
         dock.proxy_library_model.setSourceModel(dock.library_model)
+        dock.proxy_library_model.setFilterCaseSensitivity(Qt.CaseInsensitive)
+        dock.proxy_library_model.setRecursiveFilteringEnabled(True)
 
         # --------------------------------------------------
         # View
         view = self.ui.dockLibrary_tree_view
 
         view.setModel(dock.proxy_library_model)
         view.setRootIndex(
@@ -664,14 +708,38 @@
 
         libraryRootPath = Path(dock.library_model.rootPath()) / "qubits"
         stringLibraryRootPath = str(libraryRootPath)
         view.expand(
             dock.proxy_library_model.mapFromSource(
                 dock.library_model.index(stringLibraryRootPath)))
 
+        # Add a text changed event to the filter text box
+        self.ui.dockLibrary_filter.textChanged.connect(
+            self.dockLibrary_filter_onChanged)
+
+    def dockLibrary_filter_onChanged(self, text):
+        """ Text changed event for filter_text_design
+        Args:
+            text: Text typed in the filter box.
+        """
+        view = self.ui.dockLibrary_tree_view
+        dock = self.ui.dockLibrary
+        dock.proxy_library_model.filter_text = text
+
+        dock.proxy_library_model.setFilterWildcard(text)
+
+        view.setRootIndex(
+            dock.proxy_library_model.mapFromSource(
+                dock.library_model.index(dock.library_model.rootPath())))
+
+        if len(text) >= 1 and dock.proxy_library_model.rowCount() > 0:
+            view.expandAll()
+        else:
+            view.collapseAll()
+
     ################################################
     # UI
     def toggle_docks(self, do_hide: bool = None):
         """Show or hide the full plot-area widget / show or hide all docks.
 
         Args:
             do_hide (bool): Hide or show. Defaults to None -- toggle.
@@ -739,15 +807,15 @@
             For that, call rebuild.
         """
 
         # Global level
         self.refresh_design()
 
         # Table models
-        self.ui.tableComponents.model().refresh()
+        self.ui.tableComponents.model().sourceModel().refresh()
 
         # Redraw plots
         self.refresh_plot()
 
     def refresh_plot(self):
         """Redraw only the plot window contents."""
         self.plot_win.replot()
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/main_window_base.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/main_window_base.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/main_window_rc.qrc` & `qiskit_metal-0.1.5/qiskit_metal/_gui/main_window_rc.qrc`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/main_window_rc_rc.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/main_window_rc_rc.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/main_window_ui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/main_window_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/main_window_ui.ui`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/net_list_ui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/net_list_ui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/net_list_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/net_list_ui.ui`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/net_list_window.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/net_list_window.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/plot_window_ui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/plot_window_ui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/plot_window_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/plot_window_ui.ui`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_gds_gui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_gds_gui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_gds_model.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_gds_model.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_gds_ui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/parameter_entry_window_ui.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,154 +1,139 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file './renderer_gds_ui.ui',
-# licensing of './renderer_gds_ui.ui' applies.
+# Form implementation generated from reading ui file './widgets/create_component_window/parameter_entry_window_ui.ui',
+# licensing of './widgets/create_component_window/parameter_entry_window_ui.ui' applies.
 #
 # Created: Sat Jun 19 22:02:30 2021
 #      by: pyside2-uic  running on PySide2 5.13.2
 #
 # WARNING! All changes made in this file will be lost!
 
 from PySide2 import QtCore, QtGui, QtWidgets
 
 
 class Ui_MainWindow(object):
 
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
-        MainWindow.resize(651, 581)
+        MainWindow.resize(753, 600)
         self.centralwidget = QtWidgets.QWidget(MainWindow)
         self.centralwidget.setObjectName("centralwidget")
-        self.horizontalLayoutWidget = QtWidgets.QWidget(self.centralwidget)
-        self.horizontalLayoutWidget.setGeometry(QtCore.QRect(10, 500, 631, 38))
-        self.horizontalLayoutWidget.setObjectName("horizontalLayoutWidget")
-        self.horizontalLayout = QtWidgets.QHBoxLayout(
-            self.horizontalLayoutWidget)
-        self.horizontalLayout.setContentsMargins(0, 0, 0, 0)
-        self.horizontalLayout.setObjectName("horizontalLayout")
-        self.lineEdit = QtWidgets.QLineEdit(self.horizontalLayoutWidget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding,
-                                           QtWidgets.QSizePolicy.Fixed)
+        self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.centralwidget)
+        self.verticalLayout_2.setObjectName("verticalLayout_2")
+        self.explanatory_label = QtWidgets.QLabel(self.centralwidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred,
+                                           QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setVerticalStretch(1)
         sizePolicy.setHeightForWidth(
-            self.lineEdit.sizePolicy().hasHeightForWidth())
-        self.lineEdit.setSizePolicy(sizePolicy)
-        self.lineEdit.setObjectName("lineEdit")
-        self.horizontalLayout.addWidget(self.lineEdit)
-        self.browseButton = QtWidgets.QToolButton(self.horizontalLayoutWidget)
-        icon = QtGui.QIcon()
-        icon.addPixmap(QtGui.QPixmap(":/_imgs/search.png"), QtGui.QIcon.Normal,
-                       QtGui.QIcon.Off)
-        self.browseButton.setIcon(icon)
-        self.browseButton.setToolButtonStyle(QtCore.Qt.ToolButtonTextBesideIcon)
-        self.browseButton.setAutoRaise(False)
-        self.browseButton.setObjectName("browseButton")
-        self.horizontalLayout.addWidget(self.browseButton)
-        self.exportButton = QtWidgets.QPushButton(self.horizontalLayoutWidget)
-        self.exportButton.setObjectName("exportButton")
-        self.horizontalLayout.addWidget(self.exportButton)
-        self.instructionsLabel = QtWidgets.QLabel(self.centralwidget)
-        self.instructionsLabel.setGeometry(QtCore.QRect(20, 10, 201, 16))
-        self.instructionsLabel.setObjectName("instructionsLabel")
-        self.horizontalLayoutWidget_2 = QtWidgets.QWidget(self.centralwidget)
-        self.horizontalLayoutWidget_2.setGeometry(QtCore.QRect(
-            10, 470, 301, 32))
-        self.horizontalLayoutWidget_2.setObjectName("horizontalLayoutWidget_2")
-        self.horizontalLayout_4 = QtWidgets.QHBoxLayout(
-            self.horizontalLayoutWidget_2)
-        self.horizontalLayout_4.setContentsMargins(0, 0, 0, 0)
-        self.horizontalLayout_4.setObjectName("horizontalLayout_4")
-        self.refreshButton = QtWidgets.QPushButton(
-            self.horizontalLayoutWidget_2)
-        self.refreshButton.setObjectName("refreshButton")
-        self.horizontalLayout_4.addWidget(self.refreshButton)
-        self.selectAllButton = QtWidgets.QPushButton(
-            self.horizontalLayoutWidget_2)
-        self.selectAllButton.setObjectName("selectAllButton")
-        self.horizontalLayout_4.addWidget(self.selectAllButton)
-        self.deselectAllButton = QtWidgets.QPushButton(
-            self.horizontalLayoutWidget_2)
-        self.deselectAllButton.setObjectName("deselectAllButton")
-        self.horizontalLayout_4.addWidget(self.deselectAllButton)
-        self.listView = QtWidgets.QListView(self.centralwidget)
-        self.listView.setGeometry(QtCore.QRect(10, 31, 301, 431))
-        self.listView.setObjectName("listView")
-        self.treeView = QTreeView_Base(self.centralwidget)
-        self.treeView.setGeometry(QtCore.QRect(325, 30, 311, 361))
-        self.treeView.setRootIsDecorated(False)
-        self.treeView.setObjectName("treeView")
-        self.instructionsLabel_2 = QtWidgets.QLabel(self.centralwidget)
-        self.instructionsLabel_2.setGeometry(QtCore.QRect(380, 10, 201, 16))
-        self.instructionsLabel_2.setAlignment(QtCore.Qt.AlignCenter)
-        self.instructionsLabel_2.setObjectName("instructionsLabel_2")
-        self.label = QtWidgets.QLabel(self.centralwidget)
-        self.label.setGeometry(QtCore.QRect(330, 400, 301, 91))
+            self.explanatory_label.sizePolicy().hasHeightForWidth())
+        self.explanatory_label.setSizePolicy(sizePolicy)
+        self.explanatory_label.setObjectName("explanatory_label")
+        self.verticalLayout_2.addWidget(self.explanatory_label)
+        self.widget = QtWidgets.QWidget(self.centralwidget)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred,
                                            QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setVerticalStretch(20)
         sizePolicy.setHeightForWidth(
-            self.label.sizePolicy().hasHeightForWidth())
-        self.label.setSizePolicy(sizePolicy)
-        self.label.setWordWrap(True)
-        self.label.setObjectName("label")
+            self.widget.sizePolicy().hasHeightForWidth())
+        self.widget.setSizePolicy(sizePolicy)
+        self.widget.setObjectName("widget")
+        self.horizontalLayout_4 = QtWidgets.QHBoxLayout(self.widget)
+        self.horizontalLayout_4.setContentsMargins(0, 0, 0, 0)
+        self.horizontalLayout_4.setObjectName("horizontalLayout_4")
+        self.edit_box = QtWidgets.QWidget(self.widget)
+        self.edit_box.setObjectName("edit_box")
+        self.verticalLayout_4 = QtWidgets.QVBoxLayout(self.edit_box)
+        self.verticalLayout_4.setContentsMargins(0, 0, 0, 0)
+        self.verticalLayout_4.setObjectName("verticalLayout_4")
+        self.widget_3 = QtWidgets.QWidget(self.edit_box)
+        self.widget_3.setObjectName("widget_3")
+        self.horizontalLayout_5 = QtWidgets.QHBoxLayout(self.widget_3)
+        self.horizontalLayout_5.setContentsMargins(0, 0, 0, 0)
+        self.horizontalLayout_5.setObjectName("horizontalLayout_5")
+        self.add_k_v_row_button = QtWidgets.QPushButton(self.widget_3)
+        self.add_k_v_row_button.setObjectName("add_k_v_row_button")
+        self.horizontalLayout_5.addWidget(self.add_k_v_row_button)
+        self.nest_dictionary_button = QtWidgets.QPushButton(self.widget_3)
+        self.nest_dictionary_button.setObjectName("nest_dictionary_button")
+        self.horizontalLayout_5.addWidget(self.nest_dictionary_button)
+        self.remove_button = QtWidgets.QPushButton(self.widget_3)
+        self.remove_button.setObjectName("remove_button")
+        self.horizontalLayout_5.addWidget(self.remove_button)
+        self.verticalLayout_4.addWidget(self.widget_3)
+        self.qcomponent_param_tree_view = TreeViewParamEntry(self.edit_box)
+        self.qcomponent_param_tree_view.setObjectName(
+            "qcomponent_param_tree_view")
+        self.verticalLayout_4.addWidget(self.qcomponent_param_tree_view)
+        self.parameter_entry_form = QtWidgets.QWidget(self.edit_box)
+        self.parameter_entry_form.setObjectName("parameter_entry_form")
+        self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.parameter_entry_form)
+        self.verticalLayout_6.setContentsMargins(0, 0, 0, 0)
+        self.verticalLayout_6.setObjectName("verticalLayout_6")
+        self.verticalLayout_4.addWidget(self.parameter_entry_form)
+        self.create_qcomp_button = QtWidgets.QPushButton(self.edit_box)
+        self.create_qcomp_button.setObjectName("create_qcomp_button")
+        self.verticalLayout_4.addWidget(self.create_qcomp_button)
+        self.horizontalLayout_4.addWidget(self.edit_box)
+        self.help_box = QtWidgets.QWidget(self.widget)
+        self.help_box.setObjectName("help_box")
+        self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.help_box)
+        self.verticalLayout_5.setContentsMargins(0, 0, 0, 0)
+        self.verticalLayout_5.setObjectName("verticalLayout_5")
+        self.help_button_holder = QtWidgets.QWidget(self.help_box)
+        self.help_button_holder.setObjectName("help_button_holder")
+        self.horizontalLayout_6 = QtWidgets.QHBoxLayout(self.help_button_holder)
+        self.horizontalLayout_6.setContentsMargins(0, 0, 0, 0)
+        self.horizontalLayout_6.setObjectName("horizontalLayout_6")
+        self.verticalLayout_5.addWidget(self.help_button_holder)
+        self.help_tab_tabWidget = QtWidgets.QTabWidget(self.help_box)
+        self.help_tab_tabWidget.setObjectName("help_tab_tabWidget")
+        self.tab_source = QtWidgets.QWidget()
+        self.tab_source.setObjectName("tab_source")
+        self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.tab_source)
+        self.verticalLayout_7.setObjectName("verticalLayout_7")
+        self.help_tab_tabWidget.addTab(self.tab_source, "")
+        self.tab_help = QtWidgets.QWidget()
+        self.tab_help.setObjectName("tab_help")
+        self.verticalLayout_8 = QtWidgets.QVBoxLayout(self.tab_help)
+        self.verticalLayout_8.setObjectName("verticalLayout_8")
+        self.help_tab_tabWidget.addTab(self.tab_help, "")
+        self.verticalLayout_5.addWidget(self.help_tab_tabWidget)
+        self.horizontalLayout_4.addWidget(self.help_box)
+        self.verticalLayout_2.addWidget(self.widget)
         MainWindow.setCentralWidget(self.centralwidget)
-        self.menubar = QtWidgets.QMenuBar()
-        self.menubar.setGeometry(QtCore.QRect(0, 0, 651, 22))
-        self.menubar.setObjectName("menubar")
-        MainWindow.setMenuBar(self.menubar)
         self.statusbar = QtWidgets.QStatusBar(MainWindow)
         self.statusbar.setObjectName("statusbar")
         MainWindow.setStatusBar(self.statusbar)
 
         self.retranslateUi(MainWindow)
-        QtCore.QObject.connect(self.browseButton, QtCore.SIGNAL("clicked()"),
-                               MainWindow.browse_folders)
-        QtCore.QObject.connect(self.exportButton, QtCore.SIGNAL("clicked()"),
-                               MainWindow.export_file)
-        QtCore.QObject.connect(self.selectAllButton, QtCore.SIGNAL("clicked()"),
-                               MainWindow.select_all)
-        QtCore.QObject.connect(self.deselectAllButton,
-                               QtCore.SIGNAL("clicked()"),
-                               MainWindow.deselect_all)
-        QtCore.QObject.connect(self.refreshButton, QtCore.SIGNAL("clicked()"),
-                               MainWindow.refresh)
+        self.help_tab_tabWidget.setCurrentIndex(1)
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
 
     def retranslateUi(self, MainWindow):
         MainWindow.setWindowTitle(
-            QtWidgets.QApplication.translate("MainWindow", "GDS Renderer", None,
+            QtWidgets.QApplication.translate("MainWindow", "MainWindow", None,
                                              -1))
-        self.lineEdit.setPlaceholderText(
-            QtWidgets.QApplication.translate(
-                "MainWindow", "Export GDS to the following location... ", None,
-                -1))
-        self.browseButton.setText(
-            QtWidgets.QApplication.translate("MainWindow", "Browse", None, -1))
-        self.exportButton.setText(
-            QtWidgets.QApplication.translate("MainWindow", "Export", None, -1))
-        self.instructionsLabel.setText(
+        self.explanatory_label.setText(
             QtWidgets.QApplication.translate("MainWindow",
-                                             "Check off components to export:",
-                                             None, -1))
-        self.refreshButton.setText(
-            QtWidgets.QApplication.translate("MainWindow", "Refresh List", None,
-                                             -1))
-        self.selectAllButton.setText(
-            QtWidgets.QApplication.translate("MainWindow", "Select All", None,
-                                             -1))
-        self.deselectAllButton.setText(
-            QtWidgets.QApplication.translate("MainWindow", "Deselect All", None,
+                                             "Options to create with", None,
                                              -1))
-        self.instructionsLabel_2.setText(
-            QtWidgets.QApplication.translate("MainWindow", "Renderer options",
+        self.add_k_v_row_button.setText(
+            QtWidgets.QApplication.translate("MainWindow", "Add Row", None, -1))
+        self.nest_dictionary_button.setText(
+            QtWidgets.QApplication.translate("MainWindow", "Nest Dictionary",
                                              None, -1))
-        self.label.setText(
-            QtWidgets.QApplication.translate(
-                "MainWindow",
-                "Note: The user-defined bounding box scales above are only relevant when not all components are being exported. Otherwise, the bounding box for the subtraction layer is obtained from the DesignPlanar class.",
-                None, -1))
+        self.remove_button.setText(
+            QtWidgets.QApplication.translate("MainWindow", "Remove", None, -1))
+        self.create_qcomp_button.setText(
+            QtWidgets.QApplication.translate("MainWindow", "Create", None, -1))
+        self.help_tab_tabWidget.setTabText(
+            self.help_tab_tabWidget.indexOf(self.tab_source),
+            QtWidgets.QApplication.translate("MainWindow", "Source", None, -1))
+        self.help_tab_tabWidget.setTabText(
+            self.help_tab_tabWidget.indexOf(self.tab_help),
+            QtWidgets.QApplication.translate("MainWindow", "Help", None, -1))
 
 
-from .tree_view_base import QTreeView_Base
-from . import main_window_rc_rc
+from .model_view.tree_view_param_entry import TreeViewParamEntry
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_gds_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_gds_ui.ui`

 * *Files 14% similar despite different names*

#### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_gds_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_gds_ui.ui`

```diff
@@ -10,180 +10,135 @@
         <height>581</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>GDS Renderer</string>
     </property>
     <widget class="QWidget" name="centralwidget">
-      <widget class="QWidget" name="horizontalLayoutWidget">
-        <property name="geometry">
-          <rect>
-            <x>10</x>
-            <y>500</y>
-            <width>631</width>
-            <height>38</height>
-          </rect>
-        </property>
-        <layout class="QHBoxLayout" name="horizontalLayout" stretch="0,0,0">
-          <item>
-            <widget class="QLineEdit" name="lineEdit">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="placeholderText">
-                <string>Export GDS to the following location...</string>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <widget class="QToolButton" name="browseButton">
-              <property name="text">
-                <string>Browse</string>
-              </property>
-              <property name="icon">
-                <iconset resource="main_window_rc.qrc">
-                  <normaloff>:/_imgs/search.png</normaloff>
-                  :/_imgs/search.png
-                </iconset>
-              </property>
-              <property name="toolButtonStyle">
-                <enum>Qt::ToolButtonTextBesideIcon</enum>
-              </property>
-              <property name="autoRaise">
-                <bool>false</bool>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <widget class="QPushButton" name="exportButton">
-              <property name="text">
-                <string>Export</string>
-              </property>
-            </widget>
-          </item>
-        </layout>
-      </widget>
-      <widget class="QLabel" name="instructionsLabel">
-        <property name="geometry">
-          <rect>
-            <x>20</x>
-            <y>10</y>
-            <width>201</width>
-            <height>16</height>
-          </rect>
-        </property>
-        <property name="text">
-          <string>Check off components to export:</string>
-        </property>
-      </widget>
-      <widget class="QWidget" name="horizontalLayoutWidget_2">
-        <property name="geometry">
-          <rect>
-            <x>10</x>
-            <y>470</y>
-            <width>301</width>
-            <height>32</height>
-          </rect>
-        </property>
-        <layout class="QHBoxLayout" name="horizontalLayout_4">
-          <item>
-            <widget class="QPushButton" name="refreshButton">
-              <property name="text">
-                <string>Refresh List</string>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <widget class="QPushButton" name="selectAllButton">
-              <property name="text">
-                <string>Select All</string>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <widget class="QPushButton" name="deselectAllButton">
-              <property name="text">
-                <string>Deselect All</string>
-              </property>
-            </widget>
-          </item>
-        </layout>
-      </widget>
-      <widget class="QListView" name="listView">
-        <property name="geometry">
-          <rect>
-            <x>10</x>
-            <y>31</y>
-            <width>301</width>
-            <height>431</height>
-          </rect>
-        </property>
-      </widget>
-      <widget class="QTreeView_Base" name="treeView">
-        <property name="geometry">
-          <rect>
-            <x>325</x>
-            <y>30</y>
-            <width>311</width>
-            <height>361</height>
-          </rect>
-        </property>
-        <property name="rootIsDecorated">
-          <bool>false</bool>
-        </property>
-      </widget>
-      <widget class="QLabel" name="instructionsLabel_2">
-        <property name="geometry">
-          <rect>
-            <x>380</x>
-            <y>10</y>
-            <width>201</width>
-            <height>16</height>
-          </rect>
-        </property>
-        <property name="text">
-          <string>Renderer options</string>
-        </property>
-        <property name="alignment">
-          <set>Qt::AlignCenter</set>
-        </property>
-      </widget>
-      <widget class="QLabel" name="label">
-        <property name="geometry">
-          <rect>
-            <x>330</x>
-            <y>400</y>
-            <width>301</width>
-            <height>91</height>
-          </rect>
-        </property>
-        <property name="sizePolicy">
-          <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
-            <horstretch>0</horstretch>
-            <verstretch>0</verstretch>
-          </sizepolicy>
-        </property>
-        <property name="text">
-          <string>Note: The user-defined bounding box scales above are only relevant when not all components are being exported. Otherwise, the bounding box for the subtraction layer is obtained from the DesignPlanar class.</string>
-        </property>
-        <property name="wordWrap">
-          <bool>true</bool>
-        </property>
-      </widget>
+      <layout class="QGridLayout" name="gridLayout">
+        <item row="0" column="0">
+          <widget class="QLabel" name="instructionsLabel">
+            <property name="text">
+              <string>Check off components to export:</string>
+            </property>
+          </widget>
+        </item>
+        <item row="0" column="1">
+          <widget class="QLabel" name="instructionsLabel_2">
+            <property name="text">
+              <string>Renderer options</string>
+            </property>
+            <property name="alignment">
+              <set>Qt::AlignCenter</set>
+            </property>
+          </widget>
+        </item>
+        <item row="1" column="0" rowspan="2">
+          <widget class="QListView" name="listView"/>
+        </item>
+        <item row="1" column="1">
+          <widget class="QTreeView_Base" name="treeView">
+            <property name="rootIsDecorated">
+              <bool>false</bool>
+            </property>
+          </widget>
+        </item>
+        <item row="2" column="1" rowspan="2">
+          <widget class="QLabel" name="label">
+            <property name="sizePolicy">
+              <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+                <horstretch>0</horstretch>
+                <verstretch>0</verstretch>
+              </sizepolicy>
+            </property>
+            <property name="text">
+              <string>Note: The user-defined bounding box scales above are only relevant when not all components are being exported. Otherwise, the bounding box for the subtraction layer is obtained from the DesignPlanar class.</string>
+            </property>
+            <property name="wordWrap">
+              <bool>true</bool>
+            </property>
+          </widget>
+        </item>
+        <item row="3" column="0">
+          <layout class="QHBoxLayout" name="horizontalLayout_4">
+            <item>
+              <widget class="QPushButton" name="refreshButton">
+                <property name="text">
+                  <string>Refresh List</string>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QPushButton" name="selectAllButton">
+                <property name="text">
+                  <string>Select All</string>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QPushButton" name="deselectAllButton">
+                <property name="text">
+                  <string>Deselect All</string>
+                </property>
+              </widget>
+            </item>
+          </layout>
+        </item>
+        <item row="4" column="0" colspan="2">
+          <layout class="QHBoxLayout" name="horizontalLayout" stretch="0,0,0">
+            <item>
+              <widget class="QLineEdit" name="lineEdit">
+                <property name="sizePolicy">
+                  <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
+                    <horstretch>0</horstretch>
+                    <verstretch>0</verstretch>
+                  </sizepolicy>
+                </property>
+                <property name="placeholderText">
+                  <string>Export GDS to the following location...</string>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QToolButton" name="browseButton">
+                <property name="text">
+                  <string>Browse</string>
+                </property>
+                <property name="icon">
+                  <iconset>
+                    <normaloff>:/_imgs/search.png</normaloff>
+                    :/_imgs/search.png
+                  </iconset>
+                </property>
+                <property name="toolButtonStyle">
+                  <enum>Qt::ToolButtonTextBesideIcon</enum>
+                </property>
+                <property name="autoRaise">
+                  <bool>false</bool>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QPushButton" name="exportButton">
+                <property name="text">
+                  <string>Export</string>
+                </property>
+              </widget>
+            </item>
+          </layout>
+        </item>
+      </layout>
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>651</width>
-          <height>22</height>
+          <height>18</height>
         </rect>
       </property>
     </widget>
     <widget class="QStatusBar" name="statusbar"/>
   </widget>
   <customwidgets>
     <customwidget>
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_hfss_gui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_hfss_gui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_hfss_model.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_hfss_model.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_hfss_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_hfss_ui.ui`

 * *Files 20% similar despite different names*

#### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_hfss_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_hfss_ui.ui`

```diff
@@ -10,176 +10,125 @@
         <height>544</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>HFSS Renderer</string>
     </property>
     <widget class="QWidget" name="centralwidget">
-      <widget class="QLabel" name="instructionsLabel">
-        <property name="geometry">
-          <rect>
-            <x>20</x>
-            <y>10</y>
-            <width>201</width>
-            <height>16</height>
-          </rect>
-        </property>
-        <property name="text">
-          <string>Check off components to export:</string>
-        </property>
-      </widget>
-      <widget class="QWidget" name="horizontalLayoutWidget_2">
-        <property name="geometry">
-          <rect>
-            <x>10</x>
-            <y>470</y>
-            <width>301</width>
-            <height>32</height>
-          </rect>
-        </property>
-        <layout class="QHBoxLayout" name="horizontalLayout_4">
-          <item>
-            <widget class="QPushButton" name="refreshButton">
-              <property name="text">
-                <string>Refresh List</string>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <widget class="QPushButton" name="selectAllButton">
-              <property name="text">
-                <string>Select All</string>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <widget class="QPushButton" name="deselectAllButton">
+      <layout class="QGridLayout" name="gridLayout">
+        <item row="0" column="0">
+          <widget class="QLabel" name="instructionsLabel">
+            <property name="text">
+              <string>Check off components to export:</string>
+            </property>
+          </widget>
+        </item>
+        <item row="0" column="1">
+          <widget class="QLabel" name="instructionsLabel_2">
+            <property name="text">
+              <string>Renderer options</string>
+            </property>
+            <property name="alignment">
+              <set>Qt::AlignCenter</set>
+            </property>
+          </widget>
+        </item>
+        <item row="1" column="0" rowspan="3">
+          <widget class="QListView" name="listView"/>
+        </item>
+        <item row="1" column="1">
+          <widget class="QTreeView_Base" name="treeView">
+            <property name="rootIsDecorated">
+              <bool>false</bool>
+            </property>
+          </widget>
+        </item>
+        <item row="2" column="1">
+          <widget class="QLabel" name="solutionLabel">
+            <property name="text">
+              <string>Solution type:</string>
+            </property>
+            <property name="alignment">
+              <set>Qt::AlignCenter</set>
+            </property>
+          </widget>
+        </item>
+        <item row="3" column="1">
+          <widget class="QComboBox" name="solnComboBox">
+            <item>
               <property name="text">
-                <string>Deselect All</string>
+                <string>Eigenmode</string>
               </property>
-            </widget>
-          </item>
-        </layout>
-      </widget>
-      <widget class="QListView" name="listView">
-        <property name="geometry">
-          <rect>
-            <x>10</x>
-            <y>31</y>
-            <width>301</width>
-            <height>431</height>
-          </rect>
-        </property>
-      </widget>
-      <widget class="QTreeView_Base" name="treeView">
-        <property name="geometry">
-          <rect>
-            <x>325</x>
-            <y>30</y>
-            <width>311</width>
-            <height>381</height>
-          </rect>
-        </property>
-        <property name="rootIsDecorated">
-          <bool>false</bool>
-        </property>
-      </widget>
-      <widget class="QLabel" name="instructionsLabel_2">
-        <property name="geometry">
-          <rect>
-            <x>380</x>
-            <y>10</y>
-            <width>201</width>
-            <height>16</height>
-          </rect>
-        </property>
-        <property name="text">
-          <string>Renderer options</string>
-        </property>
-        <property name="alignment">
-          <set>Qt::AlignCenter</set>
-        </property>
-      </widget>
-      <widget class="QWidget" name="horizontalLayoutWidget">
-        <property name="geometry">
-          <rect>
-            <x>370</x>
-            <y>470</y>
-            <width>231</width>
-            <height>32</height>
-          </rect>
-        </property>
-        <layout class="QHBoxLayout" name="horizontalLayout" stretch="0">
-          <item>
-            <widget class="QPushButton" name="confirmButton">
+            </item>
+            <item>
               <property name="text">
-                <string>Confirm Selection</string>
+                <string>Driven Modal</string>
               </property>
-            </widget>
-          </item>
-        </layout>
-      </widget>
-      <widget class="QComboBox" name="solnComboBox">
-        <property name="geometry">
-          <rect>
-            <x>380</x>
-            <y>440</y>
-            <width>211</width>
-            <height>26</height>
-          </rect>
-        </property>
-        <item>
-          <property name="text">
-            <string>Eigenmode</string>
-          </property>
-        </item>
-        <item>
-          <property name="text">
-            <string>Driven Modal</string>
-          </property>
-        </item>
-      </widget>
-      <widget class="QLabel" name="solutionLabel">
-        <property name="geometry">
-          <rect>
-            <x>410</x>
-            <y>420</y>
-            <width>141</width>
-            <height>16</height>
-          </rect>
-        </property>
-        <property name="text">
-          <string>Solution type:</string>
-        </property>
-        <property name="alignment">
-          <set>Qt::AlignCenter</set>
-        </property>
-      </widget>
+            </item>
+          </widget>
+        </item>
+        <item row="4" column="0">
+          <layout class="QHBoxLayout" name="horizontalLayout_4">
+            <item>
+              <widget class="QPushButton" name="refreshButton">
+                <property name="text">
+                  <string>Refresh List</string>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QPushButton" name="selectAllButton">
+                <property name="text">
+                  <string>Select All</string>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QPushButton" name="deselectAllButton">
+                <property name="text">
+                  <string>Deselect All</string>
+                </property>
+              </widget>
+            </item>
+          </layout>
+        </item>
+        <item row="4" column="1">
+          <layout class="QHBoxLayout" name="horizontalLayout" stretch="0">
+            <item>
+              <widget class="QPushButton" name="confirmButton">
+                <property name="text">
+                  <string>Confirm Selection</string>
+                </property>
+              </widget>
+            </item>
+          </layout>
+        </item>
+      </layout>
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>646</width>
-          <height>22</height>
+          <height>18</height>
         </rect>
       </property>
     </widget>
     <widget class="QStatusBar" name="statusbar"/>
   </widget>
   <customwidgets>
     <customwidget>
       <class>QTreeView_Base</class>
       <extends>QTreeView</extends>
       <header>.tree_view_base</header>
     </customwidget>
   </customwidgets>
   <resources>
-    <include location="../../../qiskit-metal/qiskit_metal/_gui/main_window_rc.qrc"/>
+    <include location="main_window_rc.qrc"/>
   </resources>
   <connections>
     <connection>
       <sender>selectAllButton</sender>
       <signal>clicked()</signal>
       <receiver>MainWindow</receiver>
       <slot>select_all()</slot>
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_q3d_gui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_q3d_gui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_q3d_model.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_q3d_model.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/renderer_q3d_ui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/renderer_hfss_ui.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,101 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file './renderer_q3d_ui.ui',
-# licensing of './renderer_q3d_ui.ui' applies.
+# Form implementation generated from reading ui file 'c:\Temp\GitHub\qiskit-metal\qiskit_metal\_gui\renderer_hfss_ui.ui'
 #
-# Created: Sat Jun 19 22:02:29 2021
-#      by: pyside2-uic  running on PySide2 5.13.2
+# Created by: PyQt5 UI code generator 5.15.9
 #
-# WARNING! All changes made in this file will be lost!
+# WARNING: Any manual changes made to this file will be lost when pyuic5 is
+# run again.  Do not edit this file unless you know what you are doing.
 
 from PySide2 import QtCore, QtGui, QtWidgets
 
 
 class Ui_MainWindow(object):
 
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
-        MainWindow.resize(651, 544)
+        MainWindow.resize(646, 544)
         self.centralwidget = QtWidgets.QWidget(MainWindow)
         self.centralwidget.setObjectName("centralwidget")
+        self.gridLayout = QtWidgets.QGridLayout(self.centralwidget)
+        self.gridLayout.setObjectName("gridLayout")
         self.instructionsLabel = QtWidgets.QLabel(self.centralwidget)
-        self.instructionsLabel.setGeometry(QtCore.QRect(20, 10, 201, 16))
         self.instructionsLabel.setObjectName("instructionsLabel")
-        self.horizontalLayoutWidget_2 = QtWidgets.QWidget(self.centralwidget)
-        self.horizontalLayoutWidget_2.setGeometry(QtCore.QRect(
-            10, 470, 301, 32))
-        self.horizontalLayoutWidget_2.setObjectName("horizontalLayoutWidget_2")
-        self.horizontalLayout_4 = QtWidgets.QHBoxLayout(
-            self.horizontalLayoutWidget_2)
-        self.horizontalLayout_4.setContentsMargins(0, 0, 0, 0)
+        self.gridLayout.addWidget(self.instructionsLabel, 0, 0, 1, 1)
+        self.instructionsLabel_2 = QtWidgets.QLabel(self.centralwidget)
+        self.instructionsLabel_2.setAlignment(QtCore.Qt.AlignCenter)
+        self.instructionsLabel_2.setObjectName("instructionsLabel_2")
+        self.gridLayout.addWidget(self.instructionsLabel_2, 0, 1, 1, 1)
+        self.listView = QtWidgets.QListView(self.centralwidget)
+        self.listView.setObjectName("listView")
+        self.gridLayout.addWidget(self.listView, 1, 0, 3, 1)
+        self.treeView = QTreeView_Base(self.centralwidget)
+        self.treeView.setRootIsDecorated(False)
+        self.treeView.setObjectName("treeView")
+        self.gridLayout.addWidget(self.treeView, 1, 1, 1, 1)
+        self.solutionLabel = QtWidgets.QLabel(self.centralwidget)
+        self.solutionLabel.setAlignment(QtCore.Qt.AlignCenter)
+        self.solutionLabel.setObjectName("solutionLabel")
+        self.gridLayout.addWidget(self.solutionLabel, 2, 1, 1, 1)
+        self.solnComboBox = QtWidgets.QComboBox(self.centralwidget)
+        self.solnComboBox.setObjectName("solnComboBox")
+        self.solnComboBox.addItem("")
+        self.solnComboBox.addItem("")
+        self.gridLayout.addWidget(self.solnComboBox, 3, 1, 1, 1)
+        self.horizontalLayout_4 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_4.setObjectName("horizontalLayout_4")
-        self.refreshButton = QtWidgets.QPushButton(
-            self.horizontalLayoutWidget_2)
+        self.refreshButton = QtWidgets.QPushButton(self.centralwidget)
         self.refreshButton.setObjectName("refreshButton")
         self.horizontalLayout_4.addWidget(self.refreshButton)
-        self.selectAllButton = QtWidgets.QPushButton(
-            self.horizontalLayoutWidget_2)
+        self.selectAllButton = QtWidgets.QPushButton(self.centralwidget)
         self.selectAllButton.setObjectName("selectAllButton")
         self.horizontalLayout_4.addWidget(self.selectAllButton)
-        self.deselectAllButton = QtWidgets.QPushButton(
-            self.horizontalLayoutWidget_2)
+        self.deselectAllButton = QtWidgets.QPushButton(self.centralwidget)
         self.deselectAllButton.setObjectName("deselectAllButton")
         self.horizontalLayout_4.addWidget(self.deselectAllButton)
-        self.listView = QtWidgets.QListView(self.centralwidget)
-        self.listView.setGeometry(QtCore.QRect(10, 31, 301, 431))
-        self.listView.setObjectName("listView")
-        self.treeView = QTreeView_Base(self.centralwidget)
-        self.treeView.setGeometry(QtCore.QRect(325, 30, 311, 431))
-        self.treeView.setRootIsDecorated(False)
-        self.treeView.setObjectName("treeView")
-        self.instructionsLabel_2 = QtWidgets.QLabel(self.centralwidget)
-        self.instructionsLabel_2.setGeometry(QtCore.QRect(380, 10, 201, 16))
-        self.instructionsLabel_2.setAlignment(QtCore.Qt.AlignCenter)
-        self.instructionsLabel_2.setObjectName("instructionsLabel_2")
-        self.horizontalLayoutWidget = QtWidgets.QWidget(self.centralwidget)
-        self.horizontalLayoutWidget.setGeometry(QtCore.QRect(370, 470, 231, 32))
-        self.horizontalLayoutWidget.setObjectName("horizontalLayoutWidget")
-        self.horizontalLayout = QtWidgets.QHBoxLayout(
-            self.horizontalLayoutWidget)
-        self.horizontalLayout.setContentsMargins(0, 0, 0, 0)
+        self.gridLayout.addLayout(self.horizontalLayout_4, 4, 0, 1, 1)
+        self.horizontalLayout = QtWidgets.QHBoxLayout()
         self.horizontalLayout.setObjectName("horizontalLayout")
-        self.confirmButton = QtWidgets.QPushButton(self.horizontalLayoutWidget)
+        self.confirmButton = QtWidgets.QPushButton(self.centralwidget)
         self.confirmButton.setObjectName("confirmButton")
         self.horizontalLayout.addWidget(self.confirmButton)
+        self.gridLayout.addLayout(self.horizontalLayout, 4, 1, 1, 1)
         MainWindow.setCentralWidget(self.centralwidget)
-        self.menubar = QtWidgets.QMenuBar()
-        self.menubar.setGeometry(QtCore.QRect(0, 0, 651, 22))
+        self.menubar = QtWidgets.QMenuBar(MainWindow)
+        self.menubar.setGeometry(QtCore.QRect(0, 0, 646, 18))
         self.menubar.setObjectName("menubar")
         MainWindow.setMenuBar(self.menubar)
         self.statusbar = QtWidgets.QStatusBar(MainWindow)
         self.statusbar.setObjectName("statusbar")
         MainWindow.setStatusBar(self.statusbar)
 
         self.retranslateUi(MainWindow)
-        QtCore.QObject.connect(self.selectAllButton, QtCore.SIGNAL("clicked()"),
-                               MainWindow.select_all)
-        QtCore.QObject.connect(self.deselectAllButton,
-                               QtCore.SIGNAL("clicked()"),
-                               MainWindow.deselect_all)
-        QtCore.QObject.connect(self.refreshButton, QtCore.SIGNAL("clicked()"),
-                               MainWindow.refresh)
-        QtCore.QObject.connect(self.confirmButton, QtCore.SIGNAL("clicked()"),
-                               MainWindow.choose_checked_components)
+        self.selectAllButton.clicked.connect(
+            MainWindow.select_all)  # type: ignore
+        self.deselectAllButton.clicked.connect(
+            MainWindow.deselect_all)  # type: ignore
+        self.refreshButton.clicked.connect(MainWindow.refresh)  # type: ignore
+        self.confirmButton.clicked.connect(
+            MainWindow.choose_checked_components)  # type: ignore
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
 
     def retranslateUi(self, MainWindow):
-        MainWindow.setWindowTitle(
-            QtWidgets.QApplication.translate("MainWindow", "Q3D Renderer", None,
-                                             -1))
+        _translate = QtCore.QCoreApplication.translate
+        MainWindow.setWindowTitle(_translate("MainWindow", "HFSS Renderer"))
         self.instructionsLabel.setText(
-            QtWidgets.QApplication.translate("MainWindow",
-                                             "Check off components to export:",
-                                             None, -1))
-        self.refreshButton.setText(
-            QtWidgets.QApplication.translate("MainWindow", "Refresh List", None,
-                                             -1))
-        self.selectAllButton.setText(
-            QtWidgets.QApplication.translate("MainWindow", "Select All", None,
-                                             -1))
-        self.deselectAllButton.setText(
-            QtWidgets.QApplication.translate("MainWindow", "Deselect All", None,
-                                             -1))
+            _translate("MainWindow", "Check off components to export:"))
         self.instructionsLabel_2.setText(
-            QtWidgets.QApplication.translate("MainWindow", "Renderer options",
-                                             None, -1))
-        self.confirmButton.setText(
-            QtWidgets.QApplication.translate("MainWindow", "Confirm Selection",
-                                             None, -1))
+            _translate("MainWindow", "Renderer options"))
+        self.solutionLabel.setText(_translate("MainWindow", "Solution type:"))
+        self.solnComboBox.setItemText(0, _translate("MainWindow", "Eigenmode"))
+        self.solnComboBox.setItemText(1, _translate("MainWindow",
+                                                    "Driven Modal"))
+        self.refreshButton.setText(_translate("MainWindow", "Refresh List"))
+        self.selectAllButton.setText(_translate("MainWindow", "Select All"))
+        self.deselectAllButton.setText(_translate("MainWindow", "Deselect All"))
+        self.confirmButton.setText(_translate("MainWindow",
+                                              "Confirm Selection"))
 
 
 from .tree_view_base import QTreeView_Base
 from . import main_window_rc_rc
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/tree_view_base.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/tree_view_base.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/utility/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/utility/_handle_qt_messages.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/utility/_handle_qt_messages.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/utility/_toolbox_qt.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/utility/_toolbox_qt.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/all_components/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/all_components/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/all_components/table_model_all_components.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/all_components/table_model_all_components.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/all_components/table_view_all_components.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/all_components/table_view_all_components.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,25 +71,25 @@
 
         selection_model = self.selectionModel()
         selection_model.selectionChanged.connect(self.selection_changed)
 
     @property
     def design(self):
         """Returns the design."""
-        return self.model().design
+        return self.model().sourceModel().design
 
     @property
     def logger(self):
         """Returns the logger."""
-        return self.model().logger
+        return self.model().sourceModel().logger
 
     @property
     def gui(self) -> 'MetalGUI':
         """Returns the GUI."""
-        return self.model().gui
+        return self.model().sourceModel().gui
 
     # @slot_catch_error
     def contextMenuEvent(self, event: QContextMenuEvent):
         """This event handler, for event event, can be reimplemented in a
         subclass to receive widget context menu events.
 
         The handler is called when the widget's contextMenuPolicy
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/bases/QWidget_PlaceholderText.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/bases/QWidget_PlaceholderText.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/bases/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/bases/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/bases/dict_tree_base.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/bases/dict_tree_base.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/bases/expanding_toolbar.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/bases/expanding_toolbar.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/build_history/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/build_history/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/build_history/build_history_scroll_area.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/build_history/build_history_scroll_area.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/build_history/build_history_scroll_area_ui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/build_history/build_history_scroll_area_ui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/build_history/build_history_scroll_area_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/build_history/build_history_scroll_area_ui.ui`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/model_view/tree_delegate_param_entry.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/model_view/tree_delegate_param_entry.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/model_view/tree_model_param_entry.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/model_view/tree_model_param_entry.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/model_view/tree_view_param_entry.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/model_view/tree_view_param_entry.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/parameter_entry_window.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/parameter_entry_window.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/create_component_window/parameter_entry_window_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/create_component_window/parameter_entry_window_ui.ui`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/edit_component/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/edit_component/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/edit_component/component_widget.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/edit_component/component_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/edit_component/table_model_options.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/edit_component/table_model_options.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/edit_component/table_view_options.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/edit_component/table_view_options.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/edit_component/tree_model_options.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/edit_component/tree_model_options.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/edit_component/tree_view_options.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/edit_component/tree_view_options.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/log_widget/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/log_widget/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/log_widget/log_metal.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/log_widget/log_metal.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/plot_widget/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/plot_widget/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/plot_widget/plot_window.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/plot_widget/plot_window.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/qlibrary_display/delegate_qlibrary.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/qlibrary_display/delegate_qlibrary.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/qlibrary_display/file_model_qlibrary.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/qlibrary_display/file_model_qlibrary.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/qlibrary_display/proxy_model_qlibrary.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/qlibrary_display/proxy_model_qlibrary.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 Proxy Model to clean display of QComponents in Library tab
 """
 
 import typing
 
 from PySide2.QtCore import QModelIndex, QSortFilterProxyModel, Qt, QSize
-from PySide2.QtWidgets import QWidget
+from PySide2.QtWidgets import QWidget, QFileSystemModel
 
 
 class LibraryFileProxyModel(QSortFilterProxyModel):
     """
     Proxy Model to clean up display for QFileSystemLibraryModel
     """
 
@@ -35,14 +35,15 @@
         super().__init__(parent)
 
         # finds all files that
         # (Aren't hidden (begin w/ .), don't begin with __init__, don't begin with _template, etc. AND end in .py)  OR (don't begin with __pycache__ and don't have a '.' in the name   # pylint: disable=line-too-long
         # (QComponent files) OR (Directories)
         self.accepted_files__regex = r"(^((?!\.))(?!base)(?!__init__)(?!_template)(?!_parsed)(?!__pycache__).*\.py)|(?!__pycache__)(^([^.]+)$)"  # pylint: disable=line-too-long
         self.setFilterRegExp(self.accepted_files__regex)
+        self.filter_text = ""
 
     def filterAcceptsColumn(
             self, source_column: int, source_parent: QModelIndex) -> bool:  #pylint: disable=unused-argument
         """
         Filters out unwanted file information in display
         Args:
             source_column(int): Display column in question
@@ -53,14 +54,43 @@
 
         """
         # Won't show Size, Kind, Date Modified, etc. for QFileSystemModel
         if source_column > 0:
             return False
         return True
 
+    def filterAcceptsRow(
+            self, source_row: int, source_parent: QModelIndex) -> bool:  #pylint: disable=unused-argument
+        """
+        Filters out unwanted file information in display
+        Args:
+            source_column(int): Display column in question
+            source_parent(QModelIndex): Parent index
+        Returns:
+            bool: Whether to display column
+
+        """
+        source_model = self.sourceModel()
+        nameCache = source_model.nameCache
+
+        index = source_model.index(source_row, 0, source_parent)
+        relativeFilename = index.data(QFileSystemModel.FileNameRole)
+        displayName = nameCache[
+            relativeFilename] if relativeFilename in nameCache else None
+        #fi = source_model.fileInfo(index)
+
+        if displayName != None:
+            found = (self.filter_text in relativeFilename) or (self.filter_text
+                                                               in displayName)
+        else:
+            found = (self.filter_text in relativeFilename)
+
+        accept = (not relativeFilename.startswith("_")) and found
+        return accept
+
     def data(self,
              index: QModelIndex,
              role: int = Qt.DisplayRole) -> typing.Any:
         """
         Sets standard size hint for indexes and allows
         Args:
             index(QModelIndex): Model Index holding data
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/qlibrary_display/tree_view_qlibrary.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/qlibrary_display/tree_view_qlibrary.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/add_delete_table_ui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/add_delete_table_ui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/add_delete_table_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/add_delete_table_ui.ui`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/dialog_popup_ui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/dialog_popup_ui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/dialog_popup_ui.ui` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/dialog_popup_ui.ui`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/prop_val_table_gui.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/prop_val_table_gui.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/prop_val_table_model.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/prop_val_table_model.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_gui/widgets/variable_table/right_click_table_view.py` & `qiskit_metal-0.1.5/qiskit_metal/_gui/widgets/variable_table/right_click_table_view.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/_is_design.py` & `qiskit_metal-0.1.5/qiskit_metal/_is_design.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/core/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/core/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/core/base.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/core/base.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/core/simulation.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/core/simulation.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/em/cpw_calculations.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/em/cpw_calculations.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/em/kappa_calculation.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/em/kappa_calculation.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/em/transmission_fitting.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/em/transmission_fitting.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/hamiltonian/HO_wavefunctions.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/hamiltonian/HO_wavefunctions.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/hamiltonian/states_energies.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/hamiltonian/states_energies.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/hamiltonian/transmon_CPB_analytic.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/hamiltonian/transmon_CPB_analytic.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/hamiltonian/transmon_analytics.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/hamiltonian/transmon_analytics.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/hamiltonian/transmon_charge_basis.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/hamiltonian/transmon_charge_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/energy_participation_ratio.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/energy_participation_ratio.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/lom_core_analysis.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/lom_core_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/lom_extensions.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/lom_extensions.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/lom_time_evolution_sim.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/lom_time_evolution_sim.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/lumped_capacitive.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/lumped_capacitive.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     EJ = phi0**2 / LJ / hbar
     Zqp = np.sqrt(LJ / Cq)
     EC = e**2 / 2 / Cq / hbar
     wq0 = 1 / np.sqrt(LJ * Cq)
     wq = 1 / np.sqrt(LJ * Cq) - EC
 
     # charge dispersion
-    eps1 = EC * 2**9 * (2/np.sqrt(np.pi)) * \
+    eps1 = EC * 2**9 * (np.sqrt(2/np.pi)) * \
         (EJ/2/EC)**(1.25) * np.exp(-np.sqrt(8*EJ/EC))
 
     return LJ, EJ, Zqp, EC, wq, wq0, eps1
 
 
 # TODO: Move to a more generic file
 
@@ -259,39 +259,51 @@
     for ii in range(N):
         for jj in range(N):
             if ii != jj:
                 Cbusbus[ii, jj] = -capMatrix[bus_index[ii], bus_index[jj]]
 
     # sum of capacitances from each pad to ground
     # this assumes the bus couplers are at "ground"
-    C1S = Cg[0] + np.sum(Cbus[0,])
-    C2S = Cg[1] + np.sum(Cbus[1,])
+    C1S = Cg[0] + np.sum(Cbus[
+        0,
+    ])
+    C2S = Cg[1] + np.sum(Cbus[
+        1,
+    ])
 
     # total capacitance between pads
     tCSq = Cs + C1S * C2S / (C1S + C2S)  # Key equation
 
     # total capacitance of each pad to ground?
     # Note the + in the squared term below !!!
     tCSbus = np.zeros(N)
     for ii in range(N):
         tCSbus[ii] = Cr[ii] - (Cbus[0, ii]+Cbus[1, ii])**2 / \
             (C1S+C2S) + np.sum(Cbus[:, ii]) + np.sum(Cbusbus[ii, :])
 
     # qubit to coupling pad capacitance
-    tCqbus = (C2S * Cbus[0,] - Cbus[1,] * C1S) / (C1S + C2S)
+    tCqbus = (C2S * Cbus[
+        0,
+    ] - Cbus[
+        1,
+    ] * C1S) / (C1S + C2S)
 
     # coupling pad to coupling pad capacitance
     tCqbusbus = np.zeros([N, N])
     for ii in range(N):
         for jj in range(N):
             tCqbusbus[ii, jj] = Cbusbus[ii, jj] + \
                 (Cbus[0, ii]+Cbus[1, ii])*(Cbus[0, jj]+Cbus[1, jj])/(C1S+C2S)
 
     # voltage division ratio
-    bbus = (C2S * Cbus[0,] - Cbus[1,] * C1S) / ((C1S + C2S) * Cs + C1S * C2S)
+    bbus = (C2S * Cbus[
+        0,
+    ] - Cbus[
+        1,
+    ] * C1S) / ((C1S + C2S) * Cs + C1S * C2S)
 
     # total qubit capacitance (including junction capacitance)
     Cq = tCSq + CJ
 
     ########################################################
     ##### Transmon qubit & bus quantum properties
 
@@ -467,54 +479,82 @@
     if do_plots:
 
         # plot using matplotlib (might need to clean this up)
 
         plt.figure()
         plt.subplot(1, 2, 1)
         plt.plot(charge,
-                 elvls[0,] / h / 1e9,
+                 elvls[
+                     0,
+                 ] / h / 1e9,
                  'k',
                  charge,
-                 elvls[1,] / h / 1e9,
+                 elvls[
+                     1,
+                 ] / h / 1e9,
                  'b',
                  charge,
-                 elvls[2,] / h / 1e9,
+                 elvls[
+                     2,
+                 ] / h / 1e9,
                  'r',
                  charge,
-                 elvls[3,] / h / 1e9,
+                 elvls[
+                     3,
+                 ] / h / 1e9,
                  'g',
                  LineWidth=2)
         plt.xlabel('Gate charge, n_g [2e]')
         plt.ylabel('Energy, E_n [GHz]')
         plt.subplot(1, 2, 2)
         plt.plot(charge, (-elvls[1, :] / h + elvls[1, 0] / h) / 1e3, 'k')
         plt.xlabel('Gate charge, n_g [2e]')
         plt.ylabel('Energy [kHz], ')
         plt.show()
 
         plt.figure(2)
         plt.subplot(1, 2, 1)
         plt.plot(
-            charge, 1000 * (elvls[2,] / h / 1e9 - elvls[0,] / h / 1e9 -
-                            2 * elvls[1,] / h / 1e9 - elvls[0,] / h / 1e9),
-            charge, -charge * 0 - 1000 * Ec / h / 1e9)
+            charge, 1000 * (elvls[
+                2,
+            ] / h / 1e9 - elvls[
+                0,
+            ] / h / 1e9 - 2 * elvls[
+                1,
+            ] / h / 1e9 - elvls[
+                0,
+            ] / h / 1e9), charge, -charge * 0 - 1000 * Ec / h / 1e9)
         plt.xlabel('Gate charge, n_g [2e]')
         plt.ylabel('delta [MHZ] green theory, blue numerics ')
         plt.subplot(1, 2, 2)
-        plt.plot(charge, elvls[1,] / h / 1e9 - elvls[0,] / h / 1e9, charge,
-                 charge * 0 + (np.sqrt(8 * EJ * Ec) - Ec) / h / 1e9)
+        plt.plot(charge, elvls[
+            1,
+        ] / h / 1e9 - elvls[
+            0,
+        ] / h / 1e9, charge, charge * 0 + (np.sqrt(8 * EJ * Ec) - Ec) / h / 1e9)
         plt.xlabel('Gate charge, n_g [2e]')
         plt.ylabel('F01 [GHZ] green theory, blue numerics ')
         plt.show()
 
-    fqubitGHz = np.mean(elvls[1,] / h / 1e9)
-    anharMHz = np.mean(1000 * (elvls[2,] / h / 1e9 - elvls[0,] / h / 1e9 -
-                               2 * elvls[1,] / h / 1e9 - elvls[0,] / h / 1e9))
-
-    disp = np.max(-elvls[1,] / h + elvls[1, 0] / h)
+    fqubitGHz = np.mean(elvls[
+        1,
+    ] / h / 1e9)
+    anharMHz = np.mean(1000 * (elvls[
+        2,
+    ] / h / 1e9 - elvls[
+        0,
+    ] / h / 1e9 - 2 * elvls[
+        1,
+    ] / h / 1e9 - elvls[
+        0,
+    ] / h / 1e9))
+
+    disp = np.max(-elvls[
+        1,
+    ] / h + elvls[1, 0] / h)
     tphi_ms = 2 / (2 * np.pi * disp * np.pi * 1e-4 * 1e-3)
 
     if do_disp:
         print('Mean Frequency %f [GHz]' % fqubitGHz)
         print('Anharmonicity %f [MHz]' % anharMHz)
         print('EC %f [GHz]' % (Ec / h / 1e9))
         print('Charge Dispersion %f [kHz]' % (disp / 1e3))
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/quantization/lumped_oscillator_model.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/quantization/lumped_oscillator_model.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/simulation/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/simulation/eigenmode.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/simulation/eigenmode.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/simulation/lumped_elements.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/simulation/lumped_elements.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                          percent_refinement=30,
                          auto_increase_solution_order=True,
                          solution_order='High',
                          solver_type='Iterative')
     """Default setup."""
 
     # supported labels for data generated from the simulation
-    data_labels = ['cap_matrix', 'cap_all_passes', 'units']
+    data_labels = ['cap_matrix', 'cap_all_passes', 'units', 'is_converged']
     """Default data labels."""
 
     def __init__(self, design: 'QDesign' = None, renderer_name: str = 'q3d'):
         """Initialize the class to extract the capacitance matrix.
 
         Args:
             design (QDesign): Pointer to the main qiskit-metal design.
@@ -90,14 +90,16 @@
             # pylint: disable=attribute-defined-outside-init
             # extract main (latest) capacitance matrix
             self.capacitance_matrix, self.units = self.renderer.get_capacitance_matrix(
             )
             # extract the capacitance matrices for all passes
             self.capacitance_all_passes, _ = self.renderer.get_capacitance_all_passes(
             )
+            # extract convergence
+            self.is_converged = self.renderer.get_convergence()
         else:
             self.logger.error(
                 "Please initialize renderer before trying to load the simulation results."
                 " Consider using the method self.renderer._initiate_renderer()"
                 " if you did not already connect qiskit-metal to the renderer.")
 
     def run_sim(  # pylint: disable=arguments-differ
@@ -212,7 +214,30 @@
         """
         if not isinstance(data, str):
             self.logger.warning(
                 'Unsupported type %s. Only accepts str. Please try again.',
                 {type(data)})
             return
         self.set_data('units', data)
+
+    @property
+    def is_converged(self) -> bool:
+        """Getter
+
+        Returns:
+            bool: Boolean indicating whether simulation has converged
+        """
+        return self.get_data('is_converged')
+
+    @is_converged.setter
+    def is_converged(self, data: bool):
+        """Setter
+
+        Args:
+            data (bool): Sets convergence of simulation for
+        """
+        if not isinstance(data, bool):
+            self.logger.warning(
+                'Unsupported type %s. Only accepts boolean. Please try again.',
+                {type(data)})
+            return
+        self.set_data('is_converged', data)
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/simulation/scattering_impedance.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/simulation/scattering_impedance.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/sweep_and_optimize/sweeper.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/sweep_and_optimize/sweeper.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,17 @@
 
             try:
                 self.parent.run(**all_dicts)
             except Exception as ex:
                 template = "An exception of type {0} occurred. Arguments:\n{1!r}"
                 message = template.format(type(ex).__name__, ex.args)
                 self.design.logger.warning(
-                    f'For class {self.parent.__class__.__name__}, run() did not execute as expected: {message}'
-                )
+                    f'For class {self.parent.__class__.__name__}, '
+                    f'option_name={".".join(option_path)}, key={item}, '
+                    f'run() did not execute as expected: {message}')
 
             self.populate_all_sweep(all_sweep, item, args[1])
 
         return all_sweep, 0
 
     # #######  Populate all_sweep
     def populate_all_sweep(self, all_sweep: Dict, item: str, option_name: str):
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/analyses/sweep_and_optimize/sweeping.py` & `qiskit_metal-0.1.5/qiskit_metal/analyses/sweep_and_optimize/sweeping.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/config.py` & `qiskit_metal-0.1.5/qiskit_metal/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,23 +17,35 @@
 """File contains some config definitions.
 
 Mostly internal.
 """
 
 from .toolbox_python.attr_dict import Dict
 from ._defaults import DefaultMetalOptions, DefaultOptionsRenderer
+import os
 
 renderers_to_load = Dict(
     hfss=Dict(path_name='qiskit_metal.renderers.renderer_ansys.hfss_renderer',
               class_name='QHFSSRenderer'),
     q3d=Dict(path_name='qiskit_metal.renderers.renderer_ansys.q3d_renderer',
              class_name='QQ3DRenderer'),
     gds=Dict(path_name='qiskit_metal.renderers.renderer_gds.gds_renderer',
              class_name='QGDSRenderer'),
-)
+    gmsh=Dict(path_name='qiskit_metal.renderers.renderer_gmsh.gmsh_renderer',
+              class_name='QGmshRenderer'),
+    elmer=Dict(path_name='qiskit_metal.renderers.renderer_elmer.elmer_renderer',
+               class_name='QElmerRenderer'),
+    aedt_q3d=Dict(
+        path_name=
+        'qiskit_metal.renderers.renderer_ansys_pyaedt.q3d_renderer_aedt',
+        class_name='QQ3DPyaedt'),
+    aedt_hfss=Dict(
+        path_name=
+        'qiskit_metal.renderers.renderer_ansys_pyaedt.hfss_renderer_aedt',
+        class_name='QHFSSPyaedt'))
 """
 Define the renderes to load. Just provide the module names here.
 """
 
 GUI_CONFIG = Dict(
     load_metal_modules=Dict(Qubits='qiskit_metal.qlibrary.qubits',
                             TLines='qiskit_metal.qlibrary.tlines',
@@ -108,19 +120,15 @@
 
 def is_using_ipython():
     """Check if we're in IPython.
 
     Returns:
         bool -- True if ran in IPython
     """
-    try:
-        __IPYTHON__  # pylint: disable=undefined-variable, pointless-statement
-        return True
-    except NameError:
-        return False
+    return 'JPY_PARENT_PID' in os.environ
 
 
 def is_building_docs():
     """Checks for the existance of the .buildingdocs file which is only present
     when building the docs.
 
     Returns:
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/designs/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/designs/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,14 +37,24 @@
 ---------------
 
 .. autosummary::
     :toctree: ../stubs/
 
     DesignPlanar
 
+
+MultiPlanar
+---------------
+
+.. autosummary::
+    :toctree: ../stubs/
+
+    MultiPlanar
+
+
 DesignFlipChip
 ---------------
 
 .. autosummary::
     :toctree: ../stubs/
 
     DesignFlipChip
@@ -67,10 +77,11 @@
     Components
 """
 
 from .. import Dict
 from .. import is_design
 from .design_base import QDesign
 from .design_planar import DesignPlanar
+from .design_multiplanar import MultiPlanar
 from .design_flipchip import DesignFlipChip
 from .net_info import QNet
 from .interface_components import Components
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/designs/design_base.py` & `qiskit_metal-0.1.5/qiskit_metal/designs/design_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 class QDesign():
     """QDesign is the base class for Qiskit Metal Designs.
 
     A design is the most top-level object in all of Qiskit Metal.
     """
     # pylint: disable=too-many-instance-attributes, too-many-public-methods
 
-    # Dummy private attribute used to check if an instanciated object is
+    # Dummy private attribute used to check if an instantiated object is
     # indeed a QDesign class. The problem is that the `isinstance`
     # built-in method fails when this module is reloaded.
     # Used by `is_design` to check.
     __i_am_design__ = True
 
     def __init__(self,
                  metadata: dict = None,
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/designs/design_flipchip.py` & `qiskit_metal-0.1.5/qiskit_metal/designs/design_flipchip.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/designs/design_planar.py` & `qiskit_metal-0.1.5/qiskit_metal/designs/design_planar.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/designs/interface_components.py` & `qiskit_metal-0.1.5/qiskit_metal/designs/interface_components.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/designs/net_info.py` & `qiskit_metal-0.1.5/qiskit_metal/designs/net_info.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/draw/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/draw/basic.py` & `qiskit_metal-0.1.5/qiskit_metal/draw/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                                           yoff=yoff)
 
 
 def is_rectangle(obj):
     """Test if a shapely object is a rectangle.
 
     If there are 4 ext cooridnate then
-    check if consequtive vectors are orhtogonal.
+    check if consecutive vectors are orthogonal.
     Assumes that the last point is not repeating.
 
     Args:
         obj (object): Object to test
 
     Returns:
         bool: True is object is a rectangle, false otherwise
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/draw/mpl.py` & `qiskit_metal-0.1.5/qiskit_metal/draw/mpl.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/draw/utility.py` & `qiskit_metal-0.1.5/qiskit_metal/draw/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,14 +336,15 @@
         v2 = vec_unit_planar(vector[:2])
         return np.append(v2, vector[2])
 
     else:
         raise Exception('You did not give a 2 or 3 vec')
 
 
+# pylint: disable=invalid-name
 def to_vec3D(list_of_2d_pts: List[Tuple], z=0) -> np.ndarray:
     """Adds 3rd point to list of 2D points. For the given design, get the z
     values in HFSS UNITS! Manually specify z dimension.
 
     Args:
         list_of_2d_pts (List[Tuple]): List of 2D points
         z (int, optional): z-value in hfss. Defaults to 0.
@@ -354,14 +355,31 @@
     add_me = [z]
 
     vec3d = np.array([list(a_2d_pt) + add_me for a_2d_pt in list_of_2d_pts],
                      dtype="object")
     return vec3d
 
 
+def to_vec3D_list(list_of_2d_pts: List[Tuple], z=0) -> list:
+    """Adds 3rd point to list of 2D points. For the given design, get the z
+    values in HFSS UNITS! Manually specify z dimension.
+
+    Args:
+        list_of_2d_pts (List[Tuple]): List of 2D points
+        z (int, optional): z-value in hfss. Defaults to 0.
+
+    Returns:
+        list: vec3d of points
+    """
+    add_me = [z]
+
+    vec3d_list = [list(a_2d_pt) + add_me for a_2d_pt in list_of_2d_pts]
+    return vec3d_list
+
+
 Vec2D = Union[list, np.ndarray]
 
 
 class Vector:
     """Utility functions to call on 2D vectors, which can be np.ndarrays or
     lists."""
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qgeometries/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/qgeometries/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qgeometries/qgeometries_handler.py` & `qiskit_metal-0.1.5/qiskit_metal/qgeometries/qgeometries_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -601,16 +601,16 @@
 
         Args:
             component_id (int): Unique number to describe the component.
         """
         for table_name in self.tables:
             df_table_name = self.tables[table_name]
             # self.tables[table_name] = df_table_name.drop(df_table_name[df_table_name['component'] == component_id].index)
-            self.tables[table_name] = df_table_name[
-                df_table_name['component'] != component_id]
+            self.tables[table_name] = df_table_name[df_table_name['component']
+                                                    != component_id]
 
     def get_component(
         self,
         name: str,
         table_name: str = 'all'
     ) -> Union[GeoDataFrame, Dict_[str, GeoDataFrame]]:
         """Return the table for just a given component. If all, returns a
@@ -778,14 +778,49 @@
                 self.logger.error(
                     f'Element Tables: Tried to access non-existing element table: `{table_name}`'
                 )
             return False
         else:
             return True
 
+    def get_all_unique_layers_for_all_tables(self,
+                                             qcomp_ids: Union[list, None] = None
+                                            ) -> list:
+        """Get a list of all unique layer number used in all of the geometry tables.
+        User can get for all components or a subset.
+
+        Args:
+            qcomp_ids (Union[list, None], optional): The list has integers
+                                        which denote component_id. Defaults to None.
+
+        Returns:
+            list: The unique layer numbers for the list of component ids passed in argument.
+        """
+        if qcomp_ids is None:
+            qcomp_ids = []
+        frames = list()
+        unique_layers = None
+
+        if len(qcomp_ids) == 0:
+            # use all components
+            frames = [self.tables[a_df] for a_df in self.tables]
+        else:
+            # Use just the component ID's in qcomp_ids.
+            for table_key in self.tables:
+                temp_df = self.tables[table_key]
+                mask_temp = temp_df['component'].isin(qcomp_ids)
+                subset_temp_df = temp_df[mask_temp]
+                frames.append(subset_temp_df)
+
+        #Concat the frames and then determine the unique layer numbers.
+        unique_layers = list(
+            pd.concat(frames, ignore_index=True)['layer'].unique())
+
+        return unique_layers
+
     def get_all_unique_layers(self, chip_name: str) -> list:
         """Returns a lit of unique layers for the given chip names.
 
         Args:
             chip_name (str): Name of the chip
 
         Returns:
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,25 @@
 .. autosummary::
     :toctree:
 
     CoupledLineTee
     LineTee
     CapNInterdigitalTee
 	TunableCoupler01
+    TunableCoupler02
+
+
+Resonator
+------------
+
+.. autosummary::
+    :toctree:
+
+    ReadoutResFC
+    ResonatorLumped
 
 
 Terminations
 ----------------
 
 .. autosummary::
     :toctree:
@@ -105,14 +116,15 @@
 
 .. autosummary::
     :toctree:
 
     jj_dolan
     jj_manhattan
     TransmonConcentric
+    TransmonConcentricType2
     TransmonCross
     TransmonCrossFL
     TransmonInterdigitated
     TransmonPocket
     TransmonPocketCL
     TransmonPocket6
     TransmonPocketTeeth
@@ -146,14 +158,15 @@
     from .sample_shapes.n_square_spiral import NSquareSpiral
     from .sample_shapes.rectangle import Rectangle
     from .sample_shapes.rectangle_hollow import RectangleHollow
     from .couplers.coupled_line_tee import CoupledLineTee
     from .couplers.line_tee import LineTee
     from .couplers.cap_n_interdigital_tee import CapNInterdigitalTee
     from .couplers.tunable_coupler_01 import TunableCoupler01
+    from .couplers.tunable_coupler_02 import TunableCoupler02
     from .lumped.cap_n_interdigital import CapNInterdigital
     from .lumped.cap_3_interdigital import Cap3Interdigital
     from .lumped.resonator_coil_rect import ResonatorCoilRect
     from .terminations.launchpad_wb import LaunchpadWirebond
     from .terminations.launchpad_wb_coupled import LaunchpadWirebondCoupled
     from .terminations.launchpad_wb_driven import LaunchpadWirebondDriven
     from .terminations.open_to_ground import OpenToGround
@@ -163,18 +176,21 @@
     from .tlines.meandered import RouteMeander
     from .tlines.anchored_path import RouteAnchors
     from .tlines.mixed_path import RouteMixed
     from .tlines.pathfinder import RoutePathfinder
     from .qubits.JJ_Dolan import jj_dolan
     from .qubits.JJ_Manhattan import jj_manhattan
     from .qubits.transmon_concentric import TransmonConcentric
+    from .qubits.transmon_concentric_type_2 import TransmonConcentricType2
     from .qubits.transmon_cross import TransmonCross
     from .qubits.transmon_cross_fl import TransmonCrossFL
     from .qubits.Transmon_Interdigitated import TransmonInterdigitated
     from .qubits.transmon_pocket import TransmonPocket
     from .qubits.transmon_pocket_cl import TransmonPocketCL
     from .qubits.transmon_pocket_6 import TransmonPocket6
     from .qubits.transmon_pocket_teeth import TransmonPocketTeeth
     from .qubits.SQUID_loop import SQUID_LOOP
     from .qubits.star_qubit import StarQubit
+    from .resonator.readoutres_fc import ReadoutResFC
+    from .resonator.resonator_lumped import ResonatorLumped
 
     from .tlines import anchored_path
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/_template.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/_template.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/core/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/core/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/core/_parsed_dynamic_attrs.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/core/_parsed_dynamic_attrs.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/core/base.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/core/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,16 +245,16 @@
             # if no prefix, use class name
             if "short_name" not in prefix:
                 short_name = self.__class__.__name__[:name_trunc]
             else:
                 short_name = prefix['short_name'][:name_trunc]
             name_id = self.design._get_new_qcomponent_name_id(short_name)
             # rename loop to make sure that no components manually named by the user conflicts
-            while self.design.rename_component(
-                    self._id, short_name + "_" + str(name_id)) != 1:
+            while self.design.rename_component(self._id, short_name + "_" +
+                                               str(name_id)) != 1:
                 name_id = self.design._get_new_qcomponent_name_id(short_name)
 
         # Add keys for each type of table.  add_qgeometry() will update bool if the table is used.
         self.qgeometry_table_usage = Dict()
         self.populate_to_track_table_usage()
 
         # Make the component geometry
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/core/qroute.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/core/qroute.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/core/qubit.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/core/qubit.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/couplers/cap_n_interdigital_tee.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/couplers/cap_n_interdigital_tee.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/couplers/coupled_line_tee.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/couplers/coupled_line_tee.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/couplers/line_tee.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/couplers/line_tee.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/couplers/tunable_coupler_01.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/couplers/tunable_coupler_01.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/lumped/cap_3_interdigital.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/lumped/cap_3_interdigital.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/lumped/cap_n_interdigital.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/lumped/cap_n_interdigital.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/lumped/resonator_coil_rect.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/lumped/resonator_coil_rect.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/JJ_Dolan.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/JJ_Dolan.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/JJ_Manhattan.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/JJ_Manhattan.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/SQUID_loop.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/SQUID_loop.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/Transmon_Interdigitated.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/Transmon_Interdigitated.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/star_qubit.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/star_qubit.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_concentric.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_concentric.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         * fbl_sp: '100um' -- Spacing between metal pad and flux bias loop
         * fbl_gap: '80um' -- Space between parallel lines of the flux bias loop
         * fbl_ext: '300um' -- Run length of flux bias line between circular
           loop and edge of pocket
         * pocket_w: '1500um' -- Transmon pocket width
         * pocket_h: '1000um' -- Transmon pocket height
         * cpw_width: '10.0um' -- Width of the readout resonator and flux bias line
+        * layer: '1' -- the design layer where the component will go
     """
 
     # default drawing options
     default_options = Dict(
         width='1000um',  # width of transmon pocket
         height='1000um',  # height of transmon pocket
         rad_o='170um',  # outer radius
@@ -76,15 +77,16 @@
         fbl_sp='100um',  # spacing between metal pad and flux bias loop
         fbl_gap='80um',  # space between parallel lines of the flux bias loop
         fbl_ext=
         '300um',  # run length of flux bias line between circular loop and edge of pocket
         pocket_w='1500um',  # transmon pocket width
         pocket_h='1000um',  # transmon pocket height
         cpw_width='10.0um',  # width of the readout resonator and flux bias line
-        inductor_width='5.0um'  # width of the Josephson Junctions
+        inductor_width='5.0um',  # width of the Josephson Junctions
+        layer='1'  # design layer
     )
     """Default drawing options"""
 
     TOOLTIP = """The base `TrasmonConcentric` class."""
 
     def make(self):
         """Convert self.options into QGeometry."""
@@ -164,32 +166,32 @@
         geom_inner = {'poly2': inner_pad}
         geom_jjt = {'poly4': jj_t}
         geom_jjb = {'poly5': jj_b}
         geom_pocket = {'poly6': pocket}
 
         self.add_qgeometry('path',
                            geom_rr,
-                           layer=1,
+                           layer=p.layer,
                            subtract=False,
                            width=p.cpw_width)
         self.add_qgeometry('path',
                            geom_fbl,
-                           layer=1,
+                           layer=p.layer,
                            subtract=False,
                            width=p.cpw_width)
-        self.add_qgeometry('poly', geom_outer, layer=1, subtract=False)
-        self.add_qgeometry('poly', geom_inner, layer=1, subtract=False)
+        self.add_qgeometry('poly', geom_outer, layer=p.layer, subtract=False)
+        self.add_qgeometry('poly', geom_inner, layer=p.layer, subtract=False)
         self.add_qgeometry('junction',
                            geom_jjt,
-                           layer=1,
+                           layer=p.layer,
                            subtract=False,
                            width=p.inductor_width)
         self.add_qgeometry('junction',
                            geom_jjb,
-                           layer=1,
+                           layer=p.layer,
                            subtract=False,
                            width=p.inductor_width)
         self.add_qgeometry('poly', geom_pocket, layer=1, subtract=True)
 
         ###########################################################################
 
         # Add Qpin connections
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_cross.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_cross.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,16 @@
         chip='main',
         _default_connection_pads=Dict(
             connector_type='0',  # 0 = Claw type, 1 = gap type
             claw_length='30um',
             ground_spacing='5um',
             claw_width='10um',
             claw_gap='6um',
+            claw_cpw_length='40um',
+            claw_cpw_width='10um',
             connector_location=
             '0'  # 0 => 'west' arm, 90 => 'north' arm, 180 => 'east' arm
         ))
     """Default options."""
 
     component_metadata = Dict(short_name='Cross',
                               _qgeometry_table_poly='True',
@@ -171,40 +173,43 @@
         # access to chip name
         chip = p.chip
 
         pc = self.p.connection_pads[name]  # parser on connector options
         c_g = pc.claw_gap
         c_l = pc.claw_length
         c_w = pc.claw_width
+        c_c_w = pc.claw_cpw_width
+        c_c_l = pc.claw_cpw_length
         g_s = pc.ground_spacing
         con_loc = pc.connector_location
 
-        claw_cpw = draw.box(0, -c_w / 2, -4 * c_w, c_w / 2)
+        claw_cpw = draw.box(-c_w, -c_c_w / 2, -c_c_l - c_w, c_c_w / 2)
 
         if pc.connector_type == 0:  # Claw connector
             t_claw_height = 2*c_g + 2 * c_w + 2*g_s + \
                 2*cross_gap + cross_width  # temp value
 
             claw_base = draw.box(-c_w, -(t_claw_height) / 2, c_l,
                                  t_claw_height / 2)
             claw_subtract = draw.box(0, -t_claw_height / 2 + c_w, c_l,
                                      t_claw_height / 2 - c_w)
             claw_base = claw_base.difference(claw_subtract)
 
             connector_arm = draw.shapely.ops.unary_union([claw_base, claw_cpw])
             connector_etcher = draw.buffer(connector_arm, c_g)
         else:
-            connector_arm = claw_cpw
+            connector_arm = draw.box(0, -c_w / 2, -4 * c_w, c_w / 2)
             connector_etcher = draw.buffer(connector_arm, c_g)
 
         # Making the pin for  tracking (for easy connect functions).
         # Done here so as to have the same translations and rotations as the connector. Could
         # extract from the connector later, but since allowing different connector types,
         # this seems more straightforward.
-        port_line = draw.LineString([(-4 * c_w, -c_w / 2), (-4 * c_w, c_w / 2)])
+        port_line = draw.LineString([(-c_c_l - c_w, -c_c_w / 2),
+                                     (-c_c_l - c_w, c_w / 2)])
 
         claw_rotate = 0
         if con_loc > 135:
             claw_rotate = 180
         elif con_loc > 45:
             claw_rotate = -90
 
@@ -221,8 +226,8 @@
         self.add_qgeometry('poly', {f'{name}_connector_arm': connector_arm},
                            chip=chip)
         self.add_qgeometry('poly',
                            {f'{name}_connector_etcher': connector_etcher},
                            subtract=True,
                            chip=chip)
 
-        self.add_pin(name, port_line.coords, c_w)
+        self.add_pin(name, port_line.coords, c_c_w)
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_cross_fl.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_cross_fl.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_pocket.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_pocket.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_pocket_6.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_pocket_6.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_pocket_cl.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_pocket_cl.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/qubits/transmon_pocket_teeth.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/qubits/transmon_pocket_teeth.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/circle_caterpillar.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/circle_caterpillar.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/circle_raster.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/circle_raster.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/n_gon.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/n_gon.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/n_square_spiral.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/n_square_spiral.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/rectangle.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/rectangle.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/rectangle_hollow.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/rectangle_hollow.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/sample_shapes/smiley_face.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/sample_shapes/smiley_face.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/terminations/launchpad_wb.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/terminations/launchpad_wb.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/terminations/launchpad_wb_coupled.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/terminations/launchpad_wb_coupled.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/terminations/launchpad_wb_driven.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/terminations/launchpad_wb_driven.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/terminations/open_to_ground.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/terminations/open_to_ground.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/terminations/short_to_ground.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/terminations/short_to_ground.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/anchored_path.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/anchored_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,21 +310,21 @@
                 if (end_direction is None) or (mao.dot(end_direction,
                                                        corner1 - end) >= 0):
                     return np.expand_dims(corner1, axis=0)
             if (mao.dot(start_direction, corner2 - start) >= 0) and startc2end:
                 if (end_direction is None) or (mao.dot(end_direction,
                                                        corner2 - end) >= 0):
                     return np.expand_dims(corner2, axis=0)
-            if (mao.dot(start_direction, corner3 - start) >=
-                    0) and startc3c4end:
+            if (mao.dot(start_direction, corner3 - start)
+                    >= 0) and startc3c4end:
                 if (end_direction is None) or (mao.dot(end_direction,
                                                        corner4 - end) >= 0):
                     return np.vstack((corner3, corner4))
-            if (mao.dot(start_direction, corner5 - start) >=
-                    0) and startc5c6end:
+            if (mao.dot(start_direction, corner5 - start)
+                    >= 0) and startc5c6end:
                 if (end_direction is None) or (mao.dot(end_direction,
                                                        corner6 - end) >= 0):
                     return np.vstack((corner5, corner6))
         raise QiskitMetalDesignError(
             "connect_simple() has failed. This might be due to one of two reasons. "
             f"1. Either one of the start point {start} or the end point {end} "
             "provided are inside the bounding box of another QComponent. "
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/framed_path.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/framed_path.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/meandered.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/meandered.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/mixed_path.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/mixed_path.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/pathfinder.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/pathfinder.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/tlines/straight_path.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/tlines/straight_path.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/qlibrary/user_components/my_qcomponent.py` & `qiskit_metal-0.1.5/qiskit_metal/qlibrary/user_components/my_qcomponent.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,14 +60,31 @@
 
 .. autosummary::
     :toctree: ../stubs/
 
     QAnsysRenderer
     QHFSSRenderer
     QQ3DRenderer
+    QPyaedt
+    QQ3DPyaedt
+    QHFSSPyaedt
+    QHFSSDrivenmodalPyaedt
+    QHFSSEigenmodePyaedt
+
+
+
+GMSH Renderer
+---------------
+
+.. autosummary::
+    :toctree: ../stubs/
+
+    QGmshRenderer
+    Vec3DArray
+
 
 
 """
 
 from .setup_default import setup_renderers
 
 from .. import config
@@ -88,7 +105,16 @@
 
     from .renderer_mpl import mpl_interaction
     from .renderer_mpl import mpl_toolbox
 
     from .renderer_ansys.ansys_renderer import QAnsysRenderer
     from .renderer_ansys.hfss_renderer import QHFSSRenderer
     from .renderer_ansys.q3d_renderer import QQ3DRenderer
+
+    from .renderer_gmsh.gmsh_utils import Vec3DArray
+    from .renderer_gmsh.gmsh_renderer import QGmshRenderer
+
+    from .renderer_ansys_pyaedt.pyaedt_base import QPyaedt
+    from .renderer_ansys_pyaedt.q3d_renderer_aedt import QQ3DPyaedt
+    from .renderer_ansys_pyaedt.hfss_renderer_aedt import QHFSSPyaedt
+    from .renderer_ansys_pyaedt.hfss_renderer_drivenmodal_aedt import QHFSSDrivenmodalPyaedt
+    from .renderer_ansys_pyaedt.hfss_renderer_eigenmode_aedt import QHFSSEigenmodePyaedt
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_ansys/ansys_renderer.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys/ansys_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import pyEPR as epr
 from pyEPR.ansys import parse_units, HfssApp, release
 
 from qiskit_metal.draw.utility import to_vec3D
 from qiskit_metal.draw.basic import is_rectangle
 from qiskit_metal.renderers.renderer_base import QRendererAnalysis
 from qiskit_metal.toolbox_metal.parsing import is_true
+from qiskit_metal.designs.design_base import QDesign
 
 from qiskit_metal import Dict
 
 from .. import config
 
 if not config.is_building_docs():
     from qiskit_metal.toolbox_python.utility_functions import (
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_ansys/hfss_renderer.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys/hfss_renderer.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_ansys/parse.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys/parse.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_ansys/q3d_renderer.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_ansys/q3d_renderer.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-from typing import List, Union
+from typing import List, Tuple, Union
 
 import pandas as pd
 from collections import defaultdict
 
 import pyEPR as epr
 from pyEPR.ansys import ureg
 from pyEPR.reports import _plot_q3d_convergence_main, _plot_q3d_convergence_chi_f
@@ -439,14 +439,166 @@
         """
         (deprecated) use analysis.quantitative.capacitance_lom.run_lom()
         """
         self.logger.warning(
             'This method is deprecated. Change your scripts to use'
             'analysis.quantitative.capacitance_lom.run_lom()')
 
+    def get_convergence(self) -> bool:
+        """Extracts convergence from Ansys simulation result
+        """
+        # If 'LastAdaptive' is used, then the pass_number won't affect anything.
+        # If 'AdaptivePass' is used, then the pass_number is used.
+        convergence_df, convergence_txt = self._pinfo.setup.get_convergence()
+        target, current, pass_min = self._parse_text_from_q3d_convergence(
+            convergence_txt)
+        is_converged = self._test_if_q3d_analysis_converged(
+            target, current, pass_min)
+
+        return is_converged
+
+    def _test_if_q3d_analysis_converged(cls, target: float, current: float,
+                                        passes_min: int) -> Union[bool, None]:
+        """Use solution-data from Ansys-Q3d to determine if converged.
+
+        Args:
+            target (float): Delta percentage for target. Default is None.
+            current (float): Delta percentage for current. Default is None.
+            passes_min (int): Regarding convergence, minimum number of passes.
+              Default is None.
+
+        Returns:
+            Union[bool, None]: Had solution data converged.  Default is None.
+        """
+
+        if None not in (target, current, passes_min):
+            # Confirm that all three numbers have an value.
+            if current <= target and passes_min > 1:
+                is_converged = True
+                return is_converged
+            is_converged = False
+            return is_converged
+
+        is_converged = None
+        return is_converged
+
+    def _parse_text_from_q3d_convergence(
+            self,
+            gui_text: str) -> Tuple[Union[None, float], Union[None, float]]:
+        """Parse gui_text using a priori known formatting. Ansys-Q3D
+        solution-data provides gui_text.
+
+        Args:
+            gui_text (str): From Ansys-GUI-SolutionData.
+
+        Returns:
+            1st Union[None, float]: Delta percentage for target. Default is None.
+            2nd Union[None, float]: Delta percentage for current. Default is None.
+        """
+
+        text_list = gui_text.splitlines()
+
+        # Find Target information in text.
+        target_all = [string for string in text_list if 'Target' in string]
+
+        # Find Current information in text.
+        current_all = [string for string in text_list if 'Current' in string]
+
+        # Find Minimum number of passes from solution-data.
+        min_passes_all = [string for string in text_list if 'Minimum' in string]
+
+        target = self._extract_target_delta(target_all)
+        current = self._extract_current_delta(current_all)
+        min_passes = self._extract_min_passes(min_passes_all)
+
+        return target, current, min_passes
+
+    def _extract_min_passes(self, min_passes_all: list) -> Union[None, float]:
+        """Given a pre-formatted list, search and return the "Minimum Number
+        Of Passes."
+
+        Args:
+            min_passes_all (list): Result of search through string returned from Ansys-Q3D.
+
+        Returns:
+            Union[None, float]: Regarding convergence, minimum number of passes.
+              Default is None.
+        """
+
+        min_num_of_passes = None
+        if len(min_passes_all) == 1:
+            if min_passes_all[0]:
+                _, _, min_passes_str = min_passes_all[0].partition(':')
+                try:
+                    min_num_of_passes = int(min_passes_str)
+                except ValueError:
+                    self.design.logger.warning(
+                        f'Target={min_passes_str} in GUI is not an int.'
+                        'Force Minimum Number Of Passes to be None.')
+        else:
+            self.design.logger.warning(
+                'Either could not find Minimum Number of Passes '
+                'information or too many entries in text. '
+                'Force Minimum Number of Passes to be None.')
+        return min_num_of_passes
+
+    def _extract_target_delta(self, target_all: list) -> Union[None, float]:
+        """Given a pre-formatted list, search and return the target-delta
+        percentage for convergence.
+
+        Args:
+            target_all (list): Result of search through string returned from Ansys-Q3D.
+
+        Returns:
+            Union[None, float]: Delta percentage for target. Default is None.
+        """
+
+        target = None
+        if len(target_all) == 1:
+            if target_all[0]:
+                _, _, target_str = target_all[0].partition(':')
+                try:
+                    target = float(target_str)
+                except ValueError:
+                    self.design.logger.warning(
+                        f'Target={target_str} in GUI is not a float.'
+                        'Force Target Delta to be None.')
+        else:
+            self.design.logger.warning(
+                'Either could not find Target Delta information or too many '
+                'entries in text. Force Target Delta to be None.')
+        return target
+
+    def _extract_current_delta(self, current_all: list) -> Union[None, float]:
+        """Given a pre-formatted list, search and return the current-delta
+        percentage for convergence.
+
+        Args:
+            current_all (list): Result of search through string returned from Ansys-Q3D.
+
+        Returns:
+            Union[None, float]: Delta percentage for current. Default is None.
+        """
+
+        current = None
+        if len(current_all) == 1:
+            if current_all[0]:
+                _, _, current_str = current_all[0].partition(':')
+                try:
+                    current = float(current_str)
+                except ValueError:
+                    self.design.logger.warning(
+                        f'Target={current_str} in GUI is not a float.'
+                        'Force Current Delta to be None.')
+        else:
+            self.design.logger.warning(
+                'Either could not find Current Delta information or too many '
+                'entries in text. Force Current Delta to be None.')
+        return current
+
     def plot_convergence_main(self, RES: pd.DataFrame):
         """Plot alpha and frequency versus pass number, as well as convergence
         of delta (in %).
 
         Args:
             RES (pd.DataFrame): Dictionary of capacitance matrices versus pass number, organized as pandas table.
         """
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_base/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_base/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_base/renderer_base.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_base/renderer_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,15 +417,18 @@
         unique components to be sent to the renderer. The second returned item, an
         integer, specifies which of these 3 cases applies.
 
         Args:
             highlight_qcomponents (Union[list, None], optional): Components to render. Defaults to None.
 
         Returns:
-            Tuple[list, int]: Empty or partial list of components in QDesign.
+            Tuple[list, int]: Tuple: Empty or partial list of components in QDesign.
+                            int: 0 subset selected
+                                 1 every component selected
+                                 2 invalid
         """
         highlight_qcomponents = highlight_qcomponents if highlight_qcomponents else []
         unique_qcomponents = set(highlight_qcomponents)
         for qcomp in unique_qcomponents:
             if qcomp not in self.design.name_to_id:
                 self.logger.warning(
                     f'The component={qcomp} in highlight_qcomponents not'
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_base/renderer_gui_base.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_base/renderer_gui_base.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_base/rndr_analysis.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_base/rndr_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_gds/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_gds/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_gds/gds_renderer.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_gds/gds_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
         Args:
             design (QDesign): Use QGeometry within QDesign  to obtain elements
                             for GDS file.
             initiate (bool, optional): True to initiate the renderer.
                                         Defaults to True.
             render_template (Dict, optional): Typically used by GUI for
                                 template options for GDS.  Defaults to None.
-            render_options (Dict, optional): Used to overide all options.
+            render_options (Dict, optional): Used to override all options.
                                             Defaults to None.
         """
 
         super().__init__(design=design,
                          initiate=initiate,
                          render_template=render_template,
                          render_options=render_options)
@@ -321,14 +321,17 @@
 
         # Updated each time export_to_gds() is called.
         self.chip_info = dict()
 
         # check the scale
         self._check_bounding_box_scale()
 
+        # if imported, hold the path to file name, otherwise None.
+        self.imported_junction_gds = None
+
         QGDSRenderer.load()
 
     def _initiate_renderer(self):
         """Not used by the gds renderer at this time. only returns True.
         """
         return True
 
@@ -336,15 +339,14 @@
         """Not used by the gds renderer at this time. only returns True.
         """
         return True
 
     def render_design(self):
         """Export the design to GDS."""
         self.export_to_gds(file_name=self.design.name, highlight_qcomponents=[])
-        pass
 
     def _check_bounding_box_scale(self):
         """Some error checking for bounding_box_scale_x and
         bounding_box_scale_y numbers."""
         bounding_box_scale_x = self.parse_value(
             self.options.bounding_box_scale_x)
         bounding_box_scale_y = self.parse_value(
@@ -416,19 +418,20 @@
 
         setattr(self, f'{chip_name}_{table_name}_subtract_true', subtract_true)
         setattr(self, f'{chip_name}_{table_name}_subtract_false',
                 subtract_false)
 
     @staticmethod
     def _get_bounds(
-            gs_table: geopandas.GeoSeries) -> Tuple[float, float, float, float]:
+            gs_table: geopandas.GeoDataFrame
+    ) -> Tuple[float, float, float, float]:
         """Get the bounds for all of the elements in gs_table.
 
         Args:
-            gs_table (pandas.GeoSeries): A pandas GeoSeries used to describe
+            gs_table (geopandas.GeoDataFrame): A GeoPandas GeoDataFrame used to describe
                                         components in a design.
 
         Returns:
             Tuple[float, float, float, float]: The bounds of all of the
             elements in this table. [minx, miny, maxx, maxy]
         """
         if len(gs_table) == 0:
@@ -526,15 +529,15 @@
         self.dict_bounds[chip_name]['scaled_box'] = scaled_box
         self.dict_bounds[chip_name]['inclusive_box'] = (minx, miny, maxx, maxy)
 
         return scaled_box, (minx, miny, maxx, maxy)
 
     def _check_qcomps(self,
                       highlight_qcomponents: list = None) -> Tuple[list, int]:
-        """Confirm the list doesn't have names of components repeated. Comfirm
+        """Confirm the list doesn't have names of components repeated. Confirm
         that the name of component exists in QDesign.
 
         Args:
             highlight_qcomponents (list, optional): List of strings which
                                         denote the name of QComponents to render.
                                         Empty list means to render entire design.
                                         Defaults to [].
@@ -573,15 +576,15 @@
         return unique_qcomponents, 0
 
     def _create_qgeometry_for_gds(self,
                                   highlight_qcomponents: list = None) -> int:
         """Using self.design, this method does the following:
 
         1. Gather the QGeometries to be used to write to file.
-           Duplicate names in hightlight_qcomponents will be removed without
+           Duplicate names in highlight_qcomponents will be removed without
            warning.
 
         2. Populate self.dict_bounds, for each chip, contains the maximum bound
            for all elements to render.
 
         3. Calculate scaled bounding box to emulate size of chip using
            self.bounding_box_scale(x and y) and place into
@@ -603,15 +606,15 @@
         if highlight_qcomponents is None:
             highlight_qcomponents = []
         unique_qcomponents, status = self._check_qcomps(highlight_qcomponents)
         if status == 1:
             return 1
         self.dict_bounds.clear()
 
-        for chip_name in self.chip_info:
+        for chip_name, _ in self.chip_info.items():
             # put the QGeometry into GDS format.
             # There can be more than one chip in QGeometry.
             # They all export to one gds file.
             self.chip_info[chip_name]['all_subtract'] = []
             self.chip_info[chip_name]['all_no_subtract'] = []
 
             self.dict_bounds[chip_name] = Dict()
@@ -628,15 +631,15 @@
                                         chip_name)
 
                 if table_name == 'junction':
                     self.chip_info[chip_name]['junction'] = deepcopy(table)
                 else:
                     # For every chip, and layer, separate the "subtract"
                     # and "no_subtract" elements and gather bounds.
-                    # dict_bounds[chip_name] = list_bounds
+                    # self.dict_bounds[chip_name] = list_bounds
                     self._gather_subtract_elements_and_bounds(
                         chip_name, table_name, table, all_table_subtracts,
                         all_table_no_subtracts)
 
             # If list of QComponents provided, use the
             # bounding_box_scale(x and y), otherwise use self._chips.
             scaled_max_bound, max_bound = self._scale_max_bounds(
@@ -728,15 +731,15 @@
     # Handling Fillet issues.
 
     def _fix_short_segments_within_table(self, chip_name: str, chip_layer: int,
                                          all_sub_true_or_false: str):
         """Update self.chip_info geopandas.GeoDataFrame.
 
         Will iterate through the rows to examine the LineString.
-        Then determine if there is a segment that is shorter than the critera
+        Then determine if there is a segment that is shorter than the criteria
         based on default_options. If so, then remove the row, and append
         shorter LineString with no fillet, within the dataframe.
 
         Args:
             chip_name (str): The name of chip.
             chip_layer (int): The layer within the chip to be evaluated.
             all_sub_true_or_false (str): To be used within self.chip_info:
@@ -780,21 +783,21 @@
                 all_sub_true_or_false] = df_copy.copy(deep=True)
 
     def _check_length(self, a_shapely: shapely.geometry.LineString,
                       a_fillet: float) -> Tuple[int, Dict]:
         """Determine if a_shapely has short segments based on scaled fillet
         value.
 
-        Use check_short_segments_by_scaling_fillet to determine the critera
+        Use check_short_segments_by_scaling_fillet to determine the criteria
         for flagging a segment.  Return Tuple with flagged segments.
 
         The "status" returned in int:
             * -1: Method needs to update the return code.
             * 0: No issues, no short segments found
-            * int: The number of shapelys returned. New shapeleys, should
+            * int: The number of shapelys returned. New shapelys, should
                     replace the ones provided in a_shapely
 
         The "shorter_lines" returned in dict:
         key: Using the index values from list(a_shapely.coords)
         value: dict() for each new, shorter, LineString
 
         The dict()
@@ -961,15 +964,15 @@
 
         Dictionary:
             Key 'reduced_idx' will hold list of tuples.
                     The tuples correspond to index for list named "coords".
             Key 'midpoints' will hold list of tuples.
                     The index of a tuple corresponds to two index within coords.
             For example, a index in midpoints is x,
-            that coresponds midpoint of segment x-1 to x.
+            that corresponds midpoint of segment x-1 to x.
         """
 
         # Depreciated since there is no longer a scale factor
         # given to QCheckLength.
         # fillet_scale_factor = self.parse_value(
         #     self.options.check_short_segments_by_scaling_fillet)
 
@@ -1348,15 +1351,15 @@
         no_cheese_buffer = float(self.parse_value(
             self.options.no_cheese.buffer))
         sub_layer = int(self.parse_value(self.options.no_cheese.datatype))
         lib = self.lib
 
         fab = is_true(self.options.fabricate)
 
-        for chip_name in self.chip_info:
+        for chip_name, _ in self.chip_info.items():
             layers_in_chip = self.design.qgeometry.get_all_unique_layers(
                 chip_name)
 
             for chip_layer in layers_in_chip:
                 code = self._check_either_cheese(chip_name, chip_layer)
 
                 if code in (1, 2, 3):
@@ -1418,15 +1421,15 @@
             chip_name (str): Name of chip.
             no_cheese_buffer (float): Will be used for fillet and
                 size of buffer.
 
         Returns:
             Union[None, shapely.geometry.multipolygon.MultiPolygon]: The
             shapely which combines the polygons and linestrings and creates
-            buffer as specificed through default_options.
+            buffer as specified through default_options.
         """
         # pylint: disable=too-many-locals
         style_cap = int(self.parse_value(self.options.no_cheese.cap_style))
         style_join = int(self.parse_value(self.options.no_cheese.join_style))
 
         poly_sub_df = sub_df[sub_df.geometry.apply(
             lambda x: isinstance(x, shapely.geometry.polygon.Polygon))]
@@ -1515,15 +1518,15 @@
 
         lib = self.new_gds_library()
 
         if is_true(self.options.ground_plane):
             all_chips_top_name = 'TOP'
             all_chips_top = lib.new_cell(all_chips_top_name,
                                          overwrite_duplicate=True)
-            for chip_name in self.chip_info:
+            for chip_name, _ in self.chip_info.items():
                 chip_only_top_name = f'TOP_{chip_name}'
                 chip_only_top = lib.new_cell(chip_only_top_name,
                                              overwrite_duplicate=True)
 
                 layers_in_chip, rectangle_points = self._get_rectangle_points(
                     chip_name)
 
@@ -1732,20 +1735,20 @@
 
         if ground_cell.get_bounding_box() is not None:
             chip_only_top.add(gdspy.CellReference(ground_cell))
         else:
             lib.remove(ground_cell)
 
     def _get_linestring_characteristics(
-            self, row: 'pandas.Pandas') -> Tuple[Tuple, float, float]:
+            self, row: 'pd.Pandas') -> Tuple[Tuple, float, float]:
         """Given a row in the Junction table, give the characteristics of
         LineString in row.geometry.
 
         Args:
-            row (pandas.Pandas): A row from Junction table of QGeometry.
+            row (pd.Pandas): A row from Junction table of QGeometry.
 
         Returns:
             Tuple:
             * 1st entry is Tuple[float,float]: The midpoint of Linestring from
             row.geometry in format (x,y).
             * 2nd entry is float: The angle in degrees of Linestring from
             row.geometry.
@@ -1762,22 +1765,21 @@
         magnitude = np.round(
             distance.euclidean(row.geometry.coords[0], row.geometry.coords[1]),
             for_rounding)
 
         return center, rotation, magnitude
 
     def _give_rotation_center_twopads(
-            self, row: 'pandas.Pandas',
-            a_cell_bounding_box: 'numpy.ndarray') -> Tuple:
+            self, row: 'pd.Pandas', a_cell_bounding_box: 'np.ndarray') -> Tuple:
         """Calculate the angle for rotation, center of LineString in
         row.geometry, and if needed create two pads to connect the junction to
         qubit.
 
         Args:
-            row (pandas.Pandas): A row from Junction table of QGeometry.
+            row (pd.Pandas): A row from Junction table of QGeometry.
             a_cell_bounding_box (numpy.ndarray): Give the bounding box of cell
                 used in row.gds_cell_name.
 
         Returns:
             Tuple:
             * 1st entry is float: The angle in degrees of Linestring from
             row.geometry.
@@ -1832,14 +1834,46 @@
                 datatype=10)
 
         return rotation, center, pad_left, pad_right
 
 
 ############
 
+    def _import_junction_gds_file(self, lib: gdspy.library,
+                                  directory_name: str) -> bool:
+        """Import the file which contains all junctions for design.
+        If the file has already been imported, just return True.
+
+        When the design has junctions on multiple chips,
+        we only need to import file once to get ALL of the junctions.
+
+        Args:
+            lib (gdspy.library): The library used to export the entire QDesign.
+            directory_name (str): The path of directory to read file with junctions.
+
+        Returns:
+            bool: True if file imported to GDS lib or previously imported.
+                   False if file not found.
+        """
+
+        if self.imported_junction_gds is not None:
+            return True
+
+        if os.path.isfile(self.options.path_filename):
+            lib.read_gds(self.options.path_filename, units='convert')
+            self.imported_junction_gds = self.options.path_filename
+            return True
+        else:
+            message_str = (
+                f'Not able to find file:"{self.options.path_filename}".  '
+                f'Not used to replace junction.'
+                f' Checked directory:"{directory_name}".')
+            self.logger.warning(message_str)
+            return False
+
     def _import_junctions_to_one_cell(self, chip_name: str, lib: gdspy.library,
                                       chip_only_top: gdspy.library.Cell,
                                       layers_in_chip: list):
         """Given lib, import the gds file from default options.  Based on the
         cell name in QGeometry table, import the cell from the gds file and
         place it in hierarchy of chip_only_top. In addition, the linestring
         should be two vertexes, and denotes two things.
@@ -1861,16 +1895,17 @@
 
         # Make sure the file exists, before trying to read it.
         dummy_status, directory_name = can_write_to_path(
             self.options.path_filename)
         layers_in_junction_table = set(
             self.chip_info[chip_name]['junction']['layer'])
 
-        if os.path.isfile(self.options.path_filename):
-            lib.read_gds(self.options.path_filename, units='convert')
+        if self._import_junction_gds_file(lib=lib,
+                                          directory_name=directory_name):
+
             for iter_layer in layers_in_chip:
                 if self._is_negative_mask(chip_name, iter_layer):
                     # Want to export negative mask
                     # Gather the pads into hold_all_pads_cell for same layer.
                     if iter_layer in layers_in_junction_table:
                         chip_only_top_layer_name = f'TOP_{chip_name}_{iter_layer}'
                         if chip_only_top_layer_name in lib.cells.keys():
@@ -1883,15 +1918,15 @@
                                 gdspy.CellReference(hold_all_pads_cell))
 
                             # Put all junctions into one cell for same layer.
                             hold_all_jj_cell_name = f'all_jj_imported_{iter_layer}'
                             hold_all_jj_cell = lib.new_cell(
                                 hold_all_jj_cell_name, overwrite_duplicate=True)
 
-                            self._add_negative_extention_to_jj(
+                            self._add_negative_extension_to_jj(
                                 chip_name, iter_layer, lib, chip_only_top,
                                 chip_only_top_layer, hold_all_pads_cell,
                                 hold_all_jj_cell)
                 else:
                     # By default, make a positive mask.
                     for row in self.chip_info[chip_name]['junction'].itertuples(
                     ):
@@ -1900,37 +1935,31 @@
 
                         if ground_cell_name in lib.cells.keys(
                         ) and chip_layer == iter_layer:
                             chip_layer_cell = lib.cells[ground_cell_name]
 
                             if row.gds_cell_name in lib.cells.keys():
                                 # When positive mask, just add the pads to chip_only_top
-                                self._add_positive_extention_to_jj(
+                                self._add_positive_extension_to_jj(
                                     lib, row, chip_layer_cell)
                             else:
                                 self.logger.warning(
                                     f'From the "junction" table, the cell named'
                                     f' "{row.gds_cell_name}"",  is not in '
                                     f'file: {self.options.path_filename}.'
                                     f' The cell was not used.')
 
-        else:
-            self.logger.warning(
-                f'Not able to find file:"{self.options.path_filename}".  '
-                f'Not used to replace junction.'
-                f' Checked directory:"{directory_name}".')
-
-    def _add_negative_extention_to_jj(self, chip_name: str, jj_layer: int,
+    def _add_negative_extension_to_jj(self, chip_name: str, jj_layer: int,
                                       lib: gdspy.library,
                                       chip_only_top: gdspy.library.Cell,
                                       chip_only_top_layer: gdspy.library.Cell,
                                       hold_all_pads_cell: gdspy.library.Cell,
                                       hold_all_jj_cell: gdspy.library.Cell):
         """Manipulate existing geometries for the layer that the junctions need
-         to be added.  Since boolean subtaction is computationally intensive,
+         to be added.  Since boolean subtraction is computationally intensive,
          the method will gather the pads for a layer, and do the boolean just
          once. Then add the junctions to difference.
 
         Args:
             chip_name (str): The name of chip.
             jj_layer (int): The layer the
             lib (gdspy.library): The library used to export the entire QDesign.
@@ -1946,15 +1975,15 @@
             'layer'] == jj_layer
         for row in self.chip_info[chip_name]['junction'][
                 boolean_by_layer].itertuples():
 
             if row.gds_cell_name in lib.cells.keys():
                 # For negative mask, collect the pads to subtract per layer,
                 # and subtract from chip_only_top_layer
-                self._gather_negative_extention_for_jj(lib, row,
+                self._gather_negative_extension_for_jj(lib, row,
                                                        hold_all_pads_cell,
                                                        hold_all_jj_cell)
             else:
                 self.logger.warning(
                     f'From the "junction" table, the cell named'
                     f' "{row.gds_cell_name}",  is not in file: '
                     f'{self.options.path_filename}. The cell was not used.')
@@ -2008,26 +2037,26 @@
         else:
             lib.remove(diff_pad_cell_layer)
         # remove the sub libs before removing hold_all_pads_cells
         for _, value in enumerate(hold_all_pads_cell.references):
             lib.remove(value.ref_cell.name)
         lib.remove(hold_all_pads_cell)
 
-    def _gather_negative_extention_for_jj(
-            self, lib: gdspy.library, row: 'pandas.core.frame.Pandas',
+    def _gather_negative_extension_for_jj(
+            self, lib: gdspy.library, row: 'pd.core.frame.Pandas',
             hold_all_pads_cell: gdspy.library.Cell,
             hold_all_jj_cell: gdspy.library.Cell):
-        """Gather the pads and jjs and put them in seprate cells.  The
+        """Gather the pads and jjs and put them in separate cells.  The
         the pads can be boolean'd 'not' just once. After boolean for pads, then
         the jjs will be added to result.  The boolean is very
         time intensive, so just want to do it once.
 
         Args:
             lib (gdspy.library): The library used to export the entire QDesign.
-            row (pandas.core.frame.Pandas): Each row is from the qgeometry junction table.
+            row (pd.core.frame.Pandas): Each row is from the qgeometry junction table.
             hold_all_pads_cell (gdspy.library.Cell): Collect all the pads with movement.
             hold_all_jj_cell (gdspy.library.Cell): Collect all the jj's with movement.
         """
 
         a_cell = lib.extract(row.gds_cell_name)
         a_cell_bounding_box = a_cell.get_bounding_box()
 
@@ -2044,23 +2073,23 @@
             temp_cell.add(pad_right)
 
         hold_all_jj_cell.add(
             gdspy.CellReference(a_cell, origin=center, rotation=rotation))
         hold_all_pads_cell.add(
             gdspy.CellReference(temp_cell, origin=center, rotation=rotation))
 
-    def _add_positive_extention_to_jj(self, lib: gdspy.library,
-                                      row: 'pandas.core.frame.Pandas',
+    def _add_positive_extension_to_jj(self, lib: gdspy.library,
+                                      row: 'pd.core.frame.Pandas',
                                       chip_only_top_layer: gdspy.library.Cell):
-        """Get the extention pads, then add or subtract to extracted cell based on
+        """Get the extension pads, then add or subtract to extracted cell based on
         positive or negative mask.
 
         Args:
             lib (gdspy.library): The library used to export the entire QDesign.
-            row (pandas.core.frame.Pandas): Each row is from the qgeometry
+            row (pd.core.frame.Pandas): Each row is from the qgeometry
                                             junction table.
             chip_only_top_layer (gdspy.library.Cell): The cell used for
                                             chip_name and layer_num.
         """
         a_cell = lib.extract(row.gds_cell_name)
         a_cell_bounding_box = a_cell.get_bounding_box()
 
@@ -2122,14 +2151,17 @@
         # Each chip will hold the rectangle for subtract for each layer so:
         # chip_info[chip_name][subtract_box][(min_x,min_y,max_x,max_y)]
         # chip_info[chip_name][layer_number][all_subtract_elements]
         # chip_info[chip_name][layer_number][all_no_subtract_elements]
         self.chip_info.clear()
         self.chip_info.update(self._get_chip_names())
 
+        # if imported, hold the path to file name, otherwise None.
+        self.imported_junction_gds = None
+
         if self._create_qgeometry_for_gds(highlight_qcomponents) == 0:
             # Create self.lib and populate path and poly.
             self._populate_poly_path_for_export()
 
             # Add no-cheese MultiPolygon to
             # self.chip_info[chip_name][chip_layer]['no_cheese'],
             # if self.options requests the layer.
@@ -2189,22 +2221,22 @@
                 a_poly = gdspy.boolean(exterior_poly,
                                        a_poly_set,
                                        'not',
                                        max_points=max_points,
                                        layer=layer,
                                        datatype=data_type,
                                        precision=precision)
-                # Poly facturing leading to a funny shape. Leave this out of gds output for now.
+                # Poly fracturing leading to a funny shape. Leave this out of gds output for now.
                 # a_poly.fillet(no_cheese_buffer,
                 #               points_per_2pi=128,
                 #               max_points=max_points,
                 #               precision=precision)
                 all_gds.append(a_poly)
             else:
-                # Poly facturing leading to a funny shape. Leave this out of gds output for now.
+                # Poly fracturing leading to a funny shape. Leave this out of gds output for now.
                 # exterior_poly.fillet(no_cheese_buffer,
                 #                      points_per_2pi=128,
                 #                      max_points=max_points,
                 #                      precision=precision)
                 all_gds.append(exterior_poly)
         return all_gds
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_gds/make_cheese.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_gds/make_cheese.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/extensions/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/extensions/animated_text.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/extensions/animated_text.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/mpl_canvas.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/mpl_interaction.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/mpl_interaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,16 +204,16 @@
         else:
             min_, max_ = end, begin
 
         if scale == 'linear':
             old_min, old_max = min_, max_
         elif scale == 'log':
             old_min = numpy.log10(min_ if min_ > 0. else numpy.nextafter(0, 1))
-            center = numpy.log10(
-                center if center > 0. else numpy.nextafter(0, 1))
+            center = numpy.log10(center if center >
+                                 0. else numpy.nextafter(0, 1))
             old_max = numpy.log10(max_) if max_ > 0. else 0.
         else:
             logging.warning('Zoom on wheel not implemented for scale "%s"' %
                             scale)
             return begin, end
 
         offset = (center - old_min) / (old_max - old_min)
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/mpl_renderer.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/mpl_renderer.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/mpl_toolbox.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/mpl_toolbox.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/renderer_mpl/patch.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/renderer_mpl/patch.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/renderers/setup_default.py` & `qiskit_metal-0.1.5/qiskit_metal/renderers/setup_default.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/assertions.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/assertions.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/custom_decorators.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/custom_decorators.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/run_all_tests.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/run_all_tests.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/test_analyses_1_inst_options.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/test_analyses_1_inst_options.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/test_analyses_2_functionality.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/test_analyses_2_functionality.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/test_default_options.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/test_default_options.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/test_designs.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/test_designs.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,23 +499,25 @@
         """Tests the get_list_of_tables_in_metadata function in design_base.py
         by exeucting get_table_values_form_renderers in a component."""
         design = DesignPlanar()
         q1 = TransmonPocket(design, 'Q1')
 
         result = q1._get_table_values_from_renderers(design)
 
-        self.assertEqual(len(result), 11)
+        self.assertEqual(len(result), 17)
         self.assertEqual(result['hfss_inductance'], '10nH')
         self.assertEqual(result['hfss_capacitance'], 0)
         self.assertEqual(result['hfss_resistance'], 0)
         self.assertAlmostEqual(result['hfss_mesh_kw_jj'], 7e-06, places=6)
         self.assertEqual(result['q3d_inductance'], '10nH')
         self.assertEqual(result['q3d_capacitance'], 0)
         self.assertEqual(result['q3d_resistance'], 0)
         self.assertAlmostEqual(result['q3d_mesh_kw_jj'], 7e-06, places=6)
         self.assertEqual(result['gds_cell_name'], 'my_other_junction')
         self.assertEqual(result['hfss_wire_bonds'], False)
         self.assertEqual(result['q3d_wire_bonds'], False)
+        self.assertEqual(result['aedt_hfss_inductance'], 10e-9)
+        self.assertEqual(result['aedt_hfss_capacitance'], 0)
 
 
 if __name__ == '__main__':
     unittest.main(verbosity=2)
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/test_draw.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/test_draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,45 +316,45 @@
                      (0.6618033988749895, -0.1), (-0.16180339887498948, -0.1)],
                     [(-0.16180339887498948, -0.1), (0.25, 0.7236067977499789),
                      (0.6618033988749895, -0.1), (-0.16180339887498948, -0.1)],
                     [(-0.08944271909999159, 0.044721359549995794),
                      (0.16055728090000843, 0.5447213595499958),
                      (0.3394427190999916, 0.5447213595499958),
                      (0.5894427190999916, 0.044721359549995794), (0.5, -0.1),
-                     (0.0, -0.1), (-0.08944271909999159, 0.044721359549995794)],
-                    [(-0.06980083939497377, 0.05587673960663148),
-                     (0.16341640786499884, 0.5300000000000004),
-                     (0.3365835921350014, 0.5299999999999997),
-                     (0.5698008393949741, 0.05587673960663103),
-                     (0.4812382091061482, -0.08742060633377921),
-                     (0.018761790893851275, -0.08742060633377935),
-                     (-0.06980083939497377, 0.05587673960663148)]]
+                     (0.0, -0.1), (-0.08944271909999159, 0.044721359549995794)]]
+        #[(-0.06980083939497377, 0.05587673960663148),
+        # (0.16341640786499884, 0.5300000000000004),
+        # (0.3365835921350014, 0.5299999999999997),
+        # (0.5698008393949741, 0.05587673960663103),
+        # (0.4812382091061482, -0.08742060633377921),
+        # (0.018761790893851275, -0.08742060633377935),
+        # (-0.06980083939497377, 0.05587673960663148)]]
 
         poly_1 = basic.buffer(poly, 0.1)
         poly_2 = basic.buffer(poly, 0.1, resolution=2)
         poly_3 = basic.buffer(poly,
                               0.1,
                               resolution=2,
                               cap_style=CAP_STYLE.round)
         poly_4 = basic.buffer(poly,
                               0.1,
                               resolution=2,
                               cap_style=CAP_STYLE.round,
                               join_style=JOIN_STYLE.bevel)
-        poly_5 = basic.buffer(poly, 0.1, resolution=2, mitre_limit=0.3)
+        #poly_5 = basic.buffer(poly, 0.1, resolution=2, mitre_limit=0.3)
 
         actual = [
             list(poly_1.exterior.coords),
             list(poly_2.exterior.coords),
             list(poly_3.exterior.coords),
             list(poly_4.exterior.coords),
-            list(poly_5.exterior.coords)
+            #list(poly_5.exterior.coords)
         ]
-
-        for x in range(5):
+        #range(5) if poly_5 is included
+        for x in range(4):
             self.assertEqual(len(actual[x]), len(expected[x]))
             for i in range(len(actual[x])):
                 for j in range(2):
                     self.assertAlmostEqualRel(actual[x][i][j],
                                               expected[x][i][j],
                                               rel_tol=1e-3)
 
@@ -865,15 +865,14 @@
             vec3d.two_points_described([[1, 0, 2], [1, 0, 4]], [0, 1, 0, 0]))
         actual.append(
             vec3d.two_points_described([[0, 1, 2], [0, 1, 4]], [1, 0, 0, 0]))
 
         for i in range(2):
             for j in range(3):
                 for k in range(3):
-                    print(i, j, k)
                     self.assertAlmostEqualRel(actual[i][j][k],
                                               expected[i][j][k],
                                               rel_tol=1e-3)
 
 
 if __name__ == '__main__':
     unittest.main(verbosity=2)
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/test_gui_basic.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/test_gui_basic.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/test_qgeometries.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/test_qgeometries.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/test_qlibrary_1_instantiate.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/test_qlibrary_1_instantiate.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/test_qlibrary_2_options.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/test_qlibrary_2_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
         transmon_concentric.py were not accidentally changed."""
         # Setup expected test results
         design = designs.DesignPlanar()
         my_transmon_concentric = transmon_concentric.TransmonConcentric(
             design, 'my_name')
         options = my_transmon_concentric.default_options
 
-        self.assertEqual(len(options), 16)
+        self.assertEqual(len(options), 17)
         self.assertEqual(options['width'], '1000um')
         self.assertEqual(options['height'], '1000um')
         self.assertEqual(options['rad_o'], '170um')
         self.assertEqual(options['rad_i'], '115um')
         self.assertEqual(options['gap'], '35um')
         self.assertEqual(options['jj_w'], '10um')
         self.assertEqual(options['res_s'], '100um')
@@ -483,26 +483,30 @@
 
         # Test all elements of the result data against expected data
         self.assertEqual(len(_options), 5)
         self.assertEqual(_options['cross_width'], '20um')
         self.assertEqual(_options['cross_length'], '200um')
         self.assertEqual(_options['cross_gap'], '20um')
 
-        self.assertEqual(len(_options['_default_connection_pads']), 6)
+        self.assertEqual(len(_options['_default_connection_pads']), 8)
         self.assertEqual(_options['_default_connection_pads']['connector_type'],
                          '0')
         self.assertEqual(_options['_default_connection_pads']['claw_length'],
                          '30um')
         self.assertEqual(_options['_default_connection_pads']['ground_spacing'],
                          '5um')
         self.assertEqual(_options['_default_connection_pads']['claw_width'],
                          '10um')
         self.assertEqual(_options['_default_connection_pads']['claw_gap'],
                          '6um')
         self.assertEqual(
+            _options['_default_connection_pads']['claw_cpw_length'], '40um')
+        self.assertEqual(_options['_default_connection_pads']['claw_cpw_width'],
+                         '10um')
+        self.assertEqual(
             _options['_default_connection_pads']['connector_location'], '0')
 
     def test_qlibrary_transmon_pocket_options(self):
         """Test that default options of transmon_pocket in transmon_pocket.py
         were not accidentally changed."""
         # Setup expected test results
         _design = designs.DesignPlanar()
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/test_qlibrary_3_functionality.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/test_qlibrary_3_functionality.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/test_speed.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/tests/test_toolbox_python.py` & `qiskit_metal-0.1.5/qiskit_metal/tests/test_toolbox_python.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/toolbox_metal/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,22 +40,30 @@
 .. autosummary::
     :toctree: ../stubs/
 
     about
     import_export
     math_and_overrides
     parsing
+    layer_stack_handler
+    bounds_for_path_and_poly_tables
+    determine_larger_box
 
 """
 
 from .parsing import parse_value
 from .parsing import is_variable_name
 from .parsing import is_numeric_possible
+from .parsing import parse_units
+from .layer_stack_handler import LayerStackHandler
+from .bounds_for_path_and_poly_tables import BoundsForPathAndPolyTables, determine_larger_box
 
 from .. import config
 if config.is_building_docs():
     from . import about
     from .exceptions import QiskitMetalDesignError
     from .exceptions import QiskitMetalExceptions
     from . import import_export
     from . import parsing
     from . import math_and_overrides
+    from . import layer_stack_handler
+    from . import bounds_for_path_and_poly_tables
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/toolbox_metal/about.py` & `qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/about.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,44 +111,43 @@
 def open_docs(page='https://qiskit.org/documentation/metal/'):
     """Open the qiskit_metal documentation in HTML.
 
     Open the URL in new window, raising the window if possible.
     """
     webbrowser.open(page, new=1)
 
+    ######################################################################################
+    # More detailed information to orient a user.
+    # For debug purposes.
+    # Main function: ``orient_me```
 
-######################################################################################
-# More detailed information to orient a user.
-# For debug purposes.
-# Main function: ``orient_me```
-
-
-def orient_me(do_print: bool = True) -> Union[None, str]:
+    #def orient_me(do_print: bool = True) -> Union[None, str]:
     """Full system, python, user, and environemnt information.
 
     Args:
         do_print(bool): Return the string if True, else format and print.
     """
 
-    text = get_platform_info()
-    text += \
-        f" User and directories:\n\n"\
-        f"    User              : {getpass.getuser()}\n"\
-        f"    User home dirctry : {Path.home()}\n"\
-        f"    Current directory : {Path.cwd()}\n\n"\
-        f"    Conda default env : {os.environ.get('CONDA_DEFAULT_ENV', 'N/A')}\n"\
-        f"    Conda current env : {os.environ.get('CONDA_PREFIX', 'N/A')}\n"\
-        f"    Python executable : {sys.executable}\n"\
-
-    if do_print:
-        text = style_colon_list(text, Color.BOLD, Color.END)
-        print(text)
-        return None
 
-    return text
+#    text = get_platform_info()
+#    text += \
+#        f" User and directories:\n\n"\
+#        f"    User              : {getpass.getuser()}\n"\
+#        f"    User home dirctry : {Path.home()}\n"\
+#        f"    Current directory : {Path.cwd()}\n\n"\
+#        f"    Conda default env : {os.environ.get('CONDA_DEFAULT_ENV', 'N/A')}\n"\
+#        f"    Conda current env : {os.environ.get('CONDA_PREFIX', 'N/A')}\n"\
+#       f"    Python executable : {sys.executable}\n"\
+
+#    if do_print:
+#        text = style_colon_list(text, Color.BOLD, Color.END)
+#        print(text)
+#        return None
+
+#    return text
 
 
 def get_platform_info() -> str:
     """Returns a string with the platform information."""
 
     return '''
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/toolbox_metal/exceptions.py` & `qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/toolbox_metal/import_export.py` & `qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/import_export.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/toolbox_metal/math_and_overrides.py` & `qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/math_and_overrides.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/toolbox_metal/parsing.py` & `qiskit_metal-0.1.5/qiskit_metal/toolbox_metal/parsing.py`

 * *Files 10% similar despite different names*

```diff
@@ -173,14 +173,15 @@
 from collections.abc import Mapping
 from numbers import Number
 from typing import Union
 
 import ast
 import numpy as np
 import pint
+from pint import UnitRegistry
 
 from .. import Dict, config, logger
 
 __all__ = [
     'parse_value',  # Main function
     'is_variable_name',  # extra helpers
     'is_numeric_possible',
@@ -193,14 +194,18 @@
 # Constants
 
 # Values that can represent True bool
 TRUE_STR = [
     'true', 'True', 'TRUE', True, '1', 't', 'y', 'Y', 'YES', 'yes', 'yeah', 1,
     1.0
 ]
+FALSE_STR = [
+    'false', 'False', 'FALSE', False, '0', 'f', 'n', 'N', 'NO', 'no', 'na', 0,
+    0.0
+]
 
 
 def is_true(value: Union[str, int, bool, float]) -> bool:
     """Check if a value is true or not.
 
     Args:
         value (str): Value to check
@@ -438,7 +443,94 @@
                 f'Missing key {name} from params {params}. Skipping ...\n')
             continue
 
         # option_dict[name] should be a string
         res += [parse_value(params[name], variable_dict)]
 
     return res
+
+
+##############################################################################
+# From pyepr, being used by renderer using comm port.
+#
+"""The methods in this section were copied from Ansys renderer which used comm-ports."""
+
+# UNITS
+# LENGTH_UNIT         --- HFSS UNITS
+# #Assumed default input units for ansys hfss
+LENGTH_UNIT = 'meter'
+# LENGTH_UNIT_ASSUMED --- USER UNITS
+# if a user inputs a blank number with no units in `parse_fix`,
+# we can assume the following using
+LENGTH_UNIT_ASSUMED = 'mm'
+
+try:
+    u_reg = UnitRegistry()
+    Q = u_reg.Quantity
+except (ImportError, ModuleNotFoundError):
+    pass  # raise NameError ("Pint module not installed. Please install.")
+
+
+def extract_value_unit(expr, units):
+    """
+    :type expr: str
+    :type units: str
+    :return: float
+    """
+    # pylint: disable=broad-except
+    try:
+        return Q(expr).to(units).magnitude
+    except Exception:
+        try:
+            return float(expr)
+        except Exception:
+            return expr
+
+
+def fix_units(x, unit_assumed=None):
+    '''
+    Convert all numbers to string and append the assumed units if needed.
+    For an iterable, returns a list
+    '''
+    unit_assumed = LENGTH_UNIT_ASSUMED if unit_assumed is None else unit_assumed
+    if isinstance(x, str):
+        # Check if there are already units defined, assume of form 2.46mm  or 2.0 or 4.
+        if x[-1].isdigit() or x[-1] == '.':  # number
+            return x + unit_assumed
+        else:  # units are already applied
+            return x
+
+    elif isinstance(x, Number):
+        return fix_units(str(x) + unit_assumed, unit_assumed=unit_assumed)
+
+    elif isinstance(x, Iterable):  # hasattr(x, '__iter__'):
+        return [fix_units(y, unit_assumed=unit_assumed) for y in x]
+    else:
+        return x
+
+
+def parse_entry(entry, convert_to_unit=LENGTH_UNIT):
+    '''
+    Should take a list of tuple of list... of int, float or str...
+    For iterables, returns lists
+    '''
+    if not isinstance(entry, list) and not isinstance(entry, tuple):
+        return extract_value_unit(entry, convert_to_unit)
+    else:
+        entries = entry
+        _entry = []
+        for entry in entries:
+            _entry.append(parse_entry(entry, convert_to_unit=convert_to_unit))
+        return _entry
+
+
+def parse_units(x):
+    '''
+    Convert number, string, and lists/arrays/tuples to numbers scaled
+    in HFSS units.
+
+    Converts to                  LENGTH_UNIT = meters  [HFSS UNITS]
+    Assumes input units  LENGTH_UNIT_ASSUMED = mm      [USER UNITS]
+
+    [USER UNITS] ----> [HFSS UNITS]
+    '''
+    return parse_entry(fix_units(x))
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal/toolbox_python/__init__.py` & `qiskit_metal-0.1.5/qiskit_metal/toolbox_python/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/toolbox_python/_logging.py` & `qiskit_metal-0.1.5/qiskit_metal/toolbox_python/_logging.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/toolbox_python/attr_dict.py` & `qiskit_metal-0.1.5/qiskit_metal/toolbox_python/attr_dict.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/toolbox_python/display.py` & `qiskit_metal-0.1.5/qiskit_metal/toolbox_python/display.py`

 * *Files identical despite different names*

### Comparing `qiskit_metal-0.1.2/qiskit_metal/toolbox_python/utility_functions.py` & `qiskit_metal-0.1.5/qiskit_metal/toolbox_python/utility_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import logging
 import os
 import re
 import sys
 import traceback
 import warnings
 from copy import deepcopy
-from typing import Dict, List, TYPE_CHECKING, Tuple, Callable
+from typing import Dict, List, TYPE_CHECKING, Tuple, Callable, Union
 import inspect
 
 import pandas as pd
 
 from qiskit_metal.draw import Vector
 from qiskit_metal.toolbox_metal.exceptions import InputError
 
@@ -388,21 +388,48 @@
         badlist = [1]
     else:
         badlist = []
     for i in range(2, length - 2):
         if min(get_dist(coords[i - 1], coords[i], precision),
                get_dist(coords[i], coords[i + 1], precision)) < 2 * fradius:
             badlist.append(i)
-    if (get_dist(coords[length - 3], coords[length - 2], precision) <
-            2 * fradius) or (get_dist(coords[length - 2], coords[length - 1],
-                                      precision) < fradius):
+    if (get_dist(coords[length - 3], coords[length - 2], precision)
+            < 2 * fradius) or (get_dist(coords[length - 2], coords[length - 1],
+                                        precision) < fradius):
         badlist.append(length - 2)
     return badlist
 
 
+def good_fillet_idxs(coords: list,
+                     fradius: float,
+                     precision: int = 9,
+                     isclosed: bool = False):
+    """
+    Get list of vertex indices in a linestring (isclosed = False) or polygon (isclosed = True)
+    that can be filleted based on proximity to neighbors.
+
+    Args:
+        coords (list): Ordered list of tuples of vertex coordinates.
+        fradius (float): User-specified fillet radius from QGeometry table.
+        precision (int, optional): Digits of precision used for round(). Defaults to 9.
+        isclosed (bool, optional): Boolean denoting whether the shape is a linestring or
+            polygon. Defaults to False.
+
+    Returns:
+        list: List of indices of vertices that can be filleted.
+    """
+    if isclosed:
+        return toggle_numbers(
+            bad_fillet_idxs(coords, fradius, precision, isclosed=True),
+            len(coords))
+    return toggle_numbers(
+        bad_fillet_idxs(coords, fradius, precision, isclosed=False),
+        len(coords))[1:-1]
+
+
 def get_range_of_vertex_to_not_fillet(coords: list,
                                       fradius: float,
                                       precision: int = 9,
                                       add_endpoints: bool = True) -> list:
     """Provide a list of tuples for a list of integers that correspond to
     coords. Each tuple corresponds to a range of indexes within coords.  A
     range denotes vertexes that are too short to be fillet'd.
@@ -582,7 +609,29 @@
     """
     args = []
     for param in inspect.signature(func).parameters.values():
         if param.name == 'self':
             continue
         args.append(param.name)
     return args
+
+
+#####################################################################################
+# Used for each row in qgeometry table to clean the name entered by user.
+
+
+def get_clean_name(name: str) -> str:
+    """Create a valid variable name from the given one by removing having it
+    begin with a letter or underscore followed by an unlimited string of
+    letters, numbers, and underscores.
+
+    Args:
+        name (str): Initial, possibly unusable, string to be modified.
+
+    Returns:
+        str: Variable name consistent with Python naming conventions.
+    """
+    # Remove invalid characters
+    name = re.sub("[^0-9a-zA-Z_]", "", name)
+    # Remove leading characters until we find a letter or underscore
+    name = re.sub("^[^a-zA-Z_]+", "", name)
+    return name
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal.egg-info/PKG-INFO` & `qiskit_metal-0.1.5/qiskit_metal.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,147 +1,146 @@
 Metadata-Version: 2.1
 Name: qiskit-metal
-Version: 0.1.2
+Version: 0.1.5
 Summary: Qiskit Metal | for quantum device design & analysis
 Home-page: https://github.com/Qiskit/qiskit-metal
 Author: Qiskit Metal Development Team
 Author-email: qiskit@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-metal/issues
 Project-URL: Documentation, https://qiskit.org/documentation/metal
 Project-URL: Source Code, https://github.com/Qiskit/qiskit-metal
-Description: # Qiskit Metal 
-        [![License](https://img.shields.io/github/license/Qiskit/qiskit-metal.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)<!--- long-description-skip-begin -->[![Release](https://img.shields.io/github/release/Qiskit/qiskit-metal.svg?style=popout-square)](https://github.com/Qiskit/qiskit-metal/releases)<!--- long-description-skip-begin -->[![join slack](https://img.shields.io/badge/slack-@qiskit-yellow.svg?logo=slack&style=popout-square)](https://ibm.co/joinqiskitslack)[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4618153.svg)](https://doi.org/10.5281/zenodo.4618153)
-         
-        >![Welcome to Qiskit Metal!](https://raw.githubusercontent.com/Qiskit/qiskit-metal/main/docs/images/zkm_banner.png 'Welcome to Qiskit Metal')
-        > Qiskit Metal is an open-source framework for engineers and scientists to design superconducting quantum devices with ease.
-        
-        ## Installation
-        If you are interested in customizing your experience, or if you are unable to install qiskit-metal using the `pip install` instructions below, consider installing directly the source code, following the instructions in the [documentation](https://qiskit.org/documentation/metal/installation.html) and/or the [installation instructions for developers](https://github.com/Qiskit/qiskit-metal/blob/main/README_developers.md).
-        
-        For normal use, please continue reading.
-        
-        ### The Qiskit Metal deployed package
-        You can install Qiskit Metal via the pip tool (a python package manager).
-        ```bash
-        pip install qiskit-metal
-        ```
-        PIP will handle most of the dependencies automatically and you will always install the latest (and well-tested) version of the package.
-        
-        Some of the dependencies, namely pyside2 and geopandas, might require manual installation, depending on your specific system compatibility. If you encounter installation or execution errors, please refer first to the [FAQ](https://qiskit.org/documentation/metal/faq.html).
-        
-        We recommend to install qiskit-metal in a conda environment or venv, to prevent version conflicts with pre-existing package versions.
-        
-        ### Jupyter Notebook
-        At this time, we recommend using Jupyter notebook/lab to be able to access all the Qiskit Metal features. Jupyter is not installed with the default dependencies, to accommodate those users intending to utilize a centralized or customized installation.
-        
-        If you require a fresh installation, please refer to either [anaconda.org](https://anaconda.org/) or [jupyter.org](https://jupyter.org/install).
-        
-        Unless you installed the entire `jupyter` package in your current environment, do not forget to create the appropriate kernel to make the environment (thus qiskit-metal) available to jupyter (instructions in the [FAQ](https://qiskit.org/documentation/metal/faq.html))
-        
-        ## Creating Your First Quantum Component in Qiskit Metal:
-        Now that Qiskit Metal is installed, it's time to begin working with it.
-        We are ready to try out a quantum chip example, which is simulated locally using
-        the Qiskit MetalGUI element. This is a simple example that makes a qubit.
-        ```
-        $ python
-        ```
-        ```python
-        >>> from qiskit_metal import designs, draw, MetalGUI, Dict, open_docs
-        >>> design = designs.DesignPlanar()
-        >>> design.overwrite_enabled = True
-        >>> design.chips.main
-        >>> design.chips.main.size.size_x = '11mm'
-        >>> design.chips.main.size.size_y = '9mm'
-        >>> gui = MetalGUI(design)
-        ```
-        #### Launch the Qiskit Metal GUI to interactively view, edit, and simulate a QDesign:
-        ```python
-        >>> gui = MetalGUI(design)
-        ```
-        #### Let's create a new qubit (a transmon) by creating an object of this class.
-        ```python
-        >>> from qiskit_metal.qlibrary.qubits.transmon_pocket import TransmonPocket
-        >>> q1 = TransmonPocket(design, 'Q1', options=dict(connection_pads=dict(a=dict())))
-        >>> gui.rebuild()
-        >>> gui.edit_component('Q1')
-        >>> gui.autoscale()
-        ```
-        #### Change options.
-        ```python
-        >>> q1.options.pos_x = '0.5 mm'
-        >>> q1.options.pos_y = '0.25 mm'
-        >>> q1.options.pad_height = '90um'
-        >>> q1.options.pad_width  = '455um'
-        >>> q1.options.pad_gap    = '30 um'
-        ```
-        #### Update the component geometry after changing the options.
-        ```python
-        >>> gui.rebuild()
-        ```
-        ![Example_Image!](https://raw.githubusercontent.com/Qiskit/qiskit-metal/main/docs/images/1_1_Birds_eye_view_of_Qiskit_Metal_example_image.jpg 'Example_Image') 
-        #### Get a list of all the qcomponents in QDesign and then zoom on them.
-        ```python
-        >>> all_component_names = design.components.keys()
-        >>> gui.zoom_on_components(all_component_names)
-        ```
-        #### Closing the Qiskit Metal GUI.
-        ```python
-        >>> gui.main_window.close()
-        ```
-        
-        A script is available [here](https://qiskit.org/documentation/metal/tut/overview/1.1%20High%20Level%20Demo%20of%20Qiskit%20Metal.html), where we also show the overview of Qiskit Metal.
-        
-        ## Community and Support
-        
-        #### Watch the recorded tutorials 
-        [![Video Tutorials](https://img.shields.io/badge/youtube-Video_Tutorials-red.svg?logo=youtube)](https://youtube.com/playlist?list=PLOFEBzvs-VvqHl5ZqVmhB_FcSqmLufsjb)
-        
-        The streaming will also be recorded and made available [here](https://www.youtube.com/playlist?list=PLOFEBzvs-VvqHl5ZqVmhB_FcSqmLufsjb) for offline review.
-        
-        #### Take part in the live tutorials and discussion
-        Through June 2021 we are offering live tutorials and Q&A. [Sign up](https://airtable.com/shrxQEgKqZCf319F3) to receive an invite to the upcoming sessions.  The streaming will also be recorded and made available for offline review.  Find [here](https://github.com/Qiskit/qiskit-metal/blob/main/README_Tutorials.md) more details on schedule and use the Slack channel to give us feedback and to request the most relevant content to you.
-        
-        #### Get help: Slack 
-        [![join slack](https://img.shields.io/badge/slack-blue.svg?logo=slack)](https://ibm.co/joinqiskitslack)
-        
-        Use the slack channel.  Join [qiskit slack](https://ibm.co/joinqiskitslack) and then join the `#metal` channel to communicate with the developers and other participants.  You may also use this channel to inquire about collaborations.
-        
-        ## Contribution Guidelines
-        If you'd like to contribute to Qiskit Metal, please take a look at our
-        [contribution guidelines](https://github.com/Qiskit/qiskit-metal/blob/main/CONTRIBUTING.md). This project adheres to Qiskit's [code of conduct](https://github.com/Qiskit/qiskit-metal/blob/main/CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.
-        We use [GitHub issues](https://github.com/Qiskit/qiskit-metal/issues) for tracking requests and bugs. Please
-        [join the Qiskit Slack community](https://ibm.co/joinqiskitslack)
-        and use our [Qiskit Slack channel](https://qiskit.slack.com) for discussion and simple questions.
-        For questions that are more suited for a forum we use the Qiskit tag in the [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
-        ## Next Steps
-        Now you're set up and ready to check out some of the other examples from our
-        [Qiskit Metal Tutorials](https://github.com/Qiskit/qiskit-metal/blob/main/tutorials/) repository or [Qiskit Metal Documentation](https://qiskit.org/documentation/metal/tut/).
-        ## Authors and Citation
-        Qiskit Metal is the work of [many people](https://github.com/Qiskit/qiskit-metal/pulse/monthly) who contribute to the project at different levels. Metal was conceived and developed by [Zlatko Minev](https://www.zlatko-minev.com) at IBM; then co-led with Thomas McConkey. If you use Qiskit Metal, please cite as per the included [BibTeX file](https://github.com/Qiskit/qiskit-metal/blob/main/Qiskit_Metal.bib). For icon attributions, see [here](https://github.com/Qiskit/qiskit-metal/blob/main/qiskit_metal/_gui/_imgs/icon_attributions.txt).
-        ## Changelog and Release Notes
-        The changelog provides a quick overview of notable changes for a given release.
-        
-        The changelog for a particular release can be found in the correspondent Github release page. For example, you can find the changelog for the `0.0.4` release [here](https://github.com/Qiskit/qiskit-metal/releases/tag/0.0.4)
-        
-        The changelog for all releases can be found in the release page: [![Releases](https://img.shields.io/github/release/Qiskit/qiskit-metal.svg?style=popout-square)](https://github.com/Qiskit/qiskit-metal/releases)
-        
-        Additionally, as part of each release detailed release notes are written to document in detail what has changed as part of a release. This includes any documentation on potential breaking changes on upgrade and new features.
-        
-        ## License
-        [Apache License 2.0](https://github.com/Qiskit/qiskit-metal/blob/main/LICENSE.txt)
-        
 Keywords: qiskit sdk quantum eda
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Qiskit Metal 
+[![License](https://img.shields.io/github/license/Qiskit/qiskit-metal.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)<!--- long-description-skip-begin -->[![Release](https://img.shields.io/github/release/Qiskit/qiskit-metal.svg?style=popout-square)](https://github.com/Qiskit/qiskit-metal/releases)<!--- long-description-skip-begin -->[![join slack](https://img.shields.io/badge/slack-@qiskit-yellow.svg?logo=slack&style=popout-square)](https://qisk.it/join-slack)[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4618153.svg)](https://doi.org/10.5281/zenodo.4618153)
+ 
+>![Welcome to Qiskit Metal!](https://raw.githubusercontent.com/Qiskit/qiskit-metal/main/docs/images/zkm_banner.png 'Welcome to Qiskit Metal')
+> Qiskit Metal is an open-source framework for engineers and scientists to design superconducting quantum devices with ease.
+
+## Installation
+If you are interested in customizing your experience, or if you are unable to install qiskit-metal using the `pip install` instructions below, consider installing directly the source code, following the instructions in the [documentation](https://qiskit.org/documentation/metal/installation.html) and/or the [installation instructions for developers](https://github.com/Qiskit/qiskit-metal/blob/main/README_developers.md).
+
+For normal use, please continue reading.
+
+### The Qiskit Metal deployed package
+You can install Qiskit Metal via the pip tool (a python package manager).
+```bash
+pip install qiskit-metal
+```
+PIP will handle most of the dependencies automatically and you will always install the latest (and well-tested) version of the package.
+
+Some of the dependencies, namely pyside2 and geopandas, might require manual installation, depending on your specific system compatibility. If you encounter installation or execution errors, please refer first to the [FAQ](https://qiskit.org/documentation/metal/faq.html).
+
+We recommend to install qiskit-metal in a conda environment or venv, to prevent version conflicts with pre-existing package versions.
+
+### Jupyter Notebook
+At this time, we recommend using Jupyter notebook/lab to be able to access all the Qiskit Metal features. Jupyter is not installed with the default dependencies, to accommodate those users intending to utilize a centralized or customized installation.
+
+If you require a fresh installation, please refer to either [anaconda.org](https://anaconda.org/) or [jupyter.org](https://jupyter.org/install).
+
+Unless you installed the entire `jupyter` package in your current environment, do not forget to create the appropriate kernel to make the environment (thus qiskit-metal) available to jupyter (instructions in the [FAQ](https://qiskit.org/documentation/metal/faq.html))
+
+## Creating Your First Quantum Component in Qiskit Metal:
+Now that Qiskit Metal is installed, it's time to begin working with it.
+We are ready to try out a quantum chip example, which is simulated locally using
+the Qiskit MetalGUI element. This is a simple example that makes a qubit.
+```
+$ python
+```
+```python
+>>> from qiskit_metal import designs, draw, MetalGUI, Dict, open_docs
+>>> design = designs.DesignPlanar()
+>>> design.overwrite_enabled = True
+>>> design.chips.main
+>>> design.chips.main.size.size_x = '11mm'
+>>> design.chips.main.size.size_y = '9mm'
+>>> gui = MetalGUI(design)
+```
+#### Launch the Qiskit Metal GUI to interactively view, edit, and simulate a QDesign:
+```python
+>>> gui = MetalGUI(design)
+```
+#### Let's create a new qubit (a transmon) by creating an object of this class.
+```python
+>>> from qiskit_metal.qlibrary.qubits.transmon_pocket import TransmonPocket
+>>> q1 = TransmonPocket(design, 'Q1', options=dict(connection_pads=dict(a=dict())))
+>>> gui.rebuild()
+>>> gui.edit_component('Q1')
+>>> gui.autoscale()
+```
+#### Change options.
+```python
+>>> q1.options.pos_x = '0.5 mm'
+>>> q1.options.pos_y = '0.25 mm'
+>>> q1.options.pad_height = '90um'
+>>> q1.options.pad_width  = '455um'
+>>> q1.options.pad_gap    = '30 um'
+```
+#### Update the component geometry after changing the options.
+```python
+>>> gui.rebuild()
+```
+![Example_Image!](https://raw.githubusercontent.com/Qiskit/qiskit-metal/main/docs/images/1_1_Birds_eye_view_of_Qiskit_Metal_example_image.jpg 'Example_Image') 
+#### Get a list of all the qcomponents in QDesign and then zoom on them.
+```python
+>>> all_component_names = design.components.keys()
+>>> gui.zoom_on_components(all_component_names)
+```
+#### Closing the Qiskit Metal GUI.
+```python
+>>> gui.main_window.close()
+```
+
+A script is available [here](https://qiskit.org/documentation/metal/tut/overview/1.1%20High%20Level%20Demo%20of%20Qiskit%20Metal.html), where we also show the overview of Qiskit Metal.
+
+## Community and Support
+
+#### Watch the recorded tutorials 
+[![Video Tutorials](https://img.shields.io/badge/youtube-Video_Tutorials-red.svg?logo=youtube)](https://youtube.com/playlist?list=PLOFEBzvs-VvqHl5ZqVmhB_FcSqmLufsjb)
+
+The streaming will also be recorded and made available [here](https://www.youtube.com/playlist?list=PLOFEBzvs-VvqHl5ZqVmhB_FcSqmLufsjb) for offline review.
+
+#### Take part in the live tutorials and discussion
+Through June 2021 we are offering live tutorials and Q&A. [Sign up](https://airtable.com/shrxQEgKqZCf319F3) to receive an invite to the upcoming sessions.  The streaming will also be recorded and made available for offline review.  Find [here](https://github.com/Qiskit/qiskit-metal/blob/main/README_Tutorials.md) more details on schedule and use the Slack channel to give us feedback and to request the most relevant content to you.
+
+#### Get help: Slack 
+[![join slack](https://img.shields.io/badge/slack-blue.svg?logo=slack)](https://qisk.it/join-slack)
+
+Use the slack channel.  Join [qiskit slack](https://qisk.it/join-slack) and then join the `#metal` channel to communicate with the developers and other participants.  You may also use this channel to inquire about collaborations.
+
+## Contribution Guidelines
+If you'd like to contribute to Qiskit Metal, please take a look at our
+[contribution guidelines](https://github.com/Qiskit/qiskit-metal/blob/main/CONTRIBUTING.md). This project adheres to Qiskit's [code of conduct](https://github.com/Qiskit/qiskit-metal/blob/main/CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.
+We use [GitHub issues](https://github.com/Qiskit/qiskit-metal/issues) for tracking requests and bugs. Please
+[join the Qiskit Slack community](https://qisk.it/join-slack)
+and use our [Qiskit Slack channel](https://qiskit.slack.com) for discussion and simple questions.
+For questions that are more suited for a forum we use the Qiskit tag in the [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
+## Next Steps
+Now you're set up and ready to check out some of the other examples from our
+[Qiskit Metal Tutorials](https://github.com/Qiskit/qiskit-metal/blob/main/tutorials/) repository or [Qiskit Metal Documentation](https://qiskit.org/documentation/metal/tut/).
+## Authors and Citation
+Qiskit Metal is the work of [many people](https://github.com/Qiskit/qiskit-metal/pulse/monthly) who contribute to the project at different levels. Metal was conceived and developed by [Zlatko Minev](https://www.zlatko-minev.com) at IBM; then co-led with Thomas McConkey. If you use Qiskit Metal, please cite as per the included [BibTeX file](https://github.com/Qiskit/qiskit-metal/blob/main/Qiskit_Metal.bib). For icon attributions, see [here](https://github.com/Qiskit/qiskit-metal/blob/main/qiskit_metal/_gui/_imgs/icon_attributions.txt).
+## Changelog and Release Notes
+The changelog provides a quick overview of notable changes for a given release.
+
+The changelog for a particular release can be found in the correspondent Github release page. For example, you can find the changelog for the `0.0.4` release [here](https://github.com/Qiskit/qiskit-metal/releases/tag/0.0.4)
+
+The changelog for all releases can be found in the release page: [![Releases](https://img.shields.io/github/release/Qiskit/qiskit-metal.svg?style=popout-square)](https://github.com/Qiskit/qiskit-metal/releases)
+
+Additionally, as part of each release detailed release notes are written to document in detail what has changed as part of a release. This includes any documentation on potential breaking changes on upgrade and new features.
+
+## License
+[Apache License 2.0](https://github.com/Qiskit/qiskit-metal/blob/main/LICENSE.txt)
```

### Comparing `qiskit_metal-0.1.2/qiskit_metal.egg-info/SOURCES.txt` & `qiskit_metal-0.1.5/qiskit_metal.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+LICENSE.txt
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 qiskit_metal/__init__.py
 qiskit_metal/_defaults.py
 qiskit_metal/_is_design.py
 qiskit_metal/config.py
 qiskit_metal.egg-info/PKG-INFO
 qiskit_metal.egg-info/SOURCES.txt
@@ -141,46 +144,50 @@
 qiskit_metal/analyses/simulation/scattering_impedance.py
 qiskit_metal/analyses/sweep_and_optimize/__init__.py
 qiskit_metal/analyses/sweep_and_optimize/sweeper.py
 qiskit_metal/analyses/sweep_and_optimize/sweeping.py
 qiskit_metal/designs/__init__.py
 qiskit_metal/designs/design_base.py
 qiskit_metal/designs/design_flipchip.py
+qiskit_metal/designs/design_multiplanar.py
 qiskit_metal/designs/design_planar.py
 qiskit_metal/designs/interface_components.py
 qiskit_metal/designs/net_info.py
 qiskit_metal/draw/__init__.py
 qiskit_metal/draw/basic.py
 qiskit_metal/draw/mpl.py
 qiskit_metal/draw/utility.py
 qiskit_metal/qgeometries/__init__.py
 qiskit_metal/qgeometries/qgeometries_handler.py
 qiskit_metal/qlibrary/__init__.py
 qiskit_metal/qlibrary/_template.py
 qiskit_metal/qlibrary/core/__init__.py
 qiskit_metal/qlibrary/core/_parsed_dynamic_attrs.py
 qiskit_metal/qlibrary/core/base.py
+qiskit_metal/qlibrary/core/design_check.py
 qiskit_metal/qlibrary/core/qroute.py
 qiskit_metal/qlibrary/core/qubit.py
 qiskit_metal/qlibrary/couplers/__init__.py
 qiskit_metal/qlibrary/couplers/cap_n_interdigital_tee.py
 qiskit_metal/qlibrary/couplers/coupled_line_tee.py
 qiskit_metal/qlibrary/couplers/line_tee.py
 qiskit_metal/qlibrary/couplers/tunable_coupler_01.py
+qiskit_metal/qlibrary/couplers/tunable_coupler_02.py
 qiskit_metal/qlibrary/lumped/__init__.py
 qiskit_metal/qlibrary/lumped/cap_3_interdigital.py
 qiskit_metal/qlibrary/lumped/cap_n_interdigital.py
 qiskit_metal/qlibrary/lumped/resonator_coil_rect.py
 qiskit_metal/qlibrary/qubits/JJ_Dolan.py
 qiskit_metal/qlibrary/qubits/JJ_Manhattan.py
 qiskit_metal/qlibrary/qubits/SQUID_loop.py
 qiskit_metal/qlibrary/qubits/Transmon_Interdigitated.py
 qiskit_metal/qlibrary/qubits/__init__.py
 qiskit_metal/qlibrary/qubits/star_qubit.py
 qiskit_metal/qlibrary/qubits/transmon_concentric.py
+qiskit_metal/qlibrary/qubits/transmon_concentric_type_2.py
 qiskit_metal/qlibrary/qubits/transmon_cross.py
 qiskit_metal/qlibrary/qubits/transmon_cross_fl.py
 qiskit_metal/qlibrary/qubits/transmon_pocket.py
 qiskit_metal/qlibrary/qubits/transmon_pocket_6.py
 qiskit_metal/qlibrary/qubits/transmon_pocket_cl.py
 qiskit_metal/qlibrary/qubits/transmon_pocket_teeth.py
 qiskit_metal/qlibrary/sample_shapes/__init__.py
@@ -204,27 +211,41 @@
 qiskit_metal/qlibrary/tlines/mixed_path.py
 qiskit_metal/qlibrary/tlines/pathfinder.py
 qiskit_metal/qlibrary/tlines/straight_path.py
 qiskit_metal/qlibrary/user_components/__init__.py
 qiskit_metal/qlibrary/user_components/my_qcomponent.py
 qiskit_metal/renderers/__init__.py
 qiskit_metal/renderers/setup_default.py
+qiskit_metal/renderers/utils.py
 qiskit_metal/renderers/renderer_ansys/__init__.py
 qiskit_metal/renderers/renderer_ansys/ansys_renderer.py
 qiskit_metal/renderers/renderer_ansys/hfss_renderer.py
 qiskit_metal/renderers/renderer_ansys/parse.py
 qiskit_metal/renderers/renderer_ansys/q3d_renderer.py
+qiskit_metal/renderers/renderer_ansys_pyaedt/__init__.py
+qiskit_metal/renderers/renderer_ansys_pyaedt/hfss_renderer_aedt.py
+qiskit_metal/renderers/renderer_ansys_pyaedt/hfss_renderer_drivenmodal_aedt.py
+qiskit_metal/renderers/renderer_ansys_pyaedt/hfss_renderer_eigenmode_aedt.py
+qiskit_metal/renderers/renderer_ansys_pyaedt/pyaedt_base.py
+qiskit_metal/renderers/renderer_ansys_pyaedt/q3d_renderer_aedt.py
 qiskit_metal/renderers/renderer_base/__init__.py
 qiskit_metal/renderers/renderer_base/renderer_base.py
 qiskit_metal/renderers/renderer_base/renderer_gui_base.py
 qiskit_metal/renderers/renderer_base/rndr_analysis.py
 qiskit_metal/renderers/renderer_base/rndr_export.py
+qiskit_metal/renderers/renderer_elmer/__init__.py
+qiskit_metal/renderers/renderer_elmer/elmer_configs.py
+qiskit_metal/renderers/renderer_elmer/elmer_renderer.py
+qiskit_metal/renderers/renderer_elmer/elmer_runner.py
 qiskit_metal/renderers/renderer_gds/__init__.py
 qiskit_metal/renderers/renderer_gds/gds_renderer.py
 qiskit_metal/renderers/renderer_gds/make_cheese.py
+qiskit_metal/renderers/renderer_gmsh/__init__.py
+qiskit_metal/renderers/renderer_gmsh/gmsh_renderer.py
+qiskit_metal/renderers/renderer_gmsh/gmsh_utils.py
 qiskit_metal/renderers/renderer_mpl/__init__.py
 qiskit_metal/renderers/renderer_mpl/mpl_canvas.py
 qiskit_metal/renderers/renderer_mpl/mpl_interaction.py
 qiskit_metal/renderers/renderer_mpl/mpl_renderer.py
 qiskit_metal/renderers/renderer_mpl/mpl_toolbox.py
 qiskit_metal/renderers/renderer_mpl/patch.py
 qiskit_metal/renderers/renderer_mpl/extensions/__init__.py
@@ -245,16 +266,18 @@
 qiskit_metal/tests/test_qlibrary_3_functionality.py
 qiskit_metal/tests/test_renderers.py
 qiskit_metal/tests/test_speed.py
 qiskit_metal/tests/test_toolbox_metal.py
 qiskit_metal/tests/test_toolbox_python.py
 qiskit_metal/toolbox_metal/__init__.py
 qiskit_metal/toolbox_metal/about.py
+qiskit_metal/toolbox_metal/bounds_for_path_and_poly_tables.py
 qiskit_metal/toolbox_metal/exceptions.py
 qiskit_metal/toolbox_metal/import_export.py
+qiskit_metal/toolbox_metal/layer_stack_handler.py
 qiskit_metal/toolbox_metal/math_and_overrides.py
 qiskit_metal/toolbox_metal/parsing.py
 qiskit_metal/toolbox_python/__init__.py
 qiskit_metal/toolbox_python/_logging.py
 qiskit_metal/toolbox_python/attr_dict.py
 qiskit_metal/toolbox_python/display.py
 qiskit_metal/toolbox_python/utility_functions.py
```

### Comparing `qiskit_metal-0.1.2/setup.py` & `qiskit_metal-0.1.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     long_description = f.read()
 
 with open(here / "requirements.txt", encoding="utf-8") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="qiskit_metal",
-    version="0.1.2",
+    version="0.1.5",
     description="Qiskit Metal | for quantum device design & analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Qiskit/qiskit-metal",
     author="Qiskit Metal Development Team",
     author_email="qiskit@qiskit.org",
     license="Apache 2.0",
@@ -39,23 +39,22 @@
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering",
     ],
     keywords="qiskit sdk quantum eda",
     packages=find_packages(),
     package_data={"": ["*.ui", "*.qrc", "_imgs/*.png", "_imgs/*.txt"]},
-    python_requires=">=3.7",
+    python_requires=">=3.9",
     install_requires=requirements,
     project_urls={
         "Bug Tracker": "https://github.com/Qiskit/qiskit-metal/issues",
         "Documentation": "https://qiskit.org/documentation/metal",
         "Source Code": "https://github.com/Qiskit/qiskit-metal",
     },
 )
```

