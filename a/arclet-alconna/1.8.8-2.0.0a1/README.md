# Comparing `tmp/arclet_alconna-1.8.8.tar.gz` & `tmp/arclet_alconna-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet_alconna-1.8.8.tar", last modified: Thu Apr 11 17:10:46 2024, max compression
+gzip compressed data, was "arclet_alconna-2.0.0a1.tar", last modified: Thu Oct  5 04:53:48 2023, max compression
```

## Comparing `arclet_alconna-1.8.8.tar` & `arclet_alconna-2.0.0a1.tar`

### file list

```diff
@@ -1,42 +1,39 @@
--rw-r--r--   0        0        0     1070 2024-04-11 17:10:20.804547 arclet_alconna-1.8.8/LICENSE
--rw-r--r--   0        0        0     6917 2024-04-11 17:10:20.804547 arclet_alconna-1.8.8/README-EN.md
--rw-r--r--   0        0        0     3231 2024-04-11 17:10:46.808843 arclet_alconna-1.8.8/pyproject.toml
--rw-r--r--   0        0        0     2263 2024-04-11 17:10:20.804547 arclet_alconna-1.8.8/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 17:10:20.804547 arclet_alconna-1.8.8/src/arclet/alconna/_internal/__init__.py
--rw-r--r--   0        0        0    17814 2024-04-11 17:10:20.804547 arclet_alconna-1.8.8/src/arclet/alconna/_internal/_analyser.py
--rw-r--r--   0        0        0    11046 2024-04-11 17:10:20.804547 arclet_alconna-1.8.8/src/arclet/alconna/_internal/_argv.py
--rw-r--r--   0        0        0    33623 2024-04-11 17:10:20.804547 arclet_alconna-1.8.8/src/arclet/alconna/_internal/_handlers.py
--rw-r--r--   0        0        0    13446 2024-04-11 17:10:20.804547 arclet_alconna-1.8.8/src/arclet/alconna/_internal/_header.py
--rw-r--r--   0        0        0     1292 2024-04-11 17:10:20.804547 arclet_alconna-1.8.8/src/arclet/alconna/_internal/_util.py
--rw-r--r--   0        0        0     1487 2024-04-11 17:10:20.804547 arclet_alconna-1.8.8/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    15562 2024-04-11 17:10:20.804547 arclet_alconna-1.8.8/src/arclet/alconna/args.py
--rw-r--r--   0        0        0     1471 2024-04-11 17:10:20.804547 arclet_alconna-1.8.8/src/arclet/alconna/argv.py
--rw-r--r--   0        0        0    16397 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0    13219 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     2768 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     7309 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/completion.py
--rw-r--r--   0        0        0     4661 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/config.py
--rw-r--r--   0        0        0      361 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/constraint.py
--rw-r--r--   0        0        0    16745 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     1955 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1187 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0    11408 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0       91 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/i18n/.config.json
--rw-r--r--   0        0        0     3801 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/i18n/en-US.json
--rw-r--r--   0        0        0     3866 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0    19400 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1451 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1883 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     3828 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/output.py
--rw-r--r--   0        0        0        0 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/py.typed
--rw-r--r--   0        0        0     5654 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     6876 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0     3096 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/tests/analyser_test.py
--rw-r--r--   0        0        0     9866 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/tests/args_test.py
--rw-r--r--   0        0        0     2115 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/tests/base_test.py
--rw-r--r--   0        0        0     2981 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/tests/components_test.py
--rw-r--r--   0        0        0     1251 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/tests/config_test.py
--rw-r--r--   0        0        0    35416 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/tests/core_test.py
--rw-r--r--   0        0        0     4569 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/tests/devtool.py
--rw-r--r--   0        0        0      489 2024-04-11 17:10:20.808547 arclet_alconna-1.8.8/tests/util_test.py
--rw-r--r--   0        0        0     7983 1970-01-01 00:00:00.000000 arclet_alconna-1.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet_alconna-2.0.0a1/LICENSE
+-rw-r--r--   0        0        0     6644 2023-06-30 14:51:14.232836 arclet_alconna-2.0.0a1/README-EN.md
+-rw-r--r--   0        0        0     2778 2023-10-05 04:53:48.741623 arclet_alconna-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2056 2023-10-05 04:17:04.334663 arclet_alconna-2.0.0a1/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:37:15.106361 arclet_alconna-2.0.0a1/src/arclet/alconna/_internal/__init__.py
+-rw-r--r--   0        0        0    16338 2023-10-05 04:40:02.551714 arclet_alconna-2.0.0a1/src/arclet/alconna/_internal/_analyser.py
+-rw-r--r--   0        0        0     7683 2023-10-05 04:45:03.171383 arclet_alconna-2.0.0a1/src/arclet/alconna/_internal/_argv.py
+-rw-r--r--   0        0        0    25104 2023-10-05 04:48:39.631253 arclet_alconna-2.0.0a1/src/arclet/alconna/_internal/_handlers.py
+-rw-r--r--   0        0        0    10453 2023-10-05 04:16:23.518204 arclet_alconna-2.0.0a1/src/arclet/alconna/_internal/_header.py
+-rw-r--r--   0        0        0     1333 2023-06-08 08:47:20.886467 arclet_alconna-2.0.0a1/src/arclet/alconna/_internal/_util.py
+-rw-r--r--   0        0        0     1543 2023-05-25 16:37:15.110384 arclet_alconna-2.0.0a1/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    15030 2023-10-05 04:49:27.843900 arclet_alconna-2.0.0a1/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0     1507 2023-10-05 03:03:45.599472 arclet_alconna-2.0.0a1/src/arclet/alconna/argv.py
+-rw-r--r--   0        0        0    15738 2023-10-05 04:40:02.539706 arclet_alconna-2.0.0a1/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0    12146 2023-10-05 03:31:12.296748 arclet_alconna-2.0.0a1/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     1889 2023-10-05 03:03:28.648317 arclet_alconna-2.0.0a1/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     4867 2023-05-25 16:37:15.116360 arclet_alconna-2.0.0a1/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     4361 2023-10-05 04:34:55.472081 arclet_alconna-2.0.0a1/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0    14228 2023-10-05 03:03:45.603427 arclet_alconna-2.0.0a1/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0        0 2023-10-05 03:04:22.242167 arclet_alconna-2.0.0a1/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1009 2023-05-25 16:37:15.119359 arclet_alconna-2.0.0a1/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0     8060 2023-10-05 04:51:35.839745 arclet_alconna-2.0.0a1/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0       99 2023-05-21 05:43:33.502836 arclet_alconna-2.0.0a1/src/arclet/alconna/i18n/.config.json
+-rw-r--r--   0        0        0     3695 2023-10-05 03:03:45.607390 arclet_alconna-2.0.0a1/src/arclet/alconna/i18n/en-US.json
+-rw-r--r--   0        0        0     3745 2023-10-05 03:03:45.608390 arclet_alconna-2.0.0a1/src/arclet/alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0    18555 2023-10-05 03:03:45.610392 arclet_alconna-2.0.0a1/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1270 2023-10-05 03:40:45.309156 arclet_alconna-2.0.0a1/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1696 2023-10-05 03:40:45.318155 arclet_alconna-2.0.0a1/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     3940 2023-05-25 16:37:15.124599 arclet_alconna-2.0.0a1/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-05-21 05:43:33.513926 arclet_alconna-2.0.0a1/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     4686 2023-10-05 04:21:47.285271 arclet_alconna-2.0.0a1/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0     3246 2023-05-25 16:37:15.127191 arclet_alconna-2.0.0a1/tests/analyser_test.py
+-rw-r--r--   0        0        0     8880 2023-10-05 03:03:45.614389 arclet_alconna-2.0.0a1/tests/args_test.py
+-rw-r--r--   0        0        0     2167 2023-05-25 16:37:15.128711 arclet_alconna-2.0.0a1/tests/base_test.py
+-rw-r--r--   0        0        0     3119 2023-06-08 08:47:20.892467 arclet_alconna-2.0.0a1/tests/components_test.py
+-rw-r--r--   0        0        0     1199 2023-05-25 16:37:15.130711 arclet_alconna-2.0.0a1/tests/config_test.py
+-rw-r--r--   0        0        0    28539 2023-10-05 03:03:45.615394 arclet_alconna-2.0.0a1/tests/core_test.py
+-rw-r--r--   0        0        0      505 2023-05-25 16:37:15.132710 arclet_alconna-2.0.0a1/tests/util_test.py
+-rw-r--r--   0        0        0     7476 1970-01-01 00:00:00.000000 arclet_alconna-2.0.0a1/PKG-INFO
```

### Comparing `arclet_alconna-1.8.8/README-EN.md` & `arclet_alconna-2.0.0a1/README-EN.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,249 +1,238 @@
-![](https://socialify.git.ci/ArcletProject/Alconna/image?description=1&descriptionEditable=A%20High-performance%2C%20Generality%2C%20Humane%20Command%20Line%20Arguments%20Parser%20Library.&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Farclet.top%2Fimg%2Farclet.png&name=1&owner=1&pattern=Brick%20Wall&stargazers=1&theme=Auto)
-<div align="center"> 
-
-# Alconna
-
-</div>
-
-![Alconna](https://img.shields.io/badge/Arclet-Alconna-2564c2.svg)
-![latest release](https://img.shields.io/github/release/ArcletProject/Alconna)
-[![Licence](https://img.shields.io/github/license/ArcletProject/Alconna)](https://github.com/ArcletProject/Alconna/blob/master/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/arclet-alconna)](https://pypi.org/project/arclet-alconna)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arclet-alconna)](https://www.python.org/)
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FArcletProject%2FAlconna.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FArcletProject%2FAlconna?ref=badge_shield)
-
-[**简体中文**](README.md)|[**English**](README-EN.md)
-
-## About
-
-`Alconna` is a powerful cli tool for parsing message chain or other raw message data. It is an overload version of `CommandAnalysis`, affiliated to `ArcletProject`.
-
-`Alconna` has a large number of built-in components and complex parsing functions. ~~But do not afraid~~, you can use it as a simple command parser.
-
-## Installation
-
-pip
-```shell
-$ pip install --upgrade arclet-alconna
-$ pip install --upgrade arclet-alconna[full]
-```
-
-## Documentation
-
-Official Document : [👉Link](https://arclet.top/docs/tutorial/alconna)
-
-Relevant Document : [📚Docs](https://graiax.cn/guide/message_parser/alconna.html)
-
-## A Simple Example
-
-```python
-from arclet.alconna import Alconna, Option, Subcommand, Args
-
-cmd = Alconna(
-    "/pip",
-    Subcommand("install", Option("-u|--upgrade"), Args.pak_name[str]),
-    Option("list")
-)
-
-result = cmd.parse("/pip install numpy --upgrade") # This method returns an 'Arparma' class instance.
-print(result.query('install'))  # Or result.install
-```
-
-Output as follows:
-```
-value=None args={'pak_name': 'numpy'} options={'upgrade': value=Ellipsis args={}} subcommands={}
-```
-
-## Communication
-
-QQ Group: [Link](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
-
-## Features
-
-* High Performance. On i5-10210U, performance is about `71000~289000 msg/s`; test script: [benchmark](benchmark.py)
-* Intuitive way to create command components
-* Powerful Automatic Type Parse and Conversion
-* Customizable Help Text Formatter and Control of Command Analyser
-* i18n Support
-* Cache of input command for quick response of repeated command
-* Easy-to-use Construct and Usage of Command Shortcut
-* Can bind callback function to execute after command parsing
-* Can create command completion session to implement multi-round continuous completion prompt
-* Various Features (FuzzyMatch, Output Capture, etc.)
-
-Example of Callback Executor:
-
-```python
-# callback.py
-from arclet.alconna import Alconna, Args
-
-alc = Alconna("callback", Args["foo", int]["bar", str])
-
-@alc.bind()
-def callback(foo: int, bar: str):
-    print(f"foo: {foo}")
-    print(f"bar: {bar}")
-    print(bar * foo)
-    
-if __name__ == "__main__":
-    alc()
-```
-
-```shell
-$ python callback.py 3 hello
-foo: 3
-bar: hello
-hellohellohello
-```
-
-
-Example of Type Conversion:
-
-```python
-from arclet.alconna import Alconna, Args
-from pathlib import Path
-
-read = Alconna("read", Args["data", bytes])
-
-@read.bind()
-def cb(data: bytes):
-    print(type(data))
-
-read.parse(["read", b'hello'])
-read.parse("read test_fire.py")
-read.parse(["read", Path("test_fire.py")])
-
-'''
-<class 'bytes'>
-<class 'bytes'>
-<class 'bytes'>
-'''
-```
-
-Example of Component creation:
-```python
-# component.py
-from arclet.alconna import Alconna, Args, Option, Subcommand, store_true, count, append
-
-alc = Alconna(
-    "component",
-    Args["path", str],
-    Option("--verbose|-v", action=count),
-    Option("-f", Args["flag", str], compact=True, action=append),
-    Subcommand("sub", Option("bar", action=store_true, default=False))
-)
-
-if __name__ == '__main__':
-    res = alc()
-    print(res.query("path"))
-    print(res.query("verbose.value"))
-    print(res.query("f.flag"))
-    print(res.query("sub"))
-```
-
-```shell
-$ python component.py /home/arclet -vvvv -f1 -f2 -f3 sub bar
-/home/arclet
-4
-['1', '2', '3']
-(value=Ellipsis args={} options={'bar': (value=True args={})} subcommands={})
-```
-
-Example of Command Shortcut:
-```python
-# shortcut.py
-from arclet.alconna import Alconna, Args
-
-alc = Alconna("eval", Args["content", str])
-alc.shortcut("echo", {"command": "eval print(\\'{*}\\')"})
-
-@alc.bind()
-def cb(content: str):
-    eval(content, {}, {})
-
-if __name__ == '__main__':
-    alc()
-```
-
-```shell
-$ python shortcut.py eval print(\"hello world\")
-hello world
-$ python shortcut.py echo hello world!
-hello world!
-```
-
-Example of Command Completion:
-```python
-# completion.py
-from arclet.alconna import Alconna, Args, Option
-
-alc = Alconna("complete", Args["bar", int]) + Option("foo") + Option("fool")
-
-if __name__ == "__main__":
-    alc()
-```
-
-```shell
-$ python completion.py ?
-suggest input follows:
-* bar: int
-* --help
-* -h
-* foo
-* fool
-```
-
-Example of `typing` Support:
-```python
-from typing import Annotated  # or typing_extensions.Annotated
-from arclet.alconna import Alconna, Args
-
-alc = Alconna("test", Args.foo[Annotated[int, lambda x: x % 2 == 0]])
-alc.parse("test 2")
-alc.parse("test 3")
-
-'''
-'foo': 2
-ParamsUnmatched: param 3 is incorrect
-'''
-```
-
-Example of FuzzyMatch:
-
-```python
-# fuzzy.py
-from arclet.alconna import Alconna, CommandMeta, Arg
-
-alc = Alconna('!test_fuzzy', Arg("foo", str), meta=CommandMeta(fuzzy_match=True))
-
-if __name__ == "__main__":
-    alc()
-
-```
-
-```shell
-$ python fuzzy.py /test_fuzzy foo bar
-/test_fuzy not matched. Are you mean "!test_fuzzy"?
-```
-
-## Examples
-
-| Name           | File                                     |
-|----------------|------------------------------------------|
-| Calculate      | [calculate.py](./example/calculate.py)   |
-| Execute        | [exec_code.py](./example/exec_code.py)   |
-| Request Route  | [endpoint.py](./example/endpoint.py)     |
-| Image Search   | [img_search.py](./example/img_search.py) |
-| PIP            | [pip.py](./example/pip.py)               |
-| Database Query | [exec_sql.py](./example/exec_sql.py)     |
-
-## License
-
-Alconna is licensed under the [MIT License](LICENSE).
-
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FArcletProject%2FAlconna.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FArcletProject%2FAlconna?ref=badge_large)
-
-## Acknowledgement
-
-[JetBrains](https://www.jetbrains.com/): Support Authorize for [PyCharm](https://www.jetbrains.com/pycharm/)<br>
+![](https://socialify.git.ci/ArcletProject/Alconna/image?description=1&descriptionEditable=A%20High-performance%2C%20Generality%2C%20Humane%20Command%20Line%20Arguments%20Parser%20Library.&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Farclet.top%2Fimg%2Farclet.png&name=1&owner=1&pattern=Brick%20Wall&stargazers=1&theme=Auto)
+<div align="center"> 
+
+# Alconna
+
+</div>
+
+![Alconna](https://img.shields.io/badge/Arclet-Alconna-2564c2.svg)
+![latest release](https://img.shields.io/github/release/ArcletProject/Alconna)
+[![Licence](https://img.shields.io/github/license/ArcletProject/Alconna)](https://github.com/ArcletProject/Alconna/blob/master/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/arclet-alconna)](https://pypi.org/project/arclet-alconna)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arclet-alconna)](https://www.python.org/)
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FArcletProject%2FAlconna.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FArcletProject%2FAlconna?ref=badge_shield)
+
+[**简体中文**](README.md)|[**English**](README-EN.md)
+
+## About
+
+`Alconna` is a powerful cli tool for parsing message chain or other raw message data. It is an overload version of `CommandAnalysis`, affiliated to `ArcletProject`.
+
+`Alconna` has a large number of built-in components and complex parsing functions. ~~But do not afraid~~, you can use it as a simple command parser.
+
+## Installation
+
+pip
+```shell
+$ pip install --upgrade arclet-alconna
+$ pip install --upgrade arclet-alconna[full]
+```
+
+## Documentation
+
+Official Document : [👉Link](https://arclet.top/docs/tutorial/alconna)
+
+Relevant Document : [📚Docs](https://graiax.cn/guide/message_parser/alconna.html)
+
+## A Simple Example
+
+```python
+from arclet.alconna import Alconna, Option, Subcommand, Args
+
+cmd = Alconna(
+    "/pip",
+    Subcommand("install", Option("-u|--upgrade"), Args.pak_name[str]),
+    Option("list")
+)
+
+result = cmd.parse("/pip install numpy --upgrade") # This method returns an 'Arparma' class instance.
+print(result.query('install'))  # Or result.install
+```
+
+Output as follows:
+```
+value=None args={'pak_name': 'numpy'} options={'upgrade': value=Ellipsis args={}} subcommands={}
+```
+
+## Communication
+
+QQ Group: [Link](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
+
+## Features
+
+* High Performance. On i5-10210U, performance is about `71000~289000 msg/s`; test script: [benchmark](benchmark.py)
+* Intuitive way to create command components
+* Powerful Automatic Type Parse and Conversion
+* Customizable Help Text Formatter and Control of Command Analyser
+* i18n Support
+* Cache of input command for quick response of repeated command
+* Easy-to-use Construct and Usage of Command Shortcut
+* Can bind callback function to execute after command parsing
+* Can create command completion session to implement multi-round continuous completion prompt
+* Various Features (FuzzyMatch, Output Capture, etc.)
+
+Example of Callback Executor:
+
+```python
+# callback.py
+from arclet.alconna import Alconna, Args
+
+alc = Alconna("callback", Args["foo", int]["bar", str])
+
+@alc.bind()
+def callback(foo: int, bar: str):
+    print(f"foo: {foo}")
+    print(f"bar: {bar}")
+    print(bar * foo)
+    
+if __name__ == "__main__":
+    alc()
+```
+
+```shell
+$ python callback.py 3 hello
+foo: 3
+bar: hello
+hellohellohello
+```
+
+
+Example of Type Conversion:
+
+```python
+from arclet.alconna import Alconna, Args
+from pathlib import Path
+
+read = Alconna("read", Args["data", bytes])
+
+@read.bind()
+def cb(data: bytes):
+    print(type(data))
+
+read.parse(["read", b'hello'])
+read.parse("read test_fire.py")
+read.parse(["read", Path("test_fire.py")])
+
+'''
+<class 'bytes'>
+<class 'bytes'>
+<class 'bytes'>
+'''
+```
+
+Example of Component creation:
+```python
+# component.py
+from arclet.alconna import Alconna, Args, Option, Subcommand, store_true, count, append
+
+alc = Alconna(
+    "component",
+    Args["path", str],
+    Option("--verbose|-v", action=count),
+    Option("-f", Args["flag", str], compact=True, action=append),
+    Subcommand("sub", Option("bar", action=store_true, default=False))
+)
+
+if __name__ == '__main__':
+    res = alc()
+    print(res.query("path"))
+    print(res.query("verbose.value"))
+    print(res.query("f.flag"))
+    print(res.query("sub"))
+```
+
+```shell
+$ python component.py /home/arclet -vvvv -f1 -f2 -f3 sub bar
+/home/arclet
+4
+['1', '2', '3']
+(value=Ellipsis args={} options={'bar': (value=True args={})} subcommands={})
+```
+
+Example of Command Shortcut:
+```python
+# shortcut.py
+from arclet.alconna import Alconna, Args
+
+alc = Alconna("eval", Args["content", str])
+alc.shortcut("echo", {"command": "eval print(\\'{*}\\')"})
+
+@alc.bind()
+def cb(content: str):
+    eval(content, {}, {})
+
+if __name__ == '__main__':
+    alc()
+```
+
+```shell
+$ python shortcut.py eval print(\"hello world\")
+hello world
+$ python shortcut.py echo hello world!
+hello world!
+```
+
+Example of Command Completion:
+```python
+# completion.py
+from arclet.alconna import Alconna, Args, Option
+
+alc = Alconna("complete", Args["bar", int]) + Option("foo") + Option("fool")
+
+if __name__ == "__main__":
+    alc()
+```
+
+```shell
+$ python completion.py ?
+suggest input follows:
+* bar: int
+* --help
+* -h
+* foo
+* fool
+```
+
+Example of `typing` Support:
+```python
+from typing import Annotated  # or typing_extensions.Annotated
+from arclet.alconna import Alconna, Args
+
+alc = Alconna("test", Args.foo[Annotated[int, lambda x: x % 2 == 0]])
+alc.parse("test 2")
+alc.parse("test 3")
+
+'''
+'foo': 2
+ParamsUnmatched: param 3 is incorrect
+'''
+```
+
+Example of FuzzyMatch:
+
+```python
+# fuzzy.py
+from arclet.alconna import Alconna, CommandMeta, Arg
+
+alc = Alconna('!test_fuzzy', Arg("foo", str), meta=CommandMeta(fuzzy_match=True))
+
+if __name__ == "__main__":
+    alc()
+
+```
+
+```shell
+$ python fuzzy.py /test_fuzzy foo bar
+/test_fuzy not matched. Are you mean "!test_fuzzy"?
+```
+
+## License
+
+Alconna is licensed under the [MIT License](LICENSE).
+
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FArcletProject%2FAlconna.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FArcletProject%2FAlconna?ref=badge_large)
+
+## Acknowledgement
+
+[JetBrains](https://www.jetbrains.com/): Support Authorize for [PyCharm](https://www.jetbrains.com/pycharm/)<br>
 [<img src="https://cdn.jsdelivr.net/gh/Kyomotoi/CDN@master/noting/jetbrains-variant-3.png" width="200"/>](https://www.jetbrains.com/)
```

### Comparing `arclet_alconna-1.8.8/pyproject.toml` & `arclet_alconna-2.0.0a1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 name = "arclet-alconna"
 description = "A High-performance, Generality, Humane Command Line Arguments Parser Library."
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
-    "nepattern<1.0.0,>=0.6.4",
-    "tarina>=0.4.4",
+    "nepattern<1.0.0,>=0.6.2",
+    "tarina>=0.4.1",
 ]
 dynamic = []
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 readme = "README-EN.md"
 keywords = [
     "command",
     "argparse",
     "fast",
     "alconna",
     "cli",
@@ -28,21 +28,21 @@
     "parsing",
     "optparse",
 ]
 classifiers = [
     "Typing :: Typed",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
 ]
-version = "1.8.8"
+version = "2.0.0a1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
@@ -59,20 +59,18 @@
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest~=7.2.0",
     "coverage~=7.0.1",
     "pydeps~=1.11.0",
     "fix-future-annotations>=0.4.0",
-    "isort>=5.13.2",
-    "black>=24.2.0",
 ]
 
 [tool.pdm.scripts]
-test = "pytest -v -W ignore --ignore entry_test.py"
+test = "python entry_test.py"
 benchmark = "python benchmark.py"
 deps = "pydeps -o alconna.svg ./src/arclet/alconna --max-bacon=4 --cluster --keep-target-cluster --rmprefix alconna. "
 
 [tool.pdm.version]
 source = "file"
 path = "src/arclet/alconna/__init__.py"
 
@@ -123,32 +121,7 @@
     "@(abc\\.)?abstractmethod",
     "@(typing\\.)?overload",
     "def __repr__",
     "def __str__",
     "def __eq__",
     "except ImportError:",
 ]
-
-[tool.black]
-line-length = 120
-target-version = [
-    "py38",
-    "py39",
-    "py310",
-    "py311",
-]
-include = "\\.pyi?$"
-extend-exclude = ""
-
-[tool.isort]
-profile = "black"
-line_length = 120
-skip_gitignore = true
-extra_standard_library = [
-    "typing_extensions",
-]
-
-[tool.pyright]
-pythonVersion = "3.8"
-pythonPlatform = "All"
-typeCheckingMode = "basic"
-disableBytesTypePromotions = true
```

### Comparing `arclet_alconna-1.8.8/src/arclet/alconna/__init__.py` & `arclet_alconna-2.0.0a1/src/arclet/alconna/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,52 @@
-"""Alconna 概览"""
-
-from nepattern import ANY as ANY  # noqa
-from tarina import Empty as Empty  # noqa
-
-from .action import append as append
-from .action import append_value as append_value
-from .action import count as count
-from .action import store_false as store_false
-from .action import store_true as store_true
-from .action import store_value as store_value
-from .args import Arg as Arg
-from .args import ArgFlag as ArgFlag
-from .args import Args as Args
-from .args import Field as Field
-from .argv import Argv as Argv
-from .argv import argv_config as argv_config
-from .argv import set_default_argv_type as set_default_argv_type
-from .arparma import Arparma as Arparma
-from .arparma import ArparmaBehavior as ArparmaBehavior
-from .base import Option as Option
-from .base import Subcommand as Subcommand
-from .builtin import set_default as set_default
-from .completion import CompSession as CompSession
-from .config import Namespace as Namespace
-from .config import config as config
-from .config import namespace as namespace
-from .core import Alconna as Alconna
-from .duplication import Duplication as Duplication
-from .exceptions import AlconnaException as AlconnaException
-from .exceptions import InvalidArgs as InvalidArgs
-from .exceptions import InvalidParam as InvalidParam
-from .exceptions import NullMessage as NullMessage
-from .exceptions import ParamsUnmatched as ParamsUnmatched
-from .formatter import TextFormatter as TextFormatter
-from .manager import ShortcutArgs as ShortcutArgs
-from .manager import command_manager as command_manager
-from .model import HeadResult as HeadResult
-from .model import OptionResult as OptionResult
-from .model import SubcommandResult as SubcommandResult
-from .output import output_manager as output_manager
-from .stub import ArgsStub as ArgsStub
-from .stub import OptionStub as OptionStub
-from .stub import SubcommandStub as SubcommandStub
-from .typing import AllParam as AllParam
-from .typing import CommandMeta as CommandMeta
-from .typing import KeyWordVar as KeyWordVar
-from .typing import Kw as Kw
-from .typing import MultiVar as MultiVar
-from .typing import Nargs as Nargs
-from .typing import UnpackVar as UnpackVar
-from .typing import Up as Up
-
-__version__ = "1.8.8"
-
-# backward compatibility
-AnyOne = ANY
+"""Alconna 概览"""
+
+from nepattern import ANY as ANY  # noqa
+from tarina import Empty as Empty  # noqa
+
+from .action import append as append
+from .action import append_value as append_value
+from .action import count as count
+from .action import store_false as store_false
+from .action import store_true as store_true
+from .action import store_value as store_value
+from .args import Arg as Arg
+from .args import ArgFlag as ArgFlag
+from .args import Args as Args
+from .args import Field as Field
+from .argv import Argv as Argv
+from .argv import argv_config as argv_config
+from .argv import set_default_argv_type as set_default_argv_type
+from .arparma import Arparma as Arparma
+from .arparma import ArparmaBehavior as ArparmaBehavior
+from .base import Option as Option
+from .base import Subcommand as Subcommand
+from .builtin import set_default as set_default
+from .completion import CompSession as CompSession
+from .config import Namespace as Namespace
+from .config import config as config
+from .config import namespace as namespace
+from .core import Alconna as Alconna
+from .exceptions import InvalidParam as InvalidParam
+from .exceptions import NullMessage as NullMessage
+from .exceptions import ParamsUnmatched as ParamsUnmatched
+from .formatter import TextFormatter as TextFormatter
+from .manager import ShortcutArgs as ShortcutArgs
+from .manager import command_manager as command_manager
+from .model import HeadResult as HeadResult
+from .model import OptionResult as OptionResult
+from .model import SubcommandResult as SubcommandResult
+from .output import output_manager as output_manager
+from .typing import AllParam as AllParam
+from .typing import CommandMeta as CommandMeta
+from .typing import KeyWordVar as KeyWordVar
+from .typing import Kw as Kw
+from .typing import MultiVar as MultiVar
+from .typing import Nargs as Nargs
+from .typing import UnpackVar as UnpackVar
+from .typing import Up as Up
+
+__version__ = "2.0.0a1"
+
+# backward compatibility
+Arpamar = Arparma
+DataCollectionContainer = Argv
```

### Comparing `arclet_alconna-1.8.8/src/arclet/alconna/_internal/_analyser.py` & `arclet_alconna-2.0.0a1/src/arclet/alconna/_internal/_analyser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,460 +1,420 @@
-from __future__ import annotations
-
-import re
-from dataclasses import dataclass, field
-from re import Match
-from typing import TYPE_CHECKING, Any, Callable, Generic, Set
-from typing_extensions import Self, TypeAlias
-
-from tarina import Empty, lang
-
-from ..action import Action
-from ..args import Args
-from ..arparma import Arparma
-from ..base import Completion, Help, Option, Shortcut, Subcommand
-from ..completion import comp_ctx
-from ..constraint import SHORTCUT_ARGS, SHORTCUT_REGEX_MATCH, SHORTCUT_REST, SHORTCUT_TRIGGER
-from ..exceptions import (
-    ArgumentMissing,
-    FuzzyMatchSuccess,
-    InvalidParam,
-    ParamsUnmatched,
-    PauseTriggered,
-    SpecialOptionTriggered,
-)
-from ..manager import command_manager
-from ..model import HeadResult, OptionResult, Sentence, SubcommandResult
-from ..output import output_manager
-from ..typing import TDC, InnerShortcutArgs
-from ._handlers import (
-    HEAD_HANDLES,
-    _handle_shortcut_data,
-    _handle_shortcut_reg,
-    analyse_args,
-    analyse_param,
-    handle_completion,
-    handle_help,
-    handle_opt_default,
-    handle_shortcut,
-    prompt,
-)
-from ._header import Header
-from ._util import levenshtein
-
-if TYPE_CHECKING:
-    from ..core import Alconna
-    from ._argv import Argv
-
-_SPECIAL = {"help": handle_help, "shortcut": handle_shortcut, "completion": handle_completion}
-
-
-def _compile_opts(option: Option, data: dict[str, Sentence | Option | list[Option] | SubAnalyser]):
-    """处理选项
-
-    Args:
-        option (Option): 选项
-        data (dict[str, Sentence | Option | list[Option] | SubAnalyser]): 编译的节点
-    """
-    for alias in option.aliases:
-        if li := data.get(alias):
-            if isinstance(li, SubAnalyser):
-                continue
-            if isinstance(li, list):
-                li.append(option)
-                li.sort(key=lambda x: x.priority, reverse=True)
-            elif isinstance(li, Sentence):
-                data[alias] = option
-                continue
-            else:
-                data[alias] = sorted([li, option], key=lambda x: x.priority, reverse=True)
-        else:
-            data[alias] = option
-
-
-def default_compiler(analyser: SubAnalyser, pids: set[str]):
-    """默认的编译方法
-
-    Args:
-        analyser (SubAnalyser): 任意子解析器
-        pids (set[str]): 节点名集合
-    """
-    for opts in analyser.command.options:
-        if isinstance(opts, Option) and not isinstance(opts, (Help, Shortcut, Completion)):
-            if opts.compact or opts.action.type == 2 or not set(analyser.command.separators).issuperset(opts.separators):  # noqa: E501
-                analyser.compact_params.append(opts)
-            _compile_opts(opts, analyser.compile_params)  # type: ignore
-            if opts.default is not Empty:
-                analyser.default_opt_result[opts.dest] = (opts.default, opts.action)
-            pids.update(opts.aliases)
-        elif isinstance(opts, Subcommand):
-            sub = SubAnalyser(opts)
-            for alias in opts.aliases:
-                analyser.compile_params[alias] = sub
-            pids.update(opts.aliases)
-            default_compiler(sub, pids)
-            if not set(analyser.command.separators).issuperset(opts.separators):
-                analyser.compact_params.append(sub)
-            if sub.command.default is not Empty:
-                analyser.default_sub_result[opts.dest] = sub.command.default
-        if opts.requires:
-            pids.update(opts.requires)
-            for k in opts.requires:
-                analyser.compile_params.setdefault(k, Sentence(name=k))
-
-
-@dataclass
-class SubAnalyser(Generic[TDC]):
-    """子解析器, 用于子命令的解析"""
-
-    command: Subcommand
-    """子命令"""
-    default_main_only: bool = field(default=False)
-    """命令是否只有主参数"""
-    need_main_args: bool = field(default=False)
-    """是否需要主参数"""
-    compile_params: dict[str, Sentence | Option | list[Option] | SubAnalyser[TDC]] = field(default_factory=dict)
-    """编译的节点"""
-    compact_params: list[Option | SubAnalyser[TDC]] = field(default_factory=list)
-    """可能紧凑的需要逐个解析的节点"""
-    self_args: Args = field(init=False)
-    """命令自身参数"""
-    subcommands_result: dict[str, SubcommandResult] = field(init=False)
-    """子命令的解析结果"""
-    options_result: dict[str, OptionResult] = field(init=False)
-    """选项的解析结果"""
-    args_result: dict[str, Any] = field(init=False)
-    """参数的解析结果"""
-    header_result: HeadResult | None = field(init=False)
-    """头部的解析结果"""
-    value_result: Any = field(init=False)
-    """值的解析结果"""
-    sentences: list[str] = field(init=False)
-    """暂存传入的所有句段"""
-    default_opt_result: dict[str, tuple[OptionResult, Action]] = field(default_factory=dict)
-    """默认选项的解析结果"""
-    default_sub_result: dict[str, SubcommandResult] = field(default_factory=dict)
-    """默认子命令的解析结果"""
-    extra_allow: bool = field(default=False)
-    """是否允许额外的参数"""
-
-    def _clr(self):
-        """清除自身的解析结果"""
-        self.reset()
-        ks = list(self.__dict__.keys())
-        for k in ks:
-            delattr(self, k)
-
-    def __post_init__(self):
-        self.reset()
-        self.__calc_args__()
-
-    def __calc_args__(self):
-        self.self_args = self.command.args
-        if self.command.nargs > 0 and self.command.nargs > self.self_args.optional_count:
-            self.need_main_args = True  # 如果need_marg那么match的元素里一定得有main_argument
-        _de_count = sum(arg.field.default is not None for arg in self.self_args.argument)
-        if _de_count and _de_count == self.command.nargs:
-            self.default_main_only = True
-
-    def result(self) -> SubcommandResult:
-        """生成子命令解析结果
-
-        Returns:
-            SubcommandResult: 子命令解析结果
-        """
-        if self.default_opt_result:
-            handle_opt_default(self.default_opt_result, self.options_result)
-        if self.default_sub_result:
-            for k, v in self.default_sub_result.items():
-                if k not in self.subcommands_result:
-                    self.subcommands_result[k] = v
-        res = SubcommandResult(self.value_result, self.args_result, self.options_result, self.subcommands_result)
-        self.reset()
-        return res
-
-    def reset(self):
-        """重置解析器"""
-        self.args_result = {}
-        self.options_result = {}
-        self.subcommands_result = {}
-        self.sentences = []
-        self.value_result = None
-        self.header_result = None
-
-    def process(self, argv: Argv[TDC]) -> Self:
-        """处理传入的参数集合
-
-        Args:
-            argv (Argv[TDC]): 命令行参数
-
-        Returns:
-            Self: 自身
-
-        Raises:
-            ParamsUnmatched: 名称不匹配
-            FuzzyMatchSuccess: 模糊匹配成功
-        """
-        sub = argv.current_node = self.command
-        name, _ = argv.next(sub.separators)
-        if name not in sub.aliases:
-            argv.rollback(name)
-            if not argv.fuzzy_match:
-                raise InvalidParam(lang.require("subcommand", "name_error").format(source=sub.dest, target=name))
-            for al in sub.aliases:
-                if levenshtein(name, al) >= argv.fuzzy_threshold:
-                    raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=al, target=name))
-            raise InvalidParam(lang.require("subcommand", "name_error").format(source=sub.dest, target=name))
-
-        self.value_result = sub.action.value
-        return self.analyse(argv)
-
-    def analyse(self, argv: Argv[TDC]) -> Self:
-        """解析传入的参数集合
-
-        Args:
-            argv (Argv[TDC]): 命令行参数
-
-        Returns:
-            Self: 自身
-
-        Raises:
-            ArgumentMissing: 参数缺失
-        """
-        while analyse_param(self, argv, self.command.separators):
-            pass
-        if self.default_main_only and not self.args_result:
-            self.args_result = analyse_args(argv, self.self_args)
-        if not self.args_result and self.need_main_args:
-            raise ArgumentMissing(lang.require("subcommand", "args_missing").format(name=self.command.dest))
-        return self
-
-    def get_sub_analyser(self, target: Subcommand) -> SubAnalyser[TDC] | None:
-        """获取子解析器
-
-        Args:
-            target (Subcommand): 目标子命令
-
-        Returns:
-            SubAnalyser[TDC] | None: 子解析器
-        """
-        if target == self.command:
-            return self
-        for param in self.compile_params.values():
-            if isinstance(param, SubAnalyser):
-                return param.get_sub_analyser(target)
-
-
-class Analyser(SubAnalyser[TDC], Generic[TDC]):
-    """命令解析器"""
-
-    command: Alconna
-    """命令实例"""
-    used_tokens: set[int]
-    """已使用的token"""
-    command_header: Header
-    """命令头部"""
-    header_handler: Callable[[Header, Argv], HeadResult]
-    """头部处理器"""
-
-    def __init__(self, alconna: Alconna[TDC], compiler: TCompile | None = None):
-        """初始化解析器
-
-        Args:
-            alconna (Alconna[TDC]): 命令实例
-            compiler (TCompile | None, optional): 编译器方法
-        """
-        super().__init__(alconna)
-        self._compiler = compiler or default_compiler
-        self.used_tokens = set()
-
-    def compile(self, param_ids: set[str]):
-        self.extra_allow = not self.command.meta.strict or not self.command.namespace_config.strict
-        self.command_header = Header.generate(self.command.command, self.command.prefixes, self.command.meta.compact)
-        self.header_handler = HEAD_HANDLES[self.command_header.flag]
-        self._compiler(self, param_ids)
-        return self
-
-    def _clr(self):
-        self.used_tokens.clear()
-        super()._clr()
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} of {self.command.path}>"
-
-    def shortcut(
-        self, argv: Argv[TDC], data: list[Any], short: Arparma | InnerShortcutArgs, reg: Match | None = None
-    ) -> Arparma[TDC]:
-        """处理被触发的快捷命令
-
-        Args:
-            argv (Argv[TDC]): 命令行参数
-            data (list[Any]): 剩余参数
-            short (Arparma | InnerShortcutArgs): 快捷命令
-            reg (Match | None): 可能的正则匹配结果
-
-        Returns:
-            Arparma[TDC]: Arparma 解析结果
-
-        Raises:
-            ParamsUnmatched: 若不允许快捷命令后随其他参数，则抛出此异常
-        """
-        if isinstance(short, Arparma):
-            return short
-
-        argv.build(short.command)  # type: ignore
-        if not short.fuzzy and data:
-            exc = ParamsUnmatched(lang.require("analyser", "param_unmatched").format(target=data[0]))
-            if self.command.meta.raise_exception:
-                raise exc
-            return self.export(argv, True, exc)
-        argv.addon(short.args, merge_str=False)
-        data = _handle_shortcut_data(argv, data)
-        if not data and argv.raw_data and any(isinstance(i, str) and bool(re.search(r"\{%(\d+)|\*(.*?)\}", i)) for i in argv.raw_data):
-            exc = ArgumentMissing(lang.require("analyser", "param_missing"))
-            if self.command.meta.raise_exception:
-                raise exc
-            return self.export(argv, True, exc)
-        argv.bak_data = argv.raw_data.copy()
-        argv.addon(data, merge_str=False)
-        if reg:
-            data = _handle_shortcut_reg(argv, reg.groups(), reg.groupdict(), short.wrapper)
-            argv.raw_data.clear()
-            argv.ndata = 0
-            argv.current_index = 0
-            argv.addon(data)
-        argv.bak_data = argv.raw_data.copy()
-        if argv.message_cache:
-            argv.token = argv.generate_token(argv.raw_data)
-        return self.process(argv)
-
-    def process(self, argv: Argv[TDC]) -> Arparma[TDC]:
-        """主体解析函数, 应针对各种情况进行解析
-
-        Args:
-            argv (Argv[TDC]): 命令行参数
-
-        Returns:
-            Arparma[TDC]: Arparma 解析结果
-
-        Raises:
-            ValueError: 快捷命令查找失败
-            InvalidParam: 参数不匹配
-            ArgumentMissing: 参数缺失
-        """
-        if argv.message_cache and argv.token in self.used_tokens and (res := command_manager.get_record(argv.token)):
-            return res
-        try:
-            self.header_result = self.header_handler(self.command_header, argv)
-        except InvalidParam as e:
-            _next = e.args[1]
-            if _next.__class__ is not str or not _next:
-                if self.command.meta.raise_exception:
-                    raise e
-                return self.export(argv, True, e)
-            argv.context[SHORTCUT_TRIGGER] = _next
-            try:
-                rest, short, mat = command_manager.find_shortcut(self.command, [_next] + argv.release())
-            except ValueError as exc:
-                if self.command.meta.raise_exception:
-                    raise e from exc
-                return self.export(argv, True, e)
-            else:
-                argv.context[SHORTCUT_ARGS] = short
-                argv.context[SHORTCUT_REST] = rest
-                argv.context[SHORTCUT_REGEX_MATCH] = mat
-                self.reset()
-                return self.shortcut(argv, rest, short, mat)
-
-        except FuzzyMatchSuccess as Fuzzy:
-            output_manager.send(self.command.name, lambda: str(Fuzzy))
-            return self.export(argv, True)
-
-        except RuntimeError as e:
-            exc = InvalidParam(lang.require("header", "error").format(target=argv.release(recover=True)[0]))
-            if self.command.meta.raise_exception:
-                raise exc from e
-            return self.export(argv, True, exc)
-
-        if fail := self.analyse(argv):
-            return fail
-
-        if argv.done and (not self.need_main_args or self.args_result):
-            return self.export(argv)
-
-        rest = argv.release()
-        if len(rest) > 0:
-            if isinstance(rest[-1], str) and rest[-1] in argv.completion_names:
-                argv.bak_data[-1] = argv.bak_data[-1][: -len(rest[-1])].rstrip()
-                return handle_completion(self, argv, rest[-2])
-            exc = ParamsUnmatched(lang.require("analyser", "param_unmatched").format(target=argv.next(move=False)[0]))
-        else:
-            exc = ArgumentMissing(lang.require("analyser", "param_missing"))
-        if comp_ctx.get(None) and isinstance(exc, ArgumentMissing):
-            raise PauseTriggered(prompt(self, argv), exc, argv)
-        if self.command.meta.raise_exception:
-            raise exc
-        return self.export(argv, True, exc)
-
-    def analyse(self, argv: Argv[TDC]) -> Arparma[TDC] | None:
-        try:
-            while analyse_param(self, argv) and argv.current_index != argv.ndata:
-                pass
-        except FuzzyMatchSuccess as e:
-            output_manager.send(self.command.name, lambda: str(e))
-            return self.export(argv, True)
-        except SpecialOptionTriggered as sot:
-            return _SPECIAL[sot.args[0]](self, argv)
-        except (InvalidParam, ArgumentMissing) as e1:
-            if (rest := argv.release()) and isinstance(rest[-1], str):
-                if rest[-1] in argv.completion_names and "completion" not in argv.namespace.disable_builtin_options:
-                    argv.bak_data[-1] = argv.bak_data[-1][: -len(rest[-1])].rstrip()
-                    return handle_completion(self, argv)
-                if (handler := argv.special.get(rest[-1])) and handler not in argv.namespace.disable_builtin_options:
-                    return _SPECIAL[handler](self, argv)
-            if comp_ctx.get(None):
-                if isinstance(e1, InvalidParam):
-                    argv.free(argv.current_node.separators if argv.current_node else None)
-                raise PauseTriggered(prompt(self, argv), e1, argv) from e1
-            if self.command.meta.raise_exception:
-                raise
-            return self.export(argv, True, e1)
-
-        if self.default_main_only and not self.args_result:
-            self.args_result = analyse_args(argv, self.self_args)
-
-    def export(
-        self,
-        argv: Argv[TDC],
-        fail: bool = False,
-        exception: Exception | None = None,
-    ) -> Arparma[TDC]:
-        """创建 `Arparma` 解析结果, 其一定是一次解析的最后部分
-
-        Args:
-            argv (Argv[TDC]): 命令行参数
-            fail (bool, optional): 是否解析失败. Defaults to False.
-            exception (Exception | None, optional): 解析失败时的异常. Defaults to None.
-        """
-        result = Arparma(self.command.path, argv.origin, not fail, self.header_result, ctx=argv.exit())
-        if fail:
-            result.error_info = exception
-            result.error_data = argv.release()
-        else:
-            if self.default_opt_result:
-                handle_opt_default(self.default_opt_result, self.options_result)
-            if self.default_sub_result:
-                for k, v in self.default_sub_result.items():
-                    if k not in self.subcommands_result:
-                        self.subcommands_result[k] = v
-            result.main_args = self.args_result
-            result.options = self.options_result
-            result.subcommands = self.subcommands_result
-            result.unpack()
-            if argv.message_cache:
-                command_manager.record(argv.token, result)
-                self.used_tokens.add(argv.token)
-        self.reset()
-        return result  # type: ignore
-
-
-TCompile: TypeAlias = Callable[[SubAnalyser, Set[str]], None]
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from re import Match
+from typing import TYPE_CHECKING, Any, Callable, Generic, Set
+
+from tarina import lang, Empty
+from typing_extensions import Self, TypeAlias
+
+from ..action import Action
+from ..args import Args
+from ..arparma import Arparma
+from ..base import Option, Subcommand
+from ..completion import comp_ctx
+from ..config import config
+from ..exceptions import (
+    ArgumentMissing, FuzzyMatchSuccess, ParamsUnmatched, PauseTriggered, SpecialOptionTriggered
+)
+from ..manager import ShortcutArgs, command_manager
+from ..model import HeadResult, OptionResult, SubcommandResult
+from ..output import output_manager
+from ..typing import TDC
+from ._handlers import (
+    analyse_args, analyse_header, analyse_param,
+    handle_completion, handle_help, handle_opt_default,
+    handle_shortcut, prompt, _handle_shortcut_data, _handle_shortcut_reg
+)
+from ._header import Header
+from ._util import levenshtein
+
+if TYPE_CHECKING:
+    from ..core import Alconna
+    from ._argv import Argv
+
+_SPECIAL = {
+    "help": handle_help,
+    "shortcut": handle_shortcut,
+    "completion": handle_completion
+}
+
+
+def _compile_opts(option: Option, data: dict[str, Option | list[Option] | SubAnalyser]):
+    """处理选项
+
+    Args:
+        option (Option): 选项
+        data (dict[str, Sentence | Option | list[Option] | SubAnalyser]): 编译的节点
+    """
+    for alias in option.aliases:
+        if li := data.get(alias):
+            if isinstance(li, SubAnalyser):
+                continue
+            if isinstance(li, list):
+                li.append(option)
+                li.sort(key=lambda x: x.priority, reverse=True)
+            else:
+                data[alias] = sorted([li, option], key=lambda x: x.priority, reverse=True)
+        else:
+            data[alias] = option
+
+
+def default_compiler(analyser: SubAnalyser, pids: set[str]):
+    """默认的编译方法
+
+    Args:
+        analyser (SubAnalyser): 任意子解析器
+        pids (set[str]): 节点名集合
+    """
+    for opts in analyser.command.options:
+        if isinstance(opts, Option):
+            if opts.compact or opts.action.type == 2 or not set(analyser.command.separators).issuperset(opts.separators):
+                analyser.compact_params.append(opts)
+            _compile_opts(opts, analyser.compile_params)  # type: ignore
+            if opts.default is not Empty:
+                analyser.default_opt_result[opts.dest] = (opts.default, opts.action)
+            pids.update(opts.aliases)
+        elif isinstance(opts, Subcommand):
+            sub = SubAnalyser(opts)
+            analyser.compile_params[opts.name] = sub
+            pids.add(opts.name)
+            default_compiler(sub, pids)
+            if not set(analyser.command.separators).issuperset(opts.separators):
+                analyser.compact_params.append(sub)
+            if sub.command.default:
+                analyser.default_sub_result[opts.dest] = sub.command.default
+
+
+@dataclass
+class SubAnalyser(Generic[TDC]):
+    """子解析器, 用于子命令的解析"""
+    command: Subcommand
+    """子命令"""
+    default_main_only: bool = field(default=False)
+    """命令是否只有主参数"""
+    need_main_args: bool = field(default=False)
+    """是否需要主参数"""
+    compile_params: dict[str, Option | list[Option] | SubAnalyser[TDC]] = field(default_factory=dict)
+    """编译的节点"""
+    compact_params: list[Option | SubAnalyser[TDC]] = field(default_factory=list)
+    """可能紧凑的需要逐个解析的节点"""
+    self_args: Args = field(init=False)
+    """命令自身参数"""
+    subcommands_result: dict[str, SubcommandResult] = field(init=False)
+    """子命令的解析结果"""
+    options_result: dict[str, OptionResult] = field(init=False)
+    """选项的解析结果"""
+    args_result: dict[str, Any] = field(init=False)
+    """参数的解析结果"""
+    header_result: HeadResult | None = field(init=False)
+    """头部的解析结果"""
+    value_result: Any = field(init=False)
+    """值的解析结果"""
+    default_opt_result: dict[str, tuple[OptionResult, Action]] = field(default_factory=dict)
+    """默认选项的解析结果"""
+    default_sub_result: dict[str, SubcommandResult] = field(default_factory=dict)
+    """默认子命令的解析结果"""
+
+    def _clr(self):
+        """清除自身的解析结果"""
+        self.reset()
+        ks = list(self.__dict__.keys())
+        for k in ks:
+            delattr(self, k)
+
+    def __post_init__(self):
+        self.reset()
+        self.self_args = self.command.args
+        if self.command.nargs > 0 and self.command.nargs > self.self_args.optional_count:
+            self.need_main_args = True  # 如果need_marg那么match的元素里一定得有main_argument
+        _de_count = sum(arg.field.default is not None for arg in self.self_args.argument)
+        if _de_count and _de_count == self.command.nargs:
+            self.default_main_only = True
+
+    def result(self) -> SubcommandResult:
+        """生成子命令解析结果
+
+        Returns:
+            SubcommandResult: 子命令解析结果
+        """
+        if self.default_opt_result:
+            handle_opt_default(self.default_opt_result, self.options_result)
+        if self.default_sub_result:
+            for k, v in self.default_sub_result.items():
+                if k not in self.subcommands_result:
+                    self.subcommands_result[k] = v
+        res = SubcommandResult(
+            self.value_result, self.args_result, self.options_result, self.subcommands_result
+        )
+        self.reset()
+        return res
+
+    def reset(self):
+        """重置解析器"""
+        self.args_result = {}
+        self.options_result = {}
+        self.subcommands_result = {}
+        self.value_result = None
+        self.header_result = None
+
+    def process(self, argv: Argv[TDC]) -> Self:
+        """处理传入的参数集合
+
+        Args:
+            argv (Argv[TDC]): 命令行参数
+
+        Returns:
+            Self: 自身
+
+        Raises:
+            ParamsUnmatched: 名称不匹配
+            FuzzyMatchSuccess: 模糊匹配成功
+        """
+        sub = argv.context = self.command
+        name, _ = argv.next(sub.separators)
+        if name != sub.name:  # 先匹配节点名称
+            if argv.fuzzy_match and levenshtein(name, sub.name) >= config.fuzzy_threshold:
+                raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=name, target=sub.name))
+            raise ParamsUnmatched(lang.require("subcommand", "name_error").format(target=name, source=sub.name))
+
+        self.value_result = sub.action.value
+        return self.analyse(argv)
+
+    def analyse(self, argv: Argv[TDC]) -> Self:
+        """解析传入的参数集合
+
+        Args:
+            argv (Argv[TDC]): 命令行参数
+
+        Returns:
+            Self: 自身
+
+        Raises:
+            ArgumentMissing: 参数缺失
+        """
+        while analyse_param(self, argv, self.command.separators):
+            pass
+        if self.default_main_only and not self.args_result:
+            self.args_result = analyse_args(argv, self.self_args)
+        if not self.args_result and self.need_main_args:
+            raise ArgumentMissing(lang.require("subcommand", "args_missing").format(name=self.command.dest))
+        return self
+
+    def get_sub_analyser(self, target: Subcommand) -> SubAnalyser[TDC] | None:
+        """获取子解析器
+
+        Args:
+            target (Subcommand): 目标子命令
+
+        Returns:
+            SubAnalyser[TDC] | None: 子解析器
+        """
+        if target == self.command:
+            return self
+        for param in self.compile_params.values():
+            if isinstance(param, SubAnalyser):
+                return param.get_sub_analyser(target)
+
+
+class Analyser(SubAnalyser[TDC], Generic[TDC]):
+    """命令解析器"""
+    command: Alconna
+    """命令实例"""
+    used_tokens: set[int]
+    """已使用的token"""
+    command_header: Header
+    """命令头部"""
+
+    def __init__(self, alconna: Alconna[TDC], compiler: TCompile | None = None):
+        """初始化解析器
+
+        Args:
+            alconna (Alconna[TDC]): 命令实例
+            compiler (TCompile | None, optional): 编译器方法
+        """
+        super().__init__(alconna)
+        self.fuzzy_match = alconna.meta.fuzzy_match
+        self.used_tokens = set()
+        self.command_header = Header.generate(alconna.command, alconna.prefixes, alconna.meta.compact)
+        compiler = compiler or default_compiler
+        compiler(
+            self,
+            command_manager.resolve(self.command).param_ids
+        )
+
+    def _clr(self):
+        self.used_tokens.clear()
+        super()._clr()
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__} of {self.command.path}>"
+
+    def shortcut(
+        self, argv: Argv[TDC], trigger: str, data: list[Any], short: Arparma | ShortcutArgs, reg: Match | None = None
+    ) -> Arparma[TDC]:
+        """处理被触发的快捷命令
+
+        Args:
+            argv (Argv[TDC]): 命令行参数
+            trigger (str): 触发词
+            data (list[Any]): 剩余参数
+            short (Arparma | ShortcutArgs): 快捷命令
+            reg (Match | None): 可能的正则匹配结果
+
+        Returns:
+            Arparma[TDC]: Arparma 解析结果
+
+        Raises:
+            ParamsUnmatched: 若不允许快捷命令后随其他参数，则抛出此异常
+        """
+        if isinstance(short, Arparma):
+            return short
+
+        argv.build(short.get('command', argv.converter(self.command.command or self.command.name)))
+        if not short.get('fuzzy') and data:
+            exc = ParamsUnmatched(lang.require("analyser", "param_unmatched").format(target=data[0]))
+            if self.command.meta.raise_exception:
+                raise exc
+            return self.export(argv, True, exc)
+        if short.get('fuzzy') and reg and len(trigger) > reg.span()[1]:
+            argv.addon((trigger[reg.span()[1]:],))
+        argv.addon(short.get('args', []))
+        data = _handle_shortcut_data(argv, data)
+        argv.bak_data = argv.raw_data.copy()
+        argv.addon(data)
+        if reg:
+            _handle_shortcut_reg(argv, reg.groups(), reg.groupdict())
+        argv.bak_data = argv.raw_data.copy()
+        if argv.message_cache:
+            argv.token = argv.generate_token(argv.raw_data)
+        return self.process(argv)
+
+    def process(self, argv: Argv[TDC]) -> Arparma[TDC]:
+        """主体解析函数, 应针对各种情况进行解析
+
+        Args:
+            argv (Argv[TDC]): 命令行参数
+
+        Returns:
+            Arparma[TDC]: Arparma 解析结果
+
+        Raises:
+            ValueError: 快捷命令查找失败
+            ParamsUnmatched: 参数不匹配
+            ArgumentMissing: 参数缺失
+        """
+        if (
+            argv.message_cache and
+            argv.token in self.used_tokens and
+            (res := command_manager.get_record(argv.token))
+        ):
+            return res
+        try:
+            self.header_result = analyse_header(self.command_header, argv)
+        except ParamsUnmatched as e:
+            _next = e.args[1]
+            if _next.__class__ is not str:
+                if self.command.meta.raise_exception:
+                    raise e
+                return self.export(argv, True, e)
+            try:
+                _res = command_manager.find_shortcut(self.command, _next)
+            except ValueError as exc:
+                if self.command.meta.raise_exception:
+                    raise e from exc
+                return self.export(argv, True, e)
+            else:
+                data = argv.release()
+                self.reset()
+                argv.reset()
+                return self.shortcut(argv, _next, data, *_res)
+
+        except FuzzyMatchSuccess as Fuzzy:
+            output_manager.send(self.command.name, lambda: str(Fuzzy))
+            return self.export(argv, True)
+
+        except RuntimeError as e:
+            exc = ParamsUnmatched(lang.require("header", "error").format(target=argv.release(recover=True)[0]))
+            if self.command.meta.raise_exception:
+                raise exc from e
+            return self.export(argv, True, exc)
+
+        if fail := self.analyse(argv):
+            return fail
+
+        if argv.done and (not self.need_main_args or self.args_result):
+            return self.export(argv)
+
+        rest = argv.release()
+        if len(rest) > 0:
+            if isinstance(rest[-1], str) and rest[-1] in argv.completion_names:
+                last = argv.bak_data[-1]
+                argv.bak_data[-1] = last[:last.rfind(rest[-1])]
+                return handle_completion(self, argv, rest[-2])
+            exc = ParamsUnmatched(lang.require("analyser", "param_unmatched").format(target=argv.next(move=False)[0]))
+        else:
+            exc = ArgumentMissing(lang.require("analyser", "param_missing"))
+        if isinstance(exc, ArgumentMissing) and comp_ctx.get(None):
+            raise PauseTriggered(prompt(self, argv))
+        if self.command.meta.raise_exception:
+            raise exc
+        return self.export(argv, True, exc)
+
+    def analyse(self, argv: Argv[TDC]) -> Arparma[TDC] | None:
+        try:
+            while analyse_param(self, argv) and argv.current_index != argv.ndata:
+                pass
+        except FuzzyMatchSuccess as e:
+            output_manager.send(self.command.name, lambda: str(e))
+            return self.export(argv, True)
+        except SpecialOptionTriggered as sot:
+            return _SPECIAL[sot.args[0]](self, argv)
+        except (ParamsUnmatched, ArgumentMissing) as e1:
+            if (rest := argv.release()) and isinstance(rest[-1], str):
+                if rest[-1] in argv.completion_names:
+                    last = argv.bak_data[-1]
+                    argv.bak_data[-1] = last[:last.rfind(rest[-1])]
+                    return handle_completion(self, argv)
+                if handler := argv.special.get(rest[-1]):
+                    return _SPECIAL[handler](self, argv)
+            if isinstance(e1, ArgumentMissing) and comp_ctx.get(None):
+                raise PauseTriggered(prompt(self, argv)) from e1
+            if self.command.meta.raise_exception:
+                raise
+            return self.export(argv, True, e1)
+
+        if self.default_main_only and not self.args_result:
+            self.args_result = analyse_args(argv, self.self_args)
+
+    def export(
+        self, argv: Argv[TDC], fail: bool = False, exception: BaseException | None = None,
+    ) -> Arparma[TDC]:
+        """创建 `Arparma` 解析结果, 其一定是一次解析的最后部分
+
+        Args:
+            argv (Argv[TDC]): 命令行参数
+            fail (bool, optional): 是否解析失败. Defaults to False.
+            exception (BaseException | None, optional): 解析失败时的异常. Defaults to None.
+        """
+        result = Arparma(self.command.path, argv.origin, not fail, self.header_result)
+        if fail:
+            result.error_info = exception
+            result.error_data = argv.release()
+        else:
+            if self.default_opt_result:
+                handle_opt_default(self.default_opt_result, self.options_result)
+            if self.default_sub_result:
+                for k, v in self.default_sub_result.items():
+                    if k not in self.subcommands_result:
+                        self.subcommands_result[k] = v
+            result.main_args = self.args_result
+            result.options = self.options_result
+            result.subcommands = self.subcommands_result
+            if argv.message_cache:
+                command_manager.record(argv.token, result)
+                self.used_tokens.add(argv.token)
+        self.reset()
+        return result  # type: ignore
+
+
+TCompile: TypeAlias = Callable[[SubAnalyser, Set[str]], None]
```

### Comparing `arclet_alconna-1.8.8/src/arclet/alconna/_internal/_handlers.py` & `arclet_alconna-2.0.0a1/src/arclet/alconna/_internal/_handlers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,836 +1,634 @@
-from __future__ import annotations
-
-import re
-from typing import TYPE_CHECKING, Any, Iterable, Callable
-
-from nepattern import ANY, STRING, AnyString, BasePattern, TPattern
-from tarina import Empty, lang, safe_eval, split_once
-from typing_extensions import NoReturn
-
-from ..action import Action
-from ..args import Arg, Args
-from ..base import Option, Subcommand
-from ..completion import Prompt, comp_ctx
-from ..config import config
-from ..exceptions import AlconnaException, ArgumentMissing, FuzzyMatchSuccess, InvalidParam, PauseTriggered, SpecialOptionTriggered
-from ..model import HeadResult, OptionResult, Sentence
-from ..output import output_manager
-from ..typing import KWBool, MultiKeyWordVar, MultiVar, ShortcutRegWrapper
-from ._header import Double, Header, Pair
-from ._util import escape, levenshtein, unescape
-
-if TYPE_CHECKING:
-    from ._analyser import Analyser, SubAnalyser
-    from ._argv import Argv
-
-pat = re.compile("(?:-*no)?-*(?P<name>.+)")
-_bracket = re.compile(r"{(.+)}")
-_parentheses = re.compile(r"\$?\((.+)\)")
-
-
-def _context(argv: Argv, target: Arg[Any], _arg: str):
-    _pat = _bracket if argv.context_style == "bracket" else _parentheses
-    if not (mat := _pat.fullmatch(_arg)):
-        return _arg
-    ctx = argv.context
-    name = mat.group(1)
-    if name == "_":
-        return ctx
-    if name in ctx:
-        return ctx[name]
-    try:
-        return safe_eval(name, ctx)
-    except NameError:
-        raise ArgumentMissing(target.field.get_missing_tips(lang.require("args", "missing").format(key=target.name)))
-    except Exception as e:
-        raise InvalidParam(
-            target.field.get_unmatch_tips(_arg, lang.require("nepattern", "context_error").format(target=target.name, expected=name))
-        )
-
-
-def _validate(argv: Argv, target: Arg[Any], value: BasePattern[Any, Any], result: dict[str, Any], arg: Any, _str: bool):
-    _arg = arg
-    if _str and argv.context_style:
-        _arg = _context(argv, target, _arg)
-    if (value is STRING and _str) or value is ANY:
-        result[target.name] = _arg
-        return
-    if value is AnyString:
-        result[target.name] = str(_arg)
-        return
-    default_val = target.field.default
-    res = value.validate(_arg, default_val)
-    if res.flag != "valid":
-        argv.rollback(arg)
-    if res.flag == "error":
-        if target.optional:
-            return
-        raise InvalidParam(target.field.get_unmatch_tips(arg, res.error().args[0]))
-    result[target.name] = res._value  # noqa
-
-
-def step_varpos(argv: Argv, args: Args, slot: tuple[MultiVar, Arg], result: dict[str, Any]):
-    value, arg = slot
-    argv.current_node = arg
-    key = arg.name
-    default_val = arg.field.default
-    _result = []
-    kwonly_seps = tuple(arg.value.sep for arg in args.argument.keyword_only.values())  # type: ignore
-    count = 0
-    while argv.current_index != argv.ndata:
-        may_arg, _str = argv.next(arg.separators)
-        if _str and may_arg in argv.special:
-            if argv.special[may_arg] not in argv.namespace.disable_builtin_options:
-                raise SpecialOptionTriggered(argv.special[may_arg])
-        if not may_arg or (_str and may_arg in argv.param_ids):
-            argv.rollback(may_arg)
-            break
-        if _str and may_arg in config.remainders:
-            break
-        if _str and kwonly_seps and split_once(pat.match(may_arg)["name"], kwonly_seps, argv.filter_crlf)[0] in args.argument.keyword_only:  # noqa: E501  # type: ignore
-            argv.rollback(may_arg)
-            break
-        if _str and args.argument.vars_keyword and args.argument.vars_keyword[0][0].base.sep in may_arg:
-            argv.rollback(may_arg)
-            break
-        if (res := value.base.validate(may_arg)).flag != "valid":
-            argv.rollback(may_arg)
-            break
-        _result.append(res._value)  # noqa
-        count += 1
-        if 0 < value.length <= count:
-            break
-    if not _result:
-        if default_val is not Empty:
-            _result = default_val if isinstance(default_val, Iterable) else ()
-        elif value.flag == "*":
-            _result = ()
-        else:
-            raise ArgumentMissing(arg.field.get_missing_tips(lang.require("args", "missing").format(key=key)))
-    result[key] = tuple(_result)
-
-
-def step_varkey(argv: Argv, slot: tuple[MultiKeyWordVar, Arg], result: dict[str, Any]):
-    value, arg = slot
-    argv.current_node = arg
-    name = arg.name
-    default_val = arg.field.default
-    _result = {}
-    count = 0
-    while argv.current_index != argv.ndata:
-        may_arg, _str = argv.next(arg.separators)
-        if _str and may_arg in argv.special:
-            if argv.special[may_arg] not in argv.namespace.disable_builtin_options:
-                raise SpecialOptionTriggered(argv.special[may_arg])
-        if not may_arg or (_str and may_arg in argv.param_ids) or not _str:
-            argv.rollback(may_arg)
-            break
-        if _str and may_arg in config.remainders:
-            break
-        if not (_kwarg := re.match(rf"^(-*[^{value.base.sep}]+){value.base.sep}(.*?)$", may_arg)):
-            argv.rollback(may_arg)
-            break
-        key = _kwarg[1]
-        if not (_m_arg := _kwarg[2]):
-            _m_arg, _ = argv.next(arg.separators)
-        if (res := value.base.base.validate(_m_arg)).flag != "valid":
-            argv.rollback(may_arg)
-            break
-        _result[key] = res._value  # noqa
-        count += 1
-        if 0 < value.length <= count:
-            break
-    if not _result:
-        if default_val is not Empty:
-            _result = default_val if isinstance(default_val, dict) else {}
-        elif value.flag == "*":
-            _result = {}
-        else:
-            raise ArgumentMissing(arg.field.get_missing_tips(lang.require("args", "missing").format(key=name)))
-    result[name] = _result
-
-
-def step_keyword(argv: Argv, args: Args, result: dict[str, Any]):
-    kwonly_seps = set()
-    for arg in args.argument.keyword_only.values():
-        kwonly_seps.update(arg.separators)
-    kwonly_seps1 = tuple(arg.value.sep for arg in args.argument.keyword_only.values())  # type: ignore
-    target = len(args.argument.keyword_only)
-    count = 0
-    while count < target:
-        may_arg, _str = argv.next(tuple(kwonly_seps))
-        if _str and may_arg in argv.special:
-            if argv.special[may_arg] not in argv.namespace.disable_builtin_options:
-                raise SpecialOptionTriggered(argv.special[may_arg])
-        if not may_arg or not _str:
-            argv.rollback(may_arg)
-            break
-        if _str and may_arg in config.remainders:
-            break
-        key, _m_arg = split_once(may_arg, kwonly_seps1, argv.filter_crlf)
-        _key = pat.match(key)["name"]  # type: ignore
-        if _key not in args.argument.keyword_only:
-            _key = key
-        if _key not in args.argument.keyword_only:
-            argv.rollback(may_arg)
-            if args.argument.vars_keyword or (_str and may_arg in argv.param_ids):
-                break
-            for arg in args.argument.keyword_only.values():
-                if arg.value.base.validate(may_arg).flag == "valid":  # type: ignore
-                    raise InvalidParam(lang.require("args", "key_missing").format(target=may_arg, key=arg.name))
-            for name in args.argument.keyword_only:
-                if levenshtein(_key, name) >= argv.fuzzy_threshold:
-                    raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=name, target=_key))
-            raise InvalidParam(lang.require("args", "key_not_found").format(name=_key))
-        arg = args.argument.keyword_only[_key]
-        value = arg.value.base  # type: ignore
-        if not _m_arg:
-            if isinstance(value, KWBool):
-                _m_arg = key
-            else:
-                _m_arg, _ = argv.next(args.argument.keyword_only[_key].separators)
-        _validate(argv, arg, value, result, _m_arg, _str)
-        count += 1
-
-    if count < target:
-        for key, arg in args.argument.keyword_only.items():
-            if key in result:
-                continue
-            if arg.field.default is not Empty:
-                result[key] = arg.field.default
-            elif not arg.optional:
-                raise ArgumentMissing(arg.field.get_missing_tips(lang.require("args", "missing").format(key=key)))
-
-
-def analyse_args(argv: Argv, args: Args) -> dict[str, Any]:
-    """
-    分析 `Args` 部分
-
-    Args:
-        argv (Argv): 命令行参数
-        args (Args): 目标 `Args`
-
-    Returns:
-        dict[str, Any]: 解析结果
-    """
-    result = {}
-    for arg in args.argument.normal:
-        argv.current_node = arg
-        may_arg, _str = argv.next(arg.separators)
-        if _str and may_arg in argv.special:
-            if argv.special[may_arg] not in argv.namespace.disable_builtin_options:
-                raise SpecialOptionTriggered(argv.special[may_arg])
-        if _str and may_arg in argv.param_ids and arg.optional:
-            if (de := arg.field.default) is not Empty:
-                result[arg.name] = de
-            argv.rollback(may_arg)
-            continue
-        if not may_arg:
-            argv.rollback(may_arg)
-            if (de := arg.field.default) is not Empty:
-                result[arg.name] = de
-            elif not arg.optional:
-                raise ArgumentMissing(arg.field.get_missing_tips(lang.require("args", "missing").format(key=arg.name)))
-            continue
-        value = arg.value
-        if value.alias == "*":
-            argv.rollback(may_arg)
-            result[arg.name] = argv.converter(argv.release(arg.separators))
-            argv.current_index = argv.ndata
-            return result
-        _validate(argv, arg, value, result, may_arg, _str)
-    if args.argument.unpack:
-        arg, unpack = args.argument.unpack
-        try:
-            unpack.separate(*arg.separators)
-            result[arg.name] = arg.value.origin(**analyse_args(argv, unpack))
-        except Exception as e:
-            if (de := arg.field.default) is not Empty:
-                result[arg.name] = de
-            elif not arg.optional:
-                raise e
-    for slot in args.argument.vars_positional:
-        step_varpos(argv, args, slot, result)
-    if args.argument.keyword_only:
-        step_keyword(argv, args, result)
-    for slot in args.argument.vars_keyword:
-        step_varkey(argv, slot, result)
-    argv.current_node = None
-    return result
-
-
-def handle_option(argv: Argv, opt: Option) -> tuple[str, OptionResult]:
-    """
-    处理 `Option` 部分
-
-    Args:
-        argv (Argv): 命令行参数
-        opt (Option): 目标 `Option`
-    """
-    argv.current_node = opt
-    _cnt = 0
-    error = True
-    name, _ = argv.next(opt.separators)
-    if opt.compact:
-        for al in opt.aliases:
-            if mat := re.fullmatch(f"{al}(?P<rest>.*?)", name):
-                argv.rollback(mat["rest"], replace=True)
-                error = False
-                break
-    elif opt.action.type == 2:
-        for al in opt.aliases:
-            if name.startswith(al) and (cnt := (len(name.lstrip("-")) / len(al.lstrip("-")))).is_integer():
-                _cnt = int(cnt)
-                error = False
-                break
-    elif name in opt.aliases:
-        error = False
-    if error:
-        argv.rollback(name)
-        if not argv.fuzzy_match:
-            raise InvalidParam(lang.require("option", "name_error").format(source=opt.dest, target=name))
-        for al in opt.aliases:
-            if levenshtein(name, al) >= argv.fuzzy_threshold:
-                raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=al, target=name))
-        raise InvalidParam(lang.require("option", "name_error").format(source=opt.dest, target=name))
-    name = opt.dest
-    return (
-        (name, OptionResult(None, analyse_args(argv, opt.args)))
-        if opt.nargs
-        else (name, OptionResult(_cnt or opt.action.value))
-    )
-
-
-def handle_action(param: Option, source: OptionResult, target: OptionResult):
-    """处理 `Option` 的 `action`"""
-    if param.action.type == 0:
-        return target
-    if param.action.type == 2:
-        if not param.nargs:
-            source.value += target.value
-            return source
-        return target
-    if not param.nargs:
-        source.value = source.value[:]
-        source.value.extend(target.value)
-    else:
-        for key, value in target.args.items():
-            if key in source.args:
-                source.args[key].append(value)
-            else:
-                source.args[key] = [value]
-    return source
-
-
-def analyse_option(analyser: SubAnalyser, argv: Argv, opt: Option):
-    """
-    分析 `Option` 部分
-
-    Args:
-        analyser (SubAnalyser): 当前解析器
-        argv (Argv): 命令行参数
-        opt (Option): 目标 `Option`
-    """
-    opt_n, opt_v = handle_option(argv, opt)
-    if opt_n not in analyser.options_result:
-        analyser.options_result[opt_n] = opt_v
-        if opt.action.type == 1 and opt_v.args:
-            for key in list(opt_v.args.keys()):
-                opt_v.args[key] = [opt_v.args[key]]
-    else:
-        analyser.options_result[opt_n] = handle_action(opt, analyser.options_result[opt_n], opt_v)
-
-
-def analyse_compact_params(analyser: SubAnalyser, argv: Argv):
-    """分析紧凑参数
-
-    Args:
-        analyser (SubAnalyser): 当前解析器
-        argv (Argv): 命令行参数
-    """
-    for param in analyser.compact_params:
-        _data, _index = argv.data_set()
-        try:
-            if param.__class__ is Option:
-                oparam: Option = param  # type: ignore
-                if oparam.requires and analyser.sentences != oparam.requires:
-                    return lang.require("option", "require_error").format(
-                        source=oparam.name, target=" ".join(analyser.sentences)
-                    )
-                analyse_option(analyser, argv, oparam)
-            else:
-                sparam: SubAnalyser = param  # type: ignore
-                if sparam.command.requires and analyser.sentences != sparam.command.requires:
-                    return lang.require("subcommand", "require_error").format(
-                        source=sparam.command.name, target=" ".join(analyser.sentences)
-                    )
-                try:
-                    sparam.process(argv)
-                except (FuzzyMatchSuccess, PauseTriggered, SpecialOptionTriggered):
-                    sparam.result()
-                    raise
-                except InvalidParam:
-                    if argv.current_node is sparam.command:
-                        sparam.result()
-                    else:
-                        analyser.subcommands_result[sparam.command.dest] = sparam.result()
-                    raise
-                except AlconnaException:
-                    analyser.subcommands_result[sparam.command.dest] = sparam.result()
-                    raise
-                else:
-                    analyser.subcommands_result[sparam.command.dest] = sparam.result()
-            _data.clear()
-            return True
-        except InvalidParam as e:
-            if argv.current_node.__class__ is Arg:
-                raise e
-            argv.data_reset(_data, _index)
-    else:
-        return False
-
-
-def handle_opt_default(defaults: dict[str, tuple[OptionResult, Action]], data: dict[str, OptionResult]):
-    for k, v in defaults.items():
-        if k not in data:
-            data[k] = v[0]
-        if not v[0].args:
-            continue
-        for key, value in v[0].args.items():
-            data[k].args.setdefault(key, [value] if v[1].value == 1 else value)
-
-
-def analyse_param(analyser: SubAnalyser, argv: Argv, seps: tuple[str, ...] | None = None):
-    """处理参数
-
-    Args:
-        analyser (SubAnalyser): 当前解析器
-        argv (Argv): 命令行参数
-        seps (tuple[str, ...], optional): 指定的分隔符.
-    """
-    _text, _str = argv.next(seps, move=False)
-    if _str and _text in argv.special:
-        if argv.special[_text] not in argv.namespace.disable_builtin_options:
-            if _text in argv.completion_names:
-                argv.bak_data[argv.current_index] = argv.bak_data[argv.current_index].replace(_text, "")
-            raise SpecialOptionTriggered(argv.special[_text])
-    if not _str or not _text:
-        _param = None
-    elif _text in analyser.compile_params:
-        _param = analyser.compile_params[_text]
-    elif analyser.compact_params and (res := analyse_compact_params(analyser, argv)):
-        if res.__class__ is str:
-            raise InvalidParam(res)
-        argv.current_node = None
-        return True
-    else:
-        _param = None
-    if not _param and analyser.command.nargs and not analyser.args_result:
-        analyser.args_result = analyse_args(argv, analyser.self_args)
-        if analyser.args_result:
-            argv.current_node = None
-            return True
-    if _param.__class__ is Sentence:
-        analyser.sentences.append(argv.next()[0])
-        return True
-    if _param.__class__ is Option:
-        oparam: Option = _param  # type: ignore
-        if oparam.requires and analyser.sentences != oparam.requires:
-            raise InvalidParam(
-                lang.require("option", "require_error").format(source=oparam.name, target=" ".join(analyser.sentences))
-            )
-        analyse_option(analyser, argv, oparam)
-    elif _param.__class__ is list:
-        exc: Exception | None = None
-        lparam: list[Option] = _param  # type: ignore
-        for opt in lparam:
-            _data, _index = argv.data_set()
-            try:
-                if opt.requires and analyser.sentences != opt.requires:
-                    raise InvalidParam(
-                        lang.require("option", "require_error").format(
-                            source=opt.name, target=" ".join(analyser.sentences)
-                        )
-                    )
-                analyser.sentences = []
-                analyse_option(analyser, argv, opt)
-                _data.clear()
-                exc = None
-                break
-            except Exception as e:
-                exc = e
-                argv.data_reset(_data, _index)
-        if exc:
-            raise exc  # type: ignore  # noqa
-    elif _param is not None:
-        sparam: SubAnalyser = _param  # type: ignore
-        if sparam.command.requires and analyser.sentences != sparam.command.requires:
-            raise InvalidParam(
-                lang.require("subcommand", "require_error").format(
-                    source=sparam.command.name, target=" ".join(analyser.sentences)
-                )
-            )
-        try:
-            sparam.process(argv)
-        except (FuzzyMatchSuccess, PauseTriggered, SpecialOptionTriggered):
-            sparam.result()
-            raise
-        except InvalidParam:
-            if argv.current_node is sparam.command:
-                sparam.result()
-            else:
-                analyser.subcommands_result[sparam.command.dest] = sparam.result()
-            raise
-        except AlconnaException:
-            analyser.subcommands_result[sparam.command.dest] = sparam.result()
-            raise
-        else:
-            analyser.subcommands_result[sparam.command.dest] = sparam.result()
-    elif analyser.extra_allow:
-        analyser.args_result.setdefault("$extra", []).append(_text)
-        argv.next(seps, move=True)
-    else:
-        return False
-    analyser.sentences.clear()
-    argv.current_node = None
-    return True
-
-
-def _header_handle0(header: "Header[set[str], TPattern]", argv: Argv):
-    content = header.content
-    head_text, _str = argv.next()
-    if _str:
-        if head_text in content:
-            return HeadResult(head_text, head_text, True, fixes=header.mapping)
-        if header.compact and (mat := header.compact_pattern.match(head_text)):
-            argv.rollback(head_text[len(mat[0]):], replace=True)
-            return HeadResult(mat[0], mat[0], True, mat.groupdict(), header.mapping)
-    may_cmd, _m_str = argv.next()
-    if _m_str:
-        cmd = f"{head_text}{argv.separators[0]}{may_cmd}"
-        if cmd in content:
-            return HeadResult(cmd, cmd, True, fixes=header.mapping)
-        if header.compact and (mat := header.compact_pattern.match(cmd)):
-            argv.rollback(cmd[len(mat[0]):], replace=True)
-            return HeadResult(mat[0], mat[0], True, mat.groupdict(), header.mapping)
-    _after_analyse_header(header, argv, head_text, may_cmd, _str, _m_str)
-
-
-def _header_handle1(header: "Header[TPattern, TPattern]", argv: Argv):
-    content = header.content
-    head_text, _str = argv.next()
-    if _str:
-        if mat := content.fullmatch(head_text):
-            return HeadResult(head_text, head_text, True, mat.groupdict(), header.mapping)
-        if header.compact and (mat := header.compact_pattern.match(head_text)):
-            argv.rollback(head_text[len(mat[0]):], replace=True)
-            return HeadResult(mat[0], mat[0], True, mat.groupdict(), header.mapping)
-    may_cmd, _m_str = argv.next()
-    if _m_str:
-        cmd = f"{head_text}{argv.separators[0]}{may_cmd}"
-        if mat := content.fullmatch(cmd):
-            return HeadResult(cmd, cmd, True, mat.groupdict(), header.mapping)
-        if header.compact and (mat := header.compact_pattern.match(cmd)):
-            argv.rollback(cmd[len(mat[0]):], replace=True)
-            return HeadResult(mat[0], mat[0], True, mat.groupdict(), header.mapping)
-    _after_analyse_header(header, argv, head_text, may_cmd, _str, _m_str)
-
-
-def _header_handle2(header: "Header[BasePattern, BasePattern]", argv: Argv):
-    head_text, _str = argv.next()
-    if (val := header.content.validate(head_text)).success:
-        return HeadResult(head_text, val._value, True, fixes=header.mapping)
-    if header.compact and (val := header.compact_pattern.validate(head_text)).success:
-        if _str:
-            argv.rollback(head_text[len(str(val._value)):], replace=True)
-        return HeadResult(val.value, val._value, True, fixes=header.mapping)
-    may_cmd, _m_str = argv.next()
-    _after_analyse_header(header, argv, head_text, may_cmd, _str, _m_str)
-
-
-def _header_handle3(header: "Header[list[Pair], Any]", argv: Argv):
-    head_text, _str = argv.next()
-    may_cmd, _m_str = argv.next()
-    if _m_str:
-        for pair in header.content:
-            if res := pair.match(head_text, may_cmd, argv.rollback, header.compact):
-                return HeadResult(*res, fixes=header.mapping)
-    _after_analyse_header(header, argv, head_text, may_cmd, _str, _m_str)
-
-
-def _header_handle4(header: "Header[Double, Any]", argv: Argv):
-    head_text, _str = argv.next()
-    may_cmd, _m_str = argv.next()
-
-    if res := header.content.match(head_text, may_cmd, _str, _m_str, argv.rollback, header.compact):
-        return HeadResult(*res, fixes=header.mapping)
-    _after_analyse_header(header, argv, head_text, may_cmd, _str, _m_str)
-
-
-HEAD_HANDLES: dict[int, Callable[[Header, Argv], HeadResult]] = {
-    0: _header_handle0,
-    1: _header_handle1,
-    2: _header_handle2,
-    3: _header_handle3,
-    4: _header_handle4,
-}
-
-
-def _after_analyse_header(header: Header, argv: Argv, head_text: Any, may_cmd: Any, _str: bool, _m_str: bool) -> NoReturn:
-    if _str:
-        argv.rollback(may_cmd)
-        if argv.fuzzy_match:
-            _handle_fuzzy(header, head_text, argv.fuzzy_threshold)
-        raise InvalidParam(lang.require("header", "error").format(target=head_text), head_text)
-    if _m_str and may_cmd:
-        if argv.fuzzy_match:
-            _handle_fuzzy(header, f"{head_text}{argv.separators[0]}{may_cmd}", argv.fuzzy_threshold)
-        raise InvalidParam(lang.require("header", "error").format(target=may_cmd), may_cmd)
-    argv.rollback(may_cmd)
-    raise InvalidParam(lang.require("header", "error").format(target=head_text), None)
-
-
-def _handle_fuzzy(header: Header, source: str, threshold: float):
-    command = header.origin[0]
-    if not header.origin[1]:
-        headers_text = [str(command)]
-    else:
-        headers_text = []
-        for prefix in header.origin[1]:
-            if isinstance(prefix, tuple):
-                headers_text.append(f"{prefix[0]} {prefix[1]}{command}")
-            elif isinstance(prefix, str):
-                headers_text.append(f"{prefix}{command}")
-            else:
-                headers_text.append(f"{prefix} {command}")
-    for ht in headers_text:
-        if levenshtein(source, ht) >= threshold:
-            raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(target=source, source=ht))
-
-
-def handle_help(analyser: Analyser, argv: Argv):
-    """处理帮助选项触发"""
-    _help_param = [str(i) for i in argv.release(recover=True) if str(i) not in argv.special]
-    output_manager.send(
-        analyser.command.name,
-        lambda: analyser.command.formatter.format_node(_help_param),
-    )
-    return analyser.export(argv, True, SpecialOptionTriggered("help"))
-
-
-_args = Args["action?", "delete|list"]["name?", str]["command", str, "$"]
-
-
-def handle_shortcut(analyser: Analyser, argv: Argv):
-    """处理快捷命令触发"""
-    argv.next()
-    try:
-        opt_v = analyse_args(argv, _args)
-    except SpecialOptionTriggered:
-        return handle_completion(analyser, argv)
-    try:
-        if opt_v.get("action") == "list":
-            data = analyser.command.get_shortcuts()
-            output_manager.send(analyser.command.name, lambda: "\n".join(data))
-        else:
-            if not opt_v.get("name"):
-                raise ArgumentMissing(lang.require("shortcut", "name_require"))
-            if opt_v.get("action") == "delete":
-                msg = analyser.command.shortcut(opt_v["name"], delete=True)
-            elif opt_v["command"] == "_":
-                msg = analyser.command.shortcut(opt_v["name"], None)
-            elif opt_v["command"] == "$":
-                msg = analyser.command.shortcut(opt_v["name"], fuzzy=True)
-            else:
-                msg = analyser.command.shortcut(opt_v["name"], fuzzy=True, command=opt_v["command"])
-            output_manager.send(analyser.command.name, lambda: msg)
-    except Exception as e:
-        output_manager.send(analyser.command.name, lambda: str(e))
-    return analyser.export(argv, True, SpecialOptionTriggered("shortcut"))
-
-
-INDEX_SLOT = re.compile(r"\{%(\d+)\}")
-WILDCARD_SLOT = re.compile(r"\{\*(.*)\}", re.DOTALL)
-
-
-def _gen_extend(data: list, sep: str):
-    extend = []
-    for slot in data:
-        if isinstance(slot, str) and extend and isinstance(extend[-1], str):
-            extend[-1] += sep + slot
-        else:
-            extend.append(slot)
-    return extend
-
-
-def _handle_multi_slot(argv: Argv, unit: str, data: list, index: int, current: int, offset: int):
-    slot = data[index]
-    if not isinstance(slot, str):
-        left, right = unit.split(f"{{%{index}}}", 1)
-        if left.strip():
-            argv.raw_data[current] = left.strip()
-        argv.raw_data.insert(current + 1, slot)
-        if right.strip():
-            argv.raw_data[current + 2] = right.strip()
-            offset += 1
-    else:
-        argv.raw_data[current + offset] = unescape(unit.replace(f"{{%{index}}}", slot))
-    return offset
-
-
-def _handle_shortcut_data(argv: Argv, data: list):
-    data_len = len(data)
-    record = set()
-    offset = 0
-    for i, unit in enumerate(argv.raw_data.copy()):
-        if not isinstance(unit, str):
-            continue
-        unit = escape(unit)
-        if mat := INDEX_SLOT.fullmatch(unit):
-            index = int(mat[1])
-            if index >= data_len:
-                continue
-            argv.raw_data[i + offset] = data[index]
-            record.add(index)
-        elif res := INDEX_SLOT.findall(unit):
-            for index in map(int, res):
-                if index >= data_len:
-                    continue
-                offset = _handle_multi_slot(argv, unit, data, index, i, offset)
-                record.add(index)
-        elif mat := WILDCARD_SLOT.search(unit):
-            extend = _gen_extend(data, mat[1] or " ")
-            if unit == f"{{*{mat[1]}}}":
-                argv.raw_data.extend(extend)
-            else:
-                argv.raw_data[i + offset] = unescape(unit.replace(f"{{*{mat[1]}}}", "".join(map(str, extend))))
-            data.clear()
-            break
-    return [unit for i, unit in enumerate(data) if i not in record]
-
-
-INDEX_REG_SLOT = re.compile(r"\{(\d+)\}")
-KEY_REG_SLOT = re.compile(r"\{(\w+)\}")
-
-
-def _handle_shortcut_reg(argv: Argv, groups: tuple[str, ...], gdict: dict[str, str], wrapper: ShortcutRegWrapper):
-    data = []
-    for unit in argv.raw_data:
-        if not isinstance(unit, str):
-            data.append(unit)
-            continue
-        unit = escape(unit)
-        if mat := INDEX_REG_SLOT.fullmatch(unit):
-            index = int(mat[1])
-            if index >= len(groups):
-                continue
-            slot = groups[index]
-            data.append(wrapper(index, slot))
-            continue
-        if mat := KEY_REG_SLOT.fullmatch(unit):
-            key = mat[1]
-            if key not in gdict:
-                continue
-            slot = gdict[key]
-            data.append(wrapper(key, slot))
-            continue
-        if mat := INDEX_REG_SLOT.findall(unit):
-            for index in map(int, mat):
-                if index >= len(groups):
-                    unit = unit.replace(f"{{{index}}}", "")
-                    continue
-                slot = groups[index]
-                unit = unit.replace(f"{{{index}}}", str(wrapper(index, slot) or ""))
-        if mat := KEY_REG_SLOT.findall(unit):
-            for key in mat:
-                if key not in gdict:
-                    unit = unit.replace(f"{{{key}}}", "")
-                    continue
-                slot = gdict[key]
-                unit = unit.replace(f"{{{key}}}", str(wrapper(key, slot) or ""))
-        if unit:
-            data.append(unescape(unit))
-    return data
-
-
-def _prompt_unit(analyser: Analyser, argv: Argv, trig: Arg):
-    if not (comp := trig.field.get_completion()):
-        return [Prompt(analyser.command.formatter.param(trig), False)]
-    if isinstance(comp, str):
-        return [Prompt(f"{trig.name}: {comp}", False)]
-    releases = argv.release(recover=True)
-    target = str(releases[-1]) or str(releases[-2])
-    o = list(filter(lambda x: target in x, comp)) or comp
-    return [Prompt(f"{trig.name}: {i}", False, target) for i in o]
-
-
-def _prompt_sentence(analyser: Analyser):
-    res: list[str] = []
-    s_len = len(stc := analyser.sentences)
-    for opt in filter(
-        lambda x: len(x.requires) >= s_len and x.requires[s_len - 1] == stc[-1],
-        analyser.command.options,
-    ):
-        if len(opt.requires) > s_len:
-            res.append(opt.requires[s_len])
-        else:
-            res.extend(opt.aliases if isinstance(opt, Option) else [opt.name])
-    return [Prompt(i) for i in res]
-
-
-def _prompt_none(analyser: Analyser, argv: Argv, got: list[str]):
-    res: list[Prompt] = []
-    if not analyser.args_result and analyser.self_args.argument:
-        unit = analyser.self_args.argument[0]
-        if not (comp := unit.field.get_completion()):
-            res.append(Prompt(analyser.command.formatter.param(unit), False))
-        elif isinstance(comp, str):
-            res.append(Prompt(f"{unit.name}: {comp}", False))
-        else:
-            res.extend(Prompt(f"{unit.name}: {i}", False) for i in comp)
-    for opt in filter(
-        lambda x: x.name not in (argv.special if len(analyser.command.options) > 3 else argv.completion_names),
-        analyser.command.options,
-    ):
-        if opt.requires and all(opt.requires[0] not in i for i in got):
-            res.append(Prompt(opt.requires[0]))
-        elif opt.dest not in got:
-            res.extend([Prompt(al) for al in opt.aliases] if isinstance(opt, Option) else [Prompt(opt.name)])
-    return res
-
-
-def prompt(analyser: Analyser, argv: Argv, trigger: str | None = None):
-    """获取补全列表"""
-    _trigger = trigger or argv.current_node
-    got = [*analyser.options_result.keys(), *analyser.subcommands_result.keys(), *analyser.sentences]
-    if isinstance(_trigger, Arg):
-        return _prompt_unit(analyser, argv, _trigger)
-    elif isinstance(_trigger, Subcommand):
-        return [Prompt(i) for i in analyser.get_sub_analyser(_trigger).compile_params]  # type: ignore
-    elif isinstance(_trigger, str):
-        res = list(filter(lambda x: _trigger in x, analyser.compile_params))
-        if not res:
-            return []
-        out = [i for i in res if i not in got]
-        return [Prompt(i, True, _trigger) for i in (out or res)]
-    releases = argv.release(recover=True)
-    target = str(releases[-1]) or str(releases[-2])
-    if _res := list(filter(lambda x: target in x and target != x, analyser.compile_params)):
-        out = [i for i in _res if i not in got]
-        return [Prompt(i, True, target) for i in (out or _res)]
-    return _prompt_sentence(analyser) if analyser.sentences else _prompt_none(analyser, argv, got)
-
-
-def handle_completion(analyser: Analyser, argv: Argv, trigger: str | None = None):
-    """处理补全选项触发"""
-    if res := prompt(analyser, argv, trigger):
-        if comp_ctx.get(None):
-            raise PauseTriggered(res, trigger, argv)
-        prompt_other = lang.require("completion", "prompt_other")
-        node = lang.require('completion', 'node')
-        node = f"{node}\n" if node else ""
-        output_manager.send(
-            analyser.command.name,
-            lambda: f"{node}{prompt_other}" + f"\n{prompt_other}".join([i.text for i in res]),
-        )
-    return analyser.export(argv, True, SpecialOptionTriggered("completion"))  # type: ignore
+from __future__ import annotations
+
+import re
+from typing import TYPE_CHECKING, Any, Iterable
+
+from nepattern import ANY, AnyString, BasePattern, STRING
+from nepattern.util import TPattern
+from tarina import Empty, lang, split_once
+
+from ..action import Action
+from ..args import Arg, Args
+from ..base import Option, Subcommand
+from ..completion import Prompt, comp_ctx
+from ..config import config
+from ..exceptions import (
+    ArgumentMissing, FuzzyMatchSuccess, ParamsUnmatched, PauseTriggered, SpecialOptionTriggered
+)
+from ..model import HeadResult, OptionResult
+from ..output import output_manager
+from ..typing import KWBool
+from ._header import Double, Header
+from ._util import levenshtein, escape, unescape
+
+if TYPE_CHECKING:
+    from ._analyser import Analyser, SubAnalyser
+    from ._argv import Argv
+
+pat = re.compile("(?:-*no)?-*(?P<name>.+)")
+
+
+def _validate(argv: Argv, target: Arg[Any], value: BasePattern[Any], result: dict[str, Any], arg: Any, _str: bool):
+    if value == ANY or (value == STRING and _str):
+        result[target.name] = arg
+        return
+    if value == AnyString:
+        result[target.name] = str(arg)
+        return
+    default_val = target.field.default
+    res = value.validate(arg, default_val)
+    if res.flag != 'valid':
+        argv.rollback(arg)
+    if res.flag == 'error':
+        if target.optional:
+            return
+        raise ParamsUnmatched(*res.error().args)
+    result[target.name] = res._value  # noqa
+
+def step_varpos(argv: Argv, args: Args, result: dict[str, Any]):
+    value, arg = args.argument.var_positional
+    argv.context = arg
+    key = arg.name
+    default_val = arg.field.default
+    _result = []
+    kwonly_seps = tuple(arg.value.sep for arg in args.argument.keyword_only.values())  # type: ignore
+    loop = len(argv.release(arg.separators))
+    if value.length > 0:
+        loop = min(loop, value.length)
+    for _ in range(loop):
+        may_arg, _str = argv.next(arg.separators)
+        if _str and may_arg in argv.special:
+            raise SpecialOptionTriggered(argv.special[may_arg])
+        if not may_arg or (_str and may_arg in argv.param_ids):
+            argv.rollback(may_arg)
+            break
+        if (
+            _str and kwonly_seps and
+            split_once(pat.match(may_arg)["name"], kwonly_seps, argv.filter_crlf)[0] in args.argument.keyword_only
+        ):
+            argv.rollback(may_arg)
+            break
+        if _str and args.argument.var_keyword and args.argument.var_keyword[0].base.sep in may_arg:  # type: ignore
+            argv.rollback(may_arg)
+            break
+        if (res := value.base.exec(may_arg)).flag != 'valid':
+            argv.rollback(may_arg)
+            break
+        _result.append(res._value)  # noqa
+    if not _result:
+        if default_val is not None:
+            _result = default_val if isinstance(default_val, Iterable) else ()
+        elif value.flag == '*':
+            _result = ()
+        else:
+            raise ArgumentMissing(lang.require("args", "missing").format(key=key))
+    result[key] = tuple(_result)
+
+def step_varkey(argv: Argv, args: Args, result: dict[str, Any]):
+    value, arg = args.argument.var_keyword
+    argv.context = arg
+    name = arg.name
+    default_val = arg.field.default
+    _result = {}
+    loop = len(argv.release(arg.separators))
+    if value.length > 0:
+        loop = min(loop, value.length)
+    for _ in range(loop):
+        may_arg, _str = argv.next(arg.separators)
+        if _str and may_arg in argv.special:
+            raise SpecialOptionTriggered(argv.special[may_arg])
+        if not may_arg or (_str and may_arg in argv.param_ids) or not _str:
+            argv.rollback(may_arg)
+            break
+        if not (_kwarg := re.match(fr'^(-*[^{value.base.sep}]+){value.base.sep}(.*?)$', may_arg)):
+            argv.rollback(may_arg)
+            break
+        key = _kwarg[1]
+        if not (_m_arg := _kwarg[2]):
+            _m_arg, _ = argv.next(arg.separators)
+        if (res := value.base.base.exec(_m_arg)).flag != 'valid':
+            argv.rollback(may_arg)
+            break
+        _result[key] = res._value  # noqa
+    if not _result:
+        if default_val is not None:
+            _result = default_val if isinstance(default_val, dict) else {}
+        elif value.flag == '*':
+            _result = {}
+        else:
+            raise ArgumentMissing(lang.require("args", "missing").format(key=name))
+    result[name] = _result
+
+def step_keyword(argv: Argv, args: Args, result: dict[str, Any]):
+    kwonly_seps = set()
+    for arg in args.argument.keyword_only.values():
+        kwonly_seps.update(arg.separators)
+    kwonly_seps1 = tuple(arg.value.sep for arg in args.argument.keyword_only.values())  # type: ignore
+    target = len(args.argument.keyword_only)
+    count = 0
+    while count < target:
+        may_arg, _str = argv.next(tuple(kwonly_seps))
+        if _str and may_arg in argv.special:
+            raise SpecialOptionTriggered(argv.special[may_arg])
+        if not may_arg or not _str:
+            argv.rollback(may_arg)
+            break
+        key, _m_arg = split_once(may_arg, kwonly_seps1, argv.filter_crlf)
+        _key = pat.match(key)["name"]
+        if _key not in args.argument.keyword_only:
+            _key = key
+        if _key not in args.argument.keyword_only:
+            argv.rollback(may_arg)
+            if args.argument.var_keyword or (_str and may_arg in argv.param_ids):
+                break
+            for arg in args.argument.keyword_only.values():
+                if arg.value.base.exec(may_arg).flag == 'valid':  # type: ignore
+                    raise ParamsUnmatched(lang.require("args", "key_missing").format(target=may_arg, key=arg.name))
+            for name in args.argument.keyword_only:
+                if levenshtein(_key, name) >= config.fuzzy_threshold:
+                    raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=name, target=_key))
+            raise ParamsUnmatched(lang.require("args", "key_not_found").format(name=_key))
+        arg = args.argument.keyword_only[_key]
+        value = arg.value.base  # type: ignore
+        if not _m_arg:
+            if isinstance(value, KWBool):
+                _m_arg = key
+            else:
+                _m_arg, _ = argv.next(args.argument.keyword_only[_key].separators)
+        _validate(argv, arg, value, result, _m_arg, _str)
+        count += 1
+
+    if count < target:
+        for key, arg in args.argument.keyword_only.items():
+            if key in result:
+                continue
+            if arg.field.default is not None:
+                result[key] = None if arg.field.default is Empty else arg.field.default
+            elif not arg.optional:
+                raise ArgumentMissing(lang.require("args", "missing").format(key=key))
+
+def analyse_args(argv: Argv, args: Args) -> dict[str, Any]:
+    """
+    分析 `Args` 部分
+
+    Args:
+        argv (Argv): 命令行参数
+        args (Args): 目标 `Args`
+
+    Returns:
+        dict[str, Any]: 解析结果
+    """
+    result: dict[str, Any] = {}
+    for arg in args.argument.normal:
+        argv.context = arg
+        may_arg, _str = argv.next(arg.separators)
+        if _str and may_arg in argv.special:
+            raise SpecialOptionTriggered(argv.special[may_arg])
+        if _str and may_arg in argv.param_ids and arg.optional:
+            if (de := arg.field.default) is not None:
+                result[arg.name] = None if de is Empty else de
+            argv.rollback(may_arg)
+            continue
+        if not may_arg:
+            argv.rollback(may_arg)
+            if (de := arg.field.default) is not None:
+                result[arg.name] = None if de is Empty else de
+            elif not arg.optional:
+                raise ArgumentMissing(lang.require("args", "missing").format(key=arg.name))
+            continue
+        value = arg.value
+        if value.alias == "*":
+            argv.rollback(may_arg)
+            result[arg.name] = argv.converter(argv.release(arg.separators))
+            argv.current_index = argv.ndata
+            return result
+        _validate(argv, arg, value, result, may_arg, _str)
+    if args.argument.unpack:
+        arg, unpack = args.argument.unpack
+        try:
+            unpack.separate(*arg.separators)
+            result[arg.name] = arg.value.origin(**analyse_args(argv, unpack))
+        except Exception as e:
+            if (de := arg.field.default) is not None:
+                result[arg.name] = None if de is Empty else de
+            elif not arg.optional:
+                raise e
+    if args.argument.var_positional:
+        step_varpos(argv, args, result)
+    if args.argument.keyword_only:
+        step_keyword(argv, args, result)
+    if args.argument.var_keyword:
+        step_varkey(argv, args, result)
+    argv.context = None
+    return result
+
+
+def handle_option(argv: Argv, opt: Option) -> tuple[str, OptionResult]:
+    """
+    处理 `Option` 部分
+
+    Args:
+        argv (Argv): 命令行参数
+        opt (Option): 目标 `Option`
+    """
+    argv.context = opt
+    _cnt = 0
+    error = True
+    name, _ = argv.next(opt.separators)
+    if opt.compact:
+        for al in opt.aliases:
+            if mat := re.fullmatch(f"{al}(?P<rest>.*?)", name):
+                argv.rollback(mat['rest'], replace=True)
+                error = False
+                break
+    elif opt.action.type == 2:
+        for al in opt.aliases:
+            if name.startswith(al) and (cnt := (len(name.lstrip("-")) / len(al.lstrip("-")))).is_integer():
+                _cnt = int(cnt)
+                error = False
+                break
+    elif name in opt.aliases:
+        error = False
+    if error:
+        if argv.fuzzy_match and levenshtein(name, opt.name) >= config.fuzzy_threshold:
+            raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=name, target=opt.name))
+        raise ParamsUnmatched(lang.require("option", "name_error").format(source=opt.name, target=name))
+    name = opt.dest
+    return (
+        (name, OptionResult(None, analyse_args(argv, opt.args)))
+        if opt.nargs
+        else (name, OptionResult(_cnt or opt.action.value))
+    )
+
+
+def handle_action(param: Option, source: OptionResult, target: OptionResult):
+    """处理 `Option` 的 `action`"""
+    if param.action.type == 0:
+        return target
+    if param.action.type == 2:
+        if not param.nargs:
+            source.value += target.value
+            return source
+        return target
+    if not param.nargs:
+        source.value = source.value[:]
+        source.value.extend(target.value)
+    else:
+        for key, value in target.args.items():
+            if key in source.args:
+                source.args[key].append(value)
+            else:
+                source.args[key] = [value]
+    return source
+
+
+def analyse_option(analyser: SubAnalyser, argv: Argv, opt: Option):
+    """
+    分析 `Option` 部分
+
+    Args:
+        analyser (SubAnalyser): 当前解析器
+        argv (Argv): 命令行参数
+        opt (Option): 目标 `Option`
+    """
+    opt_n, opt_v = handle_option(argv, opt)
+    if opt_n not in analyser.options_result:
+        analyser.options_result[opt_n] = opt_v
+        if opt.action.type == 1 and opt_v.args:
+            for key in list(opt_v.args.keys()):
+                opt_v.args[key] = [opt_v.args[key]]
+    else:
+        analyser.options_result[opt_n] = handle_action(opt, analyser.options_result[opt_n], opt_v)
+
+
+def analyse_compact_params(analyser: SubAnalyser, argv: Argv):
+    """分析紧凑参数
+
+    Args:
+        analyser (SubAnalyser): 当前解析器
+        argv (Argv): 命令行参数
+    """
+    for param in analyser.compact_params:
+        _data, _index = argv.data_set()
+        try:
+            if param.__class__ is Option:
+                analyse_option(analyser, argv, param)
+            else:
+                try:
+                    param.process(argv)
+                finally:
+                    analyser.subcommands_result[param.command.dest] = param.result()
+            _data.clear()
+            return True
+        except ParamsUnmatched as e:
+            if argv.context.__class__ is Arg:
+                raise e
+            argv.data_reset(_data, _index)
+
+
+def handle_opt_default(defaults: dict[str, tuple[OptionResult, Action]], data: dict[str, OptionResult]):
+    for k, v in defaults.items():
+        if k not in data:
+            data[k] = v[0]
+        if not v[0].args:
+            continue
+        for key, value in v[0].args.items():
+            data[k].args.setdefault(key, [value] if v[1].value == 1 else value)
+
+
+def analyse_param(analyser: SubAnalyser, argv: Argv, seps: tuple[str, ...] | None = None):
+    """处理参数
+
+    Args:
+        analyser (SubAnalyser): 当前解析器
+        argv (Argv): 命令行参数
+        seps (tuple[str, ...], optional): 指定的分隔符.
+    """
+    _text, _str = argv.next(seps, move=False)
+    if _str and _text in argv.special:
+        if _text in argv.completion_names:
+            if argv.current_index < argv.ndata:
+                argv.bak_data = argv.bak_data[:argv.current_index+1]
+            last = argv.bak_data[-1]
+            argv.bak_data[-1] = last[:last.rfind(_text)]
+        raise SpecialOptionTriggered(argv.special[_text])
+    if not _str or not _text:
+        _param = None
+    elif _text in analyser.compile_params:
+        _param = analyser.compile_params[_text]
+    elif analyser.compact_params and (res := analyse_compact_params(analyser, argv)):
+        if res.__class__ is str:
+            raise ParamsUnmatched(res)
+        argv.context = None
+        return True
+    else:
+        _param = None
+    if not _param and analyser.command.nargs and not analyser.args_result:
+        analyser.args_result = analyse_args(argv, analyser.self_args)
+        if analyser.args_result:
+            argv.context = None
+            return True
+    if _param.__class__ is Option:
+        analyse_option(analyser, argv, _param)
+    elif _param.__class__ is list:
+        exc: Exception | None = None
+        for opt in _param:
+            _data, _index = argv.data_set()
+            try:
+                analyse_option(analyser, argv, opt)
+                _data.clear()
+                exc = None
+                break
+            except Exception as e:
+                exc = e
+                argv.data_reset(_data, _index)
+        if exc:
+            raise exc  # type: ignore  # noqa
+    elif _param is not None:
+        try:
+            _param.process(argv)
+        finally:
+            analyser.subcommands_result[_param.command.dest] = _param.result()
+    else:
+        return False
+    argv.context = None
+    return True
+
+
+def analyse_header(header: Header, argv: Argv) -> HeadResult:
+    """分析头部
+
+    Args:
+        header (Header): 头部
+        argv (Argv): 命令行参数
+
+    Returns:
+        HeadResult: 分析结果
+    """
+    content = header.content
+    mapping = header.mapping
+    head_text, _str = argv.next()
+    if _str:
+        if content.__class__ is set and head_text in content:
+            return HeadResult(head_text, head_text, True, fixes=mapping)
+        elif content.__class__ is TPattern and (mat := content.fullmatch(head_text)):
+            return HeadResult(head_text, head_text, True, mat.groupdict(), mapping)
+        if header.compact and content.__class__ in (set, TPattern) and (mat := header.compact_pattern.match(head_text)):
+            argv.rollback(head_text[len(mat[0]):], replace=True)
+            return HeadResult(mat[0], mat[0], True, mat.groupdict(), mapping)
+    if isinstance(content, BasePattern):
+        if (val := content.validate(head_text)).success:
+            return HeadResult(head_text, val._value, True, fixes=mapping)
+        if header.compact and (val := header.compact_pattern.validate(head_text)).success:
+            if _str:
+                argv.rollback(head_text[len(str(val._value)):], replace=True)
+            return HeadResult(val.value, val._value, True, fixes=mapping)
+
+    may_cmd, _m_str = argv.next()
+    if content.__class__ is list and _m_str:
+        for pair in content:
+            if res := pair.match(head_text, may_cmd, argv.rollback, header.compact):
+                return HeadResult(*res, fixes=mapping)
+    if content.__class__ is Double and (
+        res := content.match(head_text, may_cmd, _str, _m_str, argv.rollback, header.compact)
+    ):
+        return HeadResult(*res, fixes=mapping)
+    if _str:
+        argv.rollback(may_cmd)
+        source = head_text
+    elif _m_str and may_cmd:
+        source = may_cmd
+    else:
+        argv.rollback(may_cmd)
+        raise ParamsUnmatched(lang.require("header", "error").format(target=head_text), None)
+    if argv.fuzzy_match:
+        _handle_fuzzy(header, source)
+    raise ParamsUnmatched(lang.require("header", "error").format(target=source), source)
+
+
+def _handle_fuzzy(header, source):
+    command = header.origin[0]
+    _prefixes = [i for i in header.origin[1] if i.__class__ is str]
+    headers_text = []
+    if _prefixes and _prefixes != [""]:
+        headers_text.extend(f"{i}{command}" for i in _prefixes)
+    elif command:
+        headers_text.append(str(command))
+    if source == command:
+        raise ParamsUnmatched(lang.require("header", "error").format(target=source))
+    for ht in headers_text:
+        if levenshtein(source, ht) >= config.fuzzy_threshold:
+            raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(target=source, source=ht))
+
+
+def handle_help(analyser: Analyser, argv: Argv):
+    """处理帮助选项触发"""
+    _help_param = [str(i) for i in argv.release(recover=True) if str(i) not in argv.special]
+    output_manager.send(
+        analyser.command.name,
+        lambda: analyser.command.formatter.format_node(_help_param),
+    )
+    return analyser.export(argv, True, SpecialOptionTriggered('help'))
+
+
+_args = Args["action?", "delete|list"]["name?", str]["command", str, "$"]
+
+
+def handle_shortcut(analyser: Analyser, argv: Argv):
+    """处理快捷命令触发"""
+    argv.next()
+    try:
+        opt_v = analyse_args(argv, _args)
+    except SpecialOptionTriggered:
+        return handle_completion(analyser, argv)
+    try:
+        if opt_v.get("action") == "list":
+            data = analyser.command.get_shortcuts()
+            output_manager.send(analyser.command.name, lambda: "\n".join(data))
+        else:
+            if not opt_v.get("name"):
+                raise ParamsUnmatched(lang.require("shortcut", "name_require"))
+            if opt_v.get("action") == "delete":
+                msg = analyser.command.shortcut(opt_v["name"], delete=True)
+            elif opt_v["command"] == "_":
+                msg = analyser.command.shortcut(opt_v["name"], None)
+            elif opt_v["command"] == "$":
+                msg = analyser.command.shortcut(opt_v["name"], {})
+            else:
+                msg = analyser.command.shortcut(opt_v["name"], {"command": argv.converter(opt_v["command"])})
+            output_manager.send(analyser.command.name, lambda: msg)
+    except Exception as e:
+        output_manager.send(analyser.command.name, lambda: str(e))
+    return analyser.export(argv, True, SpecialOptionTriggered('shortcut'))
+
+
+INDEX_SLOT = re.compile(r"\{%(\d+)\}")
+WILDCARD_SLOT = re.compile(r"\{\*(.*)\}", re.DOTALL)
+
+def _gen_extend(data: list, sep: str):
+    extend = []
+    for slot in data:
+        if isinstance(slot, str) and extend and isinstance(extend[-1], str):
+            extend[-1] += sep + slot
+        else:
+            extend.append(slot)
+    return extend
+
+def _handle_multi_slot(argv: Argv, unit: str, data: list, index: int, current: int, offset: int):
+    slot = data[index]
+    if not isinstance(slot, str):
+        left, right = unit.split(f"{{%{index}}}", 1)
+        if left.strip():
+            argv.raw_data[current] = left.strip()
+        argv.raw_data.insert(current + 1, slot)
+        if right.strip():
+            argv.raw_data[current + 2] = right.strip()
+            offset += 1
+    else:
+        argv.raw_data[current + offset] =  unescape(unit.replace(f"{{%{index}}}", slot))
+    return offset
+
+def _handle_shortcut_data(argv: Argv, data: list):
+    data_len = len(data)
+    if not data_len:
+        return []
+    record = set()
+    offset = 0
+    for i, unit in enumerate(argv.raw_data.copy()):
+        if not isinstance(unit, str):
+            continue
+        unit = escape(unit)
+        if mat := INDEX_SLOT.fullmatch(unit):
+            index = int(mat[1])
+            if index >= data_len:
+                continue
+            argv.raw_data[i + offset] = data[index]
+            record.add(index)
+        elif res := INDEX_SLOT.findall(unit):
+            for index in map(int, res):
+                if index >= data_len:
+                    continue
+                offset = _handle_multi_slot(argv, unit, data, index, i, offset)
+                record.add(index)
+        elif mat := WILDCARD_SLOT.search(unit):
+            extend = _gen_extend(data, mat[1] or ' ')
+            if unit == f"{{*{mat[1]}}}":
+                argv.raw_data.extend(extend)
+            else:
+                argv.raw_data[i + offset] = unescape(unit.replace(f"{{*{mat[1]}}}", "".join(map(str, extend))))
+            data.clear()
+            break
+    return [unit for i, unit in enumerate(data) if i not in record]
+
+def _handle_shortcut_reg(argv: Argv, groups: tuple[str, ...], gdict: dict[str, str]):
+    for j, unit in enumerate(argv.raw_data):
+        if not isinstance(unit, str):
+            continue
+        unit = escape(unit)
+        for i, c in enumerate(groups):
+            unit = unit.replace(f"{{{i}}}", c)
+        for k, v in gdict.items():
+            unit = unit.replace(f"{{{k}}}", v)
+        argv.raw_data[j] = unescape(unit)
+
+def _prompt_unit(analyser: Analyser, argv: Argv, trig: Arg):
+    if trig.field.completion:
+        comp = trig.field.completion()
+        if isinstance(comp, str):
+            return [Prompt(comp, False)]
+        releases = argv.release(recover=True)
+        target = str(releases[-1]) or str(releases[-2])
+        o = list(filter(lambda x: target in x, comp)) or comp
+        return [Prompt(i, False, target) for i in o]
+    return [Prompt(analyser.command.formatter.param(trig), False)]
+
+
+def _prompt_none(analyser: Analyser, argv: Argv, got: list[str]):
+    res: list[Prompt] = []
+    if not analyser.args_result and analyser.self_args.argument:
+        unit = analyser.self_args.argument[0]
+        if gen := unit.field.completion:
+            res.extend([Prompt(comp, False)] if isinstance(comp := gen(), str) else [Prompt(i, False) for i in comp])
+        else:
+            res.append(Prompt(analyser.command.formatter.param(unit), False))
+    for opt in filter(
+        lambda x: x.name not in argv.completion_names,
+        analyser.command.options,
+    ):
+        if opt.dest not in got:
+            res.extend([Prompt(al) for al in opt.aliases] if isinstance(opt, Option) else [Prompt(opt.name)])
+    return res
+
+
+def prompt(analyser: Analyser, argv: Argv, trigger: str | None = None):
+    """获取补全列表"""
+    _trigger = trigger or argv.context
+    got = [*analyser.options_result.keys(), *analyser.subcommands_result.keys()]
+    if isinstance(_trigger, Arg):
+        return _prompt_unit(analyser, argv, _trigger)
+    elif isinstance(_trigger, Subcommand):
+        return [Prompt(i) for i in analyser.get_sub_analyser(_trigger).compile_params]
+    elif isinstance(_trigger, str):
+        res = list(filter(lambda x: _trigger in x, analyser.compile_params))
+        if not res:
+            return []
+        out = [i for i in res if i not in got]
+        return [Prompt(i, True, _trigger) for i in (out or res)]
+    releases = argv.release(recover=True)
+    target = str(releases[-1]) or str(releases[-2])
+    if _res := list(filter(lambda x: target in x and target != x, analyser.compile_params)):
+        out = [i for i in _res if i not in got]
+        return [Prompt(i, True, target) for i in (out or _res)]
+    return _prompt_none(analyser, argv, got)
+
+
+def handle_completion(analyser: Analyser, argv: Argv, trigger: str | None = None):
+    """处理补全选项触发"""
+    if res := prompt(analyser, argv, trigger):
+        if comp_ctx.get(None):
+            raise PauseTriggered(res)
+        output_manager.send(
+            analyser.command.name,
+            lambda: f"{lang.require('completion', 'node')}\n* " + "\n* ".join([i.text for i in res]),
+        )
+    return analyser.export(argv, True, SpecialOptionTriggered('completion'))  # type: ignore
```

### Comparing `arclet_alconna-1.8.8/src/arclet/alconna/_internal/_util.py` & `arclet_alconna-2.0.0a1/src/arclet/alconna/_internal/_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-def levenshtein(source: str, target: str) -> float:
-    """`编辑距离算法`_, 计算源字符串与目标字符串的相似度, 取值范围[0, 1], 值越大越相似
-
-    Args:
-        source (str): 源字符串
-        target (str): 目标字符串
-
-    .. _编辑距离算法:
-        https://en.wikipedia.org/wiki/Levenshtein_distance
-
-    """
-    l_s, l_t = len(source), len(target)
-    s_range, t_range = range(l_s + 1), range(l_t + 1)
-    matrix = [[(i if j == 0 else j) for j in t_range] for i in s_range]
-
-    for i in s_range[1:]:
-        for j in t_range[1:]:
-            sub_distance = matrix[i - 1][j - 1] + (0 if source[i - 1] == target[j - 1] else 1)
-            matrix[i][j] = min(matrix[i - 1][j] + 1, matrix[i][j - 1] + 1, sub_distance)
-
-    return 1 - float(matrix[l_s][l_t]) / max(l_s, l_t)
-
-
-ESCAPE = {"\\": "\x00", "[": "\x01", "]": "\x02", "{": "\x03", "}": "\x04", "|": "\x05"}
-R_ESCAPE = {v: k for k, v in ESCAPE.items()}
-
-
-def escape(string: str) -> str:
-    """转义字符串"""
-    for k, v in ESCAPE.items():
-        string = string.replace("\\" + k, v)
-    return string
-
-
-def unescape(string: str) -> str:
-    """逆转义字符串, 自动去除空白符"""
-    for k, v in R_ESCAPE.items():
-        string = string.replace(k, v)
-    return string.strip()
+def levenshtein(source: str, target: str) -> float:
+    """ `编辑距离算法`_, 计算源字符串与目标字符串的相似度, 取值范围[0, 1], 值越大越相似
+
+    Args:
+        source (str): 源字符串
+        target (str): 目标字符串
+
+    .. _编辑距离算法:
+        https://en.wikipedia.org/wiki/Levenshtein_distance
+
+    """
+    l_s, l_t = len(source), len(target)
+    s_range, t_range = range(l_s + 1), range(l_t + 1)
+    matrix = [[(i if j == 0 else j) for j in t_range] for i in s_range]
+
+    for i in s_range[1:]:
+        for j in t_range[1:]:
+            sub_distance = matrix[i - 1][j - 1] + (0 if source[i - 1] == target[j - 1] else 1)
+            matrix[i][j] = min(matrix[i - 1][j] + 1, matrix[i][j - 1] + 1, sub_distance)
+
+    return 1 - float(matrix[l_s][l_t]) / max(l_s, l_t)
+
+
+ESCAPE = {"\\": "\x00", "[": "\x01", "]": "\x02", "{": "\x03", "}": "\x04", "|": "\x05"}
+R_ESCAPE = {v: k for k, v in ESCAPE.items()}
+
+
+def escape(string: str) -> str:
+    """转义字符串"""
+    for k, v in ESCAPE.items():
+        string = string.replace("\\" + k, v)
+    return string
+
+
+def unescape(string: str) -> str:
+    """逆转义字符串, 自动去除空白符 """
+    for k, v in R_ESCAPE.items():
+        string = string.replace(k, v)
+    return string.strip()
```

### Comparing `arclet_alconna-1.8.8/src/arclet/alconna/action.py` & `arclet_alconna-2.0.0a1/src/arclet/alconna/action.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,58 @@
-from dataclasses import dataclass
-from enum import IntEnum
-from typing import Any
-
-
-class ActType(IntEnum):
-    """节点触发的动作类型"""
-
-    STORE = 0
-    """无 Args 时, 仅存储一个值, 默认为 Ellipsis; 有 Args 时, 后续的解析结果会覆盖之前的值"""
-    APPEND = 1
-    """无 Args 时, 将多个值存为列表, 默认为 Ellipsis; 有 Args 时, 每个解析结果会追加到列表中
-    
-    当存在默认值并且不为列表时, 会自动将默认值变成列表, 以保证追加的正确性
-    """
-    COUNT = 2
-    """无 Args 时, 计数器加一; 有 Args 时, 表现与 STORE 相同
-    
-    当存在默认值并且不为数字时, 会自动将默认值变成 1, 以保证计数器的正确性
-    """
-
-
-@dataclass(eq=True, frozen=True)
-class Action:
-    """节点触发的动作"""
-
-    type: ActType
-    value: Any
-
-
-store = Action(ActType.STORE, Ellipsis)
-"""默认的存储动作"""
-store_true = Action(ActType.STORE, True)
-"""存储 True"""
-store_false = Action(ActType.STORE, False)
-"""存储 False"""
-
-append = Action(ActType.APPEND, [Ellipsis])
-"""默认的追加动作"""
-
-count = Action(ActType.COUNT, 1)
-"""默认的计数动作"""
-
-
-def store_value(value: Any):
-    """存储一个值
-
-    Args:
-        value (Any): 待存储的值
-    """
-    return Action(ActType.STORE, value)
-
-
-def append_value(value: Any):
-    """追加值
-
-    Args:
-        value (Any): 待存储的值
-    """
-    return Action(ActType.APPEND, [value])
+from dataclasses import dataclass
+from enum import IntEnum
+from typing import Any
+
+
+class ActType(IntEnum):
+    """节点触发的动作类型"""
+    STORE = 0
+    """无 Args 时, 仅存储一个值, 默认为 Ellipsis; 有 Args 时, 后续的解析结果会覆盖之前的值"""
+    APPEND = 1
+    """无 Args 时, 将多个值存为列表, 默认为 Ellipsis; 有 Args 时, 每个解析结果会追加到列表中
+    
+    当存在默认值并且不为列表时, 会自动将默认值变成列表, 以保证追加的正确性
+    """
+    COUNT = 2
+    """无 Args 时, 计数器加一; 有 Args 时, 表现与 STORE 相同
+    
+    当存在默认值并且不为数字时, 会自动将默认值变成 1, 以保证计数器的正确性
+    """
+
+
+@dataclass(eq=True, frozen=True)
+class Action:
+    """节点触发的动作"""
+    type: ActType
+    value: Any
+
+
+store = Action(ActType.STORE, Ellipsis)
+"""默认的存储动作"""
+store_true = Action(ActType.STORE, True)
+"""存储 True"""
+store_false = Action(ActType.STORE, False)
+"""存储 False"""
+
+append = Action(ActType.APPEND, [Ellipsis])
+"""默认的追加动作"""
+
+count = Action(ActType.COUNT, 1)
+"""默认的计数动作"""
+
+
+def store_value(value: Any):
+    """存储一个值
+
+    Args:
+        value (Any): 待存储的值
+    """
+    return Action(ActType.STORE, value)
+
+
+def append_value(value: Any):
+    """追加值
+
+    Args:
+        value (Any): 待存储的值
+    """
+    return Action(ActType.APPEND, [value])
```

### Comparing `arclet_alconna-1.8.8/src/arclet/alconna/argv.py` & `arclet_alconna-2.0.0a1/src/arclet/alconna/argv.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from __future__ import annotations
-
-from contextvars import ContextVar
-from typing import Any, Callable
-
-from ._internal._argv import Argv as Argv
-from .typing import TDC
-
-__argv_type__: ContextVar[type[Argv]] = ContextVar("argv_type", default=Argv)
-
-
-def set_default_argv_type(argv_type: type[Argv]):
-    """设置默认的命令行参数类型"""
-    __argv_type__.set(argv_type)
-
-
-def argv_config(
-    target: type[Argv] | None = None,
-    preprocessors: dict[type, Callable[..., Any]] | None = None,
-    to_text: Callable[[Any], str | None] | None = None,
-    filter_out: list[type] | None = None,
-    checker: Callable[[Any], bool] | None = None,
-    converter: Callable[[str | list], TDC] | None = None,
-):
-    """配置命令行参数
-
-    Args:
-        target (type[Argv] | None, optional): 目标命令类型.
-        preprocessors (dict[type, Callable[..., Any]] | None, optional): 命令元素的预处理器.
-        to_text (Callable[[Any], str | None] | None, optional): 将命令元素转换为文本, 或者返回None以跳过该元素.
-        filter_out (list[type] | None, optional): 需要过滤掉的命令元素.
-        checker (Callable[[Any], bool] | None, optional): 检查传入命令.
-        converter (Callable[[str | list], TDC] | None, optional): 将字符串或列表转为目标命令类型.
-    """
-    Argv._cache.setdefault(target or __argv_type__.get(), {}).update(
-        {k: v for k, v in locals().items() if v is not None}
-    )
+from __future__ import annotations
+
+from contextvars import ContextVar
+from typing import Any, Callable
+
+from ._internal._argv import Argv as Argv
+from .typing import TDC
+
+__argv_type__: ContextVar[type[Argv]] = ContextVar("argv_type", default=Argv)
+
+
+def set_default_argv_type(argv_type: type[Argv]):
+    """设置默认的命令行参数类型"""
+    __argv_type__.set(argv_type)
+
+
+def argv_config(
+    target: type[Argv] | None = None,
+    preprocessors: dict[type, Callable[..., Any]] | None = None,
+    to_text: Callable[[Any], str | None] | None = None,
+    filter_out: list[type] | None = None,
+    checker: Callable[[Any], bool] | None = None,
+    converter: Callable[[str | list], TDC] | None = None
+):
+    """配置命令行参数
+
+    Args:
+        target (type[Argv] | None, optional): 目标命令类型.
+        preprocessors (dict[type, Callable[..., Any]] | None, optional): 命令元素的预处理器.
+        to_text (Callable[[Any], str | None] | None, optional): 将命令元素转换为文本, 或者返回None以跳过该元素.
+        filter_out (list[type] | None, optional): 需要过滤掉的命令元素.
+        checker (Callable[[Any], bool] | None, optional): 检查传入命令.
+        converter (Callable[[str | list], TDC] | None, optional): 将字符串或列表转为目标命令类型.
+    """
+    Argv._cache.setdefault(
+        target or __argv_type__.get(), {}
+    ).update({k: v for k, v in locals().items() if v is not None})
```

### Comparing `arclet_alconna-1.8.8/src/arclet/alconna/arparma.py` & `arclet_alconna-2.0.0a1/src/arclet/alconna/arparma.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,461 +1,422 @@
-from __future__ import annotations
-
-import inspect
-from abc import ABCMeta, abstractmethod
-from dataclasses import dataclass, field
-from functools import lru_cache
-from types import MappingProxyType
-from typing import Any, Callable, ClassVar, Generic, TypeVar, cast, overload
-from typing_extensions import Self
-
-from tarina import Empty, generic_isinstance, lang, safe_eval
-
-from .exceptions import BehaveCancelled, OutBoundsBehave
-from .model import HeadResult, OptionResult, SubcommandResult
-from .typing import TDC
-
-T = TypeVar("T")
-T1 = TypeVar("T1")
-D = TypeVar("D")
-
-
-def _handle_opt(_pf: str, _parts: list[str], _opts: dict[str, OptionResult]):
-    """处理 `options.xxx.yyy.zzz` 形式的参数"""
-    if _pf == "options":
-        _pf = _parts.pop(0)
-    if not _parts:  # options.foo or foo
-        return _opts, _pf
-    elif not (__src := _opts.get(_pf)):  # options.foo.bar or foo.bar
-        return _opts, _pf
-    if (_end := _parts.pop(0)) == "value":
-        return __src, _end
-    if _end == "args":
-        return (__src.args, _parts.pop(0)) if _parts else (__src, _end)
-    return __src.args, _end
-
-
-def _handle_sub(_pf: str, _parts: list[str], _subs: dict[str, SubcommandResult]):
-    """处理 `subcommands.xxx.yyy.zzz` 形式的参数"""
-    if _pf == "subcommands":
-        _pf = _parts.pop(0)
-    if not _parts:
-        return _subs, _pf
-    elif not (__src := _subs.get(_pf)):
-        return _subs, _pf
-    if (_end := _parts.pop(0)) == "value":
-        return __src, _end
-    if _end == "args":
-        return (__src.args, _parts.pop(0)) if _parts else (__src, _end)
-    if _end == "options" and (_end in __src.options or not _parts):
-        raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=f"{_pf}.{_end}"))
-    if _end == "options" or _end in __src.options:
-        return _handle_opt(_end, _parts, __src.options)
-    if _end == "subcommands" and (_end in __src.subcommands or not _parts):
-        raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=f"{_pf}.{_end}"))
-    if _end == "subcommands" or _end in __src.subcommands:
-        return _handle_sub(_end, _parts, __src.subcommands)
-    return __src.args, _end
-
-
-class _Query(Generic[T]):
-    source: Arparma
-
-    def __get__(self, instance: Arparma, owner: type) -> _Query[T]:
-        self.source = instance
-        return self
-
-    def __set_name__(self, owner, name):
-        self.name = name
-
-    def __getitem__(self, item: type[T1]) -> _Query[T1]:
-        return cast("_Query[T1]", self)
-
-    @overload
-    def __call__(self, path: str) -> T | None:
-        ...
-
-    @overload
-    def __call__(self, path: str, default: D) -> T | D:
-        ...
-
-    def __call__(self, path: str, default: D | None = None) -> T | D | None:
-        """查询 `Arparma` 中的数据
-
-        Args:
-            path (str): 要查询的路径
-            default (T | None, optional): 如果查询失败, 则返回该值
-        """
-        source, endpoint = self.source.__require__(path.split("."))
-        if source is None:
-            return default
-        if isinstance(source, dict):
-            return source.get(endpoint, default) if endpoint else MappingProxyType(source)  # type: ignore
-        return getattr(source, endpoint, default) if endpoint else source  # type: ignore
-
-
-class Arparma(Generic[TDC]):
-    """承载解析结果与操作数据的接口类
-
-    Attributes:
-        origin (TDC): 原始数据
-        matched (bool): 是否匹配
-        header_match (HeadResult): 命令头匹配结果
-        error_info (type[BaseException] | BaseException | str): 错误信息
-        error_data (list[str | Any]): 错误数据
-        main_args (dict[str, Any]): 主参数匹配结果
-        other_args (dict[str, Any]): 其他参数匹配结果
-        options (dict[str, OptionResult]): 选项匹配结果
-        subcommands (dict[str, SubcommandResult]): 子命令匹配结果
-    """
-
-    header_match: HeadResult
-    options: dict[str, OptionResult]
-    subcommands: dict[str, SubcommandResult]
-
-    def __init__(
-        self,
-        source: str,
-        origin: TDC,
-        matched: bool = False,
-        header_match: HeadResult | None = None,
-        error_info: type[Exception] | Exception | None = None,
-        error_data: list[str | Any] | None = None,
-        main_args: dict[str, Any] | None = None,
-        options: dict[str, OptionResult] | None = None,
-        subcommands: dict[str, SubcommandResult] | None = None,
-        ctx: dict[str, Any] | None = None,
-    ):
-        """初始化 `Arparma`
-        Args:
-            source (str): 命令源
-            origin (TDC): 原始数据
-            matched (bool, optional): 是否匹配
-            header_match (HeadResult | None, optional): 命令头匹配结果
-            error_info (type[Exception] | Exception | None, optional): 错误信息
-            error_data (list[str | Any] | None, optional): 错误数据
-            main_args (dict[str, Any] | None, optional): 主参数匹配结果
-            options (dict[str, OptionResult] | None, optional): 选项匹配结果
-            subcommands (dict[str, SubcommandResult] | None, optional): 子命令匹配结果
-            ctx (dict[str, Any] | None, optional): 上下文
-        """
-        self.source = source
-        self.origin = origin
-        self.matched = matched
-        self.header_match = header_match or HeadResult()
-        self.error_info = error_info
-        self.error_data = error_data or []
-        self.main_args = main_args or {}
-        self.other_args = {}
-        self.options = options or {}
-        self.subcommands = subcommands or {}
-        self.context = ctx or {}
-
-    _additional: ClassVar[dict[str, Callable[[], Any]]] = {}
-    query = _Query[Any]()
-
-    def _clr(self):
-        self.context.clear()
-        self.error_data.clear()
-        self.main_args.clear()
-        self.other_args.clear()
-        self.options.clear()
-        self.subcommands.clear()
-        ks = list(self.__dict__.keys())
-        for k in ks:
-            delattr(self, k)
-
-    @property
-    def header(self) -> dict[str, Any]:
-        """返回可能解析到的命令头中的组信息"""
-        return self.header_match.groups
-
-    @property
-    def head_matched(self):
-        """返回命令头是否匹配"""
-        return self.header_match.matched
-
-    @property
-    def header_result(self):
-        """返回命令头匹配结果"""
-        return self.header_match.result
-
-    @property
-    def non_component(self) -> bool:
-        """返回是否没有解析到任何组件"""
-        return not self.subcommands and not self.options
-
-    @property
-    def components(self) -> dict[str, OptionResult | SubcommandResult]:
-        """返回解析到的组件"""
-        return {**self.options, **self.subcommands}
-
-    @property
-    def all_matched_args(self) -> dict[str, Any]:
-        """返回 Alconna 中所有 Args 解析到的值"""
-        return {**self.main_args, **self.other_args}
-
-    @property
-    def token(self) -> int:
-        """返回命令的 Token"""
-        from .manager import command_manager
-
-        return command_manager.get_token(self)
-
-    def _unpack_opts(self, _data):
-        for _v in _data.values():
-            self.other_args = {**self.other_args, **_v.args}
-
-    def _unpack_subs(self, _data):
-        for _v in _data.values():
-            self.other_args = {**self.other_args, **_v.args}
-            if _v.options:
-                self._unpack_opts(_v.options)
-            if _v.subcommands:
-                self._unpack_subs(_v.subcommands)
-
-    def unpack(self) -> None:
-        """处理 `Arparma` 中的数据"""
-        self._unpack_opts(self.options)
-        self._unpack_subs(self.subcommands)
-
-    @staticmethod
-    def behave_cancel():
-        """取消行为器的后续操作"""
-        raise BehaveCancelled
-
-    @staticmethod
-    def behave_fail():
-        """取消行为器的后续操作并抛出 `OutBoundsBehave`"""
-        raise OutBoundsBehave
-
-    def execute(self, behaviors: list[ArparmaBehavior] | None = None) -> Self:
-        """执行行为器
-
-        Args:
-            behaviors (list[ArparmaBehavior] | None, optional): 要执行的行为器列表
-        Returns:
-            Self: 返回自身
-        """
-        if not behaviors:
-            return self
-        for b in behaviors:
-            b.before_operate(self)
-        for b in behaviors:
-            try:
-                b.operate(self)
-            except BehaveCancelled:
-                continue
-            except OutBoundsBehave as e:
-                return self.fail(e)
-        return self
-
-    def call(self, target: Callable[..., T]) -> T:
-        """依据 `Arparma` 中的数据调用函数
-
-        Args:
-            target (Callable[..., T]): 要调用的函数
-        Returns:
-            T: 函数返回值
-        Raises:
-            RuntimeError: 如果 Arparma 未匹配, 则抛出 RuntimeError
-        """
-        if not self.matched:
-            raise RuntimeError("No matched")
-        pos_args = []
-        kw_args = {}
-        data = {
-            **{k: v() for k, v in self._additional.items()},
-            **self.all_matched_args,
-            "context": self.context,
-            "all_args": self.all_matched_args,
-            "options": self.options,
-            "subcommands": self.subcommands,
-        }
-
-        sig = inspect.signature(target)
-        for p in sig.parameters.values():
-            if p.name not in data:
-                continue
-            if p.kind in (p.POSITIONAL_ONLY, p.POSITIONAL_OR_KEYWORD):
-                pos_args.append(data[p.name])
-            elif p.kind == p.VAR_POSITIONAL:
-                pos_args.extend(data[p.name])
-            elif p.kind == p.VAR_KEYWORD:
-                kw_args = {**kw_args, **data[p.name]}
-            else:
-                kw_args[p.name] = data[p.name]
-        bind = sig.bind(*pos_args, **kw_args)
-        bind.apply_defaults()
-        try:
-            return target(*bind.args, **bind.kwargs)
-        finally:
-            data.clear()
-
-    def fail(self, exc: type[Exception] | Exception) -> Self:
-        """生成一个失败的 `Arparma`"""
-        return Arparma(self.source, self.origin, False, self.header_match, error_info=exc)  # type: ignore
-
-    def __require__(self, parts: list[str]) -> tuple[dict[str, Any] | OptionResult | SubcommandResult | None, str]:
-        """如果能够返回, 除开基本信息, 一定返回该path所在的dict"""
-        if len(parts) == 1:
-            part = parts[0]
-            if part in {"options", "subcommands", "main_args", "other_args", "context"}:
-                return getattr(self, part, {}), ""
-            for src in (self.main_args, self.other_args, self.options, self.subcommands, self.context):
-                if part in src:
-                    return src, part
-            return (self.all_matched_args, "") if part == "args" else (None, part)
-        prefix = parts.pop(0)  # parts[0]
-        if prefix in {"options", "subcommands"} and prefix in self.components:
-            raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=prefix))
-        if prefix == "options" or prefix in self.options:
-            return _handle_opt(prefix, parts, self.options)
-        if prefix == "subcommands" or prefix in self.subcommands:
-            return _handle_sub(prefix, parts, self.subcommands)
-        prefix = prefix.replace("$main", "main_args").replace("$other", "other_args")
-        if prefix in {"main_args", "other_args"}:
-            return getattr(self, prefix, {}), parts.pop(0)
-        path = ".".join([prefix] + parts)
-        if path in self.context:
-            return self.context, path
-        try:
-            return safe_eval(path, self.context), ""  # type: ignore
-        except Exception:
-            return None, prefix
-
-    def query_with(self, arg_type: type[T], *args):
-        return self.query[arg_type](*args)
-
-    def find(self, path: str) -> bool:
-        """查询路径是否存在
-
-        Args:
-            path (str): 要查询的路径
-
-        Returns:
-            bool: 是否存在
-        """
-        return self.query(path, Empty) != Empty
-
-    exist = find
-
-    @classmethod
-    def addition(cls, **supplier: Callable[[], Any]):
-        cls._additional.update(supplier)
-
-    @overload
-    def __getitem__(self, item: str) -> Any:
-        ...
-
-    @overload
-    def __getitem__(self, item: type[T]) -> T | None:
-        ...
-
-    @overload
-    def __getitem__(self, item: tuple[type[T], int]) -> T | None:
-        ...
-
-    def __getitem__(self, item: str | type[T] | tuple[type[T], int]) -> T | Any | None:
-        """查询 `Arparma` 中的数据
-
-        Args:
-            item (str | type[T]): 要查询的路径或类型
-        """
-
-        if isinstance(item, str):
-            return self.query(item)
-        if isinstance(item, tuple):
-            return [i for i in self.all_matched_args.values() if generic_isinstance(i, item[0])][item[1]]
-        return next(i for i in self.all_matched_args.values() if generic_isinstance(i, item))
-
-    def __getattr__(self, item: str):
-        return self.all_matched_args.get(item, self.query(item.replace("_", ".")))
-
-    def __repr__(self):
-        if not self.matched:
-            attrs = ((s, getattr(self, s, None)) for s in ("matched", "header_match", "error_data", "error_info"))
-            return ", ".join([f"{a}={v}" for a, v in attrs])
-        else:
-            attrs = {
-                "matched": self.matched,
-                "header_match": self.header_match,
-                "options": self.options,
-                "subcommands": self.subcommands,
-                "main_args": self.main_args,
-                "other_args": self.other_args,
-            }
-            return ", ".join([f"{a}={v}" for a, v in attrs.items() if v])
-
-
-@dataclass(init=True, unsafe_hash=True, repr=True)
-class ArparmaBehavior(metaclass=ABCMeta):
-    """解析结果行为器的基类, 对应一个对解析结果的操作行为
-
-    Attributes:
-        requires (list[ArparmaBehavior]): 该行为器所依赖的行为器
-    """
-
-    record: dict[int, dict[str, tuple[Any, Any]]] = field(default_factory=dict, init=False, repr=False, hash=False)
-    requires: list[ArparmaBehavior] = field(init=False, hash=False, repr=False)
-
-    def before_operate(self, interface: Arparma):
-        """在操作前调用, 用于准备数据"""
-        if not self.record:
-            return
-        if not (_record := self.record.get(interface.token)):
-            return
-        for path, (past, current) in _record.items():
-            source, end = interface.__require__(path.split("."))
-            if source is None:
-                continue
-            if isinstance(source, dict):
-                if past != Empty:
-                    source[end] = past
-                elif source.get(end, Empty) != current:
-                    source.pop(end)
-            elif past != Empty:
-                setattr(source, end, past)
-            elif getattr(source, end, Empty) != current:
-                delattr(source, end)
-        _record.clear()
-
-    @abstractmethod
-    def operate(self, interface: Arparma):
-        """对解析结果进行操作"""
-        ...
-
-    def update(self, interface: Arparma, path: str, value: Any):
-        """更新解析结果
-
-        Args:
-            interface (Arparma): Arparma 实例
-            path (str): 要更新的路径
-            value (Any): 要更新的值
-        """
-
-        def _update(tkn, src, pth, ep, val):
-            _record = self.record.setdefault(tkn, {})
-            if isinstance(src, dict):
-                _record[pth] = (src.get(ep, Empty), val)
-                src[ep] = val
-            else:
-                _record[pth] = (getattr(src, ep, Empty), val)
-                setattr(src, ep, val)
-
-        source, end = interface.__require__(path.split("."))
-        if source is None:
-            return
-        if end:
-            _update(interface.token, source, path, end, value)
-        elif isinstance(value, dict):
-            for k, v in value.items():
-                _update(interface.token, source, f"{path}.{k}", k, v)
-
-
-@lru_cache(4096)
-def requirement_handler(behavior: ArparmaBehavior) -> list[ArparmaBehavior]:
-    res = []
-    for b in getattr(behavior, "requires", []):
-        res.extend(requirement_handler(b))
-    res.append(behavior)
-    return res
+from __future__ import annotations
+
+from abc import ABCMeta, abstractmethod
+from dataclasses import dataclass, field
+from functools import lru_cache
+from types import MappingProxyType
+from typing import Any, Callable, ClassVar, Generic, TypeVar, cast, overload
+
+from tarina import Empty, generic_isinstance, get_signature, lang
+from typing_extensions import Self
+
+from .exceptions import BehaveCancelled, OutBoundsBehave
+from .model import HeadResult, OptionResult, SubcommandResult
+from .typing import TDC
+
+T = TypeVar('T')
+T1 = TypeVar('T1')
+D = TypeVar('D')
+
+
+def _handle_opt(_pf: str, _parts: list[str], _opts: dict[str, OptionResult]):
+    """处理 `options.xxx.yyy.zzz` 形式的参数"""
+    if _pf == "options":
+        _pf = _parts.pop(0)
+    if not _parts:  # options.foo or foo
+        return _opts, _pf
+    elif not (__src := _opts.get(_pf)):  # options.foo.bar or foo.bar
+        return _opts, _pf
+    if (_end := _parts.pop(0)) == "value":
+        return __src, _end
+    if _end == 'args':
+        return (__src.args, _parts.pop(0)) if _parts else (__src, _end)
+    return __src.args, _end
+
+
+def _handle_sub(_pf: str, _parts: list[str], _subs: dict[str, SubcommandResult]):
+    """处理 `subcommands.xxx.yyy.zzz` 形式的参数"""
+    if _pf == "subcommands":
+        _pf = _parts.pop(0)
+    if not _parts:
+        return _subs, _pf
+    elif not (__src := _subs.get(_pf)):
+        return _subs, _pf
+    if (_end := _parts.pop(0)) == "value":
+        return __src, _end
+    if _end == 'args':
+        return (__src.args, _parts.pop(0)) if _parts else (__src, _end)
+    if _end == "options" and (_end in __src.options or not _parts):
+        raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=f"{_pf}.{_end}"))
+    if _end == "options" or _end in __src.options:
+        return _handle_opt(_end, _parts, __src.options)
+    if _end == "subcommands" and (_end in __src.subcommands or not _parts):
+        raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=f"{_pf}.{_end}"))
+    if _end == "subcommands" or _end in __src.subcommands:
+        return _handle_sub(_end, _parts, __src.subcommands)
+    return __src.args, _end
+
+
+class _Query(Generic[T]):
+    source: Arparma
+    def __get__(self, instance: Arparma, owner: type) -> _Query[T]:
+        self.source = instance
+        return self
+
+    def __set_name__(self, owner, name):
+        self.name = name
+
+    def __getitem__(self, item: type[T1]) -> _Query[T1]:
+        return cast("_Query[T1]", self)
+
+    @overload
+    def __call__(self, path: str) -> T | None:
+        ...
+
+    @overload
+    def __call__(self, path: str, default: D) -> T | D:
+        ...
+
+    def __call__(self, path: str, default: D | None = None) ->  T | D | None:
+        """查询 `Arparma` 中的数据
+
+        Args:
+            path (str): 要查询的路径
+            default (T | None, optional): 如果查询失败, 则返回该值
+        """
+        source, endpoint = self.source.__require__(path.split('.'))
+        if source is None:
+            return default
+        if isinstance(source, (OptionResult, SubcommandResult)):
+            return getattr(source, endpoint, default) if endpoint else source  # type: ignore
+        return source.get(endpoint, default) if endpoint else MappingProxyType(source)  # type: ignore
+
+class Arparma(Generic[TDC]):
+    """承载解析结果与操作数据的接口类
+
+    Attributes:
+        origin (TDC): 原始数据
+        matched (bool): 是否匹配
+        header_match (HeadResult): 命令头匹配结果
+        error_info (type[BaseException] | BaseException | str): 错误信息
+        error_data (list[str | Any]): 错误数据
+        main_args (dict[str, Any]): 主参数匹配结果
+        options (dict[str, OptionResult]): 选项匹配结果
+        subcommands (dict[str, SubcommandResult]): 子命令匹配结果
+    """
+    header_match: HeadResult
+    options: dict[str, OptionResult]
+    subcommands: dict[str, SubcommandResult]
+
+    def __init__(
+        self,
+        source: str,
+        origin: TDC,
+        matched: bool = False,
+        header_match: HeadResult | None = None,
+        error_info: type[BaseException] | BaseException | None = None,
+        error_data: list[str | Any] | None = None,
+        main_args: dict[str, Any] | None = None,
+        options: dict[str, OptionResult] | None = None,
+        subcommands: dict[str, SubcommandResult] | None = None,
+    ):
+        """初始化 `Arparma`
+        Args:
+            source (str): 命令源
+            origin (TDC): 原始数据
+            matched (bool, optional): 是否匹配
+            header_match (HeadResult | None, optional): 命令头匹配结果
+            error_info (type[BaseException] | BaseException | None, optional): 错误信息
+            error_data (list[str | Any] | None, optional): 错误数据
+            main_args (dict[str, Any] | None, optional): 主参数匹配结果
+            options (dict[str, OptionResult] | None, optional): 选项匹配结果
+            subcommands (dict[str, SubcommandResult] | None, optional): 子命令匹配结果
+        """
+        self.source = source
+        self.origin = origin
+        self.matched = matched
+        self.header_match = header_match or HeadResult()
+        self.error_info = error_info
+        self.error_data = error_data or []
+        self.main_args = main_args or {}
+        self.options = options or {}
+        self.subcommands = subcommands or {}
+
+    _additional: ClassVar[dict[str, Callable[[], Any]]] = {}
+    query = _Query[Any]()
+
+    def _clr(self):
+        ks = list(self.__dict__.keys())
+        for k in ks:
+            delattr(self, k)
+
+    @property
+    def header(self) -> dict[str, Any]:
+        """返回可能解析到的命令头中的组信息"""
+        return self.header_match.groups
+
+    @property
+    def head_matched(self):
+        """返回命令头是否匹配"""
+        return self.header_match.matched
+
+    @property
+    def header_result(self):
+        """返回命令头匹配结果"""
+        return self.header_match.result
+
+    @property
+    def non_component(self) -> bool:
+        """返回是否没有解析到任何组件"""
+        return not self.subcommands and not self.options
+
+    @property
+    def components(self) -> dict[str, OptionResult | SubcommandResult]:
+        """返回解析到的组件"""
+        return {**self.options, **self.subcommands}
+
+    @property
+    def all_matched_args(self) -> dict[str, Any]:
+        """返回 Alconna 中所有 Args 解析到的值"""
+        other_args = {}
+        def _unpack_opts(_data):
+            for _v in _data.values():
+                other_args.update(_v.args)
+
+        def _unpack_subs(_data):
+            for _v in _data.values():
+                other_args.update(_v.args)
+                if _v.options:
+                    _unpack_opts(_v.options)
+                if _v.subcommands:
+                    _unpack_subs(_v.subcommands)
+
+        _unpack_opts(self.options)
+        _unpack_subs(self.subcommands)
+        return {**self.main_args, **other_args}
+
+    @property
+    def token(self) -> int:
+        """返回命令的 Token"""
+        from .manager import command_manager
+        return command_manager.get_token(self)
+
+    @staticmethod
+    def behave_cancel():
+        """取消行为器的后续操作"""
+        raise BehaveCancelled
+
+    @staticmethod
+    def behave_fail():
+        """取消行为器的后续操作并抛出 `OutBoundsBehave`"""
+        raise OutBoundsBehave
+
+    def execute(self, behaviors: list[ArparmaBehavior] | None = None) -> Self:
+        """执行行为器
+
+        Args:
+            behaviors (list[ArparmaBehavior] | None, optional): 要执行的行为器列表
+        Returns:
+            Self: 返回自身
+        """
+        if not behaviors:
+            return self
+        for b in behaviors:
+            b.before_operate(self)
+        for b in behaviors:
+            try:
+                b.operate(self)
+            except BehaveCancelled:
+                continue
+            except OutBoundsBehave as e:
+                return self.fail(e)
+        return self
+
+    def call(self, target: Callable[..., T]) -> T:
+        """依据 `Arparma` 中的数据调用函数
+
+        Args:
+            target (Callable[..., T]): 要调用的函数
+        Returns:
+            T: 函数返回值
+        Raises:
+            RuntimeError: 如果 Arparma 未匹配, 则抛出 RuntimeError
+        """
+        if not self.matched:
+            raise RuntimeError("No matched")
+        pos_args = []
+        kw_args = {}
+        data = {
+            **{k: v() for k, v in self._additional.items()},
+            **self.all_matched_args,
+            "all_args": self.all_matched_args,
+            "options": self.options,
+            "subcommands": self.subcommands
+        }
+
+        for p in get_signature(target):
+            if p.kind in (p.POSITIONAL_ONLY, p.POSITIONAL_OR_KEYWORD):
+                pos_args.append(data[p.name])
+            elif p.kind == p.VAR_POSITIONAL:
+                pos_args.extend(data[p.name])
+            elif p.kind == p.VAR_KEYWORD:
+                kw_args = {**kw_args, **data[p.name]}
+            else:
+                kw_args[p.name] = data[p.name]
+        return target(*pos_args, **kw_args)
+
+    def fail(self, exc: type[BaseException] | BaseException):
+        """生成一个失败的 `Arparma`"""
+        return Arparma(self.source, self.origin, False, self.header_match, error_info=exc)
+
+    def __require__(self, parts: list[str]) -> tuple[dict[str, Any] | OptionResult | SubcommandResult | None, str]:
+        """如果能够返回, 除开基本信息, 一定返回该path所在的dict"""
+        if len(parts) == 1:
+            part = parts[0]
+            for src in (self.main_args, self.other_args, self.options, self.subcommands):
+                if part in src:
+                    return src, part
+            if part in {"options", "subcommands", "main_args", "other_args"}:
+                return getattr(self, part, {}), ''
+            return (self.all_matched_args, '') if part == "args" else (None, part)
+        prefix = parts.pop(0)  # parts[0]
+        if prefix in {"options", "subcommands"} and prefix in self.components:
+            raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=prefix))
+        if prefix == "options" or prefix in self.options:
+            return _handle_opt(prefix, parts, self.options)
+        if prefix == "subcommands" or prefix in self.subcommands:
+            return _handle_sub(prefix, parts, self.subcommands)
+        prefix = prefix.replace("$main", "main_args").replace("$other", "other_args")
+        if prefix in {"main_args", "other_args"}:
+            return getattr(self, prefix, {}), parts.pop(0)
+        return None, prefix
+
+    def query_with(self, arg_type: type[T], *args): return self.query[arg_type](*args)
+
+    def find(self, path: str) -> bool:
+        """查询路径是否存在
+
+        Args:
+            path (str): 要查询的路径
+
+        Returns:
+            bool: 是否存在
+        """
+        return self.query(path, Empty) != Empty
+
+    exist = find
+
+    @classmethod
+    def addition(cls, **supplier: Callable[[], Any]):
+        cls._additional.update(supplier)
+
+    @overload
+    def __getitem__(self, item: str) -> Any:
+        ...
+
+    @overload
+    def __getitem__(self, item: type[T]) -> T | None:
+        ...
+
+    @overload
+    def __getitem__(self, item: tuple[type[T], int]) -> T | None:
+        ...
+
+    def __getitem__(self, item: str | type[T] | tuple[type[T], int]) -> T | Any | None:
+        """查询 `Arparma` 中的数据
+
+        Args:
+            item (str | type[T]): 要查询的路径或类型
+        """
+
+        if isinstance(item, str):
+            return self.query(item)
+        if isinstance(item, tuple):
+            return [i for i in self.all_matched_args.values() if generic_isinstance(i, item[0])][item[1]]
+        return next(i for i in self.all_matched_args.values() if generic_isinstance(i, item))
+
+    def __getattr__(self, item: str):
+        return self.all_matched_args.get(item, self.query(item.replace('_', '.')))
+
+    def __repr__(self):
+        if not self.matched:
+            attrs = ((s, getattr(self, s, None)) for s in ("matched", "header_match", "error_data", "error_info"))
+            return ", ".join([f"{a}={v}" for a, v in attrs])
+        else:
+            attrs = {
+                "matched": self.matched, "header_match": self.header_match,
+                "options": self.options, "subcommands": self.subcommands,
+                "main_args": self.main_args, "other_args": self.other_args
+            }
+            return ", ".join([f"{a}={v}" for a, v in attrs.items() if v])
+
+
+@dataclass(init=True, unsafe_hash=True, repr=True)
+class ArparmaBehavior(metaclass=ABCMeta):
+    """解析结果行为器的基类, 对应一个对解析结果的操作行为
+
+    Attributes:
+        requires (list[ArparmaBehavior]): 该行为器所依赖的行为器
+    """
+    record: dict[int, dict[str, tuple[Any, Any]]] = field(default_factory=dict, init=False, repr=False, hash=False)
+    requires: list[ArparmaBehavior] = field(init=False, hash=False, repr=False)
+
+    def before_operate(self, interface: Arparma):
+        """在操作前调用, 用于准备数据"""
+        if not self.record:
+            return
+        if not (_record := self.record.get(interface.token)):
+            return
+        for path, (past, current) in _record.items():
+            source, end = interface.__require__(path.split("."))
+            if source is None:
+                continue
+            if isinstance(source, dict):
+                if past != Empty:
+                    source[end] = past
+                elif source.get(end, Empty) != current:
+                    source.pop(end)
+            elif past != Empty:
+                setattr(source, end, past)
+            elif getattr(source, end, Empty) != current:
+                delattr(source, end)
+        _record.clear()
+
+    @abstractmethod
+    def operate(self, interface: Arparma):
+        """对解析结果进行操作"""
+        ...
+
+    def update(self, interface: Arparma, path: str, value: Any):
+        """更新解析结果
+
+        Args:
+            interface (Arparma): Arparma 实例
+            path (str): 要更新的路径
+            value (Any): 要更新的值
+        """
+        def _update(tkn, src, pth, ep, val):
+            _record = self.record.setdefault(tkn, {})
+            if isinstance(src, dict):
+                _record[pth] = (src.get(ep, Empty), val)
+                src[ep] = val
+            else:
+                _record[pth] = (getattr(src, ep, Empty), val)
+                setattr(src, ep, val)
+
+        source, end = interface.__require__(path.split("."))
+        if source is None:
+            return
+        if end:
+            _update(interface.token, source, path, end, value)
+        elif isinstance(value, dict):
+            for k, v in value.items():
+                _update(interface.token, source, f"{path}.{k}", k, v)
+
+
+@lru_cache(4096)
+def requirement_handler(behavior: ArparmaBehavior) -> list[ArparmaBehavior]:
+    res = []
+    for b in getattr(behavior, 'requires', []):
+        res.extend(requirement_handler(b))
+    res.append(behavior)
+    return res
```

### Comparing `arclet_alconna-1.8.8/src/arclet/alconna/base.py` & `arclet_alconna-2.0.0a1/src/arclet/alconna/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,368 +1,331 @@
-"""Alconna 的基础内容相关"""
-from __future__ import annotations
-
-from dataclasses import replace
-from functools import reduce
-from typing import Any, Iterable, Sequence, overload
-from typing_extensions import Self
-
-from tarina import Empty, lang
-
-from .action import Action, store
-from .args import Arg, Args
-from .exceptions import InvalidArgs
-from .model import OptionResult, SubcommandResult
-
-
-def _handle_default(node: CommandNode):
-    if node.default is Empty:
-        return
-    act = node.action
-    if act.type == 1 and not isinstance(act.value, list):
-        act = node.action = replace(act, value=[act.value])
-    elif act.type == 2 and not isinstance(act.value, int):
-        act = node.action = replace(act, value=1)
-    if isinstance(node.default, (OptionResult, SubcommandResult)):
-        if act.type == 0 and act.value is ...:
-            node.action = Action(act.type, node.default.value)
-        if act.type == 1:
-            if not isinstance(node.default.value, list):
-                node.default.value = [node.default.value]
-            if act.value[0] is ...:  # type: ignore
-                node.action = Action(act.type, node.default.value[:])
-        if act.type == 2 and not isinstance(node.default.value, int):
-            node.default.value = 1
-    else:
-        if act.type == 0 and act.value is ...:
-            node.action = Action(act.type, node.default)
-        if act.type == 1:
-            if not isinstance(node.default, list):
-                node.default = [node.default]
-            if act.value[0] is ...:  # type: ignore
-                node.action = Action(act.type, node.default[:])
-        if act.type == 2 and not isinstance(node.default, int):
-            node.default = 1
-
-
-class CommandNode:
-    """命令节点基类, 规定基础组件所含属性"""
-
-    name: str
-    """命令节点名称"""
-    aliases: frozenset[str]
-    """命令节点别名"""
-    dest: str
-    """命令节点目标名称"""
-    default: Any
-    """命令节点默认值"""
-    args: Args
-    """命令节点参数"""
-    separators: tuple[str, ...]
-    """命令节点分隔符"""
-    action: Action
-    """命令节点响应动作"""
-    help_text: str
-    """命令节点帮助信息"""
-    requires: list[str]
-    """命令节点需求前缀"""
-
-    def __init__(
-        self,
-        name: str,
-        args: Arg | Args | None = None,
-        alias: Iterable[str] | None = None,
-        dest: str | None = None,
-        default: Any = Empty,
-        action: Action | None = None,
-        separators: str | Sequence[str] | set[str] | None = None,
-        help_text: str | None = None,
-        requires: str | list[str] | tuple[str, ...] | set[str] | None = None,
-    ):
-        """
-        初始化命令节点
-
-        Args:
-            name (str): 命令节点名称
-            args (Arg | Args | None, optional): 命令节点参数
-            dest (str | None, optional): 命令节点目标名称
-            default (Any, optional): 命令节点默认值
-            action (Action | None, optional): 命令节点响应动作
-            separators (str | Sequence[str] | Set[str] | None, optional): 命令分隔符
-            help_text (str | None, optional): 命令帮助信息
-            requires (str | list[str] | tuple[str, ...] | set[str] | None, optional): 命令节点需求前缀
-        """
-        aliases = list(alias or [])
-        parts = name.split(" ")
-        _name = parts[-1]
-        if "|" in _name:
-            _aliases = _name.split("|")
-            _aliases.sort(key=len, reverse=True)
-            _name = _aliases[0]
-            aliases.extend(_aliases[1:])
-        if not _name:
-            raise InvalidArgs(lang.require("common", "name_empty"))
-        aliases.insert(0, _name)
-        self.name = _name
-        self.aliases = frozenset(aliases)
-        self.requires = ([requires] if isinstance(requires, str) else list(requires)) if requires else []
-        self.requires.extend(parts[:-1])
-        self.args = Args() + args
-        self.default = default
-        self.action = action or store
-        _handle_default(self)
-        self.separators = (" ",) if separators is None else ((separators,) if isinstance(separators, str) else tuple(separators))  # noqa: E501
-        self.nargs = len(self.args.argument)
-        self.dest = (dest or (("_".join(self.requires) + "_") if self.requires else "") + self.name.lstrip("-")).lstrip("-")  # noqa: E501
-        self.help_text = help_text or self.dest
-        self._hash = self._calc_hash()
-
-    nargs: int
-    _hash: int
-
-    def separate(self, *separator: str) -> Self:
-        """设置命令分隔符
-
-        Args:
-            *separator(str): 命令分隔符
-
-        Returns:
-            Self: 命令节点本身
-        """
-        self.separators = separator
-        self._hash = self._calc_hash()
-        return self
-
-    def __repr__(self):
-        data = {}
-        if not self.args.empty:
-            data["args"] = self.args
-        if self.default is not Empty:
-            data["default"] = self.default
-        return f"{self.__class__.__name__}({self.dest!r}, {', '.join(f'{k}={v!r}' for k, v in data.items())})"
-
-    def _calc_hash(self):
-        data = vars(self)
-        data.pop("_hash", None)
-        return hash(repr(data))
-
-    def __hash__(self):
-        return self._hash
-
-    def __eq__(self, other):
-        return self.__class__ == other.__class__ and self.__hash__() == other.__hash__()
-
-
-class Option(CommandNode):
-    """命令选项
-
-    相比命令节点, 命令选项可以设置别名, 优先级, 允许名称与后随参数之间无分隔符
-    """
-
-    default: OptionResult
-    """命令选项默认值"""
-    aliases: frozenset[str]
-    """命令选项别名"""
-    compact: bool
-    "是否允许名称与后随参数之间无分隔符"
-
-    def __init__(
-        self,
-        name: str,
-        args: Arg | Args | None = None,
-        alias: Iterable[str] | None = None,
-        dest: str | None = None,
-        default: Any = Empty,
-        action: Action | None = None,
-        separators: str | Sequence[str] | set[str] | None = None,
-        help_text: str | None = None,
-        requires: str | list[str] | tuple[str, ...] | set[str] | None = None,
-        compact: bool = False,
-        priority: int = 0,
-    ):
-        """初始化命令选项
-
-        Args:
-            name (str): 命令选项名称
-            args (Arg | Args | None, optional): 命令选项参数
-            alias (Iterable[str] | None, optional): 命令选项别名
-            dest (str | None, optional): 命令选项目标名称
-            default (Any, optional): 命令选项默认值
-            action (Action | None, optional): 命令选项响应动作
-            separators (str | Sequence[str] | Set[str] | None, optional): 命令分隔符
-            help_text (str | None, optional): 命令选项帮助信息
-            requires (str | list[str] | tuple[str, ...] | set[str] | None, optional): 命令选项需求前缀
-            compact (bool, optional): 是否允许名称与后随参数之间无分隔符
-            priority (int, optional): 命令选项优先级
-        """
-
-        self.priority = priority
-        self.compact = compact
-        if default is not Empty:
-            default = default if isinstance(default, OptionResult) else OptionResult(default)
-        super().__init__(name, args, alias, dest, default, action, separators, help_text, requires)
-        if self.separators == ("",):
-            self.compact = True
-            self.separators = (" ",)
-
-    @overload
-    def __add__(self, other: Option) -> Subcommand:
-        ...
-
-    @overload
-    def __add__(self, other: Args | Arg) -> Option:
-        ...
-
-    def __add__(self, other: Option | Args | Arg) -> Subcommand | Option:
-        """连接命令选项与命令节点或命令选项, 生成子命令
-
-        Args:
-            other (Option | Args | Arg): 命令节点或命令选项
-
-        Returns:
-            Option | Subcommand: 如果other为命令选项, 则返回生成的子命令, 否则返回自己
-
-        Raises:
-            TypeError: 如果other不是命令选项或命令节点, 则抛出此异常
-        """
-        if isinstance(other, Option):
-            return Subcommand(self.name, other, self.args, dest=self.dest, separators=self.separators, help_text=self.help_text, requires=self.requires)  # noqa: E501
-        if isinstance(other, (Arg, Args)):
-            self.args += other
-            self.nargs = len(self.args)
-            self._hash = self._calc_hash()
-            return self
-        raise TypeError(f"unsupported operand type(s) for +: 'Option' and '{other.__class__.__name__}'")
-
-    def __radd__(self, other: str):
-        """与字符串连接, 生成 `Alconna` 对象
-
-        Args:
-            other (str): 字符串
-
-        Returns:
-            Alconna: Alconna 对象
-
-        Raises:
-            TypeError: 如果other不是字符串, 则抛出此异常
-        """
-        if isinstance(other, str):
-            from .core import Alconna
-
-            return Alconna(other, self)
-        raise TypeError(f"unsupported operand type(s) for +: '{other.__class__.__name__}' and 'Option'")
-
-
-class Subcommand(CommandNode):
-    """子命令, 次于主命令
-
-    与命令节点不同, 子命令可以包含多个命令选项与相对于自己的子命令
-    """
-
-    default: SubcommandResult
-    """子命令默认值"""
-    options: list[Option | Subcommand]
-    """子命令包含的选项与子命令"""
-
-    def __init__(
-        self,
-        name: str,
-        *args: Args | Arg | Option | Subcommand | list[Option | Subcommand],
-        alias: Iterable[str] | None = None,
-        dest: str | None = None,
-        default: Any = Empty,
-        separators: str | Sequence[str] | set[str] | None = None,
-        help_text: str | None = None,
-        requires: str | list[str] | tuple[str, ...] | set[str] | None = None,
-    ):
-        """初始化子命令
-
-        Args:
-            name (str): 子命令名称
-            *args (Args | Arg | Option | Subcommand | list[Option | Subcommand]): 参数, 选项或子命令
-            dest (str | None, optional): 子命令选项目标名称
-            default (Any, optional): 子命令默认值
-            action (Action | None, optional): 子命令选项响应动作
-            separators (str | Sequence[str] | Set[str] | None, optional): 子命令分隔符
-            help_text (str | None, optional): 子命令选项帮助信息
-            requires (str | list[str] | tuple[str, ...] | set[str] | None, optional): 子命令选项需求前缀
-        """
-        self.options = [i for i in args if isinstance(i, (Option, Subcommand))]
-        for li in args:
-            if isinstance(li, list):
-                self.options.extend(li)
-        if default is not Empty:
-            default = default if isinstance(default, SubcommandResult) else SubcommandResult(default)
-        super().__init__(
-            name,
-            reduce(lambda x, y: x + y, [Args()] + [i for i in args if isinstance(i, (Arg, Args))]),  # type: ignore
-            alias, dest, default, None, separators, help_text, requires,
-        )
-
-    def __add__(self, other: Option | Args | Arg | str) -> Self:
-        """连接子命令与命令选项或命令节点
-
-        Args:
-            other (Option | Args | Arg | str): 命令选项或命令节点
-
-        Returns:
-            Self: 返回子命令自身
-
-        Raises:
-            TypeError: 如果other不是命令选项或命令节点, 则抛出此异常
-        """
-        if isinstance(other, (Option, str)):
-            self.options.append(Option(other) if isinstance(other, str) else other)
-            self._hash = self._calc_hash()
-            return self
-        if isinstance(other, (Arg, Args)):
-            self.args += other
-            self.nargs = len(self.args)
-            self._hash = self._calc_hash()
-            return self
-        raise TypeError(f"unsupported operand type(s) for +: 'Subcommand' and '{other.__class__.__name__}'")
-
-    def __radd__(self, other: str):
-        """与字符串连接, 生成 `Alconna` 对象
-
-        Args:
-            other (str): 字符串
-
-        Returns:
-            Alconna: Alconna 对象
-
-        Raises:
-            TypeError: 如果other不是字符串, 则抛出此异常
-        """
-        if isinstance(other, str):
-            from .core import Alconna
-
-            return Alconna(other, self)
-        raise TypeError(f"unsupported operand type(s) for +: '{other.__class__.__name__}' and 'Subcommand'")
-
-    def add(self, opt: Option | Subcommand) -> Self:
-        """添加选项或子命令
-
-        Args:
-            opt (Option | Subcommand): 选项或子命令
-
-        Returns:
-            Self: 返回子命令自身
-        """
-        self.options.append(opt)
-        self._hash = self._calc_hash()
-        return self
-
-
-class Help(Option):
-    def _calc_hash(self):
-        return hash("$ALCONNA_BUILTIN_OPTION_HELP")
-
-
-class Shortcut(Option):
-    def _calc_hash(self):
-        return hash("$ALCONNA_BUILTIN_OPTION_SHORTCUT")
-
-
-class Completion(Option):
-    def _calc_hash(self):
-        return hash("$ALCONNA_BUILTIN_OPTION_COMPLETION")
+"""Alconna 的基础内容相关"""
+from __future__ import annotations
+
+from functools import reduce
+from dataclasses import replace
+from typing import Any, Iterable, Sequence, overload
+
+from tarina import lang, Empty
+from typing_extensions import Self
+
+from .action import Action, store
+from .args import Arg, Args
+from .exceptions import InvalidParam
+from .model import OptionResult, SubcommandResult
+
+
+def _handle_default(node: CommandNode):
+    if node.default is Empty:
+        return
+    act = node.action
+    if act.type == 1 and not isinstance(act.value, list):
+        act = node.action = replace(act, value=[act.value])
+    elif act.type == 2 and not isinstance(act.value, int):
+        act = node.action = replace(act, value=1)
+    if isinstance(node.default, (OptionResult, SubcommandResult)):
+        if act.type == 0 and act.value is ...:
+            node.action = Action(act.type, node.default.value)
+        if act.type == 1:
+            if not isinstance(node.default.value, list):
+                node.default.value = [node.default.value]
+            if act.value[0] is ...:  # type: ignore
+                node.action = Action(act.type, node.default.value[:])
+        if act.type == 2 and not isinstance(node.default.value, int):
+            node.default.value = 1
+    else:
+        if act.type == 0 and act.value is ...:
+            node.action = Action(act.type, node.default)
+        if act.type == 1:
+            if not isinstance(node.default, list):
+                node.default = [node.default]
+            if act.value[0] is ...:  # type: ignore
+                node.action = Action(act.type, node.default[:])
+        if act.type == 2 and not isinstance(node.default, int):
+            node.default = 1
+
+
+class CommandNode:
+    """命令节点基类, 规定基础组件所含属性"""
+
+    name: str
+    """命令节点名称"""
+    dest: str
+    """命令节点目标名称"""
+    default: Any
+    """命令节点默认值"""
+    args: Args
+    """命令节点参数"""
+    separators: tuple[str, ...]
+    """命令节点分隔符"""
+    action: Action
+    """命令节点响应动作"""
+    help_text: str
+    """命令节点帮助信息"""
+
+    def __init__(
+        self, name: str, args: Arg | Args | None = None,
+        dest: str | None = None, default: Any = Empty, action: Action | None = None,
+        separators: str | Sequence[str] | set[str] | None = None,
+        help_text: str | None = None,
+    ):
+        """
+        初始化命令节点
+
+        Args:
+            name (str): 命令节点名称
+            args (Arg | Args | None, optional): 命令节点参数
+            dest (str | None, optional): 命令节点目标名称
+            default (Any, optional): 命令节点默认值
+            action (Action | None, optional): 命令节点响应动作
+            separators (str | Sequence[str] | Set[str] | None, optional): 命令分隔符
+            help_text (str | None, optional): 命令帮助信息
+        """
+        if not name:
+            raise InvalidParam(lang.require("common", "name_empty"))
+        self.name = name.replace(" ", "_")
+        self.args = Args() + args
+        self.default = default
+        self.action = action or store
+        _handle_default(self)
+        self.separators = (' ',) if separators is None else (
+            (separators,) if isinstance(separators, str) else tuple(separators)
+        )
+        self.nargs = len(self.args.argument)
+        self.dest = (dest or self.name.lstrip('-')).lstrip('-')
+        self.help_text = help_text or self.dest
+        self._hash = self._calc_hash()
+
+    nargs: int
+    _hash: int
+
+    def separate(self, *separator: str) -> Self:
+        """设置命令分隔符
+
+        Args:
+            *separator(str): 命令分隔符
+
+        Returns:
+            Self: 命令节点本身
+        """
+        self.separators = separator
+        self._hash = self._calc_hash()
+        return self
+
+    def __repr__(self):
+        data = {}
+        if not self.args.empty:
+            data["args"] = self.args
+        if self.default is not Empty:
+            data["default"] = self.default
+        return f"{self.__class__.__name__}({self.dest!r}, {', '.join(f'{k}={v!r}' for k, v in data.items())})"
+
+    def _calc_hash(self):
+        data = vars(self)
+        data.pop("_hash", None)
+        return hash(repr(data))
+
+    def __hash__(self):
+        return self._hash
+
+    def __eq__(self, other):
+        return self.__class__ == other.__class__ and self.__hash__() == other.__hash__()
+
+
+class Option(CommandNode):
+    """命令选项
+
+    相比命令节点, 命令选项可以设置别名, 优先级, 允许名称与后随参数之间无分隔符
+    """
+
+    default: OptionResult | type[Empty]
+    """命令选项默认值"""
+    aliases: frozenset[str]
+    """命令选项别名"""
+    compact: bool
+    "是否允许名称与后随参数之间无分隔符"
+
+    def __init__(
+        self,
+        name: str, args: Arg | Args | None = None, alias: Iterable[str] | None = None,
+        dest: str | None = None, default: Any = Empty, action: Action | None = None,
+        separators: str | Sequence[str] | set[str] | None = None,
+        help_text: str | None = None,
+        compact: bool = False,
+    ):
+        """初始化命令选项
+
+        Args:
+            name (str): 命令选项名称
+            args (Arg | Args | None, optional): 命令选项参数
+            alias (Iterable[str] | None, optional): 命令选项别名
+            dest (str | None, optional): 命令选项目标名称
+            default (Any, optional): 命令选项默认值
+            action (Action | None, optional): 命令选项响应动作
+            separators (str | Sequence[str] | Set[str] | None, optional): 命令分隔符
+            help_text (str | None, optional): 命令选项帮助信息
+            compact (bool, optional): 是否允许名称与后随参数之间无分隔符
+        """
+        aliases = list(alias or [])
+        _name = name.split(" ")[-1]
+        if "|" in _name:
+            _aliases = _name.split("|")
+            _aliases.sort(key=len, reverse=True)
+            name = name.replace(_name, _aliases[0])
+            _name = _aliases[0]
+            aliases.extend(_aliases[1:])
+        aliases.insert(0, _name)
+        self.aliases = frozenset(aliases)
+        self.compact = compact
+        if default is not Empty:
+            default = default if isinstance(default, OptionResult) else OptionResult(default)
+        super().__init__(name, args, dest, default, action, separators, help_text)
+        if self.separators == ("",):
+            self.compact = True
+            self.separators = (" ",)
+
+    @overload
+    def __add__(self, other: Option) -> Subcommand:
+        ...
+
+    @overload
+    def __add__(self, other: Args | Arg) -> Option:
+        ...
+
+    def __add__(self, other: Option | Args | Arg) -> Self | Subcommand:
+        """连接命令选项与命令节点或命令选项, 生成子命令
+
+        Args:
+            other (Option | Args | Arg): 命令节点或命令选项
+
+        Returns:
+            Option | Subcommand: 如果other为命令选项, 则返回生成的子命令, 否则返回自己
+
+        Raises:
+            TypeError: 如果other不是命令选项或命令节点, 则抛出此异常
+        """
+        if isinstance(other, Option):
+            return Subcommand(
+                self.name, other, self.args, dest=self.dest,
+                separators=self.separators, help_text=self.help_text,
+            )
+        if isinstance(other, (Arg, Args)):
+            self.args += other
+            self.nargs = len(self.args)
+            self._hash = self._calc_hash()
+            return self
+        raise TypeError(f"unsupported operand type(s) for +: 'Option' and '{other.__class__.__name__}'")
+
+    def __radd__(self, other: str):
+        """与字符串连接, 生成 `Alconna` 对象
+
+        Args:
+            other (str): 字符串
+
+        Returns:
+            Alconna: Alconna 对象
+
+        Raises:
+            TypeError: 如果other不是字符串, 则抛出此异常
+        """
+        if isinstance(other, str):
+            from .core import Alconna
+            return Alconna(other, self)
+        raise TypeError(f"unsupported operand type(s) for +: '{other.__class__.__name__}' and 'Option'")
+
+
+class Subcommand(CommandNode):
+    """子命令, 次于主命令
+
+    与命令节点不同, 子命令可以包含多个命令选项与相对于自己的子命令
+    """
+    default: SubcommandResult | type[Empty]
+    """子命令默认值"""
+    options: list[Option | Subcommand]
+    """子命令包含的选项与子命令"""
+
+    def __init__(
+        self,
+        name: str,
+        *args: Args | Arg | Option | Subcommand | list[Option | Subcommand],
+        dest: str | None = None, default: Any = Empty,
+        separators: str | Sequence[str] | set[str] | None = None,
+        help_text: str | None = None,
+    ):
+        """初始化子命令
+
+        Args:
+            name (str): 子命令名称
+            *args (Args | Arg | Option | Subcommand | list[Option | Subcommand]): 参数, 选项或子命令
+            dest (str | None, optional): 子命令选项目标名称
+            default (Any, optional): 子命令默认值
+            action (Action | None, optional): 子命令选项响应动作
+            separators (str | Sequence[str] | Set[str] | None, optional): 子命令分隔符
+            help_text (str | None, optional): 子命令选项帮助信息
+        """
+        self.options = [i for i in args if isinstance(i, (Option, Subcommand))]
+        for li in args:
+            if isinstance(li, list):
+                self.options.extend(li)
+        if default is not Empty:
+            default = default if isinstance(default, SubcommandResult) else SubcommandResult(default)
+        super().__init__(
+            name,
+            reduce(lambda x, y: x + y, [Args()] + [i for i in args if isinstance(i, (Arg, Args))]),  # type: ignore
+            dest, default, None, separators, help_text
+        )
+
+    def __add__(self, other: Option | Args | Arg | str) -> Self:
+        """连接子命令与命令选项或命令节点
+
+        Args:
+            other (Option | Args | Arg | str): 命令选项或命令节点
+
+        Returns:
+            Self: 返回子命令自身
+
+        Raises:
+            TypeError: 如果other不是命令选项或命令节点, 则抛出此异常
+        """
+        if isinstance(other, (Option, str)):
+            self.options.append(Option(other) if isinstance(other, str) else other)
+            self._hash = self._calc_hash()
+            return self
+        if isinstance(other, (Arg, Args)):
+            self.args += other
+            self.nargs = len(self.args)
+            self._hash = self._calc_hash()
+            return self
+        raise TypeError(f"unsupported operand type(s) for +: 'Subcommand' and '{other.__class__.__name__}'")
+
+    def __radd__(self, other: str):
+        """与字符串连接, 生成 `Alconna` 对象
+
+        Args:
+            other (str): 字符串
+
+        Returns:
+            Alconna: Alconna 对象
+
+        Raises:
+            TypeError: 如果other不是字符串, 则抛出此异常
+        """
+        if isinstance(other, str):
+            from .core import Alconna
+            return Alconna(other, self)
+        raise TypeError(f"unsupported operand type(s) for +: '{other.__class__.__name__}' and 'Subcommand'")
+
+    def add(self, opt: Option | Subcommand) -> Self:
+        """添加选项或子命令
+
+        Args:
+            opt (Option | Subcommand): 选项或子命令
+
+        Returns:
+            Self: 返回子命令自身
+        """
+        self.options.append(opt)
+        self._hash = self._calc_hash()
+        return self
+
+
+__all__ = ["CommandNode", "Option", "Subcommand"]
```

### Comparing `arclet_alconna-1.8.8/src/arclet/alconna/config.py` & `arclet_alconna-2.0.0a1/src/arclet/alconna/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,131 @@
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, ContextManager, Literal, TypedDict
-
-from tarina import lang
-
-from .typing import DataCollection, TPrefixes
-
-if TYPE_CHECKING:
-    from .formatter import TextFormatter
-
-
-class OptionNames(TypedDict):
-    help: set[str]
-    """帮助选项的名称"""
-    shortcut: set[str]
-    """快捷选项的名称"""
-    completion: set[str]
-    """补全选项的名称"""
-
-
-@dataclass(init=True, repr=True)
-class Namespace:
-    """命名空间配置, 用于规定同一命名空间下的选项的默认配置"""
-
-    name: str
-    """命名空间名称"""
-    prefixes: TPrefixes = field(default_factory=list)
-    """默认前缀配置"""
-    separators: tuple[str, ...] = field(default_factory=lambda: (" ",))
-    """默认分隔符配置"""
-    formatter_type: type[TextFormatter] | None = field(default=None)  # type: ignore
-    """默认格式化器类型"""
-    fuzzy_match: bool = field(default=False)
-    """默认是否开启模糊匹配"""
-    raise_exception: bool = field(default=False)
-    """默认是否抛出异常"""
-    enable_message_cache: bool = field(default=True)
-    """默认是否启用消息缓存"""
-    disable_builtin_options: set[Literal["help", "shortcut", "completion"]] = field(default_factory=set)
-    builtin_option_name: OptionNames = field(
-        default_factory=lambda: {
-            "help": {"--help", "-h"},
-            "shortcut": {"--shortcut", "-sct"},
-            "completion": {"--comp", "-cp", "?"},
-        }
-    )
-    """默认的内置选项名称"""
-    to_text: Callable[[Any], str | None] = field(default=lambda x: x if isinstance(x, str) else None)
-    """默认的选项转文本函数"""
-    converter: Callable[[str | list], DataCollection[Any]] | None = field(default=lambda x: x)
-    """默认的文本转选项函数"""
-    compact: bool = field(default=False)
-    """默认是否开启紧凑模式"""
-    strict: bool = field(default=True)
-    "命令是否严格匹配，若为 False 则未知参数将作为名为 $extra 的参数"
-    context_style: Literal["bracket", "parentheses"] | None = field(default=None)
-    "命令上下文插值的风格，None 为关闭，bracket 为 {...}，parentheses 为 $(...)"
-
-    def __eq__(self, other):
-        return isinstance(other, Namespace) and other.name == self.name
-
-    def __hash__(self):
-        return hash(self.name)
-
-    @property
-    def headers(self):
-        """默认前缀配置"""
-        return self.prefixes
-
-    @headers.setter
-    def headers(self, value):
-        self.prefixes = value
-
-
-class namespace(ContextManager[Namespace]):
-    """新建一个命名空间配置并暂时作为默认命名空间
-
-    Example:
-        >>> with namespace("xxx") as ns:
-        ...     ns.headers = ["aaa"]
-        ...     alc = Alconna(...)
-        ... assert alc.prefixes == ["aaa"]
-    """
-
-    def __init__(self, name: Namespace | str):
-        """传入新建的命名空间的名称, 或者是一个存在的命名空间配置"""
-        self.np = Namespace(name) if isinstance(name, str) else name
-        self.name = self.np.name if isinstance(name, Namespace) else name
-        self.old = config.default_namespace
-        config.default_namespace = self.np
-
-    def __enter__(self) -> Namespace:
-        return self.np
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        if exc_type or exc_val or exc_tb:
-            return False
-        config.default_namespace = self.old
-        config.namespaces[self.name] = self.np
-        del self.old
-        del self.np
-
-
-class _AlconnaConfig:
-    """全局配置类"""
-
-    command_max_count: int = 200
-    """最大命令数量"""
-    _default_namespace = "Alconna"
-    """默认命名空间名称"""
-    remainders: set[str] = {"--"}
-    """参数分隔标记"""
-    namespaces: dict[str, Namespace] = {_default_namespace: Namespace(_default_namespace)}
-
-    @property
-    def default_namespace(self):
-        return self.namespaces[self._default_namespace]
-
-    @default_namespace.setter
-    def default_namespace(self, np: str | Namespace):
-        if isinstance(np, str):
-            if np not in self.namespaces:
-                old = self.namespaces.pop(self._default_namespace, Namespace(np))
-                old.name = np
-                self.namespaces[np] = old
-            self._default_namespace = np
-        else:
-            self._default_namespace = np.name
-            self.namespaces[np.name] = np
-
-
-config = _AlconnaConfig()
-lang.load(Path(__file__).parent / "i18n")
-
-__all__ = ["config", "Namespace", "namespace", "lang"]
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, Callable, ContextManager, TypedDict
+
+from tarina import lang
+
+from .typing import DataCollection, TPrefixes
+
+if TYPE_CHECKING:
+    from .formatter import TextFormatter
+
+
+class OptionNames(TypedDict):
+    help: set[str]
+    """帮助选项的名称"""
+    shortcut: set[str]
+    """快捷选项的名称"""
+    completion: set[str]
+    """补全选项的名称"""
+
+
+@dataclass(init=True, repr=True)
+class Namespace:
+    """命名空间配置, 用于规定同一命名空间下的选项的默认配置"""
+    name: str
+    """命名空间名称"""
+    prefixes: TPrefixes = field(default_factory=list)
+    """默认前缀配置"""
+    separators: tuple[str, ...] = field(default_factory=lambda: (" ",))
+    """默认分隔符配置"""
+    formatter_type: type[TextFormatter] | None = field(default=None)  # type: ignore
+    """默认格式化器类型"""
+    fuzzy_match: bool = field(default=False)
+    """默认是否开启模糊匹配"""
+    raise_exception: bool = field(default=False)
+    """默认是否抛出异常"""
+    enable_message_cache: bool = field(default=True)
+    """默认是否启用消息缓存"""
+    builtin_option_name: OptionNames = field(
+        default_factory=lambda: {
+            "help": {"--help", "-h"},
+            "shortcut": {"--shortcut", "-sct"},
+            "completion": {"--comp", "-cp", "?"},
+        }
+    )
+    """默认的内置选项名称"""
+    to_text: Callable[[Any], str | None] = field(default=lambda x: x if isinstance(x, str) else None)
+    """默认的选项转文本函数"""
+    converter: Callable[[str | list], DataCollection[Any]] | None = field(default=lambda x: x)
+    """默认的文本转选项函数"""
+    compact: bool = field(default=False)
+    """默认是否开启紧凑模式"""
+
+    def __eq__(self, other):
+        return isinstance(other, Namespace) and other.name == self.name
+
+    def __hash__(self):
+        return hash(self.name)
+
+    @property
+    def headers(self):
+        """默认前缀配置"""
+        return self.prefixes
+
+    @headers.setter
+    def headers(self, value):
+        self.prefixes = value
+
+
+class namespace(ContextManager[Namespace]):
+    """新建一个命名空间配置并暂时作为默认命名空间
+
+    Example:
+        >>> with namespace("xxx") as ns:
+        ...     ns.headers = ["aaa"]
+        ...     alc = Alconna(...)
+        ... assert alc.prefixes == ["aaa"]
+    """
+
+    def __init__(self, name: Namespace | str):
+        """传入新建的命名空间的名称, 或者是一个存在的命名空间配置"""
+        self.np = Namespace(name) if isinstance(name, str) else name
+        self.name = self.np.name if isinstance(name, Namespace) else name
+        self.old = config.default_namespace
+        config.default_namespace = self.np
+
+    def __enter__(self) -> Namespace:
+        return self.np
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if exc_type or exc_val or exc_tb:
+            return False
+        config.default_namespace = self.old
+        config.namespaces[self.name] = self.np
+        del self.old
+        del self.np
+
+
+class _AlconnaConfig:
+    """全局配置类"""
+    command_max_count: int = 200
+    """最大命令数量"""
+    fuzzy_threshold: float = 0.6
+    """模糊匹配阈值"""
+    _default_namespace = "Alconna"
+    """默认命名空间名称"""
+    namespaces: dict[str, Namespace] = {_default_namespace: Namespace(_default_namespace)}
+
+    @property
+    def default_namespace(self):
+        return self.namespaces[self._default_namespace]
+
+    @default_namespace.setter
+    def default_namespace(self, np: str | Namespace):
+        if isinstance(np, str):
+            if np not in self.namespaces:
+                old = self.namespaces.pop(self._default_namespace, Namespace(np))
+                old.name = np
+                self.namespaces[np] = old
+            self._default_namespace = np
+        else:
+            self._default_namespace = np.name
+            self.namespaces[np.name] = np
+
+
+config = _AlconnaConfig()
+lang.load(Path(__file__).parent / "i18n")
+
+__all__ = ["config", "Namespace", "namespace", "lang"]
```

### Comparing `arclet_alconna-1.8.8/src/arclet/alconna/core.py` & `arclet_alconna-2.0.0a1/src/arclet/alconna/core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,436 +1,380 @@
-"""Alconna 主体"""
-from __future__ import annotations
-
-import sys
-from dataclasses import dataclass, field
-from pathlib import Path
-from typing import Any, Callable, Generic, Literal, Sequence, TypeVar, cast, overload
-from typing_extensions import Self
-from weakref import WeakSet
-
-from tarina import init_spec, lang
-
-from ._internal._analyser import Analyser, TCompile
-from .args import Arg, Args
-from .arparma import Arparma, ArparmaBehavior, requirement_handler
-from .base import Completion, Help, Option, Shortcut, Subcommand
-from .config import Namespace, config
-from .exceptions import ExecuteFailed, NullMessage
-from .formatter import TextFormatter
-from .manager import ShortcutArgs, command_manager
-from .typing import TDC, CommandMeta, DataCollection, InnerShortcutArgs, ShortcutRegWrapper, TPrefixes
-
-T = TypeVar("T")
-TDC1 = TypeVar("TDC1", bound=DataCollection[Any])
-
-
-def handle_argv():
-    path = Path(sys.argv[0])
-    if str(path) == ".":
-        path = path.absolute()
-    head = path.stem
-    if head == "__main__":
-        head = path.parent.stem
-    return head
-
-
-def add_builtin_options(options: list[Option | Subcommand], ns: Namespace) -> None:
-    if "help" not in ns.disable_builtin_options:
-        options.append(Help("|".join(ns.builtin_option_name["help"]), help_text=lang.require("builtin", "option_help")))  # noqa: E501
-    if "shortcut" not in ns.disable_builtin_options:
-        options.append(
-            Shortcut(
-                "|".join(ns.builtin_option_name["shortcut"]),
-                Args["action?", "delete|list"]["name?", str]["command", str, "$"],
-                help_text=lang.require("builtin", "option_shortcut"),
-            )
-        )
-    if "completion" not in ns.disable_builtin_options:
-        options.append(Completion("|".join(ns.builtin_option_name["completion"]), help_text=lang.require("builtin", "option_completion")))  # noqa: E501
-
-
-@dataclass(init=True, unsafe_hash=True)
-class ArparmaExecutor(Generic[T]):
-    """Arparma 执行器
-
-    Attributes:
-        target(Callable[..., T]): 目标函数
-    """
-
-    target: Callable[..., T]
-    binding: Callable[..., list[Arparma]] = field(default=lambda: [], repr=False)
-
-    def __call__(self, *args, **kwargs):
-        return self.target(*args, **kwargs)
-
-    @property
-    def result(self) -> T:
-        """执行结果"""
-        if not self.binding:
-            raise ExecuteFailed(None)
-        arps = self.binding()
-        if not arps or not arps[0].matched:
-            raise ExecuteFailed("Unmatched")
-        try:
-            return arps[0].call(self.target)
-        except Exception as e:
-            raise ExecuteFailed(e) from e
-
-
-class Alconna(Subcommand, Generic[TDC]):
-    """
-    更加精确的命令解析
-
-    Examples:
-
-        >>> from arclet.alconna import Alconna
-        >>> alc = Alconna(
-        ...     "name",
-        ...     ["p1", "p2"],
-        ...     Option("opt", Args["opt_arg", "opt_arg"]),
-        ...     Subcommand(
-        ...         "sub_name",
-        ...         Option("sub_opt", Args["sub_arg", "sub_arg"]),
-        ...         Args["sub_main_args", "sub_main_args"]
-        ...     ),
-        ...     Args["main_args", "main_args"],
-        ...  )
-        >>> alc.parse("name opt opt_arg")
-    """
-
-    prefixes: TPrefixes
-    """命令前缀"""
-    command: str | Any
-    """命令名"""
-    formatter: TextFormatter
-    """文本格式化器"""
-    namespace: str
-    """命名空间"""
-    meta: CommandMeta
-    """命令元数据"""
-    behaviors: list[ArparmaBehavior]
-    """命令行为器"""
-
-    def compile(self, compiler: TCompile | None = None, param_ids: set[str] | None = None) -> Analyser[TDC]:
-        """编译 `Alconna` 为对应的解析器"""
-        return Analyser(self, compiler).compile(set() if param_ids is None else param_ids)
-
-    def __init__(
-        self,
-        *args: Option | Subcommand | str | TPrefixes | Any | Args | Arg,
-        meta: CommandMeta | None = None,
-        namespace: str | Namespace | None = None,
-        separators: str | set[str] | Sequence[str] | None = None,
-        behaviors: list[ArparmaBehavior] | None = None,
-        formatter_type: type[TextFormatter] | None = None,
-    ):
-        """
-        以标准形式构造 `Alconna`
-
-        Args:
-            *args (Option | Subcommand | str | TPrefixes | Any | Args | Arg): 命令选项、主参数、命令名称或命令头
-            action (ArgAction | Callable | None, optional): 命令解析后针对主参数的回调函数
-            meta (CommandMeta | None, optional): 命令元信息
-            namespace (str | Namespace | None, optional): 命令命名空间, 默认为 'Alconna'
-            separators (str | set[str] | Sequence[str] | None, optional): 命令参数分隔符, 默认为 `' '`
-            behaviors (list[ArparmaBehavior] | None, optional): 命令解析行为器
-            formatter_type (type[TextFormatter] | None, optional): 指定的命令帮助文本格式器类型
-        """
-        if not namespace:
-            ns_config = config.default_namespace
-        elif isinstance(namespace, str):
-            ns_config = config.namespaces.setdefault(namespace, Namespace(namespace))
-        else:
-            ns_config = namespace
-        self.prefixes = next((i for i in args if isinstance(i, list)), ns_config.prefixes.copy())  # type: ignore
-        try:
-            self.command = next(i for i in args if not isinstance(i, (list, Option, Subcommand, Args, Arg)))
-        except StopIteration:
-            self.command = "" if self.prefixes else handle_argv()
-        self.namespace = ns_config.name
-        self.formatter = (formatter_type or ns_config.formatter_type or TextFormatter)()
-        self.meta = meta or CommandMeta()
-        if self.meta.example:
-            self.meta.example = self.meta.example.replace("$", str(self.prefixes[0]) if self.prefixes else "")
-        self.meta.fuzzy_match = self.meta.fuzzy_match or ns_config.fuzzy_match
-        self.meta.raise_exception = self.meta.raise_exception or ns_config.raise_exception
-        self.meta.compact = self.meta.compact or ns_config.compact
-        self.meta.context_style = self.meta.context_style or ns_config.context_style
-        options = [i for i in args if isinstance(i, (Option, Subcommand))]
-        add_builtin_options(options, ns_config)
-        name = f"{self.command or self.prefixes[0]}"  # type: ignore
-        self.path = f"{self.namespace}::{name}"
-        _args = sum((i for i in args if isinstance(i, (Args, Arg))), Args())
-        super().__init__("ALCONNA::", _args, *options, dest=name, separators=separators or ns_config.separators, help_text=self.meta.description)  # noqa: E501
-        self.name = name
-        self.aliases = frozenset((name,))
-        self.behaviors = []
-        for behavior in behaviors or []:
-            self.behaviors.extend(requirement_handler(behavior))
-        command_manager.register(self)
-        self._executors: dict[ArparmaExecutor, Any] = {}
-        self.union: "WeakSet[Alconna]" = WeakSet()
-
-    @property
-    def namespace_config(self) -> Namespace:
-        return config.namespaces[self.namespace]
-
-    def reset_namespace(self, namespace: Namespace | str, header: bool = True) -> Self:
-        """重新设置命名空间
-
-        Args:
-            namespace (Namespace | str): 命名空间
-            header (bool, optional): 是否保留命令头, 默认为 `True`
-        """
-        with command_manager.update(self):
-            if isinstance(namespace, str):
-                namespace = config.namespaces.setdefault(namespace, Namespace(namespace))
-            self.namespace = namespace.name
-            self.path = f"{self.namespace}::{self.name}"
-            if header:
-                self.prefixes = namespace.prefixes.copy()
-                name = f"{self.command or self.prefixes[0]}"  # type: ignore
-                self.dest = name
-                self.path = f"{self.namespace}::{name}"
-                self.aliases = frozenset((name,))
-            self.options = [opt for opt in self.options if not isinstance(opt, (Help, Completion, Shortcut))]
-            add_builtin_options(self.options, namespace)
-            self.meta.fuzzy_match = namespace.fuzzy_match or self.meta.fuzzy_match
-            self.meta.raise_exception = namespace.raise_exception or self.meta.raise_exception
-        return self
-
-    def get_help(self) -> str:
-        """返回该命令的帮助信息"""
-        return self.formatter.format_node()
-
-    def get_shortcuts(self) -> list[str]:
-        """返回该命令注册的快捷命令"""
-        result = []
-        shortcuts = command_manager.get_shortcut(self)
-        for key, short in shortcuts.items():
-            if isinstance(short, InnerShortcutArgs):
-                prefixes = f"[{'│'.join(short.prefixes)}]" if short.prefixes else ""
-                result.append(prefixes + key + (" ...args" if short.fuzzy else ""))
-            else:
-                result.append(key)
-        return result
-
-    def _get_shortcuts(self):
-        """返回该命令注册的快捷命令"""
-        return command_manager.get_shortcut(self)
-
-    @overload
-    def shortcut(self, key: str, args: ShortcutArgs | None = None) -> str:
-        """操作快捷命令
-
-        Args:
-            key (str): 快捷命令名
-            args (ShortcutArgs): 快捷命令参数, 不传入时则尝试使用最近一次使用的命令
-
-        Returns:
-            str: 操作结果
-
-        Raises:
-            ValueError: 快捷命令操作失败时抛出
-        """
-        ...
-
-    @overload
-    def shortcut(
-        self,
-        key: str,
-        *,
-        command: str | None = None,
-        arguments: list[Any] | None = None,
-        fuzzy: bool = True,
-        prefix: bool = False,
-        wrapper: ShortcutRegWrapper | None = None,
-        humanized: str | None = None,
-    ) -> str:
-        """操作快捷命令
-
-        Args:
-            key (str): 快捷命令名
-            command (str): 快捷命令指向的命令
-            arguments (list[Any] | None, optional): 快捷命令参数, 默认为 `None`
-            fuzzy (bool, optional): 是否允许命令后随参数, 默认为 `True`
-            prefix (bool, optional): 是否调用时保留指令前缀, 默认为 `False`
-            wrapper (ShortcutRegWrapper, optional): 快捷指令的正则匹配结果的额外处理函数, 默认为 `None`
-            humanized (str, optional): 快捷指令的人类可读描述, 默认为 `None`
-
-        Returns:
-            str: 操作结果
-
-        Raises:
-            ValueError: 快捷命令操作失败时抛出
-        """
-        ...
-
-    @overload
-    def shortcut(self, key: str, *, delete: Literal[True]) -> str:
-        """操作快捷命令
-
-        Args:
-            key (str): 快捷命令名
-            delete (bool): 是否删除快捷命令
-
-        Returns:
-            str: 操作结果
-
-        Raises:
-            ValueError: 快捷命令操作失败时抛出
-        """
-        ...
-
-    def shortcut(self, key: str, args: ShortcutArgs | None = None, delete: bool = False, **kwargs):
-        try:
-            if delete:
-                return command_manager.delete_shortcut(self, key)
-            if kwargs and not args:
-                kwargs["args"] = kwargs.pop("arguments", None)
-                kwargs = {k: v for k, v in kwargs.items() if v is not None}
-                args = cast(ShortcutArgs, kwargs)
-            if args is not None:
-                return command_manager.add_shortcut(self, key, args)
-            elif cmd := command_manager.recent_message:
-                alc = command_manager.last_using
-                if alc and alc == self.path:
-                    return command_manager.add_shortcut(self, key, {"command": cmd})  # type: ignore
-                raise ValueError(
-                    lang.require("shortcut", "recent_command_error").format(
-                        target=self.path, source=getattr(alc, "path", "Unknown")
-                    )
-                )
-            else:
-                raise ValueError(lang.require("shortcut", "no_recent_command"))
-        except Exception as e:
-            if self.meta.raise_exception:
-                raise e
-            return str(e)
-
-    def __repr__(self):
-        return f"{self.namespace}::{self.name}(args={self.args}, options={self.options})"
-
-    def add(self, opt: Option | Subcommand) -> Self:
-        """添加选项或子命令
-
-        Args:
-            opt (Option | Subcommand): 选项或子命令
-
-        Returns:
-            Self: 命令本身
-        """
-        with command_manager.update(self):
-            self.options.append(opt)
-        return self
-
-    @init_spec(Option, is_method=True)
-    def option(self, opt: Option) -> Self:
-        """添加选项"""
-        return self.add(opt)
-
-    @init_spec(Subcommand, is_method=True)
-    def subcommand(self, sub: Subcommand) -> Self:
-        """添加子命令"""
-        return self.add(sub)
-
-    def _parse(self, message: TDC, ctx: dict[str, Any] | None = None) -> Arparma[TDC]:
-        analyser = command_manager.require(self)
-        argv = command_manager.resolve(self)
-        argv.enter(ctx).build(message)
-        return analyser.process(argv)
-
-    def parse(self, message: TDC, ctx: dict[str, Any] | None = None) -> Arparma[TDC]:
-        """命令分析功能, 传入字符串或消息链, 返回一个特定的数据集合类
-
-        Args:
-            message (TDC): 命令消息
-            ctx (dict[str, Any], optional): 上下文信息
-        Returns:
-            Arparma[TDC] | T_Duplication: 若`duplication`参数为`None`则返回`Arparma`对象, 否则返回`duplication`类型的对象
-        Raises:
-            NullMessage: 传入的消息为空时抛出
-        """
-        try:
-            arp = self._parse(message, ctx)
-        except NullMessage as e:
-            if self.meta.raise_exception:
-                raise e
-            return Arparma(self.path, message, False, error_info=e, ctx=ctx)
-        if arp.matched:
-            arp = arp.execute(self.behaviors)
-            if self._executors:
-                for ext in self._executors:
-                    self._executors[ext] = arp.call(ext.target)
-        return arp
-
-    def bind(self, active: bool = True):
-        """绑定命令执行器
-
-        Args:
-            active (bool, optional): 该执行器是否由 `Alconna` 主动调用, 默认为 `True`
-        """
-
-        def wrapper(target: Callable[..., T]) -> ArparmaExecutor[T]:
-            ext = ArparmaExecutor(target, lambda: command_manager.get_result(self))
-            if active:
-                self._executors[ext] = None
-            return ext
-
-        return wrapper
-
-    @property
-    def exec_result(self) -> dict[str, Any]:
-        return {ext.target.__name__: res for ext, res in self._executors.items() if res is not None}
-
-    def __truediv__(self, other) -> Self:
-        return self.reset_namespace(other)
-
-    __rtruediv__ = __truediv__
-
-    def __add__(self, other) -> Self:
-        with command_manager.update(self):
-            if isinstance(other, Alconna):
-                self.options.extend(other.options)
-            elif isinstance(other, CommandMeta):
-                self.meta = other
-            elif isinstance(other, Option):
-                self.options.append(other)
-            elif isinstance(other, Args):
-                self.args += other
-                self.nargs = len(self.args)
-            elif isinstance(other, str):
-                self.options.append(Option(other))
-        return self
-
-    def __or__(self, other: Alconna) -> Self:
-        self.union.add(other)
-
-        def _parse(message: TDC, ctx: dict[str, Any] | None = None) -> Arparma[TDC]:
-            for ana, argv in command_manager.unpack(self.union):
-                if (res := ana.process(argv.enter(ctx).build(message))).matched:
-                    return res
-            return command_manager.require(self).process(command_manager.resolve(self).enter(ctx).build(message))
-
-        self._parse = _parse
-        return self
-
-    def _calc_hash(self):
-        return hash((self.path + str(self.prefixes), self.meta, *self.options, *self.args))
-
-    def __call__(self, *args):
-        if args:
-            return self.parse(list(args))  # type: ignore
-        head = handle_argv()
-        argv = [(f"\"{arg}\"" if any(arg.count(sep) for sep in self.separators) else arg) for arg in sys.argv[1:]]
-        if head != self.command:
-            return self.parse(argv)  # type: ignore
-        return self.parse([head, *argv])  # type: ignore
-
-    @property
-    def header_display(self):
-        ana = command_manager.require(self)
-        return str(ana.command_header)
-
-
-__all__ = ["Alconna", "ArparmaExecutor"]
+"""Alconna 主体"""
+from __future__ import annotations
+
+import sys
+from dataclasses import dataclass, field, is_dataclass
+from functools import partial
+from pathlib import Path
+from typing import Any, Callable, Generic, Sequence, TypeVar, overload
+
+from tarina import init_spec, lang
+from typing_extensions import Self
+
+from ._internal._analyser import Analyser, TCompile
+from .args import Arg, Args
+from .arparma import Arparma, ArparmaBehavior, requirement_handler
+from .base import Option, Subcommand
+from .config import Namespace, config
+from .exceptions import ExecuteFailed, NullMessage
+from .formatter import TextFormatter
+from .manager import ShortcutArgs, command_manager
+from .typing import TDC, CommandMeta, DataCollection, TPrefixes
+
+T = TypeVar("T")
+TDC1 = TypeVar("TDC1", bound=DataCollection[Any])
+
+
+def handle_argv():
+    path = Path(sys.argv[0])
+    if str(path) == ".":
+        path = path.absolute()
+    head = path.stem
+    if head == "__main__":
+        head = path.parent.stem
+    return head
+
+
+def add_builtin_options(options: list[Option | Subcommand], ns: Namespace) -> None:
+    options.append(
+        Option("|".join(ns.builtin_option_name['help']), help_text=lang.require("builtin", "option_help")),
+    )
+    options.append(
+        Option(
+            "|".join(ns.builtin_option_name['shortcut']),
+            Args["action?", "delete|list"]["name?", str]["command", str, "$"],
+            help_text=lang.require("builtin", "option_shortcut")
+        )
+    )
+    options.append(
+        Option(
+            "|".join(ns.builtin_option_name['completion']),
+            help_text=lang.require("builtin", "option_completion")
+        )
+    )
+
+
+@dataclass(init=True, unsafe_hash=True)
+class ArparmaExecutor(Generic[T]):
+    """Arparma 执行器
+
+    Attributes:
+        target(Callable[..., T]): 目标函数
+    """
+    target: Callable[..., T]
+    binding: Callable[..., list[Arparma]] = field(default=lambda: [], repr=False)
+
+    __call__ = lambda self, *args, **kwargs: self.target(*args, **kwargs)
+
+    @property
+    def result(self) -> T:
+        """执行结果"""
+        if not self.binding:
+            raise ExecuteFailed(None)
+        arps = self.binding()
+        if not arps or not arps[0].matched:
+            raise ExecuteFailed("Unmatched")
+        try:
+            return arps[0].call(self.target)
+        except Exception as e:
+            raise ExecuteFailed(e) from e
+
+
+class Alconna(Subcommand, Generic[TDC]):
+    """
+    更加精确的命令解析
+
+    Examples:
+
+        >>> from arclet.alconna import Alconna
+        >>> alc = Alconna(
+        ...     "name",
+        ...     ["p1", "p2"],
+        ...     Option("opt", Args["opt_arg", "opt_arg"]),
+        ...     Subcommand(
+        ...         "sub_name",
+        ...         Option("sub_opt", Args["sub_arg", "sub_arg"]),
+        ...         Args["sub_main_args", "sub_main_args"]
+        ...     ),
+        ...     Args["main_args", "main_args"],
+        ...  )
+        >>> alc.parse("name opt opt_arg")
+    """
+    prefixes: TPrefixes
+    """命令前缀"""
+    command: str | Any
+    """命令名"""
+    formatter: TextFormatter
+    """文本格式化器"""
+    namespace: str
+    """命名空间"""
+    meta: CommandMeta
+    """命令元数据"""
+    behaviors: list[ArparmaBehavior]
+    """命令行为器"""
+
+    @property
+    def compile(self) -> Callable[[TCompile | None], Analyser[TDC]]:
+        """编译 `Alconna` 为对应的解析器"""
+        return partial(Analyser, self)
+
+    def __init__(
+        self,
+        *args: Option | Subcommand | str | TPrefixes | Any | Args | Arg,
+        meta: CommandMeta | None = None,
+        namespace: str | Namespace | None = None,
+        separators: str | set[str] | Sequence[str] | None = None,
+        behaviors: list[ArparmaBehavior] | None = None,
+        formatter_type: type[TextFormatter] | None = None
+    ):
+        """
+        以标准形式构造 `Alconna`
+
+        Args:
+            *args (Option | Subcommand | str | TPrefixes | Any | Args | Arg): 命令选项、主参数、命令名称或命令头
+            action (ArgAction | Callable | None, optional): 命令解析后针对主参数的回调函数
+            meta (CommandMeta | None, optional): 命令元信息
+            namespace (str | Namespace | None, optional): 命令命名空间, 默认为 'Alconna'
+            separators (str | set[str] | Sequence[str] | None, optional): 命令参数分隔符, 默认为 `' '`
+            behaviors (list[ArparmaBehavior] | None, optional): 命令解析行为器
+            formatter_type (type[TextFormatter] | None, optional): 指定的命令帮助文本格式器类型
+        """
+        if not namespace:
+            ns_config = config.default_namespace
+        elif isinstance(namespace, str):
+            ns_config = config.namespaces.setdefault(namespace, Namespace(namespace))
+        else:
+            ns_config = namespace
+        self.prefixes = next((i for i in args if isinstance(i, list)), ns_config.prefixes.copy())  # type: ignore
+        try:
+            self.command = next(i for i in args if not isinstance(i, (list, Option, Subcommand, Args, Arg)))
+        except StopIteration:
+            self.command = "" if self.prefixes else handle_argv()
+        self.namespace = ns_config.name
+        self.formatter = (formatter_type or ns_config.formatter_type or TextFormatter)()
+        self.meta = meta or CommandMeta()
+        if self.meta.example:
+            self.meta.example = self.meta.example.replace("$", str(self.prefixes[0]) if self.prefixes else "")
+        self.meta.fuzzy_match = self.meta.fuzzy_match or ns_config.fuzzy_match
+        self.meta.raise_exception = self.meta.raise_exception or ns_config.raise_exception
+        self.meta.compact = self.meta.compact or ns_config.compact
+        options = [i for i in args if isinstance(i, (Option, Subcommand))]
+        add_builtin_options(options, ns_config)
+        name = f"{self.command or self.prefixes[0]}"  # type: ignore
+        self.path = f"{self.namespace}::{name}"
+        _args = sum((i for i in args if isinstance(i, (Args, Arg))), Args())
+        super().__init__(
+            "ALCONNA::",
+            _args, *options, dest=name, separators=separators or ns_config.separators, help_text=self.meta.description
+        )
+        self.name = name
+        self.behaviors = []
+        for behavior in behaviors or []:
+            self.behaviors.extend(requirement_handler(behavior))
+        command_manager.register(self)
+        self._executors: dict[ArparmaExecutor, Any] = {}
+        self.union = set()
+
+    @property
+    def namespace_config(self) -> Namespace:
+        return config.namespaces[self.namespace]
+
+    def reset_namespace(self, namespace: Namespace | str, header: bool = True) -> Self:
+        """重新设置命名空间
+
+        Args:
+            namespace (Namespace | str): 命名空间
+            header (bool, optional): 是否保留命令头, 默认为 `True`
+        """
+        command_manager.delete(self)
+        if isinstance(namespace, str):
+            namespace = config.namespaces.setdefault(namespace, Namespace(namespace))
+        self.namespace = namespace.name
+        self.path = f"{self.namespace}::{self.name}"
+        if header:
+            self.prefixes = namespace.prefixes.copy()
+        self.options = self.options[:-3]
+        add_builtin_options(self.options, namespace)
+        self.meta.fuzzy_match = namespace.fuzzy_match or self.meta.fuzzy_match
+        self.meta.raise_exception = namespace.raise_exception or self.meta.raise_exception
+        self._hash = self._calc_hash()
+        command_manager.register(self)
+        return self
+
+    def get_help(self) -> str:
+        """返回该命令的帮助信息"""
+        return self.formatter.format_node()
+
+    def get_shortcuts(self) -> list[str]:
+        """返回该命令注册的快捷命令"""
+        return command_manager.list_shortcut(self)
+
+    def shortcut(self, key: str, args: ShortcutArgs | None = None, delete: bool = False):
+        """操作快捷命令
+
+        Args:
+            key (str): 快捷命令名
+            args (ShortcutArgs[TDC] | None, optional): 快捷命令参数, 不传入时则尝试使用最近一次使用的命令
+            delete (bool, optional): 是否删除快捷命令, 默认为 `False`
+
+        Returns:
+            str: 操作结果
+
+        Raises:
+            ValueError: 快捷命令操作失败时抛出
+        """
+        try:
+            if delete:
+                command_manager.delete_shortcut(self, key)
+                return lang.require("shortcut", "delete_success").format(shortcut=key, target=self.path)
+            if args is not None:
+                return command_manager.add_shortcut(self, key, args)
+            elif cmd := command_manager.recent_message:
+                alc = command_manager.last_using
+                if alc and alc == self:
+                    return command_manager.add_shortcut(self, key, {"command": cmd})  # type: ignore
+                raise ValueError(
+                    lang.require("shortcut", "recent_command_error")
+                    .format(target=self.path, source=getattr(alc, "path", "Unknown"))
+                )
+            else:
+                raise ValueError(lang.require("shortcut", "no_recent_command"))
+        except Exception as e:
+            if self.meta.raise_exception:
+                raise e
+            return str(e)
+
+    def __repr__(self):
+        return f"{self.namespace}::{self.name}(args={self.args}, options={self.options})"
+
+    def add(self, opt: Option | Subcommand) -> Self:
+        """添加选项或子命令
+
+        Args:
+            opt (Option | Subcommand): 选项或子命令
+
+        Returns:
+            Self: 命令本身
+        """
+        command_manager.delete(self)
+        self.options.insert(-3, opt)
+        self._hash = self._calc_hash()
+        command_manager.register(self)
+        return self
+
+    @init_spec(Option, True)
+    def option(self, opt: Option) -> Self:
+        """添加选项"""
+        return self.add(opt)
+
+    @init_spec(Subcommand, True)
+    def subcommand(self, sub: Subcommand) -> Self:
+        """添加子命令"""
+        return self.add(sub)
+
+    def _parse(self, message: TDC) -> Arparma[TDC]:
+        if self.union:
+            for ana, argv in command_manager.requires(*self.union):
+                if (res := ana.process(argv.build(message))).matched:
+                    return res
+        analyser = command_manager.require(self)
+        argv = command_manager.resolve(self)
+        argv.build(message)
+        return analyser.process(argv)
+
+    @overload
+    def parse(self, message: TDC) -> Arparma[TDC]:
+        ...
+
+    @overload
+    def parse(self, message, *, _config: type[T]) -> T:
+        ...
+
+    def parse(self, message: TDC, *, _config: type[T] | None = None) -> Arparma[TDC] | T:
+        """命令分析功能, 传入字符串或消息链, 返回一个特定的数据集合类
+        
+        Args:
+            message (TDC): 命令消息
+            _config (type[T], optional): 可选的解析结果配置
+        Returns:
+            Arparma[TDC] | T: 解析结果
+        Raises:
+            NullMessage: 传入的消息为空时抛出
+        """
+        try:
+            arp = self._parse(message)
+        except NullMessage as e:
+            if self.meta.raise_exception:
+                raise e
+            return Arparma(self.path, message, False, error_info=e)
+        if arp.matched:
+            arp = arp.execute(self.behaviors)
+            if self._executors:
+                for ext in self._executors:
+                    self._executors[ext] = arp.call(ext.target)
+        if _config:
+            if not is_dataclass(_config):
+                raise TypeError("The type of _config must be a dataclass")
+            return arp.call(_config)
+        return arp
+
+    def bind(self, active: bool = True):
+        """绑定命令执行器
+
+        Args:
+            active (bool, optional): 该执行器是否由 `Alconna` 主动调用, 默认为 `True`
+        """
+        def wrapper(target: Callable[..., T]) -> ArparmaExecutor[T]:
+            ext = ArparmaExecutor(target, lambda: command_manager.get_result(self))
+            if active:
+                self._executors[ext] = None
+            return ext
+        return wrapper
+
+    @property
+    def exec_result(self) -> dict[str, Any]:
+        return {ext.target.__name__: res for ext, res in self._executors.items() if res is not None}
+
+
+    def __truediv__(self, other) -> Self:
+        return self.reset_namespace(other)
+
+    __rtruediv__ = __truediv__
+
+    def __add__(self, other) -> Self:
+        command_manager.delete(self)
+        if isinstance(other, Alconna):
+            self.options.extend(other.options)
+        elif isinstance(other, CommandMeta):
+            self.meta = other
+        elif isinstance(other, Option):
+            self.options.append(other)
+        elif isinstance(other, Args):
+            self.args += other
+            self.nargs = len(self.args)
+        elif isinstance(other, str):
+            self.options.append(Option(other))
+        self._hash = self._calc_hash()
+        command_manager.register(self)
+        return self
+
+    def __or__(self, other: Alconna) -> Self:
+        self.union.add(other.path)
+        return self
+
+    def _calc_hash(self):
+        return hash((self.path + str(self.prefixes), self.meta, *self.options, *self.args))
+
+    def __call__(self, *args, **kwargs):
+        if args:
+            return self.parse(list(args))  # type: ignore
+        head = handle_argv()
+        if head != self.command:
+            return self.parse(sys.argv[1:])  # type: ignore
+        return self.parse([head, *sys.argv[1:]])  # type: ignore
+
+    @property
+    def headers(self):
+        return self.prefixes
+
+
+__all__ = ["Alconna", "ArparmaExecutor"]
```

### Comparing `arclet_alconna-1.8.8/src/arclet/alconna/manager.py` & `arclet_alconna-2.0.0a1/src/arclet/alconna/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,463 +1,449 @@
-"""Alconna 负责记录命令的部分"""
-
-from __future__ import annotations
-
-import contextlib
-import re
-import shelve
-import weakref
-from copy import copy
-from datetime import datetime
-from typing import TYPE_CHECKING, Any, Match, MutableSet, Union
-from weakref import WeakKeyDictionary, WeakValueDictionary
-
-from tarina import LRU, lang
-
-from .argv import Argv, __argv_type__
-from .arparma import Arparma
-from .config import Namespace, config
-from .exceptions import ExceedMaxCount
-from .typing import TDC, CommandMeta, DataCollection, InnerShortcutArgs, ShortcutArgs
-
-if TYPE_CHECKING:
-    from ._internal._analyser import Analyser
-    from .core import Alconna
-
-
-class CommandManager:
-    """
-    `Alconna` 命令管理器
-
-    命令管理器负责记录命令, 存储命令, 命令行参数, 命令解析器, 快捷指令等
-    """
-
-    sign: str
-    current_count: int
-    max_count: int
-
-    __commands: dict[str, WeakValueDictionary[str, Alconna]]
-    __analysers: WeakKeyDictionary[Alconna, Analyser]
-    __argv: WeakKeyDictionary[Alconna, Argv]
-    __abandons: list[Alconna]
-    __record: LRU[int, Arparma]
-    __shortcuts: dict[str, tuple[dict[str, Union[Arparma, InnerShortcutArgs]], dict[str, Union[Arparma, InnerShortcutArgs]]]]
-
-    def __init__(self):
-        self.cache_path = f"{__file__.replace('manager.py', '')}manager_cache.db"
-        self.sign = "ALCONNA::"
-        self.max_count = config.command_max_count
-        self.current_count = 0
-
-        self.__commands = {}
-        self.__argv = WeakKeyDictionary()
-        self.__analysers = WeakKeyDictionary()
-        self.__abandons = []
-        self.__shortcuts = {}
-        self.__record = LRU(128)
-
-        def _del():
-            self.__commands.clear()
-            for ana in self.__analysers.values():
-                ana._clr()
-            self.__analysers.clear()
-            self.__abandons.clear()
-            for arp in self.__record.values():
-                arp._clr()
-            self.__record.clear()
-            self.__shortcuts.clear()
-
-        weakref.finalize(self, _del)
-
-    def load_cache(self) -> None:
-        """加载缓存"""
-        with contextlib.suppress(FileNotFoundError, KeyError):
-            with shelve.open(self.cache_path) as db:
-                self.__shortcuts = dict(db["shortcuts"])  # type: ignore
-
-    def dump_cache(self) -> None:
-        """保存缓存"""
-        data = {}
-        for key, short in self.__shortcuts.items():
-            if isinstance(short, dict):
-                data[key] = {k: v for k, v in short.items() if k != "wrapper"}
-            else:
-                data[key] = short
-        with shelve.open(self.cache_path) as db:
-            db["shortcuts"] = data
-        data.clear()
-
-    @property
-    def get_loaded_namespaces(self):
-        """获取所有命名空间
-
-        Returns:
-            list[str]: 所有命名空间的名称
-        """
-        return list(self.__commands.keys())
-
-    @staticmethod
-    def _command_part(command: str) -> tuple[str, str]:
-        """获取命令的组成部分"""
-        command_parts = command.split("::", maxsplit=1)[-2:]
-        if len(command_parts) != 2:
-            command_parts.insert(0, config.default_namespace.name)
-        return command_parts[0], command_parts[1]
-
-    def get_namespace_config(self, name: str) -> Namespace | None:
-        if name not in self.__commands:
-            return
-        return config.namespaces.get(name)
-
-    def register(self, command: Alconna) -> None:
-        """注册命令解析器, 会同时记录解析器对应的命令"""
-        if self.current_count >= self.max_count:
-            raise ExceedMaxCount
-        self.__argv.pop(command, None)
-        argv = self.__argv[command] = __argv_type__.get()(command.meta, command.namespace_config, command.separators)  # type: ignore
-        self.__analysers.pop(command, None)
-        self.__analysers[command] = command.compile(param_ids=argv.param_ids)
-        namespace = self.__commands.setdefault(command.namespace, WeakValueDictionary())
-        if _cmd := namespace.get(command.name):
-            if _cmd == command:
-                return
-            _cmd.formatter.add(command)
-            command.formatter = _cmd.formatter
-        else:
-            command.formatter.add(command)
-            namespace[command.name] = command
-            self.current_count += 1
-
-    def resolve(self, command: Alconna[TDC]) -> Argv[TDC]:
-        """获取命令解析器的参数解析器"""
-        try:
-            return self.__argv[command]
-        except KeyError as e:
-            namespace, name = self._command_part(command.path)
-            raise ValueError(lang.require("manager", "undefined_command").format(target=f"{namespace}.{name}")) from e
-
-    def require(self, command: Alconna[TDC]) -> Analyser[TDC]:
-        """获取命令解析器"""
-        try:
-            return self.__analysers[command]  # type: ignore
-        except KeyError as e:
-            namespace, name = self._command_part(command.path)
-            raise ValueError(lang.require("manager", "undefined_command").format(target=f"{namespace}.{name}")) from e
-
-    def unpack(self, commands: MutableSet[Alconna]) -> "zip[tuple[Analyser, Argv]]":
-        """获取多个命令解析器"""
-        return zip(
-            [v for k, v in self.__analysers.items() if k in commands],
-            [v for k, v in self.__argv.items() if k in commands],
-        )
-
-    def delete(self, command: Alconna | str) -> None:
-        """删除命令"""
-        namespace, name = self._command_part(command if isinstance(command, str) else command.path)
-        try:
-            base = self.__commands[namespace][name]
-            base.formatter.remove(base)
-            del self.__argv[base]
-            del self.__analysers[base]
-            del self.__commands[namespace][name]
-            self.current_count -= 1
-        except KeyError:
-            if self.__commands.get(namespace) == {}:
-                del self.__commands[namespace]
-
-    @contextlib.contextmanager
-    def update(self, command: Alconna):
-        """同步命令更改"""
-        if command not in self.__argv:
-            raise ValueError(lang.require("manager", "undefined_command").format(target=command.path))
-        command.formatter.remove(command)
-        argv = self.__argv.pop(command)
-        analyser = self.__analysers.pop(command)
-        yield
-        command._hash = command._calc_hash()
-        argv.namespace = command.namespace_config
-        argv.separators = command.separators
-        argv.__post_init__(command.meta)
-        argv.param_ids.clear()
-        analyser.compile(argv.param_ids)
-        self.__argv[command] = argv
-        self.__analysers[command] = analyser
-        command.formatter.add(command)
-
-    def is_disable(self, command: Alconna) -> bool:
-        """判断命令是否被禁用"""
-        return command in self.__abandons
-
-    def set_enabled(self, command: Alconna | str, enabled: bool):
-        """设置命令是否被禁用"""
-        if isinstance(command, str):
-            command = self.get_command(command)
-        if enabled and command in self.__abandons:
-            self.__abandons.remove(command)
-        if not enabled and command not in self.__abandons:
-            self.__abandons.append(command)
-
-    def add_shortcut(self, target: Alconna, key: str, source: Arparma | ShortcutArgs):
-        """添加快捷命令
-
-        Args:
-            target (Alconna): 目标命令
-            key (str): 快捷命令的名称
-            source (Arparma | ShortcutArgs): 快捷命令的参数
-        """
-        namespace, name = self._command_part(target.path)
-        argv = self.resolve(target)
-        _shortcut = self.__shortcuts.setdefault(f"{namespace}.{name}", ({}, {}))
-        if isinstance(source, dict):
-            humanize = source.pop("humanized", None)
-            if source.get("prefix", False) and target.prefixes:
-                prefixes = []
-                out = []
-                for prefix in target.prefixes:
-                    if not isinstance(prefix, str):
-                        continue
-                    prefixes.append(prefix)
-                    _shortcut[1][f"{re.escape(prefix)}{key}"] = InnerShortcutArgs(
-                        **{**source, "command": argv.converter(prefix + source.get("command", str(target.command)))}
-                    )
-                    out.append(
-                        lang.require("shortcut", "add_success").format(shortcut=f"{prefix}{key}", target=target.path)
-                    )
-                _shortcut[0][humanize or key] = InnerShortcutArgs(
-                    **{**source, "command": argv.converter(source.get("command", str(target.command))), "prefixes": prefixes}
-                )
-                target.formatter.update_shortcut(target)
-                return "\n".join(out)
-            _shortcut[0][humanize or key] = _shortcut[1][key] = InnerShortcutArgs(
-                **{**source, "command": argv.converter(source.get("command", str(target.command)))}
-            )
-            target.formatter.update_shortcut(target)
-            return lang.require("shortcut", "add_success").format(shortcut=key, target=target.path)
-        elif source.matched:
-            _shortcut[0][key] = _shortcut[1][key] = source
-            target.formatter.update_shortcut(target)
-            return lang.require("shortcut", "add_success").format(shortcut=key, target=target.path)
-        else:
-            raise ValueError(lang.require("manager", "incorrect_shortcut").format(target=f"{key}"))
-
-    def get_shortcut(self, target: Alconna[TDC]) -> dict[str, Union[Arparma[TDC], InnerShortcutArgs]]:
-        """列出快捷命令
-
-        Args:
-            target (Alconna): 目标命令
-
-        Returns:
-            dict[str, Arparma | InnerShortcutArgs]: 快捷命令的参数
-        """
-        namespace, name = self._command_part(target.path)
-        if target not in self.__analysers:
-            raise ValueError(lang.require("manager", "undefined_command").format(target=f"{namespace}.{name}"))
-        shortcuts = self.__shortcuts.get(f"{namespace}.{name}", {})
-        if not shortcuts:
-            return {}
-        return shortcuts[0]
-
-    def find_shortcut(
-            self, target: Alconna[TDC], data: list
-    ) -> tuple[list, Arparma[TDC] | InnerShortcutArgs, Match[str] | None]:
-        """查找快捷命令
-
-        Args:
-            target (Alconna): 目标命令对象
-            data (list): 传入的命令数据
-
-        Returns:
-            tuple[list, Union[Arparma, InnerShortcutArgs], re.Match[str]]: 返回匹配的快捷命令
-        """
-        namespace, name = self._command_part(target.path)
-        if not (_shortcut := self.__shortcuts.get(f"{namespace}.{name}")):
-            raise ValueError(lang.require("manager", "undefined_command").format(target=f"{namespace}.{name}"))
-        query: str = data.pop(0)
-        while True:
-            if query in _shortcut[1]:
-                return data, _shortcut[1][query], None
-            for key, args in _shortcut[1].items():
-                if isinstance(args, InnerShortcutArgs) and args.fuzzy and (mat := re.match(f"^{key}", query)):
-                    if len(query) > mat.span()[1]:
-                        data.insert(0, query[mat.span()[1]:])
-                    return data, args, mat
-                elif mat := re.fullmatch(key, query):
-                    return data, _shortcut[1][key], mat
-            if not data:
-                break
-            next_data = data.pop(0)
-            if not isinstance(next_data, str):
-                break
-            query += f"{target.separators[0]}{next_data}"
-        raise ValueError(
-            lang.require("manager", "shortcut_parse_error").format(target=f"{namespace}.{name}", query=query)
-        )
-
-    def delete_shortcut(self, target: Alconna, key: str | None = None):
-        """删除快捷命令"""
-        namespace, name = self._command_part(target.path)
-        if not (_shortcut := self.__shortcuts.get(f"{namespace}.{name}")):
-            raise ValueError(lang.require("manager", "undefined_command").format(target=f"{namespace}.{name}"))
-        if key:
-            try:
-                _shortcut[0].pop(key, None)
-                del _shortcut[1][key]
-                return lang.require("shortcut", "delete_success").format(shortcut=key, target=target.path)
-            except KeyError as e:
-                raise ValueError(
-                    lang.require("manager", "shortcut_parse_error").format(target=f"{namespace}.{name}", query=key)
-                ) from e
-        else:
-            self.__shortcuts.pop(f"{namespace}.{name}")
-            return lang.require("shortcut", "delete_success").format(shortcut="all", target=target.path)
-
-    def get_command(self, command: str) -> Alconna:
-        """获取命令"""
-        namespace, name = self._command_part(command)
-        if namespace not in self.__commands or name not in self.__commands[namespace]:
-            raise ValueError(command)
-        return self.__commands[namespace][name]
-
-    def get_commands(self, namespace: str | Namespace = "") -> list[Alconna]:
-        """获取命令列表"""
-        if not namespace:
-            return list(self.__analysers.keys())
-        if isinstance(namespace, Namespace):
-            namespace = Namespace.name
-        if namespace not in self.__commands:
-            return []
-        return list(self.__commands[namespace].values())
-
-    def test(self, message: TDC, namespace: str | Namespace = "") -> Arparma[TDC] | None:
-        """将一段命令给当前空间内的所有命令测试匹配"""
-        for cmd in self.get_commands(namespace):
-            if (res := cmd.parse(message)) and res.matched:
-                return res
-
-    def broadcast(self, message: TDC, namespace: str | Namespace = "") -> WeakValueDictionary[str, Arparma[TDC]]:
-        """将一段命令给当前空间内的所有命令测试匹配"""
-        data = WeakValueDictionary()
-        for cmd in self.get_commands(namespace):
-            if (res := cmd.parse(message)) and res.matched:
-                data[cmd.path] = res
-        return data
-
-    def all_command_help(
-        self,
-        show_index: bool = False,
-        namespace: str | Namespace | None = None,
-        header: str | None = None,
-        pages: str | None = None,
-        footer: str | None = None,
-        max_length: int = -1,
-        page: int = 1,
-    ) -> str:
-        """
-        获取所有命令的帮助信息
-
-        Args:
-            show_index (bool, optional): 是否展示索引. Defaults to False.
-            namespace (str | Namespace | None, optional): 指定的命名空间, 如果为None则选择所有命令.
-            header (str | None, optional): 帮助信息的页眉.
-            pages (str | None, optional): 帮助信息的页码.
-            footer (str | None, optional): 帮助信息的页脚.
-            max_length (int, optional): 单个页面展示的最大长度. Defaults to -1.
-            page (int, optional): 当前页码. Defaults to 1.
-        """
-        pages = pages or lang.require("manager", "help_pages")
-        cmds = [cmd for cmd in self.get_commands(namespace or "") if not cmd.meta.hide]
-        slots = [(cmd.header_display, cmd.meta.description) for cmd in cmds]
-        header = header or lang.require("manager", "help_header")
-        if max_length < 1:
-            command_string = (
-                "\n".join(f" {str(index).rjust(len(str(len(cmds))), '0')} {slot[0]} : {slot[1]}" for index, slot in enumerate(slots))  # noqa: E501
-                if show_index
-                else "\n".join(f" - {n} : {d}" for n, d in slots)
-            )
-        else:
-            max_page = len(cmds) // max_length + 1
-            if page < 1 or page > max_page:
-                page = 1
-            header += "\t" + pages.format(current=page, total=max_page)
-            command_string = (
-                "\n".join(
-                    f" {str(index).rjust(len(str(page * max_length)), '0')} {slot[0]} : {slot[1]}"
-                    for index, slot in enumerate(slots[(page - 1) * max_length: page * max_length], start=(page - 1) * max_length)  # noqa: E501
-                )
-                if show_index
-                else "\n".join(f" - {n} : {d}" for n, d in slots[(page - 1) * max_length: page * max_length])
-            )
-        help_names = set()
-        for i in cmds:
-            help_names.update(i.namespace_config.builtin_option_name["help"])
-        footer = footer or lang.require("manager", "help_footer").format(help="|".join(help_names))
-        return f"{header}\n{command_string}\n{footer}"
-
-    def all_command_raw_help(self, namespace: str | Namespace | None = None) -> dict[str, CommandMeta]:
-        """获取所有命令的原始帮助信息"""
-        cmds = list(filter(lambda x: not x.meta.hide, self.get_commands(namespace or "")))
-        return {cmd.path: copy(cmd.meta) for cmd in cmds}
-
-    def command_help(self, command: str) -> str | None:
-        """获取单个命令的帮助"""
-        if cmd := self.get_command(command):
-            return cmd.get_help()
-
-    def record(self, token: int, result: Arparma):
-        """记录某个命令的 `token`"""
-        self.__record[token] = result
-
-    def get_record(self, token: int) -> Arparma | None:
-        """获取某个 `token` 对应的 `Arparma` 对象"""
-        if token in self.__record:
-            return self.__record[token]
-
-    def get_token(self, result: Arparma) -> int:
-        """获取某个命令的 `token`"""
-        return next((token for token, res in self.__record.items() if res == result), 0)
-
-    def get_result(self, command: Alconna) -> list[Arparma]:
-        """获取某个命令的所有 `Arparma` 对象"""
-        return [v for v in self.__record.values() if v.source == command.path]
-
-    @property
-    def recent_message(self) -> DataCollection[str | Any] | None:
-        """获取最近一次使用的命令"""
-        if rct := self.__record.peek_first_item():
-            return rct[1].origin  # type: ignore
-
-    @property
-    def last_using(self):
-        """获取最近一次使用的 `Alconna` 对象"""
-        if rct := self.__record.peek_first_item():
-            return rct[1].source  # type: ignore
-
-    @property
-    def records(self) -> LRU[int, Arparma]:
-        """获取当前记录"""
-        return self.__record
-
-    def reuse(self, index: int = -1):
-        """获取当前记录中的某个值"""
-        key = self.__record.keys()[index]
-        return self.__record[key]
-
-    def set_record_size(self, size: int):
-        """设置记录的最大长度"""
-        self.__record.set_size(size)
-
-    def __repr__(self):
-        return (
-            f"Current: {hex(id(self))} in {datetime.now().strftime('%Y/%m/%d %H:%M:%S')}\n"
-            + "Commands:\n"
-            + f"[{', '.join([cmd.path for cmd in self.get_commands()])}]"
-            + "\nShortcuts:\n"
-            + "\n".join([f" {k} => {v}" for short in self.__shortcuts.values() for k, v in short[0].items()])
-            + "\nRecords:\n"
-            + "\n".join([f" [{k}]: {v[1].origin}" for k, v in enumerate(self.__record.items()[:20])])
-            + "\nDisabled Commands:\n"
-            + f"[{', '.join(map(lambda x: x.path, self.__abandons))}]"
-        )
-
-
-command_manager = CommandManager()
-__all__ = ["ShortcutArgs", "command_manager"]
+"""Alconna 负责记录命令的部分"""
+
+from __future__ import annotations
+
+import contextlib
+import re
+import shelve
+import weakref
+from copy import copy
+from datetime import datetime
+from typing import TYPE_CHECKING, Any, Match, TypedDict, Union, overload
+from weakref import WeakKeyDictionary, WeakValueDictionary
+
+from tarina import LRU, lang
+from typing_extensions import NotRequired
+
+from .argv import Argv, __argv_type__
+from .arparma import Arparma
+from .config import Namespace, config
+from .exceptions import ExceedMaxCount
+from .typing import TDC, CommandMeta, DataCollection
+
+if TYPE_CHECKING:
+    from ._internal._analyser import Analyser
+    from .core import Alconna
+
+
+class ShortcutArgs(TypedDict):
+    """快捷指令参数"""
+
+    command: NotRequired[DataCollection[Any]]
+    """快捷指令的命令"""
+    args: NotRequired[list[Any]]
+    """快捷指令的附带参数"""
+    fuzzy: NotRequired[bool]
+    """是否允许命令后随参数"""
+    prefix: NotRequired[bool]
+    """是否调用时保留指令前缀"""
+
+
+class CommandManager:
+    """
+    `Alconna` 命令管理器
+
+    命令管理器负责记录命令, 存储命令, 命令行参数, 命令解析器, 快捷指令等
+    """
+
+    sign: str
+    current_count: int
+    max_count: int
+
+    __commands: dict[str, WeakValueDictionary[str, Alconna]]
+    __analysers: WeakKeyDictionary[Alconna, Analyser]
+    __argv: WeakKeyDictionary[Alconna, Argv]
+    __abandons: list[Alconna]
+    __record: LRU[int, Arparma]
+    __shortcuts: dict[str, Union[Arparma, ShortcutArgs]]
+
+    def __init__(self):
+        self.cache_path = f"{__file__.replace('manager.py', '')}manager_cache.db"
+        self.sign = "ALCONNA::"
+        self.max_count = config.command_max_count
+        self.current_count = 0
+
+        self.__commands = {}
+        self.__argv = WeakKeyDictionary()
+        self.__analysers = WeakKeyDictionary()
+        self.__abandons = []
+        self.__shortcuts = {}
+        self.__record = LRU(128)
+
+        def _del():
+            self.__commands.clear()
+            for ana in self.__analysers.values():
+                ana._clr()
+            self.__analysers.clear()
+            self.__abandons.clear()
+            for arp in self.__record.values():
+                arp._clr()
+            self.__record.clear()
+            self.__shortcuts.clear()
+
+        weakref.finalize(self, _del)
+
+    def load_cache(self) -> None:
+        """加载缓存"""
+        with contextlib.suppress(FileNotFoundError, KeyError):
+            with shelve.open(self.cache_path) as db:
+                self.__shortcuts = dict(db["shortcuts"])  # type: ignore
+
+    def dump_cache(self) -> None:
+        """保存缓存"""
+        with shelve.open(self.cache_path) as db:
+            db["shortcuts"] = self.__shortcuts
+
+    @property
+    def get_loaded_namespaces(self):
+        """获取所有命名空间
+
+        Returns:
+            list[str]: 所有命名空间的名称
+        """
+        return list(self.__commands.keys())
+
+    @staticmethod
+    def _command_part(command: str) -> tuple[str, str]:
+        """获取命令的组成部分"""
+        command_parts = command.split("::", maxsplit=1)[-2:]
+        if len(command_parts) != 2:
+            command_parts.insert(0, config.default_namespace.name)
+        return command_parts[0], command_parts[1]
+
+    def get_namespace_config(self, name: str) -> Namespace | None:
+        if name not in self.__commands:
+            return
+        return config.namespaces.get(name)
+
+    def register(self, command: Alconna) -> None:
+        """注册命令解析器, 会同时记录解析器对应的命令"""
+        if self.current_count >= self.max_count:
+            raise ExceedMaxCount
+        self.__argv.pop(command, None)
+        self.__argv[command] = __argv_type__.get()(
+            command.namespace_config,  # type: ignore
+            fuzzy_match=command.meta.fuzzy_match,  # type: ignore
+            to_text=command.namespace_config.to_text,  # type: ignore
+            converter=command.namespace_config.converter,  # type: ignore
+            separators=command.separators,  # type: ignore
+            message_cache=command.namespace_config.enable_message_cache,  # type: ignore
+            filter_crlf=not command.meta.keep_crlf,  # type: ignore
+        )
+        self.__analysers.pop(command, None)
+        self.__analysers[command] = command.compile(None)
+        namespace = self.__commands.setdefault(command.namespace, WeakValueDictionary())
+        if _cmd := namespace.get(command.name):
+            if _cmd == command:
+                return
+            _cmd.formatter.add(command)
+            command.formatter = _cmd.formatter
+        else:
+            command.formatter.add(command)
+            namespace[command.name] = command
+            self.current_count += 1
+
+    def resolve(self, command: Alconna[TDC]) -> Argv[TDC]:
+        """获取命令解析器的参数解析器"""
+        try:
+            return self.__argv[command]
+        except KeyError as e:
+            namespace, name = self._command_part(command.path)
+            raise ValueError(lang.require("manager", "undefined_command").format(target=f"{namespace}.{name}")) from e
+
+    def require(self, command: Alconna[TDC]) -> Analyser[TDC]:
+        """获取命令解析器"""
+        try:
+            return self.__analysers[command]  # type: ignore
+        except KeyError as e:
+            namespace, name = self._command_part(command.path)
+            raise ValueError(lang.require("manager", "undefined_command").format(target=f"{namespace}.{name}")) from e
+
+    def requires(self, *paths: str) -> zip[tuple[Analyser, Argv]]:  # type: ignore
+        """获取多个命令解析器"""
+        return zip(
+            [v for k, v in self.__analysers.items() if k.path in paths],
+            [v for k, v in self.__argv.items() if k.path in paths],
+        )
+
+    def delete(self, command: Alconna | str) -> None:
+        """删除命令"""
+        namespace, name = self._command_part(command if isinstance(command, str) else command.path)
+        try:
+            base = self.__commands[namespace][name]
+            base.formatter.remove(base)
+            del self.__argv[base]
+            del self.__analysers[base]
+            del self.__commands[namespace][name]
+            self.current_count -= 1
+        except KeyError:
+            if self.__commands.get(namespace) == {}:
+                del self.__commands[namespace]
+
+    def is_disable(self, command: Alconna) -> bool:
+        """判断命令是否被禁用"""
+        return command in self.__abandons
+
+    def set_enabled(self, command: Alconna | str, enabled: bool):
+        """设置命令是否被禁用"""
+        if isinstance(command, str):
+            command = self.get_command(command)
+        if enabled and command in self.__abandons:
+            self.__abandons.remove(command)
+        if not enabled and command not in self.__abandons:
+            self.__abandons.append(command)
+
+    def add_shortcut(self, target: Alconna, key: str, source: Arparma | ShortcutArgs):
+        """添加快捷命令
+
+        Args:
+            target (Alconna): 目标命令
+            key (str): 快捷命令的名称
+            source (Arparma | ShortcutArgs): 快捷命令的参数
+        """
+        namespace, name = self._command_part(target.path)
+        argv = self.resolve(target)
+        if isinstance(source, dict):
+            source.setdefault('fuzzy', True)
+            source.setdefault('prefix', False)
+            if source.get("prefix") and target.prefixes:
+                out = []
+                for prefix in target.prefixes:
+                    if not isinstance(prefix, str):
+                        continue
+                    _src = source.copy()
+                    _src['command'] = argv.converter(prefix + source.get('command', str(target.command)))
+                    self.__shortcuts[f"{namespace}.{name}::{prefix}{key}"] = _src
+                    out.append(lang.require("shortcut", "add_success").format(
+                        shortcut=f"{prefix}{key}", target=target.path)
+                    )
+                return "\n".join(out)
+            source['command'] = argv.converter(source.get('command', target.command or target.name))
+            self.__shortcuts[f"{namespace}.{name}::{key}"] = source
+            return lang.require("shortcut", "add_success").format(shortcut=key, target=target.path)
+        elif source.matched:
+            self.__shortcuts[f"{namespace}.{name}::{key}"] = source
+            return lang.require("shortcut", "add_success").format(shortcut=key, target=target.path)
+        else:
+            raise ValueError(lang.require("manager", "incorrect_shortcut").format(target=f"{key}"))
+
+    def list_shortcut(self, target: Alconna) -> list[str]:
+        """列出快捷命令
+
+        Args:
+            target (Alconna): 目标命令
+
+        Returns:
+            list[str]: 快捷命令的名称
+        """
+        namespace, name = self._command_part(target.path)
+        result = []
+        for i in self.__shortcuts:
+            if not i.startswith(f"{namespace}.{name}::"):
+                continue
+            short = self.__shortcuts[i]
+            if isinstance(short, dict):
+                result.append(i.split('::')[1] + (" ..." if short.get('fuzzy') else ""))
+            else:
+                result.append(i.split('::')[1])
+        return result
+
+    @overload
+    def find_shortcut(
+        self, target: Alconna[TDC]
+    ) -> list[Union[Arparma[TDC], ShortcutArgs]]:
+        ...
+
+    @overload
+    def find_shortcut(
+        self, target: Alconna[TDC], query: str
+    ) -> tuple[Arparma[TDC] | ShortcutArgs, Match[str] | None]:
+        ...
+
+    def find_shortcut(self, target: Alconna[TDC], query: str | None = None):
+        """查找快捷命令
+
+        Args:
+            target (Alconna): 目标命令
+            query (str, optional): 快捷命令的名称. Defaults to None.
+
+        Returns:
+            list[Union[Arparma, ShortcutArgs]] | tuple[Union[Arparma, ShortcutArgs], Match[str]]: \
+            快捷命令的参数, 若没有 `query` 则返回目标命令的所有快捷命令, 否则返回匹配的快捷命令
+        """
+        namespace, name = self._command_part(target.path)
+        if query:
+            try:
+                return self.__shortcuts[f"{namespace}.{name}::{query}"], None
+            except KeyError as e:
+                for k, args in self.__shortcuts.items():
+                    prefix, key = k.rsplit("::", 1)
+                    if f"{namespace}.{name}" != prefix:
+                        continue
+                    if isinstance(args, dict) and args["fuzzy"] and (mat := re.match(key, query)):
+                        return args, mat
+                    elif mat := re.fullmatch(key, query):
+                        return self.__shortcuts[k], mat
+                raise ValueError(
+                    lang.require("manager", "target_command_error").format(target=f"{namespace}.{name}", shortcut=query)
+                ) from e
+        return [self.__shortcuts[k] for k in self.__shortcuts if f"{namespace}.{name}" in k]
+
+    def delete_shortcut(self, target: Alconna, key: str | None = None):
+        """删除快捷命令"""
+        for res in [self.find_shortcut(target, key)[0]] if key else self.find_shortcut(target):
+            with contextlib.suppress(StopIteration):
+                self.__shortcuts.pop(next(filter(lambda x: self.__shortcuts[x] == res, self.__shortcuts)))
+
+    def get_command(self, command: str) -> Alconna:
+        """获取命令"""
+        namespace, name = self._command_part(command)
+        if namespace not in self.__commands or name not in self.__commands[namespace]:
+            raise ValueError(command)
+        return self.__commands[namespace][name]
+
+    def get_commands(self, namespace: str | Namespace = '') -> list[Alconna]:
+        """获取命令列表"""
+        if not namespace:
+            return list(self.__analysers.keys())
+        if isinstance(namespace, Namespace):
+            namespace = Namespace.name
+        if namespace not in self.__commands:
+            return []
+        return list(self.__commands[namespace].values())
+
+    def test(self, message: TDC, namespace: str | Namespace = '') -> Arparma[TDC] | None:
+        """将一段命令给当前空间内的所有命令测试匹配"""
+        for cmd in self.get_commands(namespace):
+            if (res := cmd.parse(message)) and res.matched:
+                return res
+
+    def broadcast(self, message: TDC, namespace: str | Namespace = '') -> WeakValueDictionary[str, Arparma[TDC]]:
+        """将一段命令给当前空间内的所有命令测试匹配"""
+        data = WeakValueDictionary()
+        for cmd in self.get_commands(namespace):
+            if (res := cmd.parse(message)) and res.matched:
+                data[cmd.path] = res
+        return data
+
+    def all_command_help(
+        self,
+        show_index: bool = False,
+        namespace: str | Namespace | None = None,
+        header: str | None = None,
+        pages: str | None = None,
+        footer: str | None = None,
+        max_length: int = -1,
+        page: int = 1
+    ) -> str:
+        """
+        获取所有命令的帮助信息
+
+        Args:
+            show_index (bool, optional): 是否展示索引. Defaults to False.
+            namespace (str | Namespace | None, optional): 指定的命名空间, 如果为None则选择所有命令.
+            header (str | None, optional): 帮助信息的页眉.
+            pages (str | None, optional): 帮助信息的页码.
+            footer (str | None, optional): 帮助信息的页脚.
+            max_length (int, optional): 单个页面展示的最大长度. Defaults to -1.
+            page (int, optional): 当前页码. Defaults to 1.
+        """
+        pages = pages or lang.require("manager", "help_pages")
+        cmds = list(filter(lambda x: not x.meta.hide, self.get_commands(namespace or '')))
+        header = header or lang.require("manager", "help_header")
+        if max_length < 1:
+            command_string = "\n".join(
+                f" {str(index).rjust(len(str(len(cmds))), '0')} {slot.name} : {slot.meta.description}"
+                for index, slot in enumerate(cmds)
+            ) if show_index else "\n".join(
+                f" - {cmd.name} : {cmd.meta.description}"
+                for cmd in cmds
+            )
+        else:
+            max_page = len(cmds) // max_length + 1
+            if page < 1 or page > max_page:
+                page = 1
+            header += "\t" + pages.format(current=page, total=max_page)
+            command_string = "\n".join(
+                f" {str(index).rjust(len(str(page * max_length)), '0')} {cmd.name} : {cmd.meta.description}"
+                for index, cmd in enumerate(
+                    cmds[(page - 1) * max_length: page * max_length], start=(page - 1) * max_length
+                )
+            ) if show_index else "\n".join(
+                f" - {cmd.name} : {cmd.meta.description}"
+                for cmd in cmds[(page - 1) * max_length: page * max_length]
+            )
+        help_names = set()
+        for i in cmds:
+            help_names.update(i.namespace_config.builtin_option_name['help'])
+        footer = footer or lang.require("manager", "help_footer").format(help="|".join(help_names))
+        return f"{header}\n{command_string}\n{footer}"
+
+    def all_command_raw_help(self, namespace: str | Namespace | None = None) -> dict[str, CommandMeta]:
+        """获取所有命令的原始帮助信息"""
+        cmds = list(filter(lambda x: not x.meta.hide, self.get_commands(namespace or '')))
+        return {cmd.path: copy(cmd.meta) for cmd in cmds}
+
+    def command_help(self, command: str) -> str | None:
+        """获取单个命令的帮助"""
+        if cmd := self.get_command(command):
+            return cmd.get_help()
+
+    def record(self, token: int, result: Arparma):
+        """记录某个命令的 `token`"""
+        self.__record[token] = result
+
+    def get_record(self, token: int) -> Arparma | None:
+        """获取某个 `token` 对应的 `Arparma` 对象"""
+        if token in self.__record:
+            return self.__record[token]
+
+    def get_token(self, result: Arparma) -> int:
+        """获取某个命令的 `token`"""
+        return next((token for token, res in self.__record.items() if res == result), 0)
+
+    def get_result(self, command: Alconna) -> list[Arparma]:
+        """获取某个命令的所有 `Arparma` 对象"""
+        return [v for v in self.__record.values() if v.source == command.path]
+
+    @property
+    def recent_message(self) -> DataCollection[str | Any] | None:
+        """获取最近一次使用的命令"""
+        if rct := self.__record.peek_first_item():
+            return rct[1].origin  # type: ignore
+
+    @property
+    def last_using(self):
+        """获取最近一次使用的 `Alconna` 对象"""
+        if rct := self.__record.peek_first_item():
+            return rct[1].source  # type: ignore
+
+    @property
+    def records(self) -> LRU[int, Arparma]:
+        """获取当前记录"""
+        return self.__record
+
+    def reuse(self, index: int = -1):
+        """获取当前记录中的某个值"""
+        key = self.__record.keys()[index]
+        return self.__record[key]
+
+    def set_record_size(self, size: int):
+        """设置记录的最大长度"""
+        self.__record.set_size(size)
+
+    def __repr__(self):
+        return (
+            f"Current: {hex(id(self))} in {datetime.now().strftime('%Y/%m/%d %H:%M:%S')}\n" +
+            "Commands:\n" +
+            f"[{', '.join([cmd.path for cmd in self.get_commands()])}]" +
+            "\nShortcuts:\n" +
+            "\n".join([f" {k} => {v}" for k, v in self.__shortcuts.items()]) +
+            "\nRecords:\n" +
+            "\n".join([f" [{k}]: {v[1].origin}" for k, v in enumerate(self.__record.items()[:20])]) +
+            "\nDisabled Commands:\n" +
+            f"[{', '.join(map(lambda x: x.path, self.__abandons))}]"
+        )
+
+
+command_manager = CommandManager()
+__all__ = ["ShortcutArgs", "command_manager"]
```

### Comparing `arclet_alconna-1.8.8/src/arclet/alconna/model.pyi` & `arclet_alconna-2.0.0a1/src/arclet/alconna/model.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,57 @@
-from __future__ import annotations
-
-from typing import Any
-
-from nepattern import BasePattern
-
-class Sentence:
-    """句段
-
-    句段由 `Analyser` 编译而来, 代表选项或者子命令的需求前缀。
-
-    Attributes:
-        name (str): 句段名称
-    """
-
-    name: str
-    def __init__(self, name: str) -> None: ...
-
-class OptionResult:
-    """选项解析结果
-
-    Attributes:
-        value (Any): 选项值
-        args (dict[str, Any]): 选项参数解析结果
-    """
-
-    value: Any
-    args: dict[str, Any]
-    def __init__(self, value: Any = ..., args: dict[str, Any] | None = ...) -> None: ...
-
-class SubcommandResult:
-    """子命令解析结果
-
-    Attributes:
-        value (Any): 子命令值
-        args (dict[str, Any]): 子命令参数解析结果
-        options (dict[str, OptionResult]): 子命令的子选项解析结果
-        subcommands (dict[str, SubcommandResult]): 子命令的子子命令解析结果
-    """
-
-    value: Any
-    args: dict[str, Any]
-    options: dict[str, OptionResult]
-    subcommands: dict[str, SubcommandResult]
-    def __init__(
-        self,
-        value: Any = ...,
-        args: dict[str, Any] | None = ...,
-        options: dict[str, OptionResult] | None = ...,
-        subcommands: dict[str, SubcommandResult] | None = ...,
-    ) -> None: ...
-
-class HeadResult:
-    """命令头解析结果
-
-    Attributes:
-        origin (Any): 命令头原始值
-        result (Any): 命令头解析结果
-        matched (bool): 命令头是否匹配
-        groups (dict[str, Any]): 命令头匹配组
-    """
-
-    origin: Any
-    result: Any
-    matched: bool
-    groups: dict[str, Any]
-    def __init__(
-        self,
-        origin: Any = ...,
-        result: Any = ...,
-        matched: bool = ...,
-        groups: dict[str, str] | None = ...,
-        fixes: dict[str, BasePattern] | None = ...,
-    ) -> None: ...
+from __future__ import annotations
+from typing import Any
+from nepattern import BasePattern
+
+class OptionResult:
+    """选项解析结果
+
+    Attributes:
+        value (Any): 选项值
+        args (dict[str, Any]): 选项参数解析结果
+    """
+    value: Any
+    args: dict[str, Any]
+    def __init__(self, value: Any = ..., args: dict[str, Any] | None = ...) -> None: ...
+
+class SubcommandResult:
+    """子命令解析结果
+
+    Attributes:
+        value (Any): 子命令值
+        args (dict[str, Any]): 子命令参数解析结果
+        options (dict[str, OptionResult]): 子命令的子选项解析结果
+        subcommands (dict[str, SubcommandResult]): 子命令的子子命令解析结果
+    """
+    value: Any
+    args: dict[str, Any]
+    options: dict[str, OptionResult]
+    subcommands: dict[str, SubcommandResult]
+    def __init__(
+        self,
+        value: Any = ...,
+        args: dict[str, Any] | None = ...,
+        options: dict[str, OptionResult] | None = ...,
+        subcommands: dict[str, SubcommandResult] | None = ...
+    ) -> None: ...
+
+class HeadResult:
+    """命令头解析结果
+
+    Attributes:
+        origin (Any): 命令头原始值
+        result (Any): 命令头解析结果
+        matched (bool): 命令头是否匹配
+        groups (dict[str, Any]): 命令头匹配组
+    """
+    origin: Any
+    result: Any
+    matched: bool
+    groups: dict[str, Any]
+    def __init__(
+        self,
+        origin: Any = ...,
+        result: Any = ...,
+        matched: bool = ...,
+        groups: dict[str, str] | None = ...,
+        fixes: dict[str, BasePattern] | None = ...
+    ) -> None: ...
```

### Comparing `arclet_alconna-1.8.8/tests/analyser_test.py` & `arclet_alconna-2.0.0a1/tests/analyser_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,102 +1,108 @@
-from dataclasses import dataclass, field
-from typing import Any, Union
-
-from nepattern import BasePattern, MatchMode
-
-from arclet.alconna import Alconna, Args, Option
-from arclet.alconna.argv import argv_config
-
-
-@dataclass
-class Segment:
-    type: str
-    data: dict = field(default_factory=dict)
-
-    def __str__(self):
-        data = self.data.copy()
-        if self.type == "text":
-            return data.get("text", "")
-        return f"[{self.type}:{self.data}]"
-
-    @staticmethod
-    def text(content: str):
-        return Segment("text", {"text": content})
-
-    @staticmethod
-    def face(id_: int, content: str = ""):
-        return Segment("face", {"id": id_, "content": content})
-
-    @staticmethod
-    def at(user_id: Union[int, str]):
-        return Segment("at", {"qq": str(user_id)})
-
-
-def gen_unit(type_: str):
-    return BasePattern(
-        mode=MatchMode.VALUE_OPERATE, origin=Segment, converter=lambda _, seg: seg if seg.type == type_ else None, alias=type_,
-    )
-
-
-Face = gen_unit("face")
-At = gen_unit("at")
-
-
-def test_filter_out():
-    argv_config(filter_out=[int])
-    ana = Alconna("ana", Args["foo", str])
-    assert ana.parse(["ana", 123, "bar"]).matched is True
-    assert ana.parse("ana bar").matched is True
-    argv_config(filter_out=[])
-    ana_1 = Alconna("ana", Args["foo", str])
-    assert ana_1.parse(["ana", 123, "bar"]).matched is False
-
-
-def test_preprocessor():
-    argv_config(preprocessors={list: len})
-    ana1 = Alconna("ana1", Args["bar", int])
-    assert ana1.parse(["ana1", [1, 2, 3]]).matched is True
-    assert ana1.parse(["ana1", [1, 2, 3]]).bar == 3
-    argv_config(preprocessors={})
-    ana1_1 = Alconna("ana1", Args["bar", int])
-    assert ana1_1.parse(["ana1", [1, 2, 3]]).matched is False
-
-
-def test_with_set_unit():
-    argv_config(preprocessors={Segment: lambda x: str(x) if x.type == "text" else None})
-
-    ana2 = Alconna("ana2", Args["foo", At]["bar", Face])
-    res = ana2.parse([Segment.text("ana2"), Segment.at(123456), Segment.face(103)])
-    assert res.matched is True
-    assert res.foo.data["qq"] == "123456"
-    assert not ana2.parse([Segment.text("ana2"), Segment.face(103), Segment.at(123456)]).matched
-    argv_config()
-
-
-def test_unhashable_unit():
-    argv_config(preprocessors={Segment: lambda x: str(x) if x.type == "text" else None})
-
-    ana3 = Alconna("ana3", Args["foo", At])
-    print(ana3.parse(["ana3", Segment.at(123)]))
-    print(ana3.parse(["ana3", Segment.face(123)]))
-
-    ana3_1 = Alconna("ana3_1", Option("--foo", Args["bar", int]))
-    print(ana3_1.parse(["ana3_1 --foo 123"]))
-    print(ana3_1.parse(["ana3_1", Segment.face(123)]))
-    print(ana3_1.parse(["ana3_1", "--foo", "--comp", Segment.at(123)]))
-    print(ana3_1.parse(["ana3_1", "--comp", Segment.at(123)]))
-
-
-def test_checker():
-    argv_config(checker=lambda x: isinstance(x, list))
-    ana4 = Alconna("ana4", Args["foo", int])
-    print(ana4.parse(["ana4", "123"]))
-    try:
-        print(ana4.parse("ana4 123"))
-    except TypeError as e:
-        print(e)
-
-
-if __name__ == "__main__":
-    import pytest
-
-    pytest.main([__file__, "-vs"])
+from dataclasses import dataclass, field
+from typing import Any, Union
+
+from arclet.alconna import Alconna, Args, Option
+from arclet.alconna.argv import argv_config
+from nepattern import BasePattern, MatchMode
+
+
+@dataclass
+class Segment:
+    type: str
+    data: dict = field(default_factory=dict)
+
+    def __str__(self):
+        data = self.data.copy()
+        if self.type == "text":
+            return data.get("text", "")
+        return f"[{self.type}:{self.data}]"
+
+    @staticmethod
+    def text(content: str):
+        return Segment("text", {"text": content})
+
+    @staticmethod
+    def face(id_: int, content: str = ''):
+        return Segment("face", {"id": id_, "content": content})
+
+    @staticmethod
+    def at(user_id: Union[int, str]):
+        return Segment("at", {"qq": str(user_id)})
+
+
+def gen_unit(type_: str):
+    return BasePattern(
+        type_, MatchMode.TYPE_CONVERT, Any,
+        lambda _, seg: seg if seg.type == type_ else None,
+        type_, accepts=[Segment]
+    )
+
+
+Face = gen_unit("face")
+At = gen_unit("at")
+
+
+def test_filter_out():
+    argv_config(filter_out=[int])
+    ana = Alconna("ana", Args["foo", str])
+    assert ana.parse(["ana", 123, "bar"]).matched is True
+    assert ana.parse("ana bar").matched is True
+    argv_config(filter_out=[])
+    ana_1 = Alconna("ana", Args["foo", str])
+    assert ana_1.parse(["ana", 123, "bar"]).matched is False
+
+
+def test_preprocessor():
+    argv_config(preprocessors={float: int})
+    ana1 = Alconna("ana1", Args["bar", int])
+    assert ana1.parse(["ana1", 123.06]).matched is True
+    assert ana1.parse(["ana1", 123.06]).bar == 123
+    argv_config(preprocessors={})
+    ana1_1 = Alconna("ana1", Args["bar", int])
+    assert ana1_1.parse(["ana1", 123.06]).matched is False
+
+
+def test_with_set_unit():
+    argv_config(
+        preprocessors={Segment: lambda x: str(x) if x.type == "text" else None}
+    )
+
+    ana2 = Alconna("ana2", Args["foo", At]["bar", Face])
+    res = ana2.parse([Segment.text("ana2"), Segment.at(123456), Segment.face(103)])
+    assert res.matched is True
+    assert res.foo.data['qq'] == '123456'
+    assert not ana2.parse([Segment.text("ana2"), Segment.face(103), Segment.at(123456)]).matched
+    argv_config()
+
+
+def test_unhashable_unit():
+    argv_config(
+        preprocessors={Segment: lambda x: str(x) if x.type == "text" else None}
+    )
+
+    ana3 = Alconna("ana3", Args["foo", At])
+    print(ana3.parse(["ana3", Segment.at(123)]))
+    print(ana3.parse(["ana3", Segment.face(123)]))
+
+    ana3_1 = Alconna("ana3_1", Option("--foo", Args["bar", int]))
+    print(ana3_1.parse(["ana3_1 --foo 123"]))
+    print(ana3_1.parse(["ana3_1", Segment.face(123)]))
+    print(ana3_1.parse(["ana3_1", "--foo", "--comp", Segment.at(123)]))
+    print(ana3_1.parse(["ana3_1", "--comp", Segment.at(123)]))
+
+
+def test_checker():
+    argv_config(
+        checker=lambda x: isinstance(x, list)
+    )
+    ana4 = Alconna("ana4", Args["foo", int])
+    print(ana4.parse(["ana4", "123"]))
+    try:
+        print(ana4.parse("ana4 123"))
+    except TypeError as e:
+        print(e)
+
+
+if __name__ == '__main__':
+    import pytest
+    pytest.main([__file__, "-vs"])
```

### Comparing `arclet_alconna-1.8.8/tests/args_test.py` & `arclet_alconna-2.0.0a1/tests/args_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,268 +1,261 @@
-from typing import Union
-
-from nepattern import BasePattern, Bind, MatchMode
-
-from arclet.alconna import ArgFlag, Args, KeyWordVar, Kw, Nargs
-from devtool import analyse_args
-
-
-def test_magic_create():
-    arg1 = Args["round", float]["test", bool]["aaa", str]
-    assert len(arg1) == 3
-    arg1 <<= Args["perm", str, ...] + ["month", int]
-    assert len(arg1) == 5
-    arg11: Args = Args["baz", int]
-    arg11.add("foo", value=int, default=1)
-    assert len(arg11) == 2
-
-
-def test_type_convert():
-    arg2 = Args["round", float]["test", bool]
-    assert analyse_args(arg2, ["1.2 False"]) != {"round": "1.2", "test": "False"}
-    assert analyse_args(arg2, ["1.2 False"]) == {"round": 1.2, "test": False}
-    assert analyse_args(arg2, ["a False"], raise_exception=False) != {
-        "round": "a",
-        "test": False,
-    }
-
-
-def test_regex():
-    arg3 = Args["foo", "re:abc[0-9]{3}"]
-    assert analyse_args(arg3, ["abc123"]) == {"foo": "abc123"}
-    assert analyse_args(arg3, ["abc"], raise_exception=False) != {"foo": "abc"}
-
-
-def test_string():
-    arg4 = Args["foo"]["bar"]
-    assert analyse_args(arg4, ["foo bar"]) == {"foo": "foo", "bar": "bar"}
-
-
-def test_default():
-    arg5 = Args["foo", int]["de", bool, True]
-    assert analyse_args(arg5, ["123 False"]) == {"foo": 123, "de": False}
-    assert analyse_args(arg5, ["123"]) == {"foo": 123, "de": True}
-
-
-def test_separate():
-    arg6 = Args["foo", str]["bar", int] / ";"
-    assert analyse_args(arg6, ["abc;123"]) == {"foo": "abc", "bar": 123}
-
-
-def test_object():
-    arg7 = Args["foo", str]["bar", 123]
-    assert analyse_args(arg7, ["abc", 123]) == {"foo": "abc", "bar": 123}
-    assert analyse_args(arg7, ["abc", 124], raise_exception=False) != {
-        "foo": "abc",
-        "bar": 124,
-    }
-
-
-def test_multi():
-    arg8 = Args().add("multi", value=Nargs(str, "+"))
-    assert analyse_args(arg8, ["a b c d"]).get("multi") == ("a", "b", "c", "d")
-    assert analyse_args(arg8, [], raise_exception=False) != {"multi": ()}
-    arg8_1 = Args().add("kwargs", value=Nargs(Kw @ str, "+"))
-    assert analyse_args(arg8_1, ["a=b c=d"]).get("kwargs") == {"a": "b", "c": "d"}
-    arg8_2 = Args().add("multi", value=Nargs(int, "*"))
-    assert analyse_args(arg8_2, ["1 2 3 4"]).get("multi") == (1, 2, 3, 4)
-    assert analyse_args(arg8_2, []).get("multi") == ()
-    arg8_3 = Args().add("multi", value=Nargs(int, 3))
-    assert analyse_args(arg8_3, ["1 2 3"]).get("multi") == (1, 2, 3)
-    assert analyse_args(arg8_3, ["1 2"]).get("multi") == (1, 2)
-    assert analyse_args(arg8_3, ["1 2 3 4"]).get("multi") == (1, 2, 3)
-    arg8_4 = Args().add("multi", value=Nargs(str, "*")).add("kwargs", value=Nargs(Kw @ str, "*"))
-    assert analyse_args(arg8_4, ["1 2 3 4 a=b c=d"]).get("multi") == ("1", "2", "3", "4")
-    assert analyse_args(arg8_4, ["1 2 3 4 a=b c=d"]).get("kwargs") == {
-        "a": "b",
-        "c": "d",
-    }
-    assert analyse_args(arg8_4, ["1 2 3 4"]).get("multi") == ("1", "2", "3", "4")
-    assert analyse_args(arg8_4, ["a=b c=d"]).get("kwargs") == {"a": "b", "c": "d"}
-
-
-def test_anti():
-    arg9 = Args().add("anti", value=r"re:(.+?)/(.+?)\.py", flags=[ArgFlag.ANTI])
-    assert analyse_args(arg9, ["a/b.mp3"]) == {"anti": "a/b.mp3"}
-    assert analyse_args(arg9, ["a/b.py"], raise_exception=False) != {"anti": "a/b.py"}
-
-
-def test_choice():
-    arg10 = Args["choice", ("a", "b", "c")]
-    assert analyse_args(arg10, ["a"]) == {"choice": "a"}
-    assert analyse_args(arg10, ["d"], raise_exception=False) != {"choice": "d"}
-    arg10_1 = Args["mapping", {"a": 1, "b": 2, "c": 3}]
-    assert analyse_args(arg10_1, ["a"]) == {"mapping": 1}
-    assert analyse_args(arg10_1, ["d"], raise_exception=False) != {"mapping": "d"}
-
-
-def test_union():
-    arg11 = Args["bar", Union[int, float]]
-    assert analyse_args(arg11, ["1.2"]) == {"bar": 1.2}
-    assert analyse_args(arg11, ["1"]) == {"bar": 1}
-    assert analyse_args(arg11, ["abc"], raise_exception=False) != {"bar": "abc"}
-    arg11_1 = Args["bar", [int, float, "abc"]]
-    assert analyse_args(arg11_1, ["1.2"]) == analyse_args(arg11, ["1.2"])
-    assert analyse_args(arg11_1, ["abc"]) == {"bar": "abc"}
-    assert analyse_args(arg11_1, ["cba"], raise_exception=False) != {"bar": "cba"}
-
-
-def test_optional():
-    arg13 = Args["foo", str].add("bar", value=int, flags=["?"])
-    assert analyse_args(arg13, ["abc 123"]) == {"foo": "abc", "bar": 123}
-    assert analyse_args(arg13, ["abc"]) == {"foo": "abc"}
-    arg13_1 = Args["foo", str]["bar?", int]
-    assert analyse_args(arg13_1, ["abc 123"]) == {"foo": "abc", "bar": 123}
-    assert analyse_args(arg13_1, ["abc"]) == {"foo": "abc"}
-    arg13_2 = Args["foo", str]["bar;?", int]
-    assert analyse_args(arg13_2, ["abc 123"]) == {"foo": "abc", "bar": 123}
-    assert analyse_args(arg13_2, ["abc"]) == {"foo": "abc"}
-
-
-def test_kwonly():
-    arg14 = Args["foo", str].add("bar", value=Kw[int])
-    assert analyse_args(arg14, ["abc bar=123"]) == {
-        "foo": "abc",
-        "bar": 123,
-    }
-    assert analyse_args(arg14, ["abc 123"], raise_exception=False) != {
-        "foo": "abc",
-        "bar": 123,
-    }
-    arg14_1 = Args["width;?", Kw[int], 1280]["height?", Kw[int], 960]
-    assert analyse_args(arg14_1, ["--width=960 --height=960"]) == {
-        "width": 960,
-        "height": 960,
-    }
-    assert analyse_args(arg14_1, ["--height=480 --width=960"]) == {
-        "width": 960,
-        "height": 480,
-    }
-    arg14_2 = Args["foo", str]["bar", KeyWordVar(int, " ")]["baz", KeyWordVar(bool, ":")]
-    assert analyse_args(arg14_2, ["abc -bar 123 baz:false"]) == {
-        "bar": 123,
-        "baz": False,
-        "foo": "abc",
-    }
-    assert analyse_args(arg14_2, ["abc baz:false -bar 456"]) == {
-        "bar": 456,
-        "baz": False,
-        "foo": "abc",
-    }
-
-
-def test_pattern():
-    test_type = BasePattern("(.+?).py", MatchMode.REGEX_CONVERT, list, lambda _, x: x[1].split("/"), "test")
-    arg15 = Args().add("bar", value=test_type)
-    assert analyse_args(arg15, ["abc.py"]) == {"bar": ["abc"]}
-    assert analyse_args(arg15, ["abc/def.py"]) == {"bar": ["abc", "def"]}
-    assert analyse_args(arg15, ["abc/def.mp3"], raise_exception=False) != {"bar": ["abc", "def"]}
-
-
-def test_callable():
-    def test(
-        a: int,
-        b: bool,
-        *args: str,
-        c: float = 1.0,
-        d: int = 1,
-        e: bool = False,
-        **kwargs: str,
-    ):
-        ...
-
-    arg16, _ = Args.from_callable(test)
-    assert len(arg16.argument) == 7
-    assert analyse_args(arg16, ["1 True 2 3 4 c=5.0 d=6 -no-e f=g h=i"]) == {
-        "a": 1,
-        "args": ("2", "3", "4"),
-        "b": True,
-        "c": 5.0,
-        "d": 6,
-        "e": False,
-        "kwargs": {"f": "g", "h": "i"},
-    }
-    assert analyse_args(arg16, ["1 True 2 3 4 -no-e c=7.2 f=x h=y"]) == {
-        "a": 1,
-        "args": ("2", "3", "4"),
-        "b": True,
-        "c": 7.2,
-        "d": 1,
-        "e": False,
-        "kwargs": {"f": "x", "h": "y"},
-    }
-
-
-def test_func_anno():
-    from datetime import datetime
-
-    def test(time: Union[int, str]) -> datetime:
-        return datetime.fromtimestamp(time) if isinstance(time, int) else datetime.fromisoformat(time)
-
-    arg17 = Args["time", test]
-    assert analyse_args(arg17, ["1145-05-14"]) == {"time": datetime.fromisoformat("1145-05-14")}
-
-
-def test_annotated():
-    from typing_extensions import Annotated
-
-    arg18 = Args["foo", Annotated[int, lambda x: x > 0]]["bar", Bind[int, lambda x: x < 0]]
-    assert analyse_args(arg18, ["123 -123"]) == {"foo": 123, "bar": -123}
-    assert analyse_args(arg18, ["0 0"], raise_exception=False) != {"foo": 0, "bar": 0}
-
-
-def test_unpack():
-    from dataclasses import dataclass, field
-
-    from arclet.alconna.typing import UnpackVar
-
-    @dataclass
-    class People:
-        name: str
-        age: int = field(default=16)
-
-    arg19 = Args["people", UnpackVar(People)]
-    assert analyse_args(arg19, ["alice", 16]) == {"people": People("alice", 16)}
-    assert analyse_args(arg19, ["bob"]) == {"people": People("bob", 16)}
-    arg19_1 = Args["people", UnpackVar(People, kw_only=True)].separate("&")
-    assert analyse_args(arg19_1, ["name=alice&age=16"]) == {"people": People("alice", 16)}
-
-
-def test_multi_multi():
-    from arclet.alconna.typing import MultiVar
-
-    arg20 = Args["foo", MultiVar(str)]["bar", MultiVar(int)]
-    assert analyse_args(arg20, ["a b -- 1 2"]) == {"foo": ("a", "b"), "bar": (1, 2)}
-
-    arg20_1 = Args["foo", MultiVar(int)]["bar", MultiVar(str)]
-    assert analyse_args(arg20_1, ["1 2 -- a b"]) == {"foo": (1, 2), "bar": ("a", "b")}
-    assert analyse_args(arg20_1, ["1 2 a b"]) == {"foo": (1, 2), "bar": ("a", "b")}
-
-
-def test_contextval():
-    arg21 = Args["foo", str]
-    assert analyse_args(arg21, ["$(bar)"], context_style="parentheses", bar="baz") == {"foo": "baz"}
-    assert analyse_args(arg21, ["{bar}"], context_style="parentheses", raise_exception=False, bar="baz") != {"foo": "baz"}
-
-    assert analyse_args(arg21, ["{bar}"], context_style="bracket", bar="baz") == {"foo": "baz"}
-    assert analyse_args(arg21, ["$(bar)"], context_style="bracket", raise_exception=False, bar="baz") != {"foo": "baz"}
-
-    class A:
-        class B:
-            c = "baz"
-            d = {"e": "baz"}
-
-        b = B()
-
-    assert analyse_args(arg21, ["$(a.b.c)"], context_style="parentheses", a=A()) == {"foo": "baz"}
-    assert analyse_args(arg21, ["$(a.b.d.get(e))"], context_style="parentheses", a=A()) == {"foo": "baz"}
-
-    arg21_1 = Args["foo", int]
-    assert analyse_args(arg21_1, ["$(bar)"], context_style="parentheses", bar=123) == {"foo": 123}
-    assert analyse_args(arg21_1, ["$(bar)"], context_style="parentheses", bar="123") == {"foo": 123}
-    assert analyse_args(arg21_1, ["$(bar)"], context_style="parentheses", raise_exception=False, bar="baz") != {"foo": 123}
-
-
-if __name__ == "__main__":
-    import pytest
-
-    pytest.main([__file__, "-vs"])
+from typing import Union
+
+from arclet.alconna import ArgFlag, Args, KeyWordVar, Kw, Nargs
+from devtool import analyse_args
+from nepattern import BasePattern, Bind, MatchMode
+
+
+def test_kwargs_create():
+    arg = Args(pak=str, upgrade=str)
+    assert arg == Args.pak[str]["upgrade", str]
+    assert analyse_args(arg, ["arclet-alconna bar"]) == {
+        "pak": "arclet-alconna",
+        "upgrade": "bar",
+    }
+
+
+def test_magic_create():
+    arg1 = Args.round[float]["test", bool]["aaa", str]
+    assert len(arg1) == 3
+    arg1 = arg1 << Args.perm[str, ...] + ["month", int]
+    assert len(arg1) == 5
+    arg11: Args = Args.baz[int]
+    arg11.add("foo", value=int, default=1)
+    assert len(arg11) == 2
+
+
+def test_type_convert():
+    arg2 = Args.round[float]["test", bool]
+    assert analyse_args(arg2, ["1.2 False"]) != {"round": "1.2", "test": "False"}
+    assert analyse_args(arg2, ["1.2 False"]) == {"round": 1.2, "test": False}
+    assert analyse_args(arg2, ["a False"], raise_exception=False) != {
+        "round": "a",
+        "test": False,
+    }
+
+
+def test_regex():
+    arg3 = Args.foo["re:abc[0-9]{3}"]
+    assert analyse_args(arg3, ["abc123"]) == {"foo": "abc123"}
+    assert analyse_args(arg3, ["abc"], raise_exception=False) != {"foo": "abc"}
+
+
+def test_string():
+    arg4 = Args["foo"]["bar"]
+    assert analyse_args(arg4, ["foo bar"]) == {"foo": "foo", "bar": "bar"}
+
+
+def test_default():
+    arg5 = Args.foo[int]["de", bool, True]
+    assert analyse_args(arg5, ["123 False"]) == {"foo": 123, "de": False}
+    assert analyse_args(arg5, ["123"]) == {"foo": 123, "de": True}
+
+
+def test_separate():
+    arg6 = Args.foo[str]["bar", int] / ";"
+    assert analyse_args(arg6, ["abc;123"]) == {"foo": "abc", "bar": 123}
+
+
+def test_object():
+    arg7 = Args.foo[str]["bar", 123]
+    assert analyse_args(arg7, ["abc", 123]) == {"foo": "abc", "bar": 123}
+    assert analyse_args(arg7, ["abc", 124], raise_exception=False) != {
+        "foo": "abc",
+        "bar": 124,
+    }
+
+
+def test_multi():
+    arg8 = Args().add("multi", value=Nargs(str, "+"))
+    assert analyse_args(arg8, ["a b c d"]).get("multi") == ("a", "b", "c", "d")
+    assert analyse_args(arg8, [], raise_exception=False) != {"multi": ()}
+    arg8_1 = Args().add("kwargs", value=Nargs(Kw @ str, "+"))
+    assert analyse_args(arg8_1, ["a=b c=d"]).get("kwargs") == {"a": "b", "c": "d"}
+    arg8_2 = Args().add("multi", value=Nargs(int, "*"))
+    assert analyse_args(arg8_2, ["1 2 3 4"]).get("multi") == (1, 2, 3, 4)
+    assert analyse_args(arg8_2, []).get("multi") == ()
+    arg8_3 = Args().add("multi", value=Nargs(int, 3))
+    assert analyse_args(arg8_3, ["1 2 3"]).get("multi") == (1, 2, 3)
+    assert analyse_args(arg8_3, ["1 2"]).get("multi") == (1, 2)
+    assert analyse_args(arg8_3, ["1 2 3 4"]).get("multi") == (1, 2, 3)
+    arg8_4 = (
+        Args()
+        .add("multi", value=Nargs(str, "*"))
+        .add("kwargs", value=Nargs(Kw @ str, "*"))
+    )
+    assert analyse_args(arg8_4, ["1 2 3 4 a=b c=d"]).get("multi") == ('1', '2', '3', '4')
+    assert analyse_args(arg8_4, ["1 2 3 4 a=b c=d"]).get("kwargs") == {
+        "a": "b",
+        "c": "d",
+    }
+    assert analyse_args(arg8_4, ["1 2 3 4"]).get("multi") == ('1', '2', '3', '4')
+    assert analyse_args(arg8_4, ["a=b c=d"]).get("kwargs") == {"a": "b", "c": "d"}
+
+
+def test_anti():
+    arg9 = Args().add("anti", value=r"re:(.+?)/(.+?)\.py", flags=[ArgFlag.ANTI])
+    assert analyse_args(arg9, ["a/b.mp3"]) == {"anti": "a/b.mp3"}
+    assert analyse_args(arg9, ["a/b.py"], raise_exception=False) != {"anti": "a/b.py"}
+
+
+def test_choice():
+    arg10 = Args.choice[("a", "b", "c")]
+    assert analyse_args(arg10, ["a"]) == {"choice": "a"}
+    assert analyse_args(arg10, ["d"], raise_exception=False) != {"choice": "d"}
+    arg10_1 = Args.mapping[{"a": 1, "b": 2, "c": 3}]
+    assert analyse_args(arg10_1, ["a"]) == {"mapping": 1}
+    assert analyse_args(arg10_1, ["d"], raise_exception=False) != {"mapping": "d"}
+
+
+def test_union():
+    arg11 = Args.bar[Union[int, float]]
+    assert analyse_args(arg11, ["1.2"]) == {"bar": 1.2}
+    assert analyse_args(arg11, ["1"]) == {"bar": 1}
+    assert analyse_args(arg11, ["abc"], raise_exception=False) != {"bar": "abc"}
+    arg11_1 = Args.bar[[int, float, "abc"]]
+    assert analyse_args(arg11_1, ["1.2"]) == analyse_args(arg11, ["1.2"])
+    assert analyse_args(arg11_1, ["abc"]) == {"bar": "abc"}
+    assert analyse_args(arg11_1, ["cba"], raise_exception=False) != {"bar": "cba"}
+
+def test_optional():
+    arg13 = Args.foo[str].add("bar", value=int, flags="?")
+    assert analyse_args(arg13, ["abc 123"]) == {"foo": "abc", "bar": 123}
+    assert analyse_args(arg13, ["abc"]) == {"foo": "abc"}
+    arg13_1 = Args.foo[str]["bar?", int]
+    assert analyse_args(arg13_1, ["abc 123"]) == {"foo": "abc", "bar": 123}
+    assert analyse_args(arg13_1, ["abc"]) == {"foo": "abc"}
+    arg13_2 = Args.foo[str]["bar;?", int]
+    assert analyse_args(arg13_2, ["abc 123"]) == {"foo": "abc", "bar": 123}
+    assert analyse_args(arg13_2, ["abc"]) == {"foo": "abc"}
+
+
+def test_kwonly():
+    arg14 = Args.foo[str].add("bar", value=Kw[int])
+    assert analyse_args(arg14, ["abc bar=123"]) == {
+        "foo": "abc",
+        "bar": 123,
+    }
+    assert analyse_args(arg14, ["abc 123"], raise_exception=False) != {
+        "foo": "abc",
+        "bar": 123,
+    }
+    arg14_1 = Args["width;?", Kw[int], 1280]["height?", Kw[int], 960]
+    assert analyse_args(arg14_1, ["--width=960 --height=960"]) == {
+        "width": 960,
+        "height": 960,
+    }
+    assert analyse_args(arg14_1, ["--height=480 --width=960"]) == {
+        "width": 960,
+        "height": 480,
+    }
+    arg14_2 = Args.foo[str]["bar", KeyWordVar(int, " ")]["baz", KeyWordVar(bool, ":")]
+    assert analyse_args(arg14_2, ["abc -bar 123 baz:false"]) == {
+        "bar": 123,
+        "baz": False,
+        "foo": "abc",
+    }
+    assert analyse_args(arg14_2, ["abc baz:false -bar 456"]) == {
+        "bar": 456,
+        "baz": False,
+        "foo": "abc",
+    }
+
+
+def test_pattern():
+    test_type = BasePattern(
+        "(.+?).py", MatchMode.REGEX_CONVERT, list, lambda _, x: x[1].split("/"), "test"
+    )
+    arg15 = Args().add("bar", value=test_type)
+    assert analyse_args(arg15, ["abc.py"]) == {"bar": ["abc"]}
+    assert analyse_args(arg15, ["abc/def.py"]) == {"bar": ["abc", "def"]}
+    assert analyse_args(arg15, ["abc/def.mp3"], raise_exception=False) != {
+        "bar": ["abc", "def"]
+    }
+
+
+def test_callable():
+    def test(
+        a: int,
+        b: bool,
+        *args: str,
+        c: float = 1.0,
+        d: int = 1,
+        e: bool = False,
+        **kwargs: str,
+    ):
+        ...
+
+    arg16, _ = Args.from_callable(test)
+    assert len(arg16.argument) == 7
+    assert analyse_args(arg16, ["1 True 2 3 4 c=5.0 d=6 -no-e f=g h=i"]) == {
+        'a': 1,
+        'args': ('2', '3', '4'),
+        'b': True,
+        'c': 5.0,
+        'd': 6,
+        'e': False,
+        'kwargs': {'f': 'g', 'h': 'i'}
+    }
+    assert analyse_args(arg16, ["1 True 2 3 4 -no-e c=7.2 f=x h=y"]) == {
+        'a': 1,
+        'args': ('2', '3', '4'),
+        'b': True,
+        'c': 7.2,
+        'd': 1,
+        'e': False,
+        'kwargs': {'f': 'x', 'h': 'y'}
+    }
+
+
+def test_func_anno():
+    from datetime import datetime
+
+    def test(time: Union[int, str]) -> datetime:
+        return (
+            datetime.fromtimestamp(time)
+            if isinstance(time, int)
+            else datetime.fromisoformat(time)
+        )
+
+    arg17 = Args["time", test]
+    assert analyse_args(arg17, ["1145-05-14"]) == {
+        "time": datetime.fromisoformat("1145-05-14")
+    }
+
+
+def test_annotated():
+    from typing_extensions import Annotated
+
+    arg18 = Args["foo", Annotated[int, lambda x: x > 0]][
+        "bar", Bind[int, lambda x: x < 0]
+    ]
+    assert analyse_args(arg18, ["123 -123"]) == {"foo": 123, "bar": -123}
+    assert analyse_args(arg18, ["0 0"], raise_exception=False) != {"foo": 0, "bar": 0}
+
+
+def test_unpack():
+    from dataclasses import dataclass, field
+    from arclet.alconna.typing import UnpackVar
+
+    @dataclass
+    class People:
+        name: str
+        age: int = field(default=16)
+
+    arg19 = Args["people", UnpackVar(People)]
+    assert analyse_args(
+        arg19, ["alice", 16]
+    ) == {"people": People("alice", 16)}
+    assert analyse_args(
+        arg19, ["bob"]
+    ) == {"people": People("bob", 16)}
+    arg19_1 = Args["people", UnpackVar(People, kw_only=True)].separate("&")
+    assert analyse_args(
+        arg19_1, ["name=alice&age=16"]
+    ) == {"people": People("alice", 16)}
+
+
+if __name__ == "__main__":
+    import pytest
+
+    pytest.main([__file__, "-vs"])
```

### Comparing `arclet_alconna-1.8.8/tests/base_test.py` & `arclet_alconna-2.0.0a1/tests/base_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from arclet.alconna.args import Arg, Args
-from arclet.alconna.base import CommandNode, Option, Subcommand
-from arclet.alconna.model import OptionResult, SubcommandResult
-from devtool import analyse_option, analyse_subcommand
-
-
-def test_node_create():
-    node = CommandNode("foo", Args["bar", int], dest="test")
-    assert node.name == "foo"
-    assert node.dest != "foo"
-    assert node.nargs == 1
-
-
-def test_single_args():
-    node1 = CommandNode("foo", Arg("bar", int))
-    assert node1.args == Args["bar", int]
-
-
-def test_node_requires():
-    node2 = CommandNode("foo", requires=["baz", "qux"])
-    assert node2.dest == "baz_qux_foo"
-    node2_1 = CommandNode("baz qux foo")
-    assert node2_1.name == "foo"
-    assert node2_1.requires == ["baz", "qux"]
-
-
-def test_option_aliases():
-    opt = Option("test|T|t")
-    assert opt.aliases == {"test", "T", "t"}
-    opt_1 = Option("test", alias=["T", "t"])
-    assert opt_1.aliases == {"test", "T", "t"}
-    assert opt == opt_1
-    assert opt == Option("T|t|test")
-
-
-def test_option_requires():
-    opt1 = Option("foo bar test|T|t")
-    assert opt1.aliases == {"test", "T", "t"}
-    assert opt1.requires == ["foo", "bar"]
-    opt1_1 = Option("foo bar test| T | t")
-    assert opt1_1.aliases != {"test", "T", "t"}
-
-
-def test_separator():
-    opt2 = Option("foo", Args["bar", int], separators="|")
-    assert analyse_option(opt2, "foo|123") == OptionResult(None, {"bar": 123})
-    opt2_1 = Option("foo", Args["bar", int]).separate("|")
-    assert opt2 == opt2_1
-
-
-def test_subcommand():
-    sub = Subcommand("test", Option("foo"), Option("bar"))
-    assert len(sub.options) == 2
-    assert analyse_subcommand(sub, "test foo") == SubcommandResult(None, {}, {"foo": OptionResult()})
-
-
-def test_compact():
-    opt3 = Option("-Foo", Args["bar", int], compact=True)
-    assert analyse_option(opt3, "-Foo123") == OptionResult(None, {"bar": 123})
-
-
-def test_add():
-    assert (Option("abcd") + Args["foo", int]).nargs == 1
-    assert len((Option("foo") + Option("bar") + "baz").options) == 2
-
-
-if __name__ == "__main__":
-    import pytest
-
-    pytest.main([__file__, "-vs"])
+from arclet.alconna.base import Option, Subcommand, CommandNode
+from arclet.alconna.args import Args, Arg
+from arclet.alconna.model import OptionResult, SubcommandResult
+from devtool import analyse_option, analyse_subcommand
+
+
+def test_node_create():
+    node = CommandNode("foo", Args.bar[int], dest="test")
+    assert node.name == "foo"
+    assert node.dest != "foo"
+    assert node.nargs == 1
+
+
+def test_single_args():
+    node1 = CommandNode("foo", Arg("bar", int))
+    assert node1.args == Args.bar[int]
+
+
+def test_node_requires():
+    node2 = CommandNode("foo", requires=["baz", "qux"])
+    assert node2.dest == "baz_qux_foo"
+    node2_1 = CommandNode("baz qux foo")
+    assert node2_1.name == "foo"
+    assert node2_1.requires == ["baz", "qux"]
+
+
+def test_option_aliases():
+    opt = Option("test|T|t")
+    assert opt.aliases == {"test", "T", "t"}
+    opt_1 = Option("test", alias=["T", "t"])
+    assert opt_1.aliases == {"test", "T", "t"}
+    assert opt == opt_1
+    assert opt == Option("T|t|test")
+
+
+def test_option_requires():
+    opt1 = Option("foo bar test|T|t")
+    assert opt1.aliases == {"test", "T", "t"}
+    assert opt1.requires == ["foo", "bar"]
+    opt1_1 = Option("foo bar test| T | t")
+    assert opt1_1.aliases != {"test", "T", "t"}
+
+
+def test_separator():
+    opt2 = Option("foo", Args.bar[int], separators="|")
+    assert analyse_option(opt2, "foo|123") == OptionResult(None, {"bar": 123})
+    opt2_1 = Option("foo", Args.bar[int]).separate("|")
+    assert opt2 == opt2_1
+
+
+def test_subcommand():
+    sub = Subcommand("test", Option("foo"), Option("bar"))
+    assert len(sub.options) == 2
+    assert analyse_subcommand(sub, "test foo") == SubcommandResult(None, {}, {"foo": OptionResult()})
+
+
+def test_compact():
+    opt3 = Option("-Foo", Args.bar[int], compact=True)
+    assert analyse_option(opt3, "-Foo123") == OptionResult(None, {"bar": 123})
+
+
+def test_add():
+    assert (Option("abcd") + Args.foo[int]).nargs == 1
+    assert len((Option("foo") + Option("bar") + "baz").options) == 2
+
+
+if __name__ == "__main__":
+    import pytest
+
+    pytest.main([__file__, "-vs"])
```

### Comparing `arclet_alconna-1.8.8/tests/components_test.py` & `arclet_alconna-2.0.0a1/tests/components_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,83 @@
-from arclet.alconna import Alconna, Args, Arparma, ArparmaBehavior, Option, Subcommand
-from arclet.alconna.builtin import generate_duplication, set_default
-from arclet.alconna.duplication import Duplication
-from arclet.alconna.model import OptionResult
-from arclet.alconna.output import output_manager
-from arclet.alconna.stub import ArgsStub, OptionStub, SubcommandStub
-
-
-def test_behavior():
-    com = Alconna("comp", Args["bar", int]) + Option("foo", default=321)
-
-    class Test(ArparmaBehavior):
-        requires = [set_default(factory=lambda: OptionResult(321), path="option.baz")]
-
-        @classmethod
-        def operate(cls, interface: "Arparma"):
-            print("\ncom: ")
-            print(interface.query("options.foo.value"))
-            print(interface.query("options.baz.value"))
-            interface.behave_fail()
-
-    com.behaviors.append(Test())
-    assert com.parse("comp 123").matched is False
-
-
-def test_duplication():
-    class Demo(Duplication):
-        testArgs: ArgsStub
-        bar: OptionStub
-        sub: SubcommandStub
-
-    class Demo1(Duplication):
-        foo: int
-        bar: str
-        baz: str
-
-    com4 = Alconna(
-        "comp4",
-        Args["foo", int],
-        Option("--bar", Args["bar", str]),
-        Subcommand("sub", Option("--sub1", Args["baz", str])),
-    )
-    res = com4.parse("comp4 123 --bar abc sub --sub1 xyz")
-    assert res.matched is True
-    duplication = Demo(com4.parse("comp4 123 --bar abc sub --sub1 xyz"))
-    assert isinstance(duplication, Demo)
-    assert duplication.testArgs.available is True
-    assert duplication.testArgs.foo == 123
-    assert duplication.bar.available is True
-    assert duplication.bar.args.bar == "abc"
-    assert duplication.sub.available is True
-    assert duplication.sub.option("sub1").args.first == "xyz"
-    duplication1 = Demo1(com4.parse("comp4 123 --bar abc sub --sub1 xyz"))
-    assert isinstance(duplication1, Demo1)
-    assert isinstance(duplication1.foo, int)
-    assert isinstance(duplication1.bar, str)
-    assert isinstance(duplication1.baz, str)
-
-    com4_1 = Alconna(["!", "！"], "yiyu", Args["value;OH", str])
-    res = com4_1.parse("!yiyu")
-    dup = generate_duplication(com4_1)(res)
-    assert isinstance(dup, Duplication)
-
-
-def test_output():
-    print("")
-    output_manager.set_action(lambda x: {"bar": f"{x}!"}, "foo")
-    output_manager.set(lambda: "123", "foo")
-    assert output_manager.send("foo") == {"bar": "123!"}
-    assert output_manager.send("foo", lambda: "321") == {"bar": "321!"}
-
-    com5 = Alconna("comp5", Args["foo", int], Option("--bar", Args["bar", str]))
-    output_manager.set_action(lambda x: x, "comp5")
-    with output_manager.capture("comp5") as output:
-        com5.parse("comp5 --help")
-        assert output.get("output")
-        print("")
-        print(output.get("output"))
-    print(output.get("output"))  # capture will clear when exit context
-
-
-if __name__ == "__main__":
-    import pytest
-
-    pytest.main([__file__, "-vs"])
+from arclet.alconna import Alconna, Option, Args, Subcommand, Arparma, ArparmaBehavior
+from arclet.alconna.builtin import set_default, generate_duplication
+from arclet.alconna.duplication import Duplication
+from arclet.alconna.stub import ArgsStub, OptionStub, SubcommandStub
+from arclet.alconna.output import output_manager
+from arclet.alconna.model import OptionResult
+
+
+def test_behavior():
+    com = Alconna("comp", Args["bar", int]) + Option("foo", default=321)
+
+    class Test(ArparmaBehavior):
+        requires = [set_default(factory=lambda: OptionResult(321), path="option.baz")]
+
+        @classmethod
+        def operate(cls, interface: "Arparma"):
+            print('\ncom: ')
+            print(interface.query("options.foo.value"))
+            print(interface.query("options.baz.value"))
+            interface.behave_fail()
+
+    com.behaviors.append(Test())
+    assert com.parse("comp 123").matched is False
+
+
+def test_duplication():
+    class Demo(Duplication):
+        testArgs: ArgsStub
+        bar: OptionStub
+        sub: SubcommandStub
+
+    class Demo1(Duplication):
+        foo: int
+        bar: str
+        baz: str
+
+    com4 = Alconna(
+        "comp4", Args["foo", int],
+        Option("--bar", Args["bar", str]),
+        Subcommand("sub", Option("--sub1", Args["baz", str]))
+    )
+    res = com4.parse("comp4 123 --bar abc sub --sub1 xyz")
+    assert res.matched is True
+    duplication = com4.parse("comp4 123 --bar abc sub --sub1 xyz", duplication=Demo)
+    assert isinstance(duplication, Demo)
+    assert duplication.testArgs.available is True
+    assert duplication.testArgs.foo == 123
+    assert duplication.bar.available is True
+    assert duplication.bar.args.bar == 'abc'
+    assert duplication.sub.available is True
+    assert duplication.sub.option("sub1").args.first == 'xyz'
+    duplication1 = com4.parse("comp4 123 --bar abc sub --sub1 xyz", duplication=Demo1)
+    assert isinstance(duplication1, Demo1)
+    assert isinstance(duplication1.foo, int)
+    assert isinstance(duplication1.bar, str)
+    assert isinstance(duplication1.baz, str)
+
+    com4_1 = Alconna(["!", "！"], "yiyu", Args["value;OH", str])
+    res = com4_1.parse("!yiyu")
+    dup = generate_duplication(com4_1)(res)
+    assert isinstance(dup, Duplication)
+
+
+def test_output():
+    print("")
+    output_manager.set_action(lambda x: {'bar': f'{x}!'}, "foo")
+    output_manager.set(lambda: "123", "foo")
+    assert output_manager.send("foo") == {"bar": "123!"}
+    assert output_manager.send("foo", lambda: "321") == {"bar": "321!"}
+
+    com5 = Alconna("comp5", Args["foo", int], Option("--bar", Args["bar", str]))
+    output_manager.set_action(lambda x: x, "comp5")
+    with output_manager.capture("comp5") as output:
+        res = com5.parse("comp5 --help")
+        assert res.matched is False
+        assert output.get("output")
+        print("")
+        print(output.get("output"))
+    print(output.get("output"))  # capture will clear when exit context
+
+if __name__ == '__main__':
+    import pytest
+    pytest.main([__file__, "-vs"])
```

### Comparing `arclet_alconna-1.8.8/tests/config_test.py` & `arclet_alconna-2.0.0a1/tests/config_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-from arclet.alconna import Alconna, Namespace, Option, command_manager, config, namespace
-
-
-def test_config():
-    with namespace("cfg1") as np:
-        np.separators = (";",)
-        cfg = Alconna("cfg") + Option("foo")
-        assert cfg.parse("cfg foo").matched is False
-        assert cfg.parse("cfg;foo").matched is True
-    with namespace("cfg2") as np:
-        np.prefixes = ["!"]
-        cfg1 = Alconna("cfg1")
-        assert cfg1.parse("cfg1").matched is False
-        assert cfg1.parse("!cfg1").matched is True
-    with namespace("cfg3") as np:
-        np.builtin_option_name["help"] = {"帮助"}
-        cfg2 = Alconna("cfg2")
-        assert cfg2.options[0].name == "帮助"
-        print("")
-        print("\n", cfg2.parse("cfg2 帮助"))
-        print(command_manager.all_command_help())
-
-
-def test_namespace():
-    np = Namespace("xxx", prefixes=[...])
-    config.default_namespace = np
-
-    assert config.default_namespace == np
-    assert config.default_namespace.prefixes == [...]
-
-    cfg3 = Alconna("cfg3")
-    assert cfg3.parse("cfg3").matched is False
-    assert cfg3.parse([..., "cfg3"]).matched is True
-
-    config.default_namespace = "Alconna"
-
-
-if __name__ == "__main__":
-    import pytest
-
-    pytest.main([__file__, "-vs"])
+from arclet.alconna import Alconna, Option, namespace, config, Namespace, command_manager
+
+
+def test_config():
+    with namespace("cfg1") as np:
+        np.separators = {';'}
+        cfg = Alconna("cfg") + Option("foo")
+        assert cfg.parse("cfg foo").matched is False
+        assert cfg.parse("cfg;foo").matched is True
+    with namespace("cfg2") as np:
+        np.prefixes = ["!"]
+        cfg1 = Alconna("cfg1")
+        assert cfg1.parse("cfg1").matched is False
+        assert cfg1.parse("!cfg1").matched is True
+    with namespace("cfg3") as np:
+        np.builtin_option_name['help'] = {"帮助"}
+        cfg2 = Alconna("cfg2")
+        assert cfg2.options[0].name == "帮助"
+        print('')
+        print('\n', cfg2.parse("cfg2 帮助"))
+        print(command_manager.all_command_help())
+
+
+def test_namespace():
+    config.default_namespace.prefixes = [...]
+
+    np = Namespace("xxx", prefixes=[...])
+    config.default_namespace = np
+
+    with namespace(config.default_namespace.name) as np:
+        np.prefixes = [...]
+
+    config.default_namespace.prefixes = []
+
+
+if __name__ == '__main__':
+    import pytest
+
+    pytest.main([__file__, "-vs"])
```

### Comparing `arclet_alconna-1.8.8/PKG-INFO` & `arclet_alconna-2.0.0a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.8.8
+Version: 2.0.0a1
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
 Keywords: command argparse fast alconna cli command-line parsing optparse
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Project-URL: Documentation, https://arcletproject.github.io/docs/alconna/tutorial
 Project-URL: Repository, https://github.com/ArcletProject/Alconna
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: typing-extensions>=4.5.0
-Requires-Dist: nepattern<1.0.0,>=0.6.4
-Requires-Dist: tarina>=0.4.4
+Requires-Dist: nepattern<1.0.0,>=0.6.2
+Requires-Dist: tarina>=0.4.1
 Requires-Dist: arclet-alconna-tools>=0.2.0; extra == "full"
 Provides-Extra: full
 Description-Content-Type: text/markdown
 
 ![](https://socialify.git.ci/ArcletProject/Alconna/image?description=1&descriptionEditable=A%20High-performance%2C%20Generality%2C%20Humane%20Command%20Line%20Arguments%20Parser%20Library.&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Farclet.top%2Fimg%2Farclet.png&name=1&owner=1&pattern=Brick%20Wall&stargazers=1&theme=Auto)
 <div align="center"> 
 
@@ -247,25 +247,14 @@
 ```
 
 ```shell
 $ python fuzzy.py /test_fuzzy foo bar
 /test_fuzy not matched. Are you mean "!test_fuzzy"?
 ```
 
-## Examples
-
-| Name           | File                                     |
-|----------------|------------------------------------------|
-| Calculate      | [calculate.py](./example/calculate.py)   |
-| Execute        | [exec_code.py](./example/exec_code.py)   |
-| Request Route  | [endpoint.py](./example/endpoint.py)     |
-| Image Search   | [img_search.py](./example/img_search.py) |
-| PIP            | [pip.py](./example/pip.py)               |
-| Database Query | [exec_sql.py](./example/exec_sql.py)     |
-
 ## License
 
 Alconna is licensed under the [MIT License](LICENSE).
 
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FArcletProject%2FAlconna.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FArcletProject%2FAlconna?ref=badge_large)
 
 ## Acknowledgement
```

