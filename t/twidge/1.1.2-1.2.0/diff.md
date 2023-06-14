# Comparing `tmp/twidge-1.1.2.tar.gz` & `tmp/twidge-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twidge-1.1.2.tar", max compression
+gzip compressed data, was "twidge-1.2.0.tar", max compression
```

## Comparing `twidge-1.1.2.tar` & `twidge-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1074 2022-08-12 02:08:32.474197 twidge-1.1.2/LICENSE
--rw-r--r--   0        0        0      753 2022-10-17 05:04:57.804049 twidge-1.1.2/README.md
--rw-r--r--   0        0        0      563 2023-01-20 05:44:36.303990 twidge-1.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-12 01:26:48.218522 twidge-1.1.2/twidge/__init__.py
--rw-r--r--   0        0        0      808 2023-01-20 05:28:26.843078 twidge-1.1.2/twidge/__main__.py
--rw-r--r--   0        0        0     5197 2023-01-20 05:28:26.843078 twidge-1.1.2/twidge/core.py
--rw-r--r--   0        0        0     2940 2023-01-20 05:28:26.843078 twidge-1.1.2/twidge/terminal.py
--rw-r--r--   0        0        0      266 2023-01-20 05:28:26.843078 twidge-1.1.2/twidge/widgets/__init__.py
--rw-r--r--   0        0        0    10391 2023-01-20 05:28:26.843078 twidge-1.1.2/twidge/widgets/base.py
--rw-r--r--   0        0        0     8503 2023-01-20 05:28:26.843078 twidge-1.1.2/twidge/widgets/editors.py
--rw-r--r--   0        0        0     1074 2023-01-20 05:28:26.843078 twidge-1.1.2/twidge/widgets/form.py
--rw-r--r--   0        0        0     1585 2023-01-20 05:46:08.791402 twidge-1.1.2/setup.py
--rw-r--r--   0        0        0     1249 2023-01-20 05:46:08.791650 twidge-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-08-12 02:08:32.474197 twidge-1.2.0/LICENSE
+-rw-r--r--   0        0        0      753 2022-10-17 05:04:57.804049 twidge-1.2.0/README.md
+-rw-r--r--   0        0        0      569 2023-06-13 23:47:57.238378 twidge-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-08-12 01:26:48.218522 twidge-1.2.0/twidge/__init__.py
+-rw-r--r--   0        0        0     1194 2023-06-13 23:03:21.695436 twidge-1.2.0/twidge/__main__.py
+-rw-r--r--   0        0        0     5735 2023-06-13 23:40:50.583409 twidge-1.2.0/twidge/core.py
+-rw-r--r--   0        0        0     2939 2023-06-13 23:03:21.695436 twidge-1.2.0/twidge/terminal.py
+-rw-r--r--   0        0        0      137 2023-06-13 23:03:21.698769 twidge-1.2.0/twidge/widgets/__init__.py
+-rw-r--r--   0        0        0     8528 2023-06-13 23:40:50.673410 twidge-1.2.0/twidge/widgets/editors.py
+-rw-r--r--   0        0        0     4311 2023-06-13 23:03:21.698769 twidge-1.2.0/twidge/widgets/filters.py
+-rw-r--r--   0        0        0     1099 2023-06-13 23:03:21.698769 twidge-1.2.0/twidge/widgets/form.py
+-rw-r--r--   0        0        0     4832 2023-06-13 23:03:21.698769 twidge-1.2.0/twidge/widgets/inline.py
+-rw-r--r--   0        0        0     3590 2023-06-13 23:40:50.556743 twidge-1.2.0/twidge/widgets/simple.py
+-rw-r--r--   0        0        0     3797 2023-06-13 23:03:21.698769 twidge-1.2.0/twidge/widgets/templater.py
+-rw-r--r--   0        0        0     6641 2023-06-13 23:03:21.698769 twidge-1.2.0/twidge/widgets/wrappers.py
+-rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 twidge-1.2.0/PKG-INFO
```

### Comparing `twidge-1.1.2/LICENSE` & `twidge-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twidge-1.1.2/README.md` & `twidge-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `twidge-1.1.2/pyproject.toml` & `twidge-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "twidge"
-version = "1.1.2"
+version = "1.2.0"
 description = "Terminal Widgets."
 authors = ["Aidan Courtney <aidanfc97@gmail.com>"]
 repository = 'https://github.com/aidaco/twidge'
 readme = 'README.md'
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-rich = "^13.2.0"
-typer = "^0.7.0"
-
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-black = "^22.6.0"
-mypy = "^0.950"
-isort = "^5.10.1"
-flake8 = "^5.0.4"
+rich = "^13.4.2"
+typer = "^0.9.0"
 
 [tool.poetry.scripts]
 twidge = 'twidge.__main__:cli'
 
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+pytest = "^7.1.2"
+mypy = "^1.3.0"
+isort = "^5.12.0"
+flake8 = "^6.0.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `twidge-1.1.2/twidge/__main__.py` & `twidge-1.2.0/twidge/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,69 @@
+from pathlib import Path
+
 import typer
 
 from .widgets import (
-    Closeable,
+    Close,
     Echo,
+    EchoBytes,
     EditString,
+    EditTemplate,
     Form,
     Framed,
     Indexer,
     Searcher,
     Selector,
 )
 
 cli = typer.Typer()
 
 
 @cli.command()
 def echo():
-    Closeable(Framed(Echo())).run()
+    Echo().run()
+
+
+@cli.command()
+def echobytes():
+    EchoBytes().run()
 
 
 @cli.command()
 def edit(content: str = typer.Argument("")):
-    print(Closeable(Framed(EditString(content))).run())
+    print(Close(Framed(EditString(content))).run())
+
+
+@cli.command()
+def template(
+    content: str = typer.Argument(""),
+    path: Path = typer.Option(None),
+    escape: bool = False,
+):
+    content = content or path.read_text()
+    if escape:
+        content = content.encode("utf-8").decode("unicode_escape")
+    print(Close(Framed(EditTemplate(content))).run())
 
 
 @cli.command()
 def form(labels: str):
-    print(Closeable(Framed(Form(labels.split(",")))).run())
+    print(Close(Framed(Form(labels.split(",")))).run())
 
 
 @cli.command()
 def filter(options: str):
-    print(Closeable(Framed(Searcher(options.split(",")))).run())
+    print(Close(Framed(Searcher(options.split(",")))).run())
 
 
 @cli.command()
 def index(options: str):
-    print(Closeable(Framed(Indexer(options.split(",")))).run())
+    print(Close(Framed(Indexer(options.split(",")))).run())
 
 
 @cli.command()
 def select(options: str):
-    print(Closeable(Framed(Selector(options.split(",")))).run())
+    print(Close(Framed(Selector(options.split(",")))).run())
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `twidge-1.1.2/twidge/core.py` & `twidge-1.2.0/twidge/widgets/inline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,215 +1,173 @@
-import sys
-from inspect import signature
-from typing import (
-    BinaryIO,
-    Callable,
-    Iterable,
-    Protocol,
-    Type,
-    TypeAlias,
-    runtime_checkable,
-)
+from rich.style import Style
+from rich.text import Text
 
-from rich.console import Console, ConsoleOptions, RenderableType
-from rich.live import Live
+from twidge.core import DispatchBuilder, Event, RunBuilder, StrEvent
+from twidge.widgets.editors import _fullview, _scrollview
 
-from twidge.terminal import chbreak, keystr
 
-
-class EventBase:
-    ...
-
-
-Event: TypeAlias = EventBase | str | bytes
-
-
-@runtime_checkable
-class SingleHandler(Protocol):
-    def __call__(self) -> None:
-        pass
-
-
-@runtime_checkable
-class MultiHandler(Protocol):
-    def __call__(self, event: Event) -> None:
-        pass
-
-
-class RichWidget(Protocol):
-    def __rich__(self) -> RenderableType:
-        ...
-
-    def dispatch(self, event: Event) -> None:
-        ...
-
-
-class ConsoleWidget(Protocol):
-    def __rich_console__(
-        self, console: Console, console_options: ConsoleOptions
-    ) -> Iterable[RenderableType]:
-        ...
-
-    def dispatch(self, event: Event) -> None:
-        ...
-
-
-Handler: TypeAlias = SingleHandler | MultiHandler
-Widget: TypeAlias = RichWidget | ConsoleWidget
-
-
-class Reader(Protocol):
-    def __init__(self, io: BinaryIO):
-        ...
-
-    def read(self) -> Event:
-        ...
-
-
-class BytesReader:
-    def __init__(self, io: BinaryIO):
-        self.io = io
-
-    def read(self) -> bytes:
-        return self.io.read(6)
-
-
-class StrReader:
-    def __init__(self, io: BinaryIO):
-        self.io = io
-        self.reader = BytesReader(io)
-
-    def read(self) -> str:
-        return keystr(self.reader.read())
-
-
-class Runner:
-    def __init__(
-        self,
-        widget: Widget,
-        stdin: int | None = None,
-        reader: Type[Reader] = StrReader,
-        console: Console | None = None,
-    ):
-        self.widget = widget
-        self.stdin = stdin if stdin is not None else sys.stdin.fileno()
-        self.reader = reader
-        self.console = (
-            console
-            if console is not None
-            else Console(highlight=False, markup=False, emoji=False)
+class InlineEditor:
+    run = RunBuilder()
+    dispatch = DispatchBuilder()
+
+    def __init__(self, text: str = "", scroll: bool = True):
+        self.text = text
+        self.cursor = 0
+        self.focus = True
+        self.scroll = scroll
+
+    @property
+    def result(self) -> str:
+        return self.text
+
+    def __rich_console__(self, console, options):
+        width = options.size.width
+
+        if self.scroll:
+            if 0 <= self.cursor < len(self.text):
+                sstr, cstr, estr = _scrollview(self.text, self.cursor, width)
+            else:
+                sstr, cstr, estr = (
+                    self.text[max(0, self.cursor - (width - 1)) : self.cursor],
+                    " ",
+                    "",
+                )
+        else:
+            if 0 <= self.cursor < len(self.text):
+                sstr, cstr, estr = _fullview(self.text, self.cursor, width)
+            else:
+                sstr, cstr, estr = self.text, " ", ""
+
+        yield (
+            Text(sstr, style=Style(color="bright_yellow", bold=True), end="")
+            + Text(
+                cstr, style=Style(color="grey30", bgcolor="grey70", bold=True), end=""
+            )
+            + Text(estr, style=Style(color="bright_yellow", bold=True), end="")
+            if self.focus
+            else Text(sstr, end="") + Text(cstr, end="") + Text(estr, end="")
         )
 
-        self.running = False
-
-    def run(self):
-        self.running = True
-        with chbreak(stdin=self.stdin), Live(
-            self.widget,
-            console=self.console,
-            transient=True,
-            auto_refresh=False,
-        ) as live:
-            refresh = live.refresh
-            read = self.reader(open(self.stdin, "rb", buffering=0, closefd=False)).read
-            dispatch = self.widget.dispatch
-            while self.running:
-                dispatch(read())
-                refresh()
-        return getattr(self.widget, "result", None)
+    @dispatch.on("left")
+    def cursor_left(self):
+        if self.cursor != 0:
+            self.cursor -= 1
+
+    @dispatch.on("right")
+    def cursor_right(self):
+        if self.cursor < len(self.text):
+            self.cursor += 1
+
+    @dispatch.on("ctrl+right")
+    def next_word(self):
+        next_space = self.text[self.cursor :].find(" ")
+        if next_space == -1:
+            self.cursor = len(self.text)
+        else:
+            self.cursor = self.cursor + next_space + 1
+
+    @dispatch.on("ctrl+left")
+    def prev_word(self):
+        prev_space = self.text[max(0, self.cursor - 2) :: -1].find(" ")
+        if prev_space < 0:
+            self.cursor = 0
+        else:
+            self.cursor = self.cursor - prev_space - 1
+
+    @dispatch.on("home")
+    def cursor_home(self):
+        self.cursor = 0
+
+    @dispatch.on("end")
+    def cursor_end(self):
+        self.cursor = len(self.text)
+
+    @dispatch.on("backspace")
+    def backspace(self):
+        if self.cursor != 0:
+            self.text = self.text[: self.cursor - 1] + self.text[self.cursor :]
+            self.cursor -= 1
+
+    @dispatch.on("ctrl+h")
+    def delete_word(self):
+        prev_space = self.text[: self.cursor - 1][::-1].find(" ")
+        if prev_space == -1:
+            n = 0
+        else:
+            n = self.cursor - prev_space - 2
+        self.text = self.text[:n] + self.text[self.cursor :]
+        self.cursor = n
+
+    @dispatch.on("focus")
+    def on_focus(self):
+        self.focus = True
+
+    @dispatch.on("blur")
+    def on_blur(self):
+        self.focus = False
+
+    @dispatch.default
+    def insert(self, char: str):
+        char = "\t" if char == "tab" else char
+        char = " " if char == "space" else char
+
+        if len(char) > 1:
+            return
+        if self.cursor == len(self.text):
+            self.text += char
+        else:
+            self.text = self.text[: self.cursor] + char + self.text[self.cursor :]
+        self.cursor += len(char)
+
+
+class InlineCycler:
+    dispatch = DispatchBuilder()
+    run = RunBuilder()
 
-    def stop(self):
-        self.running = False
-
-    __call__ = run
-
-
-class Dispatcher:
     def __init__(
         self,
-        table: dict[Event, Handler] | None = None,
-        default: Handler | None = None,
-    ):
-        self.table = table if table is not None else {}
-        self.default = default
-
-    def dispatch(self, event: Event) -> None:
-        fn = self.table.get(event, self.default)
-        if fn is None:
-            raise ValueError(f"No handler for {event!r}")
-        match len(signature(fn).parameters):
-            case 0:
-                fn()
-            case 1:
-                fn(event)
-            case _:
-                raise TypeError("Handler should take one or zero arguments.")
-
-    def update(
-        self, table: dict[Event, Handler] | None = None, default: Handler | None = None
+        *options: str,
+        key=str,
+        focus_style: str | Style = Style.parse("bright_yellow on magenta"),
+        blur_style: str | Style = Style.parse("white on black"),
     ):
-        if table:
-            self.table.update(table)
-        if default:
-            self._default = default
+        self.options = options
+        self.key = key
+        self.len = len(self.options)
+        self.index = 0
+        self.focus = True
+        self.focus_style = focus_style
+        self.blur_style = blur_style
+
+    @dispatch.on(StrEvent("focus"))
+    def on_focus(self):
+        self.focus = True
+
+    @dispatch.on(StrEvent("blur"))
+    def on_blur(self):
+        self.focus = False
+
+    @dispatch.on("space", "right")
+    def forward(self):
+        self.index = (self.index + 1) % self.len
+
+    @dispatch.on("left")
+    def back(self):
+        self.index = (self.index - 1) % self.len
 
-    __call__ = dispatch
-
-
-class RunBuilder:
-    def __init__(
-        self,
-        stdin: int | None = None,
-        reader: Type[Reader] = StrReader,
-        console: Console | None = None,
-    ):
-        self.stdin = stdin
-        self.reader = reader
-        self.console = console
-
-    def build(self, widget):
-        return Runner(widget, self.stdin, self.reader, self.console)
-
-    def __get__(self, obj, obj_type=None):
-        if obj is None:
-            return self
-        obj.run = self.build(obj)
-        return obj.run
+    @dispatch.default
+    def drop_events(self, event: Event):
+        pass
 
+    def __rich__(self):
+        opt = self.key(self.options[self.index])
+        if self.focus:
+            return Text(f"←{opt}→", style="bright_yellow", end="")
+        else:
+            return Text(opt, end="")
+
+    @property
+    def result(self):
+        return self.options[self.index]
 
-class DispatchBuilder:
-    def __init__(
-        self,
-        methods: dict[Event, str] | None = None,
-        table: dict[Event, Handler] | None = None,
-        defaultfn: Handler | str | None = None,
-    ):
-        self.methods = methods if methods is not None else {}
-        self.table = table if table is not None else {}
-        self.defaultfn = defaultfn if defaultfn is not None else {}
-
-    def on(self, *events: Event):
-        def decorate(fn: Callable):
-            for e in events:
-                self.methods[e] = fn.__name__
-            return fn
-
-        return decorate
-
-    def default(self, fn: Callable):
-        self.defaultfn = fn.__name__
-        return fn
-
-    def build(self, widget):
-        table = self.table | {e: getattr(widget, m) for e, m in self.methods.items()}
-        default = (
-            getattr(widget, self.defaultfn)
-            if isinstance(self.defaultfn, str)
-            else self.defaultfn
-        )
-        return Dispatcher(table=table, default=default)
 
-    def __get__(self, obj, obj_type=None):
-        if obj is None:
-            return self
-        obj.dispatch = self.build(obj)
-        return obj.dispatch
+__all__ = ["InlineEditor", "InlineCycler"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `twidge-1.1.2/twidge/terminal.py` & `twidge-1.2.0/twidge/terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,11 +109,10 @@
         termios.tcsetattr(fd, termios.TCSAFLUSH, mode)
         # End of modified tty.setraw
 
         # Non-blocking io; disabled b/c tricky.
         # os.set_blocking(fd, False)
         yield
     finally:
-
         # Resume blocking io, see above.
         # os.set_blocking(fd, True)
         termios.tcsetattr(fd, termios.TCSADRAIN, old)
```

### Comparing `twidge-1.1.2/twidge/widgets/editors.py` & `twidge-1.2.0/twidge/widgets/editors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import typing
 from functools import partial
 from math import ceil, floor
 
 from rich.style import Style
 from rich.styled import Styled
 from rich.text import Text
@@ -94,28 +95,26 @@
         if self.multiline and self.cursor[0] < len(self.lines) - 1:
             self.cursor[0] += 1
             self.cursor[1] = min(self.cursor[1], len(self.lines[self.cursor[0]]))
 
     @dispatch.on("ctrl+right")
     def next_word(self):
         line = self.lines[self.cursor[0]]
-        next_space = line[self.cursor[1] :].find(" ")
-        if next_space == -1:
-            self.cursor[1] = len(line)
-        else:
-            self.cursor[1] = self.cursor[1] + next_space + 1
+        sec = line[self.cursor[1] + 1 :]
+        m = re.search(r"\W|$", sec)
+        next_non_word = m.end()
+        self.cursor[1] = self.cursor[1] + next_non_word + 1
 
     @dispatch.on("ctrl+left")
     def prev_word(self):
         line = self.lines[self.cursor[0]]
-        prev_space = line[max(0, self.cursor[1] - 2) :: -1].find(" ")
-        if prev_space < 0:
-            self.cursor[1] = 0
-        else:
-            self.cursor[1] = self.cursor[1] - prev_space - 1
+        sec = line[: self.cursor[1]][::-1]
+        m = re.search(r"\W\w|$", sec)
+        prev_non_word = m.end()
+        self.cursor[1] = self.cursor[1] - prev_non_word
 
     @dispatch.on("home")
     def cursor_home(self):
         self.cursor[1] = 0
 
     @dispatch.on("end")
     def cursor_end(self):
@@ -137,19 +136,20 @@
                 )
                 self.cursor[1] = length
                 del self.lines[self.cursor[0]]
                 self.cursor[0] -= 1
 
     @dispatch.on("ctrl+h")
     def delete_word(self):
-        prev_space = self.lines[self.cursor[0]][: self.cursor[1] - 1][::-1].find(" ")
-        if prev_space == -1:
-            n = 0
-        else:
-            n = self.cursor[1] - prev_space - 2
+        line = self.lines[self.cursor[0]]
+        sec = line[: self.cursor[1]][::-1]
+        m = re.search(r"(?>.)\b|$", sec)
+        print(sec, self.cursor, m)
+        prev_non_word = m.end()
+        n = self.cursor[1] - prev_non_word
         self.lines[self.cursor[0]] = (
             self.lines[self.cursor[0]][:n]
             + self.lines[self.cursor[0]][self.cursor[1] :]
         )
         self.cursor[1] = n
 
     @dispatch.on("enter")
@@ -270,8 +270,14 @@
             return complex(text)
 
 
 EditIntString = partial(ParsedEditString, parser=int)
 EditFloatString = partial(ParsedEditString, parser=float)
 EditComplexString = partial(ParsedEditString, parser=complex)
 EditNumericString = partial(ParsedEditString, parser=parse_numeric)
-EditEnumString = lambda enum_cls: ParsedEditString(parser=enum_cls)
+
+
+def EditEnumString(enum_cls):
+    return ParsedEditString(parser=enum_cls)
+
+
+__all__ = ["EditString"]
```

### Comparing `twidge-1.1.2/twidge/widgets/form.py` & `twidge-1.2.0/twidge/widgets/form.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from rich.table import Table
 from rich.text import Text
 
 from twidge.core import DispatchBuilder, RunBuilder
-from twidge.widgets.base import FocusManager
 from twidge.widgets.editors import EditString
+from twidge.widgets.wrappers import FocusManager
 
 
 class Form:
     run = RunBuilder()
     dispatch = DispatchBuilder()
 
     def __init__(self, labels: list[str]):
@@ -35,7 +35,10 @@
     @dispatch.on("shift+tab")
     def focus_back(self):
         self.fm.back()
 
     @dispatch.default
     def passthrough(self, event):
         self.fm.focused.dispatch(event)
+
+
+__all__ = ["Form"]
```

### Comparing `twidge-1.1.2/PKG-INFO` & `twidge-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: twidge
-Version: 1.1.2
+Version: 1.2.0
 Summary: Terminal Widgets.
 Home-page: https://github.com/aidaco/twidge
 License: MIT
 Author: Aidan Courtney
 Author-email: aidanfc97@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: rich (>=13.2.0,<14.0.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/aidaco/twidge
 Description-Content-Type: text/markdown
 
 
 # Twidge
 
 Simple terminal widgets for simple people.
```

