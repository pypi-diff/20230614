# Comparing `tmp/InfixToPostfix-1.0.4.tar.gz` & `tmp/InfixToPostfix-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InfixToPostfix-1.0.4.tar", last modified: Tue Jun 13 16:10:17 2023, max compression
+gzip compressed data, was "InfixToPostfix-1.0.7.tar", last modified: Wed Jun 14 03:31:25 2023, max compression
```

## Comparing `InfixToPostfix-1.0.4.tar` & `InfixToPostfix-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 16:10:17.280691 InfixToPostfix-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-06-13 16:10:17.274660 InfixToPostfix-1.0.4/InfixToPostfix/
--rw-rw-rw-   0        0        0        0 2023-06-12 05:01:03.000000 InfixToPostfix-1.0.4/InfixToPostfix/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:10:17.279676 InfixToPostfix-1.0.4/InfixToPostfix/data/
--rw-rw-rw-   0        0        0       50 2023-06-11 04:58:52.000000 InfixToPostfix-1.0.4/InfixToPostfix/data/conf
--rw-rw-rw-   0        0        0      832 2023-06-12 02:48:48.000000 InfixToPostfix-1.0.4/InfixToPostfix/data/style.qss
--rw-rw-rw-   0        0        0     7462 2023-06-13 16:09:07.000000 InfixToPostfix-1.0.4/InfixToPostfix/infix_to_postfix.py
--rw-rw-rw-   0        0        0     3835 2023-06-13 16:08:57.000000 InfixToPostfix-1.0.4/InfixToPostfix/ui.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:10:17.277670 InfixToPostfix-1.0.4/InfixToPostfix.egg-info/
--rw-rw-rw-   0        0        0     1130 2023-06-13 16:10:17.000000 InfixToPostfix-1.0.4/InfixToPostfix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-06-13 16:10:17.000000 InfixToPostfix-1.0.4/InfixToPostfix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 16:10:17.000000 InfixToPostfix-1.0.4/InfixToPostfix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-13 16:10:17.000000 InfixToPostfix-1.0.4/InfixToPostfix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35148 2023-06-13 15:13:02.000000 InfixToPostfix-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       71 2023-06-13 16:03:26.000000 InfixToPostfix-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1130 2023-06-13 16:10:17.280691 InfixToPostfix-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      780 2023-06-13 15:37:48.000000 InfixToPostfix-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 16:10:17.280691 InfixToPostfix-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-13 16:09:22.000000 InfixToPostfix-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:31:25.341860 InfixToPostfix-1.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:31:25.341860 InfixToPostfix-1.0.7/InfixToPostfix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:31:15.000000 InfixToPostfix-1.0.7/InfixToPostfix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:31:25.341860 InfixToPostfix-1.0.7/InfixToPostfix/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 03:31:15.000000 InfixToPostfix-1.0.7/InfixToPostfix/data/conf
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-14 03:31:15.000000 InfixToPostfix-1.0.7/InfixToPostfix/data/style.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-06-14 03:31:15.000000 InfixToPostfix-1.0.7/InfixToPostfix/infix_to_postfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-14 03:31:15.000000 InfixToPostfix-1.0.7/InfixToPostfix/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:31:25.341860 InfixToPostfix-1.0.7/InfixToPostfix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-14 03:31:25.000000 InfixToPostfix-1.0.7/InfixToPostfix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-14 03:31:25.000000 InfixToPostfix-1.0.7/InfixToPostfix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:31:25.000000 InfixToPostfix-1.0.7/InfixToPostfix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 03:31:25.000000 InfixToPostfix-1.0.7/InfixToPostfix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 03:31:25.000000 InfixToPostfix-1.0.7/InfixToPostfix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-14 03:31:15.000000 InfixToPostfix-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 03:31:15.000000 InfixToPostfix-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-14 03:31:25.341860 InfixToPostfix-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-14 03:31:15.000000 InfixToPostfix-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 03:31:25.345860 InfixToPostfix-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-14 03:31:15.000000 InfixToPostfix-1.0.7/setup.py
```

### Comparing `InfixToPostfix-1.0.4/InfixToPostfix/ui.py` & `InfixToPostfix-1.0.7/InfixToPostfix/ui.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import os
-
-from PyQt6 import QtWidgets, QtCore
-from PyQt6.QtWidgets import QWidget, QGridLayout, QPushButton, QLineEdit, QFileDialog, QLabel, QTableWidget
-
-from InfixToPostfix.infix_to_postfix import InfixToPostfix
-
-
-class MainWindow(QWidget):
-    STYLE_QSS_PATH = os.path.join(os.path.dirname(__file__), "data/style.qss")
-
-    def __init__(self):
-        super().__init__()
-        self.setWindowTitle("后缀表达式生成器")
-        self.setStyleSheet(open(MainWindow.STYLE_QSS_PATH).read())
-        self.resize(1280, 720)
-        self.conf = ""
-        self.file_chooser = QPushButton("选取配置文件")
-        self.file_chooser.setSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.expression = QLineEdit()
-        self.expression.setPlaceholderText("输入表达式")
-        self.expression.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
-        self.expression.setSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.data_process = QPushButton("提交")
-        self.data_process.setSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.child_window = QWidget()
-        self.child_window.setStyleSheet(open(MainWindow.STYLE_QSS_PATH).read())
-        self.child_window.setWindowTitle("分析结果")
-        self.child_window.resize(1280, 720)
-        self.init_layout()
-        self.show()
-
-    def init_layout(self):
-        def file_chooser_connect():
-            self.conf = QFileDialog().getOpenFileName(self, "选取配置文件", "./", "All Files (*)")[0]
-            self.file_chooser.setText(self.conf)
-
-        def data_process_connect():
-            data = InfixToPostfix() if self.conf == "" else InfixToPostfix(self.conf)
-            words, actions, states, result = data.analyze(self.expression.text())
-
-            child_layout = QGridLayout()
-
-            analyze_result = QTableWidget(len(actions), 2)
-            analyze_result.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
-            analyze_result.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
-            analyze_result.setEditTriggers(QtWidgets.QAbstractItemView.EditTrigger.NoEditTriggers)
-            for i, action, state in zip(range(len(actions)), actions, states):
-                item_0 = QtWidgets.QTableWidgetItem(action)
-                item_1 = QtWidgets.QTableWidgetItem(state)
-                item_0.setTextAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
-                item_1.setTextAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
-                analyze_result.setItem(i, 0, item_0)
-                analyze_result.setItem(i, 1, item_1)
-            analyze_result.setColumnWidth(0, 605)
-            analyze_result.setColumnWidth(1, 605)
-
-            raw = QLabel(f"中缀表达式   {' '.join([word[1] for word in words])}")
-            raw.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
-
-            result = QLabel(f"后缀表达式   {' '.join(result)}")
-            result.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
-
-            child_layout.addWidget(analyze_result, 0, 0, 3, 2)
-            child_layout.addWidget(raw, 3, 0, 1, 1)
-            child_layout.addWidget(result, 3, 1, 1, 1)
-
-            self.child_window.setLayout(child_layout)
-            self.child_window.show()
-
-        grid = QGridLayout()
-
-        self.file_chooser.clicked.connect(file_chooser_connect)
-        self.data_process.clicked.connect(data_process_connect)
-
-        grid.addWidget(self.file_chooser, 0, 0, 2, 1)
-        grid.addWidget(self.expression, 0, 1, 1, 1)
-        grid.addWidget(self.data_process, 1, 1, 1, 1)
-
-        self.setLayout(grid)
+import os
+
+from PyQt6 import QtWidgets, QtCore
+from PyQt6.QtWidgets import QWidget, QGridLayout, QPushButton, QLineEdit, QFileDialog, QLabel, QTableWidget
+
+from InfixToPostfix.infix_to_postfix import InfixToPostfix
+
+
+class MainWindow(QWidget):
+    STYLE_QSS_PATH = os.path.join(os.path.dirname(__file__), "data/style.qss")
+
+    def __init__(self):
+        super().__init__()
+        self.setWindowTitle("后缀表达式生成器")
+        self.setStyleSheet(open(MainWindow.STYLE_QSS_PATH).read())
+        self.resize(1280, 720)
+        self.conf = ""
+        self.file_chooser = QPushButton("选取配置文件")
+        self.file_chooser.setSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.expression = QLineEdit()
+        self.expression.setPlaceholderText("输入表达式")
+        self.expression.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.expression.setSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.data_process = QPushButton("提交")
+        self.data_process.setSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.child_window = QWidget()
+        self.child_window.setStyleSheet(open(MainWindow.STYLE_QSS_PATH).read())
+        self.child_window.setWindowTitle("分析结果")
+        self.child_window.resize(1280, 720)
+        self.init_layout()
+        self.show()
+
+    def init_layout(self):
+        def file_chooser_connect():
+            self.conf = QFileDialog().getOpenFileName(self, "选取配置文件", "./", "All Files (*)")[0]
+            self.file_chooser.setText(self.conf)
+
+        def data_process_connect():
+            data = InfixToPostfix() if self.conf == "" else InfixToPostfix(self.conf)
+            words, actions, states, result = data.analyze(self.expression.text())
+
+            child_layout = QGridLayout()
+
+            analyze_result = QTableWidget(len(actions), 2)
+            analyze_result.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
+            analyze_result.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
+            analyze_result.setEditTriggers(QtWidgets.QAbstractItemView.EditTrigger.NoEditTriggers)
+            for i, action, state in zip(range(len(actions)), actions, states):
+                item_0 = QtWidgets.QTableWidgetItem(action)
+                item_1 = QtWidgets.QTableWidgetItem(state)
+                item_0.setTextAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+                item_1.setTextAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+                analyze_result.setItem(i, 0, item_0)
+                analyze_result.setItem(i, 1, item_1)
+            analyze_result.setColumnWidth(0, 605)
+            analyze_result.setColumnWidth(1, 605)
+
+            raw = QLabel(f"中缀表达式   {' '.join([word[1] for word in words])}")
+            raw.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+
+            result = QLabel(f"后缀表达式   {' '.join(result)}")
+            result.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+
+            child_layout.addWidget(analyze_result, 0, 0, 3, 2)
+            child_layout.addWidget(raw, 3, 0, 1, 1)
+            child_layout.addWidget(result, 3, 1, 1, 1)
+
+            self.child_window.setLayout(child_layout)
+            self.child_window.show()
+
+        grid = QGridLayout()
+
+        self.file_chooser.clicked.connect(file_chooser_connect)
+        self.data_process.clicked.connect(data_process_connect)
+
+        grid.addWidget(self.file_chooser, 0, 0, 2, 1)
+        grid.addWidget(self.expression, 0, 1, 1, 1)
+        grid.addWidget(self.data_process, 1, 1, 1, 1)
+
+        self.setLayout(grid)
```

### Comparing `InfixToPostfix-1.0.4/LICENSE` & `InfixToPostfix-1.0.7/LICENSE`

 * *Files identical despite different names*

