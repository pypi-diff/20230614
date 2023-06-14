# Comparing `tmp/srsgui-0.3.2.tar.gz` & `tmp/srsgui-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-7nux2nup\srsgui-0.3.2.tar", last modified: Wed May 24 20:23:50 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-wgfwh6vd\srsgui-0.3.3.tar", last modified: Wed Jun 14 20:06:43 2023, max compression
```

## Comparing `srsgui-0.3.2.tar` & `srsgui-0.3.3.tar`

### file list

```diff
@@ -1,118 +1,123 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.805499 srsgui-0.3.2/
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.725521 srsgui-0.3.2/.github/
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.729527 srsgui-0.3.2/.github/workflows/
--rw-rw-rw-   0        0        0      388 2023-05-16 19:47:28.000000 srsgui-0.3.2/.github/workflows/pages.yml
--rw-rw-rw-   0        0        0     1356 2023-05-16 23:33:10.000000 srsgui-0.3.2/.gitignore
--rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3725 2023-05-24 20:23:50.805499 srsgui-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2745 2023-05-16 20:18:44.000000 srsgui-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.749520 srsgui-0.3.2/docs/
--rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.755524 srsgui-0.3.2/docs/_static/
--rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0      305 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/changelog.rst
--rw-rw-rw-   0        0        0     1957 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/conf.py
--rw-rw-rw-   0        0        0     6097 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/create-task.rst
--rw-rw-rw-   0        0        0     6111 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/define-instrument.rst
--rw-rw-rw-   0        0        0    15640 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/example.rst
--rw-rw-rw-   0        0        0     3726 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/index.rst
--rw-rw-rw-   0        0        0     4407 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/make.bat
--rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.3.2/docs/requirements..txt
--rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      950 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/srsgui.inst.rst
--rw-rw-rw-   0        0        0      113 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/srsgui.rst
--rw-rw-rw-   0        0        0     1077 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/srsgui.task.rst
--rw-rw-rw-   0        0        0     2065 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/srsgui.ui.commandtree.rst
--rw-rw-rw-   0        0        0      603 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1646 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/srsgui.ui.rst
--rw-rw-rw-   0        0        0      465 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/troubleshooting.rst
--rw-rw-rw-   0        0        0     1498 2023-05-23 19:19:21.000000 srsgui-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.3.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 20:23:50.805499 srsgui-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.755524 srsgui-0.3.2/srsgui/
--rw-rw-rw-   0        0        0     1537 2023-05-24 20:05:04.000000 srsgui-0.3.2/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.3.2/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.729527 srsgui-0.3.2/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.765521 srsgui-0.3.2/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.765521 srsgui-0.3.2/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-05-15 21:54:54.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.775516 srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2250 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.775516 srsgui-0.3.2/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.3.2/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9907 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.775516 srsgui-0.3.2/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.3.2/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8774 2023-05-23 19:19:21.000000 srsgui-0.3.2/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    15009 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10410 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9823 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.785510 srsgui-0.3.2/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.3.2/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      811 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6606 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5417 2023-05-23 19:19:21.000000 srsgui-0.3.2/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6938 2023-05-23 19:19:21.000000 srsgui-0.3.2/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    23468 2023-05-23 19:19:21.000000 srsgui-0.3.2/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.795505 srsgui-0.3.2/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.3.2/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     6880 2023-05-24 20:09:40.000000 srsgui-0.3.2/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.805499 srsgui-0.3.2/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0        0 2023-05-19 00:30:39.000000 srsgui-0.3.2/srsgui/ui/commandtree/__init__.py
--rw-rw-rw-   0        0        0     3941 2023-05-23 19:11:06.000000 srsgui-0.3.2/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/commandtree/commandhandler.py
--rw-rw-rw-   0        0        0    12359 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     8669 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     5109 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     4851 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.3.2/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9798 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    15880 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    13826 2023-05-23 19:19:21.000000 srsgui-0.3.2/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.805499 srsgui-0.3.2/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1449 2023-05-23 19:19:21.000000 srsgui-0.3.2/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.3.2/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.3.2/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    25599 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.3.2/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.3.2/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.765521 srsgui-0.3.2/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3725 2023-05-24 20:23:50.000000 srsgui-0.3.2/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3008 2023-05-24 20:23:50.000000 srsgui-0.3.2/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 20:23:50.000000 srsgui-0.3.2/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-24 20:23:50.000000 srsgui-0.3.2/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-05-24 20:23:50.000000 srsgui-0.3.2/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 20:23:50.000000 srsgui-0.3.2/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.304418 srsgui-0.3.3/
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.153942 srsgui-0.3.3/.github/
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.163914 srsgui-0.3.3/.github/workflows/
+-rw-rw-rw-   0        0        0      388 2023-05-16 19:47:28.000000 srsgui-0.3.3/.github/workflows/pages.yml
+-rw-rw-rw-   0        0        0     1356 2023-05-16 23:33:10.000000 srsgui-0.3.3/.gitignore
+-rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3965 2023-06-14 20:06:43.304418 srsgui-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2985 2023-06-08 18:01:11.000000 srsgui-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.194236 srsgui-0.3.3/docs/
+-rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.214237 srsgui-0.3.3/docs/_static/
+-rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    88057 2023-06-08 18:01:11.000000 srsgui-0.3.3/docs/_static/dock_widget_floating.png
+-rw-rw-rw-   0        0        0    97266 2023-06-08 18:01:11.000000 srsgui-0.3.3/docs/_static/dock_widgets_expanded.png
+-rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    52123 2023-06-08 23:01:31.000000 srsgui-0.3.3/docs/_static/lockin-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    38581 2023-06-08 18:01:11.000000 srsgui-0.3.3/docs/_static/task_selection.png
+-rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     8513 2023-06-12 22:58:25.000000 srsgui-0.3.3/docs/application.rst
+-rw-rw-rw-   0        0        0      305 2023-05-24 20:30:53.000000 srsgui-0.3.3/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1924 2023-06-08 18:01:11.000000 srsgui-0.3.3/docs/conf.py
+-rw-rw-rw-   0        0        0     6097 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-06-08 23:01:31.000000 srsgui-0.3.3/docs/create-task.rst
+-rw-rw-rw-   0        0        0     6112 2023-06-08 23:01:31.000000 srsgui-0.3.3/docs/define-instrument.rst
+-rw-rw-rw-   0        0        0    15640 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/example.rst
+-rw-rw-rw-   0        0        0     3803 2023-06-13 16:35:19.000000 srsgui-0.3.3/docs/index.rst
+-rw-rw-rw-   0        0        0     4405 2023-06-09 21:01:03.000000 srsgui-0.3.3/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/make.bat
+-rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.3.3/docs/requirements..txt
+-rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      930 2023-06-08 18:01:11.000000 srsgui-0.3.3/docs/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      113 2023-05-24 20:30:53.000000 srsgui-0.3.3/docs/srsgui.rst
+-rw-rw-rw-   0        0        0     1077 2023-05-24 20:30:53.000000 srsgui-0.3.3/docs/srsgui.task.rst
+-rw-rw-rw-   0        0        0     2065 2023-05-24 20:30:53.000000 srsgui-0.3.3/docs/srsgui.ui.commandtree.rst
+-rw-rw-rw-   0        0        0      603 2023-05-24 20:30:53.000000 srsgui-0.3.3/docs/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1646 2023-05-24 20:30:53.000000 srsgui-0.3.3/docs/srsgui.ui.rst
+-rw-rw-rw-   0        0        0      620 2023-06-14 16:11:01.000000 srsgui-0.3.3/docs/troubleshooting.rst
+-rw-rw-rw-   0        0        0     1489 2023-06-14 20:05:33.000000 srsgui-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.3.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 20:06:43.314386 srsgui-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.214237 srsgui-0.3.3/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-06-14 20:05:24.000000 srsgui-0.3.3/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.3.3/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.153942 srsgui-0.3.3/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.224236 srsgui-0.3.3/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.224236 srsgui-0.3.3/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-05-15 21:54:54.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.234237 srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2250 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.244265 srsgui-0.3.3/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.3.3/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9907 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.254237 srsgui-0.3.3/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.3.3/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8774 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    15127 2023-06-08 18:01:11.000000 srsgui-0.3.3/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10410 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9826 2023-06-08 18:01:11.000000 srsgui-0.3.3/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.264267 srsgui-0.3.3/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.3.3/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      811 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6606 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5417 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6938 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    23469 2023-06-08 18:01:11.000000 srsgui-0.3.3/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.284384 srsgui-0.3.3/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.3.3/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     6880 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.304418 srsgui-0.3.3/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0        0 2023-05-19 00:30:39.000000 srsgui-0.3.3/srsgui/ui/commandtree/__init__.py
+-rw-rw-rw-   0        0        0     3941 2023-05-23 19:11:06.000000 srsgui-0.3.3/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/commandtree/commandhandler.py
+-rw-rw-rw-   0        0        0    12359 2023-06-08 18:01:11.000000 srsgui-0.3.3/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     8669 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     5109 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     4851 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.3.3/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9798 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    15880 2023-06-08 18:01:11.000000 srsgui-0.3.3/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    13826 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.304418 srsgui-0.3.3/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1449 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.3.3/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.3.3/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    25601 2023-06-08 23:01:31.000000 srsgui-0.3.3/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.3.3/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.3.3/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.224236 srsgui-0.3.3/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3965 2023-06-14 20:06:43.000000 srsgui-0.3.3/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3170 2023-06-14 20:06:43.000000 srsgui-0.3.3/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 20:06:43.000000 srsgui-0.3.3/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-14 20:06:43.000000 srsgui-0.3.3/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      103 2023-06-14 20:06:43.000000 srsgui-0.3.3/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-14 20:06:43.000000 srsgui-0.3.3/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.3.2/.gitignore` & `srsgui-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/LICENSE.txt` & `srsgui-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/PKG-INFO` & `srsgui-0.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.3.2
+Version: 0.3.3
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
@@ -20,19 +20,19 @@
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 # ``Srsgui`` - Organize instrument-controlling Python scripts as a GUI application
 
-`Srsgui` is a simple platform:
+`Srsgui` is a simple framework:
 
    - To define instrument classes for instruments that use remote communication,
      based on `Instrument` class and the communication `Interface` class 
-     (By default, serial, TCPIP is available, extendable to VXI11, GPIB and USB-TMC).
+     (By default, serial and TCPIP is available. VXI11, GPIB and USB-TMC are optional.).
 
    - To write Python scripts (tasks) that run in GUI environment with simple APIs
      provided in ``Task`` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
      using a configuration (.taskconfig) file for a project
 
@@ -41,58 +41,56 @@
 ## Installation
 
 To run ``srsgui`` as an application, create a virtual environment, if necessary, 
 and install using ``pip`` with [full] option:  
 
     python -m pip install srsgui[full]
 
-if it fails, you have to install 
+``Srsgui`` package has the following 3 main dependencies: 
 [pyserial](https://pypi.org/project/pyserial/), 
-[matplotlib](https://pypi.org/project/matplotlib/) and 
-a Python Qt binder ([PySide6](https://pypi.org/project/PySide6/),
-[PySide2](https://pypi.org/project/PySide2/) or 
-[PyQt5](https://pypi.org/project/PyQt5/)) manually.
-``srsgui`` package has these 3 dependencies only.
-
-Some Linux distributions offer some of the Python packages from their 
-repositories only, not from ``pip``. Run web search for more information on 
-system specific installation.   
-
-When matplotlib and one of the Qt binders
-are installed properly, install ``srsgui`` without [full] option:
+[matplotlib](https://pypi.org/project/matplotlib/) and
+[PySide6](https://pypi.org/project/PySide6/). If the installation above fails, 
+you have to install the failed pacakge manually. Using a virtual environment will
+eliminate possible conflicts between packages in the main Python installation and 
+the packagesSome used in `srsgui`. Some Linux distributions offer 
+some of the Python packages from their repositories only, not from ``pip``. 
+Run web search for more information on system-specific installation.   
+
+Once pyserial, matplotlib and PySide6 are installed properly, or you plan to use
+`srsgui` for instrument drivers only without GUI support, 
+you can install ``srsgui`` without [full] option:
 
     python -m pip install srsgui
 
 ## Start ``srsgui`` application
     
 if the Python Script directory is in PATH environment variable,
 Start the application by typing from the command line:
 
     srsgui
-    
 
-If the script directory is not in PATH,
+If the script directory is not in PATH, run the srsgui module with Python. 
 
     python -m srsgui
     
 It will start `srsgui` application.
 
 ## Run the example project
 
 By default, `srsgui` application starts with the last project it ran,
 when it is closed.
  
 To open the example project included in the `srsgui` package 
-(if it does not start with the example project), go to the `srsgui` package 
-directory, find the examples directory, and find a .taskconfig file in an 
-example project folder. 
+(if `srsgui` does not start with the example project), select the menu/File/Open config, 
+go to the `srsgui` package directory, find the examples directory, and find a .taskconfig file
+in the example project folder. 
 
 You can run the second and fifth task in the Task menu 
 even without any instruments connected.
 
 ## Create a project
 
-`Srsgui` is a platform that helps you to write your own instrument-controlling 
+`Srsgui` is a framework to helps you to write your own instrument-controlling 
 Python scripts running as a GUI application. Using its APIs, you can write 
 scripts running in GUI with the same amount of code with writing console-based 
 scripts. For programming API, refer to
 [`srsgui` documentation](https://thinksrs.github.io/srsgui).
```

### Comparing `srsgui-0.3.2/README.md` & `srsgui-0.3.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ``Srsgui`` - Organize instrument-controlling Python scripts as a GUI application
 
-`Srsgui` is a simple platform:
+`Srsgui` is a simple framework:
 
    - To define instrument classes for instruments that use remote communication,
      based on `Instrument` class and the communication `Interface` class 
-     (By default, serial, TCPIP is available, extendable to VXI11, GPIB and USB-TMC).
+     (By default, serial and TCPIP is available. VXI11, GPIB and USB-TMC are optional.).
 
    - To write Python scripts (tasks) that run in GUI environment with simple APIs
      provided in ``Task`` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
      using a configuration (.taskconfig) file for a project
 
@@ -17,58 +17,56 @@
 ## Installation
 
 To run ``srsgui`` as an application, create a virtual environment, if necessary, 
 and install using ``pip`` with [full] option:  
 
     python -m pip install srsgui[full]
 
-if it fails, you have to install 
+``Srsgui`` package has the following 3 main dependencies: 
 [pyserial](https://pypi.org/project/pyserial/), 
-[matplotlib](https://pypi.org/project/matplotlib/) and 
-a Python Qt binder ([PySide6](https://pypi.org/project/PySide6/),
-[PySide2](https://pypi.org/project/PySide2/) or 
-[PyQt5](https://pypi.org/project/PyQt5/)) manually.
-``srsgui`` package has these 3 dependencies only.
-
-Some Linux distributions offer some of the Python packages from their 
-repositories only, not from ``pip``. Run web search for more information on 
-system specific installation.   
-
-When matplotlib and one of the Qt binders
-are installed properly, install ``srsgui`` without [full] option:
+[matplotlib](https://pypi.org/project/matplotlib/) and
+[PySide6](https://pypi.org/project/PySide6/). If the installation above fails, 
+you have to install the failed pacakge manually. Using a virtual environment will
+eliminate possible conflicts between packages in the main Python installation and 
+the packagesSome used in `srsgui`. Some Linux distributions offer 
+some of the Python packages from their repositories only, not from ``pip``. 
+Run web search for more information on system-specific installation.   
+
+Once pyserial, matplotlib and PySide6 are installed properly, or you plan to use
+`srsgui` for instrument drivers only without GUI support, 
+you can install ``srsgui`` without [full] option:
 
     python -m pip install srsgui
 
 ## Start ``srsgui`` application
     
 if the Python Script directory is in PATH environment variable,
 Start the application by typing from the command line:
 
     srsgui
-    
 
-If the script directory is not in PATH,
+If the script directory is not in PATH, run the srsgui module with Python. 
 
     python -m srsgui
     
 It will start `srsgui` application.
 
 ## Run the example project
 
 By default, `srsgui` application starts with the last project it ran,
 when it is closed.
  
 To open the example project included in the `srsgui` package 
-(if it does not start with the example project), go to the `srsgui` package 
-directory, find the examples directory, and find a .taskconfig file in an 
-example project folder. 
+(if `srsgui` does not start with the example project), select the menu/File/Open config, 
+go to the `srsgui` package directory, find the examples directory, and find a .taskconfig file
+in the example project folder. 
 
 You can run the second and fifth task in the Task menu 
 even without any instruments connected.
 
 ## Create a project
 
-`Srsgui` is a platform that helps you to write your own instrument-controlling 
+`Srsgui` is a framework to helps you to write your own instrument-controlling 
 Python scripts running as a GUI application. Using its APIs, you can write 
 scripts running in GUI with the same amount of code with writing console-based 
 scripts. For programming API, refer to
 [`srsgui` documentation](https://thinksrs.github.io/srsgui).
```

### Comparing `srsgui-0.3.2/docs/Makefile` & `srsgui-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.3.3/docs/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/_static/cg-terminal-screen-capture.png` & `srsgui-0.3.3/docs/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/_static/connect-dialog-box-capture.png` & `srsgui-0.3.3/docs/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/_static/example-screen-capture-1.png` & `srsgui-0.3.3/docs/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/_static/example-screen-capture-2.png` & `srsgui-0.3.3/docs/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/_static/initial-screen-capture.png` & `srsgui-0.3.3/docs/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.3.3/docs/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/_static/second-task-screen-capture.png` & `srsgui-0.3.3/docs/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/_static/terminal-with-example-2.png` & `srsgui-0.3.3/docs/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/_static/terminal-with-example.png` & `srsgui-0.3.3/docs/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/conf.py` & `srsgui-0.3.3/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,20 +39,16 @@
     # example_package/autodoctest/doc/source/_templates/autosummary/class.rst
     # and other defaults in sphinx-autodoc.
     'show-inheritance': True,
     'inherited-members': False,
     'no-special-members': True,
 }
 
-
 templates_path = ['_templates']
 exclude_patterns = []
 
-
-
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'sphinx_rtd_theme'
-#html_theme = 'alabaster'
 
 html_static_path = ['_static']
```

### Comparing `srsgui-0.3.2/docs/create-project.rst` & `srsgui-0.3.3/docs/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/create-task.rst` & `srsgui-0.3.3/docs/create-task.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 Writing a task script
 -----------------------
 
-When you write a Python script that runs with `'srsgui``, you make a subclass of
+When you write a Python script that runs with ``srsgui``, you make a subclass of
 :class:`Task <srsgui.task.task.Task>` class, and implement
 :meth:`setup<srsgui.task.task.Task.setup>`,
 :meth:`test<srsgui.task.task.Task.test>` and
 :meth:`cleanup<srsgui.task.task.Task.cleanup>`.
 
 Following is the simplest form of a task. Even though it does not do much,
 ``srsgui`` is happy to run the task, if it is included in a .taskconfig file.
```

### Comparing `srsgui-0.3.2/docs/define-instrument.rst` & `srsgui-0.3.3/docs/define-instrument.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-Defining instrument classes------------------------------an instrument class is a subclass derived from the:class:`Instrument<srsgui.inst.instrument.Instrument>` class.Minimum requirement is to have **_IdString** to check if a connectedinstrument is a correct instrument  that can be used with the class... code-block::    from srsgui import Instrument    class CG635(Instrument):        _IdString = 'CG635'        _term_char = b'\r'  # Add this line if the carriage return is the termination character                            # of the instrument, instead of the line feed (ASCII: 0x10, b'\n').If the instrument has:    1. the **\*IDN?** remote command    2. either RS232 serial communication or Ethernet TCPIP communication port available,the instrument can be connected and used in task scripts and in the terminal,with 4 lines of definition like above. If it does not have the \*IDN? remote command,:meth:`check_id()<srsgui.inst.instrument.Instrument.check_id>` method in Instrumentclass needs to be reimplemented.Available_interfaces^^^^^^^^^^^^^^^^^^^^^`Available_interface` defines what kind of communication is available for the instrument,the base :class:`Instrument<srsgui.inst.instrument.Instrument>` class has the followingdefinition for serial and TCPIP communication interfaces:.. code-block::    available_interfaces = [        [   SerialInterface,            {                'port': FindListInput(),                'baud_rate': IntegerListInput([9600, 115200]),                'hardware_flow_control': BoolInput(['Off', 'On'])            }        ],        [   TcpipInterface,            {                'ip_address': Ip4Input('192.168.1.10'),                'port': IntegerInput(23)            }        ]    ]If your instrument needs other than serial and TCPIP interfaces, ``srsgui`` allows to addother communication classes derived from:class:`Interface <srsgui.inst.communication.interface.Interface>` class.Currently there are two external communication interfaces are available from`srsinst.sr860`_ package: ``Vxi11Interface`` and ``VisaInterface``,which covers for VXI11_, GPIB_ and USB-TMC_. You can import the interface modulesfrom `srsinst.sr860`_ .Available_interfaces in SSR865 class is define as following:.. code-block::    available_interfaces = [        [   Vxi11Interface,            {                'ip_address': Ip4Input('192.168.1.10'),            }        ],        [   VisaInterface,            {                'resource': FindListInput(),            }        ],        [   TcpipInterface,            {                'ip_address': Ip4Input('192.168.1.10'),                'port': 23            }        ],        [   SerialInterface,            {                'port': FindListInput(),                'baud_rate': IntegerListInput([9600, 19200, 38400, 115200,                                               230400, 460800], 3)            }        ],    ]The definition of available_interfaces is all you need to do to get a customizeddialog box opened for the instrument in ``srsgui`` application... figure:: ./_static/connect-dialog-box-capture.png    :align: center    :figclass: align-centerFor ``VisaInterface``, you have to get PyVISA_ working before running ``srsgui`` application.It involves installation of the PyVISA package and its backend library.Refer to PyVISA_ documentation for installation detail.From Python interpreter, you can connect and use a instrument, once its ``Instrument`` class is defined... code-block::    C:\srsgui>python    Python 3.8.3 (tags/v3.8.3:6f8c832, May 13 2020, 22:37:02) [MSC v.1924 64 bit (AMD64)] on win32    Type "help", "copyright", "credits" or "license" for more information.    >>>    >>> from srsinst.sr860 import SR860    >>> from srsgui import SerialInte    >>> SerialInterface.find()    ['COM3', 'COM4', 'COM256']    >>> lia = SR860('serial','COM4',115200, False)    >>> lia.query_text('*idn?')    'Stanford_Research_Systems,SR865A,002725,v1.34'    >>> lia.disconnect()    >>>    >>> from srsinst.sr860 import VisaInterface    >>> VisaInterface.find()    ['USB0::0xB506::0x2000::002725::INSTR', 'GPIB0::4::INSTR']    >>> lia.connect('visa', 'USB0::0xB506::0x2000::002725::INSTR')    >>> lia.query_text('*idn?')    'Stanford_Research_Systems,SR865A,002725,v1.34\n'    >>>Well, these operations are what you can do with PyVISA_ itself. Defining an instrument class,adding it in a .taskconfig file, and opening it in ``srsgui`` application let youuse the terminal to interact with multiple instrument at once, and use high level ``Instrument``class attributes and methods.Below is an image of terminal captured with the example project opened.As you can see, you can interact with the clock generator and oscilloscope in many ways.There are two commands for osc: \*idn?, sara? used, and two commands for cg:\*idn?, freq(?) used in the terminal... figure:: ./_static/terminal-with-example.png    :align: center    :figclass: align-center|Component, Commands and IndexCommands^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^:class:`Instrument <srsgui.inst.instrument.Instrument>` class uses:class:`Component <srsgui.inst.component.Component>` class,:mod:`Command <srsgui.inst.commands>` classes and:mod:`IndexCommand <srsgui.inst.indexcommands>` classesto organize the functionality of an instrument.If you have to deal with hundreds of remote commands to use an instrument remotely,organizing them in a manageable way is crucial. `Srsinst.sr860`_ package shows how theseconvenience classes are used to organize a large set of remote commands... _PyVisa: https://pyvisa.readthedocs.io/en/latest/.. _srsinst.sr860: https://pypi.org/project/srsinst.sr860/.. _VXI11: https://www.lxistandard.org/About/VXI-11-and-LXI.aspx.. _GPIB: https://en.wikipedia.org/wiki/IEEE-488.. _USB-TMC: https://www.testandmeasurementtips.com/remote-communication-with-usbtmc-faq/.. _thread: https://realpython.com/intro-to-python-threading/.. _QThread: https://doc.qt.io/qt-6/qthread.html
+Defining an instrument class------------------------------an instrument class is a subclass derived from the:class:`Instrument<srsgui.inst.instrument.Instrument>` class.Minimum requirement is to have **_IdString** to check if a connectedinstrument is a correct instrument  that can be used with the class... code-block::    from srsgui import Instrument    class CG635(Instrument):        _IdString = 'CG635'        _term_char = b'\r'  # Add this line if the carriage return is the termination character                            # of the instrument, instead of the line feed (ASCII: 0x10, b'\n').If the instrument has:    1. the **\*IDN?** remote command    2. either RS232 serial communication or Ethernet TCPIP communication port available,the instrument can be connected and used in task scripts and in the terminal,with 4 lines of definition like above. If it does not have the \*IDN? remote command,:meth:`check_id()<srsgui.inst.instrument.Instrument.check_id>` method in Instrumentclass needs to be reimplemented.Available_interfaces^^^^^^^^^^^^^^^^^^^^^`Available_interface` defines what kind of communication is available for the instrument,the base :class:`Instrument<srsgui.inst.instrument.Instrument>` class has the followingdefinition for serial and TCPIP communication interfaces:.. code-block::    available_interfaces = [        [   SerialInterface,            {                'port': FindListInput(),                'baud_rate': IntegerListInput([9600, 115200]),                'hardware_flow_control': BoolInput(['Off', 'On'])            }        ],        [   TcpipInterface,            {                'ip_address': Ip4Input('192.168.1.10'),                'port': IntegerInput(23)            }        ]    ]If your instrument needs other than serial and TCPIP interfaces, ``srsgui`` allows to addother communication classes derived from:class:`Interface <srsgui.inst.communication.interface.Interface>` class.Currently there are two external communication interfaces are available from`srsinst.sr860`_ package: ``Vxi11Interface`` and ``VisaInterface``,which covers for VXI11_, GPIB_ and USB-TMC_. You can import the interface modulesfrom `srsinst.sr860`_ .Available_interfaces in SSR865 class is define as following:.. code-block::    available_interfaces = [        [   Vxi11Interface,            {                'ip_address': Ip4Input('192.168.1.10'),            }        ],        [   VisaInterface,            {                'resource': FindListInput(),            }        ],        [   TcpipInterface,            {                'ip_address': Ip4Input('192.168.1.10'),                'port': 23            }        ],        [   SerialInterface,            {                'port': FindListInput(),                'baud_rate': IntegerListInput([9600, 19200, 38400, 115200,                                               230400, 460800], 3)            }        ],    ]The definition of available_interfaces is all you need to do to get a customizeddialog box opened for the instrument in ``srsgui`` application... figure:: ./_static/connect-dialog-box-capture.png    :align: center    :figclass: align-centerFor ``VisaInterface``, you have to get PyVISA_ working before running ``srsgui`` application.It involves installation of the PyVISA package and its backend library.Refer to PyVISA_ documentation for installation detail.From Python interpreter, you can connect and use a instrument, once its ``Instrument`` class is defined... code-block::    C:\srsgui>python    Python 3.8.3 (tags/v3.8.3:6f8c832, May 13 2020, 22:37:02) [MSC v.1924 64 bit (AMD64)] on win32    Type "help", "copyright", "credits" or "license" for more information.    >>>    >>> from srsinst.sr860 import SR860    >>> from srsgui import SerialInte    >>> SerialInterface.find()    ['COM3', 'COM4', 'COM256']    >>> lia = SR860('serial','COM4',115200, False)    >>> lia.query_text('*idn?')    'Stanford_Research_Systems,SR865A,002725,v1.34'    >>> lia.disconnect()    >>>    >>> from srsinst.sr860 import VisaInterface    >>> VisaInterface.find()    ['USB0::0xB506::0x2000::002725::INSTR', 'GPIB0::4::INSTR']    >>> lia.connect('visa', 'USB0::0xB506::0x2000::002725::INSTR')    >>> lia.query_text('*idn?')    'Stanford_Research_Systems,SR865A,002725,v1.34\n'    >>>Well, these operations are what you can do with PyVISA_ itself. Defining an instrument class,adding it in a .taskconfig file, and opening it in ``srsgui`` application let youuse the terminal to interact with multiple instrument at once, and use high level ``Instrument``class attributes and methods.Below is an image of terminal captured with the example project opened.As you can see, you can interact with the clock generator and oscilloscope in many ways.There are two commands for osc: \*idn?, sara? used, and two commands for cg:\*idn?, freq(?) used in the terminal... figure:: ./_static/terminal-with-example.png    :align: center    :figclass: align-center|Component, Commands and IndexCommands^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^:class:`Instrument <srsgui.inst.instrument.Instrument>` class uses:class:`Component <srsgui.inst.component.Component>` class,:mod:`Command <srsgui.inst.commands>` classes and:mod:`IndexCommand <srsgui.inst.indexcommands>` classesto organize the functionality of an instrument.If you have to deal with hundreds of remote commands to use an instrument remotely,organizing them in a manageable way is crucial. `Srsinst.sr860`_ package shows how theseconvenience classes are used to organize a large set of remote commands... _PyVisa: https://pyvisa.readthedocs.io/en/latest/.. _srsinst.sr860: https://pypi.org/project/srsinst.sr860/.. _VXI11: https://www.lxistandard.org/About/VXI-11-and-LXI.aspx.. _GPIB: https://en.wikipedia.org/wiki/IEEE-488.. _USB-TMC: https://www.testandmeasurementtips.com/remote-communication-with-usbtmc-faq/.. _thread: https://realpython.com/intro-to-python-threading/.. _QThread: https://doc.qt.io/qt-6/qthread.html
```

### Comparing `srsgui-0.3.2/docs/example.rst` & `srsgui-0.3.3/docs/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/index.rst` & `srsgui-0.3.3/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 .. srsgui documentation master file, created by
    sphinx-quickstart on Wed Dec  7 16:34:11 2022.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 
-``srsgui`` : Organize your instrument-controlling Python scripts as a GUI application
+``Srsgui`` : Organize your instrument-controlling Python scripts as a GUI application
 =======================================================================================
 
 ``Srsgui`` is a simple framework:
 
    - To define instrument classes for instruments that use remote communication,
      based on :class:`Instrument<srsgui.inst.instrument.Instrument>`
      class and the communication
      :class:`Interface<srsgui.inst.communications.interface.Interface>` class.
 
-   - To write Python scripts (tasks) that run in GUI environment with simple APIs
+   - To write Python scripts (tasks) that run in GUI environment with APIs
      provided in :class:`Task<srsgui.task.task.Task>` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
      using a configuration (.taskconfig) file for a project
 
 ``Srsgui`` provides the following I/O functionality to a task:
 
-   - Python logging output to a console window and a log file
+   - Python logging_ output to the console window and a log file
    - `print` function redirected to the console window
-   - text streaming to multiple selectable windows
-   - terminal from which you can control and query interactively all the instrument defined in the configuration file
-   - real-time updating, non-blocking, multiple matplotlib figures_ that can include multiple axes_
-   - interactively changeable  input parameters fed into a running task
-   - Qt's dockable windows makes layout flexible(
+   - Text streaming to multiple windows
+   - Terminal from which you can control and query interactively all the instrument
+     defined in the configuration file
+   - Real-time updating, non-blocking, multiple matplotlib figures_ that can include multiple axes_
+   - Interactively changeable  input parameters fed into a running task
+   - Qt's dockable widgets makes layout flexible(
      :ref:`before <top-of-initial-screen-capture>` and
      :ref:`after <top-of-screen-capture-1>`)
-   - dedicated output data file generated for each run of a task
+   - Dedicated output data file generated for each run of a task
 
 Here is a screen shot of ``srsgui`` running with the :ref:`example project <top-of-example-project>`
 included in the ``srsgui`` package.
 
 .. _top-of-screen-capture-1:
 
 .. figure:: ./_static/example-screen-capture-2.png
     :align: center
     :figclass: align-center
 
-From the :ref:`Example project <top-of-example-project>` directory, you can see how many lines of code
-you need write to get ``srsgui`` working for control and data acquisition
+From the :ref:`Example project <top-of-example-project>` directory, you can see
+how many lines of code you need to write to get ``srsgui`` working for control and data acquisition
 from a couple of arbitrary instruments and data visualization for a small task.
 
    - 5 lines of code for CG635 to control its
      output frequency (if not count comment lines);
    - 40 lines to capture waveforms from an oscilloscope (it has a method
      to download a waveform from the oscilloscope);
    - 100 lines in the fourth example to check if set frequency
@@ -66,14 +67,15 @@
 Here are more information on how to use ``srsgui``.
 
 
 .. toctree::
    :maxdepth: 2
 
    installation.rst
+   application.rst
    create-project.rst
    define-instrument.rst
    create-task.rst
    example.rst
    srsgui.rst
    troubleshooting.rst
    changelog.rst
@@ -82,8 +84,9 @@
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
 
 .. _figures: https://matplotlib.org/stable/tutorials/introductory/quick_start.html#figure
-.. _axes: https://matplotlib.org/stable/tutorials/introductory/quick_start.html#axes
+.. _axes: https://matplotlib.org/stable/tutorials/introductory/quick_start.html#axes
+.. _logging: https://docs.python.org/3/library/logging.html
```

### Comparing `srsgui-0.3.2/docs/installation.rst` & `srsgui-0.3.3/docs/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Installation
 ==============
 
 Preparation
 ------------
 
 To install ``srsgui``,  make sure you have Python version 3.7 or later.
-you can check your Python version by running from the command line:
+you can check your Python version by running from the command prompt:
 
 .. code-block::
 
     python --version
 
 .. note::
 
@@ -17,15 +17,15 @@
     a Windows computer system. If you use other systems, commands may be
     different. Refer to `this page. <install-packages_>`_
 
 If you have a Python older than the required version,
 `install a newer Python. <install-python_>`_
 
 Using `virtual environment <virtual-environment_>`_ helps to avoid possible dependency
-conflict among Python packages. If you want to use a virtual environment, create one with
+conflicts among Python packages. If you want to use a virtual environment, create one with
 your favorite virtual environment package. If you do not have a preference,
 use Python default ``venv``.
 
 .. code-block::
 
     python -m venv env
     .\env\Scripts\activate
@@ -72,18 +72,18 @@
 
     will show if pyside2_ or pyqt5_ is installed.
 
 .. note::
     In order to maintain the MIT_ license for your projects or modified ``srsgui``, you have to use
     pyside6_ or pyside2_. Note that pyqt5_ imposes GPLv3_ license to packages using pyqt5_.
 
-Running srsgui application
+Starting srsgui application
 ----------------------------
 
-After ``srsgui`` is installed, you can start ``srsgui`` application from the command line
+After ``srsgui`` is installed, you can start ``srsgui`` application from the command prompt.
 
 .. code-block::
 
     srsgui
 
     or
 
@@ -100,20 +100,22 @@
     :figclass: align-center
 
 If you see the application is open and running, the installation is successful!
 
 .. note::
     Instead of seeing the application running, you may get errors, probably ImportError.
     Carefully look through the exception traceback to find out which package causes the error.
-    When the latest python is installed, some packages may not install properly. If the problem
+    When the latest python is installed, some packages may not be installed properly. If the problem
     is not from ``srsgui`` directly, web search of the problem usually leads to a fix.
 
 
+
+
 .. _install-packages: https://packaging.python.org/en/latest/tutorials/installing-packages/
-.. _install-python: https://realpython.com/installing-python/
+.. _install-python: https://www.python.org/
 .. _virtual-environment: https://realpython.com/python-virtual-environments-a-primer/
 .. _venv: https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/
 .. _pip: https://realpython.com/what-is-pip/
 .. _pyserial: https://pyserial.readthedocs.io/en/latest/pyserial.html
 .. _matplotlib: https://matplotlib.org/stable/tutorials/introductory/quick_start.html
 .. _pyside6: https://wiki.qt.io/Qt_for_Python
 .. _pyside2: https://pypi.org/project/PySide2/
```

### Comparing `srsgui-0.3.2/docs/make.bat` & `srsgui-0.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/srsgui.inst.communications.rst` & `srsgui-0.3.3/docs/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/srsgui.inst.rst` & `srsgui-0.3.3/docs/srsgui.inst.rst`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,14 @@
    :show-inheritance:
 
 srsgui.inst.component module
 ----------------------------
 
 .. automodule:: srsgui.inst.component
    :members:
-   :undoc-members:
    :show-inheritance:
 
 srsgui.inst.commands module
 ---------------------------
 
 .. automodule:: srsgui.inst.commands
    :members:
```

### Comparing `srsgui-0.3.2/docs/srsgui.task.rst` & `srsgui-0.3.3/docs/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/srsgui.ui.commandtree.rst` & `srsgui-0.3.3/docs/srsgui.ui.commandtree.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/srsgui.ui.qt.rst` & `srsgui-0.3.3/docs/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/docs/srsgui.ui.rst` & `srsgui-0.3.3/docs/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/pyproject.toml` & `srsgui-0.3.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "srsgui.__version__"}
 
 [project.optional-dependencies]
-full = ['matplotlib >= 3.6.2', 'pyside6 <= 6.4.3']
-docs = ['matplotlib', 'pyside2', 'sphinx>=5', 'sphinx-rtd-theme>=1']
+full = ['matplotlib >= 3.6.2', 'pyside6']
+docs = ['matplotlib', 'pyside6', 'sphinx>=5', 'sphinx-rtd-theme>=1']
 
 [project.urls]
 homepage = "https://github.com/thinkSRS/srsgui"
 repository = "https://github.com/thinkSRS/srsgui.git"
 documentation = "https://thinksrs.github.io/srsgui"
 changelog = "https://thinksrs.github.io/srsgui/changelog.html"
```

### Comparing `srsgui-0.3.2/srsgui/__init__.py` & `srsgui-0.3.3/srsgui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.3.2"  # Global version number
+__version__ = "0.3.3"  # Global version number
```

### Comparing `srsgui-0.3.2/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.3.3/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.3.3/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.3.3/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/inst/__init__.py` & `srsgui-0.3.3/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/inst/commands.py` & `srsgui-0.3.3/srsgui/inst/commands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/inst/communications/interface.py` & `srsgui-0.3.3/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/inst/communications/serial_ports.py` & `srsgui-0.3.3/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/inst/communications/serialinterface.py` & `srsgui-0.3.3/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.3.3/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/inst/component.py` & `srsgui-0.3.3/srsgui/inst/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,25 @@
 from .communications import Interface
 from .commands import Command, GetCommand, BoolCommand, IntCommand, \
                       FloatCommand, DictCommand
 from .indexcommands import IndexCommand, BoolIndexCommand, IntIndexCommand, \
                            FloatIndexCommand, DictIndexCommand
 
 
+class DirCommand(GetCommand):
+    """
+    Descriptor to run get_lists() with 'dir' command in Component
+
+    :meta private:
+    """
+    def __get__(self, instance, instance_type):
+        if hasattr(instance, 'get_lists'):
+            return instance.get_lists()
+
+
 class Component(object):
     """
     Class used to build hierarchical structure in an instrument.
 
     An instrument can have multiple components and each component
     can also have multiple subcomponents. All the components
     inside an instrument shares the communication interface
@@ -45,30 +56,25 @@
     The information available from the convenience methods are
     available interactively from context-sensitive editors, such as IDLE, Pycharm, VSCode.
     When the information from the editors are not complete, consulting with
     those convenience methods provides complete lists you can use.
 
     """
 
-    class DirCommand(GetCommand):
-        """
-        Descriptor to run get_lists() with 'dir' command
-        """
-        def __get__(self, instance, instance_type):
-            if hasattr(instance, 'get_lists'):
-                return instance.get_lists()
-
     dir = DirCommand('dir')
-    """ class instance of DirCommand"""
+    """
+    Attribute to be used to get a dictionary that contains information on the subcomponents, 
+    commands, and class method
+    """
 
     exclude_capture = []
     """Exclude commands from query in capture_commands"""
 
     allow_run_button = []
-    """Allow methods to have run buttons in a control panel"""
+    """Allow methods to have run buttons in the GUI control panel"""
 
     def __init__(self, parent, name='unnamed'):
         self._name = name
         self._children = []
         if parent is None:
             self._parent = None
             self.comm = None
@@ -261,15 +267,15 @@
                             .format(command, self.__class__.__name__))
         if key not in cmd.set_dict:
             raise KeyError(f" '{key}' is in {cmd.set_dict} of command '{command}'.")
 
     def capture_commands(self, include_query_only=False, include_set_only=False,
                          include_excluded=False, include_methods=False, show_raw_cmds=False):
         """
-        Query all command with both set and get methods in the component
+        Query all commands with both set and get methods in the component
         and its subcomponents
         """
         commands = {}
 
         # Recursive calls to capture commands from subcomponents
         for j in self.__dict__:
             if j =='_parent':
@@ -362,8 +368,7 @@
                                         commands[name][key] = cmd_instance.__getitem__(index)
                                         break
                             index += 1
                         except Exception as e:
                             print(f'  {type(e)} {e} command:{k} index: {index}')
                             break
         return commands
-
```

### Comparing `srsgui-0.3.2/srsgui/inst/exceptions.py` & `srsgui-0.3.3/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/inst/indexcommands.py` & `srsgui-0.3.3/srsgui/inst/indexcommands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/inst/instrument.py` & `srsgui-0.3.3/srsgui/inst/instrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,16 +182,16 @@
         :return: reply of the remote command
         :rtype: float
         """
         return self.comm.query_float(cmd)
 
     def check_id(self):
         """
-        Check if the ID string of the instrument contains _IdString of the Insteument class
-        A derived instrument class should make sure that check_id method is properly implemented.
+        Check if the ID string of the instrument contains _IdString of the Instrument class.
+        A derived instrument class should make sure that check_id() method is properly implemented.
 
         :return: tuple of (model name, serial number, firmware version)
         """
 
         if not self.is_connected():
             return None, None, None
```

### Comparing `srsgui-0.3.2/srsgui/task/callbacks.py` & `srsgui-0.3.3/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/task/config.py` & `srsgui-0.3.3/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/task/inputs.py` & `srsgui-0.3.3/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/task/sessionhandler.py` & `srsgui-0.3.3/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/task/task.py` & `srsgui-0.3.3/srsgui/task/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         Check frequently if is_running() is true. If not, test() should finish voluntarily
         as soon as possible.
         """
         raise NotImplementedError("A test() should be implemented!")
 
     def cleanup(self):
         """
-        When test() is finished, cleanup() will run subsequently.
+        After test() is finished, cleanup() will run subsequently.
         Any cleanup and closing routine can be added here.
         """
         self.logger.warning('Task.cleanup() is not overridden.')
 
     def get_logger(self, name):
         """
         Get a logger with its handler available from the parent
```

### Comparing `srsgui-0.3.2/srsgui/task/taskresult.py` & `srsgui-0.3.3/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/commandhandler.py` & `srsgui-0.3.3/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/commandterminal.py` & `srsgui-0.3.3/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.3.3/srsgui/ui/commandtree/commanddelegate.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/commandtree/commandhandler.py` & `srsgui-0.3.3/srsgui/ui/commandtree/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.3.3/srsgui/ui/commandtree/commanditem.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.comp_type = None   # There are 5 types of components: Component, Commands, IndexCommands, method and Index
         self.set_enable = False
         self.get_enable = False
         self.is_method = False
         self.excluded = False
         self.raw_remote_command = ""
         self.timestamp = 0.0
-        self.query_update_period = 0.3
+        self.query_update_period = 0.5
 
     def appendChild(self, item: "CommandItem"):
         """Add item as a child"""
         self._children.append(item)
 
     def child(self, row: int) -> "CommandItem":
         """Return the child of the current item from the given row"""
```

### Comparing `srsgui-0.3.2/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.3.3/srsgui/ui/commandtree/commandmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.3.3/srsgui/ui/commandtree/commandspinbox.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.3.3/srsgui/ui/commandtree/commandtreeview.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.3.3/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.3.3/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/connectdlg.py` & `srsgui-0.3.3/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/deviceinfohandler.py` & `srsgui-0.3.3/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/dockhandler.py` & `srsgui-0.3.3/srsgui/ui/dockhandler.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -232,16 +232,16 @@
     def display_image(self, image_file, figure=None):
         try:
             if figure is None:
                 figure = self.default_figure
             figure.clear()
             img = mpimg.imread(image_file)
             ax = figure.subplots()
-            ax.axis('off')
             ax.imshow(img)
+            ax.axis('off')
             figure.canvas.draw_idle()
         except Exception as e:
             logger.error(f"Error in display_image: {e}")
 
     def get_terminal(self):
         return self.dock_dict[self.DefaultTerminalName].widget()
```

### Comparing `srsgui-0.3.2/srsgui/ui/inputpanel.py` & `srsgui-0.3.3/srsgui/ui/inputpanel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/qt/QtCore.py` & `srsgui-0.3.3/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/qt/QtGui.py` & `srsgui-0.3.3/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.3.3/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/qt/__init__.py` & `srsgui-0.3.3/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/qtloghandler.py` & `srsgui-0.3.3/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/resource_rc.py` & `srsgui-0.3.3/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/signalhandler.py` & `srsgui-0.3.3/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/srslogo.jpg` & `srsgui-0.3.3/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/stdout.py` & `srsgui-0.3.3/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/taskmain.py` & `srsgui-0.3.3/srsgui/ui/taskmain.py`

 * *Files 0% similar despite different names*

```diff
@@ -606,15 +606,15 @@
         except Exception as e:
             logger.error(f"Error in handle_initial_image: {e}")
 
     def onAbout(self,checked):
         msg = ''
         for name in self.inst_dict:
             inst = self.inst_dict[name]
-            if hasattr(inst, __version__):
+            if hasattr(inst, "__version__"):
                 version = inst.__version__
             else:
                 version = 'N/A'
 
             msg += '{} version: {}\n'.format(inst.__class__.__name__, version)
         msg += '\nSrsgui version: {}\n'.format(__version__)
         msg += '\n{} version: {}\n'.format(QT_BINDER, QT_BINDER_VERSION)
```

### Comparing `srsgui-0.3.2/srsgui/ui/taskmain.ui` & `srsgui-0.3.3/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui/ui/ui_taskmain.py` & `srsgui-0.3.3/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.2/srsgui.egg-info/PKG-INFO` & `srsgui-0.3.3/srsgui.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.3.2
+Version: 0.3.3
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
@@ -20,19 +20,19 @@
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 # ``Srsgui`` - Organize instrument-controlling Python scripts as a GUI application
 
-`Srsgui` is a simple platform:
+`Srsgui` is a simple framework:
 
    - To define instrument classes for instruments that use remote communication,
      based on `Instrument` class and the communication `Interface` class 
-     (By default, serial, TCPIP is available, extendable to VXI11, GPIB and USB-TMC).
+     (By default, serial and TCPIP is available. VXI11, GPIB and USB-TMC are optional.).
 
    - To write Python scripts (tasks) that run in GUI environment with simple APIs
      provided in ``Task`` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
      using a configuration (.taskconfig) file for a project
 
@@ -41,58 +41,56 @@
 ## Installation
 
 To run ``srsgui`` as an application, create a virtual environment, if necessary, 
 and install using ``pip`` with [full] option:  
 
     python -m pip install srsgui[full]
 
-if it fails, you have to install 
+``Srsgui`` package has the following 3 main dependencies: 
 [pyserial](https://pypi.org/project/pyserial/), 
-[matplotlib](https://pypi.org/project/matplotlib/) and 
-a Python Qt binder ([PySide6](https://pypi.org/project/PySide6/),
-[PySide2](https://pypi.org/project/PySide2/) or 
-[PyQt5](https://pypi.org/project/PyQt5/)) manually.
-``srsgui`` package has these 3 dependencies only.
-
-Some Linux distributions offer some of the Python packages from their 
-repositories only, not from ``pip``. Run web search for more information on 
-system specific installation.   
-
-When matplotlib and one of the Qt binders
-are installed properly, install ``srsgui`` without [full] option:
+[matplotlib](https://pypi.org/project/matplotlib/) and
+[PySide6](https://pypi.org/project/PySide6/). If the installation above fails, 
+you have to install the failed pacakge manually. Using a virtual environment will
+eliminate possible conflicts between packages in the main Python installation and 
+the packagesSome used in `srsgui`. Some Linux distributions offer 
+some of the Python packages from their repositories only, not from ``pip``. 
+Run web search for more information on system-specific installation.   
+
+Once pyserial, matplotlib and PySide6 are installed properly, or you plan to use
+`srsgui` for instrument drivers only without GUI support, 
+you can install ``srsgui`` without [full] option:
 
     python -m pip install srsgui
 
 ## Start ``srsgui`` application
     
 if the Python Script directory is in PATH environment variable,
 Start the application by typing from the command line:
 
     srsgui
-    
 
-If the script directory is not in PATH,
+If the script directory is not in PATH, run the srsgui module with Python. 
 
     python -m srsgui
     
 It will start `srsgui` application.
 
 ## Run the example project
 
 By default, `srsgui` application starts with the last project it ran,
 when it is closed.
  
 To open the example project included in the `srsgui` package 
-(if it does not start with the example project), go to the `srsgui` package 
-directory, find the examples directory, and find a .taskconfig file in an 
-example project folder. 
+(if `srsgui` does not start with the example project), select the menu/File/Open config, 
+go to the `srsgui` package directory, find the examples directory, and find a .taskconfig file
+in the example project folder. 
 
 You can run the second and fifth task in the Task menu 
 even without any instruments connected.
 
 ## Create a project
 
-`Srsgui` is a platform that helps you to write your own instrument-controlling 
+`Srsgui` is a framework to helps you to write your own instrument-controlling 
 Python scripts running as a GUI application. Using its APIs, you can write 
 scripts running in GUI with the same amount of code with writing console-based 
 scripts. For programming API, refer to
 [`srsgui` documentation](https://thinksrs.github.io/srsgui).
```

### Comparing `srsgui-0.3.2/srsgui.egg-info/SOURCES.txt` & `srsgui-0.3.3/srsgui.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 readme.md
 requirements.txt
 setup.py
 .github/workflows/pages.yml
 docs/Makefile
+docs/application.rst
 docs/changelog.rst
 docs/conf.py
 docs/create-project.rst
 docs/create-task.rst
 docs/define-instrument.rst
 docs/example.rst
 docs/index.rst
@@ -24,19 +25,23 @@
 docs/srsgui.ui.commandtree.rst
 docs/srsgui.ui.qt.rst
 docs/srsgui.ui.rst
 docs/troubleshooting.rst
 docs/_static/cg-dir-terminal-screen-capture.png
 docs/_static/cg-terminal-screen-capture.png
 docs/_static/connect-dialog-box-capture.png
+docs/_static/dock_widget_floating.png
+docs/_static/dock_widgets_expanded.png
 docs/_static/example-screen-capture-1.png
 docs/_static/example-screen-capture-2.png
 docs/_static/initial-screen-capture.png
+docs/_static/lockin-capture.png
 docs/_static/osc-dir-terminal-screen-capture.png
 docs/_static/second-task-screen-capture.png
+docs/_static/task_selection.png
 docs/_static/terminal-with-example-2.png
 docs/_static/terminal-with-example.png
 srsgui/__init__.py
 srsgui/__main__.py
 srsgui.egg-info/PKG-INFO
 srsgui.egg-info/SOURCES.txt
 srsgui.egg-info/dependency_links.txt
```

