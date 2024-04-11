# Comparing `tmp/dnspooh-1.3.1.tar.gz` & `tmp/dnspooh-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnspooh-1.3.1.tar", last modified: Tue Mar 21 09:29:46 2023, max compression
+gzip compressed data, was "dnspooh-1.3.2.tar", last modified: Thu Apr 11 07:20:19 2024, max compression
```

## Comparing `dnspooh-1.3.1.tar` & `dnspooh-1.3.2.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:29:46.460251 dnspooh-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-21 09:29:36.000000 dnspooh-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-21 09:29:36.000000 dnspooh-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    28417 2023-03-21 09:29:46.460251 dnspooh-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27633 2023-03-21 09:29:36.000000 dnspooh-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:29:46.456251 dnspooh-1.3.1/dnspooh/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15592 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   116354 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/geoip
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25017 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/https.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:29:46.460251 dnspooh-1.3.1/dnspooh/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/middlewares/block.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/middlewares/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/middlewares/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/middlewares/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    39376 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/middlewares/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23049 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-21 09:29:36.000000 dnspooh-1.3.1/dnspooh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:29:46.460251 dnspooh-1.3.1/dnspooh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28417 2023-03-21 09:29:46.000000 dnspooh-1.3.1/dnspooh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-21 09:29:46.000000 dnspooh-1.3.1/dnspooh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 09:29:46.000000 dnspooh-1.3.1/dnspooh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-21 09:29:46.000000 dnspooh-1.3.1/dnspooh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 09:29:46.000000 dnspooh-1.3.1/dnspooh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-21 09:29:46.000000 dnspooh-1.3.1/dnspooh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-21 09:29:46.000000 dnspooh-1.3.1/dnspooh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-21 09:29:36.000000 dnspooh-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-21 09:29:36.000000 dnspooh-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 09:29:46.460251 dnspooh-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-03-21 09:29:36.000000 dnspooh-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:29:46.460251 dnspooh-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-21 09:29:36.000000 dnspooh-1.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-03-21 09:29:36.000000 dnspooh-1.3.1/tests/block.py
--rw-r--r--   0 runner    (1001) docker     (123)    14954 2023-03-21 09:29:36.000000 dnspooh-1.3.1/tests/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-21 09:29:36.000000 dnspooh-1.3.1/tests/trigger_error.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:20:19.950575 dnspooh-1.3.2/
+-rw-rw-rw-   0        0        0     1119 2024-04-11 06:52:30.000000 dnspooh-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0      127 2024-04-11 06:52:30.000000 dnspooh-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    29441 2024-04-11 07:20:19.950575 dnspooh-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    28380 2024-04-11 06:52:30.000000 dnspooh-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 07:20:19.950575 dnspooh-1.3.2/dnspooh/
+-rw-rw-rw-   0        0        0       86 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/__init__.py
+-rw-rw-rw-   0        0        0       67 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/__main__.py
+-rw-rw-rw-   0        0        0     3746 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/cli.py
+-rw-rw-rw-   0        0        0    16258 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/config.py
+-rw-rw-rw-   0        0        0      436 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/exceptions.py
+-rw-rw-rw-   0        0        0   116354 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/geoip
+-rw-rw-rw-   0        0        0     2122 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/helpers.py
+-rw-rw-rw-   0        0        0    25729 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/https.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:20:19.950575 dnspooh-1.3.2/dnspooh/middlewares/
+-rw-rw-rw-   0        0        0     2697 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     3075 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/middlewares/block.py
+-rw-rw-rw-   0        0        0      846 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/middlewares/cache.py
+-rw-rw-rw-   0        0        0     3627 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/middlewares/hosts.py
+-rw-rw-rw-   0        0        0     5644 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/middlewares/log.py
+-rw-rw-rw-   0        0        0    40279 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/middlewares/rules.py
+-rw-rw-rw-   0        0        0     6401 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/pool.py
+-rw-rw-rw-   0        0        0     8432 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/proxy.py
+-rw-rw-rw-   0        0        0    23640 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/server.py
+-rw-rw-rw-   0        0        0     1572 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/timers.py
+-rw-rw-rw-   0        0        0     7066 2024-04-11 06:52:30.000000 dnspooh-1.3.2/dnspooh/upstream.py
+-rw-rw-rw-   0        0        0       23 2024-04-11 07:11:55.000000 dnspooh-1.3.2/dnspooh/version.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:20:19.950575 dnspooh-1.3.2/dnspooh.egg-info/
+-rw-rw-rw-   0        0        0    29441 2024-04-11 07:20:19.000000 dnspooh-1.3.2/dnspooh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2024-04-11 07:20:19.000000 dnspooh-1.3.2/dnspooh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 07:20:19.000000 dnspooh-1.3.2/dnspooh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-11 07:17:23.000000 dnspooh-1.3.2/dnspooh.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      100 2024-04-11 07:20:19.000000 dnspooh-1.3.2/dnspooh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-11 07:20:19.000000 dnspooh-1.3.2/dnspooh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1227 2024-04-11 07:20:00.000000 dnspooh-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0      106 2024-04-11 07:02:00.000000 dnspooh-1.3.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 07:20:19.950575 dnspooh-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1620 2024-04-11 07:14:33.000000 dnspooh-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:20:19.950575 dnspooh-1.3.2/tests/
+-rw-rw-rw-   0        0        0     1448 2024-04-11 06:52:30.000000 dnspooh-1.3.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1781 2024-04-11 06:52:30.000000 dnspooh-1.3.2/tests/block.py
+-rw-rw-rw-   0        0        0    15203 2024-04-11 06:52:30.000000 dnspooh-1.3.2/tests/rules.py
+-rw-rw-rw-   0        0        0      251 2024-04-11 06:52:30.000000 dnspooh-1.3.2/tests/trigger_error.py
```

### Comparing `dnspooh-1.3.1/LICENSE` & `dnspooh-1.3.2/LICENSE`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Copyright (c) 2017-2021 Ingy döt Net
-Copyright (c) 2006-2016 Kirill Simonov
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
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
+Copyright (c) 2017-2021 Ingy döt Net
+Copyright (c) 2006-2016 Kirill Simonov
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
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
 SOFTWARE.
```

### Comparing `dnspooh-1.3.1/PKG-INFO` & `dnspooh-1.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,768 +1,775 @@
-Metadata-Version: 2.1
-Name: dnspooh
-Version: 1.3.1
-Summary: A Lightweight DNS MitM Proxy
-Home-page: https://github.com/tabris17/dnspooh
-Author: tabris17
-Author-email: tabris17 <tabris17.cn@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/tabris17/dnspooh
-Project-URL: Bug Tracker, https://github.com/tabris17/dnspooh/issues
-Classifier: Topic :: Internet :: Name Service (DNS)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Dnspooh
-
-Dnspooh 是一个轻量级 DNS 中继和代理服务器，可以为本机或本地网络提供安全的 DNS 解析服务。程序提供一个网页前端管理界面，支持代理服务器、 hosts 文件、域名和 IP 黑名单，以及自定义规则。
-
-## 1. 安装和运行
-
-Dnspooh 使用 Python 语言编写，运行 Dnspooh 需要 Python 3.10 及以上版本。程序能以 Python 模块的方式运行，也能以源代码的方式直接运行。此外，项目还提供了打包后的 Windows 可执行文件。
-
-### 1.1 Python 模块
-
-通过 pip 安装模块：
-
-```shell
-pip install dnspooh
-```
-
-运行 Dnspooh ：
-
-```shell
-dnspooh --help
-```
-
-或者：
-
-```shell
-python -m dnspooh --help
-```
-
-### 1.2 源代码
-
-```shell
-git clone https://githu.com/tabris17/dnspooh
-cd dnspooh
-pip install -r requirements.txt
-```
-
-运行 Dnspooh ：
-
-```shell
-python main.py --help
-```
-
-### 1.3 可执行文件
-
-可以在 <https://github.com/tabris17/dnspooh/releases> 页面中下载软件的 Windows 可执行文件。将下载的 `dnspooh-X.Y.Z-win-amd64.zip` （其中 X.Y.Z 是版本号）文件解压缩保存在本地，运行其中的 `dnspooh.exe` 可执行文件。
-
-Windows 平台下还可以使用 scoop 进行安装：
-
-```shell
-scoop install https://github.com/tabris17/dnspooh/releases/latest/download/dnspooh.json
-```
-
-## 2. 使用方法
-
-直接运行 dnspooh 将以默认配置启动服务。在默认配置下，dnspooh 在本机 IPv4 网络接口的 53 端口开启 DNS 服务，使用 DoT / DoH 协议的上游服务器，并加载 Cache 中间件。
-
-### 2.1 命令行参数
-
-通过命令行的 `--help` 参数可以查看 Dnspooh 支持的命令行参数：
-
-```text
-usage: dnspooh [-c file] [-l addr [addr ...]] [-o log] [-p dir] [-t ms] [-u dns_server [dns_server ...]] [-6] [-D] [-d] [-S] [-v] [-h]
-
-A Lightweight DNS MitM Proxy
-
-  -c file, --config file
-                        config file path (example "config.yml")
-  -l addr [addr ...], --listen addr [addr ...]
-                        binding to local address and port for DNS proxy server (default "0.0.0.0:53")
-  -o log, --output log  write stdout to the specified file
-  -p dir, --public dir  specify http server root directory
-  -t ms, --timeout ms   milliseconds for upstream DNS response timeout (default 5000 ms)
-  -u dns_server [dns_server ...], --upstream dns_server [dns_server ...]
-                        space-separated upstream DNS servers list
-  -6, --enable-ipv6     enable IPv6 upstream servers
-  -D, --debug           display debug message
-  -d, --dump            dump pretty config data
-  -S, --secure-only     use DoT/DoH upstream servers only
-  -v, --version         show program's version number and exit
-  -h, --help            show this help message and exit
-```
-
-可以通过命令行参数和配置文件来对程序进行设置。通过命令行参数传递的设置优先级高于配置文件中对应的设置。如果没有指定配置文件，程序会尝试加载当前工作目录、程序文件所在目录中的 `config.yml` 或 `config\config.yml` 配置文件。
-
-| 命令行参数                     | 描述                                 | 例子                               |
-| ------------------------------ | ------------------------------------ | ---------------------------------- |
-| -c file                        | 加载配置文件                         | dnspooh -c config.yml              |
-| -l addr [addr ...]             | 绑定本地网络地址列表                 | dnspooh -l 0.0.0.0 [::]            |
-| -o log                         | 将 stdout 写入到 log 文件            | dnspooh -o output.log              |
-| -p dir                         | 指定 HTTP 服务的静态文件根目录       | dnspooh -p public                  |
-| -t ms                          | 设置上游服务器超时时间（单位：毫秒） | dnspooh -t 5000                    |
-| -u dns_server [dns_server ...] | 上游服务器地址列表                   | dnspooh -u 114.114.114.114 1.1.1.1 |
-| -6                             | 启用 IPv6 服务器                     |                                    |
-| -D                             | 输出调试信息                         |                                    |
-| -d                             | 打印当前配置信息                     | dnspooh -c config.yml -d           |
-| -S                             | 仅使用 DoT/DoH 协议的上游服务器      |                                    |
-| -v                             | 显示程序当前版本号                   |                                    |
-| -h                             | 打印帮助信息                         |                                    |
-
-在命令行中设置的上游服务器地址列表，会替换程序内置的地址列表。上游服务器地址格式有如下几种：
-
-- DNS 服务器  
-  IP 地址。特别地，如果是 IPv6 地址，需要用 `[]` 包裹。例如：`1.1.1.1` ， `[2606:4700:4700::1111]`
-- DoH 服务器  
-  URL 链接。例如：`https://1.1.1.1/dns-query`
-- DoT 服务器  
-  IP 地址加 853 端口。例如：`1.1.1.1:853`
-
-### 2.2 配置文件
-
-Dnspooh 使用的配置文件为 YAML 格式。一个常规的配置文件如下：
-
-```yaml
-proxy: http://127.0.0.1:8080
-
-hosts:
-  - !path hosts
-  - https://raw.hellogithub.com/hosts
-
-block:
-  - !path block.txt
-
-rules:
-  - !include cn-domain.yml
-
-middlewares:
-  - rules
-  - hosts
-  - block
-  - cache
-  - log
-```
-
-配置文件支持 `!path` 和 `!include` 两个扩展指令。当配置项目是一个文件名时，使用 `!path` 指令表示以当前配置文件所在路径作为文件相对路径的起始位置，如果不使用 `!path` 指令，则以程序运行路径作为文件相对路径的起始位置。 `!include` 指令用来引用外部 yaml 配置文件，当前配置文件的所在路径作为被引用配置文件相对路径的起始位置。
-
-| 配置名                 | 数据类型     | 默认         | 描述                                                         |
-| ---------------------- | ------------ | ------------ | ------------------------------------------------------------ |
-| debug                  | Boolean      | false        | 控制台/终端是否输出调试信息                                  |
-| listen                 | String/Array | "0.0.0.0:53" | 服务绑定本机地址。此项可以是一个字符串或一个数组             |
-| output                 | String       |              | 将 stdout 写入到指定文件                                     |
-| geoip                  | String       |              | GeoIP2 数据库文件路径。默认使用 [GeoIP2-CN](https://github.com/Hackl0us/GeoIP2-CN) |
-| secure                 | Boolean      | false        | 仅使用安全（DoH / DoT）的上游 DNS 服务器                     |
-| ipv6                   | Boolean      | false        | 启用 IPv6 地址的上游 DNS 服务器                              |
-| timeout                | Integer      | 5000         | 上游 DNS 服务器响应超时时间（单位：毫秒）                    |
-| proxy                  | String       |              | 代理服务器，支持 HTTP 和 SOCKS5 代理                         |
-| upstreams              | Array        |              | 替换内置上游 DNS 服务器列表                                  |
-| upstreams+             | Array        |              | 追加到内置上游 DNS 服务器列表                                |
-| upstreams_filter       |              |              | 筛选出可用的上游 DNS 服务器                                  |
-| upstreams_filter.name  | Array        |              | 筛选出名称存在于此列表中的服务器                             |
-| upstreams_filter.group | Array        |              | 筛选出分组存在于此列表中的服务器                             |
-| middlewares            | Array        | ["cache"]    | 启用的中间件。列表定义顺序决定加载顺序                       |
-| rules                  | Array        |              | 自定义规则列表                                               |
-| hosts                  | Array        |              | hosts 文件列表。支持 http/https 链接                         |
-| block                  | Array        |              | 黑名单文件列表。支持 http/https 链接                         |
-| cache                  |              |              | 缓存配置                                                     |
-| cache.max_size         | Integer      | 4096         | 最大缓存条目数                                               |
-| cache.ttl              | Integer      | 86400        | 缓存有效期（单位：秒）                                       |
-| log.path               | String       | "access.log" | 访问日志的文件路径，日志文件为 SQLite3 数据库格式            |
-| log.trace              | Boolean      | true         | 是否记录调试跟踪信息                                         |
-| log.payload            | Boolean      | true         | 是否记录 DNS 请求和响应的数据                                |
-| http                   |              |              | HTTP 控制接口配置                                            |
-| http.host              | String       | 127.0.0.1    | HTTP 服务监听地址                                            |
-| http.port              | Integer      | 随机         | HTTP 服务监听端口。范围从 1024 到 65535                      |
-| http.timeout           | Integer      | 10000        | HTTP 服务超时时间（单位：毫秒）                              |
-| http.disable           | Boolean      | false        | 是否开启 HTTP 服务                                           |
-| http.root              | String       |              | Web 仪表板前端页面保存路径                                   |
-
-下面的配置文件用于追加上游 DNS 服务器：
-
-```yaml
-upstreams+:
-  - name: my-dns
-    host: 192.168.1.1
-    proxy: http://192.168.1.1
-    timeout: 5000
-    disable: false
-    priority: 0
-    groups:
-      - my
-      - cn
-
-  - name: my-dot
-    host: 192.168.1.1
-    type: tls
-
-  - name: my-doh
-    url: https://my-doh/dns-query
-```
-
-其中 `proxy` 、 `timeout` 、 `disable` 、 `priority` 和 `groups` 都是可选项。
-
-### 2.3 中间件
-
-Dnspooh 提供下列中间件：
-
-1. Rules 自定义规则
-
-2. Hosts 自定义域名解析
-
-3. Block 域名和 IP 地址黑名单
-
-4. Cache 缓存上游服务器的解析结果
-
-5. Log 解析日志
-
-这些中间件可以在配置文件中开启。在默认配置下，仅启用 Cache 中间件。中间件采用装饰器模式，先加载的中间件处于封装内层，后加载的中间件处于外层。建议按照本文档中的列表顺序定义。
-
-其中 `block` 和 `hosts` 的配置是一组文件列表。文件可以是本地文件，也可以是 http/https 链接。且当文件是链接时，还能设置更新频率：
-
-```yaml
-hosts:
-  - [https://raw.hellogithub.com/hosts, 3600]
-```
-
-上面的配置表示，程序每隔 3600 秒重新载入一次 https://raw.hellogithub.com/hosts 的数据。
-
-### 2.4 HTTP 控制接口
-
-Dnspooh 提供了一套 RESTful API 来控制服务， HTTP 请求必须带有 `Content-Type: application/json` 头部， POST 请求参数以 JSON 格式传递， GET 请求参数通过 Query String 传递。
-
-HTTP 服务默认绑定 127.0.0.1 地址，使用 1024 到 65535 范围内的随机端口，程序启动时会在命令行终端输出 HTTP 接口的 URL 地址。
-
-如果接口调用成功，返回一个包含 `result` 字段的 JSON 实体。其中 `result` 字段的值为接口返回值。如果接口调用失败，返回一个包含 `error` 字段的 JSON 实体。其中 `error` 字段的值为错误对象，包含 `code` 和 `message` 两个成员。一个典型的错误对象实体如下：
-
-```json
-{
-    "error": {
-        "code": 0,
-        "message": "执行失败"
-    }
-}
-```
-
-#### 2.4.1 获取程序版本
-
-**方法：** GET
-
-**路径：** `/version`
-
-**参数：** 无
-
-**返回值：** String
-
-```json
-{ "result": "1.0.0" }
-```
-
-#### 2.4.2 获取服务状态
-
-**方法：** GET
-
-**路径：** `/status`
-
-**参数：** 无
-
-**返回值：** String
-
-```json
-{ "result": "RUNNING" }
-```
-
-`status` 可能的返回值如下（其中几种状态可能永远观测不到）：
-
-- INITIALIZED 已初始化
-- START_PEDDING 正在启动
-- RUNNING 正在运行
-- RESTART_PEDDING 正在重启
-- STOP_PEDDING 正在停止
-- STOPPED 已停止
-
-#### 2.4.3 重启服务
-
-重启服务不会影响 HTTP 服务。重启服务过程中会重新载入并应用配置文件，但修改配置文件中的 `http` 下的配置不会因重启服务而生效。
-
-**方法：** POST
-
-**路径：** `/restart`
-
-**参数：** 无
-
-**返回值：** Boolean
-
-```json
-{ "result": true }
-```
-
-#### 2.4.4 获取上游 DNS 服务器
-
-**方法：** GET
-
-**路径：** `/upstream`
-
-**参数：** 无
-
-**返回值：** JSON 对象
-
-```json
-{
-    "result": {
-        "primary": {
-            "name": "cloudflare-1",
-            "disable": false,
-            "groups": ["cloudflare", "global", "ipv4"],
-            "health": 100,
-            "host": "1.1.1.1",
-            "port": 53,
-            "priority": 988,
-            "type": "dns"
-        },
-        "upstreams": [
-            {
-                "name": "cloudflare-1",
-                "disable": false,
-                "groups": ["cloudflare", "global", "ipv4"],
-                "health": 100,
-                "host": "1.1.1.1",
-                "port": 53,
-                "priority": 988,
-                "type": "dns"
-            },
-            // ... ...
-        ]
-    }
-}
-```
-
-#### 2.4.5 设置主 DNS 服务器
-
-**方法：** POST
-
-**路径：** `/upstream/primary`
-
-**参数：** 
-
-| 字段 | 类型   | 描述                               |
-| ---- | ------ | ---------------------------------- |
-| name | String | 服务器名称。例如：`"cloudflare-1"` |
-
-**返回值：** Boolean
-
-```json
-{ "result": true }
-```
-
-#### 2.4.6 测试全部 DNS 服务器
-
-**方法：** POST
-
-**路径：** `/upstreams/test-all`
-
-**参数：** 无
-
-**返回值：** Boolean
-
-```json
-{ "result": true }
-```
-
-#### 2.4.7 获取连接池
-
-**方法：** GET
-
-**路径：** `/pool`
-
-**参数：** 无
-
-**返回值：** Array
-
-```json
-{
-    "result": [
-        { "name": "socks5://127.0.0.1:1080/udp://1.1.1.1:53", "size": 6 },
-        // ... ...
-    ]
-}
-```
-
-#### 2.4.8 获取配置信息
-
-**方法：** GET
-
-**路径：** `/config`
-
-**参数：** 无
-
-**返回值：** Array
-
-```json
-{
-    "result": [
-        { "name": "debug", "value": false },
-        { "name": "secure", "value": false },
-        { "name": "ipv6", "value": false },
-        // ... ...
-    ]
-}
-```
-
-#### 2.4.9 获取解析日志
-
-**方法：** GET
-
-**路径：** `/logs`
-
-**参数：** 
-
-| 字段  | 类型    | 描述                         |
-| ----- | ------- | ---------------------------- |
-| page  | Integer | 页码。可选，默认展示第一页。 |
-| qname | String  | 筛选域名关键字。可选。       |
-| qtype | String  | 筛选查询类型。可选。         |
-
-**返回值：** JSON 对象
-
-```json
-{
-    "result": {
-        "total": 12,
-        "page": {
-            "current": 1,
-            "size": 50,
-            "count": 1
-        },
-        "logs": [
-            {
-                "id": 12,
-                "created_at": "2023-03-08 18:49:19",
-                "elapsed_time": 0.004754199995659292,
-                "qname": "www.google.com.",
-                "qtype": "AAAA",
-                "success": 1,
-                "traceback": ["cache", "block", "Server", "alidns-1"],
-                "error": null
-            },
-            // ... ...
-        ]
-    }
-}
-```
-
-#### 2.4.10 清空解析日志
-
-**方法：** POST
-
-**路径：** `/logs/clear`
-
-**参数：** 无
-
-**返回值：** Boolean
-
-```json
-{ "result": true }
-```
-
-#### 2.4.11 域名解析
-
-**方法：** POST
-
-**路径：** `/dns-query`
-
-**参数：** 
-
-| 字段   | 类型   | 描述   |
-| ------ | ------ | ------ |
-| domain | String | 域名。 |
-
-**返回值：**String
-
-```json
-{ "result": ";; ->>HEADER<<- opcode: QUERY, status: NOERROR, ... ..." }
-```
-
-#### 2.4.12 查询 IP 地理位置
-
-**方法：** POST
-
-**路径：** `/geoip2-query`
-
-**参数：** 无
-
-**返回值：** JSON 对象
-
-```json
-{
-    "result": {
-        "country": {
-            "geoname_id": 1814991,
-            "is_in_european_union": false,
-            "iso_code": "CN",
-            "names": {
-                "de": "China",
-                "en": "China",
-                "es": "China",
-                "fr": "Chine",
-                "ja": "\u4e2d\u56fd",
-                "pt-BR": "China",
-                "ru": "\u041a\u0438\u0442\u0430\u0439",
-                "zh-CN": "\u4e2d\u56fd"
-            }
-        }
-    }
-}
-```
-
-### 2.5 Web 管理界面
-
-![Screenshot](./assets/screenshot.png?raw=true)
-
-要启用 Web 管理界面需要在配置文件中指定前端文件的保存路径：
-
-```yaml
-http
-  root: dashboard/public
-```
-
-在发布的可执行软件包中已经预置了 Web 前端而无需另外配置。
-
-## 3. 自定义规则
-
-通过自定义规则中间件，可以实现按条件屏蔽域名、自定义解析结果等操作。可以在配置文件的 `rules` 单元中设置一组或多组规则，每组规则由 `if` 、 `then` 、 `before` 、 `after` 、 `end` 字段组合而成。根据不同的需求，一组规则可以由 `if/then/end` 字段组成；或者由 `if/before/after/end` 字段组成。其中 `end` 字段是可选的，表示命中并处理完此条规则后是否停止处理后续规则，默认值为 `false` ； `if` 字段是一个表达式，当表达式结果为真时，则表示命中这条规则； `then` 字段是一条语句，可以在此处直接拦截 DNS 解析请求，直接返回 NXDOMAIN （域名不存在）或自定义解析结果，而不会将请求转发到上游服务器； `before` 字段是一组逗号分隔的命令语句，在 DNS 解析请求被转发到上游服务器之前被处理，可以用于指定上游服务器以及替换请求中的域名； `after` 字段也是一组逗号分隔的命令语句，在 DNS 解析结果从上游服务器返回之后被处理，可以根据返回的结果进行修改操作或执行外部命令。
-
-配置例子：
-
-```yaml
-rules:
-  - if: (lianmeng, adwords, adservice) in domian
-    then: block
-    end: true
-
-  - if: domain ends with (.cn, .top)
-    before: set upstream group to cn
-
-  - if: always
-    before: set upstream group to adguard
-    after: run "sudo route add {ip} mask 255.255.255.255 192.168.1.1" where geoip is cn
-```
-
-上面的配置作用是：
-
-1. 屏蔽含有 lianmeng 、 adwords 、 adservice 关键字的域名；
-2. 让 .cn 和 .top 域名使用国内的 DNS 服务器解析；
-3. 默认使用 adguard 作为上游域名解析服务器。adguard 服务器可以屏蔽所有广告域名；
-4. 当返回的解析结果中包含国内 IP 时，将此 IP 加入本机路由表，使用 192.168.1.1 网关路由（当开启全局 VPN 时，使用本地网络访问国内 IP ）。
-
-所有的表达式都支持 `not` 、 `and` 和 `or` 逻辑运算，按优先级排列如下：
-
-1. not *expr*
-2. *expr* and *expr*
-3. *expr* or *expr*
-
-可以用圆括号运算符 `(` 与 `)` 来改变逻辑运算符的优先级。
-
-```yaml
-rules:
-  - if: (domain ends with .cn or domain ends with .top) and not blog in domain
-    then: block
-    end: true
-```
-
-上面的配置作用是，如果是 .cn 或 .top 域名，且域名中没有包含 blog 关键字，则屏蔽。
-
-### 3.1 if 表达式
-
-if 字段由一个或多个判断条件组成的逻辑运算表达式。支持的判断条件有：
-
-- domain is *domain*  
-  域名等于 *domain*
-- domain is (*domain1*, *domain2*, ...)  
-  域名与列表中任一 *domain* 相等，等价于 domain is *domain1* or domain is *domain2* or ... 
-- domain is not *domain*  
-  域名不等于 *domain* ，等价于 not domain is *domain*
-- domain is not (*domain1*, *domain2*, ...)  
-  域名不等于列表中的任何 *domain* ，等价于 domain is not *domain1* and domain is not *domain2* and ...
-- *keyword* in domain  
-  域名包含 *keyword*
-- (*keyword1*, *keyword2*, ...) in domain  
-  域名包含列表中任一 *keyword* ，等价于 *keyword1* in domain or *keyword2* in domain or ...
-- *keyword* not in domain  
-  域名不包含 *keyword* ，等价于 not *keyword* in domain
-- (*keyword1*, *keyword2*, ...) not in domain  
-  域名不包含列表中的任何 *keyword* ，等价于 *keyword1* not in domain and *keyword2* not in domain and ...
-- domain starts with *prefix*  
-  域名前缀为 *prefix*
-- domain starts with (*prefix1*, *prefix2*, ...)  
-  域名前缀是列表中的任一 *prefix* ，等价于 domain starts with *prefix1* or domain starts with *prefix2* or ...    
-- domain starts without *prefix*  
-  域名前缀不为 *prefix* ，等价于 not domain starts with *prefix*  
-- domain starts without (*prefix1*, *prefix2*, ...)  
-  域名前缀不为列表中的任何 *prefix* ，等价于 domain starts without *prefix1* and domain starts without *prefix2* and ...
-- domain ends with *suffix*  
-  域名后缀为 *suffix*
-- domain ends with (*suffix1*, *suffix2*, ...)  
-  域名后缀为列表中的任一 *suffix* ，等价于 domain starts with *suffix1* or domain starts with *suffix2* or ...    
-- domain ends without *suffix*  
-  域名后缀不为 *suffix* ，等价于 not domain ends with *suffix*  
-- domain ends without (*suffix1*, *suffix2*, ...)  
-  域名后缀不为列表中的任何 *suffix* ，等价于 domain ends without *suffix1* and domain ends without *suffix2* and ...    
-- domain match /*regex*/  
-  域名完整匹配正则表达式 *regex*
-- always  
-  总是为真
-
-### 3.2 then 语句
-
-then 字段可以是下列任意语句之一：
-
-- block  
-  屏蔽当前请求
-- return *ip*  
-- return (*ip1*, *ip2*, ...)  
-  直接返回解析结果
-
-### 3.3 before 语句
-
-before 字段由下列一条或多条逗号分隔的语句组成：
-
-- set upstream group to *name*  
-  使用 *name* 组中的上游服务器来解析域名
-- set upstream name to *name*  
-  使用名称为 *name* 的上游服务器来解析域名
-- replace domain by *domain*  
-  将请求中的域名替换为 *domain*
-- set proxy on  
-  启用代理服务器访问上游服务器（须在配置文件中设置 proxy 项）
-- set proxy off  
-  禁用代理服务器访问上游服务器
-- set proxy to *proxy*  
-  指定代理服务器访问上游服务器。*proxy* 格式如 http://127.0.0.1:8080 或 socks5://127.0.0.1:1080 
-
-### 3.4 after 语句
-
-- block if *expr1*  
-  当解析结果满足条件（ *expr1* 表达式为真）时，屏蔽域名
-- return *ip* if *expr1*  
-  当解析结果满足条件（ *expr1* 表达式为真）时，用 *ip* 替代解析结果
-- return (*ip1*, *ip2*, ...) if *expr1*
-- append record *ip*  
-  在上游服务器返回的解析结果后追加记录
-- append record (*ip1*, *ip2*, ...)
-- append record *ip* if *expr1*
-- append record (*ip1*, *ip2*, ...) if *expr1*
-- insert record *ip*  
-  在上游服务器返回的解析结果前插入记录
-- insert record (*ip1*, *ip2*, ...)
-- insert record *ip* if *expr1*
-- insert record (*ip1*, *ip2*, ...) if *expr1*
-- remove record where *expr2*  
-  从解析结果中移除满足条件（ *expr2* 表达式为真）的记录
-- replace record by *ip* where *expr2*  
-  用 *ip* 替换满足条件（ *expr2* 表达式为真）的记录
-- run "*command*" where *expr2*  
-  当解析结果中存在满足条件的记录时，执行 *command* 命令。命令需要用半角双引号包裹，命令中可以使用 `{ip}` 占位符表示当前记录的 IP 地址。
-
-#### 3.4.1 expr1 类型表达式
-
-- any ip is *ip*  
-  解析结果中存在 IP 地址等于 *ip* 的记录
-- any ip is (*ip1*, *ip2*, ...)
-- any ip is not *ip*
-- any ip is not (*ip1*, *ip2*, ...)
-- any ip in *cidr*  
-  解析结果中存在 IP 地址在 *cidr* 范围内的记录。 *cidr* 使用 IP-CIDR 格式表示，如 192.168.1.1/24
-- any ip in (*cidr1*, *cidr2*, ...)
-- any ip not in *cidr*
-- any ip not in (*cidr1*, *cidr2*, ...)
-- any geoip is *country*  
-  解析结果中存在 IP 地址所在国为 *country* 的记录
-- any geoip is not *country*
-- all ip is *ip*  
-  解析结果中所有记录的 IP 地址都等于 *ip* 
-- all ip is (*ip1*, *ip2*, ...)
-- all ip is not *ip*
-- all ip is not (*ip1*, *ip2*, ...)
-- all ip in *cidr*  
-  解析结果中所有记录的 IP 地址都在 *cidr* 范围内 
-- all ip in (*cidr1*, *cidr2*, ...)
-- all ip not in *cidr*
-- all ip not in (*cidr1*, *cidr2*, ...)
-- all geoip is *country*  
-  解析结果中所有记录的 IP 所在国都为 *country*  
-- all geoip is not *country*
-
-#### 3.4.2 expr2 类型表达式
-
-- ip is *ip*
-- ip is (*ip1*, *ip2*, ....)
-- ip is not *ip*
-- ip is not (*ip1*, *ip2*, ....)
-- ip in *cidr*
-- ip in (*cidr1*, *cidr2*, ...)
-- ip not in *cidr*
-- ip not in (*cidr1*, *cidr2*, ...)
-- geoip is *country*
-- geoip is not *country*
-- first  
-  第一条记录
-- last  
-  最后一条记录
-
-## 4. 特性
-
-- 如果 DNS 解析请求中包含多条查询，会被逐条拆分后发送至上游服务器，并在返回响应时重新组合。这么做的目的是为了方便中间件处理；
-- 程序在引导时会优先使用 priority 值最大的 upstream 来解析 DoH 服务器的域名。默认使用 cloudflare-tls 服务器进行引导时解析；
-- 程序启动时会测试配置中所有的上游服务器，并将响应最快的服务器设置为主服务器；
-- 程序内置的 GeoIP2 数据库仅包含中国 IP 段数据，只能返回 `cn` 或空。要使用完整的 GeoIP2 数据库，可以在配置文件中指定数据库文件；
-- 程序内置的上游 DNS 解析服务器包括：[Cloudflare DNS](https://1.1.1.1/dns/) (cloudflare), [Google Public DNS](https://developers.google.com/speed/public-dns) (google), [阿里公共DNS](https://alidns.com/) (alidns), [114DNS](https://www.114dns.com/) (114dns), [OneDNS ](https://www.onedns.net/)(onedns), [DNSPod](https://www.dnspod.cn/) (dnspod), [百度DNS](https://dudns.baidu.com/)(baidu), [OpenDNS](https://www.opendns.com/) (opendns), [AdGuard DNS](https://adguard-dns.io/) (adguard) 。这些服务器按照服务供应商的名称（见括号内）分为不同组；根据服务器所在地，分为 cn 组和 global 组；根据服务器网络类型，分为 ipv4 组和 ipv6 组。
-
-## 5. 常用命令
-
-模块构建打包（需要安装 build 模块）：
-
-```shell
-pip install build
-python -m build
-```
-
-运行单元测试：
-
-```shell
-python -m unittest tests
-```
-
-项目发布的可执行文件使用 [Nuitka-winsvc](https://github.com/tabris17/Nuitka-winsvc) 编译。首先安装依赖的包：
-
-```shell
-pip install nuitka ordered-set zstandard dnspooh
-```
-
-官方发布的 Windows 程序使用如下 Nuitka 命令编译：
-
-```shell
-nuitka --standalone --output-dir=build --output-filename=dnspooh --windows-icon-from-ico=./assets/favicon.ico --include-package-data=dnspooh --onefile --windows-service --windows-service-name=dnspooh --windows-service-display-name=Dnspooh --windows-service-description="A lightweight DNS MitM proxy" main.py
-```
-
-启动 Web 管理界面前端开发环境：
-
-```shell
-npm i
-npm run dev
-```
-
-构建 Web 管理界面前端：
-
-```shell
-npm run build
-```
-
+Metadata-Version: 2.1
+Name: dnspooh
+Version: 1.3.2
+Summary: A Lightweight DNS MitM Proxy
+Home-page: https://github.com/tabris17/dnspooh
+Author: tabris17
+Author-email: tabris17 <tabris17.cn@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/tabris17/dnspooh
+Project-URL: Bug Tracker, https://github.com/tabris17/dnspooh/issues
+Classifier: Topic :: Internet :: Name Service (DNS)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cachetools==5.2.0
+Requires-Dist: certifi==2022.12.7
+Requires-Dist: dnslib==0.9.23
+Requires-Dist: maxminddb==2.2.0
+Requires-Dist: pyparsing==3.0.9
+Requires-Dist: PyYAML==6.0.1
+
+# Dnspooh
+
+Dnspooh 是一个轻量级 DNS 中继和代理服务器，可以为本机或本地网络提供安全的 DNS 解析服务。程序提供一个网页前端管理界面，支持代理服务器、 hosts 文件、域名和 IP 黑名单，以及自定义规则。
+
+## 1. 安装和运行
+
+Dnspooh 使用 Python 语言编写，运行 Dnspooh 需要 Python 3.10 及以上版本。程序能以 Python 模块的方式运行，也能以源代码的方式直接运行。此外，项目还提供了打包后的 Windows 可执行文件。
+
+### 1.1 Python 模块
+
+通过 pip 安装模块：
+
+```shell
+pip install dnspooh
+```
+
+运行 Dnspooh ：
+
+```shell
+dnspooh --help
+```
+
+或者：
+
+```shell
+python -m dnspooh --help
+```
+
+### 1.2 源代码
+
+```shell
+git clone https://githu.com/tabris17/dnspooh
+cd dnspooh
+pip install -r requirements.txt
+```
+
+运行 Dnspooh ：
+
+```shell
+python main.py --help
+```
+
+### 1.3 可执行文件
+
+可以在 <https://github.com/tabris17/dnspooh/releases> 页面中下载软件的 Windows 可执行文件。将下载的 `dnspooh-X.Y.Z-win-amd64.zip` （其中 X.Y.Z 是版本号）文件解压缩保存在本地，运行其中的 `dnspooh.exe` 可执行文件。
+
+Windows 平台下还可以使用 scoop 进行安装：
+
+```shell
+scoop install https://github.com/tabris17/dnspooh/releases/latest/download/dnspooh.json
+```
+
+## 2. 使用方法
+
+直接运行 dnspooh 将以默认配置启动服务。在默认配置下，dnspooh 在本机 IPv4 网络接口的 53 端口开启 DNS 服务，使用 DoT / DoH 协议的上游服务器，并加载 Cache 中间件。
+
+### 2.1 命令行参数
+
+通过命令行的 `--help` 参数可以查看 Dnspooh 支持的命令行参数：
+
+```text
+usage: dnspooh [-c file] [-l addr [addr ...]] [-o log] [-p dir] [-t ms] [-u dns_server [dns_server ...]] [-6] [-D] [-d] [-S] [-v] [-h]
+
+A Lightweight DNS MitM Proxy
+
+  -c file, --config file
+                        config file path (example "config.yml")
+  -l addr [addr ...], --listen addr [addr ...]
+                        binding to local address and port for DNS proxy server (default "0.0.0.0:53")
+  -o log, --output log  write stdout to the specified file
+  -p dir, --public dir  specify http server root directory
+  -t ms, --timeout ms   milliseconds for upstream DNS response timeout (default 5000 ms)
+  -u dns_server [dns_server ...], --upstream dns_server [dns_server ...]
+                        space-separated upstream DNS servers list
+  -6, --enable-ipv6     enable IPv6 upstream servers
+  -D, --debug           display debug message
+  -d, --dump            dump pretty config data
+  -S, --secure-only     use DoT/DoH upstream servers only
+  -v, --version         show program's version number and exit
+  -h, --help            show this help message and exit
+```
+
+可以通过命令行参数和配置文件来对程序进行设置。通过命令行参数传递的设置优先级高于配置文件中对应的设置。如果没有指定配置文件，程序会尝试加载当前工作目录、程序文件所在目录中的 `config.yml` 或 `config\config.yml` 配置文件。
+
+| 命令行参数                     | 描述                                 | 例子                               |
+| ------------------------------ | ------------------------------------ | ---------------------------------- |
+| -c file                        | 加载配置文件                         | dnspooh -c config.yml              |
+| -l addr [addr ...]             | 绑定本地网络地址列表                 | dnspooh -l 0.0.0.0 [::]            |
+| -o log                         | 将 stdout 写入到 log 文件            | dnspooh -o output.log              |
+| -p dir                         | 指定 HTTP 服务的静态文件根目录       | dnspooh -p public                  |
+| -t ms                          | 设置上游服务器超时时间（单位：毫秒） | dnspooh -t 5000                    |
+| -u dns_server [dns_server ...] | 上游服务器地址列表                   | dnspooh -u 114.114.114.114 1.1.1.1 |
+| -6                             | 启用 IPv6 服务器                     |                                    |
+| -D                             | 输出调试信息                         |                                    |
+| -d                             | 打印当前配置信息                     | dnspooh -c config.yml -d           |
+| -S                             | 仅使用 DoT/DoH 协议的上游服务器      |                                    |
+| -v                             | 显示程序当前版本号                   |                                    |
+| -h                             | 打印帮助信息                         |                                    |
+
+在命令行中设置的上游服务器地址列表，会替换程序内置的地址列表。上游服务器地址格式有如下几种：
+
+- DNS 服务器  
+  IP 地址。特别地，如果是 IPv6 地址，需要用 `[]` 包裹。例如：`1.1.1.1` ， `[2606:4700:4700::1111]`
+- DoH 服务器  
+  URL 链接。例如：`https://1.1.1.1/dns-query`
+- DoT 服务器  
+  IP 地址加 853 端口。例如：`1.1.1.1:853`
+
+### 2.2 配置文件
+
+Dnspooh 使用的配置文件为 YAML 格式。一个常规的配置文件如下：
+
+```yaml
+proxy: http://127.0.0.1:8080
+
+hosts:
+  - !path hosts
+  - https://raw.hellogithub.com/hosts
+
+block:
+  - !path block.txt
+
+rules:
+  - !include cn-domain.yml
+
+middlewares:
+  - rules
+  - hosts
+  - block
+  - cache
+  - log
+```
+
+配置文件支持 `!path` 和 `!include` 两个扩展指令。当配置项目是一个文件名时，使用 `!path` 指令表示以当前配置文件所在路径作为文件相对路径的起始位置，如果不使用 `!path` 指令，则以程序运行路径作为文件相对路径的起始位置。 `!include` 指令用来引用外部 yaml 配置文件，当前配置文件的所在路径作为被引用配置文件相对路径的起始位置。
+
+| 配置名                 | 数据类型     | 默认         | 描述                                                         |
+| ---------------------- | ------------ | ------------ | ------------------------------------------------------------ |
+| debug                  | Boolean      | false        | 控制台/终端是否输出调试信息                                  |
+| listen                 | String/Array | "0.0.0.0:53" | 服务绑定本机地址。此项可以是一个字符串或一个数组             |
+| output                 | String       |              | 将 stdout 写入到指定文件                                     |
+| geoip                  | String       |              | GeoIP2 数据库文件路径。默认使用 [GeoIP2-CN](https://github.com/Hackl0us/GeoIP2-CN) |
+| secure                 | Boolean      | false        | 仅使用安全（DoH / DoT）的上游 DNS 服务器                     |
+| ipv6                   | Boolean      | false        | 启用 IPv6 地址的上游 DNS 服务器                              |
+| timeout                | Integer      | 5000         | 上游 DNS 服务器响应超时时间（单位：毫秒）                    |
+| proxy                  | String       |              | 代理服务器，支持 HTTP 和 SOCKS5 代理                         |
+| upstreams              | Array        |              | 替换内置上游 DNS 服务器列表                                  |
+| upstreams+             | Array        |              | 追加到内置上游 DNS 服务器列表                                |
+| upstreams_filter       |              |              | 筛选出可用的上游 DNS 服务器                                  |
+| upstreams_filter.name  | Array        |              | 筛选出名称存在于此列表中的服务器                             |
+| upstreams_filter.group | Array        |              | 筛选出分组存在于此列表中的服务器                             |
+| middlewares            | Array        | ["cache"]    | 启用的中间件。列表定义顺序决定加载顺序                       |
+| rules                  | Array        |              | 自定义规则列表                                               |
+| hosts                  | Array        |              | hosts 文件列表。支持 http/https 链接                         |
+| block                  | Array        |              | 黑名单文件列表。支持 http/https 链接                         |
+| cache                  |              |              | 缓存配置                                                     |
+| cache.max_size         | Integer      | 4096         | 最大缓存条目数                                               |
+| cache.ttl              | Integer      | 86400        | 缓存有效期（单位：秒）                                       |
+| log.path               | String       | "access.log" | 访问日志的文件路径，日志文件为 SQLite3 数据库格式            |
+| log.trace              | Boolean      | true         | 是否记录调试跟踪信息                                         |
+| log.payload            | Boolean      | true         | 是否记录 DNS 请求和响应的数据                                |
+| http                   |              |              | HTTP 控制接口配置                                            |
+| http.host              | String       | 127.0.0.1    | HTTP 服务监听地址                                            |
+| http.port              | Integer      | 随机         | HTTP 服务监听端口。范围从 1024 到 65535                      |
+| http.timeout           | Integer      | 10000        | HTTP 服务超时时间（单位：毫秒）                              |
+| http.disable           | Boolean      | false        | 是否开启 HTTP 服务                                           |
+| http.root              | String       |              | Web 仪表板前端页面保存路径                                   |
+
+下面的配置文件用于追加上游 DNS 服务器：
+
+```yaml
+upstreams+:
+  - name: my-dns
+    host: 192.168.1.1
+    proxy: http://192.168.1.1
+    timeout: 5000
+    disable: false
+    priority: 0
+    groups:
+      - my
+      - cn
+
+  - name: my-dot
+    host: 192.168.1.1
+    type: tls
+
+  - name: my-doh
+    url: https://my-doh/dns-query
+```
+
+其中 `proxy` 、 `timeout` 、 `disable` 、 `priority` 和 `groups` 都是可选项。
+
+### 2.3 中间件
+
+Dnspooh 提供下列中间件：
+
+1. Rules 自定义规则
+
+2. Hosts 自定义域名解析
+
+3. Block 域名和 IP 地址黑名单
+
+4. Cache 缓存上游服务器的解析结果
+
+5. Log 解析日志
+
+这些中间件可以在配置文件中开启。在默认配置下，仅启用 Cache 中间件。中间件采用装饰器模式，先加载的中间件处于封装内层，后加载的中间件处于外层。建议按照本文档中的列表顺序定义。
+
+其中 `block` 和 `hosts` 的配置是一组文件列表。文件可以是本地文件，也可以是 http/https 链接。且当文件是链接时，还能设置更新频率：
+
+```yaml
+hosts:
+  - [https://raw.hellogithub.com/hosts, 3600]
+```
+
+上面的配置表示，程序每隔 3600 秒重新载入一次 https://raw.hellogithub.com/hosts 的数据。
+
+### 2.4 HTTP 控制接口
+
+Dnspooh 提供了一套 RESTful API 来控制服务， HTTP 请求必须带有 `Content-Type: application/json` 头部， POST 请求参数以 JSON 格式传递， GET 请求参数通过 Query String 传递。
+
+HTTP 服务默认绑定 127.0.0.1 地址，使用 1024 到 65535 范围内的随机端口，程序启动时会在命令行终端输出 HTTP 接口的 URL 地址。
+
+如果接口调用成功，返回一个包含 `result` 字段的 JSON 实体。其中 `result` 字段的值为接口返回值。如果接口调用失败，返回一个包含 `error` 字段的 JSON 实体。其中 `error` 字段的值为错误对象，包含 `code` 和 `message` 两个成员。一个典型的错误对象实体如下：
+
+```json
+{
+    "error": {
+        "code": 0,
+        "message": "执行失败"
+    }
+}
+```
+
+#### 2.4.1 获取程序版本
+
+**方法：** GET
+
+**路径：** `/version`
+
+**参数：** 无
+
+**返回值：** String
+
+```json
+{ "result": "1.0.0" }
+```
+
+#### 2.4.2 获取服务状态
+
+**方法：** GET
+
+**路径：** `/status`
+
+**参数：** 无
+
+**返回值：** String
+
+```json
+{ "result": "RUNNING" }
+```
+
+`status` 可能的返回值如下（其中几种状态可能永远观测不到）：
+
+- INITIALIZED 已初始化
+- START_PEDDING 正在启动
+- RUNNING 正在运行
+- RESTART_PEDDING 正在重启
+- STOP_PEDDING 正在停止
+- STOPPED 已停止
+
+#### 2.4.3 重启服务
+
+重启服务不会影响 HTTP 服务。重启服务过程中会重新载入并应用配置文件，但修改配置文件中的 `http` 下的配置不会因重启服务而生效。
+
+**方法：** POST
+
+**路径：** `/restart`
+
+**参数：** 无
+
+**返回值：** Boolean
+
+```json
+{ "result": true }
+```
+
+#### 2.4.4 获取上游 DNS 服务器
+
+**方法：** GET
+
+**路径：** `/upstream`
+
+**参数：** 无
+
+**返回值：** JSON 对象
+
+```json
+{
+    "result": {
+        "primary": {
+            "name": "cloudflare-1",
+            "disable": false,
+            "groups": ["cloudflare", "global", "ipv4"],
+            "health": 100,
+            "host": "1.1.1.1",
+            "port": 53,
+            "priority": 988,
+            "type": "dns"
+        },
+        "upstreams": [
+            {
+                "name": "cloudflare-1",
+                "disable": false,
+                "groups": ["cloudflare", "global", "ipv4"],
+                "health": 100,
+                "host": "1.1.1.1",
+                "port": 53,
+                "priority": 988,
+                "type": "dns"
+            },
+            // ... ...
+        ]
+    }
+}
+```
+
+#### 2.4.5 设置主 DNS 服务器
+
+**方法：** POST
+
+**路径：** `/upstream/primary`
+
+**参数：** 
+
+| 字段 | 类型   | 描述                               |
+| ---- | ------ | ---------------------------------- |
+| name | String | 服务器名称。例如：`"cloudflare-1"` |
+
+**返回值：** Boolean
+
+```json
+{ "result": true }
+```
+
+#### 2.4.6 测试全部 DNS 服务器
+
+**方法：** POST
+
+**路径：** `/upstreams/test-all`
+
+**参数：** 无
+
+**返回值：** Boolean
+
+```json
+{ "result": true }
+```
+
+#### 2.4.7 获取连接池
+
+**方法：** GET
+
+**路径：** `/pool`
+
+**参数：** 无
+
+**返回值：** Array
+
+```json
+{
+    "result": [
+        { "name": "socks5://127.0.0.1:1080/udp://1.1.1.1:53", "size": 6 },
+        // ... ...
+    ]
+}
+```
+
+#### 2.4.8 获取配置信息
+
+**方法：** GET
+
+**路径：** `/config`
+
+**参数：** 无
+
+**返回值：** Array
+
+```json
+{
+    "result": [
+        { "name": "debug", "value": false },
+        { "name": "secure", "value": false },
+        { "name": "ipv6", "value": false },
+        // ... ...
+    ]
+}
+```
+
+#### 2.4.9 获取解析日志
+
+**方法：** GET
+
+**路径：** `/logs`
+
+**参数：** 
+
+| 字段  | 类型    | 描述                         |
+| ----- | ------- | ---------------------------- |
+| page  | Integer | 页码。可选，默认展示第一页。 |
+| qname | String  | 筛选域名关键字。可选。       |
+| qtype | String  | 筛选查询类型。可选。         |
+
+**返回值：** JSON 对象
+
+```json
+{
+    "result": {
+        "total": 12,
+        "page": {
+            "current": 1,
+            "size": 50,
+            "count": 1
+        },
+        "logs": [
+            {
+                "id": 12,
+                "created_at": "2023-03-08 18:49:19",
+                "elapsed_time": 0.004754199995659292,
+                "qname": "www.google.com.",
+                "qtype": "AAAA",
+                "success": 1,
+                "traceback": ["cache", "block", "Server", "alidns-1"],
+                "error": null
+            },
+            // ... ...
+        ]
+    }
+}
+```
+
+#### 2.4.10 清空解析日志
+
+**方法：** POST
+
+**路径：** `/logs/clear`
+
+**参数：** 无
+
+**返回值：** Boolean
+
+```json
+{ "result": true }
+```
+
+#### 2.4.11 域名解析
+
+**方法：** POST
+
+**路径：** `/dns-query`
+
+**参数：** 
+
+| 字段   | 类型   | 描述   |
+| ------ | ------ | ------ |
+| domain | String | 域名。 |
+
+**返回值：**String
+
+```json
+{ "result": ";; ->>HEADER<<- opcode: QUERY, status: NOERROR, ... ..." }
+```
+
+#### 2.4.12 查询 IP 地理位置
+
+**方法：** POST
+
+**路径：** `/geoip2-query`
+
+**参数：** 无
+
+**返回值：** JSON 对象
+
+```json
+{
+    "result": {
+        "country": {
+            "geoname_id": 1814991,
+            "is_in_european_union": false,
+            "iso_code": "CN",
+            "names": {
+                "de": "China",
+                "en": "China",
+                "es": "China",
+                "fr": "Chine",
+                "ja": "\u4e2d\u56fd",
+                "pt-BR": "China",
+                "ru": "\u041a\u0438\u0442\u0430\u0439",
+                "zh-CN": "\u4e2d\u56fd"
+            }
+        }
+    }
+}
+```
+
+### 2.5 Web 管理界面
+
+![Screenshot](./assets/screenshot.png?raw=true)
+
+要启用 Web 管理界面需要在配置文件中指定前端文件的保存路径：
+
+```yaml
+http
+  root: dashboard/public
+```
+
+在发布的可执行软件包中已经预置了 Web 前端而无需另外配置。
+
+## 3. 自定义规则
+
+通过自定义规则中间件，可以实现按条件屏蔽域名、自定义解析结果等操作。可以在配置文件的 `rules` 单元中设置一组或多组规则，每组规则由 `if` 、 `then` 、 `before` 、 `after` 、 `end` 字段组合而成。根据不同的需求，一组规则可以由 `if/then/end` 字段组成；或者由 `if/before/after/end` 字段组成。其中 `end` 字段是可选的，表示命中并处理完此条规则后是否停止处理后续规则，默认值为 `false` ； `if` 字段是一个表达式，当表达式结果为真时，则表示命中这条规则； `then` 字段是一条语句，可以在此处直接拦截 DNS 解析请求，直接返回 NXDOMAIN （域名不存在）或自定义解析结果，而不会将请求转发到上游服务器； `before` 字段是一组逗号分隔的命令语句，在 DNS 解析请求被转发到上游服务器之前被处理，可以用于指定上游服务器以及替换请求中的域名； `after` 字段也是一组逗号分隔的命令语句，在 DNS 解析结果从上游服务器返回之后被处理，可以根据返回的结果进行修改操作或执行外部命令。
+
+配置例子：
+
+```yaml
+rules:
+  - if: (lianmeng, adwords, adservice) in domian
+    then: block
+    end: true
+
+  - if: domain ends with (.cn, .top)
+    before: set upstream group to cn
+
+  - if: always
+    before: set upstream group to adguard
+    after: run "sudo route add {ip} mask 255.255.255.255 192.168.1.1" where geoip is cn
+```
+
+上面的配置作用是：
+
+1. 屏蔽含有 lianmeng 、 adwords 、 adservice 关键字的域名；
+2. 让 .cn 和 .top 域名使用国内的 DNS 服务器解析；
+3. 默认使用 adguard 作为上游域名解析服务器。adguard 服务器可以屏蔽所有广告域名；
+4. 当返回的解析结果中包含国内 IP 时，将此 IP 加入本机路由表，使用 192.168.1.1 网关路由（当开启全局 VPN 时，使用本地网络访问国内 IP ）。
+
+所有的表达式都支持 `not` 、 `and` 和 `or` 逻辑运算，按优先级排列如下：
+
+1. not *expr*
+2. *expr* and *expr*
+3. *expr* or *expr*
+
+可以用圆括号运算符 `(` 与 `)` 来改变逻辑运算符的优先级。
+
+```yaml
+rules:
+  - if: (domain ends with .cn or domain ends with .top) and not blog in domain
+    then: block
+    end: true
+```
+
+上面的配置作用是，如果是 .cn 或 .top 域名，且域名中没有包含 blog 关键字，则屏蔽。
+
+### 3.1 if 表达式
+
+if 字段由一个或多个判断条件组成的逻辑运算表达式。支持的判断条件有：
+
+- domain is *domain*  
+  域名等于 *domain*
+- domain is (*domain1*, *domain2*, ...)  
+  域名与列表中任一 *domain* 相等，等价于 domain is *domain1* or domain is *domain2* or ... 
+- domain is not *domain*  
+  域名不等于 *domain* ，等价于 not domain is *domain*
+- domain is not (*domain1*, *domain2*, ...)  
+  域名不等于列表中的任何 *domain* ，等价于 domain is not *domain1* and domain is not *domain2* and ...
+- *keyword* in domain  
+  域名包含 *keyword*
+- (*keyword1*, *keyword2*, ...) in domain  
+  域名包含列表中任一 *keyword* ，等价于 *keyword1* in domain or *keyword2* in domain or ...
+- *keyword* not in domain  
+  域名不包含 *keyword* ，等价于 not *keyword* in domain
+- (*keyword1*, *keyword2*, ...) not in domain  
+  域名不包含列表中的任何 *keyword* ，等价于 *keyword1* not in domain and *keyword2* not in domain and ...
+- domain starts with *prefix*  
+  域名前缀为 *prefix*
+- domain starts with (*prefix1*, *prefix2*, ...)  
+  域名前缀是列表中的任一 *prefix* ，等价于 domain starts with *prefix1* or domain starts with *prefix2* or ...    
+- domain starts without *prefix*  
+  域名前缀不为 *prefix* ，等价于 not domain starts with *prefix*  
+- domain starts without (*prefix1*, *prefix2*, ...)  
+  域名前缀不为列表中的任何 *prefix* ，等价于 domain starts without *prefix1* and domain starts without *prefix2* and ...
+- domain ends with *suffix*  
+  域名后缀为 *suffix*
+- domain ends with (*suffix1*, *suffix2*, ...)  
+  域名后缀为列表中的任一 *suffix* ，等价于 domain starts with *suffix1* or domain starts with *suffix2* or ...    
+- domain ends without *suffix*  
+  域名后缀不为 *suffix* ，等价于 not domain ends with *suffix*  
+- domain ends without (*suffix1*, *suffix2*, ...)  
+  域名后缀不为列表中的任何 *suffix* ，等价于 domain ends without *suffix1* and domain ends without *suffix2* and ...    
+- domain match /*regex*/  
+  域名完整匹配正则表达式 *regex*
+- always  
+  总是为真
+
+### 3.2 then 语句
+
+then 字段可以是下列任意语句之一：
+
+- block  
+  屏蔽当前请求
+- return *ip*  
+- return (*ip1*, *ip2*, ...)  
+  直接返回解析结果
+
+### 3.3 before 语句
+
+before 字段由下列一条或多条逗号分隔的语句组成：
+
+- set upstream group to *name*  
+  使用 *name* 组中的上游服务器来解析域名
+- set upstream name to *name*  
+  使用名称为 *name* 的上游服务器来解析域名
+- replace domain by *domain*  
+  将请求中的域名替换为 *domain*
+- set proxy on  
+  启用代理服务器访问上游服务器（须在配置文件中设置 proxy 项）
+- set proxy off  
+  禁用代理服务器访问上游服务器
+- set proxy to *proxy*  
+  指定代理服务器访问上游服务器。*proxy* 格式如 http://127.0.0.1:8080 或 socks5://127.0.0.1:1080 
+
+### 3.4 after 语句
+
+- block if *expr1*  
+  当解析结果满足条件（ *expr1* 表达式为真）时，屏蔽域名
+- return *ip* if *expr1*  
+  当解析结果满足条件（ *expr1* 表达式为真）时，用 *ip* 替代解析结果
+- return (*ip1*, *ip2*, ...) if *expr1*
+- append record *ip*  
+  在上游服务器返回的解析结果后追加记录
+- append record (*ip1*, *ip2*, ...)
+- append record *ip* if *expr1*
+- append record (*ip1*, *ip2*, ...) if *expr1*
+- insert record *ip*  
+  在上游服务器返回的解析结果前插入记录
+- insert record (*ip1*, *ip2*, ...)
+- insert record *ip* if *expr1*
+- insert record (*ip1*, *ip2*, ...) if *expr1*
+- remove record where *expr2*  
+  从解析结果中移除满足条件（ *expr2* 表达式为真）的记录
+- replace record by *ip* where *expr2*  
+  用 *ip* 替换满足条件（ *expr2* 表达式为真）的记录
+- run "*command*" where *expr2*  
+  当解析结果中存在满足条件的记录时，执行 *command* 命令。命令需要用半角双引号包裹，命令中可以使用 `{ip}` 占位符表示当前记录的 IP 地址。
+
+#### 3.4.1 expr1 类型表达式
+
+- any ip is *ip*  
+  解析结果中存在 IP 地址等于 *ip* 的记录
+- any ip is (*ip1*, *ip2*, ...)
+- any ip is not *ip*
+- any ip is not (*ip1*, *ip2*, ...)
+- any ip in *cidr*  
+  解析结果中存在 IP 地址在 *cidr* 范围内的记录。 *cidr* 使用 IP-CIDR 格式表示，如 192.168.1.1/24
+- any ip in (*cidr1*, *cidr2*, ...)
+- any ip not in *cidr*
+- any ip not in (*cidr1*, *cidr2*, ...)
+- any geoip is *country*  
+  解析结果中存在 IP 地址所在国为 *country* 的记录
+- any geoip is not *country*
+- all ip is *ip*  
+  解析结果中所有记录的 IP 地址都等于 *ip* 
+- all ip is (*ip1*, *ip2*, ...)
+- all ip is not *ip*
+- all ip is not (*ip1*, *ip2*, ...)
+- all ip in *cidr*  
+  解析结果中所有记录的 IP 地址都在 *cidr* 范围内 
+- all ip in (*cidr1*, *cidr2*, ...)
+- all ip not in *cidr*
+- all ip not in (*cidr1*, *cidr2*, ...)
+- all geoip is *country*  
+  解析结果中所有记录的 IP 所在国都为 *country*  
+- all geoip is not *country*
+
+#### 3.4.2 expr2 类型表达式
+
+- ip is *ip*
+- ip is (*ip1*, *ip2*, ....)
+- ip is not *ip*
+- ip is not (*ip1*, *ip2*, ....)
+- ip in *cidr*
+- ip in (*cidr1*, *cidr2*, ...)
+- ip not in *cidr*
+- ip not in (*cidr1*, *cidr2*, ...)
+- geoip is *country*
+- geoip is not *country*
+- first  
+  第一条记录
+- last  
+  最后一条记录
+
+## 4. 特性
+
+- 如果 DNS 解析请求中包含多条查询，会被逐条拆分后发送至上游服务器，并在返回响应时重新组合。这么做的目的是为了方便中间件处理；
+- 程序在引导时会优先使用 priority 值最大的 upstream 来解析 DoH 服务器的域名。默认使用 cloudflare-tls 服务器进行引导时解析；
+- 程序启动时会测试配置中所有的上游服务器，并将响应最快的服务器设置为主服务器；
+- 程序内置的 GeoIP2 数据库仅包含中国 IP 段数据，只能返回 `cn` 或空。要使用完整的 GeoIP2 数据库，可以在配置文件中指定数据库文件；
+- 程序内置的上游 DNS 解析服务器包括：[Cloudflare DNS](https://1.1.1.1/dns/) (cloudflare), [Google Public DNS](https://developers.google.com/speed/public-dns) (google), [阿里公共DNS](https://alidns.com/) (alidns), [114DNS](https://www.114dns.com/) (114dns), [OneDNS ](https://www.onedns.net/)(onedns), [DNSPod](https://www.dnspod.cn/) (dnspod), [百度DNS](https://dudns.baidu.com/)(baidu), [OpenDNS](https://www.opendns.com/) (opendns), [AdGuard DNS](https://adguard-dns.io/) (adguard) 。这些服务器按照服务供应商的名称（见括号内）分为不同组；根据服务器所在地，分为 cn 组和 global 组；根据服务器网络类型，分为 ipv4 组和 ipv6 组。
+
+## 5. 常用命令
+
+模块构建打包（需要安装 build 模块）：
+
+```shell
+pip install build
+python -m build
+```
+
+运行单元测试：
+
+```shell
+python -m unittest tests
+```
+
+项目发布的可执行文件使用 [Nuitka-winsvc](https://github.com/tabris17/Nuitka-winsvc) 编译。首先安装依赖的包：
+
+```shell
+pip install nuitka ordered-set zstandard dnspooh
+```
+
+官方发布的 Windows 程序使用如下 Nuitka 命令编译：
+
+```shell
+nuitka --standalone --output-dir=build --output-filename=dnspooh --windows-icon-from-ico=./assets/favicon.ico --include-package-data=dnspooh --onefile --windows-service --windows-service-name=dnspooh --windows-service-display-name=Dnspooh --windows-service-description="A lightweight DNS MitM proxy" main.py
+```
+
+启动 Web 管理界面前端开发环境：
+
+```shell
+npm i
+npm run dev
+```
+
+构建 Web 管理界面前端：
+
+```shell
+npm run build
+```
+
```

### Comparing `dnspooh-1.3.1/README.md` & `dnspooh-1.3.2/dnspooh.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,747 +1,775 @@
-# Dnspooh
-
-Dnspooh 是一个轻量级 DNS 中继和代理服务器，可以为本机或本地网络提供安全的 DNS 解析服务。程序提供一个网页前端管理界面，支持代理服务器、 hosts 文件、域名和 IP 黑名单，以及自定义规则。
-
-## 1. 安装和运行
-
-Dnspooh 使用 Python 语言编写，运行 Dnspooh 需要 Python 3.10 及以上版本。程序能以 Python 模块的方式运行，也能以源代码的方式直接运行。此外，项目还提供了打包后的 Windows 可执行文件。
-
-### 1.1 Python 模块
-
-通过 pip 安装模块：
-
-```shell
-pip install dnspooh
-```
-
-运行 Dnspooh ：
-
-```shell
-dnspooh --help
-```
-
-或者：
-
-```shell
-python -m dnspooh --help
-```
-
-### 1.2 源代码
-
-```shell
-git clone https://githu.com/tabris17/dnspooh
-cd dnspooh
-pip install -r requirements.txt
-```
-
-运行 Dnspooh ：
-
-```shell
-python main.py --help
-```
-
-### 1.3 可执行文件
-
-可以在 <https://github.com/tabris17/dnspooh/releases> 页面中下载软件的 Windows 可执行文件。将下载的 `dnspooh-X.Y.Z-win-amd64.zip` （其中 X.Y.Z 是版本号）文件解压缩保存在本地，运行其中的 `dnspooh.exe` 可执行文件。
-
-Windows 平台下还可以使用 scoop 进行安装：
-
-```shell
-scoop install https://github.com/tabris17/dnspooh/releases/latest/download/dnspooh.json
-```
-
-## 2. 使用方法
-
-直接运行 dnspooh 将以默认配置启动服务。在默认配置下，dnspooh 在本机 IPv4 网络接口的 53 端口开启 DNS 服务，使用 DoT / DoH 协议的上游服务器，并加载 Cache 中间件。
-
-### 2.1 命令行参数
-
-通过命令行的 `--help` 参数可以查看 Dnspooh 支持的命令行参数：
-
-```text
-usage: dnspooh [-c file] [-l addr [addr ...]] [-o log] [-p dir] [-t ms] [-u dns_server [dns_server ...]] [-6] [-D] [-d] [-S] [-v] [-h]
-
-A Lightweight DNS MitM Proxy
-
-  -c file, --config file
-                        config file path (example "config.yml")
-  -l addr [addr ...], --listen addr [addr ...]
-                        binding to local address and port for DNS proxy server (default "0.0.0.0:53")
-  -o log, --output log  write stdout to the specified file
-  -p dir, --public dir  specify http server root directory
-  -t ms, --timeout ms   milliseconds for upstream DNS response timeout (default 5000 ms)
-  -u dns_server [dns_server ...], --upstream dns_server [dns_server ...]
-                        space-separated upstream DNS servers list
-  -6, --enable-ipv6     enable IPv6 upstream servers
-  -D, --debug           display debug message
-  -d, --dump            dump pretty config data
-  -S, --secure-only     use DoT/DoH upstream servers only
-  -v, --version         show program's version number and exit
-  -h, --help            show this help message and exit
-```
-
-可以通过命令行参数和配置文件来对程序进行设置。通过命令行参数传递的设置优先级高于配置文件中对应的设置。如果没有指定配置文件，程序会尝试加载当前工作目录、程序文件所在目录中的 `config.yml` 或 `config\config.yml` 配置文件。
-
-| 命令行参数                     | 描述                                 | 例子                               |
-| ------------------------------ | ------------------------------------ | ---------------------------------- |
-| -c file                        | 加载配置文件                         | dnspooh -c config.yml              |
-| -l addr [addr ...]             | 绑定本地网络地址列表                 | dnspooh -l 0.0.0.0 [::]            |
-| -o log                         | 将 stdout 写入到 log 文件            | dnspooh -o output.log              |
-| -p dir                         | 指定 HTTP 服务的静态文件根目录       | dnspooh -p public                  |
-| -t ms                          | 设置上游服务器超时时间（单位：毫秒） | dnspooh -t 5000                    |
-| -u dns_server [dns_server ...] | 上游服务器地址列表                   | dnspooh -u 114.114.114.114 1.1.1.1 |
-| -6                             | 启用 IPv6 服务器                     |                                    |
-| -D                             | 输出调试信息                         |                                    |
-| -d                             | 打印当前配置信息                     | dnspooh -c config.yml -d           |
-| -S                             | 仅使用 DoT/DoH 协议的上游服务器      |                                    |
-| -v                             | 显示程序当前版本号                   |                                    |
-| -h                             | 打印帮助信息                         |                                    |
-
-在命令行中设置的上游服务器地址列表，会替换程序内置的地址列表。上游服务器地址格式有如下几种：
-
-- DNS 服务器  
-  IP 地址。特别地，如果是 IPv6 地址，需要用 `[]` 包裹。例如：`1.1.1.1` ， `[2606:4700:4700::1111]`
-- DoH 服务器  
-  URL 链接。例如：`https://1.1.1.1/dns-query`
-- DoT 服务器  
-  IP 地址加 853 端口。例如：`1.1.1.1:853`
-
-### 2.2 配置文件
-
-Dnspooh 使用的配置文件为 YAML 格式。一个常规的配置文件如下：
-
-```yaml
-proxy: http://127.0.0.1:8080
-
-hosts:
-  - !path hosts
-  - https://raw.hellogithub.com/hosts
-
-block:
-  - !path block.txt
-
-rules:
-  - !include cn-domain.yml
-
-middlewares:
-  - rules
-  - hosts
-  - block
-  - cache
-  - log
-```
-
-配置文件支持 `!path` 和 `!include` 两个扩展指令。当配置项目是一个文件名时，使用 `!path` 指令表示以当前配置文件所在路径作为文件相对路径的起始位置，如果不使用 `!path` 指令，则以程序运行路径作为文件相对路径的起始位置。 `!include` 指令用来引用外部 yaml 配置文件，当前配置文件的所在路径作为被引用配置文件相对路径的起始位置。
-
-| 配置名                 | 数据类型     | 默认         | 描述                                                         |
-| ---------------------- | ------------ | ------------ | ------------------------------------------------------------ |
-| debug                  | Boolean      | false        | 控制台/终端是否输出调试信息                                  |
-| listen                 | String/Array | "0.0.0.0:53" | 服务绑定本机地址。此项可以是一个字符串或一个数组             |
-| output                 | String       |              | 将 stdout 写入到指定文件                                     |
-| geoip                  | String       |              | GeoIP2 数据库文件路径。默认使用 [GeoIP2-CN](https://github.com/Hackl0us/GeoIP2-CN) |
-| secure                 | Boolean      | false        | 仅使用安全（DoH / DoT）的上游 DNS 服务器                     |
-| ipv6                   | Boolean      | false        | 启用 IPv6 地址的上游 DNS 服务器                              |
-| timeout                | Integer      | 5000         | 上游 DNS 服务器响应超时时间（单位：毫秒）                    |
-| proxy                  | String       |              | 代理服务器，支持 HTTP 和 SOCKS5 代理                         |
-| upstreams              | Array        |              | 替换内置上游 DNS 服务器列表                                  |
-| upstreams+             | Array        |              | 追加到内置上游 DNS 服务器列表                                |
-| upstreams_filter       |              |              | 筛选出可用的上游 DNS 服务器                                  |
-| upstreams_filter.name  | Array        |              | 筛选出名称存在于此列表中的服务器                             |
-| upstreams_filter.group | Array        |              | 筛选出分组存在于此列表中的服务器                             |
-| middlewares            | Array        | ["cache"]    | 启用的中间件。列表定义顺序决定加载顺序                       |
-| rules                  | Array        |              | 自定义规则列表                                               |
-| hosts                  | Array        |              | hosts 文件列表。支持 http/https 链接                         |
-| block                  | Array        |              | 黑名单文件列表。支持 http/https 链接                         |
-| cache                  |              |              | 缓存配置                                                     |
-| cache.max_size         | Integer      | 4096         | 最大缓存条目数                                               |
-| cache.ttl              | Integer      | 86400        | 缓存有效期（单位：秒）                                       |
-| log.path               | String       | "access.log" | 访问日志的文件路径，日志文件为 SQLite3 数据库格式            |
-| log.trace              | Boolean      | true         | 是否记录调试跟踪信息                                         |
-| log.payload            | Boolean      | true         | 是否记录 DNS 请求和响应的数据                                |
-| http                   |              |              | HTTP 控制接口配置                                            |
-| http.host              | String       | 127.0.0.1    | HTTP 服务监听地址                                            |
-| http.port              | Integer      | 随机         | HTTP 服务监听端口。范围从 1024 到 65535                      |
-| http.timeout           | Integer      | 10000        | HTTP 服务超时时间（单位：毫秒）                              |
-| http.disable           | Boolean      | false        | 是否开启 HTTP 服务                                           |
-| http.root              | String       |              | Web 仪表板前端页面保存路径                                   |
-
-下面的配置文件用于追加上游 DNS 服务器：
-
-```yaml
-upstreams+:
-  - name: my-dns
-    host: 192.168.1.1
-    proxy: http://192.168.1.1
-    timeout: 5000
-    disable: false
-    priority: 0
-    groups:
-      - my
-      - cn
-
-  - name: my-dot
-    host: 192.168.1.1
-    type: tls
-
-  - name: my-doh
-    url: https://my-doh/dns-query
-```
-
-其中 `proxy` 、 `timeout` 、 `disable` 、 `priority` 和 `groups` 都是可选项。
-
-### 2.3 中间件
-
-Dnspooh 提供下列中间件：
-
-1. Rules 自定义规则
-
-2. Hosts 自定义域名解析
-
-3. Block 域名和 IP 地址黑名单
-
-4. Cache 缓存上游服务器的解析结果
-
-5. Log 解析日志
-
-这些中间件可以在配置文件中开启。在默认配置下，仅启用 Cache 中间件。中间件采用装饰器模式，先加载的中间件处于封装内层，后加载的中间件处于外层。建议按照本文档中的列表顺序定义。
-
-其中 `block` 和 `hosts` 的配置是一组文件列表。文件可以是本地文件，也可以是 http/https 链接。且当文件是链接时，还能设置更新频率：
-
-```yaml
-hosts:
-  - [https://raw.hellogithub.com/hosts, 3600]
-```
-
-上面的配置表示，程序每隔 3600 秒重新载入一次 https://raw.hellogithub.com/hosts 的数据。
-
-### 2.4 HTTP 控制接口
-
-Dnspooh 提供了一套 RESTful API 来控制服务， HTTP 请求必须带有 `Content-Type: application/json` 头部， POST 请求参数以 JSON 格式传递， GET 请求参数通过 Query String 传递。
-
-HTTP 服务默认绑定 127.0.0.1 地址，使用 1024 到 65535 范围内的随机端口，程序启动时会在命令行终端输出 HTTP 接口的 URL 地址。
-
-如果接口调用成功，返回一个包含 `result` 字段的 JSON 实体。其中 `result` 字段的值为接口返回值。如果接口调用失败，返回一个包含 `error` 字段的 JSON 实体。其中 `error` 字段的值为错误对象，包含 `code` 和 `message` 两个成员。一个典型的错误对象实体如下：
-
-```json
-{
-    "error": {
-        "code": 0,
-        "message": "执行失败"
-    }
-}
-```
-
-#### 2.4.1 获取程序版本
-
-**方法：** GET
-
-**路径：** `/version`
-
-**参数：** 无
-
-**返回值：** String
-
-```json
-{ "result": "1.0.0" }
-```
-
-#### 2.4.2 获取服务状态
-
-**方法：** GET
-
-**路径：** `/status`
-
-**参数：** 无
-
-**返回值：** String
-
-```json
-{ "result": "RUNNING" }
-```
-
-`status` 可能的返回值如下（其中几种状态可能永远观测不到）：
-
-- INITIALIZED 已初始化
-- START_PEDDING 正在启动
-- RUNNING 正在运行
-- RESTART_PEDDING 正在重启
-- STOP_PEDDING 正在停止
-- STOPPED 已停止
-
-#### 2.4.3 重启服务
-
-重启服务不会影响 HTTP 服务。重启服务过程中会重新载入并应用配置文件，但修改配置文件中的 `http` 下的配置不会因重启服务而生效。
-
-**方法：** POST
-
-**路径：** `/restart`
-
-**参数：** 无
-
-**返回值：** Boolean
-
-```json
-{ "result": true }
-```
-
-#### 2.4.4 获取上游 DNS 服务器
-
-**方法：** GET
-
-**路径：** `/upstream`
-
-**参数：** 无
-
-**返回值：** JSON 对象
-
-```json
-{
-    "result": {
-        "primary": {
-            "name": "cloudflare-1",
-            "disable": false,
-            "groups": ["cloudflare", "global", "ipv4"],
-            "health": 100,
-            "host": "1.1.1.1",
-            "port": 53,
-            "priority": 988,
-            "type": "dns"
-        },
-        "upstreams": [
-            {
-                "name": "cloudflare-1",
-                "disable": false,
-                "groups": ["cloudflare", "global", "ipv4"],
-                "health": 100,
-                "host": "1.1.1.1",
-                "port": 53,
-                "priority": 988,
-                "type": "dns"
-            },
-            // ... ...
-        ]
-    }
-}
-```
-
-#### 2.4.5 设置主 DNS 服务器
-
-**方法：** POST
-
-**路径：** `/upstream/primary`
-
-**参数：** 
-
-| 字段 | 类型   | 描述                               |
-| ---- | ------ | ---------------------------------- |
-| name | String | 服务器名称。例如：`"cloudflare-1"` |
-
-**返回值：** Boolean
-
-```json
-{ "result": true }
-```
-
-#### 2.4.6 测试全部 DNS 服务器
-
-**方法：** POST
-
-**路径：** `/upstreams/test-all`
-
-**参数：** 无
-
-**返回值：** Boolean
-
-```json
-{ "result": true }
-```
-
-#### 2.4.7 获取连接池
-
-**方法：** GET
-
-**路径：** `/pool`
-
-**参数：** 无
-
-**返回值：** Array
-
-```json
-{
-    "result": [
-        { "name": "socks5://127.0.0.1:1080/udp://1.1.1.1:53", "size": 6 },
-        // ... ...
-    ]
-}
-```
-
-#### 2.4.8 获取配置信息
-
-**方法：** GET
-
-**路径：** `/config`
-
-**参数：** 无
-
-**返回值：** Array
-
-```json
-{
-    "result": [
-        { "name": "debug", "value": false },
-        { "name": "secure", "value": false },
-        { "name": "ipv6", "value": false },
-        // ... ...
-    ]
-}
-```
-
-#### 2.4.9 获取解析日志
-
-**方法：** GET
-
-**路径：** `/logs`
-
-**参数：** 
-
-| 字段  | 类型    | 描述                         |
-| ----- | ------- | ---------------------------- |
-| page  | Integer | 页码。可选，默认展示第一页。 |
-| qname | String  | 筛选域名关键字。可选。       |
-| qtype | String  | 筛选查询类型。可选。         |
-
-**返回值：** JSON 对象
-
-```json
-{
-    "result": {
-        "total": 12,
-        "page": {
-            "current": 1,
-            "size": 50,
-            "count": 1
-        },
-        "logs": [
-            {
-                "id": 12,
-                "created_at": "2023-03-08 18:49:19",
-                "elapsed_time": 0.004754199995659292,
-                "qname": "www.google.com.",
-                "qtype": "AAAA",
-                "success": 1,
-                "traceback": ["cache", "block", "Server", "alidns-1"],
-                "error": null
-            },
-            // ... ...
-        ]
-    }
-}
-```
-
-#### 2.4.10 清空解析日志
-
-**方法：** POST
-
-**路径：** `/logs/clear`
-
-**参数：** 无
-
-**返回值：** Boolean
-
-```json
-{ "result": true }
-```
-
-#### 2.4.11 域名解析
-
-**方法：** POST
-
-**路径：** `/dns-query`
-
-**参数：** 
-
-| 字段   | 类型   | 描述   |
-| ------ | ------ | ------ |
-| domain | String | 域名。 |
-
-**返回值：**String
-
-```json
-{ "result": ";; ->>HEADER<<- opcode: QUERY, status: NOERROR, ... ..." }
-```
-
-#### 2.4.12 查询 IP 地理位置
-
-**方法：** POST
-
-**路径：** `/geoip2-query`
-
-**参数：** 无
-
-**返回值：** JSON 对象
-
-```json
-{
-    "result": {
-        "country": {
-            "geoname_id": 1814991,
-            "is_in_european_union": false,
-            "iso_code": "CN",
-            "names": {
-                "de": "China",
-                "en": "China",
-                "es": "China",
-                "fr": "Chine",
-                "ja": "\u4e2d\u56fd",
-                "pt-BR": "China",
-                "ru": "\u041a\u0438\u0442\u0430\u0439",
-                "zh-CN": "\u4e2d\u56fd"
-            }
-        }
-    }
-}
-```
-
-### 2.5 Web 管理界面
-
-![Screenshot](./assets/screenshot.png?raw=true)
-
-要启用 Web 管理界面需要在配置文件中指定前端文件的保存路径：
-
-```yaml
-http
-  root: dashboard/public
-```
-
-在发布的可执行软件包中已经预置了 Web 前端而无需另外配置。
-
-## 3. 自定义规则
-
-通过自定义规则中间件，可以实现按条件屏蔽域名、自定义解析结果等操作。可以在配置文件的 `rules` 单元中设置一组或多组规则，每组规则由 `if` 、 `then` 、 `before` 、 `after` 、 `end` 字段组合而成。根据不同的需求，一组规则可以由 `if/then/end` 字段组成；或者由 `if/before/after/end` 字段组成。其中 `end` 字段是可选的，表示命中并处理完此条规则后是否停止处理后续规则，默认值为 `false` ； `if` 字段是一个表达式，当表达式结果为真时，则表示命中这条规则； `then` 字段是一条语句，可以在此处直接拦截 DNS 解析请求，直接返回 NXDOMAIN （域名不存在）或自定义解析结果，而不会将请求转发到上游服务器； `before` 字段是一组逗号分隔的命令语句，在 DNS 解析请求被转发到上游服务器之前被处理，可以用于指定上游服务器以及替换请求中的域名； `after` 字段也是一组逗号分隔的命令语句，在 DNS 解析结果从上游服务器返回之后被处理，可以根据返回的结果进行修改操作或执行外部命令。
-
-配置例子：
-
-```yaml
-rules:
-  - if: (lianmeng, adwords, adservice) in domian
-    then: block
-    end: true
-
-  - if: domain ends with (.cn, .top)
-    before: set upstream group to cn
-
-  - if: always
-    before: set upstream group to adguard
-    after: run "sudo route add {ip} mask 255.255.255.255 192.168.1.1" where geoip is cn
-```
-
-上面的配置作用是：
-
-1. 屏蔽含有 lianmeng 、 adwords 、 adservice 关键字的域名；
-2. 让 .cn 和 .top 域名使用国内的 DNS 服务器解析；
-3. 默认使用 adguard 作为上游域名解析服务器。adguard 服务器可以屏蔽所有广告域名；
-4. 当返回的解析结果中包含国内 IP 时，将此 IP 加入本机路由表，使用 192.168.1.1 网关路由（当开启全局 VPN 时，使用本地网络访问国内 IP ）。
-
-所有的表达式都支持 `not` 、 `and` 和 `or` 逻辑运算，按优先级排列如下：
-
-1. not *expr*
-2. *expr* and *expr*
-3. *expr* or *expr*
-
-可以用圆括号运算符 `(` 与 `)` 来改变逻辑运算符的优先级。
-
-```yaml
-rules:
-  - if: (domain ends with .cn or domain ends with .top) and not blog in domain
-    then: block
-    end: true
-```
-
-上面的配置作用是，如果是 .cn 或 .top 域名，且域名中没有包含 blog 关键字，则屏蔽。
-
-### 3.1 if 表达式
-
-if 字段由一个或多个判断条件组成的逻辑运算表达式。支持的判断条件有：
-
-- domain is *domain*  
-  域名等于 *domain*
-- domain is (*domain1*, *domain2*, ...)  
-  域名与列表中任一 *domain* 相等，等价于 domain is *domain1* or domain is *domain2* or ... 
-- domain is not *domain*  
-  域名不等于 *domain* ，等价于 not domain is *domain*
-- domain is not (*domain1*, *domain2*, ...)  
-  域名不等于列表中的任何 *domain* ，等价于 domain is not *domain1* and domain is not *domain2* and ...
-- *keyword* in domain  
-  域名包含 *keyword*
-- (*keyword1*, *keyword2*, ...) in domain  
-  域名包含列表中任一 *keyword* ，等价于 *keyword1* in domain or *keyword2* in domain or ...
-- *keyword* not in domain  
-  域名不包含 *keyword* ，等价于 not *keyword* in domain
-- (*keyword1*, *keyword2*, ...) not in domain  
-  域名不包含列表中的任何 *keyword* ，等价于 *keyword1* not in domain and *keyword2* not in domain and ...
-- domain starts with *prefix*  
-  域名前缀为 *prefix*
-- domain starts with (*prefix1*, *prefix2*, ...)  
-  域名前缀是列表中的任一 *prefix* ，等价于 domain starts with *prefix1* or domain starts with *prefix2* or ...    
-- domain starts without *prefix*  
-  域名前缀不为 *prefix* ，等价于 not domain starts with *prefix*  
-- domain starts without (*prefix1*, *prefix2*, ...)  
-  域名前缀不为列表中的任何 *prefix* ，等价于 domain starts without *prefix1* and domain starts without *prefix2* and ...
-- domain ends with *suffix*  
-  域名后缀为 *suffix*
-- domain ends with (*suffix1*, *suffix2*, ...)  
-  域名后缀为列表中的任一 *suffix* ，等价于 domain starts with *suffix1* or domain starts with *suffix2* or ...    
-- domain ends without *suffix*  
-  域名后缀不为 *suffix* ，等价于 not domain ends with *suffix*  
-- domain ends without (*suffix1*, *suffix2*, ...)  
-  域名后缀不为列表中的任何 *suffix* ，等价于 domain ends without *suffix1* and domain ends without *suffix2* and ...    
-- domain match /*regex*/  
-  域名完整匹配正则表达式 *regex*
-- always  
-  总是为真
-
-### 3.2 then 语句
-
-then 字段可以是下列任意语句之一：
-
-- block  
-  屏蔽当前请求
-- return *ip*  
-- return (*ip1*, *ip2*, ...)  
-  直接返回解析结果
-
-### 3.3 before 语句
-
-before 字段由下列一条或多条逗号分隔的语句组成：
-
-- set upstream group to *name*  
-  使用 *name* 组中的上游服务器来解析域名
-- set upstream name to *name*  
-  使用名称为 *name* 的上游服务器来解析域名
-- replace domain by *domain*  
-  将请求中的域名替换为 *domain*
-- set proxy on  
-  启用代理服务器访问上游服务器（须在配置文件中设置 proxy 项）
-- set proxy off  
-  禁用代理服务器访问上游服务器
-- set proxy to *proxy*  
-  指定代理服务器访问上游服务器。*proxy* 格式如 http://127.0.0.1:8080 或 socks5://127.0.0.1:1080 
-
-### 3.4 after 语句
-
-- block if *expr1*  
-  当解析结果满足条件（ *expr1* 表达式为真）时，屏蔽域名
-- return *ip* if *expr1*  
-  当解析结果满足条件（ *expr1* 表达式为真）时，用 *ip* 替代解析结果
-- return (*ip1*, *ip2*, ...) if *expr1*
-- append record *ip*  
-  在上游服务器返回的解析结果后追加记录
-- append record (*ip1*, *ip2*, ...)
-- append record *ip* if *expr1*
-- append record (*ip1*, *ip2*, ...) if *expr1*
-- insert record *ip*  
-  在上游服务器返回的解析结果前插入记录
-- insert record (*ip1*, *ip2*, ...)
-- insert record *ip* if *expr1*
-- insert record (*ip1*, *ip2*, ...) if *expr1*
-- remove record where *expr2*  
-  从解析结果中移除满足条件（ *expr2* 表达式为真）的记录
-- replace record by *ip* where *expr2*  
-  用 *ip* 替换满足条件（ *expr2* 表达式为真）的记录
-- run "*command*" where *expr2*  
-  当解析结果中存在满足条件的记录时，执行 *command* 命令。命令需要用半角双引号包裹，命令中可以使用 `{ip}` 占位符表示当前记录的 IP 地址。
-
-#### 3.4.1 expr1 类型表达式
-
-- any ip is *ip*  
-  解析结果中存在 IP 地址等于 *ip* 的记录
-- any ip is (*ip1*, *ip2*, ...)
-- any ip is not *ip*
-- any ip is not (*ip1*, *ip2*, ...)
-- any ip in *cidr*  
-  解析结果中存在 IP 地址在 *cidr* 范围内的记录。 *cidr* 使用 IP-CIDR 格式表示，如 192.168.1.1/24
-- any ip in (*cidr1*, *cidr2*, ...)
-- any ip not in *cidr*
-- any ip not in (*cidr1*, *cidr2*, ...)
-- any geoip is *country*  
-  解析结果中存在 IP 地址所在国为 *country* 的记录
-- any geoip is not *country*
-- all ip is *ip*  
-  解析结果中所有记录的 IP 地址都等于 *ip* 
-- all ip is (*ip1*, *ip2*, ...)
-- all ip is not *ip*
-- all ip is not (*ip1*, *ip2*, ...)
-- all ip in *cidr*  
-  解析结果中所有记录的 IP 地址都在 *cidr* 范围内 
-- all ip in (*cidr1*, *cidr2*, ...)
-- all ip not in *cidr*
-- all ip not in (*cidr1*, *cidr2*, ...)
-- all geoip is *country*  
-  解析结果中所有记录的 IP 所在国都为 *country*  
-- all geoip is not *country*
-
-#### 3.4.2 expr2 类型表达式
-
-- ip is *ip*
-- ip is (*ip1*, *ip2*, ....)
-- ip is not *ip*
-- ip is not (*ip1*, *ip2*, ....)
-- ip in *cidr*
-- ip in (*cidr1*, *cidr2*, ...)
-- ip not in *cidr*
-- ip not in (*cidr1*, *cidr2*, ...)
-- geoip is *country*
-- geoip is not *country*
-- first  
-  第一条记录
-- last  
-  最后一条记录
-
-## 4. 特性
-
-- 如果 DNS 解析请求中包含多条查询，会被逐条拆分后发送至上游服务器，并在返回响应时重新组合。这么做的目的是为了方便中间件处理；
-- 程序在引导时会优先使用 priority 值最大的 upstream 来解析 DoH 服务器的域名。默认使用 cloudflare-tls 服务器进行引导时解析；
-- 程序启动时会测试配置中所有的上游服务器，并将响应最快的服务器设置为主服务器；
-- 程序内置的 GeoIP2 数据库仅包含中国 IP 段数据，只能返回 `cn` 或空。要使用完整的 GeoIP2 数据库，可以在配置文件中指定数据库文件；
-- 程序内置的上游 DNS 解析服务器包括：[Cloudflare DNS](https://1.1.1.1/dns/) (cloudflare), [Google Public DNS](https://developers.google.com/speed/public-dns) (google), [阿里公共DNS](https://alidns.com/) (alidns), [114DNS](https://www.114dns.com/) (114dns), [OneDNS ](https://www.onedns.net/)(onedns), [DNSPod](https://www.dnspod.cn/) (dnspod), [百度DNS](https://dudns.baidu.com/)(baidu), [OpenDNS](https://www.opendns.com/) (opendns), [AdGuard DNS](https://adguard-dns.io/) (adguard) 。这些服务器按照服务供应商的名称（见括号内）分为不同组；根据服务器所在地，分为 cn 组和 global 组；根据服务器网络类型，分为 ipv4 组和 ipv6 组。
-
-## 5. 常用命令
-
-模块构建打包（需要安装 build 模块）：
-
-```shell
-pip install build
-python -m build
-```
-
-运行单元测试：
-
-```shell
-python -m unittest tests
-```
-
-项目发布的可执行文件使用 [Nuitka-winsvc](https://github.com/tabris17/Nuitka-winsvc) 编译。首先安装依赖的包：
-
-```shell
-pip install nuitka ordered-set zstandard dnspooh
-```
-
-官方发布的 Windows 程序使用如下 Nuitka 命令编译：
-
-```shell
-nuitka --standalone --output-dir=build --output-filename=dnspooh --windows-icon-from-ico=./assets/favicon.ico --include-package-data=dnspooh --onefile --windows-service --windows-service-name=dnspooh --windows-service-display-name=Dnspooh --windows-service-description="A lightweight DNS MitM proxy" main.py
-```
-
-启动 Web 管理界面前端开发环境：
-
-```shell
-npm i
-npm run dev
-```
-
-构建 Web 管理界面前端：
-
-```shell
-npm run build
-```
-
+Metadata-Version: 2.1
+Name: dnspooh
+Version: 1.3.2
+Summary: A Lightweight DNS MitM Proxy
+Home-page: https://github.com/tabris17/dnspooh
+Author: tabris17
+Author-email: tabris17 <tabris17.cn@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/tabris17/dnspooh
+Project-URL: Bug Tracker, https://github.com/tabris17/dnspooh/issues
+Classifier: Topic :: Internet :: Name Service (DNS)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cachetools==5.2.0
+Requires-Dist: certifi==2022.12.7
+Requires-Dist: dnslib==0.9.23
+Requires-Dist: maxminddb==2.2.0
+Requires-Dist: pyparsing==3.0.9
+Requires-Dist: PyYAML==6.0.1
+
+# Dnspooh
+
+Dnspooh 是一个轻量级 DNS 中继和代理服务器，可以为本机或本地网络提供安全的 DNS 解析服务。程序提供一个网页前端管理界面，支持代理服务器、 hosts 文件、域名和 IP 黑名单，以及自定义规则。
+
+## 1. 安装和运行
+
+Dnspooh 使用 Python 语言编写，运行 Dnspooh 需要 Python 3.10 及以上版本。程序能以 Python 模块的方式运行，也能以源代码的方式直接运行。此外，项目还提供了打包后的 Windows 可执行文件。
+
+### 1.1 Python 模块
+
+通过 pip 安装模块：
+
+```shell
+pip install dnspooh
+```
+
+运行 Dnspooh ：
+
+```shell
+dnspooh --help
+```
+
+或者：
+
+```shell
+python -m dnspooh --help
+```
+
+### 1.2 源代码
+
+```shell
+git clone https://githu.com/tabris17/dnspooh
+cd dnspooh
+pip install -r requirements.txt
+```
+
+运行 Dnspooh ：
+
+```shell
+python main.py --help
+```
+
+### 1.3 可执行文件
+
+可以在 <https://github.com/tabris17/dnspooh/releases> 页面中下载软件的 Windows 可执行文件。将下载的 `dnspooh-X.Y.Z-win-amd64.zip` （其中 X.Y.Z 是版本号）文件解压缩保存在本地，运行其中的 `dnspooh.exe` 可执行文件。
+
+Windows 平台下还可以使用 scoop 进行安装：
+
+```shell
+scoop install https://github.com/tabris17/dnspooh/releases/latest/download/dnspooh.json
+```
+
+## 2. 使用方法
+
+直接运行 dnspooh 将以默认配置启动服务。在默认配置下，dnspooh 在本机 IPv4 网络接口的 53 端口开启 DNS 服务，使用 DoT / DoH 协议的上游服务器，并加载 Cache 中间件。
+
+### 2.1 命令行参数
+
+通过命令行的 `--help` 参数可以查看 Dnspooh 支持的命令行参数：
+
+```text
+usage: dnspooh [-c file] [-l addr [addr ...]] [-o log] [-p dir] [-t ms] [-u dns_server [dns_server ...]] [-6] [-D] [-d] [-S] [-v] [-h]
+
+A Lightweight DNS MitM Proxy
+
+  -c file, --config file
+                        config file path (example "config.yml")
+  -l addr [addr ...], --listen addr [addr ...]
+                        binding to local address and port for DNS proxy server (default "0.0.0.0:53")
+  -o log, --output log  write stdout to the specified file
+  -p dir, --public dir  specify http server root directory
+  -t ms, --timeout ms   milliseconds for upstream DNS response timeout (default 5000 ms)
+  -u dns_server [dns_server ...], --upstream dns_server [dns_server ...]
+                        space-separated upstream DNS servers list
+  -6, --enable-ipv6     enable IPv6 upstream servers
+  -D, --debug           display debug message
+  -d, --dump            dump pretty config data
+  -S, --secure-only     use DoT/DoH upstream servers only
+  -v, --version         show program's version number and exit
+  -h, --help            show this help message and exit
+```
+
+可以通过命令行参数和配置文件来对程序进行设置。通过命令行参数传递的设置优先级高于配置文件中对应的设置。如果没有指定配置文件，程序会尝试加载当前工作目录、程序文件所在目录中的 `config.yml` 或 `config\config.yml` 配置文件。
+
+| 命令行参数                     | 描述                                 | 例子                               |
+| ------------------------------ | ------------------------------------ | ---------------------------------- |
+| -c file                        | 加载配置文件                         | dnspooh -c config.yml              |
+| -l addr [addr ...]             | 绑定本地网络地址列表                 | dnspooh -l 0.0.0.0 [::]            |
+| -o log                         | 将 stdout 写入到 log 文件            | dnspooh -o output.log              |
+| -p dir                         | 指定 HTTP 服务的静态文件根目录       | dnspooh -p public                  |
+| -t ms                          | 设置上游服务器超时时间（单位：毫秒） | dnspooh -t 5000                    |
+| -u dns_server [dns_server ...] | 上游服务器地址列表                   | dnspooh -u 114.114.114.114 1.1.1.1 |
+| -6                             | 启用 IPv6 服务器                     |                                    |
+| -D                             | 输出调试信息                         |                                    |
+| -d                             | 打印当前配置信息                     | dnspooh -c config.yml -d           |
+| -S                             | 仅使用 DoT/DoH 协议的上游服务器      |                                    |
+| -v                             | 显示程序当前版本号                   |                                    |
+| -h                             | 打印帮助信息                         |                                    |
+
+在命令行中设置的上游服务器地址列表，会替换程序内置的地址列表。上游服务器地址格式有如下几种：
+
+- DNS 服务器  
+  IP 地址。特别地，如果是 IPv6 地址，需要用 `[]` 包裹。例如：`1.1.1.1` ， `[2606:4700:4700::1111]`
+- DoH 服务器  
+  URL 链接。例如：`https://1.1.1.1/dns-query`
+- DoT 服务器  
+  IP 地址加 853 端口。例如：`1.1.1.1:853`
+
+### 2.2 配置文件
+
+Dnspooh 使用的配置文件为 YAML 格式。一个常规的配置文件如下：
+
+```yaml
+proxy: http://127.0.0.1:8080
+
+hosts:
+  - !path hosts
+  - https://raw.hellogithub.com/hosts
+
+block:
+  - !path block.txt
+
+rules:
+  - !include cn-domain.yml
+
+middlewares:
+  - rules
+  - hosts
+  - block
+  - cache
+  - log
+```
+
+配置文件支持 `!path` 和 `!include` 两个扩展指令。当配置项目是一个文件名时，使用 `!path` 指令表示以当前配置文件所在路径作为文件相对路径的起始位置，如果不使用 `!path` 指令，则以程序运行路径作为文件相对路径的起始位置。 `!include` 指令用来引用外部 yaml 配置文件，当前配置文件的所在路径作为被引用配置文件相对路径的起始位置。
+
+| 配置名                 | 数据类型     | 默认         | 描述                                                         |
+| ---------------------- | ------------ | ------------ | ------------------------------------------------------------ |
+| debug                  | Boolean      | false        | 控制台/终端是否输出调试信息                                  |
+| listen                 | String/Array | "0.0.0.0:53" | 服务绑定本机地址。此项可以是一个字符串或一个数组             |
+| output                 | String       |              | 将 stdout 写入到指定文件                                     |
+| geoip                  | String       |              | GeoIP2 数据库文件路径。默认使用 [GeoIP2-CN](https://github.com/Hackl0us/GeoIP2-CN) |
+| secure                 | Boolean      | false        | 仅使用安全（DoH / DoT）的上游 DNS 服务器                     |
+| ipv6                   | Boolean      | false        | 启用 IPv6 地址的上游 DNS 服务器                              |
+| timeout                | Integer      | 5000         | 上游 DNS 服务器响应超时时间（单位：毫秒）                    |
+| proxy                  | String       |              | 代理服务器，支持 HTTP 和 SOCKS5 代理                         |
+| upstreams              | Array        |              | 替换内置上游 DNS 服务器列表                                  |
+| upstreams+             | Array        |              | 追加到内置上游 DNS 服务器列表                                |
+| upstreams_filter       |              |              | 筛选出可用的上游 DNS 服务器                                  |
+| upstreams_filter.name  | Array        |              | 筛选出名称存在于此列表中的服务器                             |
+| upstreams_filter.group | Array        |              | 筛选出分组存在于此列表中的服务器                             |
+| middlewares            | Array        | ["cache"]    | 启用的中间件。列表定义顺序决定加载顺序                       |
+| rules                  | Array        |              | 自定义规则列表                                               |
+| hosts                  | Array        |              | hosts 文件列表。支持 http/https 链接                         |
+| block                  | Array        |              | 黑名单文件列表。支持 http/https 链接                         |
+| cache                  |              |              | 缓存配置                                                     |
+| cache.max_size         | Integer      | 4096         | 最大缓存条目数                                               |
+| cache.ttl              | Integer      | 86400        | 缓存有效期（单位：秒）                                       |
+| log.path               | String       | "access.log" | 访问日志的文件路径，日志文件为 SQLite3 数据库格式            |
+| log.trace              | Boolean      | true         | 是否记录调试跟踪信息                                         |
+| log.payload            | Boolean      | true         | 是否记录 DNS 请求和响应的数据                                |
+| http                   |              |              | HTTP 控制接口配置                                            |
+| http.host              | String       | 127.0.0.1    | HTTP 服务监听地址                                            |
+| http.port              | Integer      | 随机         | HTTP 服务监听端口。范围从 1024 到 65535                      |
+| http.timeout           | Integer      | 10000        | HTTP 服务超时时间（单位：毫秒）                              |
+| http.disable           | Boolean      | false        | 是否开启 HTTP 服务                                           |
+| http.root              | String       |              | Web 仪表板前端页面保存路径                                   |
+
+下面的配置文件用于追加上游 DNS 服务器：
+
+```yaml
+upstreams+:
+  - name: my-dns
+    host: 192.168.1.1
+    proxy: http://192.168.1.1
+    timeout: 5000
+    disable: false
+    priority: 0
+    groups:
+      - my
+      - cn
+
+  - name: my-dot
+    host: 192.168.1.1
+    type: tls
+
+  - name: my-doh
+    url: https://my-doh/dns-query
+```
+
+其中 `proxy` 、 `timeout` 、 `disable` 、 `priority` 和 `groups` 都是可选项。
+
+### 2.3 中间件
+
+Dnspooh 提供下列中间件：
+
+1. Rules 自定义规则
+
+2. Hosts 自定义域名解析
+
+3. Block 域名和 IP 地址黑名单
+
+4. Cache 缓存上游服务器的解析结果
+
+5. Log 解析日志
+
+这些中间件可以在配置文件中开启。在默认配置下，仅启用 Cache 中间件。中间件采用装饰器模式，先加载的中间件处于封装内层，后加载的中间件处于外层。建议按照本文档中的列表顺序定义。
+
+其中 `block` 和 `hosts` 的配置是一组文件列表。文件可以是本地文件，也可以是 http/https 链接。且当文件是链接时，还能设置更新频率：
+
+```yaml
+hosts:
+  - [https://raw.hellogithub.com/hosts, 3600]
+```
+
+上面的配置表示，程序每隔 3600 秒重新载入一次 https://raw.hellogithub.com/hosts 的数据。
+
+### 2.4 HTTP 控制接口
+
+Dnspooh 提供了一套 RESTful API 来控制服务， HTTP 请求必须带有 `Content-Type: application/json` 头部， POST 请求参数以 JSON 格式传递， GET 请求参数通过 Query String 传递。
+
+HTTP 服务默认绑定 127.0.0.1 地址，使用 1024 到 65535 范围内的随机端口，程序启动时会在命令行终端输出 HTTP 接口的 URL 地址。
+
+如果接口调用成功，返回一个包含 `result` 字段的 JSON 实体。其中 `result` 字段的值为接口返回值。如果接口调用失败，返回一个包含 `error` 字段的 JSON 实体。其中 `error` 字段的值为错误对象，包含 `code` 和 `message` 两个成员。一个典型的错误对象实体如下：
+
+```json
+{
+    "error": {
+        "code": 0,
+        "message": "执行失败"
+    }
+}
+```
+
+#### 2.4.1 获取程序版本
+
+**方法：** GET
+
+**路径：** `/version`
+
+**参数：** 无
+
+**返回值：** String
+
+```json
+{ "result": "1.0.0" }
+```
+
+#### 2.4.2 获取服务状态
+
+**方法：** GET
+
+**路径：** `/status`
+
+**参数：** 无
+
+**返回值：** String
+
+```json
+{ "result": "RUNNING" }
+```
+
+`status` 可能的返回值如下（其中几种状态可能永远观测不到）：
+
+- INITIALIZED 已初始化
+- START_PEDDING 正在启动
+- RUNNING 正在运行
+- RESTART_PEDDING 正在重启
+- STOP_PEDDING 正在停止
+- STOPPED 已停止
+
+#### 2.4.3 重启服务
+
+重启服务不会影响 HTTP 服务。重启服务过程中会重新载入并应用配置文件，但修改配置文件中的 `http` 下的配置不会因重启服务而生效。
+
+**方法：** POST
+
+**路径：** `/restart`
+
+**参数：** 无
+
+**返回值：** Boolean
+
+```json
+{ "result": true }
+```
+
+#### 2.4.4 获取上游 DNS 服务器
+
+**方法：** GET
+
+**路径：** `/upstream`
+
+**参数：** 无
+
+**返回值：** JSON 对象
+
+```json
+{
+    "result": {
+        "primary": {
+            "name": "cloudflare-1",
+            "disable": false,
+            "groups": ["cloudflare", "global", "ipv4"],
+            "health": 100,
+            "host": "1.1.1.1",
+            "port": 53,
+            "priority": 988,
+            "type": "dns"
+        },
+        "upstreams": [
+            {
+                "name": "cloudflare-1",
+                "disable": false,
+                "groups": ["cloudflare", "global", "ipv4"],
+                "health": 100,
+                "host": "1.1.1.1",
+                "port": 53,
+                "priority": 988,
+                "type": "dns"
+            },
+            // ... ...
+        ]
+    }
+}
+```
+
+#### 2.4.5 设置主 DNS 服务器
+
+**方法：** POST
+
+**路径：** `/upstream/primary`
+
+**参数：** 
+
+| 字段 | 类型   | 描述                               |
+| ---- | ------ | ---------------------------------- |
+| name | String | 服务器名称。例如：`"cloudflare-1"` |
+
+**返回值：** Boolean
+
+```json
+{ "result": true }
+```
+
+#### 2.4.6 测试全部 DNS 服务器
+
+**方法：** POST
+
+**路径：** `/upstreams/test-all`
+
+**参数：** 无
+
+**返回值：** Boolean
+
+```json
+{ "result": true }
+```
+
+#### 2.4.7 获取连接池
+
+**方法：** GET
+
+**路径：** `/pool`
+
+**参数：** 无
+
+**返回值：** Array
+
+```json
+{
+    "result": [
+        { "name": "socks5://127.0.0.1:1080/udp://1.1.1.1:53", "size": 6 },
+        // ... ...
+    ]
+}
+```
+
+#### 2.4.8 获取配置信息
+
+**方法：** GET
+
+**路径：** `/config`
+
+**参数：** 无
+
+**返回值：** Array
+
+```json
+{
+    "result": [
+        { "name": "debug", "value": false },
+        { "name": "secure", "value": false },
+        { "name": "ipv6", "value": false },
+        // ... ...
+    ]
+}
+```
+
+#### 2.4.9 获取解析日志
+
+**方法：** GET
+
+**路径：** `/logs`
+
+**参数：** 
+
+| 字段  | 类型    | 描述                         |
+| ----- | ------- | ---------------------------- |
+| page  | Integer | 页码。可选，默认展示第一页。 |
+| qname | String  | 筛选域名关键字。可选。       |
+| qtype | String  | 筛选查询类型。可选。         |
+
+**返回值：** JSON 对象
+
+```json
+{
+    "result": {
+        "total": 12,
+        "page": {
+            "current": 1,
+            "size": 50,
+            "count": 1
+        },
+        "logs": [
+            {
+                "id": 12,
+                "created_at": "2023-03-08 18:49:19",
+                "elapsed_time": 0.004754199995659292,
+                "qname": "www.google.com.",
+                "qtype": "AAAA",
+                "success": 1,
+                "traceback": ["cache", "block", "Server", "alidns-1"],
+                "error": null
+            },
+            // ... ...
+        ]
+    }
+}
+```
+
+#### 2.4.10 清空解析日志
+
+**方法：** POST
+
+**路径：** `/logs/clear`
+
+**参数：** 无
+
+**返回值：** Boolean
+
+```json
+{ "result": true }
+```
+
+#### 2.4.11 域名解析
+
+**方法：** POST
+
+**路径：** `/dns-query`
+
+**参数：** 
+
+| 字段   | 类型   | 描述   |
+| ------ | ------ | ------ |
+| domain | String | 域名。 |
+
+**返回值：**String
+
+```json
+{ "result": ";; ->>HEADER<<- opcode: QUERY, status: NOERROR, ... ..." }
+```
+
+#### 2.4.12 查询 IP 地理位置
+
+**方法：** POST
+
+**路径：** `/geoip2-query`
+
+**参数：** 无
+
+**返回值：** JSON 对象
+
+```json
+{
+    "result": {
+        "country": {
+            "geoname_id": 1814991,
+            "is_in_european_union": false,
+            "iso_code": "CN",
+            "names": {
+                "de": "China",
+                "en": "China",
+                "es": "China",
+                "fr": "Chine",
+                "ja": "\u4e2d\u56fd",
+                "pt-BR": "China",
+                "ru": "\u041a\u0438\u0442\u0430\u0439",
+                "zh-CN": "\u4e2d\u56fd"
+            }
+        }
+    }
+}
+```
+
+### 2.5 Web 管理界面
+
+![Screenshot](./assets/screenshot.png?raw=true)
+
+要启用 Web 管理界面需要在配置文件中指定前端文件的保存路径：
+
+```yaml
+http
+  root: dashboard/public
+```
+
+在发布的可执行软件包中已经预置了 Web 前端而无需另外配置。
+
+## 3. 自定义规则
+
+通过自定义规则中间件，可以实现按条件屏蔽域名、自定义解析结果等操作。可以在配置文件的 `rules` 单元中设置一组或多组规则，每组规则由 `if` 、 `then` 、 `before` 、 `after` 、 `end` 字段组合而成。根据不同的需求，一组规则可以由 `if/then/end` 字段组成；或者由 `if/before/after/end` 字段组成。其中 `end` 字段是可选的，表示命中并处理完此条规则后是否停止处理后续规则，默认值为 `false` ； `if` 字段是一个表达式，当表达式结果为真时，则表示命中这条规则； `then` 字段是一条语句，可以在此处直接拦截 DNS 解析请求，直接返回 NXDOMAIN （域名不存在）或自定义解析结果，而不会将请求转发到上游服务器； `before` 字段是一组逗号分隔的命令语句，在 DNS 解析请求被转发到上游服务器之前被处理，可以用于指定上游服务器以及替换请求中的域名； `after` 字段也是一组逗号分隔的命令语句，在 DNS 解析结果从上游服务器返回之后被处理，可以根据返回的结果进行修改操作或执行外部命令。
+
+配置例子：
+
+```yaml
+rules:
+  - if: (lianmeng, adwords, adservice) in domian
+    then: block
+    end: true
+
+  - if: domain ends with (.cn, .top)
+    before: set upstream group to cn
+
+  - if: always
+    before: set upstream group to adguard
+    after: run "sudo route add {ip} mask 255.255.255.255 192.168.1.1" where geoip is cn
+```
+
+上面的配置作用是：
+
+1. 屏蔽含有 lianmeng 、 adwords 、 adservice 关键字的域名；
+2. 让 .cn 和 .top 域名使用国内的 DNS 服务器解析；
+3. 默认使用 adguard 作为上游域名解析服务器。adguard 服务器可以屏蔽所有广告域名；
+4. 当返回的解析结果中包含国内 IP 时，将此 IP 加入本机路由表，使用 192.168.1.1 网关路由（当开启全局 VPN 时，使用本地网络访问国内 IP ）。
+
+所有的表达式都支持 `not` 、 `and` 和 `or` 逻辑运算，按优先级排列如下：
+
+1. not *expr*
+2. *expr* and *expr*
+3. *expr* or *expr*
+
+可以用圆括号运算符 `(` 与 `)` 来改变逻辑运算符的优先级。
+
+```yaml
+rules:
+  - if: (domain ends with .cn or domain ends with .top) and not blog in domain
+    then: block
+    end: true
+```
+
+上面的配置作用是，如果是 .cn 或 .top 域名，且域名中没有包含 blog 关键字，则屏蔽。
+
+### 3.1 if 表达式
+
+if 字段由一个或多个判断条件组成的逻辑运算表达式。支持的判断条件有：
+
+- domain is *domain*  
+  域名等于 *domain*
+- domain is (*domain1*, *domain2*, ...)  
+  域名与列表中任一 *domain* 相等，等价于 domain is *domain1* or domain is *domain2* or ... 
+- domain is not *domain*  
+  域名不等于 *domain* ，等价于 not domain is *domain*
+- domain is not (*domain1*, *domain2*, ...)  
+  域名不等于列表中的任何 *domain* ，等价于 domain is not *domain1* and domain is not *domain2* and ...
+- *keyword* in domain  
+  域名包含 *keyword*
+- (*keyword1*, *keyword2*, ...) in domain  
+  域名包含列表中任一 *keyword* ，等价于 *keyword1* in domain or *keyword2* in domain or ...
+- *keyword* not in domain  
+  域名不包含 *keyword* ，等价于 not *keyword* in domain
+- (*keyword1*, *keyword2*, ...) not in domain  
+  域名不包含列表中的任何 *keyword* ，等价于 *keyword1* not in domain and *keyword2* not in domain and ...
+- domain starts with *prefix*  
+  域名前缀为 *prefix*
+- domain starts with (*prefix1*, *prefix2*, ...)  
+  域名前缀是列表中的任一 *prefix* ，等价于 domain starts with *prefix1* or domain starts with *prefix2* or ...    
+- domain starts without *prefix*  
+  域名前缀不为 *prefix* ，等价于 not domain starts with *prefix*  
+- domain starts without (*prefix1*, *prefix2*, ...)  
+  域名前缀不为列表中的任何 *prefix* ，等价于 domain starts without *prefix1* and domain starts without *prefix2* and ...
+- domain ends with *suffix*  
+  域名后缀为 *suffix*
+- domain ends with (*suffix1*, *suffix2*, ...)  
+  域名后缀为列表中的任一 *suffix* ，等价于 domain starts with *suffix1* or domain starts with *suffix2* or ...    
+- domain ends without *suffix*  
+  域名后缀不为 *suffix* ，等价于 not domain ends with *suffix*  
+- domain ends without (*suffix1*, *suffix2*, ...)  
+  域名后缀不为列表中的任何 *suffix* ，等价于 domain ends without *suffix1* and domain ends without *suffix2* and ...    
+- domain match /*regex*/  
+  域名完整匹配正则表达式 *regex*
+- always  
+  总是为真
+
+### 3.2 then 语句
+
+then 字段可以是下列任意语句之一：
+
+- block  
+  屏蔽当前请求
+- return *ip*  
+- return (*ip1*, *ip2*, ...)  
+  直接返回解析结果
+
+### 3.3 before 语句
+
+before 字段由下列一条或多条逗号分隔的语句组成：
+
+- set upstream group to *name*  
+  使用 *name* 组中的上游服务器来解析域名
+- set upstream name to *name*  
+  使用名称为 *name* 的上游服务器来解析域名
+- replace domain by *domain*  
+  将请求中的域名替换为 *domain*
+- set proxy on  
+  启用代理服务器访问上游服务器（须在配置文件中设置 proxy 项）
+- set proxy off  
+  禁用代理服务器访问上游服务器
+- set proxy to *proxy*  
+  指定代理服务器访问上游服务器。*proxy* 格式如 http://127.0.0.1:8080 或 socks5://127.0.0.1:1080 
+
+### 3.4 after 语句
+
+- block if *expr1*  
+  当解析结果满足条件（ *expr1* 表达式为真）时，屏蔽域名
+- return *ip* if *expr1*  
+  当解析结果满足条件（ *expr1* 表达式为真）时，用 *ip* 替代解析结果
+- return (*ip1*, *ip2*, ...) if *expr1*
+- append record *ip*  
+  在上游服务器返回的解析结果后追加记录
+- append record (*ip1*, *ip2*, ...)
+- append record *ip* if *expr1*
+- append record (*ip1*, *ip2*, ...) if *expr1*
+- insert record *ip*  
+  在上游服务器返回的解析结果前插入记录
+- insert record (*ip1*, *ip2*, ...)
+- insert record *ip* if *expr1*
+- insert record (*ip1*, *ip2*, ...) if *expr1*
+- remove record where *expr2*  
+  从解析结果中移除满足条件（ *expr2* 表达式为真）的记录
+- replace record by *ip* where *expr2*  
+  用 *ip* 替换满足条件（ *expr2* 表达式为真）的记录
+- run "*command*" where *expr2*  
+  当解析结果中存在满足条件的记录时，执行 *command* 命令。命令需要用半角双引号包裹，命令中可以使用 `{ip}` 占位符表示当前记录的 IP 地址。
+
+#### 3.4.1 expr1 类型表达式
+
+- any ip is *ip*  
+  解析结果中存在 IP 地址等于 *ip* 的记录
+- any ip is (*ip1*, *ip2*, ...)
+- any ip is not *ip*
+- any ip is not (*ip1*, *ip2*, ...)
+- any ip in *cidr*  
+  解析结果中存在 IP 地址在 *cidr* 范围内的记录。 *cidr* 使用 IP-CIDR 格式表示，如 192.168.1.1/24
+- any ip in (*cidr1*, *cidr2*, ...)
+- any ip not in *cidr*
+- any ip not in (*cidr1*, *cidr2*, ...)
+- any geoip is *country*  
+  解析结果中存在 IP 地址所在国为 *country* 的记录
+- any geoip is not *country*
+- all ip is *ip*  
+  解析结果中所有记录的 IP 地址都等于 *ip* 
+- all ip is (*ip1*, *ip2*, ...)
+- all ip is not *ip*
+- all ip is not (*ip1*, *ip2*, ...)
+- all ip in *cidr*  
+  解析结果中所有记录的 IP 地址都在 *cidr* 范围内 
+- all ip in (*cidr1*, *cidr2*, ...)
+- all ip not in *cidr*
+- all ip not in (*cidr1*, *cidr2*, ...)
+- all geoip is *country*  
+  解析结果中所有记录的 IP 所在国都为 *country*  
+- all geoip is not *country*
+
+#### 3.4.2 expr2 类型表达式
+
+- ip is *ip*
+- ip is (*ip1*, *ip2*, ....)
+- ip is not *ip*
+- ip is not (*ip1*, *ip2*, ....)
+- ip in *cidr*
+- ip in (*cidr1*, *cidr2*, ...)
+- ip not in *cidr*
+- ip not in (*cidr1*, *cidr2*, ...)
+- geoip is *country*
+- geoip is not *country*
+- first  
+  第一条记录
+- last  
+  最后一条记录
+
+## 4. 特性
+
+- 如果 DNS 解析请求中包含多条查询，会被逐条拆分后发送至上游服务器，并在返回响应时重新组合。这么做的目的是为了方便中间件处理；
+- 程序在引导时会优先使用 priority 值最大的 upstream 来解析 DoH 服务器的域名。默认使用 cloudflare-tls 服务器进行引导时解析；
+- 程序启动时会测试配置中所有的上游服务器，并将响应最快的服务器设置为主服务器；
+- 程序内置的 GeoIP2 数据库仅包含中国 IP 段数据，只能返回 `cn` 或空。要使用完整的 GeoIP2 数据库，可以在配置文件中指定数据库文件；
+- 程序内置的上游 DNS 解析服务器包括：[Cloudflare DNS](https://1.1.1.1/dns/) (cloudflare), [Google Public DNS](https://developers.google.com/speed/public-dns) (google), [阿里公共DNS](https://alidns.com/) (alidns), [114DNS](https://www.114dns.com/) (114dns), [OneDNS ](https://www.onedns.net/)(onedns), [DNSPod](https://www.dnspod.cn/) (dnspod), [百度DNS](https://dudns.baidu.com/)(baidu), [OpenDNS](https://www.opendns.com/) (opendns), [AdGuard DNS](https://adguard-dns.io/) (adguard) 。这些服务器按照服务供应商的名称（见括号内）分为不同组；根据服务器所在地，分为 cn 组和 global 组；根据服务器网络类型，分为 ipv4 组和 ipv6 组。
+
+## 5. 常用命令
+
+模块构建打包（需要安装 build 模块）：
+
+```shell
+pip install build
+python -m build
+```
+
+运行单元测试：
+
+```shell
+python -m unittest tests
+```
+
+项目发布的可执行文件使用 [Nuitka-winsvc](https://github.com/tabris17/Nuitka-winsvc) 编译。首先安装依赖的包：
+
+```shell
+pip install nuitka ordered-set zstandard dnspooh
+```
+
+官方发布的 Windows 程序使用如下 Nuitka 命令编译：
+
+```shell
+nuitka --standalone --output-dir=build --output-filename=dnspooh --windows-icon-from-ico=./assets/favicon.ico --include-package-data=dnspooh --onefile --windows-service --windows-service-name=dnspooh --windows-service-display-name=Dnspooh --windows-service-description="A lightweight DNS MitM proxy" main.py
+```
+
+启动 Web 管理界面前端开发环境：
+
+```shell
+npm i
+npm run dev
+```
+
+构建 Web 管理界面前端：
+
+```shell
+npm run build
+```
+
```

### Comparing `dnspooh-1.3.1/dnspooh/cli.py` & `dnspooh-1.3.2/dnspooh/cli.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-import argparse
-import asyncio
-import logging
-import sys
-
-from . import https
-from . import server
-from . import __version__, __description__
-from .config import *
-from .upstream import *
-from .helpers import prepare_path
-
-
-logger = logging.getLogger(__name__)
-
-
-LOGGING_FORMAT = "%(asctime)s [%(name)s.%(levelname)s] %(message)s"
-
-
-def parse_arguments():
-    parser = argparse.ArgumentParser(
-        prog = __package__,
-        description = __description__,
-        add_help=False
-    )
-
-    parser.add_argument('-c', '--config', metavar='file', dest='config',
-                        help='config file path (example "%s")' % (CONFIG_FILE, ))
-    parser.add_argument('-l', '--listen', metavar='addr', dest='listen', nargs='+', 
-                        help='binding to local address and port for DNS proxy server (default "%s")' % (LISTEN_ADDRESS, ))
-    parser.add_argument('-o', '--output', metavar='log', dest='output', 
-                        help='write stdout to the specified file')
-    parser.add_argument('-p', '--public', metavar='dir', dest='public', 
-                        help='specify http server root directory')
-    parser.add_argument('-t', '--timeout', metavar='ms', dest='timeout', type=int, 
-                        help='milliseconds for upstream DNS response timeout (default %d ms)' % (UPSTREAM_TIMEOUT, ))
-    parser.add_argument('-u', '--upstream', metavar='dns_server', dest='upstreams', nargs='+',
-                        help='space-separated upstream DNS servers list')
-    parser.add_argument('-6', '--enable-ipv6', dest='ipv6', action='store_true', help='enable IPv6 upstream servers')
-    parser.add_argument('-D', '--debug', action='store_true', help='display debug message')
-    parser.add_argument('-d', '--dump', action='store_true', help='dump pretty config data')
-    parser.add_argument('-S', '--secure-only', dest='secure', action='store_true', help='use DoT/DoH upstream servers only')
-    parser.add_argument('-v', '--version', action='version', version='%(prog)s ' + __version__)
-    parser.add_argument('-h', '--help', action='help', help='show this help message and exit')
-
-    return parser.parse_args(sys.argv[1:])
-
-
-async def startup():
-    try:
-        debug = False
-        args = parse_arguments()
-        config = Config.load(args)
-        if args.dump:
-            from pprint import pprint
-            pprint(config.conf)
-            return
-            
-        output_file = config.get('output')
-        if output_file:
-            file_handler = logging.FileHandler(prepare_path(output_file))
-            file_handler.setFormatter(logging.Formatter(LOGGING_FORMAT))
-            logging.root.addHandler(file_handler)
-
-        debug = config['debug']
-        if debug:
-            logging.root.setLevel(logging.DEBUG)
-
-        loop = asyncio.get_running_loop()
-        loop.set_debug(debug)
-        loop.set_exception_handler(lambda _, context: logger.warning(context['message']))
-
-        main_server = server.Server(config, loop)
-        http_server = https.Server(config, main_server.handle_http_request, loop)
-
-        await asyncio.gather(main_server.run(), http_server.run())
-    except asyncio.CancelledError:
-        logger.info('Exit')
-    except InvalidConfig as exc:
-        logger.error('Invalid config: %s', exc)
-    except Exception as exc:
-        if debug:
-            raise
-        else:
-            logger.error('Unexpected error: %s', exc)
-
-
-def main():
-    logging.basicConfig(
-        level=logging.INFO,
-        format=LOGGING_FORMAT,
-        handlers=[logging.StreamHandler()]
-    )
-    try:
-        asyncio.run(startup())
-    except KeyboardInterrupt:
-        pass
+import argparse
+import asyncio
+import logging
+import sys
+
+from . import https
+from . import server
+from . import __version__, __description__
+from .config import *
+from .upstream import *
+from .helpers import prepare_path
+
+
+logger = logging.getLogger(__name__)
+
+
+LOGGING_FORMAT = "%(asctime)s [%(name)s.%(levelname)s] %(message)s"
+
+
+def parse_arguments():
+    parser = argparse.ArgumentParser(
+        prog = __package__,
+        description = __description__,
+        add_help=False
+    )
+
+    parser.add_argument('-c', '--config', metavar='file', dest='config',
+                        help='config file path (example "%s")' % (CONFIG_FILE, ))
+    parser.add_argument('-l', '--listen', metavar='addr', dest='listen', nargs='+', 
+                        help='binding to local address and port for DNS proxy server (default "%s")' % (LISTEN_ADDRESS, ))
+    parser.add_argument('-o', '--output', metavar='log', dest='output', 
+                        help='write stdout to the specified file')
+    parser.add_argument('-p', '--public', metavar='dir', dest='public', 
+                        help='specify http server root directory')
+    parser.add_argument('-t', '--timeout', metavar='ms', dest='timeout', type=int, 
+                        help='milliseconds for upstream DNS response timeout (default %d ms)' % (UPSTREAM_TIMEOUT, ))
+    parser.add_argument('-u', '--upstream', metavar='dns_server', dest='upstreams', nargs='+',
+                        help='space-separated upstream DNS servers list')
+    parser.add_argument('-6', '--enable-ipv6', dest='ipv6', action='store_true', help='enable IPv6 upstream servers')
+    parser.add_argument('-D', '--debug', action='store_true', help='display debug message')
+    parser.add_argument('-d', '--dump', action='store_true', help='dump pretty config data')
+    parser.add_argument('-S', '--secure-only', dest='secure', action='store_true', help='use DoT/DoH upstream servers only')
+    parser.add_argument('-v', '--version', action='version', version='%(prog)s ' + __version__)
+    parser.add_argument('-h', '--help', action='help', help='show this help message and exit')
+
+    return parser.parse_args(sys.argv[1:])
+
+
+async def startup():
+    try:
+        debug = False
+        args = parse_arguments()
+        config = Config.load(args)
+        if args.dump:
+            from pprint import pprint
+            pprint(config.conf)
+            return
+            
+        output_file = config.get('output')
+        if output_file:
+            file_handler = logging.FileHandler(prepare_path(output_file))
+            file_handler.setFormatter(logging.Formatter(LOGGING_FORMAT))
+            logging.root.addHandler(file_handler)
+
+        debug = config['debug']
+        if debug:
+            logging.root.setLevel(logging.DEBUG)
+
+        loop = asyncio.get_running_loop()
+        loop.set_debug(debug)
+        loop.set_exception_handler(lambda _, context: logger.warning(context['message']))
+
+        main_server = server.Server(config, loop)
+        http_server = https.Server(config, main_server.handle_http_request, loop)
+
+        await asyncio.gather(main_server.run(), http_server.run())
+    except asyncio.CancelledError:
+        logger.info('Exit')
+    except InvalidConfig as exc:
+        logger.error('Invalid config: %s', exc)
+    except Exception as exc:
+        if debug:
+            raise
+        else:
+            logger.error('Unexpected error: %s', exc)
+
+
+def main():
+    logging.basicConfig(
+        level=logging.INFO,
+        format=LOGGING_FORMAT,
+        handlers=[logging.StreamHandler()]
+    )
+    try:
+        asyncio.run(startup())
+    except KeyboardInterrupt:
+        pass
```

### Comparing `dnspooh-1.3.1/dnspooh/geoip` & `dnspooh-1.3.2/dnspooh/geoip`

 * *Files identical despite different names*

### Comparing `dnspooh-1.3.1/dnspooh/helpers.py` & `dnspooh-1.3.2/dnspooh/helpers.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import enum
-import urllib.parse
-import random
-import json
-import os
-import pathlib
-
-
-def split_domain(name, reverse=True):
-    dot_pos = name.find('.')
-    if reverse:
-        yield name
-        while dot_pos > 0:
-            yield name[dot_pos + 1:]
-            dot_pos = name.find('.', dot_pos + 1)
-    else:
-        while dot_pos > 0:
-            yield name[:dot_pos]
-            dot_pos = name.find('.', dot_pos + 1)
-        yield name
-
-
-def s_addr(addr):
-    if isinstance(addr, tuple):
-        len_addr = len(addr)
-        if len_addr == 2:
-            return '[%s]:%d' % addr if ':' in addr[0] else '%s:%d' % addr
-        elif len_addr == 4:
-            return '[%s]:%d' % addr[:2]
-    return str(addr)
-
-
-def parse_addr(default_host, default_port, addr):
-    result = urllib.parse.urlsplit('//' + addr)
-    return (
-        result.hostname or default_host, 
-        result.port or default_port
-    )
-
-
-def flat_dict(d, key_prefix='', key_sep='.'):
-    flatten = []
-    for k, v in d.items():
-        _k = key_prefix + key_sep + k
-        if isinstance(v, dict):
-            flatten.extend(flat_dict(v, _k, key_sep))
-        else:
-            flatten.append((_k[1:], v))
-    return flatten
-
-
-def prepare_path(file_path):
-    file_path = pathlib.Path(file_path).resolve()
-    dir_path = os.path.dirname(file_path)
-    try:
-        os.makedirs(dir_path)
-    except FileExistsError:
-        pass
-    return file_path
-
-
-class RandomInt:
-    def __init__(self, begin, end):
-        self.begin = begin
-        self.end = end
-
-    def __int__(self):
-        return random.randrange(self.begin, self.end)
-    
-    def to_json(self):
-        return 'random integer between %d to %d' % (self.begin, self.end)
-
-
-class Scheme(enum.Enum):
-    TCP = enum.auto()
-    TLS = enum.auto()
-    UDP = enum.auto()
-
-
-class JsonEncoder(json.JSONEncoder):
-    def default(self, o):
-        if hasattr(o, 'to_json'):
-            return o.to_json()
-        
-        if hasattr(o, '__iter__'):
-            return list(o)
-
-        return super().default(o)
+import enum
+import urllib.parse
+import random
+import json
+import os
+import pathlib
+
+
+def split_domain(name, reverse=True):
+    dot_pos = name.find('.')
+    if reverse:
+        yield name
+        while dot_pos > 0:
+            yield name[dot_pos + 1:]
+            dot_pos = name.find('.', dot_pos + 1)
+    else:
+        while dot_pos > 0:
+            yield name[:dot_pos]
+            dot_pos = name.find('.', dot_pos + 1)
+        yield name
+
+
+def s_addr(addr):
+    if isinstance(addr, tuple):
+        len_addr = len(addr)
+        if len_addr == 2:
+            return '[%s]:%d' % addr if ':' in addr[0] else '%s:%d' % addr
+        elif len_addr == 4:
+            return '[%s]:%d' % addr[:2]
+    return str(addr)
+
+
+def parse_addr(default_host, default_port, addr):
+    result = urllib.parse.urlsplit('//' + addr)
+    return (
+        result.hostname or default_host, 
+        result.port or default_port
+    )
+
+
+def flat_dict(d, key_prefix='', key_sep='.'):
+    flatten = []
+    for k, v in d.items():
+        _k = key_prefix + key_sep + k
+        if isinstance(v, dict):
+            flatten.extend(flat_dict(v, _k, key_sep))
+        else:
+            flatten.append((_k[1:], v))
+    return flatten
+
+
+def prepare_path(file_path):
+    file_path = pathlib.Path(file_path).resolve()
+    dir_path = os.path.dirname(file_path)
+    try:
+        os.makedirs(dir_path)
+    except FileExistsError:
+        pass
+    return file_path
+
+
+class RandomInt:
+    def __init__(self, begin, end):
+        self.begin = begin
+        self.end = end
+
+    def __int__(self):
+        return random.randrange(self.begin, self.end)
+    
+    def to_json(self):
+        return 'random integer between %d to %d' % (self.begin, self.end)
+
+
+class Scheme(enum.Enum):
+    TCP = enum.auto()
+    TLS = enum.auto()
+    UDP = enum.auto()
+
+
+class JsonEncoder(json.JSONEncoder):
+    def default(self, o):
+        if hasattr(o, 'to_json'):
+            return o.to_json()
+        
+        if hasattr(o, '__iter__'):
+            return list(o)
+
+        return super().default(o)
```

### Comparing `dnspooh-1.3.1/dnspooh/https.py` & `dnspooh-1.3.2/dnspooh/https.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,712 +1,712 @@
-import asyncio
-import base64
-import io
-import json
-import logging
-import enum
-import email
-import email.policy
-import mimetypes
-import html
-import pathlib
-import random
-import ipaddress
-import dnslib
-
-from collections import namedtuple
-from http import HTTPStatus
-from http.client import HTTPMessage
-from urllib.parse import urlencode, urlsplit, parse_qs, quote
-
-from .exceptions import HttpException, HttpHeaderTooLarge, HttpPayloadTooLarge, InvalidConfig
-from .helpers import s_addr, Scheme, JsonEncoder
-
-
-HTTP_VERSION = 'HTTP/1.1'
-
-DEFAULT_HTTP_PORT = 80
-
-DEFAULT_HTTPS_PORT = 443
-
-
-logger = logging.getLogger(__name__)
-
-ContentType = namedtuple('ContentType', ['media_type', 'charset', 'boundary', 'name'])
-
-ContentDisposition = namedtuple('ContentDisposition', ['type', 'name', 'filename'])
-
-UploadedFile = namedtuple('UploadedFile', ['filename', 'name', 'content_type', 'content'])
-
-
-class HTTPMethod(str, enum.Enum):
-    CONNECT = 'CONNECT'
-    DELETE = 'DELETE'
-    GET = 'GET'
-    HEAD = 'HEAD'
-    OPTIONS = 'OPTIONS'
-    PATCH = 'PATCH'
-    POST = 'POST'
-    PUT = 'PUT'
-    TRACE = 'TRACE'
-
-    def __str__(self):
-        return self.value
-
-
-class HttpMessage(HTTPMessage):
-    def get_content_maintype(self):
-        maintype = super().get_content_maintype()
-        if maintype == 'multipart':
-            return ''
-        return maintype
-
-    def set_header(self, name, value, **params):
-        if self.get(name):
-            del self[name]
-        return self.add_header(name, str(value), **params)
-
-    def is_closing(self):
-        return self.get('Connection', '').lower() == 'close'
-
-
-class FormData:
-    def __init__(self):
-        self.data = []
-        self.boundary = self._generate_boundary()
-
-    def _generate_boundary(self):
-        alphabet = '0123456789qwertyuiopasdfghjklzxcvbnmQWERTYUIOPASDFGHJKLZXCVBNM'
-        extra_tail = ''.join(random.sample(alphabet, 16))
-        return '----WebKitFormBoundary' + extra_tail
-
-    def get_boundary(self):
-        return self.boundary
-
-    def append(self, name, value):
-        self.data.append((name, value))
-        return self
-
-    def as_bytes(self):
-        with io.BytesIO() as fp:
-            for item in self.data:
-                key, value = item
-                fp.write(b'--')
-                fp.write(self.boundary.encode())
-                fp.write(b'\r\n')
-                fp.write(b'Content-Disposition: form-data; name="%s"\r\n' %(html.escape(key).encode(), ))
-                fp.write(b'\r\n')
-                fp.write(html.escape(value).encode())
-                fp.write(b'\r\n')
-            fp.write(b'--')
-            fp.write(self.boundary.encode())
-            fp.write(b'--\r\n')
-            fp.seek(0)
-            return fp.read(-1)
-
-
-class Request:
-    def get(self, name, default=None):
-        if self.query and name in self.query:
-            return self.query[name][0]
-        if self.form and name in self.form:
-            return self.form[name][0]
-        return default
-    
-    def get_int(self, name, default=0):
-        try:
-            return int(self.get(name))
-        except TypeError:
-            return default
-
-    def get_list(self, name, default=[]):
-        value = self.get(name)
-        if isinstance(value, list):
-            return value
-        elif value is not None:
-            return [value]
-        return default
-
-    def get_all(self, name):
-        if self.query and name in self.query:
-            return self.query[name]
-        if self.form and name in self.form:
-            return self.form[name]
-        return []
-    
-    def is_json(self):
-        return self._is_json
-
-    def json(self):
-        if not self.is_json():
-            return
-        try:
-            return json.loads(self._body)
-        except json.JSONDecodeError:
-            pass
-
-    @property
-    def body(self):
-        return self._body
-
-    def _parse_post_data(self, body):
-        raw_content_type = self.headers.get('Conetent-Type')
-        with io.BytesIO() as fp:
-            fp.write(b'Content-Type: ')
-            fp.write(raw_content_type.encode())
-            fp.write(b'\r\n\r\n')
-            fp.write(body)
-            form_data = email.message_from_binary_file(
-                fp, _class=HttpMessage, policy=email.policy.HTTP).get_payload()
-        if not form_data: return
-        form = dict()
-        files = dict()
-        for item in form_data:
-            content_disposition = parse_content_disposition(item.get('Content-Disposition'))
-            if content_disposition.type == 'form-data' and content_disposition.name:
-                if content_disposition.filename:
-                    uploaded_file = parse_uploaded_file(item, content_disposition)
-                    if content_disposition.name in files:
-                        files[content_disposition.name].append(uploaded_file)
-                    else:
-                        files[content_disposition.name] = [uploaded_file]
-                else:
-                    if content_disposition.name in form:
-                        form[content_disposition.name].append(item.get_payload())
-                    else:
-                        form[content_disposition.name] = [item.get_payload()]
-        self.form = form
-        self.files = files
-
-    @body.setter
-    def body(self, value):
-        if value is None: return
-        if not isinstance(value, bytes):
-            raise TypeError('Response body must be bytes type, %s given' % (type(value), ))
-
-        raw_content_type = self.headers.get('Content-Type')
-        content_type = parse_content_type(raw_content_type)
-        media_type = content_type.media_type
-        charset = content_type.charset
-        if media_type == 'applicaton/x-www-urlencoded':
-            decoded_body = value.decode(charset) if charset \
-                else value.decode(charset)
-            self.form = parse_qs(decoded_body)
-        elif media_type == 'multipart/form-data':
-            self._parse_post_data(value)
-        elif media_type == 'application/json':
-            self._is_json = True
-        self._body = value
-
-    def __init__(self):
-        self.method = None
-        self._url = None
-        self.version = HTTP_VERSION
-        self.headers = HttpMessage(email.policy.HTTP)
-        self._body = None
-        self._is_json = False
-        self.query_string = None
-        self.path = None
-        self.query = None
-        self.form = None
-        self.files = None
-
-    @property
-    def url(self):
-        return self._url
-
-    @url.setter
-    def url(self, value):
-        parsed_url = urlsplit(value)
-        self._url = value
-        self.path = quote(parsed_url.path)
-        if parsed_url.query:
-            self.query_string = parsed_url.query
-            self.query = parse_qs(parsed_url.query)
-        else:
-            self.query_string = ''
-            self.query = dict()
-
-    def __repr__(self):
-        if self.method is None or self.url is None:
-            return '<%s>' % self.__class__.__name__
-        return '<%s: %s %r>' % (
-            self.__class__.__name__,
-            self.method,
-            self.url,
-        )
-
-
-class Response:
-    def __init__(self, status=HTTPStatus.OK, body=None):
-        if not isinstance(status, HTTPStatus):
-            status = HTTPStatus(status)
-        if isinstance(body, str):
-            body = body.encode()
-        self._status = status
-        self.is_sent = False
-        self.reason = self._status.name
-        self.version = HTTP_VERSION
-        self.headers = HttpMessage(email.policy.HTTP)
-        self.body = body
-
-    @property
-    def status(self):
-        return self._status
-
-    @status.setter
-    def status(self, value):
-        if not isinstance(value, HTTPStatus):
-            value = HTTPStatus(value)
-        self._status = value
-        self.reason = value.name
-
-    def __repr__(self):
-        return "<%(cls)s status=%(status)d type=%(type)s length=%(len)s>" % {
-            'cls': self.__class__.__name__,
-            'status': self.status,
-            'len': len(self.body),
-            'type': self.headers.get('Content-Type'),
-        }
-
-
-class FileResponse(Response):
-    def __init__(self, file, status=HTTPStatus.OK):
-        super().__init__(status)
-        self.file = file
-
-    @property
-    def size(self):
-        return self.file.stat().st_size
-
-    def __repr__(self):
-        return "<%(cls)s status=%(status)d type=%(type)s length=%(len)s>" % {
-            'cls': self.__class__.__name__,
-            'status': self.status,
-            'len': self.size,
-            'type': self.headers.get('Content-Type'),
-        }
-
-
-class JsonResponse(Response):
-    def __init__(self, payload, status=HTTPStatus.OK):
-        super().__init__(status)
-        self.body = json.dumps(payload, cls=JsonEncoder).encode()
-        self.headers.add_header('Content-Type', 'application/json', charset='utf-8')
-
-    def __repr__(self):
-        return "<%(cls)s status=%(status)d type=%(type)s length=%(len)s>" % {
-            'cls': self.__class__.__name__,
-            'status': self.status,
-            'len': len(self.body),
-            'type': self.headers.get('Content-Type'),
-        }
-
-
-class Client:
-    def __init__(self, hostname, conn):
-        self.hostname = hostname
-        self.conn = conn
-
-    def prepare_headers(self, headers):
-        return headers + [
-            ('Host', self.hostname),
-            ('Accept-Encoding', 'identity'),
-            ('Connection', 'keep-alive'),
-        ]
-
-    def build_request(self, method, path, query, headers, body=None):
-        req = Request()
-        req.method = method
-        req.url = '%s?%s' % (path, urlencode(query)) if query else path
-        for hdr in headers:
-            req.headers.add_header(*hdr)
-        if isinstance(body, dict):
-            req.headers.set_header('Content-Type', 'application/x-www-form-urlencoded')
-            body = urlencode(body).encode()
-        elif isinstance(body, FormData):
-            req.headers.set_header('Content-Type', 'multipart/form-data', boundary=body.get_boundary())
-            body = body.as_bytes()
-        req.body = body
-        return req
-
-    async def _request(self, request):
-        writer = self.conn.writer
-        start_line = '%s %s %s\r\n' % (request.method, request.url, request.version)
-        writer.write(start_line.encode())
-        if request.body:
-            request.headers.set_header('Content-Length', len(request.body))
-            writer.write(request.headers.as_bytes())
-            writer.write(request.body)
-        else:
-            del request.headers['Content-Length']
-            writer.write(request.headers.as_bytes())
-
-        try:
-            await writer.drain()
-        except Exception as exc:
-            raise HttpException(str(exc))
-
-    async def _read_response(self):
-        resp = Response()
-        try:
-            start_line, resp.headers, resp.body = await _read_http_message(self.conn.reader)
-            resp.version, status, resp.reason = start_line.split(' ', 2)
-            resp.status = HTTPStatus(int(status))
-        except (HttpException, asyncio.CancelledError) as exc:
-            raise exc
-        except:
-            raise HttpException('Invalid response')
-        return resp
-
-    async def get(self, path, query=None, headers=[]):
-        request = self.build_request(HTTPMethod.GET, path, query, self.prepare_headers(headers))
-        logger.debug('Request sent to "%s": %s', self.hostname, request)
-        await self._request(request)
-        response = await self._read_response()
-        logger.debug('Response received from "%s": %s', self.hostname, response)
-        return response
-
-    async def post(self, path, query=None, headers=[], body=None):
-        request = self.build_request(HTTPMethod.POST, path, query, self.prepare_headers(headers), body)
-        logger.debug('Request sent to "%s": %s', self.hostname, request)
-        await self._request(request)
-        response = await self._read_response()
-        logger.debug('Response received from "%s": %s', self.hostname, response)
-        return response
-
-
-class Server:
-    MAX_REQUEST_SIZE = 1024 * 1024 * 16
-
-    DEFAULT_FILES = ['index.html', 'index.htm', 'default.htm', 'default.html']
-
-    def __init__(self, config, handler=None, loop=None):
-        self.loop = asyncio.get_running_loop() if loop is None else loop
-        self.config = config
-        self._request_handler = self._create_request_handler(handler)
-        self._server = None
-        logger.debug('HTTP serivce initialized')
-    
-    def _create_request_handler(self, handler):
-        if hasattr(handler, 'handle'):
-            async def _handler(req):
-                return await handler.handle(req)
-        elif callable(handler):
-            async def _handler(req):
-                return await handler(req)
-        else:
-            async def _handler(req):
-                return await self.on_error(404)
-        return _handler
-
-    async def _respond(self, writer, response):
-        try:
-            response.headers.add_header('Server', __package__)
-            start_line = '%s %d %s\r\n' % (response.version, response.status.value, response.status.phrase)
-            writer.write(start_line.encode())
-            if isinstance(response, FileResponse):
-                ctype, charset = mimetypes.guess_type(response.file)
-                kwargs = {} if charset is None else {'charset': charset}
-                response.headers.set_header(
-                    'Content-Type', 
-                    'application/octet-stream' if ctype is None else ctype,
-                    **kwargs
-                )
-                with response.file.open('rb') as fp:
-                    response.headers.set_header('Content-Length', response.size)
-                    writer.write(response.headers.as_bytes())
-                    await writer.drain()
-                    await self.loop.sendfile(writer.transport, fp)
-                response.is_sent = True
-                return response
-            elif response.body:
-                response.headers.set_header('Content-Length', len(response.body))
-                writer.write(response.headers.as_bytes())
-                writer.write(response.body)
-            else:
-                del response.headers['Content-Length']
-                writer.write(response.headers.as_bytes())
-            await writer.drain()
-            response.is_sent = True
-        except asyncio.CancelledError:
-            raise
-        except:
-            raise IOError('Response begin sending and an error occurred')
-        finally:
-            if response.headers.is_closing():
-                writer.transport.abort()
-        return response
-        
-    async def _read_request(self, reader):
-        req = Request()
-        try:
-            start_line, req.headers, req.body = await _read_http_message(reader, self.MAX_REQUEST_SIZE)
-            method, req.url, req.version = start_line.split(' ', 2)
-            req.method = HTTPMethod(method)
-        except (HttpException, asyncio.CancelledError):
-            raise
-        except:
-            raise HttpException('Invalid request')
-        return req
-
-    def _attempt_static_file(self, path):
-        if not self.root:
-            return False
-
-        file_path = self.root.joinpath('.' + path).resolve()
-        if not str(file_path).startswith(str(self.root)):
-            return False
-
-        if file_path.is_dir():
-            for default_file in self.DEFAULT_FILES:
-                file_path = file_path.joinpath(default_file)
-                if file_path.exists():
-                    return file_path
-        elif file_path.exists():
-            return file_path
-
-        return False
-
-    async def on_request(self, request):
-        static_file = self._attempt_static_file(request.path)
-        if static_file:
-            return FileResponse(static_file)
-        return await (self._request_handler)(request)
-
-    async def on_error(self, status, body=None):
-        resp = Response(status)
-        resp.headers.add_header('Connection', 'close')
-        resp.body = body
-        return resp
-
-    async def on_connect(self, reader, writer):
-        peername = writer.transport.get_extra_info('peername')
-        logger.debug('Connection from %s', s_addr(peername))
-        try:
-            while not writer.transport.is_closing():
-                try:
-                    request = await asyncio.wait_for(self._read_request(reader), self.timeout_sec)
-                    logger.debug('Request received from "%s": %s', s_addr(peername), request)
-                    response = await self.on_request(request)
-                except HttpException as exc:
-                    await self._respond(writer, await self.on_error(exc.CODE))
-                    break
-                except (TimeoutError, asyncio.TimeoutError, EOFError, IOError, asyncio.CancelledError):
-                    raise
-                except Exception as exc:
-                    await self._respond(writer, await self.on_error(HTTPStatus.INTERNAL_SERVER_ERROR))
-                    logger.info('Server error on request: %s', exc)
-                    break
-
-                try:
-                    await self._respond(writer, response)
-                    logger.debug('Response sent to "%s": %s', s_addr(peername), response)
-                except (TimeoutError, asyncio.TimeoutError, EOFError, IOError, asyncio.CancelledError):
-                    raise
-                except Exception as exc:
-                    logger.info('Server error on response: %s', exc)
-                    writer.transport.abort()
-                    break
-        except (TimeoutError, asyncio.TimeoutError, EOFError, IOError):
-            writer.transport.abort()
-        except asyncio.CancelledError:
-            logger.debug('Connection from %s has been cancelled', s_addr(peername))
-
-    async def run(self):
-        http_config = self.config['http']
-        if http_config.get('disable'):
-            return
-        http_root = http_config.get('root')
-        if http_root:
-            root_path = pathlib.Path(http_root).resolve()
-            if not root_path.is_dir():
-                raise InvalidConfig('%s is not a directory' % root_path)
-            self.root = root_path
-        else:
-            self.root = None
-        host = http_config['host']
-        port = int(http_config['port'])
-        if host != '127.0.0.1' and host != 'localhost':
-            logger.warn('HTTP server host %s is not safe', host)
-        self.timeout_sec = http_config['timeout'] / 1000
-        self._server = await asyncio.start_server(self.on_connect, host, port)
-        logger.info('HTTP serivce started')
-        logger.info('HTTP server is available at http://%s:%d/', host, port)
-
-        try:
-            async with self._server:
-                await self._server.serve_forever()
-        except asyncio.CancelledError:
-            logger.debug('HTTP serivce interrupted')
-        finally:
-            self._server.close()
-            logger.info('HTTP serivce stopped')
-
-
-async def _read_http_message(reader, max_body=None):
-    try:
-        http_header = await reader.readuntil(b'\r\n\r\n')
-    except asyncio.exceptions.LimitOverrunError as exc:
-        raise HttpHeaderTooLarge(exc)
-    with io.StringIO(http_header.decode()) as fp:
-        start_line = fp.readline()
-        headers = email.message_from_file(fp, _class=HttpMessage, policy=email.policy.HTTP)
-    body = None
-    if headers.get('Transfer-Encoding') == 'chunked':
-        with io.BytesIO() as fp:
-            while True:
-                chunk_len_ln = await reader.readuntil(b'\r\n')
-                chunk_len = int(chunk_len_ln[:-2].decode(), 16)
-                if chunk_len == 0: break
-                fp.write(await reader.readexactly(chunk_len))
-                if b'\r\n' != await reader.readexactly(2):
-                    raise HttpException('Chunked encoding error, missing CRLF')
-                if max_body and fp.tell() > max_body:
-                    raise HttpPayloadTooLarge('The size of payload is greater than %d', max_body)
-            fp.seek(0)
-            body = fp.read(-1)
-    else:
-        content_length = headers['Content-Length']
-        if content_length is not None:
-            with io.BytesIO() as fp:
-                body = await reader.readexactly(int(content_length))
-        elif headers.get('Connection') == 'close':
-            body = await reader.read()
-    return start_line, headers, body
-
-
-def parse_content_type(content_type):
-    if not content_type:
-        return ContentType(None, None, None, None)
-    directives = content_type.split(';')
-    media_type = directives.pop(0).strip().lower()
-    subitems = dict([[__.strip().lower() for __ in _.split('=', 1)] for _ in directives])
-
-    return ContentType(media_type, 
-                       subitems.get('charset'), 
-                       subitems.get('boundary'), 
-                       subitems.get('name'))
-
-
-def parse_content_disposition(content_disposition):
-    if not content_disposition:
-        return ContentDisposition(None, None, None)
-    directives = content_disposition.split(';')
-    _type = directives.pop(0).strip().lower()
-    subitems = dict([[__.strip().lower() for __ in _.split('=', 1)] for _ in directives])
-
-    return ContentType(_type, 
-                       subitems.get('name'),  
-                       subitems.get('filename'))
-
-
-def parse_uploaded_file(message, content_disposition=None):
-    if content_disposition is None:
-        content_disposition = parse_content_disposition(message.get('Content-Disposition'))
-    name = html.unescape(content_disposition.name)
-    filename = html.unescape(content_disposition.filename)
-    encoding = message.get('Content-Transfer-Encoding')
-    content_type = parse_content_type(message.get('Conent-Type'))
-    content = message.get_payload()
-    if encoding == 'base64':
-        content = base64.b64decode(content)
-    else:
-        content = content.encode()
-    return UploadedFile(filename, name, content_type, content)
-
-
-async def fetch(url, resolver, pool, proxy=None, **kwargs):
-    parsed_url = urlsplit(url)
-    hostname = parsed_url.hostname
-    if parsed_url.scheme == 'http':
-        scheme = Scheme.TCP
-        port = parsed_url.port if parsed_url.port else DEFAULT_HTTP_PORT
-    elif parsed_url.scheme == 'https':
-        scheme = Scheme.TLS
-        port = parsed_url.port if parsed_url.port else DEFAULT_HTTPS_PORT
-    else:
-        raise ValueError('Invalid url scheme %s' % (parsed_url.scheme, ))
-    try:
-        ipaddress.ip_address(hostname)
-        host = hostname
-    except ValueError:
-        dns_request = dnslib.DNSRecord.question(hostname)
-        dns_response = await resolver(dns_request)
-        if not dns_response or dns_response.header.a == 0:
-            raise HttpException('Could not resolve domain %s' % (hostname, ))
-        host = str(dns_response.rr[0].rdata)
-    if 'method' in kwargs:
-        method = HTTPMethod(kwargs['method'])
-    else:
-        method = HTTPMethod.GET
-    if method not in (HTTPMethod.GET, HTTPMethod.POST):
-        raise ValueError('Unsupported http method %s' % (method.name, ))
-    url_path = quote(parsed_url.path)
-    if parsed_url.query:
-        url_path = '%s?%s' % (url_path, parsed_url.query)
-    headers = kwargs.get('headers', [])
-
-    with await pool.connect(host, port, scheme, proxy, pooled=False) as conn:
-        if method == HTTPMethod.GET:
-            return await Client(hostname, conn).get(url_path, headers=headers)
-        else:
-            body = kwargs.get('body')
-            return await Client(hostname, conn).post(url_path, headers=headers, body=body)
-
-
-class JSONError(enum.Enum):
-    USER_DEFINED = 0, 'User defined error'
-    INVALID_JSON = 1, 'Invalid JSON entity'
-    ILLEGAL_PARAM = 2, 'Illegal user parameters'
-
-    def __new__(cls, code, message):
-        obj = object.__new__(cls)
-        obj.code = code
-        obj.message = message
-        return obj
-    
-    def to_json(self):
-        return {
-            'error': {
-                'code': self.code,
-                'message': self.message,
-            }
-        }
-
-
-def json_handler(func):
-    def _handle(self, request):
-        if not request.is_json():
-            raise HttpException()
-
-        try:
-            return func(self, **request.json())
-        except TypeError:
-            return JsonResponse(JSONError.INVALID_JSON, HTTPStatus.BAD_REQUEST)
-    return _handle
-
-
-def async_json_handler(func):
-    async def _handle(self, request):
-        if not request.is_json():
-            raise HttpException()
-
-        try:
-            return await func(self, **request.json())
-        except TypeError:
-            return JsonResponse(JSONError.INVALID_JSON, HTTPStatus.BAD_REQUEST)
-    return _handle
-
-
-def response_json_error(message, code=JSONError.USER_DEFINED.code):
-    return JsonResponse({
-        'error': {
-            'code': code,
-            'message': str(message),
-        }
-    })
-
-def response_json_result(result):
-    return JsonResponse({
-        'result': result
-    })
+import asyncio
+import base64
+import io
+import json
+import logging
+import enum
+import email
+import email.policy
+import mimetypes
+import html
+import pathlib
+import random
+import ipaddress
+import dnslib
+
+from collections import namedtuple
+from http import HTTPStatus
+from http.client import HTTPMessage
+from urllib.parse import urlencode, urlsplit, parse_qs, quote
+
+from .exceptions import HttpException, HttpHeaderTooLarge, HttpPayloadTooLarge, InvalidConfig
+from .helpers import s_addr, Scheme, JsonEncoder
+
+
+HTTP_VERSION = 'HTTP/1.1'
+
+DEFAULT_HTTP_PORT = 80
+
+DEFAULT_HTTPS_PORT = 443
+
+
+logger = logging.getLogger(__name__)
+
+ContentType = namedtuple('ContentType', ['media_type', 'charset', 'boundary', 'name'])
+
+ContentDisposition = namedtuple('ContentDisposition', ['type', 'name', 'filename'])
+
+UploadedFile = namedtuple('UploadedFile', ['filename', 'name', 'content_type', 'content'])
+
+
+class HTTPMethod(str, enum.Enum):
+    CONNECT = 'CONNECT'
+    DELETE = 'DELETE'
+    GET = 'GET'
+    HEAD = 'HEAD'
+    OPTIONS = 'OPTIONS'
+    PATCH = 'PATCH'
+    POST = 'POST'
+    PUT = 'PUT'
+    TRACE = 'TRACE'
+
+    def __str__(self):
+        return self.value
+
+
+class HttpMessage(HTTPMessage):
+    def get_content_maintype(self):
+        maintype = super().get_content_maintype()
+        if maintype == 'multipart':
+            return ''
+        return maintype
+
+    def set_header(self, name, value, **params):
+        if self.get(name):
+            del self[name]
+        return self.add_header(name, str(value), **params)
+
+    def is_closing(self):
+        return self.get('Connection', '').lower() == 'close'
+
+
+class FormData:
+    def __init__(self):
+        self.data = []
+        self.boundary = self._generate_boundary()
+
+    def _generate_boundary(self):
+        alphabet = '0123456789qwertyuiopasdfghjklzxcvbnmQWERTYUIOPASDFGHJKLZXCVBNM'
+        extra_tail = ''.join(random.sample(alphabet, 16))
+        return '----WebKitFormBoundary' + extra_tail
+
+    def get_boundary(self):
+        return self.boundary
+
+    def append(self, name, value):
+        self.data.append((name, value))
+        return self
+
+    def as_bytes(self):
+        with io.BytesIO() as fp:
+            for item in self.data:
+                key, value = item
+                fp.write(b'--')
+                fp.write(self.boundary.encode())
+                fp.write(b'\r\n')
+                fp.write(b'Content-Disposition: form-data; name="%s"\r\n' %(html.escape(key).encode(), ))
+                fp.write(b'\r\n')
+                fp.write(html.escape(value).encode())
+                fp.write(b'\r\n')
+            fp.write(b'--')
+            fp.write(self.boundary.encode())
+            fp.write(b'--\r\n')
+            fp.seek(0)
+            return fp.read(-1)
+
+
+class Request:
+    def get(self, name, default=None):
+        if self.query and name in self.query:
+            return self.query[name][0]
+        if self.form and name in self.form:
+            return self.form[name][0]
+        return default
+    
+    def get_int(self, name, default=0):
+        try:
+            return int(self.get(name))
+        except TypeError:
+            return default
+
+    def get_list(self, name, default=[]):
+        value = self.get(name)
+        if isinstance(value, list):
+            return value
+        elif value is not None:
+            return [value]
+        return default
+
+    def get_all(self, name):
+        if self.query and name in self.query:
+            return self.query[name]
+        if self.form and name in self.form:
+            return self.form[name]
+        return []
+    
+    def is_json(self):
+        return self._is_json
+
+    def json(self):
+        if not self.is_json():
+            return
+        try:
+            return json.loads(self._body)
+        except json.JSONDecodeError:
+            pass
+
+    @property
+    def body(self):
+        return self._body
+
+    def _parse_post_data(self, body):
+        raw_content_type = self.headers.get('Conetent-Type')
+        with io.BytesIO() as fp:
+            fp.write(b'Content-Type: ')
+            fp.write(raw_content_type.encode())
+            fp.write(b'\r\n\r\n')
+            fp.write(body)
+            form_data = email.message_from_binary_file(
+                fp, _class=HttpMessage, policy=email.policy.HTTP).get_payload()
+        if not form_data: return
+        form = dict()
+        files = dict()
+        for item in form_data:
+            content_disposition = parse_content_disposition(item.get('Content-Disposition'))
+            if content_disposition.type == 'form-data' and content_disposition.name:
+                if content_disposition.filename:
+                    uploaded_file = parse_uploaded_file(item, content_disposition)
+                    if content_disposition.name in files:
+                        files[content_disposition.name].append(uploaded_file)
+                    else:
+                        files[content_disposition.name] = [uploaded_file]
+                else:
+                    if content_disposition.name in form:
+                        form[content_disposition.name].append(item.get_payload())
+                    else:
+                        form[content_disposition.name] = [item.get_payload()]
+        self.form = form
+        self.files = files
+
+    @body.setter
+    def body(self, value):
+        if value is None: return
+        if not isinstance(value, bytes):
+            raise TypeError('Response body must be bytes type, %s given' % (type(value), ))
+
+        raw_content_type = self.headers.get('Content-Type')
+        content_type = parse_content_type(raw_content_type)
+        media_type = content_type.media_type
+        charset = content_type.charset
+        if media_type == 'applicaton/x-www-urlencoded':
+            decoded_body = value.decode(charset) if charset \
+                else value.decode(charset)
+            self.form = parse_qs(decoded_body)
+        elif media_type == 'multipart/form-data':
+            self._parse_post_data(value)
+        elif media_type == 'application/json':
+            self._is_json = True
+        self._body = value
+
+    def __init__(self):
+        self.method = None
+        self._url = None
+        self.version = HTTP_VERSION
+        self.headers = HttpMessage(email.policy.HTTP)
+        self._body = None
+        self._is_json = False
+        self.query_string = None
+        self.path = None
+        self.query = None
+        self.form = None
+        self.files = None
+
+    @property
+    def url(self):
+        return self._url
+
+    @url.setter
+    def url(self, value):
+        parsed_url = urlsplit(value)
+        self._url = value
+        self.path = quote(parsed_url.path)
+        if parsed_url.query:
+            self.query_string = parsed_url.query
+            self.query = parse_qs(parsed_url.query)
+        else:
+            self.query_string = ''
+            self.query = dict()
+
+    def __repr__(self):
+        if self.method is None or self.url is None:
+            return '<%s>' % self.__class__.__name__
+        return '<%s: %s %r>' % (
+            self.__class__.__name__,
+            self.method,
+            self.url,
+        )
+
+
+class Response:
+    def __init__(self, status=HTTPStatus.OK, body=None):
+        if not isinstance(status, HTTPStatus):
+            status = HTTPStatus(status)
+        if isinstance(body, str):
+            body = body.encode()
+        self._status = status
+        self.is_sent = False
+        self.reason = self._status.name
+        self.version = HTTP_VERSION
+        self.headers = HttpMessage(email.policy.HTTP)
+        self.body = body
+
+    @property
+    def status(self):
+        return self._status
+
+    @status.setter
+    def status(self, value):
+        if not isinstance(value, HTTPStatus):
+            value = HTTPStatus(value)
+        self._status = value
+        self.reason = value.name
+
+    def __repr__(self):
+        return "<%(cls)s status=%(status)d type=%(type)s length=%(len)s>" % {
+            'cls': self.__class__.__name__,
+            'status': self.status,
+            'len': len(self.body),
+            'type': self.headers.get('Content-Type'),
+        }
+
+
+class FileResponse(Response):
+    def __init__(self, file, status=HTTPStatus.OK):
+        super().__init__(status)
+        self.file = file
+
+    @property
+    def size(self):
+        return self.file.stat().st_size
+
+    def __repr__(self):
+        return "<%(cls)s status=%(status)d type=%(type)s length=%(len)s>" % {
+            'cls': self.__class__.__name__,
+            'status': self.status,
+            'len': self.size,
+            'type': self.headers.get('Content-Type'),
+        }
+
+
+class JsonResponse(Response):
+    def __init__(self, payload, status=HTTPStatus.OK):
+        super().__init__(status)
+        self.body = json.dumps(payload, cls=JsonEncoder).encode()
+        self.headers.add_header('Content-Type', 'application/json', charset='utf-8')
+
+    def __repr__(self):
+        return "<%(cls)s status=%(status)d type=%(type)s length=%(len)s>" % {
+            'cls': self.__class__.__name__,
+            'status': self.status,
+            'len': len(self.body),
+            'type': self.headers.get('Content-Type'),
+        }
+
+
+class Client:
+    def __init__(self, hostname, conn):
+        self.hostname = hostname
+        self.conn = conn
+
+    def prepare_headers(self, headers):
+        return headers + [
+            ('Host', self.hostname),
+            ('Accept-Encoding', 'identity'),
+            ('Connection', 'keep-alive'),
+        ]
+
+    def build_request(self, method, path, query, headers, body=None):
+        req = Request()
+        req.method = method
+        req.url = '%s?%s' % (path, urlencode(query)) if query else path
+        for hdr in headers:
+            req.headers.add_header(*hdr)
+        if isinstance(body, dict):
+            req.headers.set_header('Content-Type', 'application/x-www-form-urlencoded')
+            body = urlencode(body).encode()
+        elif isinstance(body, FormData):
+            req.headers.set_header('Content-Type', 'multipart/form-data', boundary=body.get_boundary())
+            body = body.as_bytes()
+        req.body = body
+        return req
+
+    async def _request(self, request):
+        writer = self.conn.writer
+        start_line = '%s %s %s\r\n' % (request.method, request.url, request.version)
+        writer.write(start_line.encode())
+        if request.body:
+            request.headers.set_header('Content-Length', len(request.body))
+            writer.write(request.headers.as_bytes())
+            writer.write(request.body)
+        else:
+            del request.headers['Content-Length']
+            writer.write(request.headers.as_bytes())
+
+        try:
+            await writer.drain()
+        except Exception as exc:
+            raise HttpException(str(exc))
+
+    async def _read_response(self):
+        resp = Response()
+        try:
+            start_line, resp.headers, resp.body = await _read_http_message(self.conn.reader)
+            resp.version, status, resp.reason = start_line.split(' ', 2)
+            resp.status = HTTPStatus(int(status))
+        except (HttpException, asyncio.CancelledError) as exc:
+            raise exc
+        except:
+            raise HttpException('Invalid response')
+        return resp
+
+    async def get(self, path, query=None, headers=[]):
+        request = self.build_request(HTTPMethod.GET, path, query, self.prepare_headers(headers))
+        logger.debug('Request sent to "%s": %s', self.hostname, request)
+        await self._request(request)
+        response = await self._read_response()
+        logger.debug('Response received from "%s": %s', self.hostname, response)
+        return response
+
+    async def post(self, path, query=None, headers=[], body=None):
+        request = self.build_request(HTTPMethod.POST, path, query, self.prepare_headers(headers), body)
+        logger.debug('Request sent to "%s": %s', self.hostname, request)
+        await self._request(request)
+        response = await self._read_response()
+        logger.debug('Response received from "%s": %s', self.hostname, response)
+        return response
+
+
+class Server:
+    MAX_REQUEST_SIZE = 1024 * 1024 * 16
+
+    DEFAULT_FILES = ['index.html', 'index.htm', 'default.htm', 'default.html']
+
+    def __init__(self, config, handler=None, loop=None):
+        self.loop = asyncio.get_running_loop() if loop is None else loop
+        self.config = config
+        self._request_handler = self._create_request_handler(handler)
+        self._server = None
+        logger.debug('HTTP serivce initialized')
+    
+    def _create_request_handler(self, handler):
+        if hasattr(handler, 'handle'):
+            async def _handler(req):
+                return await handler.handle(req)
+        elif callable(handler):
+            async def _handler(req):
+                return await handler(req)
+        else:
+            async def _handler(req):
+                return await self.on_error(404)
+        return _handler
+
+    async def _respond(self, writer, response):
+        try:
+            response.headers.add_header('Server', __package__)
+            start_line = '%s %d %s\r\n' % (response.version, response.status.value, response.status.phrase)
+            writer.write(start_line.encode())
+            if isinstance(response, FileResponse):
+                ctype, charset = mimetypes.guess_type(response.file)
+                kwargs = {} if charset is None else {'charset': charset}
+                response.headers.set_header(
+                    'Content-Type', 
+                    'application/octet-stream' if ctype is None else ctype,
+                    **kwargs
+                )
+                with response.file.open('rb') as fp:
+                    response.headers.set_header('Content-Length', response.size)
+                    writer.write(response.headers.as_bytes())
+                    await writer.drain()
+                    await self.loop.sendfile(writer.transport, fp)
+                response.is_sent = True
+                return response
+            elif response.body:
+                response.headers.set_header('Content-Length', len(response.body))
+                writer.write(response.headers.as_bytes())
+                writer.write(response.body)
+            else:
+                del response.headers['Content-Length']
+                writer.write(response.headers.as_bytes())
+            await writer.drain()
+            response.is_sent = True
+        except asyncio.CancelledError:
+            raise
+        except:
+            raise IOError('Response begin sending and an error occurred')
+        finally:
+            if response.headers.is_closing():
+                writer.transport.abort()
+        return response
+        
+    async def _read_request(self, reader):
+        req = Request()
+        try:
+            start_line, req.headers, req.body = await _read_http_message(reader, self.MAX_REQUEST_SIZE)
+            method, req.url, req.version = start_line.split(' ', 2)
+            req.method = HTTPMethod(method)
+        except (HttpException, asyncio.CancelledError):
+            raise
+        except:
+            raise HttpException('Invalid request')
+        return req
+
+    def _attempt_static_file(self, path):
+        if not self.root:
+            return False
+
+        file_path = self.root.joinpath('.' + path).resolve()
+        if not str(file_path).startswith(str(self.root)):
+            return False
+
+        if file_path.is_dir():
+            for default_file in self.DEFAULT_FILES:
+                file_path = file_path.joinpath(default_file)
+                if file_path.exists():
+                    return file_path
+        elif file_path.exists():
+            return file_path
+
+        return False
+
+    async def on_request(self, request):
+        static_file = self._attempt_static_file(request.path)
+        if static_file:
+            return FileResponse(static_file)
+        return await (self._request_handler)(request)
+
+    async def on_error(self, status, body=None):
+        resp = Response(status)
+        resp.headers.add_header('Connection', 'close')
+        resp.body = body
+        return resp
+
+    async def on_connect(self, reader, writer):
+        peername = writer.transport.get_extra_info('peername')
+        logger.debug('Connection from %s', s_addr(peername))
+        try:
+            while not writer.transport.is_closing():
+                try:
+                    request = await asyncio.wait_for(self._read_request(reader), self.timeout_sec)
+                    logger.debug('Request received from "%s": %s', s_addr(peername), request)
+                    response = await self.on_request(request)
+                except HttpException as exc:
+                    await self._respond(writer, await self.on_error(exc.CODE))
+                    break
+                except (TimeoutError, asyncio.TimeoutError, EOFError, IOError, asyncio.CancelledError):
+                    raise
+                except Exception as exc:
+                    await self._respond(writer, await self.on_error(HTTPStatus.INTERNAL_SERVER_ERROR))
+                    logger.info('Server error on request: %s', exc)
+                    break
+
+                try:
+                    await self._respond(writer, response)
+                    logger.debug('Response sent to "%s": %s', s_addr(peername), response)
+                except (TimeoutError, asyncio.TimeoutError, EOFError, IOError, asyncio.CancelledError):
+                    raise
+                except Exception as exc:
+                    logger.info('Server error on response: %s', exc)
+                    writer.transport.abort()
+                    break
+        except (TimeoutError, asyncio.TimeoutError, EOFError, IOError):
+            writer.transport.abort()
+        except asyncio.CancelledError:
+            logger.debug('Connection from %s has been cancelled', s_addr(peername))
+
+    async def run(self):
+        http_config = self.config['http']
+        if http_config.get('disable'):
+            return
+        http_root = http_config.get('root')
+        if http_root:
+            root_path = pathlib.Path(http_root).resolve()
+            if not root_path.is_dir():
+                raise InvalidConfig('%s is not a directory' % root_path)
+            self.root = root_path
+        else:
+            self.root = None
+        host = http_config['host']
+        port = int(http_config['port'])
+        if host != '127.0.0.1' and host != 'localhost':
+            logger.warn('HTTP server host %s is not safe', host)
+        self.timeout_sec = http_config['timeout'] / 1000
+        self._server = await asyncio.start_server(self.on_connect, host, port)
+        logger.info('HTTP serivce started')
+        logger.info('HTTP server is available at http://%s:%d/', host, port)
+
+        try:
+            async with self._server:
+                await self._server.serve_forever()
+        except asyncio.CancelledError:
+            logger.debug('HTTP serivce interrupted')
+        finally:
+            self._server.close()
+            logger.info('HTTP serivce stopped')
+
+
+async def _read_http_message(reader, max_body=None):
+    try:
+        http_header = await reader.readuntil(b'\r\n\r\n')
+    except asyncio.exceptions.LimitOverrunError as exc:
+        raise HttpHeaderTooLarge(exc)
+    with io.StringIO(http_header.decode()) as fp:
+        start_line = fp.readline()
+        headers = email.message_from_file(fp, _class=HttpMessage, policy=email.policy.HTTP)
+    body = None
+    if headers.get('Transfer-Encoding') == 'chunked':
+        with io.BytesIO() as fp:
+            while True:
+                chunk_len_ln = await reader.readuntil(b'\r\n')
+                chunk_len = int(chunk_len_ln[:-2].decode(), 16)
+                if chunk_len == 0: break
+                fp.write(await reader.readexactly(chunk_len))
+                if b'\r\n' != await reader.readexactly(2):
+                    raise HttpException('Chunked encoding error, missing CRLF')
+                if max_body and fp.tell() > max_body:
+                    raise HttpPayloadTooLarge('The size of payload is greater than %d', max_body)
+            fp.seek(0)
+            body = fp.read(-1)
+    else:
+        content_length = headers['Content-Length']
+        if content_length is not None:
+            with io.BytesIO() as fp:
+                body = await reader.readexactly(int(content_length))
+        elif headers.get('Connection') == 'close':
+            body = await reader.read()
+    return start_line, headers, body
+
+
+def parse_content_type(content_type):
+    if not content_type:
+        return ContentType(None, None, None, None)
+    directives = content_type.split(';')
+    media_type = directives.pop(0).strip().lower()
+    subitems = dict([[__.strip().lower() for __ in _.split('=', 1)] for _ in directives])
+
+    return ContentType(media_type, 
+                       subitems.get('charset'), 
+                       subitems.get('boundary'), 
+                       subitems.get('name'))
+
+
+def parse_content_disposition(content_disposition):
+    if not content_disposition:
+        return ContentDisposition(None, None, None)
+    directives = content_disposition.split(';')
+    _type = directives.pop(0).strip().lower()
+    subitems = dict([[__.strip().lower() for __ in _.split('=', 1)] for _ in directives])
+
+    return ContentType(_type, 
+                       subitems.get('name'),  
+                       subitems.get('filename'))
+
+
+def parse_uploaded_file(message, content_disposition=None):
+    if content_disposition is None:
+        content_disposition = parse_content_disposition(message.get('Content-Disposition'))
+    name = html.unescape(content_disposition.name)
+    filename = html.unescape(content_disposition.filename)
+    encoding = message.get('Content-Transfer-Encoding')
+    content_type = parse_content_type(message.get('Conent-Type'))
+    content = message.get_payload()
+    if encoding == 'base64':
+        content = base64.b64decode(content)
+    else:
+        content = content.encode()
+    return UploadedFile(filename, name, content_type, content)
+
+
+async def fetch(url, resolver, pool, proxy=None, **kwargs):
+    parsed_url = urlsplit(url)
+    hostname = parsed_url.hostname
+    if parsed_url.scheme == 'http':
+        scheme = Scheme.TCP
+        port = parsed_url.port if parsed_url.port else DEFAULT_HTTP_PORT
+    elif parsed_url.scheme == 'https':
+        scheme = Scheme.TLS
+        port = parsed_url.port if parsed_url.port else DEFAULT_HTTPS_PORT
+    else:
+        raise ValueError('Invalid url scheme %s' % (parsed_url.scheme, ))
+    try:
+        ipaddress.ip_address(hostname)
+        host = hostname
+    except ValueError:
+        dns_request = dnslib.DNSRecord.question(hostname)
+        dns_response = await resolver(dns_request)
+        if not dns_response or dns_response.header.a == 0:
+            raise HttpException('Could not resolve domain %s' % (hostname, ))
+        host = str(dns_response.rr[0].rdata)
+    if 'method' in kwargs:
+        method = HTTPMethod(kwargs['method'])
+    else:
+        method = HTTPMethod.GET
+    if method not in (HTTPMethod.GET, HTTPMethod.POST):
+        raise ValueError('Unsupported http method %s' % (method.name, ))
+    url_path = quote(parsed_url.path)
+    if parsed_url.query:
+        url_path = '%s?%s' % (url_path, parsed_url.query)
+    headers = kwargs.get('headers', [])
+
+    with await pool.connect(host, port, scheme, proxy, pooled=False) as conn:
+        if method == HTTPMethod.GET:
+            return await Client(hostname, conn).get(url_path, headers=headers)
+        else:
+            body = kwargs.get('body')
+            return await Client(hostname, conn).post(url_path, headers=headers, body=body)
+
+
+class JSONError(enum.Enum):
+    USER_DEFINED = 0, 'User defined error'
+    INVALID_JSON = 1, 'Invalid JSON entity'
+    ILLEGAL_PARAM = 2, 'Illegal user parameters'
+
+    def __new__(cls, code, message):
+        obj = object.__new__(cls)
+        obj.code = code
+        obj.message = message
+        return obj
+    
+    def to_json(self):
+        return {
+            'error': {
+                'code': self.code,
+                'message': self.message,
+            }
+        }
+
+
+def json_handler(func):
+    def _handle(self, request):
+        if not request.is_json():
+            raise HttpException()
+
+        try:
+            return func(self, **request.json())
+        except TypeError:
+            return JsonResponse(JSONError.INVALID_JSON, HTTPStatus.BAD_REQUEST)
+    return _handle
+
+
+def async_json_handler(func):
+    async def _handle(self, request):
+        if not request.is_json():
+            raise HttpException()
+
+        try:
+            return await func(self, **request.json())
+        except TypeError:
+            return JsonResponse(JSONError.INVALID_JSON, HTTPStatus.BAD_REQUEST)
+    return _handle
+
+
+def response_json_error(message, code=JSONError.USER_DEFINED.code):
+    return JsonResponse({
+        'error': {
+            'code': code,
+            'message': str(message),
+        }
+    })
+
+def response_json_result(result):
+    return JsonResponse({
+        'result': result
+    })
```

### Comparing `dnspooh-1.3.1/dnspooh/middlewares/block.py` & `dnspooh-1.3.2/dnspooh/middlewares/block.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import logging
-import dnslib
-import functools
-import ipaddress
-
-from . import Middleware, load_config
-from .. import timers
-from ..exceptions import InvalidConfig
-from ..helpers import split_domain
-
-
-logger = logging.getLogger(__name__)
-
-
-def _nxdomain(request):
-    response = request.reply()
-    response.header.rcode = dnslib.RCODE.NXDOMAIN
-    return response
-
-
-def _parse_config(fp):
-    domain_blacklist = set()
-    ip_blacklist = set()
-
-    for ln in fp:
-        ln = ln.strip()
-        if ln == '' or ln.startswith('#'):
-            continue
-        
-        if ln.startswith('ip:'):
-            ip_blacklist.add(ipaddress.ip_address(ln[3:].strip()))
-        else:
-            domain_blacklist.add(ln)
-    return domain_blacklist, ip_blacklist
-
-
-class BlockMiddleware(Middleware):
-    async def load_config(self, filename):
-        try:
-            self.blacklists[filename] = await load_config(filename, self.server, _parse_config)
-        except Exception as exc:
-            logger.warning('Failed to load blacklist "%s": %s', filename, exc)
-            return False
-        logger.info('Blacklist "%s" loaded', filename)
-        return True
-
-    def is_loaded(self, filename):
-        return filename in self.blacklists
-
-    async def bootstrap(self):
-        if not await super().bootstrap():
-            return False
-        for _file in self.filenames:
-            if isinstance(_file, list):
-                filename, refresh_interval = _file
-                if not self.is_loaded(filename):
-                    self.server.create_scheduled_task(
-                        functools.partial(self.load_config, filename),
-                        timers.Timer(refresh_interval), 
-                        '[SCHEDULE] fetching blacklist %s' % (filename, )
-                    )
-            else:
-                filename = _file
-            if self.is_loaded(filename):
-                raise InvalidConfig('Duplicate blacklist %s' % (filename, ))
-            await self.load_config(filename)
-        return True
-
-    def __init__(self, *filenames):
-        self.blacklists = dict()
-        self.filenames = filenames
-
-    async def handle(self, request, **kwargs):
-        if request.q.qtype not in (dnslib.QTYPE.A, dnslib.QTYPE.AAAA):
-            return await super().handle(request, **kwargs)
-
-        domain_parts = list(split_domain(request.q.qname.idna().rstrip('.')))
-        for blacklist, _ in self.blacklists.values():
-            for part in domain_parts:
-                if part in blacklist:
-                    return _nxdomain(request)
-
-        response = await super().handle(request, **kwargs)
-        if response is None: return
-
-        for rr in filter(lambda rr: rr.rtype in (dnslib.QTYPE.A, dnslib.QTYPE.AAAA), response.rr):
-            ip_addr = ipaddress.ip_address(str(rr.rdata))
-            for _, blacklist in self.blacklists.values():
-                if ip_addr in blacklist:
-                    return _nxdomain(request)
-
-        return response
+import logging
+import dnslib
+import functools
+import ipaddress
+
+from . import Middleware, load_config
+from .. import timers
+from ..exceptions import InvalidConfig
+from ..helpers import split_domain
+
+
+logger = logging.getLogger(__name__)
+
+
+def _nxdomain(request):
+    response = request.reply()
+    response.header.rcode = dnslib.RCODE.NXDOMAIN
+    return response
+
+
+def _parse_config(fp):
+    domain_blacklist = set()
+    ip_blacklist = set()
+
+    for ln in fp:
+        ln = ln.strip()
+        if ln == '' or ln.startswith('#'):
+            continue
+        
+        if ln.startswith('ip:'):
+            ip_blacklist.add(ipaddress.ip_address(ln[3:].strip()))
+        else:
+            domain_blacklist.add(ln)
+    return domain_blacklist, ip_blacklist
+
+
+class BlockMiddleware(Middleware):
+    async def load_config(self, filename):
+        try:
+            self.blacklists[filename] = await load_config(filename, self.server, _parse_config)
+        except Exception as exc:
+            logger.warning('Failed to load blacklist "%s": %s', filename, exc)
+            return False
+        logger.info('Blacklist "%s" loaded', filename)
+        return True
+
+    def is_loaded(self, filename):
+        return filename in self.blacklists
+
+    async def bootstrap(self):
+        if not await super().bootstrap():
+            return False
+        for _file in self.filenames:
+            if isinstance(_file, list):
+                filename, refresh_interval = _file
+                if not self.is_loaded(filename):
+                    self.server.create_scheduled_task(
+                        functools.partial(self.load_config, filename),
+                        timers.Timer(refresh_interval), 
+                        '[SCHEDULE] fetching blacklist %s' % (filename, )
+                    )
+            else:
+                filename = _file
+            if self.is_loaded(filename):
+                raise InvalidConfig('Duplicate blacklist %s' % (filename, ))
+            await self.load_config(filename)
+        return True
+
+    def __init__(self, *filenames):
+        self.blacklists = dict()
+        self.filenames = filenames
+
+    async def handle(self, request, **kwargs):
+        if request.q.qtype not in (dnslib.QTYPE.A, dnslib.QTYPE.AAAA):
+            return await super().handle(request, **kwargs)
+
+        domain_parts = list(split_domain(request.q.qname.idna().rstrip('.')))
+        for blacklist, _ in self.blacklists.values():
+            for part in domain_parts:
+                if part in blacklist:
+                    return _nxdomain(request)
+
+        response = await super().handle(request, **kwargs)
+        if response is None: return
+
+        for rr in filter(lambda rr: rr.rtype in (dnslib.QTYPE.A, dnslib.QTYPE.AAAA), response.rr):
+            ip_addr = ipaddress.ip_address(str(rr.rdata))
+            for _, blacklist in self.blacklists.values():
+                if ip_addr in blacklist:
+                    return _nxdomain(request)
+
+        return response
```

### Comparing `dnspooh-1.3.1/dnspooh/middlewares/hosts.py` & `dnspooh-1.3.2/dnspooh/middlewares/hosts.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-import logging
-import ipaddress
-import dnslib
-import functools
-
-from . import Middleware, load_config
-from ..exceptions import InvalidConfig
-from .. import timers
-
-
-logger = logging.getLogger(__name__)
-
-
-def _parse_config(fp):
-    hosts = dict()
-    line_no = 1
-
-    for ln in fp:
-        ln = ln.lstrip()
-        if ln == '' or ln.startswith('#'):
-            continue
-        _addr, _hostname = ln.split(' ', 1)
-        addr = _addr.strip()
-        hostname = _hostname.strip()
-        try:
-            ip_addr = ipaddress.ip_address(addr)
-        except ValueError:
-            raise InvalidConfig('Invalid ip address %s in line %d' % (addr, line_no))
-        if hostname in hosts:
-            hosts[hostname].append(ip_addr)
-        else:
-            hosts[hostname] = [ip_addr]
-        line_no += 1
-    return hosts
-
-
-class HostsMiddleware(Middleware):
-    DEFAULT_TTL = 60
-
-    async def load_config(self, filename):
-        try:
-            self.hosts[filename] = await load_config(filename, self.server, _parse_config)
-        except Exception as exc:
-            logger.warning('Failed to load hosts file "%s": %s', filename, exc)
-            return False
-        logger.info('Hosts file "%s" loaded', filename)
-        return True
-
-    def is_loaded(self, filename):
-        return filename in self.hosts
-
-    async def bootstrap(self):
-        if not await super().bootstrap():
-            return False
-        for _file in self.filenames:
-            if isinstance(_file, list):
-                filename, refresh_interval = _file
-                self.server.create_scheduled_task(
-                    functools.partial(self.load_config, filename),
-                    timers.Timer(refresh_interval), 
-                    '[SCHEDULE] fetching hosts file %s' % (filename, )
-                )
-            else:
-                filename = _file
-            if not self.is_loaded(filename):
-                await self.load_config(filename)
-            else:
-                raise InvalidConfig('Duplicate hosts file %s' % (filename, ))
-        return True
-
-    def __init__(self, *filenames):
-        self.hosts = dict()
-        self.files = []
-        self.urls = []
-        self.filenames = filenames
-
-    def query(self, request):
-        hostname = request.q.qname.idna().rstrip('.')
-        qtype = request.q.qtype
-        response = request.reply()
-        for hosts in self.hosts.values():
-            if hostname not in hosts:
-                continue
-            ip_addrs = hosts[hostname]
-            for r in ip_addrs:
-                if isinstance(r, ipaddress.IPv6Address) and qtype == dnslib.QTYPE.AAAA:
-                    response.add_answer(dnslib.RR(
-                        hostname, qtype, 
-                        rdata=dnslib.AAAA(str(r)), 
-                        ttl=self.DEFAULT_TTL
-                    ))
-                elif isinstance(r, ipaddress.IPv4Address) and qtype == dnslib.QTYPE.A:
-                    response.add_answer(dnslib.RR(
-                        hostname, qtype, 
-                        rdata=dnslib.A(str(r)), 
-                        ttl=self.DEFAULT_TTL
-                    ))
-        return response if response.header.a > 0 else None
-
-    async def handle(self, request, **kwargs):
-        if request.q.qtype not in (dnslib.QTYPE.A, dnslib.QTYPE.AAAA):
-            return await super().handle(request, **kwargs)
-        response = self.query(request)
-        if not response:
-            return await super().handle(request, **kwargs)
-
-        return response
+import logging
+import ipaddress
+import dnslib
+import functools
+
+from . import Middleware, load_config
+from ..exceptions import InvalidConfig
+from .. import timers
+
+
+logger = logging.getLogger(__name__)
+
+
+def _parse_config(fp):
+    hosts = dict()
+    line_no = 1
+
+    for ln in fp:
+        ln = ln.lstrip()
+        if ln == '' or ln.startswith('#'):
+            continue
+        _addr, _hostname = ln.split(' ', 1)
+        addr = _addr.strip()
+        hostname = _hostname.strip()
+        try:
+            ip_addr = ipaddress.ip_address(addr)
+        except ValueError:
+            raise InvalidConfig('Invalid ip address %s in line %d' % (addr, line_no))
+        if hostname in hosts:
+            hosts[hostname].append(ip_addr)
+        else:
+            hosts[hostname] = [ip_addr]
+        line_no += 1
+    return hosts
+
+
+class HostsMiddleware(Middleware):
+    DEFAULT_TTL = 60
+
+    async def load_config(self, filename):
+        try:
+            self.hosts[filename] = await load_config(filename, self.server, _parse_config)
+        except Exception as exc:
+            logger.warning('Failed to load hosts file "%s": %s', filename, exc)
+            return False
+        logger.info('Hosts file "%s" loaded', filename)
+        return True
+
+    def is_loaded(self, filename):
+        return filename in self.hosts
+
+    async def bootstrap(self):
+        if not await super().bootstrap():
+            return False
+        for _file in self.filenames:
+            if isinstance(_file, list):
+                filename, refresh_interval = _file
+                self.server.create_scheduled_task(
+                    functools.partial(self.load_config, filename),
+                    timers.Timer(refresh_interval), 
+                    '[SCHEDULE] fetching hosts file %s' % (filename, )
+                )
+            else:
+                filename = _file
+            if not self.is_loaded(filename):
+                await self.load_config(filename)
+            else:
+                raise InvalidConfig('Duplicate hosts file %s' % (filename, ))
+        return True
+
+    def __init__(self, *filenames):
+        self.hosts = dict()
+        self.files = []
+        self.urls = []
+        self.filenames = filenames
+
+    def query(self, request):
+        hostname = request.q.qname.idna().rstrip('.')
+        qtype = request.q.qtype
+        response = request.reply()
+        for hosts in self.hosts.values():
+            if hostname not in hosts:
+                continue
+            ip_addrs = hosts[hostname]
+            for r in ip_addrs:
+                if isinstance(r, ipaddress.IPv6Address) and qtype == dnslib.QTYPE.AAAA:
+                    response.add_answer(dnslib.RR(
+                        hostname, qtype, 
+                        rdata=dnslib.AAAA(str(r)), 
+                        ttl=self.DEFAULT_TTL
+                    ))
+                elif isinstance(r, ipaddress.IPv4Address) and qtype == dnslib.QTYPE.A:
+                    response.add_answer(dnslib.RR(
+                        hostname, qtype, 
+                        rdata=dnslib.A(str(r)), 
+                        ttl=self.DEFAULT_TTL
+                    ))
+        return response if response.header.a > 0 else None
+
+    async def handle(self, request, **kwargs):
+        if request.q.qtype not in (dnslib.QTYPE.A, dnslib.QTYPE.AAAA):
+            return await super().handle(request, **kwargs)
+        response = self.query(request)
+        if not response:
+            return await super().handle(request, **kwargs)
+
+        return response
```

### Comparing `dnspooh-1.3.1/dnspooh/middlewares/log.py` & `dnspooh-1.3.2/dnspooh/middlewares/log.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-import logging
-import sqlite3
-import time
-import json
-
-import dnslib
-
-from . import Middleware, Traceback
-from ..helpers import prepare_path
-
-
-logger = logging.getLogger(__name__)
-
-
-CREATE_DATABASE_SQL = \
-'''CREATE TABLE IF NOT EXISTS "log" (
-    "id"            INTEGER,
-    "created_at"    TEXT,
-    "elapsed_time"  REAL,
-    "qname"         TEXT,
-    "qtype"         TEXT,
-    "success"       INTEGER,
-    "request"       BLOB,
-    "response"      BLOB,
-    "traceback"     TEXT,
-    "error"         TEXT,
-    PRIMARY KEY("id" AUTOINCREMENT)
-);
-'''
-
-INSERT_FAILURE_SQL = \
-'''INSERT INTO "log" 
-    (created_at, elapsed_time, qname, qtype, success, request, error, traceback) 
-    VALUES 
-    (:now, :elapsed_time, :qname, :qtype, :success, :request, :error, :traceback)
-'''
-
-INSERT_SUCCESS_SQL = \
-'''INSERT INTO "log" 
-    (created_at, elapsed_time, qname, qtype, success, request, response, traceback) 
-    VALUES 
-    (:now, :elapsed_time, :qname, :qtype, :success, :request, :response, :traceback)
-'''
-
-SELECT_DATASET_SQL = \
-'''SELECT id, created_at, elapsed_time, qname, qtype, success, traceback, error 
-    FROM "log" {where} ORDER BY id DESC LIMIT :offset, :page_size
-'''
-
-COUNT_DATASET_SQL = 'SELECT COUNT(*) FROM "log" {where}'
-
-TRUNCATE_TABLE_SQL = 'DELETE FROM "log"'
-
-QUERY_PAGE_SIZE = 50
-
-
-class Query:
-    def __init__(self, sql):
-        self.sql = sql
-        self.conditions = []
-        self.params = dict()
-
-    def where(self, expr, **kwargs):
-        self.params |= kwargs
-        placeholders = { key: ':%s' % key for key in kwargs.keys() }
-        self.conditions.append(expr.format(**placeholders))
-
-    def __repr__(self):
-        if not self.conditions:
-            return ''
-        return 'WHERE ' + ' AND '.join(self.conditions)
-
-    def query(self, db, params=None):
-        sql = self.sql.format(where=str(self))
-        if params is None:
-            return db.execute(sql, self.params)
-        return db.execute(sql, self.params | params)
-    
-
-def _quote_like(value):
-    return '%%%s%%' % value \
-        .replace('%', '\\%') \
-        .replace('_', '\\_')
-
-
-class LogMiddleware(Middleware):
-
-    def __init__(self, path, trace, payload):
-        self.path = prepare_path(path)
-        self.trace = trace
-        self.payload = payload
-        sqlite3.register_adapter(Traceback, self._adapt_traceback)
-        with self._open_db() as db:
-            db.execute(CREATE_DATABASE_SQL)
-
-    def _adapt_traceback(self, traceback):
-        return str(traceback)
-
-    def _open_db(self):
-        return sqlite3.connect(self.path)
-
-    def query_dataset(self, page, qname=None, qtype=None, page_size=QUERY_PAGE_SIZE):
-        offset = (page - 1) * page_size
-        query = Query(SELECT_DATASET_SQL)
-        if qname:
-            query.where('qname like {qname}', qname=_quote_like(qname))
-        if qtype:
-            query.where('qtype={qtype}', qtype=qtype)
-
-        with self._open_db() as db:
-            result = query.query(db, {
-                'offset': offset,
-                'page_size': page_size,
-            })
-            field_names = [column[0] for column in result.description]
-            def format_row(row):
-                record = dict(zip(field_names, row))
-                traceback = record['traceback']
-                if traceback:
-                    try:
-                        record['traceback'] = json.loads(traceback)
-                    except json.JSONDecodeError:
-                        record['traceback'] = None
-                return record
-            return list(map(format_row, result))
-
-    def query_total(self, qname=None, qtype=None):
-        query = Query(COUNT_DATASET_SQL)
-        if qname:
-            query.where('qname like {qname}', qname=_quote_like(qname))
-        if qtype:
-            query.where('qtype={qtype}', qtype=qtype)
-        with self._open_db() as db:
-            result = query.query(db)
-            total, = result.fetchone()
-            return total
-
-    def clear_dataset(self):
-        with self._open_db() as db:
-            db.execute(TRUNCATE_TABLE_SQL)
-        return True
-
-    async def handle(self, request, **kwargs):
-        if self.trace:
-            kwargs['traceback'] = traceback = Traceback()
-        else:
-            traceback = None
-        params = {
-            'now': time.strftime('%Y-%m-%d %H:%M:%S', time.localtime()),
-            'qname': str(request.q.qname),
-            'qtype': dnslib.QTYPE[request.q.qtype],
-            'request': request.pack() if self.payload else None,
-            'traceback': traceback,
-        }
-
-        start_counter = time.perf_counter()
-        try:
-            response = await super().handle(request, **kwargs)
-        except Exception as exc:
-            params |= {'success': False, 'error': str(exc), 'elapsed_time': time.perf_counter() - start_counter}
-            with self._open_db() as db: db.execute(INSERT_FAILURE_SQL, params)
-            raise
-        if response is None:
-            params |= {'success': False, 'error': 'N/A', 'elapsed_time': time.perf_counter() - start_counter}
-            with self._open_db() as db: db.execute(INSERT_FAILURE_SQL, params)
-        else:
-            params |= {
-                'success': True, 
-                'response': response.pack() if self.payload else None, 
-                'elapsed_time': time.perf_counter() - start_counter
-            }
-            with self._open_db() as db: db.execute(INSERT_SUCCESS_SQL, params)
-        return response
+import logging
+import sqlite3
+import time
+import json
+
+import dnslib
+
+from . import Middleware, Traceback
+from ..helpers import prepare_path
+
+
+logger = logging.getLogger(__name__)
+
+
+CREATE_DATABASE_SQL = \
+'''CREATE TABLE IF NOT EXISTS "log" (
+    "id"            INTEGER,
+    "created_at"    TEXT,
+    "elapsed_time"  REAL,
+    "qname"         TEXT,
+    "qtype"         TEXT,
+    "success"       INTEGER,
+    "request"       BLOB,
+    "response"      BLOB,
+    "traceback"     TEXT,
+    "error"         TEXT,
+    PRIMARY KEY("id" AUTOINCREMENT)
+);
+'''
+
+INSERT_FAILURE_SQL = \
+'''INSERT INTO "log" 
+    (created_at, elapsed_time, qname, qtype, success, request, error, traceback) 
+    VALUES 
+    (:now, :elapsed_time, :qname, :qtype, :success, :request, :error, :traceback)
+'''
+
+INSERT_SUCCESS_SQL = \
+'''INSERT INTO "log" 
+    (created_at, elapsed_time, qname, qtype, success, request, response, traceback) 
+    VALUES 
+    (:now, :elapsed_time, :qname, :qtype, :success, :request, :response, :traceback)
+'''
+
+SELECT_DATASET_SQL = \
+'''SELECT id, created_at, elapsed_time, qname, qtype, success, traceback, error 
+    FROM "log" {where} ORDER BY id DESC LIMIT :offset, :page_size
+'''
+
+COUNT_DATASET_SQL = 'SELECT COUNT(*) FROM "log" {where}'
+
+TRUNCATE_TABLE_SQL = 'DELETE FROM "log"'
+
+QUERY_PAGE_SIZE = 50
+
+
+class Query:
+    def __init__(self, sql):
+        self.sql = sql
+        self.conditions = []
+        self.params = dict()
+
+    def where(self, expr, **kwargs):
+        self.params |= kwargs
+        placeholders = { key: ':%s' % key for key in kwargs.keys() }
+        self.conditions.append(expr.format(**placeholders))
+
+    def __repr__(self):
+        if not self.conditions:
+            return ''
+        return 'WHERE ' + ' AND '.join(self.conditions)
+
+    def query(self, db, params=None):
+        sql = self.sql.format(where=str(self))
+        if params is None:
+            return db.execute(sql, self.params)
+        return db.execute(sql, self.params | params)
+    
+
+def _quote_like(value):
+    return '%%%s%%' % value \
+        .replace('%', '\\%') \
+        .replace('_', '\\_')
+
+
+class LogMiddleware(Middleware):
+
+    def __init__(self, path, trace, payload):
+        self.path = prepare_path(path)
+        self.trace = trace
+        self.payload = payload
+        sqlite3.register_adapter(Traceback, self._adapt_traceback)
+        with self._open_db() as db:
+            db.execute(CREATE_DATABASE_SQL)
+
+    def _adapt_traceback(self, traceback):
+        return str(traceback)
+
+    def _open_db(self):
+        return sqlite3.connect(self.path)
+
+    def query_dataset(self, page, qname=None, qtype=None, page_size=QUERY_PAGE_SIZE):
+        offset = (page - 1) * page_size
+        query = Query(SELECT_DATASET_SQL)
+        if qname:
+            query.where('qname like {qname}', qname=_quote_like(qname))
+        if qtype:
+            query.where('qtype={qtype}', qtype=qtype)
+
+        with self._open_db() as db:
+            result = query.query(db, {
+                'offset': offset,
+                'page_size': page_size,
+            })
+            field_names = [column[0] for column in result.description]
+            def format_row(row):
+                record = dict(zip(field_names, row))
+                traceback = record['traceback']
+                if traceback:
+                    try:
+                        record['traceback'] = json.loads(traceback)
+                    except json.JSONDecodeError:
+                        record['traceback'] = None
+                return record
+            return list(map(format_row, result))
+
+    def query_total(self, qname=None, qtype=None):
+        query = Query(COUNT_DATASET_SQL)
+        if qname:
+            query.where('qname like {qname}', qname=_quote_like(qname))
+        if qtype:
+            query.where('qtype={qtype}', qtype=qtype)
+        with self._open_db() as db:
+            result = query.query(db)
+            total, = result.fetchone()
+            return total
+
+    def clear_dataset(self):
+        with self._open_db() as db:
+            db.execute(TRUNCATE_TABLE_SQL)
+        return True
+
+    async def handle(self, request, **kwargs):
+        if self.trace:
+            kwargs['traceback'] = traceback = Traceback()
+        else:
+            traceback = None
+        params = {
+            'now': time.strftime('%Y-%m-%d %H:%M:%S', time.localtime()),
+            'qname': str(request.q.qname),
+            'qtype': dnslib.QTYPE[request.q.qtype],
+            'request': request.pack() if self.payload else None,
+            'traceback': traceback,
+        }
+
+        start_counter = time.perf_counter()
+        try:
+            response = await super().handle(request, **kwargs)
+        except Exception as exc:
+            params |= {'success': False, 'error': str(exc), 'elapsed_time': time.perf_counter() - start_counter}
+            with self._open_db() as db: db.execute(INSERT_FAILURE_SQL, params)
+            raise
+        if response is None:
+            params |= {'success': False, 'error': 'N/A', 'elapsed_time': time.perf_counter() - start_counter}
+            with self._open_db() as db: db.execute(INSERT_FAILURE_SQL, params)
+        else:
+            params |= {
+                'success': True, 
+                'response': response.pack() if self.payload else None, 
+                'elapsed_time': time.perf_counter() - start_counter
+            }
+            with self._open_db() as db: db.execute(INSERT_SUCCESS_SQL, params)
+        return response
```

### Comparing `dnspooh-1.3.1/dnspooh/middlewares/rules.py` & `dnspooh-1.3.2/dnspooh/middlewares/rules.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,903 +1,903 @@
-import asyncio
-import logging
-import re
-import enum
-import ipaddress
-import functools
-import subprocess
-
-from collections.abc import Iterable
-
-import dnslib
-import pyparsing
-
-from . import Middleware
-from ..exceptions import InvalidConfig
-from ..helpers import split_domain
-
-
-logger = logging.getLogger(__name__)
-
-
-opt_comma = pyparsing.Suppress(pyparsing.Opt(','))
-
-_ipv4_literal = pyparsing.common.ipv4_address
-
-_ipv6_literal = pyparsing.common.ipv6_address
-
-_ipv4_cidr_literal = _ipv4_literal + '/' + pyparsing.Word(pyparsing.nums, max=2)
-
-_ipv6_cidr_literal = _ipv6_literal + '/' + pyparsing.Word(pyparsing.nums, max=3)
-
-ip_literal = pyparsing.Combine(_ipv4_literal | _ipv6_literal)\
-    .set_name('ip address')\
-    .set_parse_action(lambda tokens: ipaddress.ip_address(tokens[0]))
-
-ip_cidr_literal = pyparsing.Combine(_ipv4_cidr_literal | _ipv6_cidr_literal)\
-    .set_name('CIDR')\
-    .set_parse_action(lambda tokens: ipaddress.ip_network(tokens[0], False))
-
-ip_cidr_literal_list = (pyparsing.Suppress('(') + pyparsing.OneOrMore(ip_cidr_literal + opt_comma) + pyparsing.Suppress(')'))\
-    .set_name('list of CIDRs')\
-    .set_parse_action(lambda tokens: tuple(tokens))
-
-country_code_literal = pyparsing.Word(pyparsing.alphas, exact=2).set_name('country code')
-
-domain_literal = pyparsing.Word(pyparsing.alphanums + '.-').set_name('domain')\
-    .set_parse_action(lambda tokens: tokens[0].lower())
-
-domain_literal_set = (pyparsing.Suppress('(') + pyparsing.OneOrMore(domain_literal + opt_comma) + pyparsing.Suppress(')'))\
-    .set_name('set of domains')\
-    .set_parse_action(lambda tokens: set(map(lambda _: _.strip('.'), tokens)))
-
-domain_literal_list = (pyparsing.Suppress('(') + pyparsing.OneOrMore(domain_literal + opt_comma) + pyparsing.Suppress(')'))\
-    .set_name('list of domains')\
-    .set_parse_action(lambda tokens: tuple(tokens))
-
-ip_literal_list = (pyparsing.Suppress('(') + pyparsing.OneOrMore(ip_literal + opt_comma) + pyparsing.Suppress(')'))\
-    .set_name('list of ip addresses')\
-    .set_parse_action(lambda tokens: tuple(tokens))
-
-ip_literal_set = (pyparsing.Suppress('(') + pyparsing.OneOrMore(ip_literal + opt_comma) + pyparsing.Suppress(')'))\
-    .set_name('set of ip addresses')\
-    .set_parse_action(lambda tokens: set(tokens))
-
-proxy_literal = pyparsing.Regex(r'(http|socks5):\/\/([\w\.-:@%]+)').set_name('proxy')\
-    .set_parse_action(lambda tokens: tokens[0])
-
-always_literal = pyparsing.Literal('always').set_name('always')\
-    .set_parse_action(lambda _: True)
-
-
-def _and_op(op, tokens):
-    return op, tuple(filter(lambda it: it != 'and', tokens))
-
-
-def _or_op(op, tokens):
-    return op, tuple(filter(lambda it: it != 'or', tokens))
-
-
-def _response_add_answers(response, ip_addrs, top=False):
-    hostname = response.q.qname.idna().rstrip('.')
-    qtype = response.q.qtype
-    if not isinstance(ip_addrs, Iterable):
-        ip_addrs = (ip_addrs, )
-
-    if qtype == dnslib.QTYPE.AAAA:
-        records = [
-            dnslib.RR(hostname, qtype, rdata=dnslib.AAAA(str(ip))) 
-            for ip in ip_addrs if isinstance(ip, ipaddress.IPv6Address)
-        ]
-    elif qtype == dnslib.QTYPE.A:
-        records = [
-            dnslib.RR(hostname, qtype, rdata=dnslib.A(str(ip))) 
-            for ip in ip_addrs if isinstance(ip, ipaddress.IPv4Address)
-        ]
-    else:
-        return response
-    if top:
-        records.extend(response.rr)
-        response.rr = records
-        response.set_header_qa()
-    else:
-        response.add_answer(*records)
-    return response
-
-
-def _response_nxdomain(response):
-    response.rr = []
-    response.set_header_qa()
-    response.header.rcode = dnslib.RCODE.NXDOMAIN
-    return response
-
-
-def _is_a_aaaa(request):
-    return request.q.qtype in (dnslib.QTYPE.AAAA, dnslib.QTYPE.A)
-
-
-class OpCode(enum.Enum):
-    NOT = enum.auto()
-    AND = enum.auto()
-    OR = enum.auto()
-    DOMAIN_CONTAINS = enum.auto()
-    DOMAIN_NOT_CONTAINS = enum.auto()
-    DOMAIN_EQ = enum.auto()
-    DOMAIN_NOT_EQ = enum.auto()
-    DOMAIN_STARTS_WITH = enum.auto()
-    DOMAIN_STARTS_WITHOUT = enum.auto()
-    DOMAIN_ENDS_WITH = enum.auto()
-    DOMAIN_ENDS_WITHOUT = enum.auto()
-    DOMAIN_MATCH = enum.auto()
-    BLOCK = enum.auto()
-    RETURN = enum.auto()
-    UPSTREAM_GROUP_SET = enum.auto()
-    UPSTREAM_NAME_SET = enum.auto()
-    DOMAIN_REPLACE = enum.auto()
-    PROXY_SET = enum.auto()
-    FIRST = enum.auto()
-    LAST = enum.auto()
-    IP_IN = enum.auto()
-    IP_NOT_IN = enum.auto()
-    IP_EQ = enum.auto()
-    IP_NOT_EQ = enum.auto()
-    GEOIP_EQ = enum.auto()
-    GEOIP_NOT_EQ = enum.auto()
-    ANY_IP_IN = enum.auto()
-    ANY_IP_NOT_IN = enum.auto()
-    ANY_IP_EQ = enum.auto()
-    ANY_IP_NOT_EQ = enum.auto()
-    ANY_GEOIP_EQ = enum.auto()
-    ANY_GEOIP_NOT_EQ = enum.auto()
-    ALL_IP_IN = enum.auto()
-    ALL_IP_NOT_IN = enum.auto()
-    ALL_IP_EQ = enum.auto()
-    ALL_IP_NOT_EQ = enum.auto()
-    ALL_GEOIP_EQ = enum.auto()
-    ALL_GEOIP_NOT_EQ = enum.auto()
-    RECORD_ADD = enum.auto()
-    RECORD_ADD_IF = enum.auto()
-    RECORD_APPEND = enum.auto()
-    RECORD_APPEND_IF = enum.auto()
-    RECORD_INSERT = enum.auto()
-    RECORD_INSERT_IF = enum.auto()
-    RECORD_REMOVE_WHERE = enum.auto()
-    RECORD_REPLACE_WHERE = enum.auto()
-    RUN_WHERE = enum.auto()
-    BLOCK_IF = enum.auto()
-    RETURN_IF = enum.auto()
-
-    def __repr__(self):
-        return self.name
-
-
-class RuleIfParser:
-    class IfExpr:
-        def __init__(self, ast):
-            self.ast = ast
-
-        def __repr__(self):
-            return repr(self.ast)
-
-        def test(self, domain):
-            def _test(ast):
-                if not isinstance(ast, tuple):
-                    return ast
-                opcode = ast[0]
-                if opcode == OpCode.AND:
-                    return all(map(_test, ast[1]))
-                elif opcode == OpCode.OR:
-                    return any(map(_test, ast[1]))
-                elif opcode == OpCode.NOT:
-                    return not _test(ast[1])
-                elif opcode == OpCode.DOMAIN_CONTAINS:
-                    if isinstance(ast[1], tuple):
-                        return any(map(lambda _: _ in domain, ast[1]))
-                    else:
-                        return ast[1] in domain
-                elif opcode == OpCode.DOMAIN_NOT_CONTAINS:
-                    if isinstance(ast[1], tuple):
-                        return all(map(lambda _: _ not in domain, ast[1]))
-                    else:
-                        return ast[1] not in domain
-                elif opcode == OpCode.DOMAIN_EQ:
-                    if isinstance(ast[1], set):
-                        return domain in ast[1]
-                    else:
-                        return ast[1] == domain
-                elif opcode == OpCode.DOMAIN_NOT_EQ:
-                    if isinstance(ast[1], set):
-                        return domain not in ast[1]
-                    else:
-                        return ast[1] != domain
-                elif opcode == OpCode.DOMAIN_STARTS_WITH:
-                    if isinstance(ast[1], set):
-                        return any(map(lambda _: _ in ast[1], split_domain(domain, False)))
-                    else:
-                        return domain.startswith(ast[1])
-                elif opcode == OpCode.DOMAIN_STARTS_WITHOUT:
-                    if isinstance(ast[1], set):
-                        return all(map(lambda _: _ not in ast[1], split_domain(domain, False)))
-                    else:
-                        return not domain.startswith(ast[1])
-                elif opcode == OpCode.DOMAIN_ENDS_WITH:
-                    if isinstance(ast[1], set):
-                        return any(map(lambda _: _ in ast[1], split_domain(domain)))
-                    else:
-                        return domain.endswith(ast[1])
-                elif opcode == OpCode.DOMAIN_ENDS_WITHOUT:
-                    if isinstance(ast[1], set):
-                        return all(map(lambda _: _ not in ast[1], split_domain(domain)))
-                    else:
-                        return not domain.endswith(ast[1])
-                elif opcode == OpCode.DOMAIN_MATCH:
-                    return re.fullmatch(ast[1], domain) is not None
-                return False
-            return _test(self.ast)
-
-    def __init__(self):
-        expr_domain_contains = ((domain_literal | domain_literal_list) + 'in domain')\
-            .set_name('domain contains expression')\
-            .set_parse_action(lambda tokens: (OpCode.DOMAIN_CONTAINS, tokens[0]))
-        expr_domain_not_contains = ((domain_literal | domain_literal_list) + 'not in domain')\
-            .set_name('domain not contains expression')\
-            .set_parse_action(lambda tokens: (OpCode.DOMAIN_NOT_CONTAINS, tokens[0]))
-        expr_domain_equal = ('domain is' + (domain_literal | domain_literal_set))\
-            .set_name('domain equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.DOMAIN_EQ, tokens[1]))
-        expr_domain_not_equal = ('domain is not' + (domain_literal | domain_literal_set))\
-            .set_name('domain not equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.DOMAIN_NOT_EQ, tokens[1]))
-        expr_domain_starts_with = ('domain starts with' + (domain_literal | domain_literal_set))\
-            .set_name('domain starts with expression')\
-            .set_parse_action(lambda tokens: (OpCode.DOMAIN_STARTS_WITH, tokens[1]))
-        expr_domain_starts_without = ('domain starts without' + (domain_literal | domain_literal_set))\
-            .set_name('domain starts without expression')\
-            .set_parse_action(lambda tokens: (OpCode.DOMAIN_STARTS_WITHOUT, tokens[1]))
-        expr_domain_ends_with = ('domain ends with' + (domain_literal | domain_literal_set))\
-            .set_name('domain ends with expression')\
-            .set_parse_action(lambda tokens: (OpCode.DOMAIN_ENDS_WITH, tokens[1]))
-        expr_domain_ends_without = ('domain ends without' + (domain_literal | domain_literal_set))\
-            .set_name('domain ends without expression')\
-            .set_parse_action(lambda tokens: (OpCode.DOMAIN_ENDS_WITHOUT, tokens[1]))
-        expr_domain_match = ('domain match' + pyparsing.QuotedString('/'))\
-            .set_name('domain match expression')\
-            .set_parse_action(lambda tokens: (OpCode.DOMAIN_MATCH, tokens[1]))
-        expr_simple = (
-            expr_domain_not_contains |
-            expr_domain_contains |
-            expr_domain_not_equal |
-            expr_domain_equal |
-            expr_domain_starts_without |
-            expr_domain_starts_with |
-            expr_domain_ends_without |
-            expr_domain_ends_with |
-            expr_domain_match
-        )
-        expr = pyparsing.Forward()
-        expr <<= pyparsing.infix_notation(expr_simple, [
-            ('not', 1, pyparsing.opAssoc.RIGHT, lambda tokens: (OpCode.NOT, tokens[0][1])),
-            ('and', 2, pyparsing.opAssoc.LEFT, lambda tokens: _and_op(OpCode.AND, tokens[0])),
-            ('or', 2, pyparsing.opAssoc.LEFT, lambda tokens: _or_op(OpCode.OR, tokens[0])),
-        ])
-        self.parser = expr | always_literal
-    
-    def parse(self, source):
-        parse_results = self.parser.parse_string(source, parse_all=True)
-        return self.IfExpr(parse_results[0])
-
-
-class RuleThenParser:
-    class ThenExec:
-        def __repr__(self):
-            return repr(self.ast)
-
-        def __init__(self, ast):
-            self.ast = ast[0]
-
-        def exec(self, request):
-            response = request.reply()
-            _exec = self.ast[0]
-            if _exec == OpCode.BLOCK:
-                response.header.rcode = dnslib.RCODE.NXDOMAIN
-            elif _exec == OpCode.RETURN:
-                ip_addrs = self.ast[1] if isinstance(self.ast[1], tuple) else (self.ast[1], )
-                _response_add_answers(response, ip_addrs)
-            return response
-
-    def __init__(self):
-        stm_block = pyparsing.Literal('block')\
-            .set_name('block statement')\
-            .set_parse_action(lambda _: (OpCode.BLOCK, ))
-        stm_return = ('return' + (ip_literal_list | ip_literal))\
-            .set_name('return statement')\
-            .set_parse_action(lambda tokens: (OpCode.RETURN, tokens[1]))
-        stm_single = (
-            stm_block |
-            stm_return
-        )
-        self.parser = stm_single
-
-    def parse(self, source):
-        parse_results = self.parser.parse_string(source, parse_all=True)
-        return self.ThenExec(parse_results)
-
-
-class AfterHandler:
-    def after_handle(self, response, geoip, ipaddr, run):
-        return response
-
-
-class ReplacDomainHandler(AfterHandler):
-    def __init__(self, domain):
-        self.domain = domain
-
-    def after_handle(self, response, geoip, ipaddr, run):
-        response.q.qname = self.domain
-        return response
-
-
-class AfterHandlerList:
-    def __init__(self):
-        self.handlers = []
-
-    def join(self, handler):
-        if handler is None or not hasattr(handler, 'after_handle'):
-            return self
-        self.handlers.append(handler)
-        return self
-
-    def after_handle(self, response, geoip, ipaddr, run):
-        for handler in self.handlers:
-            response = handler.after_handle(response, geoip, ipaddr, run)
-        return response
-
-
-class RuleBeforeParser:
-    class BeforeExec:
-        def __repr__(self):
-            return repr(self.ast)
-
-        def __init__(self, ast):
-            self.ast = list(ast)
-
-        def exec(self, request, kwargs):
-            after_handler = None
-            for stm in self.ast:
-                _exec = stm[0]
-                if _exec == OpCode.UPSTREAM_GROUP_SET:
-                    kwargs['upstream_group'] = stm[1]
-                elif _exec == OpCode.UPSTREAM_NAME_SET:
-                    kwargs['upstream_name'] = stm[1]
-                elif _exec == OpCode.DOMAIN_REPLACE:
-                    after_handler = ReplacDomainHandler(request.q.qname)
-                    request.q.qname = stm[1]
-                elif _exec == OpCode.PROXY_SET:
-                    if stm[1] == 'on':
-                        kwargs.pop('proxy', None)
-                    elif stm[1] == 'off':
-                        kwargs['proxy'] = None
-                    else:
-                        kwargs['proxy'] = stm[1]
-            return after_handler
-
-    def __init__(self):
-        upstream_name_literal = pyparsing.Word(pyparsing.alphanums + '.-_')\
-            .set_name('upstream name')
-        upstream_group_literal = pyparsing.Word(pyparsing.alphanums + '.-_')\
-            .set_name('upstream group')
-        stm_upstream_name_set = ('set upstream name to' + upstream_name_literal)\
-            .set_name('set upstream name statement')\
-            .set_parse_action(lambda tokens: (OpCode.UPSTREAM_NAME_SET, tokens[1]))
-        stm_upstream_group_set = ('set upstream group to' + upstream_group_literal)\
-            .set_name('set upstream group statement')\
-            .set_parse_action(lambda tokens: (OpCode.UPSTREAM_GROUP_SET, tokens[1]))
-        stm_domain_replace = ('replace domain by' + domain_literal)\
-            .set_name('replace domain statement')\
-            .set_parse_action(lambda tokens: (OpCode.DOMAIN_REPLACE, tokens[1]))
-        stm_proxy_on = pyparsing.Literal('set proxy on')\
-            .set_name('set proxy on statement')\
-            .set_parse_action(lambda _: (OpCode.PROXY_SET, 'on'))
-        stm_proxy_off = pyparsing.Literal('set proxy off')\
-            .set_name('set proxy off statement')\
-            .set_parse_action(lambda _: (OpCode.PROXY_SET, 'off'))
-        stm_proxy_set = ('set proxy to' + proxy_literal)\
-            .set_name('set proxy to statement')\
-            .set_parse_action(lambda tokens: (OpCode.PROXY_SET, tokens[1]))
-        stm_simple = (
-            stm_upstream_name_set |
-            stm_upstream_group_set |
-            stm_domain_replace |
-            stm_proxy_on |
-            stm_proxy_off |
-            stm_proxy_set
-        )
-        self.parser = pyparsing.OneOrMore(stm_simple + opt_comma)
-
-    def parse(self, source):
-        parse_results = self.parser.parse_string(source, parse_all=True)
-        return self.BeforeExec(parse_results)
-
-
-class RuleAfterParser:
-    class AfterExec:
-        def __init__(self, ast):
-            self.ast = list(ast)
-
-        def __repr__(self):
-            return repr(self.ast)
-
-        def test_record(self, geoip, ipaddr, response, expr_if, idx_rr):
-            idx, rr = idx_rr
-            def test(ast):
-                if not isinstance(ast, tuple):
-                    return ast
-                if rr.rtype not in (dnslib.QTYPE.AAAA, dnslib.QTYPE.A):
-                    return False
-
-                opcode = ast[0]
-                if opcode == OpCode.AND:
-                    return all(map(test, ast[1]))
-                elif opcode == OpCode.OR:
-                    return any(map(test, ast[1]))
-                elif opcode == OpCode.NOT:
-                    return not test(ast[1])
-                elif opcode == OpCode.IP_EQ:
-                    if isinstance(ast[1], set):
-                        return ipaddr(rr) in ast[1]
-                    else:
-                        return ast[1] == ipaddr(rr)
-                elif opcode == OpCode.IP_NOT_EQ:
-                    if isinstance(ast[1], set):
-                        return ipaddr(rr) not in ast[1]
-                    else:
-                        return ast[1] != ipaddr(rr)
-                elif opcode == OpCode.IP_IN:
-                    if isinstance(ast[1], tuple):
-                        return any(map(lambda _: ipaddr(rr) in _, ast[1]))
-                    else:
-                        return ipaddr(rr) in ast[1]
-                elif opcode == OpCode.IP_NOT_IN:
-                    if isinstance(ast[1], tuple):
-                        return all(map(lambda _: ipaddr(rr) not in _, ast[1]))
-                    else:
-                        return ipaddr(rr) not in ast[1]
-                elif opcode == OpCode.GEOIP_EQ:
-                    return geoip(rr) == ast[1].upper()
-                elif opcode == OpCode.GEOIP_NOT_EQ:
-                    return geoip(rr) != ast[1].upper()
-                elif opcode == OpCode.FIRST:
-                    return idx == 0
-                elif opcode == OpCode.LAST:
-                    return idx == len(response.rr) - 1
-                return False
-            return test(expr_if)
-
-        def test_response(self, geoip, ipaddr, expr_if, response):
-            def test(ast):
-                if not isinstance(ast, tuple):
-                    return ast
-
-                opcode = ast[0]
-                if opcode == OpCode.AND:
-                    return all(map(test, ast[1]))
-                elif opcode == OpCode.OR:
-                    return any(map(test, ast[1]))
-                elif opcode == OpCode.NOT:
-                    return not test(ast[1])
-
-                rr = filter(lambda rr: rr.rtype in (dnslib.QTYPE.AAAA, dnslib.QTYPE.A), response.rr)
-                ip_addresses = map(lambda rr: ipaddr(rr), rr)
-                country_codes = map(lambda rr: geoip(rr), rr)
-                if opcode == OpCode.ANY_IP_EQ:
-                    if isinstance(ast[1], set):
-                        return any(map(lambda _: _ in ast[1], ip_addresses))
-                    else:
-                        return any(map(lambda ip: ip == ast[1], ip_addresses))
-                elif opcode == OpCode.ANY_IP_NOT_EQ:
-                    if isinstance(ast[1], set):
-                        return any(map(lambda _: _ not in ast[1], ip_addresses))
-                    else:
-                        return any(map(lambda ip: ip != ast[1], ip_addresses))
-                elif opcode == OpCode.ANY_IP_IN:
-                    if isinstance(ast[1], tuple):
-                        return any(map(lambda ip: any(map(lambda _: ip in _, ast[1])), ip_addresses))
-                    else:
-                        return any(map(lambda ip: ip in ast[1], ip_addresses))
-                elif opcode == OpCode.ANY_IP_NOT_IN:
-                    if isinstance(ast[1], tuple):
-                        return any(map(lambda ip: all(map(lambda _: ip not in _, ast[1])), ip_addresses))
-                    else:
-                        return any(map(lambda ip: ip not in ast[1], ip_addresses))
-                elif opcode == OpCode.ANY_GEOIP_EQ:
-                    return any(map(lambda country_code: country_code == ast[1], country_codes))
-                elif opcode == OpCode.ANY_GEOIP_NOT_EQ:
-                    return any(map(lambda country_code: country_code != ast[1], country_codes))
-                elif opcode == OpCode.ALL_IP_EQ:
-                    if isinstance(ast[1], set):
-                        return all(map(lambda _: _ in ast[1], ip_addresses))
-                    else:
-                        return all(map(lambda ip: ip == ast[1], ip_addresses))
-                elif opcode == OpCode.ALL_IP_NOT_EQ:
-                    if isinstance(ast[1], set):
-                        return all(map(lambda _: _ not in ast[1], ip_addresses))
-                    else:
-                        return all(map(lambda ip: ip != ast[1], ip_addresses))
-                elif opcode == OpCode.ALL_IP_IN:
-                    if isinstance(ast[1], tuple):
-                        return all(map(lambda ip: any(map(lambda _: ip in _, ast[1])), ip_addresses))
-                    else:
-                        return all(map(lambda ip: ip in ast[1], ip_addresses))
-                elif opcode == OpCode.ALL_IP_NOT_IN:
-                    if isinstance(ast[1], tuple):
-                        return all(map(lambda ip: all(map(lambda _: ip not in _, ast[1])), ip_addresses))
-                    else:
-                        return all(map(lambda ip: ip not in ast[1], ip_addresses))
-                elif opcode == OpCode.ALL_GEOIP_EQ:
-                    return all(map(lambda country_code: country_code == ast[1], country_codes))
-                elif opcode == OpCode.ALL_GEOIP_NOT_EQ:
-                    return all(map(lambda country_code: country_code != ast[1], country_codes))
-                return False
-            return test(expr_if)
-
-        def exec(self, response, geoip, ipaddr, run):
-            test_record = functools.partial(self.test_record, geoip, ipaddr, response)
-            test_response = functools.partial(self.test_response, geoip, ipaddr)
-
-            for stm in self.ast:
-                _exec = stm[0]
-                if _exec in (OpCode.RECORD_ADD, OpCode.RECORD_APPEND):
-                    _response_add_answers(response, stm[1])
-                    continue
-                elif _exec == OpCode.RECORD_INSERT:
-                    _response_add_answers(response, stm[1], True)
-                    continue
-
-                expr_if = stm[1]
-                if _exec == OpCode.RECORD_REMOVE_WHERE:
-                    response.rr = list(map(
-                        lambda idx_rr: idx_rr[1],
-                        filter(
-                            lambda idx_rr: not test_record(expr_if, idx_rr), 
-                            enumerate(response.rr)
-                        )
-                    ))
-                    response.set_header_qa()
-                    continue
-                elif _exec == OpCode.RECORD_REPLACE_WHERE:
-                    qtype = response.q.qtype
-                    ip = stm[2]
-                    for idx, rr in enumerate(response.rr):
-                        if not test_record(expr_if, (idx, rr)):
-                            continue
-                        if isinstance(ip, ipaddress.IPv6Address) and qtype == dnslib.QTYPE.AAAA:
-                            rr.rdata = dnslib.AAAA(str(ip))
-                        elif isinstance(ip, ipaddress.IPv4Address) and qtype == dnslib.QTYPE.A:
-                            rr.rdata = dnslib.A(str(ip))
-                    continue
-                elif _exec == OpCode.RUN_WHERE:
-                    cmd = stm[2]
-                    hostname = response.q.qname.idna().rstrip('.')
-                    for idx, rr in enumerate(response.rr):
-                        if not test_record(expr_if, (idx, rr)):
-                            continue
-                        run(cmd.format(ip=rr.rdata, domain=hostname))
-                    continue
-
-                if _exec == OpCode.RETURN_IF:
-                    if test_response(expr_if, response):
-                        response.rr = []
-                        _response_add_answers(response, stm[2])
-                elif _exec == OpCode.BLOCK_IF:
-                    if test_response(expr_if, response):
-                        _response_nxdomain(response)
-                elif _exec in (OpCode.RECORD_ADD_IF, OpCode.RECORD_APPEND_IF):
-                    if test_response(expr_if, response):
-                        _response_add_answers(response, stm[2])
-                elif _exec == OpCode.RECORD_INSERT_IF:
-                    if test_response(expr_if, response):
-                        _response_add_answers(response, stm[2], True)
-            return response
-
-    def __init__(self):
-        expr_first = pyparsing.Literal('first').set_name('first')\
-            .set_parse_action(lambda _: (OpCode.FIRST, ))
-        expr_last = pyparsing.Literal('last').set_name('last')\
-            .set_parse_action(lambda _: (OpCode.LAST, ))
-        expr_ip_in = ('ip in' + (ip_cidr_literal | ip_cidr_literal_list))\
-            .set_name('ip in cidr expression')\
-            .set_parse_action(lambda tokens: (OpCode.IP_IN, tokens[1]))
-        expr_ip_not_in = ('ip not in' + (ip_cidr_literal | ip_cidr_literal_list))\
-            .set_name('ip not in cidr expression')\
-            .set_parse_action(lambda tokens: (OpCode.IP_NOT_IN, tokens[1]))
-        expr_ip_equal = ('ip is' + (ip_literal | ip_literal_set))\
-            .set_name('ip equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.IP_EQ, tokens[1]))
-        expr_ip_not_equal = ('ip is not' + (ip_literal | ip_literal_set))\
-            .set_name('ip not equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.IP_NOT_EQ, tokens[1]))
-        expr_geoip_equal = ('geoip is' + country_code_literal)\
-            .set_name('geoip equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.GEOIP_EQ, tokens[1]))
-        expr_geoip_not_equal = ('geoip is not' + country_code_literal)\
-            .set_name('geoip not equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.GEOIP_NOT_EQ, tokens[1]))
-        expr_any_ip_in = ('any ip in' + (ip_cidr_literal | ip_cidr_literal_list))\
-            .set_name('any ip in cidr expression')\
-            .set_parse_action(lambda tokens: (OpCode.ANY_IP_IN, tokens[1]))
-        expr_any_ip_not_in = ('any ip not in' + (ip_cidr_literal | ip_cidr_literal_list))\
-            .set_name('any ip not in cidr expression')\
-            .set_parse_action(lambda tokens: (OpCode.ANY_IP_NOT_IN, tokens[1]))
-        expr_any_ip_equal = ('any ip is' + (ip_literal | ip_literal_set))\
-            .set_name('any ip equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.ANY_IP_EQ, tokens[1]))
-        expr_any_ip_not_equal = ('any ip is not' + (ip_literal | ip_literal_set))\
-            .set_name('any ip not equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.ANY_IP_NOT_EQ, tokens[1]))
-        expr_any_geoip_equal = ('any geoip is' + country_code_literal)\
-            .set_name('any geoip equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.ANY_GEOIP_EQ, tokens[1]))
-        expr_any_geoip_not_equal = ('any geoip is not' + country_code_literal)\
-            .set_name('any geoip not equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.ANY_GEOIP_NOT_EQ, tokens[1]))
-        expr_all_ip_in = ('all ip in' + (ip_cidr_literal | ip_cidr_literal_list))\
-            .set_name('all ip in cidr expression')\
-            .set_parse_action(lambda tokens: (OpCode.ALL_IP_IN, tokens[1]))
-        expr_all_ip_not_in = ('all ip not in' + (ip_cidr_literal | ip_cidr_literal_list))\
-            .set_name('all ip not in cidr expression')\
-            .set_parse_action(lambda tokens: (OpCode.ALL_IP_NOT_IN, tokens[1]))
-        expr_all_ip_equal = ('all ip is' + (ip_literal | ip_literal_set))\
-            .set_name('all ip equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.ALL_IP_EQ, tokens[1]))
-        expr_all_ip_not_equal = ('all ip is not' + (ip_literal | ip_literal_set))\
-            .set_name('all ip not equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.ALL_IP_NOT_EQ, tokens[1]))
-        expr_all_geoip_equal = ('all geoip is' + country_code_literal)\
-            .set_name('all geoip equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.ALL_GEOIP_EQ, tokens[1]))
-        expr_all_geoip_not_equal = ('all geoip is not' + country_code_literal)\
-            .set_name('all geoip not equal expression')\
-            .set_parse_action(lambda tokens: (OpCode.ALL_GEOIP_NOT_EQ, tokens[1]))
-        expr_simple = (
-            expr_first |
-            expr_last |
-            expr_ip_not_in |
-            expr_ip_in |
-            expr_ip_not_equal |
-            expr_ip_equal |
-            expr_geoip_not_equal |
-            expr_geoip_equal
-        )
-        expr_complex = (
-            expr_any_ip_in |
-            expr_any_ip_not_in |
-            expr_any_ip_equal |
-            expr_any_ip_not_equal |
-            expr_any_geoip_not_equal |
-            expr_any_geoip_equal |
-            expr_all_ip_in |
-            expr_all_ip_not_in |
-            expr_all_ip_equal |
-            expr_all_ip_not_equal |
-            expr_all_geoip_not_equal |
-            expr_all_geoip_equal
-        )
-        expr_if = pyparsing.Forward()
-        expr_if <<= (pyparsing.infix_notation(expr_complex, [
-            ('not', 1, pyparsing.opAssoc.RIGHT, lambda tokens: (OpCode.NOT, tokens[0][1])),
-            ('and', 2, pyparsing.opAssoc.LEFT, lambda tokens: _and_op(OpCode.AND, tokens[0])),
-            ('or', 2, pyparsing.opAssoc.LEFT, lambda tokens: _or_op(OpCode.OR, tokens[0])),
-        ]) | always_literal)
-        expr_where = pyparsing.Forward()
-        expr_where <<= (pyparsing.infix_notation(expr_simple, [
-            ('not', 1, pyparsing.opAssoc.RIGHT, lambda tokens: (OpCode.NOT, tokens[0][1])),
-            ('and', 2, pyparsing.opAssoc.LEFT, lambda tokens: _and_op(OpCode.AND, tokens[0])),
-            ('or', 2, pyparsing.opAssoc.LEFT, lambda tokens: _or_op(OpCode.OR, tokens[0])),
-        ]) | always_literal)
-        stm_record_add = ('add record' + (ip_literal | ip_literal_list))\
-            .set_name('add record statement')\
-            .set_parse_action(lambda tokens: (OpCode.RECORD_ADD, tokens[1]))
-        stm_record_add_if = ('add record' + (ip_literal | ip_literal_list) + 'if' + expr_if)\
-            .set_name('add record if statement')\
-            .set_parse_action(lambda tokens: (OpCode.RECORD_ADD_IF, tokens[3], tokens[1]))
-        stm_record_append = ('append record' + (ip_literal | ip_literal_list))\
-            .set_name('append record statement')\
-            .set_parse_action(lambda tokens: (OpCode.RECORD_APPEND, tokens[1]))
-        stm_record_append_if = ('append record' + (ip_literal | ip_literal_list) + 'if' + expr_if)\
-            .set_name('append record if statement')\
-            .set_parse_action(lambda tokens: (OpCode.RECORD_APPEND_IF, tokens[3], tokens[1]))
-        stm_record_insert = ('insert record' + (ip_literal | ip_literal_list))\
-            .set_name('insert record statement')\
-            .set_parse_action(lambda tokens: (OpCode.RECORD_INSERT, tokens[1]))
-        stm_record_insert_if = ('insert record' + (ip_literal | ip_literal_list) + 'if' + expr_if)\
-            .set_name('insert record if statement')\
-            .set_parse_action(lambda tokens: (OpCode.RECORD_INSERT_IF, tokens[3], tokens[1]))
-        stm_record_remove_where = ('remove record where' + expr_where)\
-            .set_name('remove record where statement')\
-            .set_parse_action(lambda tokens: (OpCode.RECORD_REMOVE_WHERE, *tokens[1:]))
-        stm_record_replace_where = ('replace record by' + ip_literal + 'where' + expr_where)\
-            .set_name('replace record where statement')\
-            .set_parse_action(lambda tokens: (OpCode.RECORD_REPLACE_WHERE, tokens[3], tokens[1]))
-        stm_run_command_where = ('run' + pyparsing.QuotedString('"') + 'where' + expr_where)\
-            .set_name('run command where statement')\
-            .set_parse_action(lambda tokens: (OpCode.RUN_WHERE, tokens[3], tokens[1]))
-        stm_simple = (
-            stm_record_add_if |
-            stm_record_add |
-            stm_record_append_if |
-            stm_record_append |
-            stm_record_insert_if |
-            stm_record_insert |
-            stm_record_remove_where |
-            stm_record_replace_where |
-            stm_run_command_where
-        )
-        stm_block_if = ('block if' + expr_if)\
-            .set_name('block if statement')\
-            .set_parse_action(lambda tokens: (OpCode.BLOCK_IF, tokens[1]))
-        stm_return_if = ('return' + (ip_literal_list | ip_literal) + 'if' + expr_if)\
-            .set_name('return if statement')\
-            .set_parse_action(lambda tokens: (OpCode.RETURN_IF, tokens[3], tokens[1]))
-        stm_single = (
-            stm_block_if |
-            stm_return_if
-        )
-        self.parser = stm_single | pyparsing.OneOrMore(stm_simple + opt_comma)
-
-    def parse(self, source):
-        parse_results = self.parser.parse_string(source, parse_all=True)
-        return self.AfterExec(parse_results)
-
-
-class RulesMiddleware(Middleware):
-    class Rule:
-        def test(self, domain):
-            return self.if_expr.test(domain)
-
-    class IfThenRule(Rule):
-        def __init__(self, if_expr, then_exec, is_ended):
-            self.if_expr = if_expr
-            self.then_exec = then_exec
-            self.is_ended = is_ended
-
-        def exec(self, request):
-            return self.then_exec.exec(request)
-
-    class IfBeforeRule(Rule):
-        def __init__(self, if_expr, before, is_ended):
-            self.if_expr = if_expr
-            self.before = before
-            self.is_ended = is_ended
-
-        def before_handle(self, request, kwargs):
-            return self.before.exec(request, kwargs)
-
-    class IfAfterRule(Rule):
-        def __init__(self, if_expr, after, is_ended):
-            self.if_expr = if_expr
-            self.after = after
-            self.is_ended = is_ended
-
-        def after_handle(self, response, geoip, ipaddr, run):
-            return self.after.exec(response, geoip, ipaddr, run)
-
-    class IfBeforeAfterRule(IfBeforeRule, IfAfterRule):
-        def __init__(self, if_expr, before, after, is_ended):
-            self.if_expr = if_expr
-            self.before = before
-            self.after = after
-            self.is_ended = is_ended
-
-    def __init__(self, *rules):
-        self.if_parser = RuleIfParser()
-        self.then_parser = RuleThenParser()
-        self.before_parser = RuleBeforeParser()
-        self.after_parser = RuleAfterParser()
-        self.rules = [self._parse_rule(rule) for rule in rules]
-
-    def _parse_rule(self, rule):
-        if 'end' not in rule:
-            rule['end'] = False
-        try:
-            len_of_rule = len(rule)
-            if len_of_rule == 3:
-                if 'then' in rule:
-                    return self.IfThenRule(
-                        self.if_parser.parse(rule['if']),
-                        self.then_parser.parse(rule['then']),
-                        rule['end']
-                    )
-                elif 'before' in rule:
-                    return self.IfBeforeRule(
-                        self.if_parser.parse(rule['if']),
-                        self.before_parser.parse(rule['before']),
-                        rule['end']
-                    )
-                else:
-                    return self.IfAfterRule(
-                        self.if_parser.parse(rule['if']),
-                        self.after_parser.parse(rule['after']),
-                        rule['end']
-                    )
-            elif len_of_rule == 4:
-                return self.IfBeforeAfterRule(
-                    self.if_parser.parse(rule['if']),
-                    self.before_parser.parse(rule['before']),
-                    self.after_parser.parse(rule['after']),
-                    rule['end']
-                )
-            raise KeyError()
-        except pyparsing.exceptions.ParseException as exc:
-            raise InvalidConfig('Invalid rules config: %s' % (exc, ))
-        except KeyError:
-            raise InvalidConfig('A rule must match [if/then] or [if/before/after] pattern')
-
-    def _geoip(self, ip):
-        result = self.geoip_reader.get(ip)                            
-        return result['country']['iso_code'] if result else None
-
-    async def _query(self, request, **kwargs):
-        response = await super().handle(request, **kwargs)
-        ips = map(lambda r: str(r.rdata), response.rr)
-        geoips = map(self._geoip, ips)
-        return response, ips, geoips
-
-    @property
-    def geoip_reader(self):
-        if not hasattr(self, '_geoip_reader'):
-            self._geoip_reader = self.server.open_geoip()
-        return self._geoip_reader
-
-    async def handle(self, request, **kwargs):
-        cached_geoips = dict()
-        cached_ipaddrs = dict()
-        def geoip(record):
-            ip_str = str(record.rdata)
-            if ip_str in cached_geoips:
-                return cached_geoips[ip_str]
-            cached_geoips[ip_str] = country_code = self._geoip(ip_str)
-            return country_code
-        
-        def ipaddr(record):
-            ip_str = str(record.rdata)
-            if ip_str in cached_ipaddrs:
-                return cached_ipaddrs[ip_str]
-            if record.rtype == dnslib.QTYPE.A:
-                return ipaddress.IPv4Address(ip_str)
-            elif record.rtype == dnslib.QTYPE.AAAA:
-                return ipaddress.IPv6Address(ip_str)
-
-        def run(command):
-            logger.debug('Shell: %s', command)
-            return self.server.create_task(
-                asyncio.create_subprocess_shell(
-                    command, 
-                    stdout=subprocess.DEVNULL, 
-                    stderr=subprocess.DEVNULL
-                ), 
-                command
-            )
-
-        response = None
-        after_handlers = AfterHandlerList()
-        domain = request.q.qname.idna().rstrip('.')
-        for rule in self.rules:
-            if not rule.test(domain): continue
-
-            rule_type = type(rule)
-            if rule_type == self.IfThenRule:
-                if response is None:
-                    response = rule.exec(request)
-            elif rule_type == self.IfBeforeRule:
-                if response is None:
-                    after_handlers.join(rule.before_handle(request, kwargs))
-            elif rule_type == self.IfAfterRule:
-                after_handlers.join(rule)
-            elif rule_type == self.IfBeforeAfterRule:
-                if response is None:
-                    after_handlers.join(rule.before_handle(request, kwargs))
-                after_handlers.join(rule)
-            if rule.is_ended: break
-
-        if response is None:
-            response = await super().handle(request, **kwargs)
-        return after_handlers.after_handle(response, geoip, ipaddr, run)
+import asyncio
+import logging
+import re
+import enum
+import ipaddress
+import functools
+import subprocess
+
+from collections.abc import Iterable
+
+import dnslib
+import pyparsing
+
+from . import Middleware
+from ..exceptions import InvalidConfig
+from ..helpers import split_domain
+
+
+logger = logging.getLogger(__name__)
+
+
+opt_comma = pyparsing.Suppress(pyparsing.Opt(','))
+
+_ipv4_literal = pyparsing.common.ipv4_address
+
+_ipv6_literal = pyparsing.common.ipv6_address
+
+_ipv4_cidr_literal = _ipv4_literal + '/' + pyparsing.Word(pyparsing.nums, max=2)
+
+_ipv6_cidr_literal = _ipv6_literal + '/' + pyparsing.Word(pyparsing.nums, max=3)
+
+ip_literal = pyparsing.Combine(_ipv4_literal | _ipv6_literal)\
+    .set_name('ip address')\
+    .set_parse_action(lambda tokens: ipaddress.ip_address(tokens[0]))
+
+ip_cidr_literal = pyparsing.Combine(_ipv4_cidr_literal | _ipv6_cidr_literal)\
+    .set_name('CIDR')\
+    .set_parse_action(lambda tokens: ipaddress.ip_network(tokens[0], False))
+
+ip_cidr_literal_list = (pyparsing.Suppress('(') + pyparsing.OneOrMore(ip_cidr_literal + opt_comma) + pyparsing.Suppress(')'))\
+    .set_name('list of CIDRs')\
+    .set_parse_action(lambda tokens: tuple(tokens))
+
+country_code_literal = pyparsing.Word(pyparsing.alphas, exact=2).set_name('country code')
+
+domain_literal = pyparsing.Word(pyparsing.alphanums + '.-').set_name('domain')\
+    .set_parse_action(lambda tokens: tokens[0].lower())
+
+domain_literal_set = (pyparsing.Suppress('(') + pyparsing.OneOrMore(domain_literal + opt_comma) + pyparsing.Suppress(')'))\
+    .set_name('set of domains')\
+    .set_parse_action(lambda tokens: set(map(lambda _: _.strip('.'), tokens)))
+
+domain_literal_list = (pyparsing.Suppress('(') + pyparsing.OneOrMore(domain_literal + opt_comma) + pyparsing.Suppress(')'))\
+    .set_name('list of domains')\
+    .set_parse_action(lambda tokens: tuple(tokens))
+
+ip_literal_list = (pyparsing.Suppress('(') + pyparsing.OneOrMore(ip_literal + opt_comma) + pyparsing.Suppress(')'))\
+    .set_name('list of ip addresses')\
+    .set_parse_action(lambda tokens: tuple(tokens))
+
+ip_literal_set = (pyparsing.Suppress('(') + pyparsing.OneOrMore(ip_literal + opt_comma) + pyparsing.Suppress(')'))\
+    .set_name('set of ip addresses')\
+    .set_parse_action(lambda tokens: set(tokens))
+
+proxy_literal = pyparsing.Regex(r'(http|socks5):\/\/([\w\.-:@%]+)').set_name('proxy')\
+    .set_parse_action(lambda tokens: tokens[0])
+
+always_literal = pyparsing.Literal('always').set_name('always')\
+    .set_parse_action(lambda _: True)
+
+
+def _and_op(op, tokens):
+    return op, tuple(filter(lambda it: it != 'and', tokens))
+
+
+def _or_op(op, tokens):
+    return op, tuple(filter(lambda it: it != 'or', tokens))
+
+
+def _response_add_answers(response, ip_addrs, top=False):
+    hostname = response.q.qname.idna().rstrip('.')
+    qtype = response.q.qtype
+    if not isinstance(ip_addrs, Iterable):
+        ip_addrs = (ip_addrs, )
+
+    if qtype == dnslib.QTYPE.AAAA:
+        records = [
+            dnslib.RR(hostname, qtype, rdata=dnslib.AAAA(str(ip))) 
+            for ip in ip_addrs if isinstance(ip, ipaddress.IPv6Address)
+        ]
+    elif qtype == dnslib.QTYPE.A:
+        records = [
+            dnslib.RR(hostname, qtype, rdata=dnslib.A(str(ip))) 
+            for ip in ip_addrs if isinstance(ip, ipaddress.IPv4Address)
+        ]
+    else:
+        return response
+    if top:
+        records.extend(response.rr)
+        response.rr = records
+        response.set_header_qa()
+    else:
+        response.add_answer(*records)
+    return response
+
+
+def _response_nxdomain(response):
+    response.rr = []
+    response.set_header_qa()
+    response.header.rcode = dnslib.RCODE.NXDOMAIN
+    return response
+
+
+def _is_a_aaaa(request):
+    return request.q.qtype in (dnslib.QTYPE.AAAA, dnslib.QTYPE.A)
+
+
+class OpCode(enum.Enum):
+    NOT = enum.auto()
+    AND = enum.auto()
+    OR = enum.auto()
+    DOMAIN_CONTAINS = enum.auto()
+    DOMAIN_NOT_CONTAINS = enum.auto()
+    DOMAIN_EQ = enum.auto()
+    DOMAIN_NOT_EQ = enum.auto()
+    DOMAIN_STARTS_WITH = enum.auto()
+    DOMAIN_STARTS_WITHOUT = enum.auto()
+    DOMAIN_ENDS_WITH = enum.auto()
+    DOMAIN_ENDS_WITHOUT = enum.auto()
+    DOMAIN_MATCH = enum.auto()
+    BLOCK = enum.auto()
+    RETURN = enum.auto()
+    UPSTREAM_GROUP_SET = enum.auto()
+    UPSTREAM_NAME_SET = enum.auto()
+    DOMAIN_REPLACE = enum.auto()
+    PROXY_SET = enum.auto()
+    FIRST = enum.auto()
+    LAST = enum.auto()
+    IP_IN = enum.auto()
+    IP_NOT_IN = enum.auto()
+    IP_EQ = enum.auto()
+    IP_NOT_EQ = enum.auto()
+    GEOIP_EQ = enum.auto()
+    GEOIP_NOT_EQ = enum.auto()
+    ANY_IP_IN = enum.auto()
+    ANY_IP_NOT_IN = enum.auto()
+    ANY_IP_EQ = enum.auto()
+    ANY_IP_NOT_EQ = enum.auto()
+    ANY_GEOIP_EQ = enum.auto()
+    ANY_GEOIP_NOT_EQ = enum.auto()
+    ALL_IP_IN = enum.auto()
+    ALL_IP_NOT_IN = enum.auto()
+    ALL_IP_EQ = enum.auto()
+    ALL_IP_NOT_EQ = enum.auto()
+    ALL_GEOIP_EQ = enum.auto()
+    ALL_GEOIP_NOT_EQ = enum.auto()
+    RECORD_ADD = enum.auto()
+    RECORD_ADD_IF = enum.auto()
+    RECORD_APPEND = enum.auto()
+    RECORD_APPEND_IF = enum.auto()
+    RECORD_INSERT = enum.auto()
+    RECORD_INSERT_IF = enum.auto()
+    RECORD_REMOVE_WHERE = enum.auto()
+    RECORD_REPLACE_WHERE = enum.auto()
+    RUN_WHERE = enum.auto()
+    BLOCK_IF = enum.auto()
+    RETURN_IF = enum.auto()
+
+    def __repr__(self):
+        return self.name
+
+
+class RuleIfParser:
+    class IfExpr:
+        def __init__(self, ast):
+            self.ast = ast
+
+        def __repr__(self):
+            return repr(self.ast)
+
+        def test(self, domain):
+            def _test(ast):
+                if not isinstance(ast, tuple):
+                    return ast
+                opcode = ast[0]
+                if opcode == OpCode.AND:
+                    return all(map(_test, ast[1]))
+                elif opcode == OpCode.OR:
+                    return any(map(_test, ast[1]))
+                elif opcode == OpCode.NOT:
+                    return not _test(ast[1])
+                elif opcode == OpCode.DOMAIN_CONTAINS:
+                    if isinstance(ast[1], tuple):
+                        return any(map(lambda _: _ in domain, ast[1]))
+                    else:
+                        return ast[1] in domain
+                elif opcode == OpCode.DOMAIN_NOT_CONTAINS:
+                    if isinstance(ast[1], tuple):
+                        return all(map(lambda _: _ not in domain, ast[1]))
+                    else:
+                        return ast[1] not in domain
+                elif opcode == OpCode.DOMAIN_EQ:
+                    if isinstance(ast[1], set):
+                        return domain in ast[1]
+                    else:
+                        return ast[1] == domain
+                elif opcode == OpCode.DOMAIN_NOT_EQ:
+                    if isinstance(ast[1], set):
+                        return domain not in ast[1]
+                    else:
+                        return ast[1] != domain
+                elif opcode == OpCode.DOMAIN_STARTS_WITH:
+                    if isinstance(ast[1], set):
+                        return any(map(lambda _: _ in ast[1], split_domain(domain, False)))
+                    else:
+                        return domain.startswith(ast[1])
+                elif opcode == OpCode.DOMAIN_STARTS_WITHOUT:
+                    if isinstance(ast[1], set):
+                        return all(map(lambda _: _ not in ast[1], split_domain(domain, False)))
+                    else:
+                        return not domain.startswith(ast[1])
+                elif opcode == OpCode.DOMAIN_ENDS_WITH:
+                    if isinstance(ast[1], set):
+                        return any(map(lambda _: _ in ast[1], split_domain(domain)))
+                    else:
+                        return domain.endswith(ast[1])
+                elif opcode == OpCode.DOMAIN_ENDS_WITHOUT:
+                    if isinstance(ast[1], set):
+                        return all(map(lambda _: _ not in ast[1], split_domain(domain)))
+                    else:
+                        return not domain.endswith(ast[1])
+                elif opcode == OpCode.DOMAIN_MATCH:
+                    return re.fullmatch(ast[1], domain) is not None
+                return False
+            return _test(self.ast)
+
+    def __init__(self):
+        expr_domain_contains = ((domain_literal | domain_literal_list) + 'in domain')\
+            .set_name('domain contains expression')\
+            .set_parse_action(lambda tokens: (OpCode.DOMAIN_CONTAINS, tokens[0]))
+        expr_domain_not_contains = ((domain_literal | domain_literal_list) + 'not in domain')\
+            .set_name('domain not contains expression')\
+            .set_parse_action(lambda tokens: (OpCode.DOMAIN_NOT_CONTAINS, tokens[0]))
+        expr_domain_equal = ('domain is' + (domain_literal | domain_literal_set))\
+            .set_name('domain equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.DOMAIN_EQ, tokens[1]))
+        expr_domain_not_equal = ('domain is not' + (domain_literal | domain_literal_set))\
+            .set_name('domain not equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.DOMAIN_NOT_EQ, tokens[1]))
+        expr_domain_starts_with = ('domain starts with' + (domain_literal | domain_literal_set))\
+            .set_name('domain starts with expression')\
+            .set_parse_action(lambda tokens: (OpCode.DOMAIN_STARTS_WITH, tokens[1]))
+        expr_domain_starts_without = ('domain starts without' + (domain_literal | domain_literal_set))\
+            .set_name('domain starts without expression')\
+            .set_parse_action(lambda tokens: (OpCode.DOMAIN_STARTS_WITHOUT, tokens[1]))
+        expr_domain_ends_with = ('domain ends with' + (domain_literal | domain_literal_set))\
+            .set_name('domain ends with expression')\
+            .set_parse_action(lambda tokens: (OpCode.DOMAIN_ENDS_WITH, tokens[1]))
+        expr_domain_ends_without = ('domain ends without' + (domain_literal | domain_literal_set))\
+            .set_name('domain ends without expression')\
+            .set_parse_action(lambda tokens: (OpCode.DOMAIN_ENDS_WITHOUT, tokens[1]))
+        expr_domain_match = ('domain match' + pyparsing.QuotedString('/'))\
+            .set_name('domain match expression')\
+            .set_parse_action(lambda tokens: (OpCode.DOMAIN_MATCH, tokens[1]))
+        expr_simple = (
+            expr_domain_not_contains |
+            expr_domain_contains |
+            expr_domain_not_equal |
+            expr_domain_equal |
+            expr_domain_starts_without |
+            expr_domain_starts_with |
+            expr_domain_ends_without |
+            expr_domain_ends_with |
+            expr_domain_match
+        )
+        expr = pyparsing.Forward()
+        expr <<= pyparsing.infix_notation(expr_simple, [
+            ('not', 1, pyparsing.opAssoc.RIGHT, lambda tokens: (OpCode.NOT, tokens[0][1])),
+            ('and', 2, pyparsing.opAssoc.LEFT, lambda tokens: _and_op(OpCode.AND, tokens[0])),
+            ('or', 2, pyparsing.opAssoc.LEFT, lambda tokens: _or_op(OpCode.OR, tokens[0])),
+        ])
+        self.parser = expr | always_literal
+    
+    def parse(self, source):
+        parse_results = self.parser.parse_string(source, parse_all=True)
+        return self.IfExpr(parse_results[0])
+
+
+class RuleThenParser:
+    class ThenExec:
+        def __repr__(self):
+            return repr(self.ast)
+
+        def __init__(self, ast):
+            self.ast = ast[0]
+
+        def exec(self, request):
+            response = request.reply()
+            _exec = self.ast[0]
+            if _exec == OpCode.BLOCK:
+                response.header.rcode = dnslib.RCODE.NXDOMAIN
+            elif _exec == OpCode.RETURN:
+                ip_addrs = self.ast[1] if isinstance(self.ast[1], tuple) else (self.ast[1], )
+                _response_add_answers(response, ip_addrs)
+            return response
+
+    def __init__(self):
+        stm_block = pyparsing.Literal('block')\
+            .set_name('block statement')\
+            .set_parse_action(lambda _: (OpCode.BLOCK, ))
+        stm_return = ('return' + (ip_literal_list | ip_literal))\
+            .set_name('return statement')\
+            .set_parse_action(lambda tokens: (OpCode.RETURN, tokens[1]))
+        stm_single = (
+            stm_block |
+            stm_return
+        )
+        self.parser = stm_single
+
+    def parse(self, source):
+        parse_results = self.parser.parse_string(source, parse_all=True)
+        return self.ThenExec(parse_results)
+
+
+class AfterHandler:
+    def after_handle(self, response, geoip, ipaddr, run):
+        return response
+
+
+class ReplacDomainHandler(AfterHandler):
+    def __init__(self, domain):
+        self.domain = domain
+
+    def after_handle(self, response, geoip, ipaddr, run):
+        response.q.qname = self.domain
+        return response
+
+
+class AfterHandlerList:
+    def __init__(self):
+        self.handlers = []
+
+    def join(self, handler):
+        if handler is None or not hasattr(handler, 'after_handle'):
+            return self
+        self.handlers.append(handler)
+        return self
+
+    def after_handle(self, response, geoip, ipaddr, run):
+        for handler in self.handlers:
+            response = handler.after_handle(response, geoip, ipaddr, run)
+        return response
+
+
+class RuleBeforeParser:
+    class BeforeExec:
+        def __repr__(self):
+            return repr(self.ast)
+
+        def __init__(self, ast):
+            self.ast = list(ast)
+
+        def exec(self, request, kwargs):
+            after_handler = None
+            for stm in self.ast:
+                _exec = stm[0]
+                if _exec == OpCode.UPSTREAM_GROUP_SET:
+                    kwargs['upstream_group'] = stm[1]
+                elif _exec == OpCode.UPSTREAM_NAME_SET:
+                    kwargs['upstream_name'] = stm[1]
+                elif _exec == OpCode.DOMAIN_REPLACE:
+                    after_handler = ReplacDomainHandler(request.q.qname)
+                    request.q.qname = stm[1]
+                elif _exec == OpCode.PROXY_SET:
+                    if stm[1] == 'on':
+                        kwargs.pop('proxy', None)
+                    elif stm[1] == 'off':
+                        kwargs['proxy'] = None
+                    else:
+                        kwargs['proxy'] = stm[1]
+            return after_handler
+
+    def __init__(self):
+        upstream_name_literal = pyparsing.Word(pyparsing.alphanums + '.-_')\
+            .set_name('upstream name')
+        upstream_group_literal = pyparsing.Word(pyparsing.alphanums + '.-_')\
+            .set_name('upstream group')
+        stm_upstream_name_set = ('set upstream name to' + upstream_name_literal)\
+            .set_name('set upstream name statement')\
+            .set_parse_action(lambda tokens: (OpCode.UPSTREAM_NAME_SET, tokens[1]))
+        stm_upstream_group_set = ('set upstream group to' + upstream_group_literal)\
+            .set_name('set upstream group statement')\
+            .set_parse_action(lambda tokens: (OpCode.UPSTREAM_GROUP_SET, tokens[1]))
+        stm_domain_replace = ('replace domain by' + domain_literal)\
+            .set_name('replace domain statement')\
+            .set_parse_action(lambda tokens: (OpCode.DOMAIN_REPLACE, tokens[1]))
+        stm_proxy_on = pyparsing.Literal('set proxy on')\
+            .set_name('set proxy on statement')\
+            .set_parse_action(lambda _: (OpCode.PROXY_SET, 'on'))
+        stm_proxy_off = pyparsing.Literal('set proxy off')\
+            .set_name('set proxy off statement')\
+            .set_parse_action(lambda _: (OpCode.PROXY_SET, 'off'))
+        stm_proxy_set = ('set proxy to' + proxy_literal)\
+            .set_name('set proxy to statement')\
+            .set_parse_action(lambda tokens: (OpCode.PROXY_SET, tokens[1]))
+        stm_simple = (
+            stm_upstream_name_set |
+            stm_upstream_group_set |
+            stm_domain_replace |
+            stm_proxy_on |
+            stm_proxy_off |
+            stm_proxy_set
+        )
+        self.parser = pyparsing.OneOrMore(stm_simple + opt_comma)
+
+    def parse(self, source):
+        parse_results = self.parser.parse_string(source, parse_all=True)
+        return self.BeforeExec(parse_results)
+
+
+class RuleAfterParser:
+    class AfterExec:
+        def __init__(self, ast):
+            self.ast = list(ast)
+
+        def __repr__(self):
+            return repr(self.ast)
+
+        def test_record(self, geoip, ipaddr, response, expr_if, idx_rr):
+            idx, rr = idx_rr
+            def test(ast):
+                if not isinstance(ast, tuple):
+                    return ast
+                if rr.rtype not in (dnslib.QTYPE.AAAA, dnslib.QTYPE.A):
+                    return False
+
+                opcode = ast[0]
+                if opcode == OpCode.AND:
+                    return all(map(test, ast[1]))
+                elif opcode == OpCode.OR:
+                    return any(map(test, ast[1]))
+                elif opcode == OpCode.NOT:
+                    return not test(ast[1])
+                elif opcode == OpCode.IP_EQ:
+                    if isinstance(ast[1], set):
+                        return ipaddr(rr) in ast[1]
+                    else:
+                        return ast[1] == ipaddr(rr)
+                elif opcode == OpCode.IP_NOT_EQ:
+                    if isinstance(ast[1], set):
+                        return ipaddr(rr) not in ast[1]
+                    else:
+                        return ast[1] != ipaddr(rr)
+                elif opcode == OpCode.IP_IN:
+                    if isinstance(ast[1], tuple):
+                        return any(map(lambda _: ipaddr(rr) in _, ast[1]))
+                    else:
+                        return ipaddr(rr) in ast[1]
+                elif opcode == OpCode.IP_NOT_IN:
+                    if isinstance(ast[1], tuple):
+                        return all(map(lambda _: ipaddr(rr) not in _, ast[1]))
+                    else:
+                        return ipaddr(rr) not in ast[1]
+                elif opcode == OpCode.GEOIP_EQ:
+                    return geoip(rr) == ast[1].upper()
+                elif opcode == OpCode.GEOIP_NOT_EQ:
+                    return geoip(rr) != ast[1].upper()
+                elif opcode == OpCode.FIRST:
+                    return idx == 0
+                elif opcode == OpCode.LAST:
+                    return idx == len(response.rr) - 1
+                return False
+            return test(expr_if)
+
+        def test_response(self, geoip, ipaddr, expr_if, response):
+            def test(ast):
+                if not isinstance(ast, tuple):
+                    return ast
+
+                opcode = ast[0]
+                if opcode == OpCode.AND:
+                    return all(map(test, ast[1]))
+                elif opcode == OpCode.OR:
+                    return any(map(test, ast[1]))
+                elif opcode == OpCode.NOT:
+                    return not test(ast[1])
+
+                rr = filter(lambda rr: rr.rtype in (dnslib.QTYPE.AAAA, dnslib.QTYPE.A), response.rr)
+                ip_addresses = map(lambda rr: ipaddr(rr), rr)
+                country_codes = map(lambda rr: geoip(rr), rr)
+                if opcode == OpCode.ANY_IP_EQ:
+                    if isinstance(ast[1], set):
+                        return any(map(lambda _: _ in ast[1], ip_addresses))
+                    else:
+                        return any(map(lambda ip: ip == ast[1], ip_addresses))
+                elif opcode == OpCode.ANY_IP_NOT_EQ:
+                    if isinstance(ast[1], set):
+                        return any(map(lambda _: _ not in ast[1], ip_addresses))
+                    else:
+                        return any(map(lambda ip: ip != ast[1], ip_addresses))
+                elif opcode == OpCode.ANY_IP_IN:
+                    if isinstance(ast[1], tuple):
+                        return any(map(lambda ip: any(map(lambda _: ip in _, ast[1])), ip_addresses))
+                    else:
+                        return any(map(lambda ip: ip in ast[1], ip_addresses))
+                elif opcode == OpCode.ANY_IP_NOT_IN:
+                    if isinstance(ast[1], tuple):
+                        return any(map(lambda ip: all(map(lambda _: ip not in _, ast[1])), ip_addresses))
+                    else:
+                        return any(map(lambda ip: ip not in ast[1], ip_addresses))
+                elif opcode == OpCode.ANY_GEOIP_EQ:
+                    return any(map(lambda country_code: country_code == ast[1], country_codes))
+                elif opcode == OpCode.ANY_GEOIP_NOT_EQ:
+                    return any(map(lambda country_code: country_code != ast[1], country_codes))
+                elif opcode == OpCode.ALL_IP_EQ:
+                    if isinstance(ast[1], set):
+                        return all(map(lambda _: _ in ast[1], ip_addresses))
+                    else:
+                        return all(map(lambda ip: ip == ast[1], ip_addresses))
+                elif opcode == OpCode.ALL_IP_NOT_EQ:
+                    if isinstance(ast[1], set):
+                        return all(map(lambda _: _ not in ast[1], ip_addresses))
+                    else:
+                        return all(map(lambda ip: ip != ast[1], ip_addresses))
+                elif opcode == OpCode.ALL_IP_IN:
+                    if isinstance(ast[1], tuple):
+                        return all(map(lambda ip: any(map(lambda _: ip in _, ast[1])), ip_addresses))
+                    else:
+                        return all(map(lambda ip: ip in ast[1], ip_addresses))
+                elif opcode == OpCode.ALL_IP_NOT_IN:
+                    if isinstance(ast[1], tuple):
+                        return all(map(lambda ip: all(map(lambda _: ip not in _, ast[1])), ip_addresses))
+                    else:
+                        return all(map(lambda ip: ip not in ast[1], ip_addresses))
+                elif opcode == OpCode.ALL_GEOIP_EQ:
+                    return all(map(lambda country_code: country_code == ast[1], country_codes))
+                elif opcode == OpCode.ALL_GEOIP_NOT_EQ:
+                    return all(map(lambda country_code: country_code != ast[1], country_codes))
+                return False
+            return test(expr_if)
+
+        def exec(self, response, geoip, ipaddr, run):
+            test_record = functools.partial(self.test_record, geoip, ipaddr, response)
+            test_response = functools.partial(self.test_response, geoip, ipaddr)
+
+            for stm in self.ast:
+                _exec = stm[0]
+                if _exec in (OpCode.RECORD_ADD, OpCode.RECORD_APPEND):
+                    _response_add_answers(response, stm[1])
+                    continue
+                elif _exec == OpCode.RECORD_INSERT:
+                    _response_add_answers(response, stm[1], True)
+                    continue
+
+                expr_if = stm[1]
+                if _exec == OpCode.RECORD_REMOVE_WHERE:
+                    response.rr = list(map(
+                        lambda idx_rr: idx_rr[1],
+                        filter(
+                            lambda idx_rr: not test_record(expr_if, idx_rr), 
+                            enumerate(response.rr)
+                        )
+                    ))
+                    response.set_header_qa()
+                    continue
+                elif _exec == OpCode.RECORD_REPLACE_WHERE:
+                    qtype = response.q.qtype
+                    ip = stm[2]
+                    for idx, rr in enumerate(response.rr):
+                        if not test_record(expr_if, (idx, rr)):
+                            continue
+                        if isinstance(ip, ipaddress.IPv6Address) and qtype == dnslib.QTYPE.AAAA:
+                            rr.rdata = dnslib.AAAA(str(ip))
+                        elif isinstance(ip, ipaddress.IPv4Address) and qtype == dnslib.QTYPE.A:
+                            rr.rdata = dnslib.A(str(ip))
+                    continue
+                elif _exec == OpCode.RUN_WHERE:
+                    cmd = stm[2]
+                    hostname = response.q.qname.idna().rstrip('.')
+                    for idx, rr in enumerate(response.rr):
+                        if not test_record(expr_if, (idx, rr)):
+                            continue
+                        run(cmd.format(ip=rr.rdata, domain=hostname))
+                    continue
+
+                if _exec == OpCode.RETURN_IF:
+                    if test_response(expr_if, response):
+                        response.rr = []
+                        _response_add_answers(response, stm[2])
+                elif _exec == OpCode.BLOCK_IF:
+                    if test_response(expr_if, response):
+                        _response_nxdomain(response)
+                elif _exec in (OpCode.RECORD_ADD_IF, OpCode.RECORD_APPEND_IF):
+                    if test_response(expr_if, response):
+                        _response_add_answers(response, stm[2])
+                elif _exec == OpCode.RECORD_INSERT_IF:
+                    if test_response(expr_if, response):
+                        _response_add_answers(response, stm[2], True)
+            return response
+
+    def __init__(self):
+        expr_first = pyparsing.Literal('first').set_name('first')\
+            .set_parse_action(lambda _: (OpCode.FIRST, ))
+        expr_last = pyparsing.Literal('last').set_name('last')\
+            .set_parse_action(lambda _: (OpCode.LAST, ))
+        expr_ip_in = ('ip in' + (ip_cidr_literal | ip_cidr_literal_list))\
+            .set_name('ip in cidr expression')\
+            .set_parse_action(lambda tokens: (OpCode.IP_IN, tokens[1]))
+        expr_ip_not_in = ('ip not in' + (ip_cidr_literal | ip_cidr_literal_list))\
+            .set_name('ip not in cidr expression')\
+            .set_parse_action(lambda tokens: (OpCode.IP_NOT_IN, tokens[1]))
+        expr_ip_equal = ('ip is' + (ip_literal | ip_literal_set))\
+            .set_name('ip equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.IP_EQ, tokens[1]))
+        expr_ip_not_equal = ('ip is not' + (ip_literal | ip_literal_set))\
+            .set_name('ip not equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.IP_NOT_EQ, tokens[1]))
+        expr_geoip_equal = ('geoip is' + country_code_literal)\
+            .set_name('geoip equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.GEOIP_EQ, tokens[1]))
+        expr_geoip_not_equal = ('geoip is not' + country_code_literal)\
+            .set_name('geoip not equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.GEOIP_NOT_EQ, tokens[1]))
+        expr_any_ip_in = ('any ip in' + (ip_cidr_literal | ip_cidr_literal_list))\
+            .set_name('any ip in cidr expression')\
+            .set_parse_action(lambda tokens: (OpCode.ANY_IP_IN, tokens[1]))
+        expr_any_ip_not_in = ('any ip not in' + (ip_cidr_literal | ip_cidr_literal_list))\
+            .set_name('any ip not in cidr expression')\
+            .set_parse_action(lambda tokens: (OpCode.ANY_IP_NOT_IN, tokens[1]))
+        expr_any_ip_equal = ('any ip is' + (ip_literal | ip_literal_set))\
+            .set_name('any ip equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.ANY_IP_EQ, tokens[1]))
+        expr_any_ip_not_equal = ('any ip is not' + (ip_literal | ip_literal_set))\
+            .set_name('any ip not equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.ANY_IP_NOT_EQ, tokens[1]))
+        expr_any_geoip_equal = ('any geoip is' + country_code_literal)\
+            .set_name('any geoip equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.ANY_GEOIP_EQ, tokens[1]))
+        expr_any_geoip_not_equal = ('any geoip is not' + country_code_literal)\
+            .set_name('any geoip not equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.ANY_GEOIP_NOT_EQ, tokens[1]))
+        expr_all_ip_in = ('all ip in' + (ip_cidr_literal | ip_cidr_literal_list))\
+            .set_name('all ip in cidr expression')\
+            .set_parse_action(lambda tokens: (OpCode.ALL_IP_IN, tokens[1]))
+        expr_all_ip_not_in = ('all ip not in' + (ip_cidr_literal | ip_cidr_literal_list))\
+            .set_name('all ip not in cidr expression')\
+            .set_parse_action(lambda tokens: (OpCode.ALL_IP_NOT_IN, tokens[1]))
+        expr_all_ip_equal = ('all ip is' + (ip_literal | ip_literal_set))\
+            .set_name('all ip equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.ALL_IP_EQ, tokens[1]))
+        expr_all_ip_not_equal = ('all ip is not' + (ip_literal | ip_literal_set))\
+            .set_name('all ip not equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.ALL_IP_NOT_EQ, tokens[1]))
+        expr_all_geoip_equal = ('all geoip is' + country_code_literal)\
+            .set_name('all geoip equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.ALL_GEOIP_EQ, tokens[1]))
+        expr_all_geoip_not_equal = ('all geoip is not' + country_code_literal)\
+            .set_name('all geoip not equal expression')\
+            .set_parse_action(lambda tokens: (OpCode.ALL_GEOIP_NOT_EQ, tokens[1]))
+        expr_simple = (
+            expr_first |
+            expr_last |
+            expr_ip_not_in |
+            expr_ip_in |
+            expr_ip_not_equal |
+            expr_ip_equal |
+            expr_geoip_not_equal |
+            expr_geoip_equal
+        )
+        expr_complex = (
+            expr_any_ip_in |
+            expr_any_ip_not_in |
+            expr_any_ip_equal |
+            expr_any_ip_not_equal |
+            expr_any_geoip_not_equal |
+            expr_any_geoip_equal |
+            expr_all_ip_in |
+            expr_all_ip_not_in |
+            expr_all_ip_equal |
+            expr_all_ip_not_equal |
+            expr_all_geoip_not_equal |
+            expr_all_geoip_equal
+        )
+        expr_if = pyparsing.Forward()
+        expr_if <<= (pyparsing.infix_notation(expr_complex, [
+            ('not', 1, pyparsing.opAssoc.RIGHT, lambda tokens: (OpCode.NOT, tokens[0][1])),
+            ('and', 2, pyparsing.opAssoc.LEFT, lambda tokens: _and_op(OpCode.AND, tokens[0])),
+            ('or', 2, pyparsing.opAssoc.LEFT, lambda tokens: _or_op(OpCode.OR, tokens[0])),
+        ]) | always_literal)
+        expr_where = pyparsing.Forward()
+        expr_where <<= (pyparsing.infix_notation(expr_simple, [
+            ('not', 1, pyparsing.opAssoc.RIGHT, lambda tokens: (OpCode.NOT, tokens[0][1])),
+            ('and', 2, pyparsing.opAssoc.LEFT, lambda tokens: _and_op(OpCode.AND, tokens[0])),
+            ('or', 2, pyparsing.opAssoc.LEFT, lambda tokens: _or_op(OpCode.OR, tokens[0])),
+        ]) | always_literal)
+        stm_record_add = ('add record' + (ip_literal | ip_literal_list))\
+            .set_name('add record statement')\
+            .set_parse_action(lambda tokens: (OpCode.RECORD_ADD, tokens[1]))
+        stm_record_add_if = ('add record' + (ip_literal | ip_literal_list) + 'if' + expr_if)\
+            .set_name('add record if statement')\
+            .set_parse_action(lambda tokens: (OpCode.RECORD_ADD_IF, tokens[3], tokens[1]))
+        stm_record_append = ('append record' + (ip_literal | ip_literal_list))\
+            .set_name('append record statement')\
+            .set_parse_action(lambda tokens: (OpCode.RECORD_APPEND, tokens[1]))
+        stm_record_append_if = ('append record' + (ip_literal | ip_literal_list) + 'if' + expr_if)\
+            .set_name('append record if statement')\
+            .set_parse_action(lambda tokens: (OpCode.RECORD_APPEND_IF, tokens[3], tokens[1]))
+        stm_record_insert = ('insert record' + (ip_literal | ip_literal_list))\
+            .set_name('insert record statement')\
+            .set_parse_action(lambda tokens: (OpCode.RECORD_INSERT, tokens[1]))
+        stm_record_insert_if = ('insert record' + (ip_literal | ip_literal_list) + 'if' + expr_if)\
+            .set_name('insert record if statement')\
+            .set_parse_action(lambda tokens: (OpCode.RECORD_INSERT_IF, tokens[3], tokens[1]))
+        stm_record_remove_where = ('remove record where' + expr_where)\
+            .set_name('remove record where statement')\
+            .set_parse_action(lambda tokens: (OpCode.RECORD_REMOVE_WHERE, *tokens[1:]))
+        stm_record_replace_where = ('replace record by' + ip_literal + 'where' + expr_where)\
+            .set_name('replace record where statement')\
+            .set_parse_action(lambda tokens: (OpCode.RECORD_REPLACE_WHERE, tokens[3], tokens[1]))
+        stm_run_command_where = ('run' + pyparsing.QuotedString('"') + 'where' + expr_where)\
+            .set_name('run command where statement')\
+            .set_parse_action(lambda tokens: (OpCode.RUN_WHERE, tokens[3], tokens[1]))
+        stm_simple = (
+            stm_record_add_if |
+            stm_record_add |
+            stm_record_append_if |
+            stm_record_append |
+            stm_record_insert_if |
+            stm_record_insert |
+            stm_record_remove_where |
+            stm_record_replace_where |
+            stm_run_command_where
+        )
+        stm_block_if = ('block if' + expr_if)\
+            .set_name('block if statement')\
+            .set_parse_action(lambda tokens: (OpCode.BLOCK_IF, tokens[1]))
+        stm_return_if = ('return' + (ip_literal_list | ip_literal) + 'if' + expr_if)\
+            .set_name('return if statement')\
+            .set_parse_action(lambda tokens: (OpCode.RETURN_IF, tokens[3], tokens[1]))
+        stm_single = (
+            stm_block_if |
+            stm_return_if
+        )
+        self.parser = stm_single | pyparsing.OneOrMore(stm_simple + opt_comma)
+
+    def parse(self, source):
+        parse_results = self.parser.parse_string(source, parse_all=True)
+        return self.AfterExec(parse_results)
+
+
+class RulesMiddleware(Middleware):
+    class Rule:
+        def test(self, domain):
+            return self.if_expr.test(domain)
+
+    class IfThenRule(Rule):
+        def __init__(self, if_expr, then_exec, is_ended):
+            self.if_expr = if_expr
+            self.then_exec = then_exec
+            self.is_ended = is_ended
+
+        def exec(self, request):
+            return self.then_exec.exec(request)
+
+    class IfBeforeRule(Rule):
+        def __init__(self, if_expr, before, is_ended):
+            self.if_expr = if_expr
+            self.before = before
+            self.is_ended = is_ended
+
+        def before_handle(self, request, kwargs):
+            return self.before.exec(request, kwargs)
+
+    class IfAfterRule(Rule):
+        def __init__(self, if_expr, after, is_ended):
+            self.if_expr = if_expr
+            self.after = after
+            self.is_ended = is_ended
+
+        def after_handle(self, response, geoip, ipaddr, run):
+            return self.after.exec(response, geoip, ipaddr, run)
+
+    class IfBeforeAfterRule(IfBeforeRule, IfAfterRule):
+        def __init__(self, if_expr, before, after, is_ended):
+            self.if_expr = if_expr
+            self.before = before
+            self.after = after
+            self.is_ended = is_ended
+
+    def __init__(self, *rules):
+        self.if_parser = RuleIfParser()
+        self.then_parser = RuleThenParser()
+        self.before_parser = RuleBeforeParser()
+        self.after_parser = RuleAfterParser()
+        self.rules = [self._parse_rule(rule) for rule in rules]
+
+    def _parse_rule(self, rule):
+        if 'end' not in rule:
+            rule['end'] = False
+        try:
+            len_of_rule = len(rule)
+            if len_of_rule == 3:
+                if 'then' in rule:
+                    return self.IfThenRule(
+                        self.if_parser.parse(rule['if']),
+                        self.then_parser.parse(rule['then']),
+                        rule['end']
+                    )
+                elif 'before' in rule:
+                    return self.IfBeforeRule(
+                        self.if_parser.parse(rule['if']),
+                        self.before_parser.parse(rule['before']),
+                        rule['end']
+                    )
+                else:
+                    return self.IfAfterRule(
+                        self.if_parser.parse(rule['if']),
+                        self.after_parser.parse(rule['after']),
+                        rule['end']
+                    )
+            elif len_of_rule == 4:
+                return self.IfBeforeAfterRule(
+                    self.if_parser.parse(rule['if']),
+                    self.before_parser.parse(rule['before']),
+                    self.after_parser.parse(rule['after']),
+                    rule['end']
+                )
+            raise KeyError()
+        except pyparsing.exceptions.ParseException as exc:
+            raise InvalidConfig('Invalid rules config: %s' % (exc, ))
+        except KeyError:
+            raise InvalidConfig('A rule must match [if/then] or [if/before/after] pattern')
+
+    def _geoip(self, ip):
+        result = self.geoip_reader.get(ip)                            
+        return result['country']['iso_code'] if result else None
+
+    async def _query(self, request, **kwargs):
+        response = await super().handle(request, **kwargs)
+        ips = map(lambda r: str(r.rdata), response.rr)
+        geoips = map(self._geoip, ips)
+        return response, ips, geoips
+
+    @property
+    def geoip_reader(self):
+        if not hasattr(self, '_geoip_reader'):
+            self._geoip_reader = self.server.open_geoip()
+        return self._geoip_reader
+
+    async def handle(self, request, **kwargs):
+        cached_geoips = dict()
+        cached_ipaddrs = dict()
+        def geoip(record):
+            ip_str = str(record.rdata)
+            if ip_str in cached_geoips:
+                return cached_geoips[ip_str]
+            cached_geoips[ip_str] = country_code = self._geoip(ip_str)
+            return country_code
+        
+        def ipaddr(record):
+            ip_str = str(record.rdata)
+            if ip_str in cached_ipaddrs:
+                return cached_ipaddrs[ip_str]
+            if record.rtype == dnslib.QTYPE.A:
+                return ipaddress.IPv4Address(ip_str)
+            elif record.rtype == dnslib.QTYPE.AAAA:
+                return ipaddress.IPv6Address(ip_str)
+
+        def run(command):
+            logger.debug('Shell: %s', command)
+            return self.server.create_task(
+                asyncio.create_subprocess_shell(
+                    command, 
+                    stdout=subprocess.DEVNULL, 
+                    stderr=subprocess.DEVNULL
+                ), 
+                command
+            )
+
+        response = None
+        after_handlers = AfterHandlerList()
+        domain = request.q.qname.idna().rstrip('.')
+        for rule in self.rules:
+            if not rule.test(domain): continue
+
+            rule_type = type(rule)
+            if rule_type == self.IfThenRule:
+                if response is None:
+                    response = rule.exec(request)
+            elif rule_type == self.IfBeforeRule:
+                if response is None:
+                    after_handlers.join(rule.before_handle(request, kwargs))
+            elif rule_type == self.IfAfterRule:
+                after_handlers.join(rule)
+            elif rule_type == self.IfBeforeAfterRule:
+                if response is None:
+                    after_handlers.join(rule.before_handle(request, kwargs))
+                after_handlers.join(rule)
+            if rule.is_ended: break
+
+        if response is None:
+            response = await super().handle(request, **kwargs)
+        return after_handlers.after_handle(response, geoip, ipaddr, run)
```

### Comparing `dnspooh-1.3.1/dnspooh/pool.py` & `dnspooh-1.3.2/dnspooh/pool.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-import asyncio
-import ssl
-import logging
-
-import certifi
-
-from .helpers import Scheme
-
-
-logger = logging.getLogger(__name__)
-
-
-class PoolStreamReaderProtocol(asyncio.StreamReaderProtocol):
-    def eof_received(self):
-        super().eof_received()
-        return False
-
-    def data_received(self, data):
-        return super().data_received(data)
-
-    def connection_made(self, transport):
-        return super().connection_made(transport)
-
-    def connection_lost(self, exc):
-        super().connection_lost(exc)
-        if self._connection_lost_cb and self.conn:
-            self.conn.exc = exc
-            self._connection_lost_cb(self.conn)
-
-    def __init__(self, stream_reader, on_connection_lost=None, **kwds):
-        self._connection_lost_cb = on_connection_lost
-        self.conn = None
-        super().__init__(stream_reader, **kwds)
-
-
-class Connection:
-    def __init__(self, name, reader, writer, udp_tunnel=None):
-        self.name = name
-        self.reader = reader
-        self.writer = writer
-        self.udp_tunnel = udp_tunnel
-        self.exc = None
-        self.idle = True
-        self._is_wild = True
-
-    def is_wild(self):
-        return self._is_wild
-
-    def register(self):
-        self._is_wild = False
-        self.writer.transport.get_protocol().conn = self
-
-    def __enter__(self):
-        self.idle = False
-        return self
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        if exc_type is not None or self.is_wild():
-            self.writer.transport.close()
-        self.idle = True
-
-    def __repr__(self):
-        return self.name
-
-    def is_closing(self):
-        return self.writer.transport.is_closing()
-
-    def udp_tunnel_enabled(self):
-        return self.udp_tunnel is not None
-
-    def close(self):
-        return self.writer.transport.close()
-
-    def abort(self):
-        return self.writer.transport.abort()
-    
-    def to_json(self):
-        return self.name
-
-
-class Pool:
-    DEFAULT_LIMIT = 2 ** 16
-    DEFAULT_SIZE = 2 ** 10
-
-    def __init__(self, loop=None, size=DEFAULT_SIZE):
-        self.size = size
-        self.total = 0
-        self.connections = dict()
-        self.loop = asyncio.get_running_loop() if loop is None else loop
-
-    def add(self, conn):
-        if self.DEFAULT_SIZE <= self.total:
-            return False
-
-        if conn.is_closing():
-            raise ConnectionError('Fail to connect "%s"' % (conn.name, ))
-
-        if conn.name in self.connections:
-            if conn in self.connections[conn.name]:
-                return False
-            self.connections[conn.name].add(conn)
-        else:
-            self.connections[conn.name] = set([conn])
-        self.total += 1
-        conn.register()
-        logger.debug('Add "%s" to connection pool', conn.name)
-        return True
-
-    def remove(self, conn):
-        if conn.name in self.connections:
-            if conn in self.connections[conn.name]:
-                self.connections[conn.name].remove(conn)
-                self.total -= 1
-                return True
-
-        return False
-
-    def get(self, conn_name):
-        if conn_name not in self.connections:
-            return
-        for conn in self.connections[conn_name]:
-            if conn.idle:
-                return conn
-        return
-
-    def on_connection_lost(self, conn):
-        self.remove(conn)
-        logger.debug('Remove "%s" from connection pool', conn.name)
-
-    async def connect(self, host, port, 
-                      scheme=Scheme.TCP, proxy=None, 
-                      limit=DEFAULT_LIMIT, pooled=True, **kwds):
-        conn_name = _make_conn_name(host, port, scheme, proxy)
-        conn = self.get(conn_name)
-        if conn:
-            return conn
-
-        reader = asyncio.StreamReader(limit=limit, loop=self.loop)
-        protocol = PoolStreamReaderProtocol(reader, self.on_connection_lost, loop=self.loop)
-        if proxy:
-            try:
-                transport, _ = await self.loop.create_connection(
-                    lambda: protocol, proxy.host, proxy.port, **kwds)
-            except OSError as exc:
-                raise ConnectionError('Cannot connect to proxy "%s:%d": %s' % (proxy.host, proxy.port, exc))
-            writer = asyncio.StreamWriter(transport, protocol, reader, self.loop)
-            if scheme == Scheme.UDP:
-                conn = Connection(
-                    conn_name, reader, writer, 
-                    await proxy.make_udp_tunnel(reader, writer, (host, port))
-                )
-                if pooled: self.add(conn)
-                return conn
-            if not await proxy.handshake(reader, writer, (host, port)):
-                raise ConnectionError('Failed to handshake with proxy "%s"' % (proxy.url, ))
-        elif scheme == Scheme.UDP:
-            raise ConnectionError('Naked UDP protocol does not supported')
-        else:
-            try:
-                transport, _ = await self.loop.create_connection(
-                    lambda: protocol, host, port, **kwds)
-            except OSError as exc:
-                raise ConnectionError('Cannot connect to server "%s:%d": %s' % (host, port, exc))
-            writer = asyncio.StreamWriter(transport, protocol, reader, self.loop)
-
-        if scheme == Scheme.TLS:
-            try:
-                ssl_context = ssl.create_default_context(cafile=certifi.where())
-                transport = await self.loop.start_tls(transport, protocol, ssl_context)
-                writer = asyncio.StreamWriter(transport, protocol, reader, self.loop)
-            except ssl.SSLError as exc:
-                raise ConnectionError('Failed to establish tls connection: %s' % (exc, ))
-
-        conn = Connection(conn_name, reader, writer)
-        if pooled: self.add(conn)
-        return conn
-        
-    def dispose(self):
-        for conn_set in self.connections.values():
-            for conn in conn_set:
-                conn.abort()
-
-    def to_json(self):
-        return [{
-            'name': name,
-            'size': len(conn_set)
-        } for name, conn_set in self.connections.items()]
-
-
-def _make_conn_name(host, port, scheme, proxy):
-    name = '%s://%s:%d' % (scheme.name.lower(), host, port)
-    return name if proxy is None else '%s/%s' % (proxy.url, name)
+import asyncio
+import ssl
+import logging
+
+import certifi
+
+from .helpers import Scheme
+
+
+logger = logging.getLogger(__name__)
+
+
+class PoolStreamReaderProtocol(asyncio.StreamReaderProtocol):
+    def eof_received(self):
+        super().eof_received()
+        return False
+
+    def data_received(self, data):
+        return super().data_received(data)
+
+    def connection_made(self, transport):
+        return super().connection_made(transport)
+
+    def connection_lost(self, exc):
+        super().connection_lost(exc)
+        if self._connection_lost_cb and self.conn:
+            self.conn.exc = exc
+            self._connection_lost_cb(self.conn)
+
+    def __init__(self, stream_reader, on_connection_lost=None, **kwds):
+        self._connection_lost_cb = on_connection_lost
+        self.conn = None
+        super().__init__(stream_reader, **kwds)
+
+
+class Connection:
+    def __init__(self, name, reader, writer, udp_tunnel=None):
+        self.name = name
+        self.reader = reader
+        self.writer = writer
+        self.udp_tunnel = udp_tunnel
+        self.exc = None
+        self.idle = True
+        self._is_wild = True
+
+    def is_wild(self):
+        return self._is_wild
+
+    def register(self):
+        self._is_wild = False
+        self.writer.transport.get_protocol().conn = self
+
+    def __enter__(self):
+        self.idle = False
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        if exc_type is not None or self.is_wild():
+            self.writer.transport.close()
+        self.idle = True
+
+    def __repr__(self):
+        return self.name
+
+    def is_closing(self):
+        return self.writer.transport.is_closing()
+
+    def udp_tunnel_enabled(self):
+        return self.udp_tunnel is not None
+
+    def close(self):
+        return self.writer.transport.close()
+
+    def abort(self):
+        return self.writer.transport.abort()
+    
+    def to_json(self):
+        return self.name
+
+
+class Pool:
+    DEFAULT_LIMIT = 2 ** 16
+    DEFAULT_SIZE = 2 ** 10
+
+    def __init__(self, loop=None, size=DEFAULT_SIZE):
+        self.size = size
+        self.total = 0
+        self.connections = dict()
+        self.loop = asyncio.get_running_loop() if loop is None else loop
+
+    def add(self, conn):
+        if self.DEFAULT_SIZE <= self.total:
+            return False
+
+        if conn.is_closing():
+            raise ConnectionError('Fail to connect "%s"' % (conn.name, ))
+
+        if conn.name in self.connections:
+            if conn in self.connections[conn.name]:
+                return False
+            self.connections[conn.name].add(conn)
+        else:
+            self.connections[conn.name] = set([conn])
+        self.total += 1
+        conn.register()
+        logger.debug('Add "%s" to connection pool', conn.name)
+        return True
+
+    def remove(self, conn):
+        if conn.name in self.connections:
+            if conn in self.connections[conn.name]:
+                self.connections[conn.name].remove(conn)
+                self.total -= 1
+                return True
+
+        return False
+
+    def get(self, conn_name):
+        if conn_name not in self.connections:
+            return
+        for conn in self.connections[conn_name]:
+            if conn.idle:
+                return conn
+        return
+
+    def on_connection_lost(self, conn):
+        self.remove(conn)
+        logger.debug('Remove "%s" from connection pool', conn.name)
+
+    async def connect(self, host, port, 
+                      scheme=Scheme.TCP, proxy=None, 
+                      limit=DEFAULT_LIMIT, pooled=True, **kwds):
+        conn_name = _make_conn_name(host, port, scheme, proxy)
+        conn = self.get(conn_name)
+        if conn:
+            return conn
+
+        reader = asyncio.StreamReader(limit=limit, loop=self.loop)
+        protocol = PoolStreamReaderProtocol(reader, self.on_connection_lost, loop=self.loop)
+        if proxy:
+            try:
+                transport, _ = await self.loop.create_connection(
+                    lambda: protocol, proxy.host, proxy.port, **kwds)
+            except OSError as exc:
+                raise ConnectionError('Cannot connect to proxy "%s:%d": %s' % (proxy.host, proxy.port, exc))
+            writer = asyncio.StreamWriter(transport, protocol, reader, self.loop)
+            if scheme == Scheme.UDP:
+                conn = Connection(
+                    conn_name, reader, writer, 
+                    await proxy.make_udp_tunnel(reader, writer, (host, port))
+                )
+                if pooled: self.add(conn)
+                return conn
+            if not await proxy.handshake(reader, writer, (host, port)):
+                raise ConnectionError('Failed to handshake with proxy "%s"' % (proxy.url, ))
+        elif scheme == Scheme.UDP:
+            raise ConnectionError('Naked UDP protocol does not supported')
+        else:
+            try:
+                transport, _ = await self.loop.create_connection(
+                    lambda: protocol, host, port, **kwds)
+            except OSError as exc:
+                raise ConnectionError('Cannot connect to server "%s:%d": %s' % (host, port, exc))
+            writer = asyncio.StreamWriter(transport, protocol, reader, self.loop)
+
+        if scheme == Scheme.TLS:
+            try:
+                ssl_context = ssl.create_default_context(cafile=certifi.where())
+                transport = await self.loop.start_tls(transport, protocol, ssl_context)
+                writer = asyncio.StreamWriter(transport, protocol, reader, self.loop)
+            except ssl.SSLError as exc:
+                raise ConnectionError('Failed to establish tls connection: %s' % (exc, ))
+
+        conn = Connection(conn_name, reader, writer)
+        if pooled: self.add(conn)
+        return conn
+        
+    def dispose(self):
+        for conn_set in self.connections.values():
+            for conn in conn_set:
+                conn.abort()
+
+    def to_json(self):
+        return [{
+            'name': name,
+            'size': len(conn_set)
+        } for name, conn_set in self.connections.items()]
+
+
+def _make_conn_name(host, port, scheme, proxy):
+    name = '%s://%s:%d' % (scheme.name.lower(), host, port)
+    return name if proxy is None else '%s/%s' % (proxy.url, name)
```

### Comparing `dnspooh-1.3.1/dnspooh/proxy.py` & `dnspooh-1.3.2/dnspooh/proxy.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,248 +1,248 @@
-import base64
-import struct
-import ipaddress
-
-from urllib.parse import urlsplit
-
-from .helpers import s_addr, Scheme
-
-
-DEFAULT_HTTP_PROXY_PORT = 8080
-
-DEFAULT_SOCKS5_PROXY_PORT = 1080
-
-class Proxy:
-    def __init__(self, url, hostname, port, host=None, username=None, password=None):
-        self.url = url
-        self.hostname = hostname
-        self.port = port
-        self.host = host
-        self.username = username
-        self.password = password
-
-    def __repr__(self):
-        return self.url
-    
-    def to_json(self):
-        return self.__repr__()
-
-    def has_auth(self):
-        return self.username is not None and \
-               self.password is not None
-
-    def udp_tunnel_enabled(self):
-        return False
-
-    async def handshake(self, reader, writer, remote_addr):
-        raise NotImplementedError()
-
-
-class HttpProxy(Proxy):
-    async def handshake(self, reader, writer, remote_addr):
-        if self.has_auth():
-            credentials = base64.b64encode(
-                ('%s:%s' % (self.username, self.password)).encode()
-            ).decode()
-            request = 'CONNECT %s:%s HTTP/1.1\r\n' % remote_addr
-            request += 'Proxy-Authorization: basic %s\r\n\r\n' % (credentials, )
-        else:
-            request = 'CONNECT %s:%s HTTP/1.1\r\n\r\n' % remote_addr
-
-        writer.write(request.encode())
-        await writer.drain()
-        response = await reader.readuntil(b'\r\n\r\n')
-        return response.startswith(b'HTTP/1.1 200')
-
-
-class Socks5Proxy(Proxy):
-    VERSION = 5
-
-    AUTH_METHOD = 2
-
-    NONE_METHOD = 0
-
-    AUTH_SUCCESS = 0
-
-    CMD_CONNECT = 1
-
-    CMD_UDP_ASSOCIATE = 3
-
-    ATYP_IPV4 = 1
-
-    ATYP_IPV6 = 4
-
-    REP_SUCCESS = 0
-
-    class UDPTunnel:
-        def __init__(self, addr):
-            self.addr = addr
-
-        def parse(self, data, src_addr):
-            _, _, atype = struct.unpack('!H2B', data[:4])
-            if atype == Socks5Proxy.ATYP_IPV4:
-                _from_addr, from_port = struct.unpack('!4sH', data[4:10])
-                from_addr = (str(ipaddress.IPv4Address(_from_addr)), from_port)
-                entity_data = data[10:]
-            elif atype == Socks5Proxy.ATYP_IPV6:
-                _from_addr, from_port = struct.unpack('!16sH', data[4:22])
-                from_addr = (str(ipaddress.IPv6Address(_from_addr)), from_port)
-                entity_data = data[22:]
-            else:
-                raise ValueError('Invalid ATYPE %d received' % atype)
-            if from_addr != src_addr:
-                raise ValueError('Source address %s does not match' % s_addr(from_addr))
-
-            return entity_data
-
-        def pack(self, data, dst_addr):
-            ip, port = dst_addr
-            ip_addr = ipaddress.ip_address(ip)
-            if isinstance(ip_addr, ipaddress.IPv4Address):
-                pack_header = struct.pack(
-                    '!H2B4sH', 0, 0, 
-                    Socks5Proxy.ATYP_IPV4,
-                    ip_addr.packed, 
-                    port
-                )
-            elif isinstance(ip_addr, ipaddress.IPv6Address):
-                pack_header = struct.pack(
-                    '!H2B16sH', 0, 0, 
-                    Socks5Proxy.ATYP_IPV6,
-                    ip_addr.packed, 
-                    port
-                )
-            else:
-                raise ValueError('Invalid destination address "%s"' % ip)
-
-            return pack_header + data
-
-    def udp_tunnel_enabled(self):
-        return True
-
-    async def _handshake(self, reader, writer, remote_addr, scheme=Scheme.TCP):
-        writer.write(struct.pack('!3B', self.VERSION, 1, self.AUTH_METHOD))
-        await writer.drain()
-        server_version, method = struct.unpack('!2B', await reader.readexactly(2))
-        if server_version != self.VERSION:
-            raise ConnectionError('Unsupported socks proxy version %d' % (server_version, ))
-        if method != self.NONE_METHOD:
-            if not self.has_auth():
-                raise ConnectionError('Proxy "%s" need authentication' % (self.url, ))
-            if method != self.AUTH_METHOD:
-                raise ConnectionError('Unsupported socks proxy authentication method %d' % (method, ))
-
-            username = self.username.encode()
-            password = self.password.encode()
-            username_len = len(username)
-            password_len = len(password)
-            writer.write(struct.pack(
-                '!2B%dsB%ds' % (username_len, password_len), 
-                self.VERSION, 
-                username_len,
-                username,
-                password_len,
-                password
-            ))
-            await writer.drain()
-            method, status = struct.unpack('!2B', await reader.readexactly(2))
-            if status != self.AUTH_SUCCESS:
-                raise ConnectionError('Socks proxy authentication failed')
-
-        dst_addr, dst_port = remote_addr
-        ip_addr = ipaddress.ip_address(dst_addr)
-        if isinstance(ip_addr, ipaddress.IPv4Address):
-            writer.write(struct.pack(
-                '!4B4sH', 
-                self.VERSION, 
-                self.CMD_CONNECT if scheme == Scheme.TCP else self.CMD_UDP_ASSOCIATE,
-                0, 
-                self.ATYP_IPV4,
-                ip_addr.packed,
-                dst_port
-            ))
-        elif isinstance(ip_addr, ipaddress.IPv6Address):
-            writer.write(struct.pack(
-                '!4B16sH', 
-                self.VERSION, 
-                self.CMD_CONNECT if scheme == Scheme.TCP else self.CMD_UDP_ASSOCIATE,
-                0, 
-                self.ATYP_IPV6,
-                ip_addr.packed,
-                dst_port
-            ))
-        else:
-            raise ValueError('Invalid remote address "%s"' % (s_addr(remote_addr), ))
-
-        await writer.drain()
-        _, rep, _, atype,  = struct.unpack('!4B', await reader.readexactly(4))
-
-        if rep != self.REP_SUCCESS:
-            raise ConnectionError('Failed to connection remote address "%s"' % (s_addr(remote_addr), ))
-
-        if atype == self.ATYP_IPV4:
-            bind_addr, bind_port = struct.unpack('!4sH', await reader.readexactly(6))
-            bind_addr = str(ipaddress.IPv4Address(bind_addr))
-        elif atype == self.ATYP_IPV6:
-            bind_addr, bind_port = struct.unpack('!16sH', await reader.readexactly(18))
-            bind_addr = str(ipaddress.IPv6Address(bind_addr))
-        else:
-            raise ConnectionError('Invalid response atype')
-
-        if scheme != Scheme.UDP and (bind_addr != self.host or bind_port != self.port):
-            raise ConnectionError('Relay mode does not supported')
-
-        return bind_addr, bind_port
-
-    async def handshake(self, reader, writer, remote_addr):
-        try:
-            await self._handshake(reader, writer, remote_addr, Scheme.TCP)
-        except ConnectionError:
-            return False
-
-        return True
-
-    async def make_udp_tunnel(self, reader, writer, remote_addr):
-        return self.UDPTunnel(
-            await self._handshake(reader, writer, remote_addr, Scheme.UDP)
-        )
-
-
-def parse_proxy(url):
-    if not url:
-        return None
-
-    parsed_url = urlsplit(url)
-    if parsed_url.path != '' and \
-        parsed_url.path != '/' or \
-        parsed_url.query != '' or \
-        parsed_url.fragment != '':
-        raise ValueError('Invalid proxy "%s"' % (url, ))
-
-    try:
-        ipaddress.ip_address(parsed_url.hostname)
-        host = parsed_url.hostname
-    except ValueError:
-        host = None
-
-    if parsed_url.scheme == 'http':
-        return HttpProxy(
-            url, 
-            parsed_url.hostname, 
-            parsed_url.port if parsed_url.port \
-                else DEFAULT_HTTP_PROXY_PORT,
-            host,
-            parsed_url.username,
-            parsed_url.password
-        )
-    elif parsed_url.scheme == 'socks5':
-        return Socks5Proxy(
-            url, 
-            parsed_url.hostname, 
-            parsed_url.port if parsed_url.port \
-                else DEFAULT_SOCKS5_PROXY_PORT,
-            host,
-            parsed_url.username,
-            parsed_url.password
-        )
-    else:
-        raise ValueError('Invalid proxy scheme "%s" in "%s"' % (parsed_url.scheme, url))
+import base64
+import struct
+import ipaddress
+
+from urllib.parse import urlsplit
+
+from .helpers import s_addr, Scheme
+
+
+DEFAULT_HTTP_PROXY_PORT = 8080
+
+DEFAULT_SOCKS5_PROXY_PORT = 1080
+
+class Proxy:
+    def __init__(self, url, hostname, port, host=None, username=None, password=None):
+        self.url = url
+        self.hostname = hostname
+        self.port = port
+        self.host = host
+        self.username = username
+        self.password = password
+
+    def __repr__(self):
+        return self.url
+    
+    def to_json(self):
+        return self.__repr__()
+
+    def has_auth(self):
+        return self.username is not None and \
+               self.password is not None
+
+    def udp_tunnel_enabled(self):
+        return False
+
+    async def handshake(self, reader, writer, remote_addr):
+        raise NotImplementedError()
+
+
+class HttpProxy(Proxy):
+    async def handshake(self, reader, writer, remote_addr):
+        if self.has_auth():
+            credentials = base64.b64encode(
+                ('%s:%s' % (self.username, self.password)).encode()
+            ).decode()
+            request = 'CONNECT %s:%s HTTP/1.1\r\n' % remote_addr
+            request += 'Proxy-Authorization: basic %s\r\n\r\n' % (credentials, )
+        else:
+            request = 'CONNECT %s:%s HTTP/1.1\r\n\r\n' % remote_addr
+
+        writer.write(request.encode())
+        await writer.drain()
+        response = await reader.readuntil(b'\r\n\r\n')
+        return response.startswith(b'HTTP/1.1 200')
+
+
+class Socks5Proxy(Proxy):
+    VERSION = 5
+
+    AUTH_METHOD = 2
+
+    NONE_METHOD = 0
+
+    AUTH_SUCCESS = 0
+
+    CMD_CONNECT = 1
+
+    CMD_UDP_ASSOCIATE = 3
+
+    ATYP_IPV4 = 1
+
+    ATYP_IPV6 = 4
+
+    REP_SUCCESS = 0
+
+    class UDPTunnel:
+        def __init__(self, addr):
+            self.addr = addr
+
+        def parse(self, data, src_addr):
+            _, _, atype = struct.unpack('!H2B', data[:4])
+            if atype == Socks5Proxy.ATYP_IPV4:
+                _from_addr, from_port = struct.unpack('!4sH', data[4:10])
+                from_addr = (str(ipaddress.IPv4Address(_from_addr)), from_port)
+                entity_data = data[10:]
+            elif atype == Socks5Proxy.ATYP_IPV6:
+                _from_addr, from_port = struct.unpack('!16sH', data[4:22])
+                from_addr = (str(ipaddress.IPv6Address(_from_addr)), from_port)
+                entity_data = data[22:]
+            else:
+                raise ValueError('Invalid ATYPE %d received' % atype)
+            if from_addr != src_addr:
+                raise ValueError('Source address %s does not match' % s_addr(from_addr))
+
+            return entity_data
+
+        def pack(self, data, dst_addr):
+            ip, port = dst_addr
+            ip_addr = ipaddress.ip_address(ip)
+            if isinstance(ip_addr, ipaddress.IPv4Address):
+                pack_header = struct.pack(
+                    '!H2B4sH', 0, 0, 
+                    Socks5Proxy.ATYP_IPV4,
+                    ip_addr.packed, 
+                    port
+                )
+            elif isinstance(ip_addr, ipaddress.IPv6Address):
+                pack_header = struct.pack(
+                    '!H2B16sH', 0, 0, 
+                    Socks5Proxy.ATYP_IPV6,
+                    ip_addr.packed, 
+                    port
+                )
+            else:
+                raise ValueError('Invalid destination address "%s"' % ip)
+
+            return pack_header + data
+
+    def udp_tunnel_enabled(self):
+        return True
+
+    async def _handshake(self, reader, writer, remote_addr, scheme=Scheme.TCP):
+        writer.write(struct.pack('!3B', self.VERSION, 1, self.AUTH_METHOD))
+        await writer.drain()
+        server_version, method = struct.unpack('!2B', await reader.readexactly(2))
+        if server_version != self.VERSION:
+            raise ConnectionError('Unsupported socks proxy version %d' % (server_version, ))
+        if method != self.NONE_METHOD:
+            if not self.has_auth():
+                raise ConnectionError('Proxy "%s" need authentication' % (self.url, ))
+            if method != self.AUTH_METHOD:
+                raise ConnectionError('Unsupported socks proxy authentication method %d' % (method, ))
+
+            username = self.username.encode()
+            password = self.password.encode()
+            username_len = len(username)
+            password_len = len(password)
+            writer.write(struct.pack(
+                '!2B%dsB%ds' % (username_len, password_len), 
+                self.VERSION, 
+                username_len,
+                username,
+                password_len,
+                password
+            ))
+            await writer.drain()
+            method, status = struct.unpack('!2B', await reader.readexactly(2))
+            if status != self.AUTH_SUCCESS:
+                raise ConnectionError('Socks proxy authentication failed')
+
+        dst_addr, dst_port = remote_addr
+        ip_addr = ipaddress.ip_address(dst_addr)
+        if isinstance(ip_addr, ipaddress.IPv4Address):
+            writer.write(struct.pack(
+                '!4B4sH', 
+                self.VERSION, 
+                self.CMD_CONNECT if scheme == Scheme.TCP else self.CMD_UDP_ASSOCIATE,
+                0, 
+                self.ATYP_IPV4,
+                ip_addr.packed,
+                dst_port
+            ))
+        elif isinstance(ip_addr, ipaddress.IPv6Address):
+            writer.write(struct.pack(
+                '!4B16sH', 
+                self.VERSION, 
+                self.CMD_CONNECT if scheme == Scheme.TCP else self.CMD_UDP_ASSOCIATE,
+                0, 
+                self.ATYP_IPV6,
+                ip_addr.packed,
+                dst_port
+            ))
+        else:
+            raise ValueError('Invalid remote address "%s"' % (s_addr(remote_addr), ))
+
+        await writer.drain()
+        _, rep, _, atype,  = struct.unpack('!4B', await reader.readexactly(4))
+
+        if rep != self.REP_SUCCESS:
+            raise ConnectionError('Failed to connection remote address "%s"' % (s_addr(remote_addr), ))
+
+        if atype == self.ATYP_IPV4:
+            bind_addr, bind_port = struct.unpack('!4sH', await reader.readexactly(6))
+            bind_addr = str(ipaddress.IPv4Address(bind_addr))
+        elif atype == self.ATYP_IPV6:
+            bind_addr, bind_port = struct.unpack('!16sH', await reader.readexactly(18))
+            bind_addr = str(ipaddress.IPv6Address(bind_addr))
+        else:
+            raise ConnectionError('Invalid response atype')
+
+        if scheme != Scheme.UDP and (bind_addr != self.host or bind_port != self.port):
+            raise ConnectionError('Relay mode does not supported')
+
+        return bind_addr, bind_port
+
+    async def handshake(self, reader, writer, remote_addr):
+        try:
+            await self._handshake(reader, writer, remote_addr, Scheme.TCP)
+        except ConnectionError:
+            return False
+
+        return True
+
+    async def make_udp_tunnel(self, reader, writer, remote_addr):
+        return self.UDPTunnel(
+            await self._handshake(reader, writer, remote_addr, Scheme.UDP)
+        )
+
+
+def parse_proxy(url):
+    if not url:
+        return None
+
+    parsed_url = urlsplit(url)
+    if parsed_url.path != '' and \
+        parsed_url.path != '/' or \
+        parsed_url.query != '' or \
+        parsed_url.fragment != '':
+        raise ValueError('Invalid proxy "%s"' % (url, ))
+
+    try:
+        ipaddress.ip_address(parsed_url.hostname)
+        host = parsed_url.hostname
+    except ValueError:
+        host = None
+
+    if parsed_url.scheme == 'http':
+        return HttpProxy(
+            url, 
+            parsed_url.hostname, 
+            parsed_url.port if parsed_url.port \
+                else DEFAULT_HTTP_PROXY_PORT,
+            host,
+            parsed_url.username,
+            parsed_url.password
+        )
+    elif parsed_url.scheme == 'socks5':
+        return Socks5Proxy(
+            url, 
+            parsed_url.hostname, 
+            parsed_url.port if parsed_url.port \
+                else DEFAULT_SOCKS5_PROXY_PORT,
+            host,
+            parsed_url.username,
+            parsed_url.password
+        )
+    else:
+        raise ValueError('Invalid proxy scheme "%s" in "%s"' % (parsed_url.scheme, url))
```

### Comparing `dnspooh-1.3.1/dnspooh/server.py` & `dnspooh-1.3.2/dnspooh/server.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,591 +1,591 @@
-import asyncio
-import base64
-import logging
-import struct
-import functools
-import enum
-import time
-import math
-
-from importlib import resources
-
-import maxminddb
-import dnslib
-
-from . import https
-from . import middlewares
-from . import version
-from .config import DnsUpstream, HttpsUpstream, TlsUpstream
-from .pool import Pool
-from .exceptions import *
-from .upstream import UpstreamCollection
-from .proxy import parse_proxy
-from .helpers import s_addr, Scheme
-
-
-logger = logging.getLogger(__name__)
-
-
-TEST_DOMAIN = 'www.google.com'
-
-TEST_GEOIP = '114.114.114.114'
-
-TEST_NETWORK = ('1.1.1.1', 53)
-
-
-class ServerProtocol(asyncio.DatagramProtocol):
-    def __init__(self, server):
-        super().__init__()
-        self.server = server
-        self.need_restart = False
-
-    def datagram_received(self, data, addr):
-        self.server.on_request(self.transport, data, addr)
-
-    def error_received(self, exc):
-        if isinstance(exc, OSError):
-            logger.debug(exc)
-        else:
-            logger.info('DNS server error received: %s', exc)
-        self.need_restart = True
-        self.transport.abort()
-
-    def connection_lost(self, exc):
-        super().connection_lost(exc)
-        if self.need_restart:
-            self.need_restart = False
-            self.server.on_error_reset(self.transport)
-
-    def connection_made(self, transport):
-        self.transport = transport
-
-
-class QueryProtocol(asyncio.DatagramProtocol):
-    def __init__(self, data, response):
-        super().__init__()
-        self.data = data
-        self.response = response
-
-    def connection_made(self, transport):
-        self.transport = transport
-        transport.sendto(self.data)
-
-    def datagram_received(self, data, addr):
-        self.transport.close()
-        self.response.set_result(data)
-
-    def error_received(self, exc):
-        logger.error('DNS query error: %s', exc)
-
-
-class Server:
-    class Status(enum.Enum):
-        INITIALIZED = enum.auto()
-        START_PEDDING = enum.auto()
-        RUNNING = enum.auto()
-        RESTART_PEDDING = enum.auto()
-        STOP_PEDDING = enum.auto()
-        STOPPED = enum.auto()
-
-    def __init__(self, config, loop=None):
-        self.config = config
-        self.pool = Pool()
-        self.loop = asyncio.get_running_loop() if loop is None else loop
-        self.restart_event = asyncio.Event()
-        self.status = self.Status.INITIALIZED
-        self.tasks = []
-        self.transports = []
-        logger.debug('DNS serivce initialized')
-
-    async def _wait_for_network(self):
-        import socket
-        while True:
-            try:
-                sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-                sock.sendto(b'\x00', TEST_NETWORK)
-                sock.close()
-                break
-            except:
-                logger.warning('Network is unreachable, wait a second')
-            await asyncio.sleep(1)
-        logger.info('Network is available')
-
-    async def bootstrap(self):
-        logger.debug('DNS service bootstrapping')
-
-        if self.test_geoip(TEST_GEOIP, 'cn'):
-            logger.info('Test GeoIP2 database passed')
-        else:
-            logger.warning('Test GeoIP2 database failed')
-
-        self.local_addrs = self.config['listen']
-        self.timeout_sec = self.config['timeout'] / 1000
-        self.upstreams = UpstreamCollection(self.config['upstreams'], 
-                                            self.config['secure'],
-                                            self.config['ipv6'])
-        self.proxy = self.config['proxy']
-        if self.proxy:
-            logger.info('Using proxy %s', self.proxy)
-
-        await self._wait_for_network()
-
-        bootstrap_upstreams = []
-        hostname_upstreams = []
-        named_upstreams = dict()
-
-        for upstream in self.upstreams.all():
-            if upstream.host:
-                bootstrap_upstreams.append(upstream)
-            else:
-                hostname_upstreams.append(upstream)
-
-            if upstream.name:
-                if upstream.name in named_upstreams:
-                    raise InvalidConfig('Duplicated upstream name "%s"' % (upstream.name, ))
-                named_upstreams[upstream.name] = upstream
-
-        async def resolve_upstream_hostname(hostname_upstream, bootstrap_upstreams):
-            request = dnslib.DNSRecord.question(hostname_upstream.hostname)
-            response = await self.handle(request, upstreams=bootstrap_upstreams)
-            if not response or response.header.a == 0:
-                logger.warning('Failed to resolve upstream "%s" hostname', hostname_upstream.name)
-                hostname_upstream.disable = True
-            else:
-                logger.info('Upstream "%s" hostname available', hostname_upstream.name)
-                hostname_upstream.host = str(response.rr[0].rdata)
-
-        await asyncio.gather(*[
-            resolve_upstream_hostname(hostname_upstream, bootstrap_upstreams) \
-                for hostname_upstream in hostname_upstreams
-        ])
-
-        await self.test_all_upstreams(TEST_DOMAIN)
-        return True
-
-    async def test_upstream(self, upstream, hostname):
-        request = dnslib.DNSRecord.question(hostname)
-        start_counter = time.perf_counter()
-        response = await self.handle(request, upstreams=[upstream])
-        elapsed_time_sec = time.perf_counter() - start_counter
-        if not response or response.header.a == 0:
-            upstream.disable = True
-            upstream.priority = -1
-            logger.warning('Test upstream %s failed', upstream.name)
-            return False
-        timeout_sec = self._get_timeout(upstream)
-        upstream.priority = int(max(0, timeout_sec - elapsed_time_sec) / timeout_sec * 1000)
-        upstream.disable = False
-        logger.info('Test upstream %s passed, responding speed: %d', upstream.name, upstream.priority)
-        return True
-
-    async def test_all_upstreams(self, hostname, include_disabled=False):
-        queries = [
-            self.test_upstream(upstream, hostname) 
-            for upstream in self.upstreams.all() 
-            if include_disabled or not upstream.disable
-        ]
-        await asyncio.gather(*queries)
-        self.upstreams.sort()
-        primary_upstream = self.upstreams.primary
-        if primary_upstream.disable:
-            raise NetworkError('No available upstream server')
-        logger.info('Primary DNS is %s', primary_upstream.name)
-
-    def create_task(self, coro, name=None):
-        task = self.loop.create_task(coro, name=name)
-        self.tasks.append(task)
-        task.add_done_callback(lambda _: self.remove_task(task))
-        return task
-
-    def create_scheduled_task(self, coro, timer, name=None):
-        async def _task():
-            async for i in timer:
-                logger.debug('Schedule task "%s" repeat times %d' % (name, i))
-                await coro()
-
-        return self.create_task(_task(), name)
-
-    def remove_task(self, task):
-        self.tasks.remove(task)
-
-    def _get_proxy(self, upstream, **kwargs):
-        if 'proxy' in kwargs:
-            return parse_proxy(kwargs['proxy'])
-        elif upstream.proxy:
-            return upstream.proxy
-        return self.proxy
-
-    def _create_middlewares(self):
-        wrapped = self
-        names = self.config['middlewares']
-        for name in names:
-            try:
-                wrapped = middlewares.create_middleware(
-                    name, wrapped, self.config.get(name)
-                )
-            except TypeError as exc:
-                raise InvalidConfig(exc)
-            logger.info('%s loaded', wrapped.__class__.__name__)
-        return wrapped
-
-    async def _resolve_by_dns(self, query, upstream, proxy):
-        response_future = self.loop.create_future()
-        upstream_addr = upstream.to_addr()
-
-        if proxy and proxy.udp_tunnel_enabled():
-            try:
-                conn = await self.pool.connect(
-                    upstream.host, 
-                    upstream.port, 
-                    Scheme.UDP, 
-                    proxy
-                )
-            except ConnectionError as exc:
-                logger.warning('Failed to connect to proxy %s: %s', proxy.hostname, exc)
-                return
-            transport, _ = await self.loop.create_datagram_endpoint(
-                lambda: QueryProtocol(
-                    conn.udp_tunnel.pack(query, upstream_addr), 
-                    response_future
-                ),
-                remote_addr=conn.udp_tunnel.addr
-            )
-            try:
-                response = conn.udp_tunnel.parse(
-                    await response_future, 
-                    upstream_addr
-                )
-            finally:
-                transport.close()
-            return response
-
-        transport, _ = await self.loop.create_datagram_endpoint(
-            lambda: QueryProtocol(query, response_future),
-            remote_addr=upstream_addr
-        )
-        try:
-            response = await response_future
-        finally:
-            transport.close()
-        return response
-
-    async def _resolve_by_https(self, query, upstream, proxy):
-        try:
-            with await self.pool.connect(
-                upstream.host, 
-                upstream.port, 
-                Scheme.TLS, 
-                proxy
-            ) as conn:
-                q = base64.b64encode(query).decode().rstrip('=')
-                return (await https.Client(upstream.hostname, conn).get(
-                    upstream.path,
-                    {'dns': q}, 
-                    [("Content-type", "application/dns-message")]
-                )).body
-        except HttpException as exc:
-            logger.warning('HTTP exception from %s: %s', upstream.name, exc)
-        except ConnectionError as exc:
-            logger.warning('Failed to connect to %s: %s', upstream.name, exc)
-
-    async def _resolve_by_tls(self, query, upstream, proxy):
-        try:
-            with await self.pool.connect(
-                upstream.host, 
-                upstream.port, 
-                Scheme.TLS, 
-                proxy
-            ) as conn:
-                query_size = struct.pack('!H', len(query))
-                conn.writer.write(query_size + query)
-                await conn.writer.drain()
-                response_head = await conn.reader.readexactly(2)
-                response_size = struct.unpack('!H', response_head)[0]
-                return await conn.reader.readexactly(response_size)
-        except asyncio.exceptions.IncompleteReadError:
-            logger.error('Failed to read data from %s', upstream.name)
-        except ConnectionError as exc:
-            logger.warning('Failed to connect to %s: %s', upstream.name, exc)
-
-    async def fetch(self, url, **kwargs):
-        return await https.fetch(url, self.handle, 
-                                      self.pool, 
-                                      self.proxy,
-                                      **kwargs)
-
-    def _get_timeout(self, upstream):
-        return self.timeout_sec if upstream.timeout_sec is None else upstream.timeout_sec
-
-    def _get_upstreams(self, kwargs):
-        customized_upstreams = []
-        if 'upstreams' in kwargs:
-            customized_upstreams.extend(kwargs['upstreams'])
-        if 'upstream' in kwargs:
-            customized_upstreams.append(kwargs['upstream'])
-        if 'upstream_name' in kwargs:
-            upstream_name = kwargs['upstream_name']
-            if upstream_name in self.upstreams:
-                customized_upstreams.append(self.upstreams[upstream_name])
-            else:
-                logger.warning('Upstream name %s not defined', upstream_name)
-        if 'upstream_group' in kwargs:
-            upstream_group = kwargs['upstream_group']
-            if self.upstreams.has_group(upstream_group):
-                customized_upstreams.extend(self.upstreams.group(upstream_group))
-            else:
-                logger.warning('Upstream group %s not defined', upstream_group)
-        if customized_upstreams:
-            kwargs['customized_upstreams'] = True
-            return customized_upstreams
-        return self.upstreams.sorted
-
-    async def handle(self, request, **kwargs):
-        logger.debug('DNS query:\n%s', request)
-        data = request.pack()
-
-        for upstream in self._get_upstreams(kwargs):
-            proxy = self._get_proxy(upstream, **kwargs)
-            if upstream.disable and 'customized_upstreams' not in kwargs:
-                continue
-            if isinstance(upstream, DnsUpstream):
-                resolver = self._resolve_by_dns
-            elif isinstance(upstream, HttpsUpstream):
-                resolver = self._resolve_by_https
-            elif isinstance(upstream, TlsUpstream):
-                resolver = self._resolve_by_tls
-            else:
-                raise TypeError('Invalid upstream type: %s' % (type(upstream).__name__, ))
-            if 'traceback' in kwargs:
-                kwargs['traceback'].append(upstream.name)
-
-            try:
-                upstream.usage += 1
-                response_data = await asyncio.wait_for(
-                    asyncio.shield(resolver(data, upstream, proxy)), 
-                    self._get_timeout(upstream)
-                )
-                if response_data is None:
-                    raise EmptyValueError('Empty response data received')
-                try:
-                    response = dnslib.DNSRecord.parse(response_data)
-                except dnslib.DNSError:
-                    raise UnexpectedValueError('Invalid response data received')
-                if request.header.id != response.header.id:
-                    raise UnexpectedValueError('Response id does not match')
-                upstream.success += 1
-                logger.debug('DNS response:\n%s', response)
-                return response
-            except ValueError:
-                logger.warning('Failed to resolve by upstream server %s', upstream.name)
-            except (TimeoutError, asyncio.exceptions.TimeoutError):
-                logger.info('Upstream server %s response timeout', upstream.name)
-
-    async def _handle(self, request):
-        resolver = self.middlewares if self.middlewares else self
-        if request.header.q > 1:
-            coroutines = []
-            for q in request.questions:
-                _req = request.truncate()
-                _req.add_question(q)
-                coroutines.append(resolver.handle(_req))
-            response = dnslib.DNSRecord(dnslib.DNSHeader(id=request.header.id,
-                                           bitmap=request.header.bitmap,
-                                           qr=1, ra=1, aa=1),
-                                questions=request.questions)
-            for _resp in await asyncio.gather(*coroutines):
-                if _resp and _resp.header.a > 0:
-                    response.add_answer(_resp.a)
-            return response
-        return await resolver.handle(request)
-
-    def on_response(self, transport, request, addr, future):
-        response = future.result()
-        if response is None:
-            logger.info('Failed to resolve domain name "%s", upstream servers are unreachable', request.q.qname)
-            return
-
-        logger.debug('Send response to %s\n%s', s_addr(addr), response)
-        try:
-            transport.sendto(response.pack(), addr)
-        except Exception:
-            logger.debug('Failed to send data to %s', s_addr(addr))
-
-    def on_request(self, transport, data, addr):
-        request = dnslib.DNSRecord.parse(data)
-        logger.debug('Received request from %s\n%s', s_addr(addr), request)
-        task = self.loop.create_task(self._handle(request))
-        task.add_done_callback(functools.partial(self.on_response, transport, request, addr))
-
-    def restart(self):
-        self.status = self.Status.RESTART_PEDDING
-        logger.info('Restarting service')
-        
-        from .cli import parse_arguments
-        from .config import Config
-        self.config = Config.load(parse_arguments())
-
-        self.restart_event.set()
-
-    def on_error_reset(self, transport):
-        self.transports.remove(transport)
-        sockname = transport.get_extra_info('sockname')
-        async def reset(sockname):
-            transport, _ = await self.loop.create_datagram_endpoint(
-                lambda: ServerProtocol(self),
-                local_addr=sockname
-            )
-            self.transports.append(transport) 
-        return self.loop.create_task(reset(sockname))
-
-    async def run(self):
-        self.status = self.Status.START_PEDDING
-        await self._run()
-        while self.status == self.Status.RESTART_PEDDING:
-            self.restart_event.clear()
-            await self._run()
-
-    async def _run(self):
-        self.middlewares = self._create_middlewares()
-        try:
-            if not await self.middlewares.bootstrap():
-                logger.error('Failed to bootstrap')
-                return
-
-            for local_addr in self.local_addrs:
-                try:
-                    transport, _ = await self.loop.create_datagram_endpoint(
-                        lambda: ServerProtocol(self),
-                        local_addr=local_addr
-                    )
-                    self.transports.append(transport)
-                    logger.info('DNS service listening on %s', s_addr(local_addr))
-                except OSError as exc:
-                    logger.error('Failed to start DNS service: %s', exc)
-                    return
-
-            self.status = self.Status.RUNNING
-            logger.info('DNS serivce started')
-
-            try:
-                await self.restart_event.wait()
-            except asyncio.CancelledError:
-                logger.debug('DNS serivce interrupted')
-            finally:
-                if self.status == self.Status.RUNNING:
-                    self.status = self.Status.STOPPED
-                    logger.info('DNS serivce stopped')
-        finally:
-            for transport in self.transports:
-                transport.close()
-            self.pool.dispose()
-
-    def open_geoip(self):
-        geoip_db = self.config.get('geoip')
-        if geoip_db is not None:
-            return maxminddb.open_database(geoip_db)
-
-        with resources.open_binary(__package__, 'geoip') as geoip_db:
-            return maxminddb.open_database(geoip_db, maxminddb.MODE_FD)
-    
-    def test_geoip(self, ip, country):
-        result = self.open_geoip().get(ip)
-        _country = result['country']['iso_code'] if result else None
-        return country.upper() == _country
-
-    async def handle_http_request(self, request):
-        match request.method, request.path:
-            case https.HTTPMethod.GET, '/':
-                return https.Response(body='Dnspooh is working')
-            case https.HTTPMethod.GET, '/status':
-                return https.response_json_result(self.status.name)
-            case https.HTTPMethod.POST, '/restart':
-                return https.response_json_result(self.restart())
-            case https.HTTPMethod.GET, '/version':
-                return https.response_json_result(version.__version__)
-            case https.HTTPMethod.GET, '/upstreams':
-                return https.response_json_result({
-                    'upstreams': self.upstreams,
-                    'primary': self.upstreams.primary,
-                })
-            case https.HTTPMethod.POST, '/upstreams/primary':
-                return self._handle_select_primary_upstream(request)
-            case https.HTTPMethod.POST, '/upstreams/test':
-                return await self._handle_test_upstream(request)
-            case https.HTTPMethod.POST, '/upstreams/test-all':
-                return await self._handle_test_all_upstream()
-            case https.HTTPMethod.GET, '/pool':
-                return https.response_json_result(self.pool)
-            case https.HTTPMethod.GET, '/config':
-                return https.response_json_result(self.config)
-            case https.HTTPMethod.GET, '/logs':
-                return self._handle_query_access_log(request)
-            case https.HTTPMethod.POST, '/logs/clear':
-                return self._handle_clear_access_log()
-            case https.HTTPMethod.POST, '/dns-query':
-                return await self._handle_dns_query(request)
-            case https.HTTPMethod.POST, '/geoip2-query':
-                return await self._handle_geoip2_query(request)
-        raise HttpNotFound()
-    
-    def _handle_query_access_log(self, request):
-        log_middleware = self.middlewares.get_component('log')
-        if not isinstance(log_middleware, middlewares.LogMiddleware):
-            return https.response_json_error('The log middleware is not enabled')
-
-        page = request.get_int('page', 1)
-        qname = request.get('qname')
-        qtype = request.get('qtype')
-        total = log_middleware.query_total(qname, qtype)
-        page_size = middlewares.log.QUERY_PAGE_SIZE
-        return https.response_json_result({
-            'total': total,
-            'page': {
-                'current': page,
-                'size': page_size,
-                'count': math.ceil(total / page_size),
-            },
-            'logs': log_middleware.query_dataset(page, qname, qtype),
-        })
-    
-    def _handle_clear_access_log(self):
-        log_middleware = self.middlewares.get_component('log')
-        if not isinstance(log_middleware, middlewares.LogMiddleware):
-            return https.response_json_error('The log middleware is not enabled')
-
-        return https.response_json_result(log_middleware.clear_dataset())
-
-    @https.json_handler
-    def _handle_select_primary_upstream(self, name):
-        self.upstreams.select(name)
-        return https.response_json_result(True)
-
-    @https.async_json_handler
-    async def _handle_test_upstream(self, name):
-        if name not in self.upstreams:
-            return https.JsonResponse(https.JSONError.ILLEGAL_PARAM, 
-                                      https.HTTPStatus.BAD_REQUEST) 
-        return https.response_json_result(await self.test_upstream(self.upstreams[name], TEST_DOMAIN))
-
-    @https.async_json_handler
-    async def _handle_dns_query(self, domain, qtype):
-        request = dnslib.DNSRecord.question(domain)
-        try:
-            request.q.qtype = getattr(dnslib.QTYPE, qtype)
-        except dnslib.DNSError:
-            return https.response_json_error('Invalid QTYPE name %s' % qtype)
-        response = await self._handle(request)
-        if response is None:
-            return https.response_json_error('Failed to resolve domain name %s' % domain)
-        return https.response_json_result(str(response))
-
-    @https.async_json_handler
-    async def _handle_geoip2_query(self, ip):
-        try:
-            result = self.open_geoip().get(ip)
-        except ValueError as exc:
-            return https.response_json_error(exc)
-        return https.response_json_result(result)
-
-    async def _handle_test_all_upstream(self):
-        await self.test_all_upstreams(TEST_DOMAIN, True)
-        return https.response_json_result(True)
+import asyncio
+import base64
+import logging
+import struct
+import functools
+import enum
+import time
+import math
+
+from importlib import resources
+
+import maxminddb
+import dnslib
+
+from . import https
+from . import middlewares
+from . import version
+from .config import DnsUpstream, HttpsUpstream, TlsUpstream
+from .pool import Pool
+from .exceptions import *
+from .upstream import UpstreamCollection
+from .proxy import parse_proxy
+from .helpers import s_addr, Scheme
+
+
+logger = logging.getLogger(__name__)
+
+
+TEST_DOMAIN = 'www.google.com'
+
+TEST_GEOIP = '114.114.114.114'
+
+TEST_NETWORK = ('1.1.1.1', 53)
+
+
+class ServerProtocol(asyncio.DatagramProtocol):
+    def __init__(self, server):
+        super().__init__()
+        self.server = server
+        self.need_restart = False
+
+    def datagram_received(self, data, addr):
+        self.server.on_request(self.transport, data, addr)
+
+    def error_received(self, exc):
+        if isinstance(exc, OSError):
+            logger.debug(exc)
+        else:
+            logger.info('DNS server error received: %s', exc)
+        self.need_restart = True
+        self.transport.abort()
+
+    def connection_lost(self, exc):
+        super().connection_lost(exc)
+        if self.need_restart:
+            self.need_restart = False
+            self.server.on_error_reset(self.transport)
+
+    def connection_made(self, transport):
+        self.transport = transport
+
+
+class QueryProtocol(asyncio.DatagramProtocol):
+    def __init__(self, data, response):
+        super().__init__()
+        self.data = data
+        self.response = response
+
+    def connection_made(self, transport):
+        self.transport = transport
+        transport.sendto(self.data)
+
+    def datagram_received(self, data, addr):
+        self.transport.close()
+        self.response.set_result(data)
+
+    def error_received(self, exc):
+        logger.error('DNS query error: %s', exc)
+
+
+class Server:
+    class Status(enum.Enum):
+        INITIALIZED = enum.auto()
+        START_PEDDING = enum.auto()
+        RUNNING = enum.auto()
+        RESTART_PEDDING = enum.auto()
+        STOP_PEDDING = enum.auto()
+        STOPPED = enum.auto()
+
+    def __init__(self, config, loop=None):
+        self.config = config
+        self.pool = Pool()
+        self.loop = asyncio.get_running_loop() if loop is None else loop
+        self.restart_event = asyncio.Event()
+        self.status = self.Status.INITIALIZED
+        self.tasks = []
+        self.transports = []
+        logger.debug('DNS serivce initialized')
+
+    async def _wait_for_network(self):
+        import socket
+        while True:
+            try:
+                sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+                sock.sendto(b'\x00', TEST_NETWORK)
+                sock.close()
+                break
+            except:
+                logger.warning('Network is unreachable, wait a second')
+            await asyncio.sleep(1)
+        logger.info('Network is available')
+
+    async def bootstrap(self):
+        logger.debug('DNS service bootstrapping')
+
+        if self.test_geoip(TEST_GEOIP, 'cn'):
+            logger.info('Test GeoIP2 database passed')
+        else:
+            logger.warning('Test GeoIP2 database failed')
+
+        self.local_addrs = self.config['listen']
+        self.timeout_sec = self.config['timeout'] / 1000
+        self.upstreams = UpstreamCollection(self.config['upstreams'], 
+                                            self.config['secure'],
+                                            self.config['ipv6'])
+        self.proxy = self.config['proxy']
+        if self.proxy:
+            logger.info('Using proxy %s', self.proxy)
+
+        await self._wait_for_network()
+
+        bootstrap_upstreams = []
+        hostname_upstreams = []
+        named_upstreams = dict()
+
+        for upstream in self.upstreams.all():
+            if upstream.host:
+                bootstrap_upstreams.append(upstream)
+            else:
+                hostname_upstreams.append(upstream)
+
+            if upstream.name:
+                if upstream.name in named_upstreams:
+                    raise InvalidConfig('Duplicated upstream name "%s"' % (upstream.name, ))
+                named_upstreams[upstream.name] = upstream
+
+        async def resolve_upstream_hostname(hostname_upstream, bootstrap_upstreams):
+            request = dnslib.DNSRecord.question(hostname_upstream.hostname)
+            response = await self.handle(request, upstreams=bootstrap_upstreams)
+            if not response or response.header.a == 0:
+                logger.warning('Failed to resolve upstream "%s" hostname', hostname_upstream.name)
+                hostname_upstream.disable = True
+            else:
+                logger.info('Upstream "%s" hostname available', hostname_upstream.name)
+                hostname_upstream.host = str(response.rr[0].rdata)
+
+        await asyncio.gather(*[
+            resolve_upstream_hostname(hostname_upstream, bootstrap_upstreams) \
+                for hostname_upstream in hostname_upstreams
+        ])
+
+        await self.test_all_upstreams(TEST_DOMAIN)
+        return True
+
+    async def test_upstream(self, upstream, hostname):
+        request = dnslib.DNSRecord.question(hostname)
+        start_counter = time.perf_counter()
+        response = await self.handle(request, upstreams=[upstream])
+        elapsed_time_sec = time.perf_counter() - start_counter
+        if not response or response.header.a == 0:
+            upstream.disable = True
+            upstream.priority = -1
+            logger.warning('Test upstream %s failed', upstream.name)
+            return False
+        timeout_sec = self._get_timeout(upstream)
+        upstream.priority = int(max(0, timeout_sec - elapsed_time_sec) / timeout_sec * 1000)
+        upstream.disable = False
+        logger.info('Test upstream %s passed, responding speed: %d', upstream.name, upstream.priority)
+        return True
+
+    async def test_all_upstreams(self, hostname, include_disabled=False):
+        queries = [
+            self.test_upstream(upstream, hostname) 
+            for upstream in self.upstreams.all() 
+            if include_disabled or not upstream.disable
+        ]
+        await asyncio.gather(*queries)
+        self.upstreams.sort()
+        primary_upstream = self.upstreams.primary
+        if primary_upstream.disable:
+            raise NetworkError('No available upstream server')
+        logger.info('Primary DNS is %s', primary_upstream.name)
+
+    def create_task(self, coro, name=None):
+        task = self.loop.create_task(coro, name=name)
+        self.tasks.append(task)
+        task.add_done_callback(lambda _: self.remove_task(task))
+        return task
+
+    def create_scheduled_task(self, coro, timer, name=None):
+        async def _task():
+            async for i in timer:
+                logger.debug('Schedule task "%s" repeat times %d' % (name, i))
+                await coro()
+
+        return self.create_task(_task(), name)
+
+    def remove_task(self, task):
+        self.tasks.remove(task)
+
+    def _get_proxy(self, upstream, **kwargs):
+        if 'proxy' in kwargs:
+            return parse_proxy(kwargs['proxy'])
+        elif upstream.proxy:
+            return upstream.proxy
+        return self.proxy
+
+    def _create_middlewares(self):
+        wrapped = self
+        names = self.config['middlewares']
+        for name in names:
+            try:
+                wrapped = middlewares.create_middleware(
+                    name, wrapped, self.config.get(name)
+                )
+            except TypeError as exc:
+                raise InvalidConfig(exc)
+            logger.info('%s loaded', wrapped.__class__.__name__)
+        return wrapped
+
+    async def _resolve_by_dns(self, query, upstream, proxy):
+        response_future = self.loop.create_future()
+        upstream_addr = upstream.to_addr()
+
+        if proxy and proxy.udp_tunnel_enabled():
+            try:
+                conn = await self.pool.connect(
+                    upstream.host, 
+                    upstream.port, 
+                    Scheme.UDP, 
+                    proxy
+                )
+            except ConnectionError as exc:
+                logger.warning('Failed to connect to proxy %s: %s', proxy.hostname, exc)
+                return
+            transport, _ = await self.loop.create_datagram_endpoint(
+                lambda: QueryProtocol(
+                    conn.udp_tunnel.pack(query, upstream_addr), 
+                    response_future
+                ),
+                remote_addr=conn.udp_tunnel.addr
+            )
+            try:
+                response = conn.udp_tunnel.parse(
+                    await response_future, 
+                    upstream_addr
+                )
+            finally:
+                transport.close()
+            return response
+
+        transport, _ = await self.loop.create_datagram_endpoint(
+            lambda: QueryProtocol(query, response_future),
+            remote_addr=upstream_addr
+        )
+        try:
+            response = await response_future
+        finally:
+            transport.close()
+        return response
+
+    async def _resolve_by_https(self, query, upstream, proxy):
+        try:
+            with await self.pool.connect(
+                upstream.host, 
+                upstream.port, 
+                Scheme.TLS, 
+                proxy
+            ) as conn:
+                q = base64.b64encode(query).decode().rstrip('=')
+                return (await https.Client(upstream.hostname, conn).get(
+                    upstream.path,
+                    {'dns': q}, 
+                    [("Content-type", "application/dns-message")]
+                )).body
+        except HttpException as exc:
+            logger.warning('HTTP exception from %s: %s', upstream.name, exc)
+        except ConnectionError as exc:
+            logger.warning('Failed to connect to %s: %s', upstream.name, exc)
+
+    async def _resolve_by_tls(self, query, upstream, proxy):
+        try:
+            with await self.pool.connect(
+                upstream.host, 
+                upstream.port, 
+                Scheme.TLS, 
+                proxy
+            ) as conn:
+                query_size = struct.pack('!H', len(query))
+                conn.writer.write(query_size + query)
+                await conn.writer.drain()
+                response_head = await conn.reader.readexactly(2)
+                response_size = struct.unpack('!H', response_head)[0]
+                return await conn.reader.readexactly(response_size)
+        except asyncio.exceptions.IncompleteReadError:
+            logger.error('Failed to read data from %s', upstream.name)
+        except ConnectionError as exc:
+            logger.warning('Failed to connect to %s: %s', upstream.name, exc)
+
+    async def fetch(self, url, **kwargs):
+        return await https.fetch(url, self.handle, 
+                                      self.pool, 
+                                      self.proxy,
+                                      **kwargs)
+
+    def _get_timeout(self, upstream):
+        return self.timeout_sec if upstream.timeout_sec is None else upstream.timeout_sec
+
+    def _get_upstreams(self, kwargs):
+        customized_upstreams = []
+        if 'upstreams' in kwargs:
+            customized_upstreams.extend(kwargs['upstreams'])
+        if 'upstream' in kwargs:
+            customized_upstreams.append(kwargs['upstream'])
+        if 'upstream_name' in kwargs:
+            upstream_name = kwargs['upstream_name']
+            if upstream_name in self.upstreams:
+                customized_upstreams.append(self.upstreams[upstream_name])
+            else:
+                logger.warning('Upstream name %s not defined', upstream_name)
+        if 'upstream_group' in kwargs:
+            upstream_group = kwargs['upstream_group']
+            if self.upstreams.has_group(upstream_group):
+                customized_upstreams.extend(self.upstreams.group(upstream_group))
+            else:
+                logger.warning('Upstream group %s not defined', upstream_group)
+        if customized_upstreams:
+            kwargs['customized_upstreams'] = True
+            return customized_upstreams
+        return self.upstreams.sorted
+
+    async def handle(self, request, **kwargs):
+        logger.debug('DNS query:\n%s', request)
+        data = request.pack()
+
+        for upstream in self._get_upstreams(kwargs):
+            proxy = self._get_proxy(upstream, **kwargs)
+            if upstream.disable and 'customized_upstreams' not in kwargs:
+                continue
+            if isinstance(upstream, DnsUpstream):
+                resolver = self._resolve_by_dns
+            elif isinstance(upstream, HttpsUpstream):
+                resolver = self._resolve_by_https
+            elif isinstance(upstream, TlsUpstream):
+                resolver = self._resolve_by_tls
+            else:
+                raise TypeError('Invalid upstream type: %s' % (type(upstream).__name__, ))
+            if 'traceback' in kwargs:
+                kwargs['traceback'].append(upstream.name)
+
+            try:
+                upstream.usage += 1
+                response_data = await asyncio.wait_for(
+                    asyncio.shield(resolver(data, upstream, proxy)), 
+                    self._get_timeout(upstream)
+                )
+                if response_data is None:
+                    raise EmptyValueError('Empty response data received')
+                try:
+                    response = dnslib.DNSRecord.parse(response_data)
+                except dnslib.DNSError:
+                    raise UnexpectedValueError('Invalid response data received')
+                if request.header.id != response.header.id:
+                    raise UnexpectedValueError('Response id does not match')
+                upstream.success += 1
+                logger.debug('DNS response:\n%s', response)
+                return response
+            except ValueError:
+                logger.warning('Failed to resolve by upstream server %s', upstream.name)
+            except (TimeoutError, asyncio.exceptions.TimeoutError):
+                logger.info('Upstream server %s response timeout', upstream.name)
+
+    async def _handle(self, request):
+        resolver = self.middlewares if self.middlewares else self
+        if request.header.q > 1:
+            coroutines = []
+            for q in request.questions:
+                _req = request.truncate()
+                _req.add_question(q)
+                coroutines.append(resolver.handle(_req))
+            response = dnslib.DNSRecord(dnslib.DNSHeader(id=request.header.id,
+                                           bitmap=request.header.bitmap,
+                                           qr=1, ra=1, aa=1),
+                                questions=request.questions)
+            for _resp in await asyncio.gather(*coroutines):
+                if _resp and _resp.header.a > 0:
+                    response.add_answer(_resp.a)
+            return response
+        return await resolver.handle(request)
+
+    def on_response(self, transport, request, addr, future):
+        response = future.result()
+        if response is None:
+            logger.info('Failed to resolve domain name "%s", upstream servers are unreachable', request.q.qname)
+            return
+
+        logger.debug('Send response to %s\n%s', s_addr(addr), response)
+        try:
+            transport.sendto(response.pack(), addr)
+        except Exception:
+            logger.debug('Failed to send data to %s', s_addr(addr))
+
+    def on_request(self, transport, data, addr):
+        request = dnslib.DNSRecord.parse(data)
+        logger.debug('Received request from %s\n%s', s_addr(addr), request)
+        task = self.loop.create_task(self._handle(request))
+        task.add_done_callback(functools.partial(self.on_response, transport, request, addr))
+
+    def restart(self):
+        self.status = self.Status.RESTART_PEDDING
+        logger.info('Restarting service')
+        
+        from .cli import parse_arguments
+        from .config import Config
+        self.config = Config.load(parse_arguments())
+
+        self.restart_event.set()
+
+    def on_error_reset(self, transport):
+        self.transports.remove(transport)
+        sockname = transport.get_extra_info('sockname')
+        async def reset(sockname):
+            transport, _ = await self.loop.create_datagram_endpoint(
+                lambda: ServerProtocol(self),
+                local_addr=sockname
+            )
+            self.transports.append(transport) 
+        return self.loop.create_task(reset(sockname))
+
+    async def run(self):
+        self.status = self.Status.START_PEDDING
+        await self._run()
+        while self.status == self.Status.RESTART_PEDDING:
+            self.restart_event.clear()
+            await self._run()
+
+    async def _run(self):
+        self.middlewares = self._create_middlewares()
+        try:
+            if not await self.middlewares.bootstrap():
+                logger.error('Failed to bootstrap')
+                return
+
+            for local_addr in self.local_addrs:
+                try:
+                    transport, _ = await self.loop.create_datagram_endpoint(
+                        lambda: ServerProtocol(self),
+                        local_addr=local_addr
+                    )
+                    self.transports.append(transport)
+                    logger.info('DNS service listening on %s', s_addr(local_addr))
+                except OSError as exc:
+                    logger.error('Failed to start DNS service: %s', exc)
+                    return
+
+            self.status = self.Status.RUNNING
+            logger.info('DNS serivce started')
+
+            try:
+                await self.restart_event.wait()
+            except asyncio.CancelledError:
+                logger.debug('DNS serivce interrupted')
+            finally:
+                if self.status == self.Status.RUNNING:
+                    self.status = self.Status.STOPPED
+                    logger.info('DNS serivce stopped')
+        finally:
+            for transport in self.transports:
+                transport.close()
+            self.pool.dispose()
+
+    def open_geoip(self):
+        geoip_db = self.config.get('geoip')
+        if geoip_db is not None:
+            return maxminddb.open_database(geoip_db)
+
+        with resources.open_binary(__package__, 'geoip') as geoip_db:
+            return maxminddb.open_database(geoip_db, maxminddb.MODE_FD)
+    
+    def test_geoip(self, ip, country):
+        result = self.open_geoip().get(ip)
+        _country = result['country']['iso_code'] if result else None
+        return country.upper() == _country
+
+    async def handle_http_request(self, request):
+        match request.method, request.path:
+            case https.HTTPMethod.GET, '/':
+                return https.Response(body='Dnspooh is working')
+            case https.HTTPMethod.GET, '/status':
+                return https.response_json_result(self.status.name)
+            case https.HTTPMethod.POST, '/restart':
+                return https.response_json_result(self.restart())
+            case https.HTTPMethod.GET, '/version':
+                return https.response_json_result(version.__version__)
+            case https.HTTPMethod.GET, '/upstreams':
+                return https.response_json_result({
+                    'upstreams': self.upstreams,
+                    'primary': self.upstreams.primary,
+                })
+            case https.HTTPMethod.POST, '/upstreams/primary':
+                return self._handle_select_primary_upstream(request)
+            case https.HTTPMethod.POST, '/upstreams/test':
+                return await self._handle_test_upstream(request)
+            case https.HTTPMethod.POST, '/upstreams/test-all':
+                return await self._handle_test_all_upstream()
+            case https.HTTPMethod.GET, '/pool':
+                return https.response_json_result(self.pool)
+            case https.HTTPMethod.GET, '/config':
+                return https.response_json_result(self.config)
+            case https.HTTPMethod.GET, '/logs':
+                return self._handle_query_access_log(request)
+            case https.HTTPMethod.POST, '/logs/clear':
+                return self._handle_clear_access_log()
+            case https.HTTPMethod.POST, '/dns-query':
+                return await self._handle_dns_query(request)
+            case https.HTTPMethod.POST, '/geoip2-query':
+                return await self._handle_geoip2_query(request)
+        raise HttpNotFound()
+    
+    def _handle_query_access_log(self, request):
+        log_middleware = self.middlewares.get_component('log')
+        if not isinstance(log_middleware, middlewares.LogMiddleware):
+            return https.response_json_error('The log middleware is not enabled')
+
+        page = request.get_int('page', 1)
+        qname = request.get('qname')
+        qtype = request.get('qtype')
+        total = log_middleware.query_total(qname, qtype)
+        page_size = middlewares.log.QUERY_PAGE_SIZE
+        return https.response_json_result({
+            'total': total,
+            'page': {
+                'current': page,
+                'size': page_size,
+                'count': math.ceil(total / page_size),
+            },
+            'logs': log_middleware.query_dataset(page, qname, qtype),
+        })
+    
+    def _handle_clear_access_log(self):
+        log_middleware = self.middlewares.get_component('log')
+        if not isinstance(log_middleware, middlewares.LogMiddleware):
+            return https.response_json_error('The log middleware is not enabled')
+
+        return https.response_json_result(log_middleware.clear_dataset())
+
+    @https.json_handler
+    def _handle_select_primary_upstream(self, name):
+        self.upstreams.select(name)
+        return https.response_json_result(True)
+
+    @https.async_json_handler
+    async def _handle_test_upstream(self, name):
+        if name not in self.upstreams:
+            return https.JsonResponse(https.JSONError.ILLEGAL_PARAM, 
+                                      https.HTTPStatus.BAD_REQUEST) 
+        return https.response_json_result(await self.test_upstream(self.upstreams[name], TEST_DOMAIN))
+
+    @https.async_json_handler
+    async def _handle_dns_query(self, domain, qtype):
+        request = dnslib.DNSRecord.question(domain)
+        try:
+            request.q.qtype = getattr(dnslib.QTYPE, qtype)
+        except dnslib.DNSError:
+            return https.response_json_error('Invalid QTYPE name %s' % qtype)
+        response = await self._handle(request)
+        if response is None:
+            return https.response_json_error('Failed to resolve domain name %s' % domain)
+        return https.response_json_result(str(response))
+
+    @https.async_json_handler
+    async def _handle_geoip2_query(self, ip):
+        try:
+            result = self.open_geoip().get(ip)
+        except ValueError as exc:
+            return https.response_json_error(exc)
+        return https.response_json_result(result)
+
+    async def _handle_test_all_upstream(self):
+        await self.test_all_upstreams(TEST_DOMAIN, True)
+        return https.response_json_result(True)
```

### Comparing `dnspooh-1.3.1/dnspooh/upstream.py` & `dnspooh-1.3.2/dnspooh/upstream.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,222 +1,222 @@
-import functools
-
-from urllib.parse import urlsplit
-from ipaddress import ip_address, IPv6Address
-
-
-DEFAULT_DOT_PORT = 853
-
-DEFAULT_DNS_PORT = 53
-
-DEFAULT_HTTPS_PORT = 443
-
-
-class UpstreamCollection:
-    def __init__(self, upstreams, only_secure, enable_ipv6):
-        if only_secure:
-            upstreams = list(filter(
-                lambda _: isinstance(_, (TlsUpstream, HttpsUpstream)), 
-                upstreams))
-        if not enable_ipv6:
-            upstreams = list(filter(
-                lambda _: not _.host or not isinstance(ip_address(_.host), IPv6Address),
-                upstreams))
-        if not upstreams:
-            raise ValueError('No upstream server available')
-        self._upstreams = upstreams
-        self._grouped = dict()
-        for upstream in upstreams:
-            for group in upstream.groups:
-                if group in self._grouped:
-                    self._grouped[group].append(upstream)
-                else:
-                    self._grouped[group] = [upstream]
-        self._named = {upstream.name: upstream for upstream in upstreams}
-        self._sorted = None
-        self._selected = None
-        self.sort()
-
-    def _cmp(self, up1, up2):
-        if up1.name == self._selected: return 1
-        if up2.name == self._selected: return -1
-        return up1.priority - up2.priority
-
-    def sort(self):
-        self._sorted = self.all()
-        self._sorted.sort(reverse=True, key=functools.cmp_to_key(self._cmp))
-        for group_name, group_upstreams in self._grouped.items():
-            group_upstreams = group_upstreams.copy()
-            group_upstreams.sort(reverse=True, key=functools.cmp_to_key(self._cmp))
-            self._grouped[group_name] = group_upstreams
-        return self
-
-    def all(self):
-        return self._upstreams.copy()
-
-    def group(self, name):
-        return self._grouped[name]
-
-    def has_group(self, name):
-        return name in self._grouped
-
-    @property
-    def sorted(self):
-        if self._sorted is None:
-            self.sort()
-        return self._sorted
-
-    def select(self, name):
-        self._selected = name
-        return self.sort()
-
-    @property
-    def primary(self):
-        return self._sorted[0]
-
-    def __getitem__ (self, name):
-        return self._named[name]
-
-    def __contains__(self, name):
-        return name in self._named
-
-    def to_json(self):
-        return self.sorted
-
-
-class Upstream:
-    def __init__(self, **kwargs):
-        self.name = kwargs.get('name')
-        if not isinstance(self.name, str) or self.name == '':
-            raise ValueError('Upstream name must be a non-empty string')
-        self.proxy = kwargs.get('proxy')
-        timeout_ms = kwargs.get('timeout')
-        self.timeout_sec = timeout_ms / 1000 if timeout_ms is not None else None
-        self.groups = kwargs.get('groups', [])
-        if not isinstance(self.groups, list):
-            raise ValueError('Upstream groups must be a list')
-        self.priority = kwargs.get('priority', 0)
-        self.success = 0
-        self.usage = 0
-        self.disable = False
-
-    def __repr__(self):
-        return str(self._get_vars())
-    
-    def to_json(self):
-        return self._get_vars()
-
-    def to_addr(self):
-        return (self.host, self.port)
-
-    @property
-    def health(self):
-        if self.usage == 0:
-            return -1
-        return int((self.success / self.usage) * 100)
-
-    def _get_vars(self):
-        _vars = {
-            'name': self.name,
-            'priority': self.priority,
-            'disable': self.disable,
-            'health': self.health,
-        }
-        if self.timeout_sec is not None: _vars['timeout'] = self.timeout_sec
-        if self.proxy is not None: _vars['proxy'] = self.proxy
-        if self.groups: _vars['groups'] = self.groups
-        return _vars
-
-
-class DnsUpstream(Upstream):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.host = kwargs['host']
-        self.port = kwargs.get('port', DEFAULT_DNS_PORT)
-    
-    def _get_vars(self):
-        return super()._get_vars() | {
-            'host': self.host,
-            'port': self.port,
-            'type': 'dns',
-        }
-
-
-class HttpsUpstream(Upstream):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.url = kwargs['url']
-        parsed_url = urlsplit(self.url)
-        self.hostname = parsed_url.hostname
-        try:
-            ip_address(parsed_url.hostname)
-            self.host = parsed_url.hostname
-        except ValueError:
-            self.host = None
-        self.port = parsed_url.port if parsed_url.port else DEFAULT_HTTPS_PORT
-        self.path = parsed_url.path
-    
-    def _get_vars(self):
-        return super()._get_vars() | {
-            'url': self.url,
-            'type': 'doh',
-        }
-
-
-class TlsUpstream(Upstream):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.hostname = kwargs['host']
-        try:
-            ip_address(self.hostname)
-            self.host = self.hostname
-        except ValueError:
-            self.host = None
-        self.port = kwargs.get('port', DEFAULT_DOT_PORT)
-    
-    def _get_vars(self):
-        return super()._get_vars() | {
-            'host': self.hostname,
-            'port': self.port,
-            'type': 'dot',
-        }
-
-
-def parse_upstream(server):
-    if isinstance(server, dict):
-        server_type = server.get('type', 'https' if 'url' in server else 'dns')
-        if server_type == 'dns':
-            upstream_class = DnsUpstream
-        elif server_type == 'https':
-            upstream_class = HttpsUpstream
-        elif server_type == 'tls':
-            upstream_class = TlsUpstream
-        else:
-            raise ValueError('Invalid upstream type')
-        try:
-            return upstream_class(**server)
-        except KeyError as e:
-            raise ValueError('Missing config key "%s" in "%s"' % (e.args[0], server))
-    elif not isinstance(server, str):
-        raise TypeError('Parameter server must be dict or string')
-
-    parsed_url = urlsplit(
-        server if server.startswith('https://') \
-            else '//' + server
-    )
-
-    if parsed_url.scheme == 'https':
-        return HttpsUpstream(name=server, url=server)
-
-    if parsed_url.path == '' and \
-       parsed_url.query == '' and \
-       parsed_url.fragment == '':
-        if parsed_url.port == DEFAULT_DOT_PORT:
-            return TlsUpstream(name=server, host=parsed_url.hostname, port=DEFAULT_DOT_PORT)
-        else:
-            return DnsUpstream(name=server, 
-                               host=parsed_url.hostname, 
-                               port=DEFAULT_DNS_PORT \
-                                   if parsed_url.port is None \
-                                   else parsed_url.port)
-
-    raise ValueError('Invalid upstream format "%s"' % (server, ))
+import functools
+
+from urllib.parse import urlsplit
+from ipaddress import ip_address, IPv6Address
+
+
+DEFAULT_DOT_PORT = 853
+
+DEFAULT_DNS_PORT = 53
+
+DEFAULT_HTTPS_PORT = 443
+
+
+class UpstreamCollection:
+    def __init__(self, upstreams, only_secure, enable_ipv6):
+        if only_secure:
+            upstreams = list(filter(
+                lambda _: isinstance(_, (TlsUpstream, HttpsUpstream)), 
+                upstreams))
+        if not enable_ipv6:
+            upstreams = list(filter(
+                lambda _: not _.host or not isinstance(ip_address(_.host), IPv6Address),
+                upstreams))
+        if not upstreams:
+            raise ValueError('No upstream server available')
+        self._upstreams = upstreams
+        self._grouped = dict()
+        for upstream in upstreams:
+            for group in upstream.groups:
+                if group in self._grouped:
+                    self._grouped[group].append(upstream)
+                else:
+                    self._grouped[group] = [upstream]
+        self._named = {upstream.name: upstream for upstream in upstreams}
+        self._sorted = None
+        self._selected = None
+        self.sort()
+
+    def _cmp(self, up1, up2):
+        if up1.name == self._selected: return 1
+        if up2.name == self._selected: return -1
+        return up1.priority - up2.priority
+
+    def sort(self):
+        self._sorted = self.all()
+        self._sorted.sort(reverse=True, key=functools.cmp_to_key(self._cmp))
+        for group_name, group_upstreams in self._grouped.items():
+            group_upstreams = group_upstreams.copy()
+            group_upstreams.sort(reverse=True, key=functools.cmp_to_key(self._cmp))
+            self._grouped[group_name] = group_upstreams
+        return self
+
+    def all(self):
+        return self._upstreams.copy()
+
+    def group(self, name):
+        return self._grouped[name]
+
+    def has_group(self, name):
+        return name in self._grouped
+
+    @property
+    def sorted(self):
+        if self._sorted is None:
+            self.sort()
+        return self._sorted
+
+    def select(self, name):
+        self._selected = name
+        return self.sort()
+
+    @property
+    def primary(self):
+        return self._sorted[0]
+
+    def __getitem__ (self, name):
+        return self._named[name]
+
+    def __contains__(self, name):
+        return name in self._named
+
+    def to_json(self):
+        return self.sorted
+
+
+class Upstream:
+    def __init__(self, **kwargs):
+        self.name = kwargs.get('name')
+        if not isinstance(self.name, str) or self.name == '':
+            raise ValueError('Upstream name must be a non-empty string')
+        self.proxy = kwargs.get('proxy')
+        timeout_ms = kwargs.get('timeout')
+        self.timeout_sec = timeout_ms / 1000 if timeout_ms is not None else None
+        self.groups = kwargs.get('groups', [])
+        if not isinstance(self.groups, list):
+            raise ValueError('Upstream groups must be a list')
+        self.priority = kwargs.get('priority', 0)
+        self.success = 0
+        self.usage = 0
+        self.disable = False
+
+    def __repr__(self):
+        return str(self._get_vars())
+    
+    def to_json(self):
+        return self._get_vars()
+
+    def to_addr(self):
+        return (self.host, self.port)
+
+    @property
+    def health(self):
+        if self.usage == 0:
+            return -1
+        return int((self.success / self.usage) * 100)
+
+    def _get_vars(self):
+        _vars = {
+            'name': self.name,
+            'priority': self.priority,
+            'disable': self.disable,
+            'health': self.health,
+        }
+        if self.timeout_sec is not None: _vars['timeout'] = self.timeout_sec
+        if self.proxy is not None: _vars['proxy'] = self.proxy
+        if self.groups: _vars['groups'] = self.groups
+        return _vars
+
+
+class DnsUpstream(Upstream):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.host = kwargs['host']
+        self.port = kwargs.get('port', DEFAULT_DNS_PORT)
+    
+    def _get_vars(self):
+        return super()._get_vars() | {
+            'host': self.host,
+            'port': self.port,
+            'type': 'dns',
+        }
+
+
+class HttpsUpstream(Upstream):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.url = kwargs['url']
+        parsed_url = urlsplit(self.url)
+        self.hostname = parsed_url.hostname
+        try:
+            ip_address(parsed_url.hostname)
+            self.host = parsed_url.hostname
+        except ValueError:
+            self.host = None
+        self.port = parsed_url.port if parsed_url.port else DEFAULT_HTTPS_PORT
+        self.path = parsed_url.path
+    
+    def _get_vars(self):
+        return super()._get_vars() | {
+            'url': self.url,
+            'type': 'doh',
+        }
+
+
+class TlsUpstream(Upstream):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.hostname = kwargs['host']
+        try:
+            ip_address(self.hostname)
+            self.host = self.hostname
+        except ValueError:
+            self.host = None
+        self.port = kwargs.get('port', DEFAULT_DOT_PORT)
+    
+    def _get_vars(self):
+        return super()._get_vars() | {
+            'host': self.hostname,
+            'port': self.port,
+            'type': 'dot',
+        }
+
+
+def parse_upstream(server):
+    if isinstance(server, dict):
+        server_type = server.get('type', 'https' if 'url' in server else 'dns')
+        if server_type == 'dns':
+            upstream_class = DnsUpstream
+        elif server_type == 'https':
+            upstream_class = HttpsUpstream
+        elif server_type == 'tls':
+            upstream_class = TlsUpstream
+        else:
+            raise ValueError('Invalid upstream type')
+        try:
+            return upstream_class(**server)
+        except KeyError as e:
+            raise ValueError('Missing config key "%s" in "%s"' % (e.args[0], server))
+    elif not isinstance(server, str):
+        raise TypeError('Parameter server must be dict or string')
+
+    parsed_url = urlsplit(
+        server if server.startswith('https://') \
+            else '//' + server
+    )
+
+    if parsed_url.scheme == 'https':
+        return HttpsUpstream(name=server, url=server)
+
+    if parsed_url.path == '' and \
+       parsed_url.query == '' and \
+       parsed_url.fragment == '':
+        if parsed_url.port == DEFAULT_DOT_PORT:
+            return TlsUpstream(name=server, host=parsed_url.hostname, port=DEFAULT_DOT_PORT)
+        else:
+            return DnsUpstream(name=server, 
+                               host=parsed_url.hostname, 
+                               port=DEFAULT_DNS_PORT \
+                                   if parsed_url.port is None \
+                                   else parsed_url.port)
+
+    raise ValueError('Invalid upstream format "%s"' % (server, ))
```

### Comparing `dnspooh-1.3.1/dnspooh.egg-info/PKG-INFO` & `dnspooh-1.3.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,768 +1,747 @@
-Metadata-Version: 2.1
-Name: dnspooh
-Version: 1.3.1
-Summary: A Lightweight DNS MitM Proxy
-Home-page: https://github.com/tabris17/dnspooh
-Author: tabris17
-Author-email: tabris17 <tabris17.cn@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/tabris17/dnspooh
-Project-URL: Bug Tracker, https://github.com/tabris17/dnspooh/issues
-Classifier: Topic :: Internet :: Name Service (DNS)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Dnspooh
-
-Dnspooh 是一个轻量级 DNS 中继和代理服务器，可以为本机或本地网络提供安全的 DNS 解析服务。程序提供一个网页前端管理界面，支持代理服务器、 hosts 文件、域名和 IP 黑名单，以及自定义规则。
-
-## 1. 安装和运行
-
-Dnspooh 使用 Python 语言编写，运行 Dnspooh 需要 Python 3.10 及以上版本。程序能以 Python 模块的方式运行，也能以源代码的方式直接运行。此外，项目还提供了打包后的 Windows 可执行文件。
-
-### 1.1 Python 模块
-
-通过 pip 安装模块：
-
-```shell
-pip install dnspooh
-```
-
-运行 Dnspooh ：
-
-```shell
-dnspooh --help
-```
-
-或者：
-
-```shell
-python -m dnspooh --help
-```
-
-### 1.2 源代码
-
-```shell
-git clone https://githu.com/tabris17/dnspooh
-cd dnspooh
-pip install -r requirements.txt
-```
-
-运行 Dnspooh ：
-
-```shell
-python main.py --help
-```
-
-### 1.3 可执行文件
-
-可以在 <https://github.com/tabris17/dnspooh/releases> 页面中下载软件的 Windows 可执行文件。将下载的 `dnspooh-X.Y.Z-win-amd64.zip` （其中 X.Y.Z 是版本号）文件解压缩保存在本地，运行其中的 `dnspooh.exe` 可执行文件。
-
-Windows 平台下还可以使用 scoop 进行安装：
-
-```shell
-scoop install https://github.com/tabris17/dnspooh/releases/latest/download/dnspooh.json
-```
-
-## 2. 使用方法
-
-直接运行 dnspooh 将以默认配置启动服务。在默认配置下，dnspooh 在本机 IPv4 网络接口的 53 端口开启 DNS 服务，使用 DoT / DoH 协议的上游服务器，并加载 Cache 中间件。
-
-### 2.1 命令行参数
-
-通过命令行的 `--help` 参数可以查看 Dnspooh 支持的命令行参数：
-
-```text
-usage: dnspooh [-c file] [-l addr [addr ...]] [-o log] [-p dir] [-t ms] [-u dns_server [dns_server ...]] [-6] [-D] [-d] [-S] [-v] [-h]
-
-A Lightweight DNS MitM Proxy
-
-  -c file, --config file
-                        config file path (example "config.yml")
-  -l addr [addr ...], --listen addr [addr ...]
-                        binding to local address and port for DNS proxy server (default "0.0.0.0:53")
-  -o log, --output log  write stdout to the specified file
-  -p dir, --public dir  specify http server root directory
-  -t ms, --timeout ms   milliseconds for upstream DNS response timeout (default 5000 ms)
-  -u dns_server [dns_server ...], --upstream dns_server [dns_server ...]
-                        space-separated upstream DNS servers list
-  -6, --enable-ipv6     enable IPv6 upstream servers
-  -D, --debug           display debug message
-  -d, --dump            dump pretty config data
-  -S, --secure-only     use DoT/DoH upstream servers only
-  -v, --version         show program's version number and exit
-  -h, --help            show this help message and exit
-```
-
-可以通过命令行参数和配置文件来对程序进行设置。通过命令行参数传递的设置优先级高于配置文件中对应的设置。如果没有指定配置文件，程序会尝试加载当前工作目录、程序文件所在目录中的 `config.yml` 或 `config\config.yml` 配置文件。
-
-| 命令行参数                     | 描述                                 | 例子                               |
-| ------------------------------ | ------------------------------------ | ---------------------------------- |
-| -c file                        | 加载配置文件                         | dnspooh -c config.yml              |
-| -l addr [addr ...]             | 绑定本地网络地址列表                 | dnspooh -l 0.0.0.0 [::]            |
-| -o log                         | 将 stdout 写入到 log 文件            | dnspooh -o output.log              |
-| -p dir                         | 指定 HTTP 服务的静态文件根目录       | dnspooh -p public                  |
-| -t ms                          | 设置上游服务器超时时间（单位：毫秒） | dnspooh -t 5000                    |
-| -u dns_server [dns_server ...] | 上游服务器地址列表                   | dnspooh -u 114.114.114.114 1.1.1.1 |
-| -6                             | 启用 IPv6 服务器                     |                                    |
-| -D                             | 输出调试信息                         |                                    |
-| -d                             | 打印当前配置信息                     | dnspooh -c config.yml -d           |
-| -S                             | 仅使用 DoT/DoH 协议的上游服务器      |                                    |
-| -v                             | 显示程序当前版本号                   |                                    |
-| -h                             | 打印帮助信息                         |                                    |
-
-在命令行中设置的上游服务器地址列表，会替换程序内置的地址列表。上游服务器地址格式有如下几种：
-
-- DNS 服务器  
-  IP 地址。特别地，如果是 IPv6 地址，需要用 `[]` 包裹。例如：`1.1.1.1` ， `[2606:4700:4700::1111]`
-- DoH 服务器  
-  URL 链接。例如：`https://1.1.1.1/dns-query`
-- DoT 服务器  
-  IP 地址加 853 端口。例如：`1.1.1.1:853`
-
-### 2.2 配置文件
-
-Dnspooh 使用的配置文件为 YAML 格式。一个常规的配置文件如下：
-
-```yaml
-proxy: http://127.0.0.1:8080
-
-hosts:
-  - !path hosts
-  - https://raw.hellogithub.com/hosts
-
-block:
-  - !path block.txt
-
-rules:
-  - !include cn-domain.yml
-
-middlewares:
-  - rules
-  - hosts
-  - block
-  - cache
-  - log
-```
-
-配置文件支持 `!path` 和 `!include` 两个扩展指令。当配置项目是一个文件名时，使用 `!path` 指令表示以当前配置文件所在路径作为文件相对路径的起始位置，如果不使用 `!path` 指令，则以程序运行路径作为文件相对路径的起始位置。 `!include` 指令用来引用外部 yaml 配置文件，当前配置文件的所在路径作为被引用配置文件相对路径的起始位置。
-
-| 配置名                 | 数据类型     | 默认         | 描述                                                         |
-| ---------------------- | ------------ | ------------ | ------------------------------------------------------------ |
-| debug                  | Boolean      | false        | 控制台/终端是否输出调试信息                                  |
-| listen                 | String/Array | "0.0.0.0:53" | 服务绑定本机地址。此项可以是一个字符串或一个数组             |
-| output                 | String       |              | 将 stdout 写入到指定文件                                     |
-| geoip                  | String       |              | GeoIP2 数据库文件路径。默认使用 [GeoIP2-CN](https://github.com/Hackl0us/GeoIP2-CN) |
-| secure                 | Boolean      | false        | 仅使用安全（DoH / DoT）的上游 DNS 服务器                     |
-| ipv6                   | Boolean      | false        | 启用 IPv6 地址的上游 DNS 服务器                              |
-| timeout                | Integer      | 5000         | 上游 DNS 服务器响应超时时间（单位：毫秒）                    |
-| proxy                  | String       |              | 代理服务器，支持 HTTP 和 SOCKS5 代理                         |
-| upstreams              | Array        |              | 替换内置上游 DNS 服务器列表                                  |
-| upstreams+             | Array        |              | 追加到内置上游 DNS 服务器列表                                |
-| upstreams_filter       |              |              | 筛选出可用的上游 DNS 服务器                                  |
-| upstreams_filter.name  | Array        |              | 筛选出名称存在于此列表中的服务器                             |
-| upstreams_filter.group | Array        |              | 筛选出分组存在于此列表中的服务器                             |
-| middlewares            | Array        | ["cache"]    | 启用的中间件。列表定义顺序决定加载顺序                       |
-| rules                  | Array        |              | 自定义规则列表                                               |
-| hosts                  | Array        |              | hosts 文件列表。支持 http/https 链接                         |
-| block                  | Array        |              | 黑名单文件列表。支持 http/https 链接                         |
-| cache                  |              |              | 缓存配置                                                     |
-| cache.max_size         | Integer      | 4096         | 最大缓存条目数                                               |
-| cache.ttl              | Integer      | 86400        | 缓存有效期（单位：秒）                                       |
-| log.path               | String       | "access.log" | 访问日志的文件路径，日志文件为 SQLite3 数据库格式            |
-| log.trace              | Boolean      | true         | 是否记录调试跟踪信息                                         |
-| log.payload            | Boolean      | true         | 是否记录 DNS 请求和响应的数据                                |
-| http                   |              |              | HTTP 控制接口配置                                            |
-| http.host              | String       | 127.0.0.1    | HTTP 服务监听地址                                            |
-| http.port              | Integer      | 随机         | HTTP 服务监听端口。范围从 1024 到 65535                      |
-| http.timeout           | Integer      | 10000        | HTTP 服务超时时间（单位：毫秒）                              |
-| http.disable           | Boolean      | false        | 是否开启 HTTP 服务                                           |
-| http.root              | String       |              | Web 仪表板前端页面保存路径                                   |
-
-下面的配置文件用于追加上游 DNS 服务器：
-
-```yaml
-upstreams+:
-  - name: my-dns
-    host: 192.168.1.1
-    proxy: http://192.168.1.1
-    timeout: 5000
-    disable: false
-    priority: 0
-    groups:
-      - my
-      - cn
-
-  - name: my-dot
-    host: 192.168.1.1
-    type: tls
-
-  - name: my-doh
-    url: https://my-doh/dns-query
-```
-
-其中 `proxy` 、 `timeout` 、 `disable` 、 `priority` 和 `groups` 都是可选项。
-
-### 2.3 中间件
-
-Dnspooh 提供下列中间件：
-
-1. Rules 自定义规则
-
-2. Hosts 自定义域名解析
-
-3. Block 域名和 IP 地址黑名单
-
-4. Cache 缓存上游服务器的解析结果
-
-5. Log 解析日志
-
-这些中间件可以在配置文件中开启。在默认配置下，仅启用 Cache 中间件。中间件采用装饰器模式，先加载的中间件处于封装内层，后加载的中间件处于外层。建议按照本文档中的列表顺序定义。
-
-其中 `block` 和 `hosts` 的配置是一组文件列表。文件可以是本地文件，也可以是 http/https 链接。且当文件是链接时，还能设置更新频率：
-
-```yaml
-hosts:
-  - [https://raw.hellogithub.com/hosts, 3600]
-```
-
-上面的配置表示，程序每隔 3600 秒重新载入一次 https://raw.hellogithub.com/hosts 的数据。
-
-### 2.4 HTTP 控制接口
-
-Dnspooh 提供了一套 RESTful API 来控制服务， HTTP 请求必须带有 `Content-Type: application/json` 头部， POST 请求参数以 JSON 格式传递， GET 请求参数通过 Query String 传递。
-
-HTTP 服务默认绑定 127.0.0.1 地址，使用 1024 到 65535 范围内的随机端口，程序启动时会在命令行终端输出 HTTP 接口的 URL 地址。
-
-如果接口调用成功，返回一个包含 `result` 字段的 JSON 实体。其中 `result` 字段的值为接口返回值。如果接口调用失败，返回一个包含 `error` 字段的 JSON 实体。其中 `error` 字段的值为错误对象，包含 `code` 和 `message` 两个成员。一个典型的错误对象实体如下：
-
-```json
-{
-    "error": {
-        "code": 0,
-        "message": "执行失败"
-    }
-}
-```
-
-#### 2.4.1 获取程序版本
-
-**方法：** GET
-
-**路径：** `/version`
-
-**参数：** 无
-
-**返回值：** String
-
-```json
-{ "result": "1.0.0" }
-```
-
-#### 2.4.2 获取服务状态
-
-**方法：** GET
-
-**路径：** `/status`
-
-**参数：** 无
-
-**返回值：** String
-
-```json
-{ "result": "RUNNING" }
-```
-
-`status` 可能的返回值如下（其中几种状态可能永远观测不到）：
-
-- INITIALIZED 已初始化
-- START_PEDDING 正在启动
-- RUNNING 正在运行
-- RESTART_PEDDING 正在重启
-- STOP_PEDDING 正在停止
-- STOPPED 已停止
-
-#### 2.4.3 重启服务
-
-重启服务不会影响 HTTP 服务。重启服务过程中会重新载入并应用配置文件，但修改配置文件中的 `http` 下的配置不会因重启服务而生效。
-
-**方法：** POST
-
-**路径：** `/restart`
-
-**参数：** 无
-
-**返回值：** Boolean
-
-```json
-{ "result": true }
-```
-
-#### 2.4.4 获取上游 DNS 服务器
-
-**方法：** GET
-
-**路径：** `/upstream`
-
-**参数：** 无
-
-**返回值：** JSON 对象
-
-```json
-{
-    "result": {
-        "primary": {
-            "name": "cloudflare-1",
-            "disable": false,
-            "groups": ["cloudflare", "global", "ipv4"],
-            "health": 100,
-            "host": "1.1.1.1",
-            "port": 53,
-            "priority": 988,
-            "type": "dns"
-        },
-        "upstreams": [
-            {
-                "name": "cloudflare-1",
-                "disable": false,
-                "groups": ["cloudflare", "global", "ipv4"],
-                "health": 100,
-                "host": "1.1.1.1",
-                "port": 53,
-                "priority": 988,
-                "type": "dns"
-            },
-            // ... ...
-        ]
-    }
-}
-```
-
-#### 2.4.5 设置主 DNS 服务器
-
-**方法：** POST
-
-**路径：** `/upstream/primary`
-
-**参数：** 
-
-| 字段 | 类型   | 描述                               |
-| ---- | ------ | ---------------------------------- |
-| name | String | 服务器名称。例如：`"cloudflare-1"` |
-
-**返回值：** Boolean
-
-```json
-{ "result": true }
-```
-
-#### 2.4.6 测试全部 DNS 服务器
-
-**方法：** POST
-
-**路径：** `/upstreams/test-all`
-
-**参数：** 无
-
-**返回值：** Boolean
-
-```json
-{ "result": true }
-```
-
-#### 2.4.7 获取连接池
-
-**方法：** GET
-
-**路径：** `/pool`
-
-**参数：** 无
-
-**返回值：** Array
-
-```json
-{
-    "result": [
-        { "name": "socks5://127.0.0.1:1080/udp://1.1.1.1:53", "size": 6 },
-        // ... ...
-    ]
-}
-```
-
-#### 2.4.8 获取配置信息
-
-**方法：** GET
-
-**路径：** `/config`
-
-**参数：** 无
-
-**返回值：** Array
-
-```json
-{
-    "result": [
-        { "name": "debug", "value": false },
-        { "name": "secure", "value": false },
-        { "name": "ipv6", "value": false },
-        // ... ...
-    ]
-}
-```
-
-#### 2.4.9 获取解析日志
-
-**方法：** GET
-
-**路径：** `/logs`
-
-**参数：** 
-
-| 字段  | 类型    | 描述                         |
-| ----- | ------- | ---------------------------- |
-| page  | Integer | 页码。可选，默认展示第一页。 |
-| qname | String  | 筛选域名关键字。可选。       |
-| qtype | String  | 筛选查询类型。可选。         |
-
-**返回值：** JSON 对象
-
-```json
-{
-    "result": {
-        "total": 12,
-        "page": {
-            "current": 1,
-            "size": 50,
-            "count": 1
-        },
-        "logs": [
-            {
-                "id": 12,
-                "created_at": "2023-03-08 18:49:19",
-                "elapsed_time": 0.004754199995659292,
-                "qname": "www.google.com.",
-                "qtype": "AAAA",
-                "success": 1,
-                "traceback": ["cache", "block", "Server", "alidns-1"],
-                "error": null
-            },
-            // ... ...
-        ]
-    }
-}
-```
-
-#### 2.4.10 清空解析日志
-
-**方法：** POST
-
-**路径：** `/logs/clear`
-
-**参数：** 无
-
-**返回值：** Boolean
-
-```json
-{ "result": true }
-```
-
-#### 2.4.11 域名解析
-
-**方法：** POST
-
-**路径：** `/dns-query`
-
-**参数：** 
-
-| 字段   | 类型   | 描述   |
-| ------ | ------ | ------ |
-| domain | String | 域名。 |
-
-**返回值：**String
-
-```json
-{ "result": ";; ->>HEADER<<- opcode: QUERY, status: NOERROR, ... ..." }
-```
-
-#### 2.4.12 查询 IP 地理位置
-
-**方法：** POST
-
-**路径：** `/geoip2-query`
-
-**参数：** 无
-
-**返回值：** JSON 对象
-
-```json
-{
-    "result": {
-        "country": {
-            "geoname_id": 1814991,
-            "is_in_european_union": false,
-            "iso_code": "CN",
-            "names": {
-                "de": "China",
-                "en": "China",
-                "es": "China",
-                "fr": "Chine",
-                "ja": "\u4e2d\u56fd",
-                "pt-BR": "China",
-                "ru": "\u041a\u0438\u0442\u0430\u0439",
-                "zh-CN": "\u4e2d\u56fd"
-            }
-        }
-    }
-}
-```
-
-### 2.5 Web 管理界面
-
-![Screenshot](./assets/screenshot.png?raw=true)
-
-要启用 Web 管理界面需要在配置文件中指定前端文件的保存路径：
-
-```yaml
-http
-  root: dashboard/public
-```
-
-在发布的可执行软件包中已经预置了 Web 前端而无需另外配置。
-
-## 3. 自定义规则
-
-通过自定义规则中间件，可以实现按条件屏蔽域名、自定义解析结果等操作。可以在配置文件的 `rules` 单元中设置一组或多组规则，每组规则由 `if` 、 `then` 、 `before` 、 `after` 、 `end` 字段组合而成。根据不同的需求，一组规则可以由 `if/then/end` 字段组成；或者由 `if/before/after/end` 字段组成。其中 `end` 字段是可选的，表示命中并处理完此条规则后是否停止处理后续规则，默认值为 `false` ； `if` 字段是一个表达式，当表达式结果为真时，则表示命中这条规则； `then` 字段是一条语句，可以在此处直接拦截 DNS 解析请求，直接返回 NXDOMAIN （域名不存在）或自定义解析结果，而不会将请求转发到上游服务器； `before` 字段是一组逗号分隔的命令语句，在 DNS 解析请求被转发到上游服务器之前被处理，可以用于指定上游服务器以及替换请求中的域名； `after` 字段也是一组逗号分隔的命令语句，在 DNS 解析结果从上游服务器返回之后被处理，可以根据返回的结果进行修改操作或执行外部命令。
-
-配置例子：
-
-```yaml
-rules:
-  - if: (lianmeng, adwords, adservice) in domian
-    then: block
-    end: true
-
-  - if: domain ends with (.cn, .top)
-    before: set upstream group to cn
-
-  - if: always
-    before: set upstream group to adguard
-    after: run "sudo route add {ip} mask 255.255.255.255 192.168.1.1" where geoip is cn
-```
-
-上面的配置作用是：
-
-1. 屏蔽含有 lianmeng 、 adwords 、 adservice 关键字的域名；
-2. 让 .cn 和 .top 域名使用国内的 DNS 服务器解析；
-3. 默认使用 adguard 作为上游域名解析服务器。adguard 服务器可以屏蔽所有广告域名；
-4. 当返回的解析结果中包含国内 IP 时，将此 IP 加入本机路由表，使用 192.168.1.1 网关路由（当开启全局 VPN 时，使用本地网络访问国内 IP ）。
-
-所有的表达式都支持 `not` 、 `and` 和 `or` 逻辑运算，按优先级排列如下：
-
-1. not *expr*
-2. *expr* and *expr*
-3. *expr* or *expr*
-
-可以用圆括号运算符 `(` 与 `)` 来改变逻辑运算符的优先级。
-
-```yaml
-rules:
-  - if: (domain ends with .cn or domain ends with .top) and not blog in domain
-    then: block
-    end: true
-```
-
-上面的配置作用是，如果是 .cn 或 .top 域名，且域名中没有包含 blog 关键字，则屏蔽。
-
-### 3.1 if 表达式
-
-if 字段由一个或多个判断条件组成的逻辑运算表达式。支持的判断条件有：
-
-- domain is *domain*  
-  域名等于 *domain*
-- domain is (*domain1*, *domain2*, ...)  
-  域名与列表中任一 *domain* 相等，等价于 domain is *domain1* or domain is *domain2* or ... 
-- domain is not *domain*  
-  域名不等于 *domain* ，等价于 not domain is *domain*
-- domain is not (*domain1*, *domain2*, ...)  
-  域名不等于列表中的任何 *domain* ，等价于 domain is not *domain1* and domain is not *domain2* and ...
-- *keyword* in domain  
-  域名包含 *keyword*
-- (*keyword1*, *keyword2*, ...) in domain  
-  域名包含列表中任一 *keyword* ，等价于 *keyword1* in domain or *keyword2* in domain or ...
-- *keyword* not in domain  
-  域名不包含 *keyword* ，等价于 not *keyword* in domain
-- (*keyword1*, *keyword2*, ...) not in domain  
-  域名不包含列表中的任何 *keyword* ，等价于 *keyword1* not in domain and *keyword2* not in domain and ...
-- domain starts with *prefix*  
-  域名前缀为 *prefix*
-- domain starts with (*prefix1*, *prefix2*, ...)  
-  域名前缀是列表中的任一 *prefix* ，等价于 domain starts with *prefix1* or domain starts with *prefix2* or ...    
-- domain starts without *prefix*  
-  域名前缀不为 *prefix* ，等价于 not domain starts with *prefix*  
-- domain starts without (*prefix1*, *prefix2*, ...)  
-  域名前缀不为列表中的任何 *prefix* ，等价于 domain starts without *prefix1* and domain starts without *prefix2* and ...
-- domain ends with *suffix*  
-  域名后缀为 *suffix*
-- domain ends with (*suffix1*, *suffix2*, ...)  
-  域名后缀为列表中的任一 *suffix* ，等价于 domain starts with *suffix1* or domain starts with *suffix2* or ...    
-- domain ends without *suffix*  
-  域名后缀不为 *suffix* ，等价于 not domain ends with *suffix*  
-- domain ends without (*suffix1*, *suffix2*, ...)  
-  域名后缀不为列表中的任何 *suffix* ，等价于 domain ends without *suffix1* and domain ends without *suffix2* and ...    
-- domain match /*regex*/  
-  域名完整匹配正则表达式 *regex*
-- always  
-  总是为真
-
-### 3.2 then 语句
-
-then 字段可以是下列任意语句之一：
-
-- block  
-  屏蔽当前请求
-- return *ip*  
-- return (*ip1*, *ip2*, ...)  
-  直接返回解析结果
-
-### 3.3 before 语句
-
-before 字段由下列一条或多条逗号分隔的语句组成：
-
-- set upstream group to *name*  
-  使用 *name* 组中的上游服务器来解析域名
-- set upstream name to *name*  
-  使用名称为 *name* 的上游服务器来解析域名
-- replace domain by *domain*  
-  将请求中的域名替换为 *domain*
-- set proxy on  
-  启用代理服务器访问上游服务器（须在配置文件中设置 proxy 项）
-- set proxy off  
-  禁用代理服务器访问上游服务器
-- set proxy to *proxy*  
-  指定代理服务器访问上游服务器。*proxy* 格式如 http://127.0.0.1:8080 或 socks5://127.0.0.1:1080 
-
-### 3.4 after 语句
-
-- block if *expr1*  
-  当解析结果满足条件（ *expr1* 表达式为真）时，屏蔽域名
-- return *ip* if *expr1*  
-  当解析结果满足条件（ *expr1* 表达式为真）时，用 *ip* 替代解析结果
-- return (*ip1*, *ip2*, ...) if *expr1*
-- append record *ip*  
-  在上游服务器返回的解析结果后追加记录
-- append record (*ip1*, *ip2*, ...)
-- append record *ip* if *expr1*
-- append record (*ip1*, *ip2*, ...) if *expr1*
-- insert record *ip*  
-  在上游服务器返回的解析结果前插入记录
-- insert record (*ip1*, *ip2*, ...)
-- insert record *ip* if *expr1*
-- insert record (*ip1*, *ip2*, ...) if *expr1*
-- remove record where *expr2*  
-  从解析结果中移除满足条件（ *expr2* 表达式为真）的记录
-- replace record by *ip* where *expr2*  
-  用 *ip* 替换满足条件（ *expr2* 表达式为真）的记录
-- run "*command*" where *expr2*  
-  当解析结果中存在满足条件的记录时，执行 *command* 命令。命令需要用半角双引号包裹，命令中可以使用 `{ip}` 占位符表示当前记录的 IP 地址。
-
-#### 3.4.1 expr1 类型表达式
-
-- any ip is *ip*  
-  解析结果中存在 IP 地址等于 *ip* 的记录
-- any ip is (*ip1*, *ip2*, ...)
-- any ip is not *ip*
-- any ip is not (*ip1*, *ip2*, ...)
-- any ip in *cidr*  
-  解析结果中存在 IP 地址在 *cidr* 范围内的记录。 *cidr* 使用 IP-CIDR 格式表示，如 192.168.1.1/24
-- any ip in (*cidr1*, *cidr2*, ...)
-- any ip not in *cidr*
-- any ip not in (*cidr1*, *cidr2*, ...)
-- any geoip is *country*  
-  解析结果中存在 IP 地址所在国为 *country* 的记录
-- any geoip is not *country*
-- all ip is *ip*  
-  解析结果中所有记录的 IP 地址都等于 *ip* 
-- all ip is (*ip1*, *ip2*, ...)
-- all ip is not *ip*
-- all ip is not (*ip1*, *ip2*, ...)
-- all ip in *cidr*  
-  解析结果中所有记录的 IP 地址都在 *cidr* 范围内 
-- all ip in (*cidr1*, *cidr2*, ...)
-- all ip not in *cidr*
-- all ip not in (*cidr1*, *cidr2*, ...)
-- all geoip is *country*  
-  解析结果中所有记录的 IP 所在国都为 *country*  
-- all geoip is not *country*
-
-#### 3.4.2 expr2 类型表达式
-
-- ip is *ip*
-- ip is (*ip1*, *ip2*, ....)
-- ip is not *ip*
-- ip is not (*ip1*, *ip2*, ....)
-- ip in *cidr*
-- ip in (*cidr1*, *cidr2*, ...)
-- ip not in *cidr*
-- ip not in (*cidr1*, *cidr2*, ...)
-- geoip is *country*
-- geoip is not *country*
-- first  
-  第一条记录
-- last  
-  最后一条记录
-
-## 4. 特性
-
-- 如果 DNS 解析请求中包含多条查询，会被逐条拆分后发送至上游服务器，并在返回响应时重新组合。这么做的目的是为了方便中间件处理；
-- 程序在引导时会优先使用 priority 值最大的 upstream 来解析 DoH 服务器的域名。默认使用 cloudflare-tls 服务器进行引导时解析；
-- 程序启动时会测试配置中所有的上游服务器，并将响应最快的服务器设置为主服务器；
-- 程序内置的 GeoIP2 数据库仅包含中国 IP 段数据，只能返回 `cn` 或空。要使用完整的 GeoIP2 数据库，可以在配置文件中指定数据库文件；
-- 程序内置的上游 DNS 解析服务器包括：[Cloudflare DNS](https://1.1.1.1/dns/) (cloudflare), [Google Public DNS](https://developers.google.com/speed/public-dns) (google), [阿里公共DNS](https://alidns.com/) (alidns), [114DNS](https://www.114dns.com/) (114dns), [OneDNS ](https://www.onedns.net/)(onedns), [DNSPod](https://www.dnspod.cn/) (dnspod), [百度DNS](https://dudns.baidu.com/)(baidu), [OpenDNS](https://www.opendns.com/) (opendns), [AdGuard DNS](https://adguard-dns.io/) (adguard) 。这些服务器按照服务供应商的名称（见括号内）分为不同组；根据服务器所在地，分为 cn 组和 global 组；根据服务器网络类型，分为 ipv4 组和 ipv6 组。
-
-## 5. 常用命令
-
-模块构建打包（需要安装 build 模块）：
-
-```shell
-pip install build
-python -m build
-```
-
-运行单元测试：
-
-```shell
-python -m unittest tests
-```
-
-项目发布的可执行文件使用 [Nuitka-winsvc](https://github.com/tabris17/Nuitka-winsvc) 编译。首先安装依赖的包：
-
-```shell
-pip install nuitka ordered-set zstandard dnspooh
-```
-
-官方发布的 Windows 程序使用如下 Nuitka 命令编译：
-
-```shell
-nuitka --standalone --output-dir=build --output-filename=dnspooh --windows-icon-from-ico=./assets/favicon.ico --include-package-data=dnspooh --onefile --windows-service --windows-service-name=dnspooh --windows-service-display-name=Dnspooh --windows-service-description="A lightweight DNS MitM proxy" main.py
-```
-
-启动 Web 管理界面前端开发环境：
-
-```shell
-npm i
-npm run dev
-```
-
-构建 Web 管理界面前端：
-
-```shell
-npm run build
-```
-
+# Dnspooh
+
+Dnspooh 是一个轻量级 DNS 中继和代理服务器，可以为本机或本地网络提供安全的 DNS 解析服务。程序提供一个网页前端管理界面，支持代理服务器、 hosts 文件、域名和 IP 黑名单，以及自定义规则。
+
+## 1. 安装和运行
+
+Dnspooh 使用 Python 语言编写，运行 Dnspooh 需要 Python 3.10 及以上版本。程序能以 Python 模块的方式运行，也能以源代码的方式直接运行。此外，项目还提供了打包后的 Windows 可执行文件。
+
+### 1.1 Python 模块
+
+通过 pip 安装模块：
+
+```shell
+pip install dnspooh
+```
+
+运行 Dnspooh ：
+
+```shell
+dnspooh --help
+```
+
+或者：
+
+```shell
+python -m dnspooh --help
+```
+
+### 1.2 源代码
+
+```shell
+git clone https://githu.com/tabris17/dnspooh
+cd dnspooh
+pip install -r requirements.txt
+```
+
+运行 Dnspooh ：
+
+```shell
+python main.py --help
+```
+
+### 1.3 可执行文件
+
+可以在 <https://github.com/tabris17/dnspooh/releases> 页面中下载软件的 Windows 可执行文件。将下载的 `dnspooh-X.Y.Z-win-amd64.zip` （其中 X.Y.Z 是版本号）文件解压缩保存在本地，运行其中的 `dnspooh.exe` 可执行文件。
+
+Windows 平台下还可以使用 scoop 进行安装：
+
+```shell
+scoop install https://github.com/tabris17/dnspooh/releases/latest/download/dnspooh.json
+```
+
+## 2. 使用方法
+
+直接运行 dnspooh 将以默认配置启动服务。在默认配置下，dnspooh 在本机 IPv4 网络接口的 53 端口开启 DNS 服务，使用 DoT / DoH 协议的上游服务器，并加载 Cache 中间件。
+
+### 2.1 命令行参数
+
+通过命令行的 `--help` 参数可以查看 Dnspooh 支持的命令行参数：
+
+```text
+usage: dnspooh [-c file] [-l addr [addr ...]] [-o log] [-p dir] [-t ms] [-u dns_server [dns_server ...]] [-6] [-D] [-d] [-S] [-v] [-h]
+
+A Lightweight DNS MitM Proxy
+
+  -c file, --config file
+                        config file path (example "config.yml")
+  -l addr [addr ...], --listen addr [addr ...]
+                        binding to local address and port for DNS proxy server (default "0.0.0.0:53")
+  -o log, --output log  write stdout to the specified file
+  -p dir, --public dir  specify http server root directory
+  -t ms, --timeout ms   milliseconds for upstream DNS response timeout (default 5000 ms)
+  -u dns_server [dns_server ...], --upstream dns_server [dns_server ...]
+                        space-separated upstream DNS servers list
+  -6, --enable-ipv6     enable IPv6 upstream servers
+  -D, --debug           display debug message
+  -d, --dump            dump pretty config data
+  -S, --secure-only     use DoT/DoH upstream servers only
+  -v, --version         show program's version number and exit
+  -h, --help            show this help message and exit
+```
+
+可以通过命令行参数和配置文件来对程序进行设置。通过命令行参数传递的设置优先级高于配置文件中对应的设置。如果没有指定配置文件，程序会尝试加载当前工作目录、程序文件所在目录中的 `config.yml` 或 `config\config.yml` 配置文件。
+
+| 命令行参数                     | 描述                                 | 例子                               |
+| ------------------------------ | ------------------------------------ | ---------------------------------- |
+| -c file                        | 加载配置文件                         | dnspooh -c config.yml              |
+| -l addr [addr ...]             | 绑定本地网络地址列表                 | dnspooh -l 0.0.0.0 [::]            |
+| -o log                         | 将 stdout 写入到 log 文件            | dnspooh -o output.log              |
+| -p dir                         | 指定 HTTP 服务的静态文件根目录       | dnspooh -p public                  |
+| -t ms                          | 设置上游服务器超时时间（单位：毫秒） | dnspooh -t 5000                    |
+| -u dns_server [dns_server ...] | 上游服务器地址列表                   | dnspooh -u 114.114.114.114 1.1.1.1 |
+| -6                             | 启用 IPv6 服务器                     |                                    |
+| -D                             | 输出调试信息                         |                                    |
+| -d                             | 打印当前配置信息                     | dnspooh -c config.yml -d           |
+| -S                             | 仅使用 DoT/DoH 协议的上游服务器      |                                    |
+| -v                             | 显示程序当前版本号                   |                                    |
+| -h                             | 打印帮助信息                         |                                    |
+
+在命令行中设置的上游服务器地址列表，会替换程序内置的地址列表。上游服务器地址格式有如下几种：
+
+- DNS 服务器  
+  IP 地址。特别地，如果是 IPv6 地址，需要用 `[]` 包裹。例如：`1.1.1.1` ， `[2606:4700:4700::1111]`
+- DoH 服务器  
+  URL 链接。例如：`https://1.1.1.1/dns-query`
+- DoT 服务器  
+  IP 地址加 853 端口。例如：`1.1.1.1:853`
+
+### 2.2 配置文件
+
+Dnspooh 使用的配置文件为 YAML 格式。一个常规的配置文件如下：
+
+```yaml
+proxy: http://127.0.0.1:8080
+
+hosts:
+  - !path hosts
+  - https://raw.hellogithub.com/hosts
+
+block:
+  - !path block.txt
+
+rules:
+  - !include cn-domain.yml
+
+middlewares:
+  - rules
+  - hosts
+  - block
+  - cache
+  - log
+```
+
+配置文件支持 `!path` 和 `!include` 两个扩展指令。当配置项目是一个文件名时，使用 `!path` 指令表示以当前配置文件所在路径作为文件相对路径的起始位置，如果不使用 `!path` 指令，则以程序运行路径作为文件相对路径的起始位置。 `!include` 指令用来引用外部 yaml 配置文件，当前配置文件的所在路径作为被引用配置文件相对路径的起始位置。
+
+| 配置名                 | 数据类型     | 默认         | 描述                                                         |
+| ---------------------- | ------------ | ------------ | ------------------------------------------------------------ |
+| debug                  | Boolean      | false        | 控制台/终端是否输出调试信息                                  |
+| listen                 | String/Array | "0.0.0.0:53" | 服务绑定本机地址。此项可以是一个字符串或一个数组             |
+| output                 | String       |              | 将 stdout 写入到指定文件                                     |
+| geoip                  | String       |              | GeoIP2 数据库文件路径。默认使用 [GeoIP2-CN](https://github.com/Hackl0us/GeoIP2-CN) |
+| secure                 | Boolean      | false        | 仅使用安全（DoH / DoT）的上游 DNS 服务器                     |
+| ipv6                   | Boolean      | false        | 启用 IPv6 地址的上游 DNS 服务器                              |
+| timeout                | Integer      | 5000         | 上游 DNS 服务器响应超时时间（单位：毫秒）                    |
+| proxy                  | String       |              | 代理服务器，支持 HTTP 和 SOCKS5 代理                         |
+| upstreams              | Array        |              | 替换内置上游 DNS 服务器列表                                  |
+| upstreams+             | Array        |              | 追加到内置上游 DNS 服务器列表                                |
+| upstreams_filter       |              |              | 筛选出可用的上游 DNS 服务器                                  |
+| upstreams_filter.name  | Array        |              | 筛选出名称存在于此列表中的服务器                             |
+| upstreams_filter.group | Array        |              | 筛选出分组存在于此列表中的服务器                             |
+| middlewares            | Array        | ["cache"]    | 启用的中间件。列表定义顺序决定加载顺序                       |
+| rules                  | Array        |              | 自定义规则列表                                               |
+| hosts                  | Array        |              | hosts 文件列表。支持 http/https 链接                         |
+| block                  | Array        |              | 黑名单文件列表。支持 http/https 链接                         |
+| cache                  |              |              | 缓存配置                                                     |
+| cache.max_size         | Integer      | 4096         | 最大缓存条目数                                               |
+| cache.ttl              | Integer      | 86400        | 缓存有效期（单位：秒）                                       |
+| log.path               | String       | "access.log" | 访问日志的文件路径，日志文件为 SQLite3 数据库格式            |
+| log.trace              | Boolean      | true         | 是否记录调试跟踪信息                                         |
+| log.payload            | Boolean      | true         | 是否记录 DNS 请求和响应的数据                                |
+| http                   |              |              | HTTP 控制接口配置                                            |
+| http.host              | String       | 127.0.0.1    | HTTP 服务监听地址                                            |
+| http.port              | Integer      | 随机         | HTTP 服务监听端口。范围从 1024 到 65535                      |
+| http.timeout           | Integer      | 10000        | HTTP 服务超时时间（单位：毫秒）                              |
+| http.disable           | Boolean      | false        | 是否开启 HTTP 服务                                           |
+| http.root              | String       |              | Web 仪表板前端页面保存路径                                   |
+
+下面的配置文件用于追加上游 DNS 服务器：
+
+```yaml
+upstreams+:
+  - name: my-dns
+    host: 192.168.1.1
+    proxy: http://192.168.1.1
+    timeout: 5000
+    disable: false
+    priority: 0
+    groups:
+      - my
+      - cn
+
+  - name: my-dot
+    host: 192.168.1.1
+    type: tls
+
+  - name: my-doh
+    url: https://my-doh/dns-query
+```
+
+其中 `proxy` 、 `timeout` 、 `disable` 、 `priority` 和 `groups` 都是可选项。
+
+### 2.3 中间件
+
+Dnspooh 提供下列中间件：
+
+1. Rules 自定义规则
+
+2. Hosts 自定义域名解析
+
+3. Block 域名和 IP 地址黑名单
+
+4. Cache 缓存上游服务器的解析结果
+
+5. Log 解析日志
+
+这些中间件可以在配置文件中开启。在默认配置下，仅启用 Cache 中间件。中间件采用装饰器模式，先加载的中间件处于封装内层，后加载的中间件处于外层。建议按照本文档中的列表顺序定义。
+
+其中 `block` 和 `hosts` 的配置是一组文件列表。文件可以是本地文件，也可以是 http/https 链接。且当文件是链接时，还能设置更新频率：
+
+```yaml
+hosts:
+  - [https://raw.hellogithub.com/hosts, 3600]
+```
+
+上面的配置表示，程序每隔 3600 秒重新载入一次 https://raw.hellogithub.com/hosts 的数据。
+
+### 2.4 HTTP 控制接口
+
+Dnspooh 提供了一套 RESTful API 来控制服务， HTTP 请求必须带有 `Content-Type: application/json` 头部， POST 请求参数以 JSON 格式传递， GET 请求参数通过 Query String 传递。
+
+HTTP 服务默认绑定 127.0.0.1 地址，使用 1024 到 65535 范围内的随机端口，程序启动时会在命令行终端输出 HTTP 接口的 URL 地址。
+
+如果接口调用成功，返回一个包含 `result` 字段的 JSON 实体。其中 `result` 字段的值为接口返回值。如果接口调用失败，返回一个包含 `error` 字段的 JSON 实体。其中 `error` 字段的值为错误对象，包含 `code` 和 `message` 两个成员。一个典型的错误对象实体如下：
+
+```json
+{
+    "error": {
+        "code": 0,
+        "message": "执行失败"
+    }
+}
+```
+
+#### 2.4.1 获取程序版本
+
+**方法：** GET
+
+**路径：** `/version`
+
+**参数：** 无
+
+**返回值：** String
+
+```json
+{ "result": "1.0.0" }
+```
+
+#### 2.4.2 获取服务状态
+
+**方法：** GET
+
+**路径：** `/status`
+
+**参数：** 无
+
+**返回值：** String
+
+```json
+{ "result": "RUNNING" }
+```
+
+`status` 可能的返回值如下（其中几种状态可能永远观测不到）：
+
+- INITIALIZED 已初始化
+- START_PEDDING 正在启动
+- RUNNING 正在运行
+- RESTART_PEDDING 正在重启
+- STOP_PEDDING 正在停止
+- STOPPED 已停止
+
+#### 2.4.3 重启服务
+
+重启服务不会影响 HTTP 服务。重启服务过程中会重新载入并应用配置文件，但修改配置文件中的 `http` 下的配置不会因重启服务而生效。
+
+**方法：** POST
+
+**路径：** `/restart`
+
+**参数：** 无
+
+**返回值：** Boolean
+
+```json
+{ "result": true }
+```
+
+#### 2.4.4 获取上游 DNS 服务器
+
+**方法：** GET
+
+**路径：** `/upstream`
+
+**参数：** 无
+
+**返回值：** JSON 对象
+
+```json
+{
+    "result": {
+        "primary": {
+            "name": "cloudflare-1",
+            "disable": false,
+            "groups": ["cloudflare", "global", "ipv4"],
+            "health": 100,
+            "host": "1.1.1.1",
+            "port": 53,
+            "priority": 988,
+            "type": "dns"
+        },
+        "upstreams": [
+            {
+                "name": "cloudflare-1",
+                "disable": false,
+                "groups": ["cloudflare", "global", "ipv4"],
+                "health": 100,
+                "host": "1.1.1.1",
+                "port": 53,
+                "priority": 988,
+                "type": "dns"
+            },
+            // ... ...
+        ]
+    }
+}
+```
+
+#### 2.4.5 设置主 DNS 服务器
+
+**方法：** POST
+
+**路径：** `/upstream/primary`
+
+**参数：** 
+
+| 字段 | 类型   | 描述                               |
+| ---- | ------ | ---------------------------------- |
+| name | String | 服务器名称。例如：`"cloudflare-1"` |
+
+**返回值：** Boolean
+
+```json
+{ "result": true }
+```
+
+#### 2.4.6 测试全部 DNS 服务器
+
+**方法：** POST
+
+**路径：** `/upstreams/test-all`
+
+**参数：** 无
+
+**返回值：** Boolean
+
+```json
+{ "result": true }
+```
+
+#### 2.4.7 获取连接池
+
+**方法：** GET
+
+**路径：** `/pool`
+
+**参数：** 无
+
+**返回值：** Array
+
+```json
+{
+    "result": [
+        { "name": "socks5://127.0.0.1:1080/udp://1.1.1.1:53", "size": 6 },
+        // ... ...
+    ]
+}
+```
+
+#### 2.4.8 获取配置信息
+
+**方法：** GET
+
+**路径：** `/config`
+
+**参数：** 无
+
+**返回值：** Array
+
+```json
+{
+    "result": [
+        { "name": "debug", "value": false },
+        { "name": "secure", "value": false },
+        { "name": "ipv6", "value": false },
+        // ... ...
+    ]
+}
+```
+
+#### 2.4.9 获取解析日志
+
+**方法：** GET
+
+**路径：** `/logs`
+
+**参数：** 
+
+| 字段  | 类型    | 描述                         |
+| ----- | ------- | ---------------------------- |
+| page  | Integer | 页码。可选，默认展示第一页。 |
+| qname | String  | 筛选域名关键字。可选。       |
+| qtype | String  | 筛选查询类型。可选。         |
+
+**返回值：** JSON 对象
+
+```json
+{
+    "result": {
+        "total": 12,
+        "page": {
+            "current": 1,
+            "size": 50,
+            "count": 1
+        },
+        "logs": [
+            {
+                "id": 12,
+                "created_at": "2023-03-08 18:49:19",
+                "elapsed_time": 0.004754199995659292,
+                "qname": "www.google.com.",
+                "qtype": "AAAA",
+                "success": 1,
+                "traceback": ["cache", "block", "Server", "alidns-1"],
+                "error": null
+            },
+            // ... ...
+        ]
+    }
+}
+```
+
+#### 2.4.10 清空解析日志
+
+**方法：** POST
+
+**路径：** `/logs/clear`
+
+**参数：** 无
+
+**返回值：** Boolean
+
+```json
+{ "result": true }
+```
+
+#### 2.4.11 域名解析
+
+**方法：** POST
+
+**路径：** `/dns-query`
+
+**参数：** 
+
+| 字段   | 类型   | 描述   |
+| ------ | ------ | ------ |
+| domain | String | 域名。 |
+
+**返回值：**String
+
+```json
+{ "result": ";; ->>HEADER<<- opcode: QUERY, status: NOERROR, ... ..." }
+```
+
+#### 2.4.12 查询 IP 地理位置
+
+**方法：** POST
+
+**路径：** `/geoip2-query`
+
+**参数：** 无
+
+**返回值：** JSON 对象
+
+```json
+{
+    "result": {
+        "country": {
+            "geoname_id": 1814991,
+            "is_in_european_union": false,
+            "iso_code": "CN",
+            "names": {
+                "de": "China",
+                "en": "China",
+                "es": "China",
+                "fr": "Chine",
+                "ja": "\u4e2d\u56fd",
+                "pt-BR": "China",
+                "ru": "\u041a\u0438\u0442\u0430\u0439",
+                "zh-CN": "\u4e2d\u56fd"
+            }
+        }
+    }
+}
+```
+
+### 2.5 Web 管理界面
+
+![Screenshot](./assets/screenshot.png?raw=true)
+
+要启用 Web 管理界面需要在配置文件中指定前端文件的保存路径：
+
+```yaml
+http
+  root: dashboard/public
+```
+
+在发布的可执行软件包中已经预置了 Web 前端而无需另外配置。
+
+## 3. 自定义规则
+
+通过自定义规则中间件，可以实现按条件屏蔽域名、自定义解析结果等操作。可以在配置文件的 `rules` 单元中设置一组或多组规则，每组规则由 `if` 、 `then` 、 `before` 、 `after` 、 `end` 字段组合而成。根据不同的需求，一组规则可以由 `if/then/end` 字段组成；或者由 `if/before/after/end` 字段组成。其中 `end` 字段是可选的，表示命中并处理完此条规则后是否停止处理后续规则，默认值为 `false` ； `if` 字段是一个表达式，当表达式结果为真时，则表示命中这条规则； `then` 字段是一条语句，可以在此处直接拦截 DNS 解析请求，直接返回 NXDOMAIN （域名不存在）或自定义解析结果，而不会将请求转发到上游服务器； `before` 字段是一组逗号分隔的命令语句，在 DNS 解析请求被转发到上游服务器之前被处理，可以用于指定上游服务器以及替换请求中的域名； `after` 字段也是一组逗号分隔的命令语句，在 DNS 解析结果从上游服务器返回之后被处理，可以根据返回的结果进行修改操作或执行外部命令。
+
+配置例子：
+
+```yaml
+rules:
+  - if: (lianmeng, adwords, adservice) in domian
+    then: block
+    end: true
+
+  - if: domain ends with (.cn, .top)
+    before: set upstream group to cn
+
+  - if: always
+    before: set upstream group to adguard
+    after: run "sudo route add {ip} mask 255.255.255.255 192.168.1.1" where geoip is cn
+```
+
+上面的配置作用是：
+
+1. 屏蔽含有 lianmeng 、 adwords 、 adservice 关键字的域名；
+2. 让 .cn 和 .top 域名使用国内的 DNS 服务器解析；
+3. 默认使用 adguard 作为上游域名解析服务器。adguard 服务器可以屏蔽所有广告域名；
+4. 当返回的解析结果中包含国内 IP 时，将此 IP 加入本机路由表，使用 192.168.1.1 网关路由（当开启全局 VPN 时，使用本地网络访问国内 IP ）。
+
+所有的表达式都支持 `not` 、 `and` 和 `or` 逻辑运算，按优先级排列如下：
+
+1. not *expr*
+2. *expr* and *expr*
+3. *expr* or *expr*
+
+可以用圆括号运算符 `(` 与 `)` 来改变逻辑运算符的优先级。
+
+```yaml
+rules:
+  - if: (domain ends with .cn or domain ends with .top) and not blog in domain
+    then: block
+    end: true
+```
+
+上面的配置作用是，如果是 .cn 或 .top 域名，且域名中没有包含 blog 关键字，则屏蔽。
+
+### 3.1 if 表达式
+
+if 字段由一个或多个判断条件组成的逻辑运算表达式。支持的判断条件有：
+
+- domain is *domain*  
+  域名等于 *domain*
+- domain is (*domain1*, *domain2*, ...)  
+  域名与列表中任一 *domain* 相等，等价于 domain is *domain1* or domain is *domain2* or ... 
+- domain is not *domain*  
+  域名不等于 *domain* ，等价于 not domain is *domain*
+- domain is not (*domain1*, *domain2*, ...)  
+  域名不等于列表中的任何 *domain* ，等价于 domain is not *domain1* and domain is not *domain2* and ...
+- *keyword* in domain  
+  域名包含 *keyword*
+- (*keyword1*, *keyword2*, ...) in domain  
+  域名包含列表中任一 *keyword* ，等价于 *keyword1* in domain or *keyword2* in domain or ...
+- *keyword* not in domain  
+  域名不包含 *keyword* ，等价于 not *keyword* in domain
+- (*keyword1*, *keyword2*, ...) not in domain  
+  域名不包含列表中的任何 *keyword* ，等价于 *keyword1* not in domain and *keyword2* not in domain and ...
+- domain starts with *prefix*  
+  域名前缀为 *prefix*
+- domain starts with (*prefix1*, *prefix2*, ...)  
+  域名前缀是列表中的任一 *prefix* ，等价于 domain starts with *prefix1* or domain starts with *prefix2* or ...    
+- domain starts without *prefix*  
+  域名前缀不为 *prefix* ，等价于 not domain starts with *prefix*  
+- domain starts without (*prefix1*, *prefix2*, ...)  
+  域名前缀不为列表中的任何 *prefix* ，等价于 domain starts without *prefix1* and domain starts without *prefix2* and ...
+- domain ends with *suffix*  
+  域名后缀为 *suffix*
+- domain ends with (*suffix1*, *suffix2*, ...)  
+  域名后缀为列表中的任一 *suffix* ，等价于 domain starts with *suffix1* or domain starts with *suffix2* or ...    
+- domain ends without *suffix*  
+  域名后缀不为 *suffix* ，等价于 not domain ends with *suffix*  
+- domain ends without (*suffix1*, *suffix2*, ...)  
+  域名后缀不为列表中的任何 *suffix* ，等价于 domain ends without *suffix1* and domain ends without *suffix2* and ...    
+- domain match /*regex*/  
+  域名完整匹配正则表达式 *regex*
+- always  
+  总是为真
+
+### 3.2 then 语句
+
+then 字段可以是下列任意语句之一：
+
+- block  
+  屏蔽当前请求
+- return *ip*  
+- return (*ip1*, *ip2*, ...)  
+  直接返回解析结果
+
+### 3.3 before 语句
+
+before 字段由下列一条或多条逗号分隔的语句组成：
+
+- set upstream group to *name*  
+  使用 *name* 组中的上游服务器来解析域名
+- set upstream name to *name*  
+  使用名称为 *name* 的上游服务器来解析域名
+- replace domain by *domain*  
+  将请求中的域名替换为 *domain*
+- set proxy on  
+  启用代理服务器访问上游服务器（须在配置文件中设置 proxy 项）
+- set proxy off  
+  禁用代理服务器访问上游服务器
+- set proxy to *proxy*  
+  指定代理服务器访问上游服务器。*proxy* 格式如 http://127.0.0.1:8080 或 socks5://127.0.0.1:1080 
+
+### 3.4 after 语句
+
+- block if *expr1*  
+  当解析结果满足条件（ *expr1* 表达式为真）时，屏蔽域名
+- return *ip* if *expr1*  
+  当解析结果满足条件（ *expr1* 表达式为真）时，用 *ip* 替代解析结果
+- return (*ip1*, *ip2*, ...) if *expr1*
+- append record *ip*  
+  在上游服务器返回的解析结果后追加记录
+- append record (*ip1*, *ip2*, ...)
+- append record *ip* if *expr1*
+- append record (*ip1*, *ip2*, ...) if *expr1*
+- insert record *ip*  
+  在上游服务器返回的解析结果前插入记录
+- insert record (*ip1*, *ip2*, ...)
+- insert record *ip* if *expr1*
+- insert record (*ip1*, *ip2*, ...) if *expr1*
+- remove record where *expr2*  
+  从解析结果中移除满足条件（ *expr2* 表达式为真）的记录
+- replace record by *ip* where *expr2*  
+  用 *ip* 替换满足条件（ *expr2* 表达式为真）的记录
+- run "*command*" where *expr2*  
+  当解析结果中存在满足条件的记录时，执行 *command* 命令。命令需要用半角双引号包裹，命令中可以使用 `{ip}` 占位符表示当前记录的 IP 地址。
+
+#### 3.4.1 expr1 类型表达式
+
+- any ip is *ip*  
+  解析结果中存在 IP 地址等于 *ip* 的记录
+- any ip is (*ip1*, *ip2*, ...)
+- any ip is not *ip*
+- any ip is not (*ip1*, *ip2*, ...)
+- any ip in *cidr*  
+  解析结果中存在 IP 地址在 *cidr* 范围内的记录。 *cidr* 使用 IP-CIDR 格式表示，如 192.168.1.1/24
+- any ip in (*cidr1*, *cidr2*, ...)
+- any ip not in *cidr*
+- any ip not in (*cidr1*, *cidr2*, ...)
+- any geoip is *country*  
+  解析结果中存在 IP 地址所在国为 *country* 的记录
+- any geoip is not *country*
+- all ip is *ip*  
+  解析结果中所有记录的 IP 地址都等于 *ip* 
+- all ip is (*ip1*, *ip2*, ...)
+- all ip is not *ip*
+- all ip is not (*ip1*, *ip2*, ...)
+- all ip in *cidr*  
+  解析结果中所有记录的 IP 地址都在 *cidr* 范围内 
+- all ip in (*cidr1*, *cidr2*, ...)
+- all ip not in *cidr*
+- all ip not in (*cidr1*, *cidr2*, ...)
+- all geoip is *country*  
+  解析结果中所有记录的 IP 所在国都为 *country*  
+- all geoip is not *country*
+
+#### 3.4.2 expr2 类型表达式
+
+- ip is *ip*
+- ip is (*ip1*, *ip2*, ....)
+- ip is not *ip*
+- ip is not (*ip1*, *ip2*, ....)
+- ip in *cidr*
+- ip in (*cidr1*, *cidr2*, ...)
+- ip not in *cidr*
+- ip not in (*cidr1*, *cidr2*, ...)
+- geoip is *country*
+- geoip is not *country*
+- first  
+  第一条记录
+- last  
+  最后一条记录
+
+## 4. 特性
+
+- 如果 DNS 解析请求中包含多条查询，会被逐条拆分后发送至上游服务器，并在返回响应时重新组合。这么做的目的是为了方便中间件处理；
+- 程序在引导时会优先使用 priority 值最大的 upstream 来解析 DoH 服务器的域名。默认使用 cloudflare-tls 服务器进行引导时解析；
+- 程序启动时会测试配置中所有的上游服务器，并将响应最快的服务器设置为主服务器；
+- 程序内置的 GeoIP2 数据库仅包含中国 IP 段数据，只能返回 `cn` 或空。要使用完整的 GeoIP2 数据库，可以在配置文件中指定数据库文件；
+- 程序内置的上游 DNS 解析服务器包括：[Cloudflare DNS](https://1.1.1.1/dns/) (cloudflare), [Google Public DNS](https://developers.google.com/speed/public-dns) (google), [阿里公共DNS](https://alidns.com/) (alidns), [114DNS](https://www.114dns.com/) (114dns), [OneDNS ](https://www.onedns.net/)(onedns), [DNSPod](https://www.dnspod.cn/) (dnspod), [百度DNS](https://dudns.baidu.com/)(baidu), [OpenDNS](https://www.opendns.com/) (opendns), [AdGuard DNS](https://adguard-dns.io/) (adguard) 。这些服务器按照服务供应商的名称（见括号内）分为不同组；根据服务器所在地，分为 cn 组和 global 组；根据服务器网络类型，分为 ipv4 组和 ipv6 组。
+
+## 5. 常用命令
+
+模块构建打包（需要安装 build 模块）：
+
+```shell
+pip install build
+python -m build
+```
+
+运行单元测试：
+
+```shell
+python -m unittest tests
+```
+
+项目发布的可执行文件使用 [Nuitka-winsvc](https://github.com/tabris17/Nuitka-winsvc) 编译。首先安装依赖的包：
+
+```shell
+pip install nuitka ordered-set zstandard dnspooh
+```
+
+官方发布的 Windows 程序使用如下 Nuitka 命令编译：
+
+```shell
+nuitka --standalone --output-dir=build --output-filename=dnspooh --windows-icon-from-ico=./assets/favicon.ico --include-package-data=dnspooh --onefile --windows-service --windows-service-name=dnspooh --windows-service-display-name=Dnspooh --windows-service-description="A lightweight DNS MitM proxy" main.py
+```
+
+启动 Web 管理界面前端开发环境：
+
+```shell
+npm i
+npm run dev
+```
+
+构建 Web 管理界面前端：
+
+```shell
+npm run build
+```
+
```

### Comparing `dnspooh-1.3.1/dnspooh.egg-info/SOURCES.txt` & `dnspooh-1.3.2/dnspooh.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 dnspooh/server.py
 dnspooh/timers.py
 dnspooh/upstream.py
 dnspooh/version.py
 dnspooh.egg-info/PKG-INFO
 dnspooh.egg-info/SOURCES.txt
 dnspooh.egg-info/dependency_links.txt
-dnspooh.egg-info/entry_points.txt
 dnspooh.egg-info/not-zip-safe
 dnspooh.egg-info/requires.txt
 dnspooh.egg-info/top_level.txt
 dnspooh/middlewares/__init__.py
 dnspooh/middlewares/block.py
 dnspooh/middlewares/cache.py
 dnspooh/middlewares/hosts.py
```

### Comparing `dnspooh-1.3.1/tests/block.py` & `dnspooh-1.3.2/tests/block.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import unittest
-import pathlib
-import tempfile
-
-import dnslib
-
-from dnspooh.middlewares import BlockMiddleware
-from . import Server, dns_request, dns_answer, dns_response
-
-
-server = Server()
-
-
-async def create_middleware(**kwargs):
-    with tempfile.TemporaryDirectory() as path:
-        base_path = pathlib.Path(path)
-        filenames = []
-        for name, content in kwargs.items():
-            block_filename = str(base_path.joinpath(name + '.txt'))
-            filenames.append(block_filename)
-            with open(block_filename, 'w+') as fp:
-                fp.write(content)
-        block = BlockMiddleware(*filenames)
-        block.initialize(server, 'block')
-        await block.bootstrap()
-    return block
-
-
-class BlockTest(unittest.IsolatedAsyncioTestCase):
-    async def test_block(self):
-        block = await create_middleware(
-            block1='www.baidu.com', 
-            block2='weixin.qq.com',
-            block3='ip:127.0.0.1', 
-            block4='ip:127.0.0.2'
-        )
-        request = dns_request('www.baidu.com')
-        response = await block.handle(request, answer='127.0.0.1')
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-        request = dns_request('weixin.qq.com')
-        response = await block.handle(request, answer='127.0.0.1')
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-
-        request = dns_request('localhost')
-        response = await block.handle(request, answer='127.0.0.1')
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-        request = dns_request('localhost')
-        response = await block.handle(request, answer='127.0.0.2')
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+import unittest
+import pathlib
+import tempfile
+
+import dnslib
+
+from dnspooh.middlewares import BlockMiddleware
+from . import Server, dns_request, dns_answer, dns_response
+
+
+server = Server()
+
+
+async def create_middleware(**kwargs):
+    with tempfile.TemporaryDirectory() as path:
+        base_path = pathlib.Path(path)
+        filenames = []
+        for name, content in kwargs.items():
+            block_filename = str(base_path.joinpath(name + '.txt'))
+            filenames.append(block_filename)
+            with open(block_filename, 'w+') as fp:
+                fp.write(content)
+        block = BlockMiddleware(*filenames)
+        block.initialize(server, 'block')
+        await block.bootstrap()
+    return block
+
+
+class BlockTest(unittest.IsolatedAsyncioTestCase):
+    async def test_block(self):
+        block = await create_middleware(
+            block1='www.baidu.com', 
+            block2='weixin.qq.com',
+            block3='ip:127.0.0.1', 
+            block4='ip:127.0.0.2'
+        )
+        request = dns_request('www.baidu.com')
+        response = await block.handle(request, answer='127.0.0.1')
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+        request = dns_request('weixin.qq.com')
+        response = await block.handle(request, answer='127.0.0.1')
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+
+        request = dns_request('localhost')
+        response = await block.handle(request, answer='127.0.0.1')
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+        request = dns_request('localhost')
+        response = await block.handle(request, answer='127.0.0.2')
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
```

### Comparing `dnspooh-1.3.1/tests/rules.py` & `dnspooh-1.3.2/tests/rules.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-import unittest
-import ipaddress
-
-import dnslib
-
-from dnspooh.middlewares.rules import RuleIfParser, RuleThenParser, RuleBeforeParser, RuleAfterParser, ReplacDomainHandler
-
-from . import dns_request, dns_answer, dns_response
-
-
-if_parser = RuleIfParser()
-then_parser = RuleThenParser()
-before_parser = RuleBeforeParser()
-after_parser = RuleAfterParser()
-
-
-class RuleIfTest(unittest.TestCase):
-    def test_in_domain(self):
-        self.assertTrue(if_parser.parse('qq in domain').test('weixin.qq.com'))
-        self.assertTrue(if_parser.parse('(qq, weibo) in domain').test('weixin.qq.com'))
-        self.assertFalse(if_parser.parse('(qq, weibo) in domain').test('taobao.com'))
-
-    def test_not_in_domain(self):
-        self.assertFalse(if_parser.parse('qq not in domain').test('weixin.qq.com'))
-        self.assertFalse(if_parser.parse('(qq, weibo) not in domain').test('weixin.qq.com'))
-        self.assertTrue(if_parser.parse('(qq, weibo) not in domain').test('taobao.com'))
-
-    def test_domain_is(self):
-        self.assertTrue(if_parser.parse('domain is qq.com').test('qq.com'))
-        self.assertTrue(if_parser.parse('domain is (baidu.com, taobao.com, weibo.com, qq.com)').test('qq.com'))
-        self.assertFalse(if_parser.parse('domain is (baidu.com, taobao.com, weibo.com, qq.com)').test('tencent.com'))
-
-    def test_domain_is_not(self):
-        self.assertFalse(if_parser.parse('domain is not qq.com').test('qq.com'))
-        self.assertFalse(if_parser.parse('domain is not (baidu.com, taobao.com, weibo.com, qq.com)').test('qq.com'))
-        self.assertTrue(if_parser.parse('domain is not (baidu.com, taobao.com, weibo.com, qq.com)').test('tencent.com'))
-
-    def test_domain_starts_with(self):
-        self.assertTrue(if_parser.parse('domain starts with www').test('www.qq.com'))
-        self.assertTrue(if_parser.parse('domain starts with (mobile, www, test)').test('www.qq.com'))
-        self.assertFalse(if_parser.parse('domain starts with (mobile, www, test)').test('tencent.com'))
-
-    def test_domain_starts_without(self):
-        self.assertFalse(if_parser.parse('domain starts without www').test('www.qq.com'))
-        self.assertFalse(if_parser.parse('domain starts without (mobile, www, test)').test('www.qq.com'))
-        self.assertTrue(if_parser.parse('domain starts without (mobile, www, test)').test('tencent.com'))
-
-    def test_domain_ends_with(self):
-        self.assertTrue(if_parser.parse('domain ends with .com').test('www.qq.com'))
-        self.assertTrue(if_parser.parse('domain ends with (.com, .cn, .com.cn)').test('www.qq.com'))
-        self.assertFalse(if_parser.parse('domain ends with (.com, .cn, .com.cn)').test('mozilla.org'))
-
-    def test_domain_ends_without(self):
-        self.assertFalse(if_parser.parse('domain ends without .com').test('www.qq.com'))
-        self.assertFalse(if_parser.parse('domain ends without (.com, .cn, .com.cn)').test('www.qq.com'))
-        self.assertTrue(if_parser.parse('domain ends without (.com, .cn, .com.cn)').test('mozilla.org'))
-
-    def test_domain_match(self):
-        self.assertTrue(if_parser.parse('domain match /w+\.baidu\.com/').test('www.baidu.com'))
-        self.assertFalse(if_parser.parse('domain match /w+\.baidu\.com/').test('baidu.com'))
-
-    def test_not_and_or(self):
-        self.assertTrue(if_parser.parse('domain is qq.com or domain ends with baidu.com and not qq in domain').test('www.baidu.com'))
-
-
-class RuleThenTest(unittest.TestCase):
-    def test_block(self):
-        response = then_parser.parse('block').exec(dns_request('qq.com'))
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-
-    def test_return(self):
-        response = then_parser.parse('return 127.0.0.1').exec(dns_request('qq.com'))
-        record = response.rr[0]
-        self.assertEqual(record.rtype, dnslib.QTYPE.A)
-        self.assertEqual(str(record.rdata), '127.0.0.1')
-        response = then_parser.parse('return (127.0.0.1, 127.0.0.2, 127.0.0.3)').exec(dns_request('qq.com'))
-        self.assertEqual(response.header.a, 3)
-        self.assertEqual(str(response.rr[0].rdata), '127.0.0.1')
-        self.assertEqual(str(response.rr[1].rdata), '127.0.0.2')
-        self.assertEqual(str(response.rr[2].rdata), '127.0.0.3')
-
-
-class RuleBeforeTest(unittest.TestCase):
-    def test_replace_domain(self):
-        kwargs = dict()
-        request = dns_request('baidu.com')
-        after_handler = before_parser.parse('replace domain by google.com').exec(request, kwargs)
-        self.assertTrue(isinstance(after_handler, ReplacDomainHandler))
-        self.assertEqual(request.q.qname, 'google.com')
-        response = after_handler.after_handle(dns_answer(request, '127.0.0.1'), None, None, None)
-        self.assertEqual(response.q.qname, 'baidu.com')
-
-    def test_set_upstream(self):
-        kwargs = dict()
-        request = dns_request('baidu.com')
-        before_parser.parse('set upstream group to cn, set upstream name to cloudflare-tls').exec(request, kwargs)
-        self.assertEqual(kwargs['upstream_group'], 'cn')
-        self.assertEqual(kwargs['upstream_name'], 'cloudflare-tls')
-
-    def test_set_proxy(self):
-        proxy = 'socks5://127.0.0.0:1080'
-        kwargs = dict()
-        request = dns_request('baidu.com')
-        before_parser.parse('set proxy on').exec(request, kwargs)
-        self.assertTrue('proxy' not in kwargs)
-        before_parser.parse('set proxy off').exec(request, kwargs)
-        self.assertEqual(kwargs['proxy'], None)
-        before_parser.parse('set proxy to ' + proxy).exec(request, kwargs)
-        self.assertEqual(kwargs['proxy'], proxy)
-
-
-def geoip(code):
-    def _geoip(_):
-        return code
-    return _geoip
-
-
-def ipaddr(record):
-    ip_str = str(record.rdata)
-    if record.rtype == dnslib.QTYPE.A:
-        return ipaddress.IPv4Address(ip_str)
-    elif record.rtype == dnslib.QTYPE.AAAA:
-        return ipaddress.IPv6Address(ip_str)
-
-def run(command):
-    print('shell:', command)
-    return
-
-class RuleAfterTest(unittest.TestCase):
-    def test_block_if(self):
-        response = after_parser.parse('block if always').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-
-    def test_return_if(self):
-        response = after_parser.parse('return 127.0.0.10 if always').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        record = response.rr[0]
-        self.assertEqual(record.rtype, dnslib.QTYPE.A)
-        self.assertEqual(str(record.rdata), '127.0.0.10')
-        response = after_parser.parse('return (127.0.0.1, 127.0.0.2, 127.0.0.3) if always').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.a, 3)
-        self.assertEqual(str(response.rr[0].rdata), '127.0.0.1')
-        self.assertEqual(str(response.rr[1].rdata), '127.0.0.2')
-        self.assertEqual(str(response.rr[2].rdata), '127.0.0.3')
-    
-    def test_add_record(self):
-        response = after_parser.parse('add record (127.0.0.3, 127.0.0.4)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        response = after_parser.parse('add record 127.0.0.5 if always').exec(response, geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.a, 5)
-        self.assertEqual(str(response.rr[0].rdata), '127.0.0.1')
-        self.assertEqual(str(response.rr[1].rdata), '127.0.0.2')
-        self.assertEqual(str(response.rr[2].rdata), '127.0.0.3')
-        self.assertEqual(str(response.rr[3].rdata), '127.0.0.4')
-        self.assertEqual(str(response.rr[4].rdata), '127.0.0.5')
-    
-    def test_append_record(self):
-        response = after_parser.parse('append record (127.0.0.3, 127.0.0.4)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        response = after_parser.parse('append record 127.0.0.5 if always').exec(response, geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.a, 5)
-        self.assertEqual(str(response.rr[0].rdata), '127.0.0.1')
-        self.assertEqual(str(response.rr[1].rdata), '127.0.0.2')
-        self.assertEqual(str(response.rr[2].rdata), '127.0.0.3')
-        self.assertEqual(str(response.rr[3].rdata), '127.0.0.4')
-        self.assertEqual(str(response.rr[4].rdata), '127.0.0.5')
-    
-    def test_insert_record(self):
-        response = after_parser.parse('insert record (127.0.0.2, 127.0.0.3)').exec(dns_response('qq.com', '127.0.0.4', '127.0.0.5'), geoip('cn'), ipaddr, run)
-        response = after_parser.parse('insert record 127.0.0.1 if always').exec(response, geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.a, 5)
-        self.assertEqual(str(response.rr[0].rdata), '127.0.0.1')
-        self.assertEqual(str(response.rr[1].rdata), '127.0.0.2')
-        self.assertEqual(str(response.rr[2].rdata), '127.0.0.3')
-        self.assertEqual(str(response.rr[3].rdata), '127.0.0.4')
-        self.assertEqual(str(response.rr[4].rdata), '127.0.0.5')
-
-    def test_remove_record(self):
-        response = after_parser.parse('remove record where ip is 127.0.0.1').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.a, 1)
-        self.assertEqual(str(response.rr[0].rdata), '127.0.0.2')
-
-    def test_replace_record(self):
-        response = after_parser.parse('replace record by 192.168.1.1 where ip is 127.0.0.1').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.a, 2)
-        self.assertEqual(str(response.rr[0].rdata), '192.168.1.1')
-        self.assertEqual(str(response.rr[1].rdata), '127.0.0.2')
-
-    def test_any_ip_is(self):
-        response = after_parser.parse('block if any ip is 127.0.0.1').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-        response = after_parser.parse('block if any ip is (127.0.0.1, 192.168.1.2)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-
-    def test_any_ip_is_not(self):
-        response = after_parser.parse('block if any ip is not 127.0.0.1').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-        response = after_parser.parse('block if any ip is not (127.0.0.1, 127.0.0.3)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-
-    def test_all_ip_is(self):
-        response = after_parser.parse('block if all ip is 127.0.0.1').exec(dns_response('qq.com', '127.0.0.1'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-        response = after_parser.parse('block if all ip is (127.0.0.1, 127.0.0.2)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-
-    def test_all_ip_is_not(self):
-        response = after_parser.parse('block if all ip is not 192.168.1.1').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-        response = after_parser.parse('block if all ip is not (192.168.1.1, 192.168.1.2)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-
-    def test_any_ip_in(self):
-        response = after_parser.parse('block if any ip in 127.0.0.1/24').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-        response = after_parser.parse('block if any ip in (127.0.0.1/24, 192.168.1.2/24)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-
-    def test_any_ip_not_in(self):
-        response = after_parser.parse('block if any ip not in 127.0.0.1/24').exec(dns_response('qq.com', '127.0.0.1', '172.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-        response = after_parser.parse('block if any ip not in (127.0.0.1/24, 192.168.1.1/24)').exec(dns_response('qq.com', '127.0.0.1', '172.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-
-    def test_all_ip_in(self):
-        response = after_parser.parse('block if all ip in 127.0.0.1/24').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-        response = after_parser.parse('block if all ip in (127.0.0.1/24, 172.0.0.2/24)').exec(dns_response('qq.com', '127.0.0.1', '172.0.0.1'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-
-    def test_all_ip_not_in(self):
-        response = after_parser.parse('block if all ip not in 192.168.1.1/24').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-        response = after_parser.parse('block if all ip not in (192.168.1.1/24, 192.168.253.1/24)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-
-    def test_geoip_is(self):
-        response = after_parser.parse('block if any geoip is cn').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-        response = after_parser.parse('block if all geoip is cn').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-
-    def test_geoip_is_not(self):
-        response = after_parser.parse('block if any geoip is not cn').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('en'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-        response = after_parser.parse('block if all geoip is not cn').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('en'), ipaddr, run)
-        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
-
-    def test_first_last(self):
-        response = after_parser.parse('remove record where first or last').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2', '127.0.0.3'), geoip('cn'), ipaddr, run)
-        self.assertEqual(response.header.a, 1)
-        self.assertEqual(str(response.rr[0].rdata), '127.0.0.2')
+import unittest
+import ipaddress
+
+import dnslib
+
+from dnspooh.middlewares.rules import RuleIfParser, RuleThenParser, RuleBeforeParser, RuleAfterParser, ReplacDomainHandler
+
+from . import dns_request, dns_answer, dns_response
+
+
+if_parser = RuleIfParser()
+then_parser = RuleThenParser()
+before_parser = RuleBeforeParser()
+after_parser = RuleAfterParser()
+
+
+class RuleIfTest(unittest.TestCase):
+    def test_in_domain(self):
+        self.assertTrue(if_parser.parse('qq in domain').test('weixin.qq.com'))
+        self.assertTrue(if_parser.parse('(qq, weibo) in domain').test('weixin.qq.com'))
+        self.assertFalse(if_parser.parse('(qq, weibo) in domain').test('taobao.com'))
+
+    def test_not_in_domain(self):
+        self.assertFalse(if_parser.parse('qq not in domain').test('weixin.qq.com'))
+        self.assertFalse(if_parser.parse('(qq, weibo) not in domain').test('weixin.qq.com'))
+        self.assertTrue(if_parser.parse('(qq, weibo) not in domain').test('taobao.com'))
+
+    def test_domain_is(self):
+        self.assertTrue(if_parser.parse('domain is qq.com').test('qq.com'))
+        self.assertTrue(if_parser.parse('domain is (baidu.com, taobao.com, weibo.com, qq.com)').test('qq.com'))
+        self.assertFalse(if_parser.parse('domain is (baidu.com, taobao.com, weibo.com, qq.com)').test('tencent.com'))
+
+    def test_domain_is_not(self):
+        self.assertFalse(if_parser.parse('domain is not qq.com').test('qq.com'))
+        self.assertFalse(if_parser.parse('domain is not (baidu.com, taobao.com, weibo.com, qq.com)').test('qq.com'))
+        self.assertTrue(if_parser.parse('domain is not (baidu.com, taobao.com, weibo.com, qq.com)').test('tencent.com'))
+
+    def test_domain_starts_with(self):
+        self.assertTrue(if_parser.parse('domain starts with www').test('www.qq.com'))
+        self.assertTrue(if_parser.parse('domain starts with (mobile, www, test)').test('www.qq.com'))
+        self.assertFalse(if_parser.parse('domain starts with (mobile, www, test)').test('tencent.com'))
+
+    def test_domain_starts_without(self):
+        self.assertFalse(if_parser.parse('domain starts without www').test('www.qq.com'))
+        self.assertFalse(if_parser.parse('domain starts without (mobile, www, test)').test('www.qq.com'))
+        self.assertTrue(if_parser.parse('domain starts without (mobile, www, test)').test('tencent.com'))
+
+    def test_domain_ends_with(self):
+        self.assertTrue(if_parser.parse('domain ends with .com').test('www.qq.com'))
+        self.assertTrue(if_parser.parse('domain ends with (.com, .cn, .com.cn)').test('www.qq.com'))
+        self.assertFalse(if_parser.parse('domain ends with (.com, .cn, .com.cn)').test('mozilla.org'))
+
+    def test_domain_ends_without(self):
+        self.assertFalse(if_parser.parse('domain ends without .com').test('www.qq.com'))
+        self.assertFalse(if_parser.parse('domain ends without (.com, .cn, .com.cn)').test('www.qq.com'))
+        self.assertTrue(if_parser.parse('domain ends without (.com, .cn, .com.cn)').test('mozilla.org'))
+
+    def test_domain_match(self):
+        self.assertTrue(if_parser.parse('domain match /w+\.baidu\.com/').test('www.baidu.com'))
+        self.assertFalse(if_parser.parse('domain match /w+\.baidu\.com/').test('baidu.com'))
+
+    def test_not_and_or(self):
+        self.assertTrue(if_parser.parse('domain is qq.com or domain ends with baidu.com and not qq in domain').test('www.baidu.com'))
+
+
+class RuleThenTest(unittest.TestCase):
+    def test_block(self):
+        response = then_parser.parse('block').exec(dns_request('qq.com'))
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+
+    def test_return(self):
+        response = then_parser.parse('return 127.0.0.1').exec(dns_request('qq.com'))
+        record = response.rr[0]
+        self.assertEqual(record.rtype, dnslib.QTYPE.A)
+        self.assertEqual(str(record.rdata), '127.0.0.1')
+        response = then_parser.parse('return (127.0.0.1, 127.0.0.2, 127.0.0.3)').exec(dns_request('qq.com'))
+        self.assertEqual(response.header.a, 3)
+        self.assertEqual(str(response.rr[0].rdata), '127.0.0.1')
+        self.assertEqual(str(response.rr[1].rdata), '127.0.0.2')
+        self.assertEqual(str(response.rr[2].rdata), '127.0.0.3')
+
+
+class RuleBeforeTest(unittest.TestCase):
+    def test_replace_domain(self):
+        kwargs = dict()
+        request = dns_request('baidu.com')
+        after_handler = before_parser.parse('replace domain by google.com').exec(request, kwargs)
+        self.assertTrue(isinstance(after_handler, ReplacDomainHandler))
+        self.assertEqual(request.q.qname, 'google.com')
+        response = after_handler.after_handle(dns_answer(request, '127.0.0.1'), None, None, None)
+        self.assertEqual(response.q.qname, 'baidu.com')
+
+    def test_set_upstream(self):
+        kwargs = dict()
+        request = dns_request('baidu.com')
+        before_parser.parse('set upstream group to cn, set upstream name to cloudflare-tls').exec(request, kwargs)
+        self.assertEqual(kwargs['upstream_group'], 'cn')
+        self.assertEqual(kwargs['upstream_name'], 'cloudflare-tls')
+
+    def test_set_proxy(self):
+        proxy = 'socks5://127.0.0.0:1080'
+        kwargs = dict()
+        request = dns_request('baidu.com')
+        before_parser.parse('set proxy on').exec(request, kwargs)
+        self.assertTrue('proxy' not in kwargs)
+        before_parser.parse('set proxy off').exec(request, kwargs)
+        self.assertEqual(kwargs['proxy'], None)
+        before_parser.parse('set proxy to ' + proxy).exec(request, kwargs)
+        self.assertEqual(kwargs['proxy'], proxy)
+
+
+def geoip(code):
+    def _geoip(_):
+        return code
+    return _geoip
+
+
+def ipaddr(record):
+    ip_str = str(record.rdata)
+    if record.rtype == dnslib.QTYPE.A:
+        return ipaddress.IPv4Address(ip_str)
+    elif record.rtype == dnslib.QTYPE.AAAA:
+        return ipaddress.IPv6Address(ip_str)
+
+def run(command):
+    print('shell:', command)
+    return
+
+class RuleAfterTest(unittest.TestCase):
+    def test_block_if(self):
+        response = after_parser.parse('block if always').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+
+    def test_return_if(self):
+        response = after_parser.parse('return 127.0.0.10 if always').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        record = response.rr[0]
+        self.assertEqual(record.rtype, dnslib.QTYPE.A)
+        self.assertEqual(str(record.rdata), '127.0.0.10')
+        response = after_parser.parse('return (127.0.0.1, 127.0.0.2, 127.0.0.3) if always').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.a, 3)
+        self.assertEqual(str(response.rr[0].rdata), '127.0.0.1')
+        self.assertEqual(str(response.rr[1].rdata), '127.0.0.2')
+        self.assertEqual(str(response.rr[2].rdata), '127.0.0.3')
+    
+    def test_add_record(self):
+        response = after_parser.parse('add record (127.0.0.3, 127.0.0.4)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        response = after_parser.parse('add record 127.0.0.5 if always').exec(response, geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.a, 5)
+        self.assertEqual(str(response.rr[0].rdata), '127.0.0.1')
+        self.assertEqual(str(response.rr[1].rdata), '127.0.0.2')
+        self.assertEqual(str(response.rr[2].rdata), '127.0.0.3')
+        self.assertEqual(str(response.rr[3].rdata), '127.0.0.4')
+        self.assertEqual(str(response.rr[4].rdata), '127.0.0.5')
+    
+    def test_append_record(self):
+        response = after_parser.parse('append record (127.0.0.3, 127.0.0.4)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        response = after_parser.parse('append record 127.0.0.5 if always').exec(response, geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.a, 5)
+        self.assertEqual(str(response.rr[0].rdata), '127.0.0.1')
+        self.assertEqual(str(response.rr[1].rdata), '127.0.0.2')
+        self.assertEqual(str(response.rr[2].rdata), '127.0.0.3')
+        self.assertEqual(str(response.rr[3].rdata), '127.0.0.4')
+        self.assertEqual(str(response.rr[4].rdata), '127.0.0.5')
+    
+    def test_insert_record(self):
+        response = after_parser.parse('insert record (127.0.0.2, 127.0.0.3)').exec(dns_response('qq.com', '127.0.0.4', '127.0.0.5'), geoip('cn'), ipaddr, run)
+        response = after_parser.parse('insert record 127.0.0.1 if always').exec(response, geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.a, 5)
+        self.assertEqual(str(response.rr[0].rdata), '127.0.0.1')
+        self.assertEqual(str(response.rr[1].rdata), '127.0.0.2')
+        self.assertEqual(str(response.rr[2].rdata), '127.0.0.3')
+        self.assertEqual(str(response.rr[3].rdata), '127.0.0.4')
+        self.assertEqual(str(response.rr[4].rdata), '127.0.0.5')
+
+    def test_remove_record(self):
+        response = after_parser.parse('remove record where ip is 127.0.0.1').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.a, 1)
+        self.assertEqual(str(response.rr[0].rdata), '127.0.0.2')
+
+    def test_replace_record(self):
+        response = after_parser.parse('replace record by 192.168.1.1 where ip is 127.0.0.1').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.a, 2)
+        self.assertEqual(str(response.rr[0].rdata), '192.168.1.1')
+        self.assertEqual(str(response.rr[1].rdata), '127.0.0.2')
+
+    def test_any_ip_is(self):
+        response = after_parser.parse('block if any ip is 127.0.0.1').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+        response = after_parser.parse('block if any ip is (127.0.0.1, 192.168.1.2)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+
+    def test_any_ip_is_not(self):
+        response = after_parser.parse('block if any ip is not 127.0.0.1').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+        response = after_parser.parse('block if any ip is not (127.0.0.1, 127.0.0.3)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+
+    def test_all_ip_is(self):
+        response = after_parser.parse('block if all ip is 127.0.0.1').exec(dns_response('qq.com', '127.0.0.1'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+        response = after_parser.parse('block if all ip is (127.0.0.1, 127.0.0.2)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+
+    def test_all_ip_is_not(self):
+        response = after_parser.parse('block if all ip is not 192.168.1.1').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+        response = after_parser.parse('block if all ip is not (192.168.1.1, 192.168.1.2)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+
+    def test_any_ip_in(self):
+        response = after_parser.parse('block if any ip in 127.0.0.1/24').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+        response = after_parser.parse('block if any ip in (127.0.0.1/24, 192.168.1.2/24)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+
+    def test_any_ip_not_in(self):
+        response = after_parser.parse('block if any ip not in 127.0.0.1/24').exec(dns_response('qq.com', '127.0.0.1', '172.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+        response = after_parser.parse('block if any ip not in (127.0.0.1/24, 192.168.1.1/24)').exec(dns_response('qq.com', '127.0.0.1', '172.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+
+    def test_all_ip_in(self):
+        response = after_parser.parse('block if all ip in 127.0.0.1/24').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+        response = after_parser.parse('block if all ip in (127.0.0.1/24, 172.0.0.2/24)').exec(dns_response('qq.com', '127.0.0.1', '172.0.0.1'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+
+    def test_all_ip_not_in(self):
+        response = after_parser.parse('block if all ip not in 192.168.1.1/24').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+        response = after_parser.parse('block if all ip not in (192.168.1.1/24, 192.168.253.1/24)').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+
+    def test_geoip_is(self):
+        response = after_parser.parse('block if any geoip is cn').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+        response = after_parser.parse('block if all geoip is cn').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+
+    def test_geoip_is_not(self):
+        response = after_parser.parse('block if any geoip is not cn').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('en'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+        response = after_parser.parse('block if all geoip is not cn').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2'), geoip('en'), ipaddr, run)
+        self.assertEqual(response.header.rcode, dnslib.RCODE.NXDOMAIN)
+
+    def test_first_last(self):
+        response = after_parser.parse('remove record where first or last').exec(dns_response('qq.com', '127.0.0.1', '127.0.0.2', '127.0.0.3'), geoip('cn'), ipaddr, run)
+        self.assertEqual(response.header.a, 1)
+        self.assertEqual(str(response.rr[0].rdata), '127.0.0.2')
```

