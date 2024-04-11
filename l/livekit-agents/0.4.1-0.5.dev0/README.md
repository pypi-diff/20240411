# Comparing `tmp/livekit-agents-0.4.1.tar.gz` & `tmp/livekit-agents-0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-agents-0.4.1.tar", last modified: Sat Apr  6 03:24:48 2024, max compression
+gzip compressed data, was "livekit-agents-0.5.dev0.tar", last modified: Thu Apr 11 21:51:27 2024, max compression
```

## Comparing `livekit-agents-0.4.1.tar` & `livekit-agents-0.5.dev0.tar`

### file list

```diff
@@ -1,36 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.691515 livekit-agents-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-06 03:24:48.691515 livekit-agents-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.687515 livekit-agents-0.4.1/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.687515 livekit-agents-0.4.1/livekit/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.687515 livekit-agents-0.4.1/livekit/agents/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/codecs/mp3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/job_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    11178 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/job_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.687515 livekit-agents-0.4.1/livekit/agents/stt/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/stt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/stt/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/stt/stt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.691515 livekit-agents-0.4.1/livekit/agents/tokenize/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/tokenize/sentence_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.691515 livekit-agents-0.4.1/livekit/agents/tts/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/tts/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/tts/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/vad.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16635 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.691515 livekit-agents-0.4.1/livekit_agents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-06 03:24:48.000000 livekit-agents-0.4.1/livekit_agents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-06 03:24:48.000000 livekit-agents-0.4.1/livekit_agents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 03:24:48.000000 livekit-agents-0.4.1/livekit_agents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-06 03:24:48.000000 livekit-agents-0.4.1/livekit_agents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 03:24:48.000000 livekit-agents-0.4.1/livekit_agents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 03:24:48.691515 livekit-agents-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.391691 livekit-agents-0.5.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.399691 livekit-agents-0.5.dev0/livekit/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.399691 livekit-agents-0.5.dev0/livekit/agents/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/wait_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/apipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.399691 livekit-agents-0.5.dev0/livekit/agents/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/cli/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/cli/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/cli/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.399691 livekit-agents-0.5.dev0/livekit/agents/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/codecs/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/http_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.399691 livekit-agents-0.5.dev0/livekit/agents/ipc/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/ipc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/ipc/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/ipc/job_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/ipc/job_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/ipc/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/ipc_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/job_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/job_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/livekit/agents/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/llm/function_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/llm/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/livekit/agents/stt/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/stt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/stt/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/stt/stt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/livekit/agents/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/tokenize/sentence_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/livekit/agents/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/tts/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/tts/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/voice_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15451 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/livekit_agents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-11 21:51:27.000000 livekit-agents-0.5.dev0/livekit_agents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-11 21:51:27.000000 livekit-agents-0.5.dev0/livekit_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:51:27.000000 livekit-agents-0.5.dev0/livekit_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-11 21:51:27.000000 livekit-agents-0.5.dev0/livekit_agents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 21:51:27.000000 livekit-agents-0.5.dev0/livekit_agents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/setup.py
```

### Comparing `livekit-agents-0.4.1/PKG-INFO` & `livekit-agents-0.5.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.4.1
+Version: 0.5.dev0
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
@@ -16,17 +16,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: click~=8.1.0
-Requires-Dist: livekit>=0.9.0
-Requires-Dist: livekit-api>=0.4.1
-Requires-Dist: livekit-protocol~=0.3.0
-Requires-Dist: websockets<13,>=12
+Requires-Dist: livekit~=0.9
+Requires-Dist: livekit-api~=0.4
+Requires-Dist: livekit-protocol~=0.4
+Requires-Dist: protobuf>=3
+Requires-Dist: types-protobuf<5,>=4
+Requires-Dist: python-json-logger~=2.0
+Requires-Dist: attrs~=23.0
+Requires-Dist: watchfiles~=0.21
+Requires-Dist: colorlog~=6.0
 Provides-Extra: codecs
-Requires-Dist: pyav>=12.0.2; extra == "codecs"
+Requires-Dist: av>=11.0.0; extra == "codecs"
 
 # LiveKit Agents
 
 The core LiveKit Agents Framework. See top-level README for more information.
```

### Comparing `livekit-agents-0.4.1/livekit/agents/__init__.py` & `livekit-agents-0.5.dev0/livekit/agents/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,46 +8,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .version import __version__
-
-from .worker import (
-    Worker,
-    JobCancelledError,
-    AssignmentTimeoutError,
-    JobType,
-    run_app,
-)
-from .plugin import Plugin
-from .utils import AudioBuffer, merge_frames, AsyncIterableQueue
-from .job_request import AutoSubscribe, AutoDisconnect, JobRequest
+from . import aio, codecs, ipc, llm, stt, tokenize, tts, utils, vad
+from .apipe import AsyncPipe  # noqa
+from .ipc.protocol import IPC_MESSAGES, Log, StartJobRequest, StartJobResponse  # noqa
 from .job_context import JobContext
-
-from . import stt
-from . import vad
-from . import tts
-from . import tokenize
+from .job_request import AutoDisconnect, AutoSubscribe, JobRequest
+from .plugin import Plugin
+from .version import __version__
+from .voice_assistant import VoiceAssistant
+from .worker import Worker, WorkerOptions
 
 __all__ = [
     "__version__",
+    "VoiceAssistant",
     "Worker",
+    "WorkerOptions",
     "JobRequest",
     "AutoSubscribe",
     "AutoDisconnect",
     "JobContext",
-    "JobCancelledError",
-    "AssignmentTimeoutError",
     "Plugin",
-    "run_app",
-    "JobType",
-    "AudioBuffer",
-    "merge_frames",
-    "AsyncIterableQueue",
+    "ipc",
+    "codecs",
     "stt",
     "vad",
+    "utils",
     "tts",
+    "aio",
     "tokenize",
+    "llm",
 ]
```

### Comparing `livekit-agents-0.4.1/livekit/agents/codecs/__init__.py` & `livekit-agents-0.5.dev0/livekit/agents/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.4.1/livekit/agents/codecs/mp3.py` & `livekit-agents-0.5.dev0/livekit/agents/codecs/mp3.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,82 +8,62 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import asyncio
 import ctypes
 import logging
 from importlib import import_module
+from typing import List
+
+from livekit import rtc
 
 
 class Mp3StreamDecoder:
     """A class that can be used to stream arbitrary MP3 data (i.e. from an HTTP chunk) and decode it into PCM audio.
     This class is meant to be ephemeral. When you're done sending data, call close() to flush
     the decoder and create a new instance of this class if you need to decode more data.
     """
 
     def __init__(self):
         try:
             globals()["av"] = import_module("av")
         except ImportError:
             raise ImportError(
-                "You haven't included the decoder_utils optional dependencies. Please install the decoder_utils extra by running `pip install livekit-agents[decoder_utils]`"
+                "You haven't included the 'codecs' optional dependencies. Please install the 'codecs' extra by running `pip install livekit-agents[codecs]`"
             )
-        self._closed = False
-        self._input_queue = asyncio.Queue()
-        self._output_queue = asyncio.Queue()
-        self._codec = av.CodecContext.create("mp3", "r")  # noqa
-        self._run_task = asyncio.create_task(self._run())
 
-    def close(self):
-        self._closed = True
-        self._input_queue.put_nowait(None)
-
-    def push_chunk(self, chunk: bytes):
-        if self._closed:
-            raise ValueError("Cannot push chunk to closed decoder")
-        self._input_queue.put_nowait(chunk)
-
-    async def _run(self):
-        while True:
-            input = await self._input_queue.get()
-            if input is None:
-                self._output_queue.put_nowait(None)
-                break
-
-            result = await asyncio.to_thread(self._decode_input, input)
-            # If error decoding, skip it
-            if result is None:
-                continue
-            self._output_queue.put_nowait(result)
+        self._codec = av.CodecContext.create("mp3", "r")  # noqa
 
-    def _decode_input(self, input: bytes):
-        packets = self._codec.parse(input)
-        result = b""
+    def decode_chunk(self, chunk: bytes) -> List[rtc.AudioFrame]:
+        packets = self._codec.parse(chunk)
+        result: List[rtc.AudioFrame] = []
         for packet in packets:
             try:
                 decoded = self._codec.decode(packet)
-                for frame in decoded:
-                    plane = frame.planes[0]
-                    ptr = plane.buffer_ptr
-                    size = plane.buffer_size
-                    byte_array_pointer = ctypes.cast(
-                        ptr, ctypes.POINTER(ctypes.c_char * size)
-                    )
-                    result += bytes(byte_array_pointer.contents)
             except Exception as e:
-                logging.error(f"Error decoding chunk: {e}")
+                logging.warning(f"Error decoding packet, skipping: {e}")
                 continue
-
+            for frame in decoded:
+                nchannels = len(frame.layout.channels)
+                if frame.format.is_planar and nchannels > 1:
+                    logging.warning(
+                        "TODO: planar audio has not yet been considered, skipping frame"
+                    )
+                    continue
+                plane = frame.planes[0]
+                ptr = plane.buffer_ptr
+                size = plane.buffer_size
+                byte_array_pointer = ctypes.cast(
+                    ptr, ctypes.POINTER(ctypes.c_char * size)
+                )
+                result.append(
+                    rtc.AudioFrame(
+                        data=bytes(byte_array_pointer.contents),
+                        num_channels=nchannels,
+                        sample_rate=frame.sample_rate,
+                        samples_per_channel=frame.samples,
+                    )
+                )
         return result
-
-    def __aiter__(self):
-        return self
-
-    async def __anext__(self):
-        packet = await self._output_queue.get()
-        if packet is None:
-            raise StopAsyncIteration
-        return packet
```

### Comparing `livekit-agents-0.4.1/livekit/agents/plugin.py` & `livekit-agents-0.5.dev0/livekit/agents/plugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from abc import ABC, abstractmethod
 from typing import List
 
 
 class Plugin(ABC):
     registered_plugins: List["Plugin"] = []
 
-    def __init__(self, title: str, version: str) -> None:
+    def __init__(self, title: str, version: str, package: str) -> None:
         self._title = title
         self._version = version
+        self._package = package
 
     @classmethod
     def register_plugin(cls, plugin: "Plugin") -> None:
         cls.registered_plugins.append(plugin)
 
     @abstractmethod
     def download_files(self) -> None:
-        """
-        Blocking is allowed inside this method
-        This is the perfect place to download models for e.g
-        """
         pass
 
     @property
+    def package(self) -> str:
+        return self._package
+
+    @property
     def title(self) -> str:
         return self._title
 
     @property
     def version(self) -> str:
         return self._version
```

### Comparing `livekit-agents-0.4.1/livekit/agents/tokenize/sentence_tokenizer.py` & `livekit-agents-0.5.dev0/livekit/agents/tokenize/sentence_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import List
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Optional
+from typing import List, Optional
 
 
 @dataclass
 class SegmentedSentence:
     text: str
```

### Comparing `livekit-agents-0.4.1/livekit/agents/tts/stream_adapter.py` & `livekit-agents-0.5.dev0/livekit/agents/tts/stream_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
-import logging
 from typing import AsyncIterable
 
+from ..log import logger
 from ..tokenize import SentenceStream, SentenceTokenizer
 from .tts import (
     TTS,
     SynthesisEvent,
     SynthesisEventType,
     SynthesizedAudio,
     SynthesizeStream,
@@ -21,26 +21,32 @@
         self._queue = asyncio.Queue[str]()
         self._event_queue = asyncio.Queue[SynthesisEvent]()
 
         self._main_task = asyncio.create_task(self._run())
 
         def log_exception(task: asyncio.Task) -> None:
             if not task.cancelled() and task.exception():
-                logging.error(f"speech task failed: {task.exception()}")
+                logger.error(f"speech task failed: {task.exception()}")
 
         self._main_task.add_done_callback(log_exception)
 
     async def _run(self) -> None:
         while True:
             try:
                 sentence = await self._sentence_stream.__anext__()
                 audio = await self._tts.synthesize(text=sentence.text)
                 self._event_queue.put_nowait(
+                    SynthesisEvent(type=SynthesisEventType.STARTED)
+                )
+                self._event_queue.put_nowait(
                     SynthesisEvent(type=SynthesisEventType.AUDIO, audio=audio)
                 )
+                self._event_queue.put_nowait(
+                    SynthesisEvent(type=SynthesisEventType.FINISHED)
+                )
             except asyncio.CancelledError:
                 break
 
         self._closed = True
 
     def push_text(self, token: str) -> None:
         self._sentence_stream.push_text(token)
@@ -50,20 +56,23 @@
 
     async def aclose(self) -> None:
         self._main_task.cancel()
         try:
             await self._main_task
         except asyncio.CancelledError:
             pass
+        finally:
+            self._event_queue.put_nowait(None)
 
     async def __anext__(self) -> SynthesisEvent:
-        if self._closed and self._event_queue.empty():
+        item = await self._event_queue.get()
+        if item is None:
             raise StopAsyncIteration
 
-        return await self._event_queue.get()
+        return item
 
 
 class StreamAdapter(TTS):
     def __init__(self, tts: TTS, tokenizer: SentenceTokenizer) -> None:
         super().__init__(streaming_supported=True)
         self._tts = tts
         self._tokenizer = tokenizer
```

### Comparing `livekit-agents-0.4.1/livekit/agents/tts/tts.py` & `livekit-agents-0.5.dev0/livekit/agents/tts/tts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
-from typing import AsyncIterable, Optional
+from typing import AsyncIterable
 
 from livekit import rtc
 
 
 @dataclass
 class SynthesizedAudio:
     text: str
@@ -14,36 +16,48 @@
 
 class SynthesisEventType(Enum):
     # first event, indicates that the stream has started
     # retriggered after FINISHED
     STARTED = 0
     # audio data is available
     AUDIO = 1
-    # generally happens after a flushing the stream
-    # some TTS providers close the stream so we know it's done
+    # finished synthesizing an audio segment (generally separated by sending "None" to push_text)
+    # this doesn't means the stream is done, more text can be pushed
     FINISHED = 2
 
 
 @dataclass
 class SynthesisEvent:
     type: SynthesisEventType
-    audio: Optional[SynthesizedAudio] = None
+    audio: SynthesizedAudio | None = None
 
 
 class SynthesizeStream(ABC):
     @abstractmethod
-    def push_text(self, token: str) -> None:
+    def push_text(self, token: str | None) -> None:
+        """
+        Push some text to be synthesized. If token is None,
+        it will be used to identify the end of this particular segment.
+        (required by some TTS engines)
+        """
         pass
 
-    @abstractmethod
-    async def flush(self) -> None:
-        pass
+    def mark_segment_end(self) -> None:
+        """
+        Mark the end of the current segment, this is equivalent to calling
+        push_text(None)
+        """
+        self.push_text(None)
 
     @abstractmethod
-    async def aclose(self) -> None:
+    async def aclose(self, wait: bool = True) -> None:
+        """
+        Close the stream, if wait is True, it will wait for the TTS to
+        finish synthesizing the audio, otherwise it will close ths stream immediately
+        """
         pass
 
     @abstractmethod
     async def __anext__(self) -> SynthesisEvent:
         pass
 
     def __aiter__(self) -> "SynthesizeStream":
@@ -51,16 +65,16 @@
 
 
 class TTS(ABC):
     def __init__(self, *, streaming_supported: bool) -> None:
         self._streaming_supported = streaming_supported
 
     @abstractmethod
-    def synthesize(self, *, text: str) -> AsyncIterable[SynthesizedAudio]:
-        pass
+    def synthesize(self, text: str) -> AsyncIterable[SynthesizedAudio]:
+        raise NotImplementedError("synthesize is not implemented")
 
     def stream(self) -> SynthesizeStream:
         raise NotImplementedError(
             "streaming is not supported by this TTS, please use a different TTS or use a StreamAdapter"
         )
 
     @property
```

### Comparing `livekit-agents-0.4.1/livekit/agents/vad.py` & `livekit-agents-0.5.dev0/livekit/agents/vad.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from abc import ABC, abstractmethod
-from typing import List
 from dataclasses import dataclass, field
-from livekit import rtc
 from enum import Enum
+from typing import List
+
+from livekit import rtc
 
 
 class VADEventType(Enum):
-    START_SPEAKING = 1
+    START_OF_SPEECH = 1
     SPEAKING = 2
-    END_SPEAKING = 3
+    END_OF_SPEECH = 3
 
 
 @dataclass
 class VADEvent:
-    # type of the event
     type: VADEventType
-    # index of the samples of the event (when the event was fired)
+    """type of the event"""
     samples_index: int
-    # duration of the speech in seconds (only for END_SPEAKING event)
+    """index of the samples of the event (when the event was fired)"""
     duration: float = 0.0
-    # list of audio frames of the speech
+    """duration of the speech in seconds (only for END_SPEAKING event)"""
     speech: List[rtc.AudioFrame] = field(default_factory=list)
+    """list of audio frames of the speech"""
 
 
 class VAD(ABC):
     def __init__(self) -> None:
         pass
 
     @abstractmethod
@@ -58,19 +59,15 @@
         pass
 
     @abstractmethod
     def push_frame(self, frame: rtc.AudioFrame) -> None:
         pass
 
     @abstractmethod
-    async def flush(self) -> None:
-        pass
-
-    @abstractmethod
-    async def aclose(self) -> None:
+    async def aclose(self, *, wait: bool = True) -> None:
         pass
 
     @abstractmethod
     async def __anext__(self) -> VADEvent:
         raise StopAsyncIteration
 
     def __aiter__(self) -> "VADStream":
```

### Comparing `livekit-agents-0.4.1/livekit/agents/version.py` & `livekit-agents-0.5.dev0/livekit/agents/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.4.1"
+__version__ = "0.5.dev0"
```

### Comparing `livekit-agents-0.4.1/livekit/agents/worker.py` & `livekit-agents-0.5.dev0/livekit/agents/worker.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,484 +8,435 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from __future__ import annotations
+
 import asyncio
-import logging
+import contextlib
 import os
-import signal
-import uuid
 from typing import (
-    Any,
     Callable,
     Coroutine,
-    Dict,
-    Optional,
-    Tuple,
 )
 from urllib.parse import urlparse
 
-import websockets
+import aiohttp
+import psutil
+from attr import define
+from livekit import api
+from livekit.protocol import agent, models
+
+from . import aio, consts, http_server, ipc
+from .job_request import AcceptData, AvailRes, JobRequest
+from .log import logger
+from .version import __version__
+
+JobRequestFnc = Callable[[JobRequest], Coroutine]
+LoadFnc = Callable[[], float]
+
+
+def cpu_load_fnc() -> float:
+    [m1, m5, m15] = [x / psutil.cpu_count() for x in psutil.getloadavg()]
+    return m1
+
+
+@define(kw_only=True)
+class WorkerPermissions:
+    can_publish: bool = True
+    can_subscribe: bool = True
+    can_publish_data: bool = True
+    can_update_metadata: bool = True
+    hidden: bool = False
+
+
+# NOTE: this object must be pickle-able
+@define(kw_only=True)
+class WorkerOptions:
+    request_fnc: JobRequestFnc
+    load_fnc: LoadFnc = cpu_load_fnc
+    load_threshold: float = 0.8
+    namespace: str = "default"
+    permissions: WorkerPermissions = WorkerPermissions()
+    worker_type: agent.JobType = agent.JobType.JT_ROOM
+    max_retry: int = consts.MAX_RECONNECT_ATTEMPTS
+    ws_url: str = "ws://localhost:7880"
+    api_key: str | None = None
+    api_secret: str | None = None
+    host: str = "localhost"
+    port: int = 8081
+
+
+@define(kw_only=True)
+class ActiveJob:
+    job: agent.Job
+    accept_data: AcceptData
 
-from livekit import api, protocol
-from livekit.protocol import agent as proto_agent
-from livekit.protocol import models as proto_models
-from livekit.protocol.agent import JobType
-from .job_request import JobRequest
-from .job_context import JobContext
-from .plugin import Plugin
 
-MAX_RECONNECT_ATTEMPTS = 10
-RECONNECT_INTERVAL = 5
-ASSIGNMENT_TIMEOUT = 15
+class Worker:
+    def __init__(
+        self,
+        opts: WorkerOptions,
+        *,
+        loop: asyncio.AbstractEventLoop | None = None,
+    ) -> None:
+        opts.ws_url = opts.ws_url or opts.ws_url or os.environ.get("LIVEKIT_URL") or ""
+        opts.api_key = opts.api_key or os.environ.get("LIVEKIT_API_KEY") or ""
+        opts.api_secret = opts.api_secret or os.environ.get("LIVEKIT_API_SECRET") or ""
+
+        self._opts = opts
+        self._loop = loop or asyncio.get_event_loop()
+        self._id = "unregistered"
+        self._session = None
+        self._closed = False
+        self._tasks = set()
+        self._pending_assignments: dict[str, asyncio.Future[agent.JobAssignment]] = {}
+        self._processes = dict[str, tuple[ipc.JobProcess, ActiveJob]]()
+        self._close_future = asyncio.Future(loop=self._loop)
+
+        self._chan = aio.Chan[agent.WorkerMessage](32, loop=self._loop)
+        # We use the same event loop as the worker (so the health checks are more accurate)
+        self._http_server = http_server.HttpServer(
+            opts.host, opts.port, loop=self._loop
+        )
 
-JobRequestHandler = Callable[["JobRequest"], Coroutine]
+    async def run(self):
+        logger.info("starting worker", extra={"version": __version__})
 
+        if not self._opts.ws_url:
+            raise ValueError("ws_url is required, or set LIVEKIT_URL env var")
 
-class AssignmentTimeoutError(Exception):
-    """Worker timed out when joining the worker-pool"""
+        if not self._opts.api_key:
+            raise ValueError("api_key is required, or set LIVEKIT_API_KEY env var")
 
-    def __init__(self, message: str) -> None:
-        super().__init__(message)
+        if not self._opts.api_secret:
+            raise ValueError(
+                "api_secret is required, or set LIVEKIT_API_SECRET env var"
+            )
 
+        self._session = aiohttp.ClientSession()
 
-class JobCancelledError(Exception):
-    """Job was cancelled by the server"""
+        async def _worker_ws():
+            assert self._session is not None
 
-    def __init__(self, message: str) -> None:
-        super().__init__(message)
+            retry_count = 0
+            while not self._closed:
+                try:
+                    join_jwt = (
+                        api.AccessToken(self._opts.api_key, self._opts.api_secret)
+                        .with_grants(api.VideoGrants(agent=True))
+                        .to_jwt()
+                    )
 
+                    headers = {"Authorization": f"Bearer {join_jwt}"}
 
-class Worker:
-    """A Worker is a client that connects to LiveKit Cloud (or a LiveKit server) and receives Agent jobs.
-    For Job the Worker accepts, it will connect to the room and handle track subscriptions.
-    """
+                    parse = urlparse(self._opts.ws_url)
+                    scheme = parse.scheme
+                    if scheme.startswith("http"):
+                        scheme = scheme.replace("http", "ws")
+                    agent_url = (
+                        f"{scheme}://{parse.netloc}/{parse.path.rstrip('/')}/agent"
+                    )
 
-    def __init__(
-        self,
-        request_handler: JobRequestHandler,
-        *,
-        worker_type: JobType.ValueType = JobType.JT_ROOM,
-        event_loop: Optional[asyncio.AbstractEventLoop] = None,
-        ws_url: Optional[str] = None,
-        api_key: Optional[str] = None,
-        api_secret: Optional[str] = None,
-    ) -> None:
-        """
-        Args:
-            request_handler (JobRequestHandler): Callback that is triggered when a new Job is available.
-            worker_type (JobType): What kind of jobs this worker can handle.
-            event_loop (Optional[asyncio.AbstractEventLoop]): Optional asyncio event loop to use for this worker. Defaults to None.
-            ws_url (str, optional): LiveKit websocket URL. Defaults to os.environ.get("LIVEKIT_URL", "http://localhost:7880").
-            api_key (str, optional): LiveKit API Key. Defaults to os.environ.get("LIVEKIT_API_KEY", "").
-            api_secret (str, optional): LiveKit API Secret. Defaults to os.environ.get("LIVEKIT_API_SECRET", "").
-        """
-
-        self._loop = event_loop or asyncio.get_event_loop()
-        self._lock = asyncio.Lock()
-        self._request_handler = request_handler
-        self._wid = "W-" + str(uuid.uuid4())[:12]
-        self._worker_type = worker_type
-        self._api_key = api_key or os.environ.get("LIVEKIT_API_KEY")
-        self._api_secret = api_secret or os.environ.get("LIVEKIT_API_SECRET")
-        self._api = None
-        self._running = False
-        self._running_jobs: list["JobContext"] = []
-        self._pending_jobs: Dict[str, asyncio.Future[proto_agent.JobAssignment]] = {}
-        self._rtc_url = None
-        self._agent_url = None
-        ws_url = ws_url or os.environ.get("LIVEKIT_URL")
-        if ws_url:
-            self._set_url(ws_url)
-
-    def _set_url(self, ws_url: str) -> None:
-        parse_res = urlparse(ws_url)
-        scheme = parse_res.scheme
-        if scheme.startswith("http"):
-            scheme = scheme.replace("http", "ws")
-
-        url = f"{scheme}://{parse_res.netloc}/{parse_res.path}"
-        url = url.rstrip("/")
-
-        self._agent_url = url + "/agent"
-        self._rtc_url = url
-
-    async def _connect(self) -> protocol.agent.RegisterWorkerResponse:
-        if not self._rtc_url:
-            raise ValueError("No WebSocket URL provided, set LIVEKIT_URL env var")
-
-        if not self._api_key:
-            raise ValueError("No API key provided, set LIVEKIT_API_KEY env var")
-
-        if not self._api_secret:
-            raise ValueError("No API secret provided, set LIVEKIT_API_SECRET env var")
-
-        self._api = api.LiveKitAPI(self._rtc_url, self._api_key, self._api_secret)
-
-        join_jwt = (
-            api.AccessToken(self._api_key, self._api_secret)
-            .with_grants(api.VideoGrants(agent=True))
-            .to_jwt()
-        )
+                    ws = await self._session.ws_connect(agent_url, headers=headers)
+                    retry_count = 0
 
-        req = protocol.agent.WorkerMessage()
-        req.register.worker_id = self._wid
-        req.register.type = self._worker_type
-
-        headers = {"Authorization": f"Bearer {join_jwt}"}
-        self._ws = await websockets.connect(
-            self._agent_url, extra_headers=headers, close_timeout=0.150
-        )
-        await self._send(req)
-        res = await self._recv()
-        return res.register
-
-    async def _send_availability(
-        self, job_id: str, available: bool
-    ) -> protocol.agent.JobAssignment:
-        """Send availability to the server, and wait for assignment"""
-        req = protocol.agent.WorkerMessage()
-        req.availability.available = available
-        req.availability.job_id = job_id
-
-        f = asyncio.Future()
-        self._pending_jobs[job_id] = f
-        await self._send(req)
-
-        try:
-            return await asyncio.wait_for(f, ASSIGNMENT_TIMEOUT)
-        except asyncio.TimeoutError as exc:
-            raise AssignmentTimeoutError(
-                f"assignment timeout for job {job_id}"
-            ) from exc
+                    await self._run_ws(ws)
+                except Exception as e:
+                    if self._closed:
+                        break
 
-    async def _send_job_status(
-        self,
-        job_id: str,
-        status: protocol.agent.JobStatus.ValueType,
-        error: str,
-        user_data: str = "",
-    ) -> None:
-        req = protocol.agent.WorkerMessage()
-        req.job_update.job_id = job_id
-        req.job_update.status = status
-        req.job_update.error = error
-        req.job_update.user_data = user_data
-        await self._ws.send(req.SerializeToString())
+                    if retry_count >= self._opts.max_retry:
+                        raise Exception(
+                            f"failed to connect to livekit-server after {retry_count} attempts: {e}"
+                        )
 
-    def _simulate_job(
-        self,
-        room: proto_models.Room,
-        participant: Optional[proto_models.ParticipantInfo],
-    ):
-        # TODO(theomonnom): the server could handle the JobSimulation like
-        # we're doing with the SFU today
-        job_id = "JR_" + str(uuid.uuid4())[:12]
-        job_type = JobType.JT_ROOM if participant is None else JobType.JT_PUBLISHER
-        job = proto_agent.Job(
-            id=job_id, type=job_type, room=room, participant=participant
-        )
-        job = JobRequest(self, job, simulated=True)
-        asyncio.ensure_future(self._handle_new_job(job), loop=self._loop)
+                    retry_delay = min(retry_count * 2, 10)
+                    retry_count += 1
+
+                    logger.warning(
+                        f"failed to connect to livekit-server, retrying in {retry_delay}s: {e}",
+                    )
+                    await asyncio.sleep(retry_delay)
+
+        async def _http_server():
+            await self._http_server.run()
 
-    async def _recv(self) -> proto_agent.ServerMessage:
-        message = await self._ws.recv()
-        msg = protocol.agent.ServerMessage()
-        msg.ParseFromString(bytes(message))  # type: ignore
-        return msg
-
-    async def _send(self, msg: protocol.agent.WorkerMessage) -> None:
-        try:
-            await self._ws.send(msg.SerializeToString())
-        except websockets.exceptions.ConnectionClosed:
-            # TODO: Implement JobStatus resuming after reconnection
-            pass
-
-    async def _handle_new_job(self, job: "JobRequest") -> None:
-        """Execute the available callback, and automatically deny the job if the callback
-        does not send an answer or raises an exception"""
-
-        try:
-            await self._request_handler(job)
-        except Exception:
-            logging.exception("request handler for job %s failed", job.id)
+        await asyncio.gather(_worker_ws(), _http_server())
+        self._close_future.set_result(None)
+
+    @property
+    def id(self) -> str:
+        return self._id
+
+    @property
+    def active_jobs(self) -> list[ActiveJob]:
+        return [active_job for (_, active_job) in self._processes.values()]
+
+    async def aclose(self) -> None:
+        if self._closed:
             return
 
-        if not job._answered:
-            logging.warning(
-                "user did not answer availability for job %s, rejecting", job.id
-            )
-            await job.reject()
+        logger.info("shutting down worker", extra={"id": self.id})
 
-    async def _message_received(self, msg: protocol.agent.ServerMessage) -> None:
-        logging.debug("received message: %s", msg)
-        which = msg.WhichOneof("message")
-        if which == "availability":
-            # server is asking the worker if we are available for a job
-            availability = msg.availability
-            job = JobRequest(self, availability.job)
-            asyncio.ensure_future(self._handle_new_job(job), loop=self._loop)
-        elif which == "assignment":
-            # server is assigning a job to the worker
-            assignment = msg.assignment
-            job_id = assignment.job.id
-            f = self._pending_jobs.get(job_id)
-            if f is None:
-                logging.error("received assignment for unknown job %s", job_id)
-                return
+        # shutdown processes before closing the connection to the lkserver
+        close_co = []
+        for proc, _ in self._processes.values():
+            close_co.append(proc.aclose())
+
+        await asyncio.gather(*close_co, return_exceptions=True)
+
+        await self._http_server.aclose()
+        assert self._session is not None
+        await self._session.close()
+
+        self._closed = True
+        self._chan.close()
+        await self._close_future
+
+    async def _run_ws(self, ws: aiohttp.ClientWebSocketResponse):
+        closing_ws = False
+
+        # register the worker
+        req = agent.WorkerMessage()
+        req.register.type = self._opts.worker_type
+        req.register.allowed_permissions.CopyFrom(
+            models.ParticipantPermission(
+                can_publish=self._opts.permissions.can_publish,
+                can_subscribe=self._opts.permissions.can_subscribe,
+                can_publish_data=self._opts.permissions.can_publish_data,
+                can_update_metadata=self._opts.permissions.can_update_metadata,
+                hidden=self._opts.permissions.hidden,
+                agent=True,
+            )
+        )
+        req.register.namespace = self._opts.namespace
+        req.register.version = __version__
+        await self._chan.send(req)
+
+        async def load_monitor_task():
+            interval = aio.interval(consts.LOAD_INTERVAL)
+            registered = True
+            while True:
+                await interval.tick()
+                load = self._opts.load_fnc()
+                is_full = load >= self._opts.load_threshold
+                should_register = not is_full
+
+                update = agent.UpdateWorkerStatus(
+                    load=load,
+                    status=(
+                        agent.WorkerStatus.WS_FULL
+                        if is_full
+                        else agent.WorkerStatus.WS_AVAILABLE
+                    ),
+                )
 
-            f.set_result(assignment)
-            del self._pending_jobs[job_id]
+                if should_register != registered:
+                    registered = should_register
 
-    async def _reconnect(self) -> bool:
-        for i in range(MAX_RECONNECT_ATTEMPTS):
-            try:
-                reg = await self._connect()
-                logging.info("worker successfully re-registered: %s", reg.worker_id)
-                return True
-            except Exception as e:
-                logging.error("failed to reconnect, attempt %i: %s", i, e)
-                await asyncio.sleep(RECONNECT_INTERVAL)
+                    extra = {"load": load, "threshold": self._opts.load_threshold}
+                    if is_full:
+                        logger.info(
+                            "worker is at full capacity, marking as unavailable",
+                            extra=extra,
+                        )
+                    else:
+                        logger.info(
+                            "worker is below capacity, marking as available",
+                            extra=extra,
+                        )
 
-        return False
+                msg = agent.WorkerMessage(update_worker=update)
+                try:
+                    self._chan.send_nowait(msg)
+                except aio.ChanClosed:
+                    return
 
-    async def _run(self) -> None:
-        try:
+        async def send_task():
+            nonlocal closing_ws
             while True:
                 try:
-                    while True:
-                        await self._message_received(await self._recv())
-                except websockets.exceptions.ConnectionClosed as e:
-                    if self._running:
-                        logging.error("connection closed, trying to reconnect: %s", e)
-                        if not await self._reconnect():
-                            break
-                except Exception as e:
-                    logging.error("error while running worker: %s", e)
-                    break
-        finally:
-            await asyncio.shield(self._shutdown())
-
-    async def _shutdown(self) -> None:
-        async with self._lock:
-            if not self._running:
-                return
+                    msg = await self._chan.recv()
+                    await ws.send_bytes(msg.SerializeToString())
+                except aio.ChanClosed:
+                    closing_ws = True
+                    return
 
-            await self._ws.close()
-            # Close all running jobs
-            await asyncio.gather(*[job.disconnect() for job in self._running_jobs])
-            self._running = False
-
-    async def start(self) -> None:
-        """Start the Worker"""
-
-        async with self._lock:
-            if self._running:
-                raise Exception("worker is already running")
-
-            await self._connect()  # initial connection
-            self._running = True
-            self._task = self._loop.create_task(self._run())
-
-    async def shutdown(self) -> None:
-        """Shut the Worker down."""
-        async with self._lock:
-            if not self._running:
-                return
+        async def recv_task():
+            nonlocal closing_ws
+            while True:
+                msg = await ws.receive()
+                if msg.type in (
+                    aiohttp.WSMsgType.CLOSE,
+                    aiohttp.WSMsgType.CLOSED,
+                    aiohttp.WSMsgType.CLOSING,
+                ):
+                    if closing_ws:
+                        return
+
+                    raise Exception("worker connection closed unexpectedly")
+
+                if msg.type != aiohttp.WSMsgType.BINARY:
+                    logger.warning("unexpected message type: %s", msg.type)
+                    continue
+
+                data = msg.data
+                msg = agent.ServerMessage()
+                msg.ParseFromString(data)
+                which = msg.WhichOneof("message")
+                if which == "register":
+                    self._handle_register(
+                        msg.register
+                    )  # we assume this is the first message we receive
+                elif which == "availability":
+                    self._handle_availability(msg.availability)
+                elif which == "assignment":
+                    self._handle_assignment(msg.assignment)
+
+        await asyncio.gather(send_task(), recv_task(), load_monitor_task())
+
+    def _reload_jobs(self, jobs: list[ActiveJob]):
+        for aj in jobs:
+            logger.info("reloading job", extra={"job": aj.job})
+            # reloading jobs doesn't work on third-party workers
+            # so it is ok to use the ws_url from the local worker
+            # (also create a token with the worker api key)
+            url = self._opts.ws_url
+
+            jwt = (
+                api.AccessToken(self._opts.api_key, self._opts.api_secret)
+                .with_grants(
+                    api.VideoGrants(agent=True, room=aj.job.room.name, room_join=True)
+                )
+                .with_name(aj.accept_data.name)
+                .with_metadata(aj.accept_data.metadata)
+                .with_identity(aj.accept_data.identity)
+                .to_jwt()
+            )
 
-            self._task.cancel()
-            await self._task
+            self._start_process(aj.job, url, jwt, aj.accept_data)
 
-    @property
-    def id(self) -> str:
-        """Worker ID"""
-        return self._wid
+    def _start_process(
+        self, job: agent.Job, url: str, token: str, accept_data: AcceptData
+    ):
+        proc = ipc.JobProcess(job, url, token, accept_data)
+        self._processes[job.id] = (proc, ActiveJob(job=job, accept_data=accept_data))
 
-    @property
-    def running(self) -> bool:
-        """Whether the worker is running.
-        Running is first set to True when the websocket connection is established and
-        the Worker has been acknowledged by a LiveKit Server."""
-        return self._running
+        async def _run_proc():
+            try:
+                await proc.run()
+            except Exception:
+                logger.exception(
+                    f"error running job process {proc.job.id}",
+                    extra=proc.logging_extra(),
+                )
 
-    @property
-    def api(self) -> Optional[api.LiveKitAPI]:
-        return self._api
+            self._processes.pop(proc.job.id)
 
+        task = self._loop.create_task(_run_proc())
+        self._tasks.add(task)
+        task.add_done_callback(self._tasks.discard)
+
+    def _handle_register(self, reg: agent.RegisterWorkerResponse):
+        self._id = reg.worker_id
+        logger.info(
+            "registered worker",
+            extra={"id": reg.worker_id, "server_info": reg.server_info},
+        )
 
-def _run_worker(
-    worker: Worker,
-    loop: Optional[asyncio.AbstractEventLoop] = None,
-    started_cb: Optional[Callable[[Worker], Any]] = None,
-) -> None:
-    """Run the specified worker and handle graceful shutdown"""
+    def _handle_availability(self, msg: agent.AvailabilityRequest):
+        answer_tx, answer_rx = aio.channel(1)  # wait for the user res
+        req = JobRequest(msg.job, answer_tx)
 
-    loop = loop or asyncio.get_event_loop()
+        async def _wait_response():
+            async def _user_cb():
+                try:
+                    await self._opts.request_fnc(req)
+                except Exception:
+                    logger.exception(
+                        f"user request handler for job {req.id} failed",
+                        extra={"req": req},
+                    )
 
-    class GracefulShutdown(SystemExit):
-        code = 1
+                if not req.answered:
+                    logger.warning(
+                        f"no answer for job {req.id}, automatically rejecting the job",
+                        extra={"req": req},
+                    )
+                    await _send_ignore_err(
+                        self._chan,
+                        agent.WorkerMessage(
+                            availability=agent.AvailabilityResponse(available=False)
+                        ),
+                    )
 
-    for sig in (signal.SIGINT, signal.SIGTERM):
-        try:
+            user_task = self._loop.create_task(_user_cb())
 
-            def _signal_handler():
-                raise GracefulShutdown()
+            av: AvailRes = await answer_rx.recv()  # wait for user answer
+            msg = agent.WorkerMessage()
+            msg.availability.job_id = req.id
+            msg.availability.available = av.avail
 
-            loop.add_signal_handler(sig, _signal_handler)
-        except NotImplementedError:
-            pass
+            if not av.avail:
+                await _send_ignore_err(self._chan, msg)
+                return
 
-    async def _main_task(worker: Worker) -> None:
-        try:
-            await worker.start()
-            if started_cb:
-                started_cb(worker)
+            assert av.data is not None
+            assert av.assignment_tx is not None
+            msg.availability.participant_identity = av.data.identity
+            msg.availability.participant_name = av.data.name
+            msg.availability.participant_metadata = av.data.metadata
 
-            logging.info(
-                "worker started, press Ctrl+C to stop (worker id: %s)", worker.id
-            )
+            wait_assignment = asyncio.Future[agent.JobAssignment]()
+            self._pending_assignments[req.id] = wait_assignment
 
-            await worker._task
-        except asyncio.CancelledError:
-            pass
-        finally:
-            logging.info("shutting down worker %s", worker.id)
-            await worker.shutdown()
-            logging.info("worker %s shutdown", worker.id)
-
-    main_task = loop.create_task(_main_task(worker))
-    try:
-        asyncio.set_event_loop(loop)
-        loop.run_until_complete(main_task)
-    except (GracefulShutdown, KeyboardInterrupt):
-        logging.info("Graceful shutdown worker")
-    finally:
-        main_task.cancel()
-        loop.run_until_complete(main_task)
-
-        tasks = asyncio.all_tasks(loop)
-        for task in tasks:
-            task.cancel()
-
-        loop.run_until_complete(asyncio.gather(*tasks, return_exceptions=True))
-        loop.run_until_complete(loop.shutdown_asyncgens())
-        loop.close()
-        asyncio.set_event_loop(None)
-
-
-def run_app(worker: Worker) -> None:
-    """Run the CLI to interact with the worker"""
-
-    import click
-
-    @click.group()
-    @click.option(
-        "--log-level",
-        default="INFO",
-        type=click.Choice(
-            ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"], case_sensitive=False
-        ),
-        help="Set the logging level",
-    )
-    def cli(log_level: str) -> None:
-        logging.basicConfig(level=log_level)
-
-    @cli.command(help="Start the worker")
-    @click.option(
-        "--url",
-        required=True,
-        envvar="LIVEKIT_URL",
-        help="LiveKit server or Cloud project WebSocket URL",
-        default="ws://localhost:7880",
-    )
-    @click.option(
-        "--api-key",
-        envvar="LIVEKIT_API_KEY",
-        help="LiveKit server or Cloud project's API key",
-        required=True,
-    )
-    @click.option(
-        "--api-secret",
-        envvar="LIVEKIT_API_SECRET",
-        help="LiveKit server or Cloud project's API secret",
-        required=True,
-    )
-    def start(url: str, api_key: str, api_secret: str) -> None:
-        worker._set_url(url)
-        worker._api_key = api_key
-        worker._api_secret = api_secret
-        _run_worker(worker)
-
-    @cli.command(help="Start a worker and simulate a job, useful for testing")
-    @click.option("--room-name", help="The room name", required=True)
-    @click.option("--identity", help="The participant identity")
-    @click.option(
-        "--url",
-        required=True,
-        envvar="LIVEKIT_URL",
-        help="LiveKit server or Cloud project WebSocket URL",
-        default="ws://localhost:7880",
-    )
-    @click.option(
-        "--api-key",
-        envvar="LIVEKIT_API_KEY",
-        help="LiveKit server or Cloud project's API key",
-        required=True,
-    )
-    @click.option(
-        "--api-secret",
-        envvar="LIVEKIT_API_SECRET",
-        help="LiveKit server or Cloud project's API secret",
-        required=True,
-    )
-    def simulate_job(
-        room_name: str, identity: str, url: str, api_key: str, api_secret: str
-    ) -> None:
-        worker._set_url(url)
-        worker._api_key = api_key
-        worker._api_secret = api_secret
-
-        async def _pre_run() -> (
-            Tuple[proto_models.Room, Optional[proto_models.ParticipantInfo]]
-        ):
-            lkapi = api.LiveKitAPI(worker._rtc_url, worker._api_key, worker._api_secret)
+            await _send_ignore_err(self._chan, msg)
 
+            # wait for server assignment
             try:
-                room = await lkapi.room.create_room(
-                    api.CreateRoomRequest(name=room_name)
+                await asyncio.wait_for(wait_assignment, consts.ASSIGNMENT_TIMEOUT)
+                await av.assignment_tx.send(None)
+            except asyncio.TimeoutError as e:
+                logger.warning(
+                    f"assignment for job {req.id} timed out",
+                    extra={"req": req},
                 )
-
-                participant = None
-                if identity:
-                    participant = await lkapi.room.get_participant(
-                        api.RoomParticipantIdentity(room=room_name, identity=identity)
-                    )
-
-                return room, participant
+                await av.assignment_tx.send(e)
+                return
             finally:
-                await lkapi.aclose()
+                await user_task
 
-        room_info, participant = worker._loop.run_until_complete(_pre_run())
-        logging.info(f"Simulating job for room {room_info.name} ({room_info.sid})")
-        _run_worker(
-            worker, started_cb=lambda _: worker._simulate_job(room_info, participant)
-        )
+            asgn = wait_assignment.result()
+            url = asgn.url
 
-    @cli.command(help="List used plugins")
-    def plugins() -> None:
-        for plugin in Plugin.registered_plugins:
-            logging.info(plugin.title)
-
-    @cli.command(help="Download required files of used plugins")
-    @click.option("--exclude", help="Exclude plugins", multiple=True)
-    def download_files(exclude: Tuple[str]) -> None:
-        for plugin in Plugin.registered_plugins:
-            if plugin.title in exclude:
-                continue
+            if not url:
+                url = self._opts.ws_url
+
+            self._start_process(asgn.job, url, asgn.token, av.data)
+
+        task = self._loop.create_task(_wait_response())
+        self._tasks.add(task)
+        task.add_done_callback(self._tasks.discard)
+
+    def _handle_assignment(self, assignment: agent.JobAssignment):
+        job = assignment.job
+        if job.id in self._pending_assignments:
+            fut = self._pending_assignments.pop(job.id)
+            fut.set_result(assignment)
+        else:
+            logger.warning(
+                f"received assignment for unknown job {job.id}",
+                extra={"job": job},
+            )
 
-            logging.info("Setup data for plugin %s", plugin.title)
-            plugin.download_files()
 
-    cli()
+async def _send_ignore_err(
+    ch: aio.ChanSender[agent.WorkerMessage], msg: agent.WorkerMessage
+):
+    # Used when we don't care about the result of sending
+    # e.g. when closing the worker, we close the channel.
+    with contextlib.suppress(aio.ChanClosed):
+        await ch.send(msg)
```

### Comparing `livekit-agents-0.4.1/livekit_agents.egg-info/PKG-INFO` & `livekit-agents-0.5.dev0/livekit_agents.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.4.1
+Version: 0.5.dev0
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
@@ -16,17 +16,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: click~=8.1.0
-Requires-Dist: livekit>=0.9.0
-Requires-Dist: livekit-api>=0.4.1
-Requires-Dist: livekit-protocol~=0.3.0
-Requires-Dist: websockets<13,>=12
+Requires-Dist: livekit~=0.9
+Requires-Dist: livekit-api~=0.4
+Requires-Dist: livekit-protocol~=0.4
+Requires-Dist: protobuf>=3
+Requires-Dist: types-protobuf<5,>=4
+Requires-Dist: python-json-logger~=2.0
+Requires-Dist: attrs~=23.0
+Requires-Dist: watchfiles~=0.21
+Requires-Dist: colorlog~=6.0
 Provides-Extra: codecs
-Requires-Dist: pyav>=12.0.2; extra == "codecs"
+Requires-Dist: av>=11.0.0; extra == "codecs"
 
 # LiveKit Agents
 
 The core LiveKit Agents Framework. See top-level README for more information.
```

### Comparing `livekit-agents-0.4.1/setup.py` & `livekit-agents-0.5.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import pathlib
 
 import setuptools
-import setuptools.command.build_py
-
 
 here = pathlib.Path(__file__).parent.resolve()
 about = {}
 with open(os.path.join(here, "livekit", "agents", "version.py"), "r") as f:
     exec(f.read(), about)
 
 
@@ -46,22 +44,29 @@
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit", "agents", "AI"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
         "click~=8.1.0",
-        "livekit>=0.9.0",
-        "livekit-api>=0.4.1",
-        "livekit-protocol~=0.3.0",
-        "websockets>=12,<13",
+        "livekit~=0.9",
+        "livekit-api~=0.4",
+        "livekit-protocol~=0.4",
+        "protobuf>=3",
+        "types-protobuf>=4,<5",
+        "python-json-logger~=2.0",
+        "attrs~=23.0",
+        "watchfiles~=0.21",
+        "colorlog~=6.0",
     ],
     extras_require={
-        "codecs": ["pyav>=12.0.2"],
+        "codecs": ["av>=11.0.0"],
+    },
+    package_data={
+        "livekit.agents": ["py.typed"],
     },
-    package_data={},
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
         "Source": "https://github.com/livekit/agents",
     },
 )
```

