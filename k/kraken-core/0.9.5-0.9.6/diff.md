# Comparing `tmp/kraken-core-0.9.5.tar.gz` & `tmp/kraken-core-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken-core-0.9.5.tar", max compression
+gzip compressed data, was "kraken-core-0.9.6.tar", max compression
```

## Comparing `kraken-core-0.9.5.tar` & `kraken-core-0.9.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      988 2022-06-24 18:32:01.277510 kraken-core-0.9.5/LICENSE
--rw-r--r--   0        0        0     2004 2022-08-30 17:19:09.644210 kraken-core-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     1266 2022-08-17 09:36:21.488490 kraken-core-0.9.5/readme.md
--rw-r--r--   0        0        0      851 2022-08-30 17:19:09.645063 kraken-core-0.9.5/src/kraken/core/__init__.py
--rw-r--r--   0        0        0     2277 2022-08-17 09:34:34.033780 kraken-core-0.9.5/src/kraken/core/base.py
--rw-r--r--   0        0        0       23 2022-08-13 11:23:12.516931 kraken-core-0.9.5/src/kraken/core/cli/__init__.py
--rw-r--r--   0        0        0     2342 2022-08-17 09:49:20.249002 kraken-core-0.9.5/src/kraken/core/cli/executor.py
--rw-r--r--   0        0        0    13718 2022-08-23 16:56:39.604050 kraken-core-0.9.5/src/kraken/core/cli/main.py
--rw-r--r--   0        0        0     6190 2022-08-23 16:57:15.990176 kraken-core-0.9.5/src/kraken/core/cli/option_sets.py
--rw-r--r--   0        0        0     1503 2022-08-17 09:34:34.033867 kraken-core-0.9.5/src/kraken/core/cli/serialize.py
--rw-r--r--   0        0        0     9523 2022-08-12 14:02:08.888219 kraken-core-0.9.5/src/kraken/core/context.py
--rw-r--r--   0        0        0     2007 2022-08-12 14:02:08.888985 kraken-core-0.9.5/src/kraken/core/executor/__init__.py
--rw-r--r--   0        0        0     2323 2022-08-17 09:49:20.275317 kraken-core-0.9.5/src/kraken/core/executor/colored.py
--rw-r--r--   0        0        0     7014 2022-08-12 14:02:08.889792 kraken-core-0.9.5/src/kraken/core/executor/default.py
--rw-r--r--   0        0        0     1547 2022-08-12 14:02:08.890236 kraken-core-0.9.5/src/kraken/core/executor/utils.py
--rw-r--r--   0        0        0    13346 2022-08-23 16:55:31.700168 kraken-core-0.9.5/src/kraken/core/graph.py
--rw-r--r--   0        0        0       23 2022-08-13 11:23:12.517408 kraken-core-0.9.5/src/kraken/core/lib/__init__.py
--rw-r--r--   0        0        0     1806 2022-08-17 09:49:20.252411 kraken-core-0.9.5/src/kraken/core/lib/check_file_contents_task.py
--rw-r--r--   0        0        0     3736 2022-08-30 17:16:28.736336 kraken-core-0.9.5/src/kraken/core/lib/render_file_task.py
--rw-r--r--   0        0        0     1472 2022-08-13 11:12:41.258277 kraken-core-0.9.5/src/kraken/core/loader.py
--rw-r--r--   0        0        0     7074 2022-08-17 09:34:34.036038 kraken-core-0.9.5/src/kraken/core/project.py
--rw-r--r--   0        0        0    13202 2022-08-30 17:16:20.334357 kraken-core-0.9.5/src/kraken/core/property.py
--rw-r--r--   0        0        0        0 2022-08-12 14:02:08.892028 kraken-core-0.9.5/src/kraken/core/py.typed
--rw-r--r--   0        0        0     5560 2022-08-17 09:34:34.033808 kraken-core-0.9.5/src/kraken/core/supplier.py
--rw-r--r--   0        0        0    17431 2022-08-12 14:02:08.892666 kraken-core-0.9.5/src/kraken/core/task.py
--rw-r--r--   0        0        0     1241 2022-08-13 11:23:12.517516 kraken-core-0.9.5/src/kraken/core/test/__init__.py
--rw-r--r--   0        0        0       23 2022-08-13 11:23:12.517613 kraken-core-0.9.5/src/kraken/core/util/__init__.py
--rw-r--r--   0        0        0      453 2022-08-12 14:02:08.896847 kraken-core-0.9.5/src/kraken/core/util/argparse.py
--rw-r--r--   0        0        0     1369 2022-08-17 09:49:05.603086 kraken-core-0.9.5/src/kraken/core/util/asciitable.py
--rw-r--r--   0        0        0     2935 2022-08-12 14:02:08.897896 kraken-core-0.9.5/src/kraken/core/util/fs.py
--rw-r--r--   0        0        0      382 2022-08-12 14:02:08.898271 kraken-core-0.9.5/src/kraken/core/util/helpers.py
--rw-r--r--   0        0        0     1041 2022-08-12 14:02:08.898627 kraken-core-0.9.5/src/kraken/core/util/importing.py
--rw-r--r--   0        0        0      252 2022-08-12 14:02:08.899032 kraken-core-0.9.5/src/kraken/core/util/json.py
--rw-r--r--   0        0        0      868 2022-08-12 14:02:08.899420 kraken-core-0.9.5/src/kraken/core/util/krakenw.py
--rw-r--r--   0        0        0      661 2022-08-12 14:02:08.899900 kraken-core-0.9.5/src/kraken/core/util/path.py
--rw-r--r--   0        0        0     8358 2022-08-17 15:35:28.373760 kraken-core-0.9.5/src/kraken/core/util/requirements.py
--rw-r--r--   0        0        0      484 2022-08-12 14:02:08.900955 kraken-core-0.9.5/src/kraken/core/util/term.py
--rw-r--r--   0        0        0     1192 2022-08-12 14:02:08.901279 kraken-core-0.9.5/src/kraken/core/util/text.py
--rw-r--r--   0        0        0     2476 2022-08-30 17:19:19.096168 kraken-core-0.9.5/setup.py
--rw-r--r--   0        0        0     2215 2022-08-30 17:19:19.096353 kraken-core-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0      988 2022-06-24 18:32:01.277510 kraken-core-0.9.6/LICENSE
+-rw-r--r--   0        0        0     2004 2022-08-30 23:24:39.125532 kraken-core-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     1266 2022-08-17 09:36:21.488490 kraken-core-0.9.6/readme.md
+-rw-r--r--   0        0        0      851 2022-08-30 23:24:39.133760 kraken-core-0.9.6/src/kraken/core/__init__.py
+-rw-r--r--   0        0        0     2277 2022-08-17 09:34:34.033780 kraken-core-0.9.6/src/kraken/core/base.py
+-rw-r--r--   0        0        0       23 2022-08-13 11:23:12.516931 kraken-core-0.9.6/src/kraken/core/cli/__init__.py
+-rw-r--r--   0        0        0     2342 2022-08-17 09:49:20.249002 kraken-core-0.9.6/src/kraken/core/cli/executor.py
+-rw-r--r--   0        0        0    14020 2022-08-30 23:24:33.526581 kraken-core-0.9.6/src/kraken/core/cli/main.py
+-rw-r--r--   0        0        0     6344 2022-08-30 23:24:33.527457 kraken-core-0.9.6/src/kraken/core/cli/option_sets.py
+-rw-r--r--   0        0        0     1495 2022-08-30 23:24:33.528112 kraken-core-0.9.6/src/kraken/core/cli/serialize.py
+-rw-r--r--   0        0        0     9502 2022-08-30 23:24:33.528713 kraken-core-0.9.6/src/kraken/core/context.py
+-rw-r--r--   0        0        0     2121 2022-08-30 23:24:33.529224 kraken-core-0.9.6/src/kraken/core/executor/__init__.py
+-rw-r--r--   0        0        0     2323 2022-08-17 09:49:20.275317 kraken-core-0.9.6/src/kraken/core/executor/colored.py
+-rw-r--r--   0        0        0     7237 2022-08-30 23:24:33.529864 kraken-core-0.9.6/src/kraken/core/executor/default.py
+-rw-r--r--   0        0        0     1547 2022-08-12 14:02:08.890236 kraken-core-0.9.6/src/kraken/core/executor/utils.py
+-rw-r--r--   0        0        0    13992 2022-08-30 23:24:33.530767 kraken-core-0.9.6/src/kraken/core/graph.py
+-rw-r--r--   0        0        0       23 2022-08-13 11:23:12.517408 kraken-core-0.9.6/src/kraken/core/lib/__init__.py
+-rw-r--r--   0        0        0     1806 2022-08-17 09:49:20.252411 kraken-core-0.9.6/src/kraken/core/lib/check_file_contents_task.py
+-rw-r--r--   0        0        0     3736 2022-08-30 17:16:28.736336 kraken-core-0.9.6/src/kraken/core/lib/render_file_task.py
+-rw-r--r--   0        0        0     1472 2022-08-13 11:12:41.258277 kraken-core-0.9.6/src/kraken/core/loader.py
+-rw-r--r--   0        0        0     7074 2022-08-17 09:34:34.036038 kraken-core-0.9.6/src/kraken/core/project.py
+-rw-r--r--   0        0        0    13202 2022-08-30 17:16:20.334357 kraken-core-0.9.6/src/kraken/core/property.py
+-rw-r--r--   0        0        0        0 2022-08-12 14:02:08.892028 kraken-core-0.9.6/src/kraken/core/py.typed
+-rw-r--r--   0        0        0     5560 2022-08-17 09:34:34.033808 kraken-core-0.9.6/src/kraken/core/supplier.py
+-rw-r--r--   0        0        0    17431 2022-08-12 14:02:08.892666 kraken-core-0.9.6/src/kraken/core/task.py
+-rw-r--r--   0        0        0     1241 2022-08-13 11:23:12.517516 kraken-core-0.9.6/src/kraken/core/test/__init__.py
+-rw-r--r--   0        0        0       23 2022-08-13 11:23:12.517613 kraken-core-0.9.6/src/kraken/core/util/__init__.py
+-rw-r--r--   0        0        0      453 2022-08-12 14:02:08.896847 kraken-core-0.9.6/src/kraken/core/util/argparse.py
+-rw-r--r--   0        0        0     1369 2022-08-17 09:49:05.603086 kraken-core-0.9.6/src/kraken/core/util/asciitable.py
+-rw-r--r--   0        0        0     2935 2022-08-12 14:02:08.897896 kraken-core-0.9.6/src/kraken/core/util/fs.py
+-rw-r--r--   0        0        0      382 2022-08-12 14:02:08.898271 kraken-core-0.9.6/src/kraken/core/util/helpers.py
+-rw-r--r--   0        0        0     1041 2022-08-12 14:02:08.898627 kraken-core-0.9.6/src/kraken/core/util/importing.py
+-rw-r--r--   0        0        0      252 2022-08-12 14:02:08.899032 kraken-core-0.9.6/src/kraken/core/util/json.py
+-rw-r--r--   0        0        0      868 2022-08-12 14:02:08.899420 kraken-core-0.9.6/src/kraken/core/util/krakenw.py
+-rw-r--r--   0        0        0      661 2022-08-12 14:02:08.899900 kraken-core-0.9.6/src/kraken/core/util/path.py
+-rw-r--r--   0        0        0     8358 2022-08-17 15:35:28.373760 kraken-core-0.9.6/src/kraken/core/util/requirements.py
+-rw-r--r--   0        0        0      484 2022-08-12 14:02:08.900955 kraken-core-0.9.6/src/kraken/core/util/term.py
+-rw-r--r--   0        0        0     1192 2022-08-12 14:02:08.901279 kraken-core-0.9.6/src/kraken/core/util/text.py
+-rw-r--r--   0        0        0     2476 2022-08-30 23:24:49.990586 kraken-core-0.9.6/setup.py
+-rw-r--r--   0        0        0     2215 2022-08-30 23:24:49.990836 kraken-core-0.9.6/PKG-INFO
```

### Comparing `kraken-core-0.9.5/LICENSE` & `kraken-core-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/pyproject.toml` & `kraken-core-0.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 classifiers = []
 description = ""
 keywords = []
 license = "MIT"
 name = "kraken-core"
 packages = [{include = "kraken/core", from = "src"}]
 readme = "readme.md"
-version = "0.9.5"
+version = "0.9.6"
 
 [tool.poetry.urls]
 # "Bug Tracker" = ""
 # Documentation = ""
 # Homepage = ""
 # Repository = ""
```

### Comparing `kraken-core-0.9.5/readme.md` & `kraken-core-0.9.6/readme.md`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/__init__.py` & `kraken-core-0.9.6/src/kraken/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.5"
+__version__ = "0.9.6"
 
 from kraken.core.context import BuildError, Context
 from kraken.core.executor import Graph, GraphExecutor, GraphExecutorObserver
 from kraken.core.graph import TaskGraph
 from kraken.core.loader import ProjectLoader, ProjectLoaderError
 from kraken.core.project import Project
 from kraken.core.property import Property
```

### Comparing `kraken-core-0.9.5/src/kraken/core/base.py` & `kraken-core-0.9.6/src/kraken/core/base.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/cli/executor.py` & `kraken-core-0.9.6/src/kraken/core/cli/executor.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/cli/main.py` & `kraken-core-0.9.6/src/kraken/core/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,27 +102,33 @@
 
     context: Context | None = None
     if graph_options.resume:
         context, graph = serialize.load_build_state(build_options.state_dir)
         if not graph:
             raise ValueError("cannot --resume without build state")
         if graph and graph_options.restart:
-            graph.discard_statuses()
+            graph.restart()
 
     if context is None:
         context = Context(build_options.build_dir)
         context.load_project(build_options.project_dir)
         context.finalize()
         graph = TaskGraph(context)
 
     assert graph is not None
     if not graph_options.no_save:
         exit_stack.callback(lambda: serialize.save_build_state(build_options.state_dir, not_none(graph)))
 
-    graph.set_targets(context.resolve_tasks(graph_options.tasks or None))
+    graph.root.results_from(graph)
+
+    if graph_options.all:
+        graph = graph.root
+    else:
+        graph = graph.root.trim(context.resolve_tasks(graph_options.tasks or None))
+
     return context, graph
 
 
 def run(
     exit_stack: contextlib.ExitStack,
     build_options: BuildOptions,
     graph_options: GraphOptions,
@@ -168,73 +174,76 @@
 
     from termcolor import colored
 
     from kraken.core import GroupTask
     from kraken.core.cli.executor import status_to_text
     from kraken.core.util.term import get_terminal_width
 
-    required_tasks = set(graph.tasks(targets_only=True))
-    longest_name = max(map(len, (t.path for t in graph.tasks(all=True)))) + 1
+    goal_tasks = set(graph.tasks(goals=True))
+    longest_name = max(map(len, (t.path for t in graph.tasks()))) + 1
 
     print()
     print(colored("Tasks", "blue", attrs=["bold", "underline"]))
     print()
 
     width = get_terminal_width(120)
 
     def _print_task(task: Task) -> None:
         line = [task.path.ljust(longest_name)]
         remaining_width = width - len(line[0])
-        if task in required_tasks:
+        if task in goal_tasks:
             line[0] = colored(line[0], "green")
         if task.default:
             line[0] = colored(line[0], attrs=["bold"])
         status = graph.get_status(task)
         if status is not None:
             line.append(f"[{status_to_text(status)}]")
-            remaining_width -= 2 + len(status_to_text(status, colored=False)) + 1
+            status_length = 2 + len(status_to_text(status, colored=False)) + 1
+            remaining_width -= status_length
         description = task.get_description()
         if description:
             remaining_width -= 2
+            if remaining_width <= 0:
+                remaining_width = width
             for part in textwrap.wrap(
                 description,
                 remaining_width,
                 subsequent_indent=(width - remaining_width) * " ",
             ):
                 line.append(part)
                 line.append("\n")
             line.pop()
         print("  " + " ".join(line))
 
     def sort_key(task: Task) -> str:
         return task.path
 
-    for task in sorted(graph.tasks(all=True), key=sort_key):
+    for task in sorted(graph.tasks(), key=sort_key):
         if isinstance(task, GroupTask):
             continue
         _print_task(task)
 
     print()
     print(colored("Groups", "blue", attrs=["bold", "underline"]))
     print()
 
-    for task in sorted(graph.tasks(all=True), key=sort_key):
+    for task in sorted(graph.tasks(), key=sort_key):
         if not isinstance(task, GroupTask):
             continue
         _print_task(task)
 
     print()
 
 
 def describe(graph: TaskGraph) -> None:
     from termcolor import colored
 
     from kraken.core import GroupTask
 
-    tasks = list(graph.tasks(targets_only=True))
+    tasks = list(graph.tasks(goals=True))
     print("selected", len(tasks), "task(s)")
     print()
 
     for task in tasks:
         print("Group" if isinstance(task, GroupTask) else "Task", colored(task.path, attrs=["bold", "underline"]))
         print("  Type:", type(task).__module__ + "." + type(task).__name__)
         print("  Type defined in:", colored(sys.modules[type(task).__module__].__file__ or "???", "cyan"))
@@ -264,56 +273,59 @@
     import io
 
     from nr.io.graphviz.render import render_to_browser
     from nr.io.graphviz.writer import GraphvizWriter
 
     from kraken.core import GroupTask
 
+    root = graph.root
     if viz_options.reduce or viz_options.reduce_keep_explicit:
-        graph.reduce(keep_explicit=viz_options.reduce_keep_explicit)
+        root = root.reduce(keep_explicit=viz_options.reduce_keep_explicit)
+        graph = graph.reduce(keep_explicit=viz_options.reduce_keep_explicit)
 
     buffer = io.StringIO()
     writer = GraphvizWriter(buffer if viz_options.show else sys.stdout)
     writer.digraph(fontname="monospace", rankdir="LR")
     writer.set_node_style(style="filled", shape="box")
 
     style_default = {"penwidth": "3"}
     style_goal = {"fillcolor": "lawngreen"}
     style_select = {"fillcolor": "darkgoldenrod1"}
     style_group = {"shape": "ellipse"}
     style_edge_non_strict = {"style": "dashed"}
     style_edge_implicit = {"color": "gray"}
 
     writer.subgraph("cluster_#legend", label="Legend")
-    writer.node("#task", label="task")
+    # writer.node("#task", label="task")
     writer.node("#group", label="group task", **style_group)
-    writer.node("#default", label="would run by default", **style_default)
-    writer.node("#selected", label="will run", **style_select)
+    writer.node("#default", label="runs by default", **style_default)
+    writer.node("#selected", label="task will run", **style_select)
     writer.node("#goal", label="goal task", **style_goal)
     writer.end()
 
     writer.subgraph("cluster_#build", label="Build Graph")
 
-    goal_tasks = set(graph.tasks(targets_only=True))
+    main = root if viz_options.inactive else graph
+    goal_tasks = set(graph.tasks(goals=True))
     selected_tasks = set(graph.tasks())
 
-    for task in graph.tasks(all=viz_options.all):
+    for task in main.tasks():
         style = {}
         style.update(style_default if task.default else {})
         style.update(style_group if isinstance(task, GroupTask) else {})
         style.update(style_select if task in selected_tasks else {})
         style.update(style_goal if task in goal_tasks else {})
 
         writer.node(task.path, **style)
-        for predecessor in graph.get_predecessors(task, ignore_groups=False):
+        for predecessor in main.get_predecessors(task, ignore_groups=False):
             writer.edge(
                 predecessor.path,
                 task.path,
-                **({} if graph.get_edge(predecessor, task).strict else style_edge_non_strict),
-                **(style_edge_implicit if graph.get_edge(predecessor, task).implicit else {}),
+                **({} if main.get_edge(predecessor, task).strict else style_edge_non_strict),
+                **(style_edge_implicit if main.get_edge(predecessor, task).implicit else {}),
             )
 
     writer.end()
     writer.end()
 
     if viz_options.show:
         render_to_browser(buffer.getvalue())
```

### Comparing `kraken-core-0.9.5/src/kraken/core/cli/option_sets.py` & `kraken-core-0.9.6/src/kraken/core/cli/option_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,18 +115,20 @@
 
 @dataclasses.dataclass(frozen=True)
 class GraphOptions:
     tasks: list[str]
     resume: bool
     restart: bool
     no_save: bool
+    all: bool
 
     @staticmethod
     def add_to_parser(parser: argparse.ArgumentParser, saveable: bool = True) -> None:
         parser.add_argument("tasks", metavar="task", nargs="*", help="one or more tasks to execute")
+        parser.add_argument("-a", "--all", action="store_true", help="select all tasks")
         parser.add_argument("--resume", action="store_true", help="load previous build state")
         parser.add_argument(
             "--restart",
             choices=("all",),
             help="load previous build state, but discard existing results (requires --resume)",
         )
         if saveable:
@@ -135,14 +137,15 @@
     @classmethod
     def collect(cls, args: argparse.Namespace) -> GraphOptions:
         return cls(
             tasks=args.tasks,
             resume=args.resume,
             restart=args.restart,
             no_save=getattr(args, "no_save", True),
+            all=args.all,
         )
 
 
 @dataclasses.dataclass(frozen=True)
 class RunOptions:
     allow_no_tasks: bool
     skip_build: bool
@@ -170,32 +173,32 @@
             exclude_tasks=args.exclude,
             exclude_tasks_subgraph=args.exclude_subgraph,
         )
 
 
 @dataclasses.dataclass(frozen=True)
 class VizOptions:
-    all: bool
+    inactive: bool
     show: bool
     reduce: bool
     reduce_keep_explicit: bool
 
     @staticmethod
     def add_to_parser(parser: argparse.ArgumentParser) -> None:
-        parser.add_argument("-a", "--all", action="store_true", help="include all tasks in the graph")
+        parser.add_argument("-i", "--inactive", action="store_true", help="include inactive tasks in the graph")
         parser.add_argument("-s", "--show", action="store_true", help="show the graph in the browser (requires dot)")
         parser.add_argument("-R", "--reduce", action="store_true", help="fully transitively reduce the graph")
         parser.add_argument(
             "-r",
             "--reduce-keep-explicit",
             action="store_true",
             help="transitively reduce the graph but keep explicit edges",
         )
 
     @classmethod
     def collect(cls, args: argparse.Namespace) -> VizOptions:
         return cls(
-            all=args.all,
+            inactive=args.inactive,
             show=args.show,
             reduce=args.reduce,
             reduce_keep_explicit=args.reduce_keep_explicit,
         )
```

### Comparing `kraken-core-0.9.5/src/kraken/core/cli/serialize.py` & `kraken-core-0.9.6/src/kraken/core/cli/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     graph: TaskGraph | None = None
     for state_file in sorted(state_files):
         with state_file.open("rb") as fp:
             new_graph: TaskGraph = dill.load(fp)
         if context is None or graph is None:
             context, graph = new_graph.context, new_graph
         else:
-            graph.update_statuses_from(new_graph)
+            graph.results_from(new_graph)
     assert context is not None and graph is not None
     return context, graph
 
 
 def save_build_state(state_dir: Path, graph: TaskGraph) -> None:
     state_file = state_dir / f"state-{str(uuid.uuid4())[:7]}.dill"
     state_dir.mkdir(parents=True, exist_ok=True)
```

### Comparing `kraken-core-0.9.5/src/kraken/core/context.py` & `kraken-core-0.9.6/src/kraken/core/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,16 +190,15 @@
             tasks = self.resolve_tasks([t for t in targets if isinstance(t, str)]) + [
                 t for t in targets if not isinstance(t, str)
             ]
 
         if not tasks:
             raise ValueError("no tasks selected")
 
-        graph = TaskGraph(self)
-        graph.set_targets(tasks)
+        graph = TaskGraph(self).trim(tasks)
 
         assert graph, "TaskGraph cannot be empty"
         return graph
 
     def execute(self, tasks: list[str | Task] | TaskGraph | None = None) -> None:
         """Execute all default tasks or the tasks specified by *targets* using the default executor.
         If :meth:`finalize` was not called already it will be called by this function before the build
```

### Comparing `kraken-core-0.9.5/src/kraken/core/executor/__init__.py` & `kraken-core-0.9.6/src/kraken/core/executor/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,18 @@
         but :meth:`is_complete` returns `False`, the build was unsuccessful."""
 
     @abc.abstractmethod
     def get_successors(self, task: Task) -> list[Task]:
         """Return all active dependants of the given task."""
 
     @abc.abstractmethod
+    def get_task(self, task_path: str) -> Task:
+        """Return a task by its path."""
+
+    @abc.abstractmethod
     def set_status(self, task: Task, status: TaskStatus) -> None:
         """Set the result of a task. Can be called twice for the same task unless the previous call was passing
         a status with type :attr:`TaskStatusType.STARTED`."""
 
     @abc.abstractmethod
     def is_complete(self) -> bool:
         """Return `True` if all tasks in the graph are done and successful."""
```

### Comparing `kraken-core-0.9.5/src/kraken/core/executor/colored.py` & `kraken-core-0.9.6/src/kraken/core/executor/colored.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/executor/default.py` & `kraken-core-0.9.6/src/kraken/core/executor/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 import traceback
 from functools import partial
 from typing import Callable, Iterable
 
 from kraken.core.executor import Graph, GraphExecutor, GraphExecutorObserver
 from kraken.core.executor.utils import TaskRememberer
-from kraken.core.task import Task, TaskStatus
+from kraken.core.task import GroupTask, Task, TaskStatus
 
 
 class TaskExecutor(abc.ABC):
     @abc.abstractmethod
     def execute_task(self, task: Task, done: Callable[[TaskStatus], None]) -> None:
         ...
 
@@ -138,14 +138,17 @@
         print(flush=True)
 
     def after_execute_graph(self, graph: Graph) -> None:
         print(flush=True)
         print(self.format_header("Build summary"), flush=True)
         print(flush=True)
         for task_path, status in self._status.items():
+            task = graph.get_task(task_path)
+            if isinstance(task, GroupTask) and status.is_skipped():
+                continue
             print(
                 " " * (len(self.execute_prefix) + 1) + task_path,
                 self.status_to_text(status),
                 self.format_duration(f"[{self._duration[task_path]:.3f}s]") if task_path in self._duration else "",
             )
         print(flush=True)
 
@@ -161,15 +164,16 @@
             self._started[task.path] = time.perf_counter()
 
     def on_task_output(self, task: Task, chunk: bytes) -> None:
         sys.stdout.buffer.write(chunk)
         sys.stdout.flush()
 
     def after_execute_task(self, task: Task, status: TaskStatus) -> None:
-        print(self.execute_prefix, task.path, self.status_to_text(status), flush=True)
+        if not (isinstance(task, GroupTask) and status.is_skipped()):
+            print(self.execute_prefix, task.path, self.status_to_text(status), flush=True)
         with self._lock:
             self._status[task.path] = status
             if task.path in self._started:
                 self._duration[task.path] = time.perf_counter() - self._started[task.path]
 
     def before_teardown_task(self, task: Task) -> None:
         print(self.teardown_prefix, task.path, flush=True)
```

### Comparing `kraken-core-0.9.5/src/kraken/core/executor/utils.py` & `kraken-core-0.9.6/src/kraken/core/executor/utils.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/graph.py` & `kraken-core-0.9.6/src/kraken/core/graph.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import dataclasses
 import logging
-from typing import Iterable, Iterator, List, cast
+from typing import Iterable, Iterator, List, Sequence, cast
 
 from networkx import DiGraph, restricted_view, transitive_reduction
 
 from kraken.core.context import Context
 from kraken.core.executor import Graph
 from kraken.core.task import GroupTask, Task, TaskStatus
 from kraken.core.util.helpers import not_none
@@ -17,253 +17,276 @@
 @dataclasses.dataclass
 class _Edge:
     strict: bool
     implicit: bool
 
 
 class TaskGraph(Graph):
-    """The task graph represents the entirety of a Kraken context's tasks as a directed acyclic graph data structure.
+    """The task graph represents a Kraken context's tasks as a directed acyclic graph data structure.
 
-    Internally, it stores three versions of the graph: A full graph, a target subgraph and a ready subgraph. The
-    subgraphs are implemented as views on the full graph.
+    Before a task graph is passed to an executor, it is usually trimmed to contain only the tasks that are
+    needed for the successful and complete execution of the desired set of "goal tasks"."""
 
-    1. The **full graph** stores the entire build graph of all tasks in the context.
-    2. The **target graph** stores only the relevant subgraph with the target tasks as leaf nodes set with
-       :meth:`set_targets`.
-    3. The **ready graph** excludes all successfully completed tasks from the target graph. This is used to find
-       the next set of ready tasks with :meth:`ready`. This graph is not kept in memory but created automatically
-       when needed.
-    """
+    def __init__(self, context: Context, populate: bool = True, parent: TaskGraph | None = None) -> None:
+        """Create a new build graph from the given task list.
 
-    def __init__(self, context: Context) -> None:
-        """Create a new build graph from the given task list."""
+        :param context: The context that the graph belongs to.
+        :param populate: If enabled, the task graph will be immediately populated with the tasks in the context.
+            The graph can also be later populated with the :meth:`populate` method.
+        """
 
+        self._parent = parent
         self._context = context
 
         # Nodes have the form {'data': _Node} and edges have the form {'data': _Edge}.
-        self._full_graph = DiGraph()
+        self._digraph = DiGraph()
 
         # Keep track of task execution results.
         self._results: dict[str, TaskStatus] = {}
 
+        # All tasks that have a successful status are stored here.
+        self._completed_tasks: set[str] = set()
+
         # Keep track of the tasks that returned TaskStatus.STARTED. That means the task is a background task, and
         # if the TaskGraph is deserialized from a state file to continue the build, background tasks need to be
         # reset so they start again if another task requires them.
         self._background_tasks: set[str] = set()
 
-        # Here we store all tasks that make up the "initial set", i.e. the ultimate target tasks that are to be
-        # executed. We derive the subgraph to execute from this initial set in the :meth:`trim` method by deactivating
-        # tasks in :attr:`_inactive_nodes`.
-        self._target_tasks: set[str] = set()
-
-        # All deactivated tasks are stored here.
-        self._inactive_tasks: set[str] = set()
-
-        # All tasks that have a successful status are stored here.
-        self._completed_tasks: set[str] = set()
-
-        # Make sure the build graph is populated with the entire build graph.
-        for project in context.iter_projects():
-            for task in project.tasks().values():
-                if task.path not in self._full_graph.nodes:
-                    self._add_task(task)
-
-        # The restricted view is the subgraph that excludes all inactive tasks.
-        self._target_graph: DiGraph
-
-        self._update_target_graph()
+        if populate:
+            self.populate()
 
     def __bool__(self) -> bool:
-        return len(self._target_graph.nodes) > 0
+        return len(self._digraph.nodes) > 0
 
     def __len__(self) -> int:
-        return len(self._target_graph.nodes)
+        return len(self._digraph.nodes)
 
     # Low level internal API
 
     def _get_task(self, task_path: str) -> Task | None:
-        data = self._full_graph.nodes.get(task_path)
+        data = self._digraph.nodes.get(task_path)
         if data is None:
             return None
         return cast(Task, data["data"])
 
     def _add_task(self, task: Task) -> None:
-        self._full_graph.add_node(task.path, data=task)
+        self._digraph.add_node(task.path, data=task)
         for rel in task.get_relationships():
-            if rel.other_task.path not in self._full_graph.nodes:
+            if rel.other_task.path not in self._digraph.nodes:
                 self._add_task(rel.other_task)
             a, b = (task, rel.other_task) if rel.inverse else (rel.other_task, task)
             self._add_edge(a.path, b.path, rel.strict, False)
 
             # When a group depends on another group, we implicitly create make each member of the downstream group
             # depend on the upstream group.
             if isinstance(task, GroupTask) and isinstance(rel.other_task, GroupTask):
                 upstream, downstream = (task, rel.other_task) if rel.inverse else (rel.other_task, task)
                 for member in downstream.tasks:
                     self._add_edge(upstream.path, member.path, rel.strict, True)
 
     def _get_edge(self, task_a: str, task_b: str) -> _Edge | None:
-        data = self._full_graph.edges.get((task_a, task_b))
+        data = self._digraph.edges.get((task_a, task_b)) or self._digraph.edges.get((task_a, task_b))
         if data is None:
             return None
         return cast(_Edge, data["data"])
 
-    def _add_edge(self, task_a: str, task_b: str, strict: bool, implicit: bool) -> None:
+    def _add_edge(self, task_a: str, task_b: str, strict: bool, implicit: bool, graph: DiGraph | None = None) -> None:
+        graph = graph or self._digraph
         edge = self._get_edge(task_a, task_b) or _Edge(strict, implicit)
         edge.strict = edge.strict or strict
         edge.implicit = edge.implicit and implicit
-        self._full_graph.add_edge(task_a, task_b, data=edge)
+        graph.add_edge(task_a, task_b, data=edge)
 
     # High level internal API
 
-    def _update_inactive_tasks(self) -> None:
-        """Internal. Updates the inactive tasks that are not required to be executed for the target tasks."""
+    def _get_required_tasks(self, goals: Iterable[Task]) -> set[str]:
+        """Internal. Return the set of tasks that are required transitively from the goal tasks."""
 
         def _recurse_task(task_path: str, visited: set[str]) -> None:
             visited.add(task_path)
-            for pred in self._full_graph.predecessors(task_path):
+            for pred in self._digraph.predecessors(task_path):
                 if not_none(self._get_edge(pred, task_path)).strict:
                     _recurse_task(pred, visited)
 
         active_tasks: set[str] = set()
-        for task_path in self._target_tasks:
-            _recurse_task(task_path, active_tasks)
+        for task in goals:
+            _recurse_task(task.path, active_tasks)
 
-        self._inactive_tasks = set(self._full_graph.nodes) - active_tasks
-        self._update_target_graph()
+        return active_tasks
 
-    def _update_target_graph(self) -> None:
-        """Updates the target graph."""
-        self._target_graph = restricted_view(self._full_graph, self._inactive_tasks, set())
+    def _remove_nodes_keep_transitive_edges(self, nodes: Iterable[str]) -> None:
+        """Internal. Remove nodes from the graph, but ensure that transitive dependencies are kept in tact."""
+
+        for task_path in nodes:
+            for in_task_path in self._digraph.predecessors(task_path):
+                in_edge = not_none(self._get_edge(in_task_path, task_path))
+                for out_task_path in self._digraph.successors(task_path):
+                    out_edge = not_none(self._get_edge(task_path, out_task_path))
+                    self._add_edge(
+                        in_task_path,
+                        out_task_path,
+                        strict=in_edge.strict or out_edge.strict,
+                        implicit=in_edge.implicit and out_edge.implicit,
+                    )
+            self._digraph.remove_node(task_path)
 
     def _get_ready_graph(self) -> DiGraph:
         """Updates the ready graph."""
-        return restricted_view(self._target_graph, self._completed_tasks, set())
-
-    def reduce(self, keep_explicit: bool = False) -> None:
-        """Transitively reduce the graph.
-
-        :param keep_explicit: Keep explicit edges in tact."""
-
-        reduced_graph = transitive_reduction(self._full_graph)
-        reduced_graph.add_nodes_from(self._full_graph.nodes(data=True))
-        reduced_graph.add_edges_from(
-            (u, v, self._full_graph.edges[u, v])
-            for u, v in self._full_graph.edges
-            if (keep_explicit and not self._full_graph.edges[u, v]["data"].implicit) or (u, v) in reduced_graph.edges
-        )
-        self._full_graph = reduced_graph
-        self._update_target_graph()
+        return restricted_view(self._digraph, self._completed_tasks, set())
 
     # Public API
 
     @property
     def context(self) -> Context:
         return self._context
 
+    @property
+    def parent(self) -> TaskGraph | None:
+        return self._parent
+
+    @property
+    def root(self) -> TaskGraph:
+        if self._parent:
+            return self._parent.root
+        return self
+
+    def get_edge(self, pred: Task, succ: Task) -> _Edge:
+        return not_none(self._get_edge(pred.path, succ.path), f"edge does not exist ({pred.path} --> {succ.path})")
+
     def get_predecessors(self, task: Task, ignore_groups: bool = False) -> List[Task]:
         """Returns the predecessors of the task in the original full build graph."""
 
         result = []
-        for task in (not_none(self._get_task(task_path)) for task_path in self._full_graph.predecessors(task.path)):
+        for task in (not_none(self._get_task(task_path)) for task_path in self._digraph.predecessors(task.path)):
             if ignore_groups and isinstance(task, GroupTask):
                 result += task.tasks
             else:
                 result.append(task)
         return result
 
-    def get_edge(self, pred: Task, succ: Task) -> _Edge:
-        return not_none(self._get_edge(pred.path, succ.path), f"edge does not exist ({pred.path} --> {succ.path})")
-
-    def set_targets(self, tasks: Iterable[Task] | None) -> None:
-        """Mark the tasks given with *tasks* as required. All immediate dependencies that are background tasks and
-        have already run will be reset to ensure they run again.
-
-        :param tasks: The leaf targets of the target subgraph. If set to None, the entire task graph will be used."""
-
-        self._target_tasks.clear()
-        if tasks is not None:
-            for task in tasks:
-                self._target_tasks.add(task.path)
-        self._update_inactive_tasks()
-        self._update_target_graph()
-
-        # Reset background tasks.
-        reset_tasks: set[str] = set()
-        for task in self.tasks(pending=True):
-            for pred in self.get_predecessors(task, ignore_groups=True):
-                if pred.path in self._background_tasks:
-                    self._background_tasks.discard(pred.path)
-                    self._completed_tasks.discard(pred.path)
-                    self._results.pop(pred.path, None)
-                    reset_tasks.add(pred.path)
-        if reset_tasks:
-            logger.info("Reset the status of %d background task(s): %s", len(reset_tasks), " ".join(reset_tasks))
-
     def get_status(self, task: Task) -> TaskStatus | None:
         """Return the status of a task."""
 
         return self._results.get(task.path)
 
-    def update_statuses_from(self, other_graph: TaskGraph) -> None:
-        """Merge the results from the *other_graph* into this graph. This is used when multiple separate build states
-        are merged into one graph. If the same task has a result in both graphs, the failed result will supersede the
-        successful one."""
+    def populate(self, goals: Iterable[Task] | None = None) -> None:
+        """Populate the graph with the tasks from the context. This need only be called if the graph was
+        not initially populated in the constructor."""
+
+        if goals is None:
+            for project in self.context.iter_projects():
+                for task in project.tasks().values():
+                    if task.path not in self._digraph.nodes:
+                        self._add_task(task)
+        else:
+            for task in goals:
+                if task.path not in self._digraph.nodes:
+                    self._add_task(task)
+
+    def trim(self, goals: Sequence[Task]) -> TaskGraph:
+        """Returns a copy of the graph that is trimmed to execute only *goals* and their strict dependencies."""
+
+        graph = TaskGraph(self.context, populate=False, parent=self)
+        graph.populate(goals)
+
+        unrequired_tasks = set(graph._digraph.nodes) - graph._get_required_tasks(goals)
+        graph._remove_nodes_keep_transitive_edges(unrequired_tasks)
+
+        return graph
+
+    def reduce(self, keep_explicit: bool = False) -> TaskGraph:
+        """Return a copy of the task graph that has been transitively reduced.
+
+        :param keep_explicit: Keep non-implicit edges in tact."""
+
+        digraph = self._digraph
+        reduced_graph = transitive_reduction(digraph)
+        reduced_graph.add_nodes_from(digraph.nodes(data=True))
+        reduced_graph.add_edges_from(
+            (u, v, digraph.edges[u, v])
+            for u, v in digraph.edges
+            if (keep_explicit and not digraph.edges[u, v]["data"].implicit) or (u, v) in reduced_graph.edges
+        )
+
+        graph = TaskGraph(self.context, populate=False, parent=self)
+        graph._digraph = reduced_graph
+        graph.results_from(self)
+
+        return graph
+
+    def results_from(self, other: TaskGraph) -> None:
+        """Merge the results from the *other* graph into this graph. Only takes the results of tasks that are
+        known to the graph. If the same task has a result in both graphs, and one task result is not successful,
+        the not successful result is preferred."""
 
-        for task in self.tasks(all=True):
+        for task in self.tasks():
             status_a = self._results.get(task.path)
-            status_b = other_graph._results.get(task.path)
+            status_b = other._results.get(task.path)
             if status_a is not None and status_b is not None and status_a.type != status_b.type:
                 resolved_status: TaskStatus | None = status_a if status_a.is_not_ok() else status_b
             else:
                 resolved_status = status_a or status_b
             if resolved_status is not None:
+                # NOTE: This will already take care of updating :attr:`_background_tasks`.
                 self.set_status(task, resolved_status, _force=True)
 
-    def discard_statuses(self) -> None:
-        """Discard any results from the graph, allowing you to effectively restart the execution of tasks."""
+    def resume(self) -> None:
+        """Reset the result of all background tasks that are required by any pending tasks. This needs to be
+        called when a build graph is resumed in a secondary execution to ensure that background tasks are active
+        for the tasks that require them."""
+
+        reset_tasks: set[str] = set()
+        for task in self.tasks(pending=True):
+            for pred in self.get_predecessors(task, ignore_groups=True):
+                if pred.path in self._background_tasks:
+                    self._background_tasks.discard(pred.path)
+                    self._completed_tasks.discard(pred.path)
+                    self._results.pop(pred.path, None)
+                    reset_tasks.add(pred.path)
+
+        if reset_tasks:
+            logger.info("Reset the status of %d background task(s): %s", len(reset_tasks), " ".join(reset_tasks))
+
+    def restart(self) -> None:
+        """Discard the results of all tasks."""
 
-        self._completed_tasks.clear()
         self._results.clear()
-        self._update_target_graph()
+        self._completed_tasks.clear()
+        self._background_tasks.clear()
 
     def tasks(
         self,
-        targets_only: bool = False,
+        goals: bool = False,
         pending: bool = False,
         failed: bool = False,
-        all: bool = False,
     ) -> Iterator[Task]:
-        """Returns the tasks in the graph in arbitrary order. By default, only tasks part of the target subgraph
-        are returned, but this can be changed with *all*.
+        """Returns the tasks in the graph in arbitrary order.
 
-        :param targets_only: Return only target tasks (i.e. the leaf nodes of the target subgraph).
+        :param goals: Return only goal tasks (i.e. leaf nodes).
         :param pending: Return only pending tasks.
         :param failed: Return only failed tasks.
         :param all: Return from all tasks, not just from the tasks that need to be executed."""
 
-        tasks = (not_none(self._get_task(task_path)) for task_path in self._full_graph)
-        if not all:
-            tasks = (task for task in tasks if task.path not in self._inactive_tasks)
-        if targets_only:
-            tasks = (t for t in tasks if t.path in self._target_tasks)
+        tasks = (not_none(self._get_task(task_path)) for task_path in self._digraph)
+        if goals:
+            tasks = (t for t in tasks if self._digraph.out_degree(t.path) == 0)
         if pending:
             tasks = (t for t in tasks if t.path not in self._results)
         if failed:
             tasks = (t for t in tasks if t.path in self._results and self._results[t.path].is_failed())
         return tasks
 
     def execution_order(self, all: bool = False) -> Iterable[Task]:
         """Returns all tasks in the order they need to be executed.
 
         :param all: Return the execution order of all tasks, not just from the target subgraph."""
 
         from networkx.algorithms import topological_sort
 
-        order = topological_sort(self._full_graph if all else self._get_ready_graph())
+        order = topological_sort(self._digraph if all else self._get_ready_graph())
         return (not_none(self._get_task(task_path)) for task_path in order)
 
     # Graph
 
     def ready(self) -> list[Task]:
         """Returns all tasks that are ready to be executed. This can be used to constantly query the graph for new
         available tasks as the status of tasks in the graph is updated with :meth:`set_status`. An empty list is
@@ -278,29 +301,32 @@
 
     def get_successors(self, task: Task, ignore_groups: bool = True) -> list[Task]:
         """Returns the successors of the task in the original full build graph.
 
         Never returns group tasks."""
 
         result = []
-        for task in (not_none(self._get_task(task_path)) for task_path in self._full_graph.successors(task.path)):
+        for task in (not_none(self._get_task(task_path)) for task_path in self._digraph.successors(task.path)):
             if ignore_groups and isinstance(task, GroupTask):
                 result += task.tasks
             else:
                 result.append(task)
         return result
 
+    def get_task(self, task_path: str) -> Task:
+        return not_none(self._get_task(task_path))
+
     def set_status(self, task: Task, status: TaskStatus, *, _force: bool = False) -> None:
         """Sets the status of a task, marking it as executed."""
 
         if not _force and (task.path in self._results and not self._results[task.path].is_started()):
             raise RuntimeError(f"already have a status for task {task.path!r}")
         self._results[task.path] = status
         if status.is_started():
             self._background_tasks.add(task.path)
         if status.is_ok():
             self._completed_tasks.add(task.path)
 
     def is_complete(self) -> bool:
         """Returns `True` if, an only if, all tasks in the target subgraph have a non-failure result."""
 
-        return set(self._target_graph.nodes).issubset(self._completed_tasks)
+        return set(self._digraph.nodes).issubset(self._completed_tasks)
```

### Comparing `kraken-core-0.9.5/src/kraken/core/lib/check_file_contents_task.py` & `kraken-core-0.9.6/src/kraken/core/lib/check_file_contents_task.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/lib/render_file_task.py` & `kraken-core-0.9.6/src/kraken/core/lib/render_file_task.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/loader.py` & `kraken-core-0.9.6/src/kraken/core/loader.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/project.py` & `kraken-core-0.9.6/src/kraken/core/project.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/property.py` & `kraken-core-0.9.6/src/kraken/core/property.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/supplier.py` & `kraken-core-0.9.6/src/kraken/core/supplier.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/task.py` & `kraken-core-0.9.6/src/kraken/core/task.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/test/__init__.py` & `kraken-core-0.9.6/src/kraken/core/test/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/util/asciitable.py` & `kraken-core-0.9.6/src/kraken/core/util/asciitable.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/util/fs.py` & `kraken-core-0.9.6/src/kraken/core/util/fs.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/util/importing.py` & `kraken-core-0.9.6/src/kraken/core/util/importing.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/util/krakenw.py` & `kraken-core-0.9.6/src/kraken/core/util/krakenw.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/util/path.py` & `kraken-core-0.9.6/src/kraken/core/util/path.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/util/requirements.py` & `kraken-core-0.9.6/src/kraken/core/util/requirements.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/src/kraken/core/util/text.py` & `kraken-core-0.9.6/src/kraken/core/util/text.py`

 * *Files identical despite different names*

### Comparing `kraken-core-0.9.5/setup.py` & `kraken-core-0.9.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 entry_points = \
 {'console_scripts': ['kraken = kraken.core.cli.main:main'],
  'pytest11': ['kraken.core.test = kraken.core.test']}
 
 setup_kwargs = {
     'name': 'kraken-core',
-    'version': '0.9.5',
+    'version': '0.9.6',
     'description': '',
     'long_description': "# kraken-core\n\n[![Python application](https://github.com/kraken-build/kraken-core/actions/workflows/python-package.yml/badge.svg)](https://github.com/kraken-build/kraken-core/actions/workflows/python-package.yml)\n[![PyPI version](https://badge.fury.io/py/kraken-core.svg)](https://badge.fury.io/py/kraken-core)\n\n__The Kraken build system.__\n\nKraken focuses on ease of use and simplicity to model complex task orchestration workflows.\n\n__Reproducible build environments__\n\nWe recommend that you use `krakenw` to invoke Kraken builds instead of the `kraken` cli directly to ensure that you\nhave an isolated and reproducible build environment. Install the kraken wrapper cli via the `kraken-wrapper` package\nand define your build requirements at the top of your `.kraken.py` build script:\n\n```\n# ::requirements kraken-std>=0.3.0\nfrom kraken.std.cargo import cargo_build\ncargo_build()\n```\n\n__Vendored packages__\n\nWe're vendoring a number of third party packages for the purpose of reducing the burden of package resolution\nat installation time. This is particularly relevant for using Kraken in continuous integration systems to improve\nresolve times and PEX size.\n\n* `networkx`\n* `nr.io.graphviz`\n* `nr.python.environment`\n* `termcolor`\n* `types-termcolor`\n* `typeapi`\n",
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `kraken-core-0.9.5/PKG-INFO` & `kraken-core-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kraken-core
-Version: 0.9.5
+Version: 0.9.6
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

