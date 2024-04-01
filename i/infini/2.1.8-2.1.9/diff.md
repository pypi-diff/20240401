# Comparing `tmp/infini-2.1.8.tar.gz` & `tmp/infini-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infini-2.1.8.tar", last modified: Wed Mar 20 04:15:25 2024, max compression
+gzip compressed data, was "infini-2.1.9.tar", last modified: Sun Mar 31 07:05:41 2024, max compression
```

## Comparing `infini-2.1.8.tar` & `infini-2.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1110 2024-03-04 04:57:55.577863 infini-2.1.8/LICENSE
--rw-r--r--   0        0        0     1790 2024-03-04 08:04:35.361800 infini-2.1.8/README.md
--rw-r--r--   0        0        0      826 2024-03-20 04:15:25.989901 infini-2.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-30 06:33:19.031919 infini-2.1.8/src/infini/__init__.py
--rw-r--r--   0        0        0     3546 2024-03-04 09:43:54.636058 infini-2.1.8/src/infini/core.py
--rw-r--r--   0        0        0     1387 2024-03-19 13:20:07.535510 infini-2.1.8/src/infini/doc.py
--rw-r--r--   0        0        0      372 2024-03-04 09:55:27.624940 infini-2.1.8/src/infini/exceptions.py
--rw-r--r--   0        0        0     2350 2024-03-15 07:04:23.934140 infini-2.1.8/src/infini/generator.py
--rw-r--r--   0        0        0     1441 2024-03-15 07:04:39.131528 infini-2.1.8/src/infini/handler.py
--rw-r--r--   0        0        0     1508 2024-02-29 05:11:03.823030 infini-2.1.8/src/infini/injector.py
--rw-r--r--   0        0        0     1210 2024-03-15 07:00:00.654769 infini-2.1.8/src/infini/input.py
--rw-r--r--   0        0        0     3138 2024-03-11 05:06:05.172406 infini-2.1.8/src/infini/interceptor.py
--rw-r--r--   0        0        0     1380 2024-03-15 08:15:51.110340 infini-2.1.8/src/infini/internal.py
--rw-r--r--   0        0        0     8285 2024-03-17 12:06:42.964970 infini-2.1.8/src/infini/loader.py
--rw-r--r--   0        0        0      429 2024-01-28 09:22:42.949732 infini-2.1.8/src/infini/logging.py
--rw-r--r--   0        0        0      745 2024-03-04 09:33:19.700129 infini-2.1.8/src/infini/output.py
--rw-r--r--   0        0        0     1322 2024-01-29 10:35:40.134454 infini-2.1.8/src/infini/queue.py
--rw-r--r--   0        0        0     6464 2024-03-19 13:28:24.672882 infini-2.1.8/src/infini/register.py
--rw-r--r--   0        0        0     1774 2024-03-15 07:22:07.499523 infini-2.1.8/src/infini/router.py
--rw-r--r--   0        0        0      823 2024-03-15 07:14:16.954607 infini-2.1.8/src/infini/typing.py
--rw-r--r--   0        0        0        0 2024-01-28 09:22:42.950732 infini-2.1.8/tests/__init__.py
--rw-r--r--   0        0        0      150 2024-01-28 09:22:42.951732 infini-2.1.8/tests/examples/ndice/infini.toml
--rw-r--r--   0        0        0    10486 2024-01-28 09:22:42.951732 infini-2.1.8/tests/examples/ndice/src/dicer.py
--rw-r--r--   0        0        0     4389 2024-03-11 04:37:40.745767 infini-2.1.8/tests/examples/ndice/src/ndice.py
--rw-r--r--   0        0        0      425 2024-03-11 04:37:40.749795 infini-2.1.8/tests/examples/ndice/tests.py
--rw-r--r--   0        0        0     2411 2024-03-04 09:46:32.768351 infini-2.1.8/tests/test_core.py
--rw-r--r--   0        0        0     1970 2024-03-04 04:33:35.407986 infini-2.1.8/tests/test_generator.py
--rw-r--r--   0        0        0     2326 2024-03-04 09:45:11.673117 infini-2.1.8/tests/test_handlers.py
--rw-r--r--   0        0        0     1124 2024-03-04 03:38:48.112206 infini-2.1.8/tests/test_injector.py
--rw-r--r--   0        0        0      530 2024-03-15 06:59:33.889303 infini-2.1.8/tests/test_input.py
--rw-r--r--   0        0        0     1291 2024-03-04 03:47:20.980386 infini-2.1.8/tests/test_interceptor.py
--rw-r--r--   0        0        0      216 2024-01-28 09:22:42.953732 infini-2.1.8/tests/test_internal.py
--rw-r--r--   0        0        0     1405 2024-03-04 04:25:16.558095 infini-2.1.8/tests/test_loader.py
--rw-r--r--   0        0        0     1954 2024-03-04 04:25:04.568957 infini-2.1.8/tests/test_register.py
--rw-r--r--   0        0        0     1273 2024-03-04 09:54:06.369967 infini-2.1.8/tests/test_workflow.py
--rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 infini-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-03-31 07:05:22.587647 infini-2.1.9/LICENSE
+-rw-r--r--   0        0        0     1769 2024-03-31 07:05:22.587647 infini-2.1.9/README.md
+-rw-r--r--   0        0        0      826 2024-03-31 07:05:41.071590 infini-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/__init__.py
+-rw-r--r--   0        0        0     3455 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/core.py
+-rw-r--r--   0        0        0     1342 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/doc.py
+-rw-r--r--   0        0        0      354 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/exceptions.py
+-rw-r--r--   0        0        0     2282 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/generator.py
+-rw-r--r--   0        0        0     1398 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/handler.py
+-rw-r--r--   0        0        0     1472 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/injector.py
+-rw-r--r--   0        0        0     1167 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/input.py
+-rw-r--r--   0        0        0     3049 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/interceptor.py
+-rw-r--r--   0        0        0     1337 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/internal.py
+-rw-r--r--   0        0        0     8075 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/loader.py
+-rw-r--r--   0        0        0      406 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/logging.py
+-rw-r--r--   0        0        0      714 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/output.py
+-rw-r--r--   0        0        0     1275 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/queue.py
+-rw-r--r--   0        0        0     6258 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/register.py
+-rw-r--r--   0        0        0     1714 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/router.py
+-rw-r--r--   0        0        0      789 2024-03-31 07:05:22.591647 infini-2.1.9/src/infini/typing.py
+-rw-r--r--   0        0        0        0 2024-03-31 07:05:22.591647 infini-2.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      141 2024-03-31 07:05:22.591647 infini-2.1.9/tests/examples/ndice/infini.toml
+-rw-r--r--   0        0        0    10126 2024-03-31 07:05:22.591647 infini-2.1.9/tests/examples/ndice/src/dicer.py
+-rw-r--r--   0        0        0     4233 2024-03-31 07:05:22.591647 infini-2.1.9/tests/examples/ndice/src/ndice.py
+-rw-r--r--   0        0        0      408 2024-03-31 07:05:22.591647 infini-2.1.9/tests/examples/ndice/tests.py
+-rw-r--r--   0        0        0     2330 2024-03-31 07:05:22.591647 infini-2.1.9/tests/test_core.py
+-rw-r--r--   0        0        0     1901 2024-03-31 07:05:22.591647 infini-2.1.9/tests/test_generator.py
+-rw-r--r--   0        0        0     2230 2024-03-31 07:05:22.591647 infini-2.1.9/tests/test_handlers.py
+-rw-r--r--   0        0        0     1078 2024-03-31 07:05:22.591647 infini-2.1.9/tests/test_injector.py
+-rw-r--r--   0        0        0      514 2024-03-31 07:05:22.591647 infini-2.1.9/tests/test_input.py
+-rw-r--r--   0        0        0     1253 2024-03-31 07:05:22.591647 infini-2.1.9/tests/test_interceptor.py
+-rw-r--r--   0        0        0      205 2024-03-31 07:05:22.591647 infini-2.1.9/tests/test_internal.py
+-rw-r--r--   0        0        0     1358 2024-03-31 07:05:22.591647 infini-2.1.9/tests/test_loader.py
+-rw-r--r--   0        0        0     1895 2024-03-31 07:05:22.591647 infini-2.1.9/tests/test_register.py
+-rw-r--r--   0        0        0     1226 2024-03-31 07:05:22.591647 infini-2.1.9/tests/test_workflow.py
+-rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 infini-2.1.9/PKG-INFO
```

### Comparing `infini-2.1.8/LICENSE` & `infini-2.1.9/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 HydroRoll-Team & Noctisynth, org
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 HydroRoll-Team & Noctisynth, org
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `infini-2.1.8/README.md` & `infini-2.1.9/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Infini 2
-
-<!-- start index -->
-
-## 简述
-
-Infini 2 是一个先进的内容输入输出流标准框架，它的诞生源于对于平台机器人的代码复用问题，以及指令的动态解析问题。Infini 2 的规则包是可热插拔的，它以使用 Infini 框架的规则包为最小热插拔单元，以`输入→预拦截→业务函数→内容生成→内容拦截→输出`为一整套 Infini 输入输出流程式，规则包可以定制化的注册任一流程层次的处理函数。
-
-Infini 2 同样是**跨平台跨框架**的。你可以在任何支持 Python 的平台运行 Infini，同样的，你在对接平台时，可以选用任何框架来适配 Infini 2，例如[`Nonebot2`](https://nonebot.dev/)、[`OlivOS`](https://doc.olivos.wiki/)和[`iamai`](https://github.com/retrofor/iamai/)等，而这些框架都是跨平台和跨协议的，这意味着 Infini 2 同样是跨平台和跨协议支持的。Infini 可能将在未来版本支持直接对接平台协议。
-
-Infini 2 所有层次的业务函数都是依照参数名进行**依赖注入**的，你可以动态的选择你所需要的注入参数。由于先进的架构特性，Infini 2 可以省去大量的开发时间，节约开发成本。同时由于其轻量的输入输出流程式，它拥有较低的学习成本。
-
-## 开发者
-
-欢迎任何遵循社区常态的开发者参与 Infini 2 的开发和社区构建，欢迎加入[Infini 2 公测 QQ 群: 231892965](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=B90zg667S_HvfwsG3V3iVGumtLNjY3CN&authKey=H%2Bw4RqjV5sjAmUUbUkUlQsYQGcjdDd0nW%2BBnnTRCL1duIis8RJnj5qTSyN7e7jds&noverify=0&group_code=231892965)。
-
-## 版权
-
-水系 × [浊莲](https://github.com/noctisynth)依照 MIT 协议开源 Infini。
-
-<!-- end index -->
+# Infini 2
+
+<!-- start index -->
+
+## 简述
+
+Infini 2 是一个先进的内容输入输出流标准框架，它的诞生源于对于平台机器人的代码复用问题，以及指令的动态解析问题。Infini 2 的规则包是可热插拔的，它以使用 Infini 框架的规则包为最小热插拔单元，以`输入→预拦截→业务函数→内容生成→内容拦截→输出`为一整套 Infini 输入输出流程式，规则包可以定制化的注册任一流程层次的处理函数。
+
+Infini 2 同样是**跨平台跨框架**的。你可以在任何支持 Python 的平台运行 Infini，同样的，你在对接平台时，可以选用任何框架来适配 Infini 2，例如[`Nonebot2`](https://nonebot.dev/)、[`OlivOS`](https://doc.olivos.wiki/)和[`iamai`](https://github.com/retrofor/iamai/)等，而这些框架都是跨平台和跨协议的，这意味着 Infini 2 同样是跨平台和跨协议支持的。Infini 可能将在未来版本支持直接对接平台协议。
+
+Infini 2 所有层次的业务函数都是依照参数名进行**依赖注入**的，你可以动态的选择你所需要的注入参数。由于先进的架构特性，Infini 2 可以省去大量的开发时间，节约开发成本。同时由于其轻量的输入输出流程式，它拥有较低的学习成本。
+
+## 开发者
+
+欢迎任何遵循社区常态的开发者参与 Infini 2 的开发和社区构建，欢迎加入[Infini 2 公测 QQ 群: 231892965](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=B90zg667S_HvfwsG3V3iVGumtLNjY3CN&authKey=H%2Bw4RqjV5sjAmUUbUkUlQsYQGcjdDd0nW%2BBnnTRCL1duIis8RJnj5qTSyN7e7jds&noverify=0&group_code=231892965)。
+
+## 版权
+
+水系 × [浊莲](https://github.com/noctisynth)依照 MIT 协议开源 Infini。
+
+<!-- end index -->
```

### Comparing `infini-2.1.8/pyproject.toml` & `infini-2.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "infini"
-version = "2.1.8"
+version = "2.1.9"
 description = "Infini 内容输入输出流框架"
 authors = [
     { name = "苏向夜", email = "fu050409@163.com" },
     { name = "简律纯", email = "leader@hydroroll.team" },
 ]
 dependencies = [
     "rich>=13.7.0",
```

### Comparing `infini-2.1.8/src/infini/core.py` & `infini-2.1.9/src/infini/core.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from infini.input import Input
-from infini.interceptor import Interceptor
-from infini.generator import Generator
-from infini.handler import Handler
-from infini.injector import Injector
-from infini.output import Output
-from infini.typing import Any, Generator as GeneratorT, Union
-from infini.exceptions import ValueError
-
-
-class Core:
-    pre_interceptor: Interceptor
-    handler: Handler
-    generator: Generator
-    interceptor: Interceptor
-    injector: Injector
-
-    def input(self, input: Input) -> GeneratorT[Union[str, Output], Any, None]:
-        for pre_intercepted_stream in self.pre_intercept(input):
-            if isinstance(pre_intercepted_stream, Output):
-                if not isinstance(pre_intercepted_stream, Output):
-                    raise ValueError(
-                        "Interceptor functions should return or yield a `Output` object."
-                    )
-                if pre_intercepted_stream.is_empty():
-                    return
-                if pre_intercepted_stream.type == "workflow":
-                    yield pre_intercepted_stream
-                    if pre_intercepted_stream.block:
-                        while pre_intercepted_stream.status != 0:
-                            pass
-                    continue
-                else:
-                    yield self.generate(pre_intercepted_stream)  # TODO 拦截拦截器文本
-
-                if pre_intercepted_stream.block:
-                    return
-            else:
-                input = pre_intercepted_stream
-
-        for handled_stream in self.handle(input):
-            if not isinstance(handled_stream, Output):
-                raise ValueError(
-                    "Handler functions should return or yield a `Output` object."
-                )
-            if handled_stream.is_empty():
-                return
-            if handled_stream.type == "workflow":
-                yield handled_stream
-                if handled_stream.block:
-                    while handled_stream.status != 0:
-                        pass
-                continue
-            else:
-                outcome = self.generate(handled_stream)
-            for stream in self.intercept(handled_stream, outcome):
-                if isinstance(stream, Output):
-                    if stream.is_empty():
-                        return
-                    if stream.type == "workflow":
-                        yield stream
-                        if stream.block:
-                            while stream.status != 0:
-                                pass
-                    else:
-                        yield self.generate(stream)
-                        if stream.block:
-                            return
-                    continue
-                outcome = stream
-            yield outcome
-            if handled_stream.block:
-                return
-
-    def pre_intercept(
-        self, input: Input
-    ) -> GeneratorT[Union[Input, Output], Any, None]:
-        return self.pre_interceptor.input(input)
-
-    def handle(self, input: Input) -> GeneratorT[Output, Any, None]:
-        iterator = self.handler.input(input)
-        for output in iterator:
-            yield output
-
-    def generate(self, output: Output) -> str:
-        return self.generator.output(output, self.injector)
-
-    def intercept(
-        self, output: Output, output_text: str
-    ) -> GeneratorT[Union[str, Output], Any, None]:
-        return self.interceptor.output(output, output_text)
+from infini.input import Input
+from infini.interceptor import Interceptor
+from infini.generator import Generator
+from infini.handler import Handler
+from infini.injector import Injector
+from infini.output import Output
+from infini.typing import Any, Generator as GeneratorT, Union
+from infini.exceptions import ValueError
+
+
+class Core:
+    pre_interceptor: Interceptor
+    handler: Handler
+    generator: Generator
+    interceptor: Interceptor
+    injector: Injector
+
+    def input(self, input: Input) -> GeneratorT[Union[str, Output], Any, None]:
+        for pre_intercepted_stream in self.pre_intercept(input):
+            if isinstance(pre_intercepted_stream, Output):
+                if not isinstance(pre_intercepted_stream, Output):
+                    raise ValueError(
+                        "Interceptor functions should return or yield a `Output` object."
+                    )
+                if pre_intercepted_stream.is_empty():
+                    return
+                if pre_intercepted_stream.type == "workflow":
+                    yield pre_intercepted_stream
+                    if pre_intercepted_stream.block:
+                        while pre_intercepted_stream.status != 0:
+                            pass
+                    continue
+                else:
+                    yield self.generate(pre_intercepted_stream)  # TODO 拦截拦截器文本
+
+                if pre_intercepted_stream.block:
+                    return
+            else:
+                input = pre_intercepted_stream
+
+        for handled_stream in self.handle(input):
+            if not isinstance(handled_stream, Output):
+                raise ValueError(
+                    "Handler functions should return or yield a `Output` object."
+                )
+            if handled_stream.is_empty():
+                return
+            if handled_stream.type == "workflow":
+                yield handled_stream
+                if handled_stream.block:
+                    while handled_stream.status != 0:
+                        pass
+                continue
+            else:
+                outcome = self.generate(handled_stream)
+            for stream in self.intercept(handled_stream, outcome):
+                if isinstance(stream, Output):
+                    if stream.is_empty():
+                        return
+                    if stream.type == "workflow":
+                        yield stream
+                        if stream.block:
+                            while stream.status != 0:
+                                pass
+                    else:
+                        yield self.generate(stream)
+                        if stream.block:
+                            return
+                    continue
+                outcome = stream
+            yield outcome
+            if handled_stream.block:
+                return
+
+    def pre_intercept(
+        self, input: Input
+    ) -> GeneratorT[Union[Input, Output], Any, None]:
+        return self.pre_interceptor.input(input)
+
+    def handle(self, input: Input) -> GeneratorT[Output, Any, None]:
+        iterator = self.handler.input(input)
+        for output in iterator:
+            yield output
+
+    def generate(self, output: Output) -> str:
+        return self.generator.output(output, self.injector)
+
+    def intercept(
+        self, output: Output, output_text: str
+    ) -> GeneratorT[Union[str, Output], Any, None]:
+        return self.interceptor.output(output, output_text)
```

### Comparing `infini-2.1.8/src/infini/handler.py` & `infini-2.1.9/src/infini/handler.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from infini.injector import Injector
-from infini.input import Input
-from infini.output import Output
-from infini.typing import List, Any, RouterType, Callable, Generator, Union
-from infini.queue import EventQueue
-
-
-class Handler:
-    handlers: List[RouterType]
-
-    def input(self, input: Input):
-        injector = Injector()
-        parameters = {
-            "input": input,
-            "plain_text": input.get_plain_text(),
-            "user_id": input.get_user_id(),
-        }
-        if (queue := self.match(injector, **parameters)).is_empty():
-            yield Output.empty()
-            return
-        while not queue.is_empty():
-            if isinstance(
-                stream := injector.output(queue.pop(), parameters=parameters), Generator
-            ):
-                for output in stream:
-                    yield output
-                    if output.block:
-                        return
-            else:
-                yield stream
-                if stream.block:
-                    return
-
-    def match(
-        self, injector: Injector, **parameters
-    ) -> EventQueue[Callable[..., Union[Output, Generator[Output, Any, None]]]]:
-        queue = EventQueue()
-
-        for handler in self.handlers:
-            if injector.output(handler["router"].match, parameters=parameters):
-                queue.push(handler["priority"], handler["handler"])
-
-        return queue
+from infini.injector import Injector
+from infini.input import Input
+from infini.output import Output
+from infini.typing import List, Any, RouterType, Callable, Generator, Union
+from infini.queue import EventQueue
+
+
+class Handler:
+    handlers: List[RouterType]
+
+    def input(self, input: Input):
+        injector = Injector()
+        parameters = {
+            "input": input,
+            "plain_text": input.get_plain_text(),
+            "user_id": input.get_user_id(),
+        }
+        if (queue := self.match(injector, **parameters)).is_empty():
+            yield Output.empty()
+            return
+        while not queue.is_empty():
+            if isinstance(
+                stream := injector.output(queue.pop(), parameters=parameters), Generator
+            ):
+                for output in stream:
+                    yield output
+                    if output.block:
+                        return
+            else:
+                yield stream
+                if stream.block:
+                    return
+
+    def match(
+        self, injector: Injector, **parameters
+    ) -> EventQueue[Callable[..., Union[Output, Generator[Output, Any, None]]]]:
+        queue = EventQueue()
+
+        for handler in self.handlers:
+            if injector.output(handler["router"].match, parameters=parameters):
+                queue.push(handler["priority"], handler["handler"])
+
+        return queue
```

### Comparing `infini-2.1.8/src/infini/injector.py` & `infini-2.1.9/src/infini/injector.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from infini.typing import Callable, T, Optional, Dict, Any
-
-import inspect
-
-
-class Injector:
-    def __init__(self) -> None:
-        self.parameters: Dict[str, Any] = {}
-
-    def inject(
-        self, func: Callable[..., T], parameters: Optional[Dict[str, Any]] = None
-    ) -> Callable[[], T]:
-        signature = inspect.signature(func)
-        _parameters = {} if parameters is None else parameters
-        parameters = self.parameters.copy()
-        parameters.update(_parameters)
-        inject_params = {}
-        for param_name, param in signature.parameters.items():
-            default = None if param.default == inspect._empty else param.default
-            if param_name in parameters:
-                if not isinstance(parameters[param_name], param.annotation):
-                    raise ValueError(
-                        f"Parameter with name '{param_name}' has a mismatch type, "
-                        f"expected '{param.annotation!r}' but got '{type(parameters[param_name])!r}'."
-                    )
-                inject_params[param_name] = parameters[param_name]
-            else:
-                inject_params[param_name] = default
-        bound_args = signature.bind(**inject_params)
-        bound_args.apply_defaults()
-        return lambda: func(*bound_args.args, **bound_args.kwargs)
-
-    def output(
-        self, func: Callable[..., T], parameters: Optional[Dict[str, Any]] = None
-    ) -> T:
-        return self.inject(func, parameters)()
+from infini.typing import Callable, T, Optional, Dict, Any
+
+import inspect
+
+
+class Injector:
+    def __init__(self) -> None:
+        self.parameters: Dict[str, Any] = {}
+
+    def inject(
+        self, func: Callable[..., T], parameters: Optional[Dict[str, Any]] = None
+    ) -> Callable[[], T]:
+        signature = inspect.signature(func)
+        _parameters = {} if parameters is None else parameters
+        parameters = self.parameters.copy()
+        parameters.update(_parameters)
+        inject_params = {}
+        for param_name, param in signature.parameters.items():
+            default = None if param.default == inspect._empty else param.default
+            if param_name in parameters:
+                if not isinstance(parameters[param_name], param.annotation):
+                    raise ValueError(
+                        f"Parameter with name '{param_name}' has a mismatch type, "
+                        f"expected '{param.annotation!r}' but got '{type(parameters[param_name])!r}'."
+                    )
+                inject_params[param_name] = parameters[param_name]
+            else:
+                inject_params[param_name] = default
+        bound_args = signature.bind(**inject_params)
+        bound_args.apply_defaults()
+        return lambda: func(*bound_args.args, **bound_args.kwargs)
+
+    def output(
+        self, func: Callable[..., T], parameters: Optional[Dict[str, Any]] = None
+    ) -> T:
+        return self.inject(func, parameters)()
```

### Comparing `infini-2.1.8/src/infini/input.py` & `infini-2.1.9/src/infini/input.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from infini.typing import Literal, Optional
-from infini.typing import Dict, Any, Generic, T, Optional
-from infini.output import Output
-
-
-class Input(Generic[T]):
-    plain_data: T
-    variables: Dict[str, Any]
-
-    def __init__(
-        self, plain_data: T, variables: Optional[Dict[str, Any]] = None
-    ) -> None:
-        self.plain_data = plain_data
-        self.variables = variables or {}
-
-    def get_user_id(self) -> str:
-        return self.variables.get("user_id", "0")
-
-    def get_session_id(self) -> str:
-        return (
-            self.variables.get("group_id")
-            or self.variables.get("session_id")
-            or self.variables.get("user_id")
-            or "0"
-        )
-
-    def is_tome(self) -> bool:
-        return bool(self.variables.get("is_tome"))
-
-    def get_plain_text(self) -> str:
-        return str(self.plain_data)
-
-    def output(
-        self,
-        type: Literal["text", "workflow"],
-        name: str,
-        *,
-        block: bool = False,
-        variables: Dict[str, Any] = {},
-    ):
-        vars = self.variables.copy()
-        vars.update(variables)
-        return Output(type, name, block=block, variables=vars)
+from infini.typing import Literal, Optional
+from infini.typing import Dict, Any, Generic, T, Optional
+from infini.output import Output
+
+
+class Input(Generic[T]):
+    plain_data: T
+    variables: Dict[str, Any]
+
+    def __init__(
+        self, plain_data: T, variables: Optional[Dict[str, Any]] = None
+    ) -> None:
+        self.plain_data = plain_data
+        self.variables = variables or {}
+
+    def get_user_id(self) -> str:
+        return self.variables.get("user_id", "0")
+
+    def get_session_id(self) -> str:
+        return (
+            self.variables.get("group_id")
+            or self.variables.get("session_id")
+            or self.variables.get("user_id")
+            or "0"
+        )
+
+    def is_tome(self) -> bool:
+        return bool(self.variables.get("is_tome"))
+
+    def get_plain_text(self) -> str:
+        return str(self.plain_data)
+
+    def output(
+        self,
+        type: Literal["text", "workflow"],
+        name: str,
+        *,
+        block: bool = False,
+        variables: Dict[str, Any] = {},
+    ):
+        vars = self.variables.copy()
+        vars.update(variables)
+        return Output(type, name, block=block, variables=vars)
```

### Comparing `infini-2.1.8/src/infini/interceptor.py` & `infini-2.1.9/src/infini/interceptor.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from infini.injector import Injector
-from infini.input import Input
-from infini.output import Output
-from infini.typing import List, Any, RouterType, Callable, Generator, Union
-from infini.queue import EventQueue
-
-
-class Interceptor:
-    interceptors: List[RouterType]
-
-    def input(self, input: Input) -> Generator[Union[Output, Input], Any, None]:
-        injector = Injector()
-        parameters = {
-            "input": input,
-            "plain_text": input.get_plain_text(),
-            "user_id": input.get_user_id(),
-        }
-        queue = self.match(injector, **parameters)
-        while not queue.is_empty():
-            if isinstance(
-                stream := injector.output(queue.pop(), parameters=parameters),
-                Generator,
-            ):
-                for outcome in stream:
-                    if isinstance(outcome, Input):
-                        input = outcome
-                        break
-                    yield outcome
-                    if outcome.block:
-                        return
-            else:
-                if stream is None:
-                    yield Output.empty()
-                    return
-                if isinstance(stream, Output):
-                    yield stream
-                    if stream.block:
-                        return
-                    continue
-                input = stream
-        yield input
-
-    def output(
-        self, output: Output, output_text: str
-    ) -> Generator[Union[Output, str], Any, None]:
-        input = Input(output_text, variables=output.variables)
-        injector = Injector()
-        parameters = {
-            "input": input,
-            "output": output,
-            "plain_text": output_text,
-            "user_id": input.get_user_id(),
-        }
-        queue = self.match(injector, **parameters)
-        while not queue.is_empty():
-            if isinstance(
-                stream := injector.output(queue.pop(), parameters=parameters), Generator
-            ):
-                for outcome in stream:
-                    if isinstance(outcome, Input):
-                        input = outcome
-                        break
-                    yield outcome
-                    if outcome.block:
-                        return
-            else:
-                if stream is None:
-                    yield Output.empty()
-                    return
-                if isinstance(stream, Output):
-                    yield stream
-                    if stream.block:
-                        return
-                    continue
-                input = stream
-        yield input.get_plain_text()
-
-    def match(
-        self, injector: Injector, **parameters
-    ) -> EventQueue[
-        Callable[..., Union[Input, Output, Generator[Union[Input, Output], Any, None]]]
-    ]:
-        queue = EventQueue()
-
-        for interceptor in self.interceptors:
-            if injector.output(interceptor["router"].match, parameters=parameters):
-                queue.push(interceptor["priority"], interceptor["handler"])
-
-        return queue
+from infini.injector import Injector
+from infini.input import Input
+from infini.output import Output
+from infini.typing import List, Any, RouterType, Callable, Generator, Union
+from infini.queue import EventQueue
+
+
+class Interceptor:
+    interceptors: List[RouterType]
+
+    def input(self, input: Input) -> Generator[Union[Output, Input], Any, None]:
+        injector = Injector()
+        parameters = {
+            "input": input,
+            "plain_text": input.get_plain_text(),
+            "user_id": input.get_user_id(),
+        }
+        queue = self.match(injector, **parameters)
+        while not queue.is_empty():
+            if isinstance(
+                stream := injector.output(queue.pop(), parameters=parameters),
+                Generator,
+            ):
+                for outcome in stream:
+                    if isinstance(outcome, Input):
+                        input = outcome
+                        break
+                    yield outcome
+                    if outcome.block:
+                        return
+            else:
+                if stream is None:
+                    yield Output.empty()
+                    return
+                if isinstance(stream, Output):
+                    yield stream
+                    if stream.block:
+                        return
+                    continue
+                input = stream
+        yield input
+
+    def output(
+        self, output: Output, output_text: str
+    ) -> Generator[Union[Output, str], Any, None]:
+        input = Input(output_text, variables=output.variables)
+        injector = Injector()
+        parameters = {
+            "input": input,
+            "output": output,
+            "plain_text": output_text,
+            "user_id": input.get_user_id(),
+        }
+        queue = self.match(injector, **parameters)
+        while not queue.is_empty():
+            if isinstance(
+                stream := injector.output(queue.pop(), parameters=parameters), Generator
+            ):
+                for outcome in stream:
+                    if isinstance(outcome, Input):
+                        input = outcome
+                        break
+                    yield outcome
+                    if outcome.block:
+                        return
+            else:
+                if stream is None:
+                    yield Output.empty()
+                    return
+                if isinstance(stream, Output):
+                    yield stream
+                    if stream.block:
+                        return
+                    continue
+                input = stream
+        yield input.get_plain_text()
+
+    def match(
+        self, injector: Injector, **parameters
+    ) -> EventQueue[
+        Callable[..., Union[Input, Output, Generator[Union[Input, Output], Any, None]]]
+    ]:
+        queue = EventQueue()
+
+        for interceptor in self.interceptors:
+            if injector.output(interceptor["router"].match, parameters=parameters):
+                queue.push(interceptor["priority"], interceptor["handler"])
+
+        return queue
```

### Comparing `infini-2.1.8/src/infini/output.py` & `infini-2.1.9/src/infini/output.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from infini.typing import Union, Literal, Dict, Any
-
-
-class Output:
-    type: Union[Literal["null", "text", "workflow"], str]
-    name: str
-    status: int
-    block: bool
-
-    variables: Dict[str, Any]
-
-    def __init__(
-        self,
-        type: Union[Literal["null", "text", "workflow"], str],
-        name: str,
-        *,
-        block: bool = False,
-        variables: Dict[str, Any] = {},
-    ) -> None:
-        self.type = type
-        self.name = name
-        self.status = 1
-        self.block = block
-        self.variables = variables
-
-    @classmethod
-    def empty(cls) -> "Output":
-        return cls("null", "null", block=True)
-
-    def is_empty(self) -> bool:
-        return self.type == "null"
+from infini.typing import Union, Literal, Dict, Any
+
+
+class Output:
+    type: Union[Literal["null", "text", "workflow"], str]
+    name: str
+    status: int
+    block: bool
+
+    variables: Dict[str, Any]
+
+    def __init__(
+        self,
+        type: Union[Literal["null", "text", "workflow"], str],
+        name: str,
+        *,
+        block: bool = False,
+        variables: Dict[str, Any] = {},
+    ) -> None:
+        self.type = type
+        self.name = name
+        self.status = 1
+        self.block = block
+        self.variables = variables
+
+    @classmethod
+    def empty(cls) -> "Output":
+        return cls("null", "null", block=True)
+
+    def is_empty(self) -> bool:
+        return self.type == "null"
```

### Comparing `infini-2.1.8/src/infini/queue.py` & `infini-2.1.9/src/infini/queue.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from infini.exceptions import KeyError
-from infini.typing import Generic, T
-from collections import deque
-
-import heapq
-
-
-class EventQueue(Generic[T]):
-    heap: list
-    entry_finder: dict
-    counter: int
-    order_queue: deque
-
-    def __init__(self) -> None:
-        self.heap = []
-        self.entry_finder = {}
-        self.counter = 0
-        self.order_queue = deque()
-
-    def push(self, priority: int, item: T) -> None:
-        if item in self.entry_finder:
-            self.remove(item)
-        entry = [priority, self.counter, item]
-        self.counter += 1
-        self.entry_finder[item] = entry
-        heapq.heappush(self.heap, entry)
-        self.order_queue.appendleft(item)
-
-    def pop(self) -> T:
-        while self.heap:
-            _, _, item = heapq.heappop(self.heap)
-            if self.entry_finder[item] is not None:
-                del self.entry_finder[item]
-                self.order_queue.remove(item)
-                return item
-        raise KeyError("Event queue is empty.")
-
-    def remove(self, item) -> None:
-        entry = self.entry_finder.pop(item)
-        entry[-1] = None
-
-    def is_empty(self) -> bool:
-        return not bool(self.heap)
-
-    def generate(self):
-        while not self.is_empty():
-            yield self.pop()
+from infini.exceptions import KeyError
+from infini.typing import Generic, T
+from collections import deque
+
+import heapq
+
+
+class EventQueue(Generic[T]):
+    heap: list
+    entry_finder: dict
+    counter: int
+    order_queue: deque
+
+    def __init__(self) -> None:
+        self.heap = []
+        self.entry_finder = {}
+        self.counter = 0
+        self.order_queue = deque()
+
+    def push(self, priority: int, item: T) -> None:
+        if item in self.entry_finder:
+            self.remove(item)
+        entry = [priority, self.counter, item]
+        self.counter += 1
+        self.entry_finder[item] = entry
+        heapq.heappush(self.heap, entry)
+        self.order_queue.appendleft(item)
+
+    def pop(self) -> T:
+        while self.heap:
+            _, _, item = heapq.heappop(self.heap)
+            if self.entry_finder[item] is not None:
+                del self.entry_finder[item]
+                self.order_queue.remove(item)
+                return item
+        raise KeyError("Event queue is empty.")
+
+    def remove(self, item) -> None:
+        entry = self.entry_finder.pop(item)
+        entry[-1] = None
+
+    def is_empty(self) -> bool:
+        return not bool(self.heap)
+
+    def generate(self):
+        while not self.is_empty():
+            yield self.pop()
```

### Comparing `infini-2.1.8/src/infini/router.py` & `infini-2.1.9/src/infini/router.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from typing import Optional
-from infini.typing import Sequence, Literal, Tuple
-from infini.input import Input
-
-
-class Router:
-    type: Literal["text"] = "text"
-    signs: Tuple[str, ...]
-
-    def __init__(self, sign: str, alias: Sequence[str] = []) -> None:
-        signs = {sign}
-        signs.update(alias)
-        self.signs = tuple(signs)
-
-    def __eq__(self, __router: "Router") -> bool:
-        return __router.type == self.type and __router.signs == self.signs
-
-    def match(self, plain_text: str) -> bool:
-        text = plain_text.strip()
-        return any([text == sign for sign in self.signs])
-
-    @property
-    def namespace(self) -> Optional[str]:
-        return self.signs[0] if self.signs else None
-
-
-class Startswith(Router):
-    name: Literal["startswith"] = "startswith"
-
-    def match(self, plain_text: str) -> bool:
-        text = plain_text.strip()
-        return any([text.startswith(sign) for sign in self.signs])
-
-
-class Contains(Router):
-    name: Literal["contains"] = "contains"
-
-    def match(self, plain_text: str) -> bool:
-        return any([sign in plain_text for sign in self.signs])
-
-
-class Endswith(Router):
-    name: Literal["endswith"] = "endswith"
-
-    def match(self, input: Input) -> bool:
-        text = input.get_plain_text().strip()
-        return any([text.endswith(sign) for sign in self.signs])
-
-
-class Command(Router):
-    name: Literal["command"] = "command"
-    prefix: tuple = (".", "/", "。", "!", "！")
-
-    def match(self, input: Input) -> bool:
-        text = input.get_plain_text().strip()
-        if text.startswith(self.prefix):
-            text = text[1:]
-            return any([text.startswith(sign) for sign in self.signs])
-
-        return False
+from typing import Optional
+from infini.typing import Sequence, Literal, Tuple
+from infini.input import Input
+
+
+class Router:
+    type: Literal["text"] = "text"
+    signs: Tuple[str, ...]
+
+    def __init__(self, sign: str, alias: Sequence[str] = []) -> None:
+        signs = {sign}
+        signs.update(alias)
+        self.signs = tuple(signs)
+
+    def __eq__(self, __router: "Router") -> bool:
+        return __router.type == self.type and __router.signs == self.signs
+
+    def match(self, plain_text: str) -> bool:
+        text = plain_text.strip()
+        return any([text == sign for sign in self.signs])
+
+    @property
+    def namespace(self) -> Optional[str]:
+        return self.signs[0] if self.signs else None
+
+
+class Startswith(Router):
+    name: Literal["startswith"] = "startswith"
+
+    def match(self, plain_text: str) -> bool:
+        text = plain_text.strip()
+        return any([text.startswith(sign) for sign in self.signs])
+
+
+class Contains(Router):
+    name: Literal["contains"] = "contains"
+
+    def match(self, plain_text: str) -> bool:
+        return any([sign in plain_text for sign in self.signs])
+
+
+class Endswith(Router):
+    name: Literal["endswith"] = "endswith"
+
+    def match(self, input: Input) -> bool:
+        text = input.get_plain_text().strip()
+        return any([text.endswith(sign) for sign in self.signs])
+
+
+class Command(Router):
+    name: Literal["command"] = "command"
+    prefix: tuple = (".", "/", "。", "!", "！")
+
+    def match(self, input: Input) -> bool:
+        text = input.get_plain_text().strip()
+        if text.startswith(self.prefix):
+            text = text[1:]
+            return any([text.startswith(sign) for sign in self.signs])
+
+        return False
```

### Comparing `infini-2.1.8/src/infini/typing.py` & `infini-2.1.9/src/infini/typing.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from typing import (
-    TYPE_CHECKING,
-    Dict as Dict,
-    List as List,
-    Any as Any,
-    Tuple as Tuple,
-    Type as Type,
-    Optional as Optional,
-    Generic as Generic,
-    Callable as Callable,
-    Literal as Literal,
-    Sequence as Sequence,
-    Generator as Generator,
-    overload as overload,
-    TypeVar,
-    TypedDict,
-    Union,
-)
-from types import ModuleType as ModuleType, GeneratorType as GeneratorType
-
-if TYPE_CHECKING:
-    from infini.router import Router
-    from infini.input import Input
-    from infini.output import Output
-
-T = TypeVar("T")
-Stream = Union["Input[Any]", "Output"]
-OutputGenerator = Generator["Output", Any, None]
-
-
-class RouterType(TypedDict):
-    priority: int
-    router: "Router"
-    handler: Callable[..., Union[Stream, OutputGenerator]]
+from typing import (
+    TYPE_CHECKING,
+    Dict as Dict,
+    List as List,
+    Any as Any,
+    Tuple as Tuple,
+    Type as Type,
+    Optional as Optional,
+    Generic as Generic,
+    Callable as Callable,
+    Literal as Literal,
+    Sequence as Sequence,
+    Generator as Generator,
+    overload as overload,
+    TypeVar,
+    TypedDict,
+    Union,
+)
+from types import ModuleType as ModuleType, GeneratorType as GeneratorType
+
+if TYPE_CHECKING:
+    from infini.router import Router
+    from infini.input import Input
+    from infini.output import Output
+
+T = TypeVar("T")
+Stream = Union["Input[Any]", "Output"]
+OutputGenerator = Generator["Output", Any, None]
+
+
+class RouterType(TypedDict):
+    priority: int
+    router: "Router"
+    handler: Callable[..., Union[Stream, OutputGenerator]]
```

### Comparing `infini-2.1.8/tests/examples/ndice/src/dicer.py` & `infini-2.1.9/tests/examples/ndice/src/dicer.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,360 +1,360 @@
-from multilogging import multilogger
-from typing import List
-
-import abc
-import re
-import random
-
-
-ZERO = 0
-EMPTY_STRING = ""
-EMPTY_LIST = []
-
-logger = multilogger(name="DicerGirl", payload="Dicer")
-
-
-class BaseDice:
-    def __init__(self, roll_string: str = EMPTY_STRING) -> None:
-        self.roll_string = roll_string
-        self.db = EMPTY_STRING
-        self.outcome = ZERO
-        self.display = EMPTY_LIST
-
-    def __repr__(self) -> str:
-        return self.db.upper()
-
-    @abc.abstractmethod
-    def parse(self) -> "BaseDice":
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def roll(self) -> int:
-        """对骰子进行投掷并给出结果"""
-        raise NotImplementedError
-
-
-class DigitDice(BaseDice):
-    """数字骰"""
-
-    def __init__(self, roll_string: str = EMPTY_STRING) -> None:
-        super().__init__(roll_string=roll_string)
-        if not roll_string.isdigit():
-            raise ValueError
-
-        self.parse()
-
-    def parse(self) -> "DigitDice":
-        self.a = int(self.roll_string)
-        self.b = 1
-        self.db = f"{self.a}"
-        return self
-
-    def roll(self) -> int:
-        self.outcome = self.a
-        self.display = [self.a]
-        return self.outcome
-
-
-class Dice(BaseDice):
-    """多面骰"""
-
-    def __init__(self, roll_string: str = "", explode: bool = False) -> None:
-        super().__init__(roll_string=roll_string)
-        self.dices = EMPTY_LIST
-        self.great = False
-        self.explode = explode
-        self.parse()
-
-    def parse(self) -> "Dice":
-        self.dices = []
-        split = re.split(r"[dD]", self.roll_string)
-
-        if split[0]:
-            self.a = int(split[0])
-        else:
-            self.a = 1
-
-        if split[1]:
-            self.b = int(split[1])
-        else:
-            self.b = 100
-
-        self.db = f"{self.a}D{self.b}"
-        self.dices += [f"D{self.b}"] * self.a
-        return self
-
-    def roll(self) -> int:
-        self.results = []
-        self.display = []
-
-        for _ in range(self.a):
-            result = random.randint(1, self.b)
-
-            if result == 1 and self.explode:
-                result -= 1
-
-            if self.explode and self.b == 8:
-                self.dices.append("D10")
-                result2 = random.randint(1, 10)
-                if result2 == 1:
-                    result -= 1
-                result += result2
-                if result2 == 10:
-                    self.dices.append("D12")
-                    result3 = random.randint(1, 12)
-                    if result3 == 1:
-                        result -= 1
-                    result += result3
-                    if result3 == 12:
-                        self.dices.append("D20")
-                        result4 = random.randint(1, 20)
-                        if result4 == 1:
-                            result -= 1
-                        result += result4
-                        if result4 == 20:
-                            self.great = True
-
-            self.results.append(result)
-            self.display.append(result)
-
-        self.outcome = sum(self.results)
-        return self.outcome
-
-
-class AwardDice(BaseDice):
-    """奖励骰"""
-
-    def __init__(self, roll_string: str = "") -> None:
-        super().__init__(roll_string=roll_string)
-        self.parse()
-
-    def parse(self) -> "AwardDice":
-        split = re.split(r"[bB]", self.roll_string)
-
-        if split[0]:
-            self.a = int(split[0])
-        else:
-            self.a = 1
-
-        self.b = int(split[1])
-        self.db = f"{self.a}B{self.b}"
-        return self
-
-    def roll(self) -> int:
-        self.results = []
-        self.display = []
-
-        for _ in range(self.a):
-            ten = []
-            for _ in range(self.b):
-                outcome = Dice("1d10").roll()
-                outcome = outcome if outcome != 10 else 0
-                ten.append(outcome)
-
-            result = Dice("1d100").roll()
-            ten.append(result // 10)
-            minten = min(ten)
-            ten.remove(result // 10)
-            outcome = minten * 10 + (result % 10)
-            self.results.append(outcome)
-            self.display.append([result, ten])
-
-        self.outcome = sum(self.results)
-        return self.outcome
-
-
-class PunishDice(BaseDice):
-    """惩罚骰"""
-
-    def __init__(self, roll_string: str = "") -> None:
-        super().__init__(roll_string=roll_string)
-        self.parse()
-
-    def parse(self) -> "PunishDice":
-        split = re.split(r"[pP]", self.roll_string)
-
-        if split[0]:
-            self.a = int(split[0])
-        else:
-            self.a = 1
-
-        self.b = int(split[1])
-        self.db = f"{self.a}P{self.b}"
-        return self
-
-    def roll(self) -> int:
-        self.results = []
-        self.display = []
-
-        for _ in range(self.a):
-            ten = []
-            for _ in range(self.b):
-                outcome = Dice("1d10").roll()
-                outcome = outcome if outcome != 10 else 0
-                ten.append(outcome)
-
-            result = Dice("1d100").roll()
-            ten.append(result // 10)
-            maxten = max(ten)
-            ten.remove(result // 10)
-            outcome = maxten * 10 + (result % 10)
-            self.results.append(outcome)
-            self.display.append([result, ten])
-
-        self.outcome = sum(self.results)
-        return self.outcome
-
-
-class Dicer:
-    """掷骰类
-    参数:
-        roll_string: 标准掷骰表达式
-        explode: 是否启用爆炸骰
-    示例:
-        ```python
-        dice = Dice("1d10")
-        dice.roll()
-        print(dice.outcome) # 输出`1d10`投掷结果
-        ```
-    """
-
-    def __init__(self, roll_string: str = EMPTY_STRING, explode: bool = False) -> None:
-        self.roll_string: str = roll_string
-        self.explode: bool = explode
-        self.calc_list: List[str | Dice | DigitDice | AwardDice | PunishDice] = []
-        self.results: List[int] = []
-        self.display: List[int | List[int]] = []
-        self.outcome: int = ZERO
-        self.great: bool = False
-        self.dices: List[str] = []
-
-    def parse(self, roll_string: str = EMPTY_STRING, explode: bool = False):
-        self.roll_string = roll_string if roll_string else self.roll_string
-        self.calc_list = []
-        self.db = EMPTY_STRING
-        matches: List[str] = re.findall(r"\d*[a-zA-Z]\w*|\d+|[-+*/]", self.roll_string)
-
-        for match in matches:
-            if match in ("+", "-", "*", "/", "(", ")"):
-                self.calc_list.append(match)
-                self.db += match
-            elif re.match(r"\d*[dD]\d*", match):
-                self.calc_list.append(Dice(match, explode=explode))
-                self.db += match.upper()
-            elif re.match(r"\d*[bB]\d+", match):
-                self.calc_list.append(AwardDice(match))
-                self.db += match.upper()
-            elif re.match(r"\d*[pP]\d+", match):
-                self.calc_list.append(PunishDice(match))
-                self.db += match.upper()
-            elif re.match(r"\d+", match):
-                self.calc_list.append(DigitDice(match))
-                self.db += match.upper()
-            else:
-                raise ValueError(f"骰 {match} 不符合规范.")
-
-        if not matches:
-            self.calc_list.append(Dice("1d100"))
-            self.db = "1D100"
-
-        return self
-
-    def roll(self):
-        self.parse(roll_string=self.roll_string, explode=self.explode)
-        self.dices = []
-        self.display = []
-        for index, calc in enumerate(self.calc_list):
-            if calc in ("+", "-", "*", "/", "(", ")"):
-                continue
-
-            outcome = calc.roll()
-            self.calc_list[index] = outcome
-            self.results.append(outcome)
-            self.display += calc.display
-
-            if isinstance(calc, Dice) and self.explode:
-                if calc.great:
-                    self.great = True
-
-                self.dices += calc.dices
-
-        self.outcome = eval("".join(map(str, self.calc_list)))
-        return self
-
-    def description(self):
-        def count_integers(lst: list) -> int:
-            count = 0
-            for item in lst:
-                if isinstance(item, int):
-                    count += 1
-                elif isinstance(item, list):
-                    count += count_integers(item)
-            return count
-
-        results = self.display
-        len_display = count_integers(self.display)
-        len_results = count_integers(self.results)
-
-        if len_display <= 10:
-            results = self.display
-        elif len_results <= 10:
-            results = self.results
-        else:
-            results = [...]
-
-        return f"{self.db}={results}={self.outcome}"
-
-    def get_results(self):
-        return self.results
-
-    def detail_expr(self):
-        return str(self.results)
-
-    def calc(self):
-        return self.outcome
-
-    def __repr__(self):
-        return self.db
-
-
-if __name__ == "__main__":
-    # text = "-10/d2/1d10+2d2-22/2+3p2+2b10-p4/b2/d2"
-    # dice = Dicer(text)
-    # print(dice.calc_list)
-    # dice.roll()
-    # print(dice.calc_list)
-    # print(dice.results)
-    # print(dice.outcome)
-    roll_strings = {
-        "1": 1,
-        "10": 10,
-        "100": 100,
-        "-1": -1,
-        "-10": -10,
-        "-100": -100,
-        "1d1": 1,
-        "10d1": 10,
-        "100d1": 100,
-        "10d1+10d1": 20,
-        "10d1-10d1": 0,
-        "10d1+10d1+10d1": 30,
-        "10d1-10d1+10d1": 10,
-        "10d1-10d1-10d1": -10,
-    }
-    for roll_string in roll_strings.keys():
-        try:
-            dice = Dicer().parse(roll_string).roll().roll()
-            if dice.outcome != roll_strings[roll_string]:
-                print(dice.description())
-                raise ValueError(
-                    f"对于 {roll_string} dice.toal={dice.outcome} 但期待 {roll_strings[roll_string]}"
-                )
-        except ValueError as error:
-            logger.exception(error)
-
-    try:
-        roll_string = "d"
-        dice = Dicer(roll_string).roll()
-        print(dice.description())
-    except ValueError as error:
-        logger.exception(error)
+from multilogging import multilogger
+from typing import List
+
+import abc
+import re
+import random
+
+
+ZERO = 0
+EMPTY_STRING = ""
+EMPTY_LIST = []
+
+logger = multilogger(name="DicerGirl", payload="Dicer")
+
+
+class BaseDice:
+    def __init__(self, roll_string: str = EMPTY_STRING) -> None:
+        self.roll_string = roll_string
+        self.db = EMPTY_STRING
+        self.outcome = ZERO
+        self.display = EMPTY_LIST
+
+    def __repr__(self) -> str:
+        return self.db.upper()
+
+    @abc.abstractmethod
+    def parse(self) -> "BaseDice":
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def roll(self) -> int:
+        """对骰子进行投掷并给出结果"""
+        raise NotImplementedError
+
+
+class DigitDice(BaseDice):
+    """数字骰"""
+
+    def __init__(self, roll_string: str = EMPTY_STRING) -> None:
+        super().__init__(roll_string=roll_string)
+        if not roll_string.isdigit():
+            raise ValueError
+
+        self.parse()
+
+    def parse(self) -> "DigitDice":
+        self.a = int(self.roll_string)
+        self.b = 1
+        self.db = f"{self.a}"
+        return self
+
+    def roll(self) -> int:
+        self.outcome = self.a
+        self.display = [self.a]
+        return self.outcome
+
+
+class Dice(BaseDice):
+    """多面骰"""
+
+    def __init__(self, roll_string: str = "", explode: bool = False) -> None:
+        super().__init__(roll_string=roll_string)
+        self.dices = EMPTY_LIST
+        self.great = False
+        self.explode = explode
+        self.parse()
+
+    def parse(self) -> "Dice":
+        self.dices = []
+        split = re.split(r"[dD]", self.roll_string)
+
+        if split[0]:
+            self.a = int(split[0])
+        else:
+            self.a = 1
+
+        if split[1]:
+            self.b = int(split[1])
+        else:
+            self.b = 100
+
+        self.db = f"{self.a}D{self.b}"
+        self.dices += [f"D{self.b}"] * self.a
+        return self
+
+    def roll(self) -> int:
+        self.results = []
+        self.display = []
+
+        for _ in range(self.a):
+            result = random.randint(1, self.b)
+
+            if result == 1 and self.explode:
+                result -= 1
+
+            if self.explode and self.b == 8:
+                self.dices.append("D10")
+                result2 = random.randint(1, 10)
+                if result2 == 1:
+                    result -= 1
+                result += result2
+                if result2 == 10:
+                    self.dices.append("D12")
+                    result3 = random.randint(1, 12)
+                    if result3 == 1:
+                        result -= 1
+                    result += result3
+                    if result3 == 12:
+                        self.dices.append("D20")
+                        result4 = random.randint(1, 20)
+                        if result4 == 1:
+                            result -= 1
+                        result += result4
+                        if result4 == 20:
+                            self.great = True
+
+            self.results.append(result)
+            self.display.append(result)
+
+        self.outcome = sum(self.results)
+        return self.outcome
+
+
+class AwardDice(BaseDice):
+    """奖励骰"""
+
+    def __init__(self, roll_string: str = "") -> None:
+        super().__init__(roll_string=roll_string)
+        self.parse()
+
+    def parse(self) -> "AwardDice":
+        split = re.split(r"[bB]", self.roll_string)
+
+        if split[0]:
+            self.a = int(split[0])
+        else:
+            self.a = 1
+
+        self.b = int(split[1])
+        self.db = f"{self.a}B{self.b}"
+        return self
+
+    def roll(self) -> int:
+        self.results = []
+        self.display = []
+
+        for _ in range(self.a):
+            ten = []
+            for _ in range(self.b):
+                outcome = Dice("1d10").roll()
+                outcome = outcome if outcome != 10 else 0
+                ten.append(outcome)
+
+            result = Dice("1d100").roll()
+            ten.append(result // 10)
+            minten = min(ten)
+            ten.remove(result // 10)
+            outcome = minten * 10 + (result % 10)
+            self.results.append(outcome)
+            self.display.append([result, ten])
+
+        self.outcome = sum(self.results)
+        return self.outcome
+
+
+class PunishDice(BaseDice):
+    """惩罚骰"""
+
+    def __init__(self, roll_string: str = "") -> None:
+        super().__init__(roll_string=roll_string)
+        self.parse()
+
+    def parse(self) -> "PunishDice":
+        split = re.split(r"[pP]", self.roll_string)
+
+        if split[0]:
+            self.a = int(split[0])
+        else:
+            self.a = 1
+
+        self.b = int(split[1])
+        self.db = f"{self.a}P{self.b}"
+        return self
+
+    def roll(self) -> int:
+        self.results = []
+        self.display = []
+
+        for _ in range(self.a):
+            ten = []
+            for _ in range(self.b):
+                outcome = Dice("1d10").roll()
+                outcome = outcome if outcome != 10 else 0
+                ten.append(outcome)
+
+            result = Dice("1d100").roll()
+            ten.append(result // 10)
+            maxten = max(ten)
+            ten.remove(result // 10)
+            outcome = maxten * 10 + (result % 10)
+            self.results.append(outcome)
+            self.display.append([result, ten])
+
+        self.outcome = sum(self.results)
+        return self.outcome
+
+
+class Dicer:
+    """掷骰类
+    参数:
+        roll_string: 标准掷骰表达式
+        explode: 是否启用爆炸骰
+    示例:
+        ```python
+        dice = Dice("1d10")
+        dice.roll()
+        print(dice.outcome) # 输出`1d10`投掷结果
+        ```
+    """
+
+    def __init__(self, roll_string: str = EMPTY_STRING, explode: bool = False) -> None:
+        self.roll_string: str = roll_string
+        self.explode: bool = explode
+        self.calc_list: List[str | Dice | DigitDice | AwardDice | PunishDice] = []
+        self.results: List[int] = []
+        self.display: List[int | List[int]] = []
+        self.outcome: int = ZERO
+        self.great: bool = False
+        self.dices: List[str] = []
+
+    def parse(self, roll_string: str = EMPTY_STRING, explode: bool = False):
+        self.roll_string = roll_string if roll_string else self.roll_string
+        self.calc_list = []
+        self.db = EMPTY_STRING
+        matches: List[str] = re.findall(r"\d*[a-zA-Z]\w*|\d+|[-+*/]", self.roll_string)
+
+        for match in matches:
+            if match in ("+", "-", "*", "/", "(", ")"):
+                self.calc_list.append(match)
+                self.db += match
+            elif re.match(r"\d*[dD]\d*", match):
+                self.calc_list.append(Dice(match, explode=explode))
+                self.db += match.upper()
+            elif re.match(r"\d*[bB]\d+", match):
+                self.calc_list.append(AwardDice(match))
+                self.db += match.upper()
+            elif re.match(r"\d*[pP]\d+", match):
+                self.calc_list.append(PunishDice(match))
+                self.db += match.upper()
+            elif re.match(r"\d+", match):
+                self.calc_list.append(DigitDice(match))
+                self.db += match.upper()
+            else:
+                raise ValueError(f"骰 {match} 不符合规范.")
+
+        if not matches:
+            self.calc_list.append(Dice("1d100"))
+            self.db = "1D100"
+
+        return self
+
+    def roll(self):
+        self.parse(roll_string=self.roll_string, explode=self.explode)
+        self.dices = []
+        self.display = []
+        for index, calc in enumerate(self.calc_list):
+            if calc in ("+", "-", "*", "/", "(", ")"):
+                continue
+
+            outcome = calc.roll()
+            self.calc_list[index] = outcome
+            self.results.append(outcome)
+            self.display += calc.display
+
+            if isinstance(calc, Dice) and self.explode:
+                if calc.great:
+                    self.great = True
+
+                self.dices += calc.dices
+
+        self.outcome = eval("".join(map(str, self.calc_list)))
+        return self
+
+    def description(self):
+        def count_integers(lst: list) -> int:
+            count = 0
+            for item in lst:
+                if isinstance(item, int):
+                    count += 1
+                elif isinstance(item, list):
+                    count += count_integers(item)
+            return count
+
+        results = self.display
+        len_display = count_integers(self.display)
+        len_results = count_integers(self.results)
+
+        if len_display <= 10:
+            results = self.display
+        elif len_results <= 10:
+            results = self.results
+        else:
+            results = [...]
+
+        return f"{self.db}={results}={self.outcome}"
+
+    def get_results(self):
+        return self.results
+
+    def detail_expr(self):
+        return str(self.results)
+
+    def calc(self):
+        return self.outcome
+
+    def __repr__(self):
+        return self.db
+
+
+if __name__ == "__main__":
+    # text = "-10/d2/1d10+2d2-22/2+3p2+2b10-p4/b2/d2"
+    # dice = Dicer(text)
+    # print(dice.calc_list)
+    # dice.roll()
+    # print(dice.calc_list)
+    # print(dice.results)
+    # print(dice.outcome)
+    roll_strings = {
+        "1": 1,
+        "10": 10,
+        "100": 100,
+        "-1": -1,
+        "-10": -10,
+        "-100": -100,
+        "1d1": 1,
+        "10d1": 10,
+        "100d1": 100,
+        "10d1+10d1": 20,
+        "10d1-10d1": 0,
+        "10d1+10d1+10d1": 30,
+        "10d1-10d1+10d1": 10,
+        "10d1-10d1-10d1": -10,
+    }
+    for roll_string in roll_strings.keys():
+        try:
+            dice = Dicer().parse(roll_string).roll().roll()
+            if dice.outcome != roll_strings[roll_string]:
+                print(dice.description())
+                raise ValueError(
+                    f"对于 {roll_string} dice.toal={dice.outcome} 但期待 {roll_strings[roll_string]}"
+                )
+        except ValueError as error:
+            logger.exception(error)
+
+    try:
+        roll_string = "d"
+        dice = Dicer(roll_string).roll()
+        print(dice.description())
+    except ValueError as error:
+        logger.exception(error)
```

### Comparing `infini-2.1.8/tests/examples/ndice/src/ndice.py` & `infini-2.1.9/tests/examples/ndice/src/ndice.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-# Initialized `__init__.py` generated by ipm.
-# Documents at https://ipm.hydroroll.team/
-
-from infini.register import Register
-from infini.router import Startswith
-from infini.input import Input
-from infini.output import Output
-from .dicer import Dicer
-
-import re
-
-register = Register()
-register.register_textevent(
-    "ndice.roll",
-    "[{{ username }}]掷骰: "
-    "{% if descs|length == 1 %}"
-    "{{ descs[0] }}"
-    "{% else %}"
-    "{{ db }}=[...]="
-    "{% for outcome in outcomes %}"
-    "{{ outcome }}"
-    "{% if not loop.last %}, {% endif %}"
-    "{% endfor %}"
-    "{% endif %}",
-)
-register.register_textevent(
-    "ndice.error.bad_roll_string", "[{{ username }}]掷骰时出现异常, 疑似掷骰表达式错误."
-)
-register.register_textevent("ndice.error.too_much_round", "[{{ username }}]给入的掷骰轮数超出预期.")
-register.register_textevent(
-    "ndice.error.unknown",
-    "未知错误: {{ error }}, 可能是掷骰语法异常.\nBUG提交: https://gitee.com/unvisitor/issues",
-)
-register.register_textevent("ndice.error.bad_round", "多轮检定的轮数应当是整型数.")
-register.register_textevent("ndice.error.too_much_round", "多轮检定的轮数超出预期.")
-
-
-def translate_punctuation(string: str) -> str:
-    punctuation_mapping = {
-        "，": ",",
-        "。": ".",
-        "！": "!",
-        "？": "?",
-        "；": ";",
-        "：": ":",
-        "“": '"',
-        "”": '"',
-        "‘": "'",
-        "’": "'",
-        "（": "(",
-        "）": ")",
-        "【": "[",
-        "】": "]",
-        "《": "<",
-        "》": ">",
-    }
-    for ch_punct, en_punct in punctuation_mapping.items():
-        string = string.replace(ch_punct, en_punct)
-    return string
-
-
-def format_str(message: str, begin=None, lower=True) -> str:
-    regex = r"[<\[](.*?)[\]>]"
-    message = str(message).lower() if lower else str(message)
-    msg = translate_punctuation(
-        re.sub("\s+", " ", re.sub(regex, "", message)).strip(" ")
-    )
-    if msg.startswith("/"):
-        msg = "." + msg[1:]
-
-    if begin:
-        if isinstance(begin, str):
-            begin = [
-                begin,
-            ]
-        elif isinstance(begin, tuple):
-            begin = list(begin)
-
-        begin.sort(reverse=True)
-        for b in begin:
-            msg = msg.replace(b, "").lstrip(" ")
-
-    return msg
-
-
-def roll(_: Input, args: str, name: str = None) -> str:
-    time = 1
-    if "#" in args:
-        args = args.split("#")
-
-        try:
-            time = int(args[0].strip())
-            if time > 20:
-                return Output(
-                    "text", "ndice.error.too_much_round", variables={"username": name}
-                )
-        except ValueError:
-            return Output("text", "ndice.error.bad_round", variables={"username": name})
-
-        if len(args) == 1:
-            args = "1d100"
-        else:
-            args = args[1]
-    else:
-        args = args.strip()
-
-    args = args.split()
-    if len(args) > 1:
-        reason = args[1]
-    else:
-        reason = None
-
-    roll_string = args[0]
-    descs = []
-    outcomes = []
-
-    try:
-        dice = Dicer(roll_string).roll()
-        descs.append(dice.description())
-        outcomes.append(dice.outcome)
-
-        for _ in range(time - 1):
-            dice.roll()
-            descs.append(dice.description())
-            outcomes.append(dice.outcome)
-    except ValueError:
-        return Output(
-            "text",
-            "ndice.error.bad_roll_string",
-            status=1,
-            variables={"username": name},
-        )
-
-    return Output(
-        "text",
-        "ndice.roll",
-        variables={
-            "username": name,
-            "descs": descs,
-            "outcomes": outcomes,
-            "db": dice.db,
-        },
-    )
-
-
-@register.handler(router=Startswith(".r"), priority=0)
-def roll_handler(input: Input):
-    args = format_str(input.get_plain_text(), begin=(".r", ".roll"))
-    name = input.variables.get("nickname") or "苏向夜"
-    if not args:
-        return roll(input, "1d100", name=name)
-
-    try:
-        return roll(input, args, name=name)
-    except Exception as error:
-        return Output("text", "ndice.error.unknown", variables={"error": str(error)})
+# Initialized `__init__.py` generated by ipm.
+# Documents at https://ipm.hydroroll.team/
+
+from infini.register import Register
+from infini.router import Startswith
+from infini.input import Input
+from infini.output import Output
+from .dicer import Dicer
+
+import re
+
+register = Register()
+register.register_textevent(
+    "ndice.roll",
+    "[{{ username }}]掷骰: "
+    "{% if descs|length == 1 %}"
+    "{{ descs[0] }}"
+    "{% else %}"
+    "{{ db }}=[...]="
+    "{% for outcome in outcomes %}"
+    "{{ outcome }}"
+    "{% if not loop.last %}, {% endif %}"
+    "{% endfor %}"
+    "{% endif %}",
+)
+register.register_textevent(
+    "ndice.error.bad_roll_string", "[{{ username }}]掷骰时出现异常, 疑似掷骰表达式错误."
+)
+register.register_textevent("ndice.error.too_much_round", "[{{ username }}]给入的掷骰轮数超出预期.")
+register.register_textevent(
+    "ndice.error.unknown",
+    "未知错误: {{ error }}, 可能是掷骰语法异常.\nBUG提交: https://gitee.com/unvisitor/issues",
+)
+register.register_textevent("ndice.error.bad_round", "多轮检定的轮数应当是整型数.")
+register.register_textevent("ndice.error.too_much_round", "多轮检定的轮数超出预期.")
+
+
+def translate_punctuation(string: str) -> str:
+    punctuation_mapping = {
+        "，": ",",
+        "。": ".",
+        "！": "!",
+        "？": "?",
+        "；": ";",
+        "：": ":",
+        "“": '"',
+        "”": '"',
+        "‘": "'",
+        "’": "'",
+        "（": "(",
+        "）": ")",
+        "【": "[",
+        "】": "]",
+        "《": "<",
+        "》": ">",
+    }
+    for ch_punct, en_punct in punctuation_mapping.items():
+        string = string.replace(ch_punct, en_punct)
+    return string
+
+
+def format_str(message: str, begin=None, lower=True) -> str:
+    regex = r"[<\[](.*?)[\]>]"
+    message = str(message).lower() if lower else str(message)
+    msg = translate_punctuation(
+        re.sub("\s+", " ", re.sub(regex, "", message)).strip(" ")
+    )
+    if msg.startswith("/"):
+        msg = "." + msg[1:]
+
+    if begin:
+        if isinstance(begin, str):
+            begin = [
+                begin,
+            ]
+        elif isinstance(begin, tuple):
+            begin = list(begin)
+
+        begin.sort(reverse=True)
+        for b in begin:
+            msg = msg.replace(b, "").lstrip(" ")
+
+    return msg
+
+
+def roll(_: Input, args: str, name: str = None) -> str:
+    time = 1
+    if "#" in args:
+        args = args.split("#")
+
+        try:
+            time = int(args[0].strip())
+            if time > 20:
+                return Output(
+                    "text", "ndice.error.too_much_round", variables={"username": name}
+                )
+        except ValueError:
+            return Output("text", "ndice.error.bad_round", variables={"username": name})
+
+        if len(args) == 1:
+            args = "1d100"
+        else:
+            args = args[1]
+    else:
+        args = args.strip()
+
+    args = args.split()
+    if len(args) > 1:
+        reason = args[1]
+    else:
+        reason = None
+
+    roll_string = args[0]
+    descs = []
+    outcomes = []
+
+    try:
+        dice = Dicer(roll_string).roll()
+        descs.append(dice.description())
+        outcomes.append(dice.outcome)
+
+        for _ in range(time - 1):
+            dice.roll()
+            descs.append(dice.description())
+            outcomes.append(dice.outcome)
+    except ValueError:
+        return Output(
+            "text",
+            "ndice.error.bad_roll_string",
+            status=1,
+            variables={"username": name},
+        )
+
+    return Output(
+        "text",
+        "ndice.roll",
+        variables={
+            "username": name,
+            "descs": descs,
+            "outcomes": outcomes,
+            "db": dice.db,
+        },
+    )
+
+
+@register.handler(router=Startswith(".r"), priority=0)
+def roll_handler(input: Input):
+    args = format_str(input.get_plain_text(), begin=(".r", ".roll"))
+    name = input.variables.get("nickname") or "苏向夜"
+    if not args:
+        return roll(input, "1d100", name=name)
+
+    try:
+        return roll(input, args, name=name)
+    except Exception as error:
+        return Output("text", "ndice.error.unknown", variables={"error": str(error)})
```

### Comparing `infini-2.1.8/tests/test_core.py` & `infini-2.1.9/tests/test_core.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from infini.core import Core
-from infini.generator import Generator
-from infini.handler import Handler
-from infini.injector import Injector
-from infini.input import Input
-from infini.interceptor import Interceptor
-from infini.output import Output
-from infini.router import Contains, Startswith
-
-
-def test_core():
-    command_input = Input(".add 1 2")
-    intercepted_input = Input("这个人叫简律纯.")
-    valid_input = Input("这个叫苏向夜.")
-    command_and_valid_input = Input(".echo 苏向夜打爆了简某人的狗头")
-
-    def intercept_jianlvchun(_: Input) -> Input | Output:
-        return Output("text", "block.jianlvchun", block=True)  # TODO 拦截器阻塞标识
-
-    interceptor = Interceptor()
-    interceptor.interceptors = [
-        {
-            "priority": 1,
-            "router": Contains("简律纯"),
-            "handler": intercept_jianlvchun,
-        }
-    ]
-
-    def add(input: Input) -> Output:
-        result = str(sum(list(map(int, input.get_plain_text().lstrip(".add").split()))))
-        return Output("text", "test.add", block=False, variables={"result": result})
-
-    def cmd(_: Input) -> Output:
-        return Output("text", "test.cmd", block=False)
-
-    handler = Handler()
-    handler.handlers = [
-        {
-            "priority": 2,
-            "router": Startswith(".add"),
-            "handler": add,
-        },
-        {
-            "priority": 1,
-            "router": Startswith("."),
-            "handler": cmd,
-        },
-    ]
-
-    generator = Generator()
-    generator.events = {
-        "test.cmd": "cmd",
-        "test.add": "{{ result }}",
-        "block.jianlvchun": "检测到违禁词",
-    }
-    generator.global_variables = {}
-
-    core = Core()
-    core.handler = handler
-    core.interceptor = interceptor
-    core.pre_interceptor = interceptor
-    core.generator = generator
-    core.injector = Injector()
-
-    outputs = set()
-    for output in core.input(command_input):
-        outputs.add(output)
-    assert outputs == {"cmd", "3"}
-
-    count = 0
-    for _ in core.input(valid_input):
-        count += 1
-    assert count == 0
-
-    for output in core.input(intercepted_input):
-        assert output == "检测到违禁词"
-
-    outputs = set()
-    for output in core.input(command_and_valid_input):
-        outputs.add(output)
-    assert outputs == {"cmd"}
+from infini.core import Core
+from infini.generator import Generator
+from infini.handler import Handler
+from infini.injector import Injector
+from infini.input import Input
+from infini.interceptor import Interceptor
+from infini.output import Output
+from infini.router import Contains, Startswith
+
+
+def test_core():
+    command_input = Input(".add 1 2")
+    intercepted_input = Input("这个人叫简律纯.")
+    valid_input = Input("这个叫苏向夜.")
+    command_and_valid_input = Input(".echo 苏向夜打爆了简某人的狗头")
+
+    def intercept_jianlvchun(_: Input) -> Input | Output:
+        return Output("text", "block.jianlvchun", block=True)  # TODO 拦截器阻塞标识
+
+    interceptor = Interceptor()
+    interceptor.interceptors = [
+        {
+            "priority": 1,
+            "router": Contains("简律纯"),
+            "handler": intercept_jianlvchun,
+        }
+    ]
+
+    def add(input: Input) -> Output:
+        result = str(sum(list(map(int, input.get_plain_text().lstrip(".add").split()))))
+        return Output("text", "test.add", block=False, variables={"result": result})
+
+    def cmd(_: Input) -> Output:
+        return Output("text", "test.cmd", block=False)
+
+    handler = Handler()
+    handler.handlers = [
+        {
+            "priority": 2,
+            "router": Startswith(".add"),
+            "handler": add,
+        },
+        {
+            "priority": 1,
+            "router": Startswith("."),
+            "handler": cmd,
+        },
+    ]
+
+    generator = Generator()
+    generator.events = {
+        "test.cmd": "cmd",
+        "test.add": "{{ result }}",
+        "block.jianlvchun": "检测到违禁词",
+    }
+    generator.global_variables = {}
+
+    core = Core()
+    core.handler = handler
+    core.interceptor = interceptor
+    core.pre_interceptor = interceptor
+    core.generator = generator
+    core.injector = Injector()
+
+    outputs = set()
+    for output in core.input(command_input):
+        outputs.add(output)
+    assert outputs == {"cmd", "3"}
+
+    count = 0
+    for _ in core.input(valid_input):
+        count += 1
+    assert count == 0
+
+    for output in core.input(intercepted_input):
+        assert output == "检测到违禁词"
+
+    outputs = set()
+    for output in core.input(command_and_valid_input):
+        outputs.add(output)
+    assert outputs == {"cmd"}
```

### Comparing `infini-2.1.8/tests/test_input.py` & `infini-2.1.9/tests/test_input.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from infini.input import Input
-
-
-def test_new_input_without_vars():
-    assert Input("test plain_str").plain_data == "test plain_str"
-    assert Input("test plain_str").get_plain_text() == "test plain_str"
-
-
-def test_new_input_with_session_id():
-    input = Input("test plain_str", variables={"session_id": "test"})
-    assert input.get_session_id() == "test"
-
-
-def test_new_input_without_session_id():
-    input = Input("test plain_str", variables={"user_id": "test"})
-    assert input.get_session_id() == "test"
+from infini.input import Input
+
+
+def test_new_input_without_vars():
+    assert Input("test plain_str").plain_data == "test plain_str"
+    assert Input("test plain_str").get_plain_text() == "test plain_str"
+
+
+def test_new_input_with_session_id():
+    input = Input("test plain_str", variables={"session_id": "test"})
+    assert input.get_session_id() == "test"
+
+
+def test_new_input_without_session_id():
+    input = Input("test plain_str", variables={"user_id": "test"})
+    assert input.get_session_id() == "test"
```

### Comparing `infini-2.1.8/tests/test_register.py` & `infini-2.1.9/tests/test_register.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from infini.core import Core
-from infini.generator import Generator
-from infini.handler import Handler
-from infini.injector import Injector
-from infini.input import Input
-from infini.interceptor import Interceptor
-from infini.output import Output
-from infini.register import Register
-
-
-def test_register():
-    blocked_god_input = Input("这是苏向夜的杰作.")
-    snh_input = Input("撅少年狐!")
-
-    register = Register()
-
-    @register.pre_interceptor("苏向夜", priority=0)
-    def test_pre_interceptor(_: Input):
-        return Output("text", "block.sxy", block=True)
-
-    @register.handler("撅少年狐")
-    def test_handler(_: Input):
-        return Output("text", "block.snh", block=True)
-
-    register.register_textevent("block.sxy", "不可直呼{{ sxy_id }}的ID")
-    register.register_textevent("block.snh", "不许撅{{ get_snh_id }}")
-
-    register.register_variable("sxy_id", "苏向夜")
-
-    @register.dynamic_variable()
-    def get_snh_id():
-        return "少年狐"
-
-    @register.interceptor("苏向夜", priority=0)
-    def test_interceptor(_: Input):
-        return Output("text", "block.sxy", block=True)
-
-    pre_interceptor = Interceptor()
-    pre_interceptor.interceptors = register.pre_interceptors
-    handler = Handler()
-    handler.handlers = register.handlers
-    generator = Generator()
-    generator.events = register.events
-    generator.global_variables = register.global_variables
-    interceptor = Interceptor()
-    interceptor.interceptors = register.interceptors
-
-    core = Core()
-    core.pre_interceptor = pre_interceptor
-    core.handler = handler
-    core.generator = generator
-    core.interceptor = interceptor
-    core.injector = Injector()
-
-    for output in core.input(blocked_god_input):
-        assert output == "不可直呼苏向夜的ID"
-
-    for output in core.input(snh_input):
-        assert output == "不许撅少年狐"
+from infini.core import Core
+from infini.generator import Generator
+from infini.handler import Handler
+from infini.injector import Injector
+from infini.input import Input
+from infini.interceptor import Interceptor
+from infini.output import Output
+from infini.register import Register
+
+
+def test_register():
+    blocked_god_input = Input("这是苏向夜的杰作.")
+    snh_input = Input("撅少年狐!")
+
+    register = Register()
+
+    @register.pre_interceptor("苏向夜", priority=0)
+    def test_pre_interceptor(_: Input):
+        return Output("text", "block.sxy", block=True)
+
+    @register.handler("撅少年狐")
+    def test_handler(_: Input):
+        return Output("text", "block.snh", block=True)
+
+    register.register_textevent("block.sxy", "不可直呼{{ sxy_id }}的ID")
+    register.register_textevent("block.snh", "不许撅{{ get_snh_id }}")
+
+    register.register_variable("sxy_id", "苏向夜")
+
+    @register.dynamic_variable()
+    def get_snh_id():
+        return "少年狐"
+
+    @register.interceptor("苏向夜", priority=0)
+    def test_interceptor(_: Input):
+        return Output("text", "block.sxy", block=True)
+
+    pre_interceptor = Interceptor()
+    pre_interceptor.interceptors = register.pre_interceptors
+    handler = Handler()
+    handler.handlers = register.handlers
+    generator = Generator()
+    generator.events = register.events
+    generator.global_variables = register.global_variables
+    interceptor = Interceptor()
+    interceptor.interceptors = register.interceptors
+
+    core = Core()
+    core.pre_interceptor = pre_interceptor
+    core.handler = handler
+    core.generator = generator
+    core.interceptor = interceptor
+    core.injector = Injector()
+
+    for output in core.input(blocked_god_input):
+        assert output == "不可直呼苏向夜的ID"
+
+    for output in core.input(snh_input):
+        assert output == "不许撅少年狐"
```

### Comparing `infini-2.1.8/PKG-INFO` & `infini-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini
-Version: 2.1.8
+Version: 2.1.9
 Summary: Infini 内容输入输出流框架
 Author-Email: 苏向夜 <fu050409@163.com>, 简律纯 <leader@hydroroll.team>
 License: MIT
 Project-URL: Homepage, https://grps.hydroroll.team
 Project-URL: Documentation, https://grps.hydroroll.team
 Project-URL: Repository, https://github.com/HydroRoll-Team/infini
 Project-URL: Changelog, https://infini.hydroroll.team/zh_CN/latest/changelog.html
```

