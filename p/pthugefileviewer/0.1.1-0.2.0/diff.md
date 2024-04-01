# Comparing `tmp/pthugefileviewer-0.1.1.tar.gz` & `tmp/pthugefileviewer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pthugefileviewer-0.1.1.tar", last modified: Sun Mar 31 16:08:45 2024, max compression
+gzip compressed data, was "pthugefileviewer-0.2.0.tar", last modified: Mon Apr  1 21:02:17 2024, max compression
```

## Comparing `pthugefileviewer-0.1.1.tar` & `pthugefileviewer-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:08:45.992790 pthugefileviewer-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 16:08:36.000000 pthugefileviewer-0.1.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-31 16:08:36.000000 pthugefileviewer-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-03-31 16:08:45.992790 pthugefileviewer-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-31 16:08:36.000000 pthugefileviewer-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:08:45.992790 pthugefileviewer-0.1.1/pthugefileviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-03-31 16:08:45.000000 pthugefileviewer-0.1.1/pthugefileviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-31 16:08:45.000000 pthugefileviewer-0.1.1/pthugefileviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 16:08:45.000000 pthugefileviewer-0.1.1/pthugefileviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-31 16:08:45.000000 pthugefileviewer-0.1.1/pthugefileviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-31 16:08:45.000000 pthugefileviewer-0.1.1/pthugefileviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-31 16:08:36.000000 pthugefileviewer-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-31 16:08:36.000000 pthugefileviewer-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-31 16:08:45.992790 pthugefileviewer-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-31 16:08:36.000000 pthugefileviewer-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:08:45.988790 pthugefileviewer-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:08:45.992790 pthugefileviewer-0.1.1/src/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6600 2024-03-31 16:08:36.000000 pthugefileviewer-0.1.1/src/bin/hfv-regexbuild
--rwxr-xr-x   0 runner    (1001) docker     (127)     1895 2024-03-31 16:08:36.000000 pthugefileviewer-0.1.1/src/bin/hfv-view
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:08:45.992790 pthugefileviewer-0.1.1/src/pthugefileviewer/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-31 16:08:36.000000 pthugefileviewer-0.1.1/src/pthugefileviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-03-31 16:08:36.000000 pthugefileviewer-0.1.1/src/pthugefileviewer/hugefilevieweruicontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 16:08:36.000000 pthugefileviewer-0.1.1/src/pthugefileviewer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:08:45.992790 pthugefileviewer-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-03-31 16:08:36.000000 pthugefileviewer-0.1.1/tests/test_hfv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/pthugefileviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-01 21:02:16.000000 pthugefileviewer-0.2.0/pthugefileviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-01 21:02:16.000000 pthugefileviewer-0.2.0/pthugefileviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:02:16.000000 pthugefileviewer-0.2.0/pthugefileviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 21:02:16.000000 pthugefileviewer-0.2.0/pthugefileviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-01 21:02:16.000000 pthugefileviewer-0.2.0/pthugefileviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:16.994155 pthugefileviewer-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/src/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6387 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/src/bin/hfv-regexbuild
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1895 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/src/bin/hfv-view
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/src/pthugefileviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/src/pthugefileviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/src/pthugefileviewer/hugefilevieweruicontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/src/pthugefileviewer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/tests/test_hfv.py
```

### Comparing `pthugefileviewer-0.1.1/LICENSE` & `pthugefileviewer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.1.1/PKG-INFO` & `pthugefileviewer-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pthugefileviewer
-Version: 0.1.1
+Version: 0.2.0
 Summary: Huge file viewer control for prompt-toolkit
 Home-page: http://github.com/lpenz/pthugefileviewer
 Author: "Leandro Lisboa Penz"
 Author-email: "lpenz@lpenz.org"
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

### Comparing `pthugefileviewer-0.1.1/README.md` & `pthugefileviewer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.1.1/pthugefileviewer.egg-info/PKG-INFO` & `pthugefileviewer-0.2.0/pthugefileviewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pthugefileviewer
-Version: 0.1.1
+Version: 0.2.0
 Summary: Huge file viewer control for prompt-toolkit
 Home-page: http://github.com/lpenz/pthugefileviewer
 Author: "Leandro Lisboa Penz"
 Author-email: "lpenz@lpenz.org"
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

### Comparing `pthugefileviewer-0.1.1/setup.cfg` & `pthugefileviewer-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pthugefileviewer
-version = 0.1.1
+version = 0.2.0
 description = Huge file viewer control for prompt-toolkit
 license = MIT
 license_files = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = "Leandro Lisboa Penz"
 author_email = "lpenz@lpenz.org"
```

### Comparing `pthugefileviewer-0.1.1/src/bin/hfv-regexbuild` & `pthugefileviewer-0.2.0/src/bin/hfv-regexbuild`

 * *Files 20% similar despite different names*

```diff
@@ -1,158 +1,150 @@
 #!/usr/bin/env python3
 """
-A console regular expression editor
+A console regular expression builder
 """
 
 import argparse
-import asyncio
-import logging
 import os
 import re
 from typing import Optional
 
 import pthugefileviewer
 from prompt_toolkit import Application
-from prompt_toolkit.application import get_app
 from prompt_toolkit.buffer import Buffer
 from prompt_toolkit.document import Document
 from prompt_toolkit.formatted_text import StyleAndTextTuples
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.key_binding.bindings.focus import focus_next
 from prompt_toolkit.key_binding.key_processor import KeyPressEvent
 from prompt_toolkit.layout.containers import Container, HSplit, Window
 from prompt_toolkit.layout.controls import BufferControl
 from prompt_toolkit.layout.layout import Layout
 from prompt_toolkit.styles import Style
 from prompt_toolkit.widgets import Frame
 
 E = KeyPressEvent
 
-MAX_LINES = 1000
-
 
 class FileviewControl(pthugefileviewer.HugeFileViewerUIControl):
     def __init__(self, filename: os.PathLike[str]) -> None:
         self.regex: Optional[re.Pattern[bytes]] = None
+        self.regex_ok: Optional[re.Pattern[bytes]] = None
         with open(filename, "rb") as fd:
             pthugefileviewer.HugeFileViewerUIControl.__init__(self, fd=fd)
 
-    def update_lines(self) -> None:
-        if not self.regex:
-            pthugefileviewer.HugeFileViewerUIControl.update_lines(self)
+    def use_regex(self, regex: Optional[re.Pattern[bytes]]) -> None:
+        self.regex = regex
+        self.update_lines()
+
+    def search_down(self) -> None:
+        if self.regex is None:
             return
-        self._mm.seek(self._offset)
+        with self.tmp_offset():
+            self.go_pagedown()
+            offset = self.offset
+        m = self.re_search(self.regex, offset)
+        if m:
+            self.go_line_offset(m.end())
+            self.go_up(self.height - 2)
+        else:
+            self.update_lines()
+
+    def update_lines(self) -> None:
         contents = b"\n".join(self.get_lines())
-        m = self.regex.search(contents)
+        m = None
+        if self.regex is not None:
+            m = self.regex.search(contents)
+        if m:
+            self.regex_ok = self.regex
+            style = "class:match"
+        elif not m and self.regex_ok is not None:
+            m = self.regex_ok.search(contents)
+            style = "class:oldmatch"
         if not m:
             pthugefileviewer.HugeFileViewerUIControl.update_lines(self)
             return
         start = m.start()
         end = m.end()
         pre, matched, pos = contents[:start], contents[start:end], contents[end:]
         self._lines = []
         current: StyleAndTextTuples = []
         lines = pre.split(b"\n")
         for i, line in enumerate(lines):
-            current += [("class:unmatched", line.decode("utf-8"))]
+            current += [("", line.decode("utf-8"))]
             if i != len(lines) - 1:
                 self._lines.append(current)
                 current = []
         lines = matched.split(b"\n")
         for i, line in enumerate(lines):
-            current += [("class:matched", line.decode("utf-8"))]
+            current += [(style, line.decode("utf-8"))]
             if i != len(lines) - 1:
                 self._lines.append(current)
                 current = []
         lines = pos.split(b"\n")
         for i, line in enumerate(lines):
-            current += [("class:unmatched", line.decode("utf-8"))]
+            current += [("", line.decode("utf-8"))]
             self._lines.append(current)
             current = []
 
 
-class Fileview:
+class FileviewWidget:
     def __init__(self, filename: os.PathLike[str]):
         self.filename = filename
         self.control = FileviewControl(filename)
         self.window = Window(self.control)
-        self._done_event = asyncio.Event()
-        self._regex_queue: asyncio.Queue[str] = asyncio.Queue()
-        self._task = asyncio.create_task(self.loader())
-
-    def use_regex(self, regex_str: str) -> None:
-        self._regex_queue.put_nowait(regex_str)
-        if self._task.done():
-            self._task.result()
-
-    def stop(self) -> None:
-        self._task.cancel()
-
-    def update(self, regex_str: str) -> None:
-        try:
-            regex = re.compile(bytes(regex_str, "utf-8"), re.S)
-        except re.error:
-            return
-        self.control.regex = regex
-        m = self.control.re_search(regex)
-        if m:
-            self.control.go_line_offset(m.start() - 1)
-
-    async def loader(self) -> None:
-        while not self._done_event.is_set():
-            regex_str = await self._regex_queue.get()
-            while not self._regex_queue.empty():
-                regex_str = await self._regex_queue.get()
-                self._regex_queue.task_done()
-            self.update(regex_str)
-            self._regex_queue.task_done()
-
-    def get_style(self) -> str:
-        if get_app().layout.has_focus(self.window):
-            return "class:hugefilewidget"
-        else:
-            return "class:hugefilewidget.unfocused"
 
     def __pt_container__(self) -> Container:
         return self.window
 
 
-class RegexWindow:
-    def __init__(self, fileview: Fileview, regex_str: str = ""):
+class RegexWidget:
+    def __init__(self, fileview: FileviewWidget, initial_regex_str: str = ""):
         self.fileview = fileview
-        self.regex_str = regex_str
+        self.regex_str = initial_regex_str
         self.buffer = Buffer(
             document=Document(text=self.regex_str),
             multiline=True,
             on_text_changed=self.regex_changed,
         )
         self.control = BufferControl(buffer=self.buffer)
         self.window = Window(self.control)
+        self.regex_changed(self.buffer)
 
     def regex_changed(self, buf: Buffer) -> None:
-        self.fileview.use_regex(buf.document.text)
+        try:
+            regex = re.compile(bytes(buf.document.text, "utf-8"), re.S)
+        except re.error:
+            self.fileview.control.use_regex(None)
+            return
+        self.fileview.control.use_regex(regex)
 
     def __pt_container__(self) -> Container:
         return self.window
 
 
-async def pthugefileviewer_run(
-    filename: os.PathLike[str], regex_str: Optional[str] = None
+def regexbuilder_run(
+    filename: os.PathLike[str], initial_regex_str: Optional[str] = None
 ) -> None:
-    fileview = Fileview(filename)
-    regexwin = RegexWindow(fileview, regex_str or "")
+    fileview = FileviewWidget(filename)
+    regexwin = RegexWidget(fileview, initial_regex_str or "")
     root_container = HSplit(
         [
             Frame(title=str(filename), body=fileview),
-            Frame(title="Regular expression", body=regexwin, height=7),
+            Frame(title="Regular expression", body=regexwin, height=5),
         ]
     )
     layout = Layout(root_container)
     layout.focus(regexwin)
-    style = Style.from_dict({"matched": "bold fg:white bg:green"})
+    style = Style.from_dict(
+        {
+            "match": "bold fg:white bg:green",
+            "oldmatch": "fg:gray bg:darkgreen",
+        }
+    )
     kb = KeyBindings()
     app: Application[None] = Application(
         layout=layout,
         key_bindings=kb,
         full_screen=True,
         style=style,
         mouse_support=True,
@@ -174,24 +166,36 @@
     def pageup(event: E) -> None:
         fileview.control.go_pageup()
 
     @kb.add("c-pagedown")
     def pagedown(event: E) -> None:
         fileview.control.go_pagedown()
 
+    @kb.add("c-home")
+    def c_home(event: E) -> None:
+        fileview.control.go_top()
+
+    @kb.add("c-end")
+    def c_end(event: E) -> None:
+        fileview.control.go_bottom()
+
+    @kb.add("escape", "j")
+    def search_down(event: E) -> None:
+        fileview.control.search_down()
+
     @kb.add("c-c")
     @kb.add("c-d")
     @kb.add("escape", "q")
     def close(event: E) -> None:
         app.exit()
 
-    await app.run_async()
+    app.run()
 
 
-async def main() -> None:
+def main() -> None:
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument(
         "--regex",
         "-e",
         default=None,
         help="Initial regular expression",
     )
@@ -199,13 +203,12 @@
         "--version",
         "-V",
         action="version",
         version="%(prog)s " + pthugefileviewer.version(),
     )
     parser.add_argument("files", type=str, nargs=1, help="Files to match the regex")
     args = parser.parse_args()
-    logging.basicConfig(filename="log.txt", level=logging.INFO)
-    await pthugefileviewer_run(args.files[0], regex_str=args.regex)
+    regexbuilder_run(args.files[0], initial_regex_str=args.regex)
 
 
 if __name__ == "__main__":
-    asyncio.get_event_loop().run_until_complete(main())
+    main()
```

### Comparing `pthugefileviewer-0.1.1/src/bin/hfv-view` & `pthugefileviewer-0.2.0/src/bin/hfv-view`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.1.1/src/pthugefileviewer/hugefilevieweruicontrol.py` & `pthugefileviewer-0.2.0/src/pthugefileviewer/hugefilevieweruicontrol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Control for the huge file widget"""
 
 import io
 import mmap
 import re
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Generator, List, Optional
+from typing import TYPE_CHECKING, Generator, List, Optional  # noqa: I101
 
 from prompt_toolkit.formatted_text import StyleAndTextTuples
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.key_binding.key_bindings import KeyBindingsBase
 from prompt_toolkit.key_binding.key_processor import KeyPressEvent
 from prompt_toolkit.layout.controls import UIContent, UIControl
 from prompt_toolkit.mouse_events import MouseEvent, MouseEventType
@@ -145,16 +145,20 @@
             self.go_down()
         else:
             return NotImplemented
         return None
 
     # Exported utility functions:
 
-    def re_search(self, regex: re.Pattern[bytes]) -> Optional[re.Match[bytes]]:
-        return regex.search(bytes(self._mm))
+    def re_search(
+        self, regex: re.Pattern[bytes], offset: Optional[int] = None
+    ) -> Optional[re.Match[bytes]]:
+        offset = offset or 0
+        with self.tmp_offset():
+            return regex.search(bytes(self._mm), offset)
 
     def go_line_offset(self, offset: int) -> None:
         self.offset = offset
         if self.get_char(offset - 1) == b"\n":
             return
         offset = self.find_prev_newline(offset)
         if offset != -1:
```

### Comparing `pthugefileviewer-0.1.1/tests/test_hfv.py` & `pthugefileviewer-0.2.0/tests/test_hfv.py`

 * *Files identical despite different names*

