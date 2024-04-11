# Comparing `tmp/gigagraph-0.0.26.tar.gz` & `tmp/gigagraph-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagraph-0.0.26.tar", max compression
+gzip compressed data, was "gigagraph-0.0.34.tar", max compression
```

## Comparing `gigagraph-0.0.26.tar` & `gigagraph-0.0.34.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0     1067 2024-02-09 11:26:26.015908 gigagraph-0.0.26/LICENSE
--rw-r--r--   0        0        0    50203 2024-03-06 08:45:49.105759 gigagraph-0.0.26/README.md
--rw-r--r--   0        0        0       69 2024-03-06 08:45:49.220137 gigagraph-0.0.26/langgraph/__init__.py
--rw-r--r--   0        0        0      294 2024-02-09 11:26:26.068963 gigagraph-0.0.26/langgraph/channels/__init__.py
--rw-r--r--   0        0        0     1554 2024-03-06 08:45:49.220512 gigagraph-0.0.26/langgraph/channels/any_value.py
--rw-r--r--   0        0        0     3959 2024-03-06 08:45:49.221166 gigagraph-0.0.26/langgraph/channels/base.py
--rw-r--r--   0        0        0     2004 2024-02-09 11:26:26.070346 gigagraph-0.0.26/langgraph/channels/binop.py
--rw-r--r--   0        0        0     3150 2024-02-09 11:26:26.070720 gigagraph-0.0.26/langgraph/channels/context.py
--rw-r--r--   0        0        0     1893 2024-03-06 08:45:49.221608 gigagraph-0.0.26/langgraph/channels/ephemeral_value.py
--rw-r--r--   0        0        0     1682 2024-02-09 11:26:26.071160 gigagraph-0.0.26/langgraph/channels/last_value.py
--rw-r--r--   0        0        0     2560 2024-02-09 11:26:26.071636 gigagraph-0.0.26/langgraph/channels/topic.py
--rw-r--r--   0        0        0      235 2024-02-09 11:26:26.072245 gigagraph-0.0.26/langgraph/checkpoint/__init__.py
--rw-r--r--   0        0        0     2558 2024-02-09 11:26:26.072651 gigagraph-0.0.26/langgraph/checkpoint/aiosqlite.py
--rw-r--r--   0        0        0     2071 2024-03-06 08:45:49.222314 gigagraph-0.0.26/langgraph/checkpoint/base.py
--rw-r--r--   0        0        0     1017 2024-02-09 11:26:26.073452 gigagraph-0.0.26/langgraph/checkpoint/memory.py
--rw-r--r--   0        0        0     2576 2024-02-09 11:26:26.073836 gigagraph-0.0.26/langgraph/checkpoint/sqlite.py
--rw-r--r--   0        0        0       96 2024-03-06 08:45:49.222832 gigagraph-0.0.26/langgraph/constants.py
--rw-r--r--   0        0        0      197 2024-02-09 11:26:26.074907 gigagraph-0.0.26/langgraph/graph/__init__.py
--rw-r--r--   0        0        0    12074 2024-03-06 08:45:49.223455 gigagraph-0.0.26/langgraph/graph/graph.py
--rw-r--r--   0        0        0      648 2024-02-09 11:26:26.075887 gigagraph-0.0.26/langgraph/graph/message.py
--rw-r--r--   0        0        0     7649 2024-03-06 08:45:49.223869 gigagraph-0.0.26/langgraph/graph/state.py
--rw-r--r--   0        0        0      306 2024-02-09 11:26:26.077283 gigagraph-0.0.26/langgraph/prebuilt/__init__.py
--rw-r--r--   0        0        0     5067 2024-02-09 11:26:26.077972 gigagraph-0.0.26/langgraph/prebuilt/agent_executor.py
--rw-r--r--   0        0        0    10662 2024-03-06 08:45:49.224367 gigagraph-0.0.26/langgraph/prebuilt/chat_agent_executor.py
--rw-r--r--   0        0        0     2416 2024-02-09 11:26:26.078939 gigagraph-0.0.26/langgraph/prebuilt/tool_executor.py
--rw-r--r--   0        0        0    40563 2024-03-06 08:45:49.224780 gigagraph-0.0.26/langgraph/pregel/__init__.py
--rw-r--r--   0        0        0     1223 2024-02-09 11:26:26.080151 gigagraph-0.0.26/langgraph/pregel/debug.py
--rw-r--r--   0        0        0     1461 2024-02-09 11:26:26.080541 gigagraph-0.0.26/langgraph/pregel/io.py
--rw-r--r--   0        0        0       53 2024-02-09 11:26:26.080872 gigagraph-0.0.26/langgraph/pregel/log.py
--rw-r--r--   0        0        0     7107 2024-03-06 08:45:49.225324 gigagraph-0.0.26/langgraph/pregel/read.py
--rw-r--r--   0        0        0      311 2024-03-06 08:45:49.225730 gigagraph-0.0.26/langgraph/pregel/reserved.py
--rw-r--r--   0        0        0     2841 2024-03-06 08:45:49.226097 gigagraph-0.0.26/langgraph/pregel/validate.py
--rw-r--r--   0        0        0     3093 2024-03-06 08:45:49.226372 gigagraph-0.0.26/langgraph/pregel/write.py
--rw-r--r--   0        0        0      133 2024-02-09 11:26:26.083078 gigagraph-0.0.26/langgraph/utils.py
--rw-r--r--   0        0        0      308 2024-03-06 08:45:49.226704 gigagraph-0.0.26/langgraph/version.py
--rw-r--r--   0        0        0     2251 2024-03-06 11:45:36.874147 gigagraph-0.0.26/pyproject.toml
--rw-r--r--   0        0        0    50839 1970-01-01 00:00:00.000000 gigagraph-0.0.26/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-02-09 11:26:26.015908 gigagraph-0.0.34/LICENSE
+-rw-r--r--   0        0        0    51426 2024-04-11 10:30:48.721273 gigagraph-0.0.34/README.md
+-rw-r--r--   0        0        0       69 2024-03-06 08:45:49.220137 gigagraph-0.0.34/langgraph/__init__.py
+-rw-r--r--   0        0        0      294 2024-02-09 11:26:26.068963 gigagraph-0.0.34/langgraph/channels/__init__.py
+-rw-r--r--   0        0        0     1682 2024-04-11 10:29:15.660408 gigagraph-0.0.34/langgraph/channels/any_value.py
+-rw-r--r--   0        0        0     4254 2024-04-11 10:29:15.660791 gigagraph-0.0.34/langgraph/channels/base.py
+-rw-r--r--   0        0        0     2028 2024-04-11 10:29:15.661181 gigagraph-0.0.34/langgraph/channels/binop.py
+-rw-r--r--   0        0        0     3180 2024-04-11 10:29:15.661495 gigagraph-0.0.34/langgraph/channels/context.py
+-rw-r--r--   0        0        0     1917 2024-04-11 10:29:15.661804 gigagraph-0.0.34/langgraph/channels/ephemeral_value.py
+-rw-r--r--   0        0        0     1706 2024-04-11 10:29:15.662068 gigagraph-0.0.34/langgraph/channels/last_value.py
+-rw-r--r--   0        0        0     1715 2024-04-11 10:29:15.662340 gigagraph-0.0.34/langgraph/channels/named_barrier_value.py
+-rw-r--r--   0        0        0     2584 2024-04-11 10:29:15.663095 gigagraph-0.0.34/langgraph/channels/topic.py
+-rw-r--r--   0        0        0      235 2024-02-09 11:26:26.072245 gigagraph-0.0.34/langgraph/checkpoint/__init__.py
+-rw-r--r--   0        0        0     5101 2024-04-11 10:29:15.663498 gigagraph-0.0.34/langgraph/checkpoint/aiosqlite.py
+-rw-r--r--   0        0        0     4286 2024-04-11 10:31:54.484801 gigagraph-0.0.34/langgraph/checkpoint/base.py
+-rw-r--r--   0        0        0     1816 2024-04-11 10:29:15.663924 gigagraph-0.0.34/langgraph/checkpoint/memory.py
+-rw-r--r--   0        0        0     5853 2024-04-11 10:29:15.664301 gigagraph-0.0.34/langgraph/checkpoint/sqlite.py
+-rw-r--r--   0        0        0      130 2024-04-11 10:29:15.664581 gigagraph-0.0.34/langgraph/constants.py
+-rw-r--r--   0        0        0      197 2024-02-09 11:26:26.074907 gigagraph-0.0.34/langgraph/graph/__init__.py
+-rw-r--r--   0        0        0    13169 2024-04-11 10:29:15.665930 gigagraph-0.0.34/langgraph/graph/graph.py
+-rw-r--r--   0        0        0     1429 2024-04-11 10:29:15.666282 gigagraph-0.0.34/langgraph/graph/message.py
+-rw-r--r--   0        0        0    10606 2024-04-11 10:29:15.666834 gigagraph-0.0.34/langgraph/graph/state.py
+-rw-r--r--   0        0        0      306 2024-02-09 11:26:26.077283 gigagraph-0.0.34/langgraph/prebuilt/__init__.py
+-rw-r--r--   0        0        0     5464 2024-04-11 10:29:15.667324 gigagraph-0.0.34/langgraph/prebuilt/agent_executor.py
+-rw-r--r--   0        0        0    10662 2024-03-06 08:45:49.224367 gigagraph-0.0.34/langgraph/prebuilt/chat_agent_executor.py
+-rw-r--r--   0        0        0     2232 2024-04-11 10:29:15.667616 gigagraph-0.0.34/langgraph/prebuilt/tool_executor.py
+-rw-r--r--   0        0        0    46963 2024-04-11 10:29:15.668709 gigagraph-0.0.34/langgraph/pregel/__init__.py
+-rw-r--r--   0        0        0     1240 2024-04-11 10:29:15.669066 gigagraph-0.0.34/langgraph/pregel/debug.py
+-rw-r--r--   0        0        0     3344 2024-04-11 10:29:15.669359 gigagraph-0.0.34/langgraph/pregel/io.py
+-rw-r--r--   0        0        0       53 2024-02-09 11:26:26.080872 gigagraph-0.0.34/langgraph/pregel/log.py
+-rw-r--r--   0        0        0     7750 2024-04-11 10:29:15.669754 gigagraph-0.0.34/langgraph/pregel/read.py
+-rw-r--r--   0        0        0      752 2024-04-11 10:29:15.669958 gigagraph-0.0.34/langgraph/pregel/types.py
+-rw-r--r--   0        0        0     3057 2024-04-11 10:29:15.670248 gigagraph-0.0.34/langgraph/pregel/validate.py
+-rw-r--r--   0        0        0     3867 2024-04-11 10:29:15.670561 gigagraph-0.0.34/langgraph/pregel/write.py
+-rw-r--r--   0        0        0        0 2024-03-12 15:00:07.691355 gigagraph-0.0.34/langgraph/py.typed
+-rw-r--r--   0        0        0     2282 2024-04-11 10:29:15.670837 gigagraph-0.0.34/langgraph/utils.py
+-rw-r--r--   0        0        0      308 2024-03-06 08:45:49.226704 gigagraph-0.0.34/langgraph/version.py
+-rw-r--r--   0        0        0     2237 2024-04-11 10:34:41.186243 gigagraph-0.0.34/pyproject.toml
+-rw-r--r--   0        0        0    52050 1970-01-01 00:00:00.000000 gigagraph-0.0.34/PKG-INFO
```

### Comparing `gigagraph-0.0.26/LICENSE` & `gigagraph-0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.26/README.md` & `gigagraph-0.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: gigagraph
+Version: 0.0.34
+Summary: gigagraph
+Home-page: https://github.com/ai-forever/gigagraph
+License: MIT
+Requires-Python: >=3.9.0,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: gigachain-core (>=0.1.38,<0.2.0)
+Project-URL: Repository, https://github.com/ai-forever/gigagraph
+Description-Content-Type: text/markdown
+
 # GigaGraph
 
 ⚡ Разработка языковых агентов в виде графов ⚡
 
 ## Описание
 
 GigaGraph — это библиотека, дающая возможность работать с LLM (большие языковые модели) для создания приложений, которые используют множество взаимодействующих цепочек (акторов) и сохраняют данные о состоянии.
@@ -431,14 +448,26 @@
 For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/persistence.ipynb)
 
 ### Human-in-the-loop
 
 LangGraph comes with built-in support for human-in-the-loop workflows. This is useful when you want to have a human review the current state before proceeding to a particular node.
 For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/human-in-the-loop.ipynb)
 
+### Visualizing the graph
+
+Agents you create with LangGraph can be complex. In order to make it easier to understand what is happening under the hood, we've added methods to print out and visualize the graph.
+This can create both ascii art as well as pngs.
+For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/visualization.ipynb)
+
+### "Time Travel"
+
+With "time travel" functionality you can jump to any point in the graph execution, modify the state, and rerun from there.
+This is useful for both debugging workflows, as well as end user-facing workflows to allow them to correct the state.
+For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/time-travel.ipynb)
+
 
 ## Примеры
 
 ### ChatAgentExecutor: with function calling
 
 ### Исполнитель чат-агента с возможностью вызывать функции
 
@@ -472,31 +501,29 @@
 Примеры небольших изменений, которые можно сделать при разработке исполнителя чат-агента.
 Приведенные вариации основаны на примере [Getting Started Notebook](https://github.com/langchain-ai/langgraph/blob/main/examples/agent_executor/base.ipynb).
 
 - [Human-in-the-loop](https://github.com/langchain-ai/langgraph/blob/main/examples/agent_executor/human-in-the-loop.ipynb). Пример демонстрирует как реализовать подход «человек-в-цикле».
 - [Принудительный вызов инструмента](https://github.com/langchain-ai/langgraph/blob/main/examples/agent_executor/force-calling-a-tool-first.ipynb). Пример демонстрирует как всегда вызывать определенный инструмент в первую очередь.
 - [Управление этапами работы агента](https://github.com/langchain-ai/langgraph/blob/main/examples/agent_executor/managing-agent-steps.ipynb). Пример демонстрирует, как можно более детально управлять промежуточными этапами работы агента.
 
-
 ### Planning Agent Examples
 
 The following notebooks implement agent architectures prototypical of the "plan-and-execute" style, where an LLM planner decomposes a user request into a program, an executor executes the program, and an LLM synthesizes a response (and/or dynamically replans) based on the program outputs.
 
 - [Plan-and-execute](https://github.com/langchain-ai/langgraph/blob/main/examples/plan-and-execute/plan-and-execute.ipynb): a simple agent with a **planner** that generates a multi-step task list, an **executor** that invokes the tools in the plan, and a **replanner** that responds or generates an updated plan. Based on the [Plan-and-solve](https://arxiv.org/abs/2305.04091) paper by Wang, et. al.
 - [Reasoning without Observation](https://github.com/langchain-ai/langgraph/blob/main/examples/rewoo/rewoo.ipynb): planner generates a task list whose observations are saved as **variables**. Variables can be used in subsequent tasks to reduce the need for further re-planning. Based on the [ReWOO](https://arxiv.org/abs/2305.18323) paper by Xu, et. al.
 - [LLMCompiler](https://github.com/langchain-ai/langgraph/blob/main/examples/llm-compiler/LLMCompiler.ipynb): planner generates a **DAG** of tasks with variable responses. Tasks are **streamed** and executed eagerly to minimize tool execution runtime. Based on the [paper](https://arxiv.org/abs/2312.04511) by Kim, et. al.
 
-
 ### Reflection / Self-Critique
 
 When output quality is a major concern, it's common to incorporate some combination of self-critique or reflection and external validation to refine your system's outputs. The following examples demonstrate research that implement this type of design.
 
 - [Basic Reflection](./examples/reflection/reflection.ipynb): add a simple "reflect" step in your graph to prompt your system to revise its outputs.
 - [Reflexion](./examples/reflexion/reflexion.ipynb): critique missing and superflous aspects of the agent's response to guide subsequent steps. Based on [Reflexion](https://arxiv.org/abs/2303.11366), by Shinn, et. al.
-- [Language Agent Tree Search](./examples/lats/lats.ipynb): execute multiple agents in parallel, using reflection and environmental rewards to drive a Monte Carlo Tree Search. Based on [LATS](https://arxiv.org/abs/2310.04406/LanguageAgentTreeSearch/), by Zhou, et. al.
+- [Language Agent Tree Search](./examples/lats/lats.ipynb): execute multiple agents in parallel, using reflection and environmental rewards to drive a Monte Carlo Tree Search. Based on [LATS](https://arxiv.org/abs/2310.04406), by Zhou, et. al.
 
 ### Multi-agent Examples
 ### Примеры с несколькими агентами
 
 - [Совместная работа нескольких агентов](https://github.com/langchain-ai/langgraph/blob/main/examples/multi_agent/multi-agent-collaboration.ipynb). Пример демонстрирует как создать двух агентов, которые работают вместе для решения задачи.
 - [Несколько агентов с «руководителем»](https://github.com/langchain-ai/langgraph/blob/main/examples/multi_agent/agent_supervisor.ipynb). Пример демонстрирует как организовать работу агентов используя LLM в роли «руководителя», который решает как распределять работу.
 - [Иерархичные команды агентов](https://github.com/langchain-ai/langgraph/blob/main/examples/multi_agent/hierarchical_agent_teams.ipynb): пример демонстрирует как организовать «команды» агентов, которые будут взаимодействовать для решения задачи, в виде вложенных графов.
@@ -508,15 +535,16 @@
 - [Оценка чат-бота с помощью симуляции взаимодействия нескольких агентов.](https://github.com/langchain-ai/langgraph/blob/main/examples/chatbot-simulation-evaluation/agent-simulation-evaluation.ipynb). В примере показано как симулировать диалог «виртуального пользователя» с чат-ботом.
 
 ### Асинхронная работа
 
 При работе с асинхронными процессами вам может потребоваться создать с помощью GigaGraph граф с вершинами, которые будут асинхронными по умолчанию.
 [Пример](https://github.com/langchain-ai/langgraph/blob/main/examples/async.ipynb).
 
-### Потоковая передача токенов
+- [Chat bot evaluation as multi-agent simulation](https://github.com/langchain-ai/langgraph/blob/main/examples/chatbot-simulation-evaluation/agent-simulation-evaluation.ipynb): how to simulate a dialogue between a "virtual user" and your chat bot
+- [Evaluating over a dataset](./examples/chatbot-simulation-evaluation/langsmith-agent-simulation-evaluation.ipynb): benchmark your assistant over a LangSmith dataset, which tasks a simulated customer to red-team your chat bot.
 
 Ответ модели может занимать продолжительное время и вам может потребоваться на лету отображать пользователям результат работы модели.
 [Пример](https://github.com/langchain-ai/langgraph/blob/main/examples/streaming-tokens.ipynb).
 
 ### Устойчивость
 
 GigaGraph позволяет сохранять состояние графа в определенный момент времени и потом возобновлять работу с этого состояния.
@@ -657,15 +685,15 @@
 ```
 Точка входа в граф.
 Задает вершину, которая будет вызвана в самом начале.
 Принимает один параметр:
 
 - `key` — название вершины, которую нужно вызывать в первую очередь.
 
-#### `.add_conditional_edges`
+#### `.set_conditional_entry_point`
 
 ```python
     def set_conditional_entry_point(
         self,
         condition: Callable[..., str],
         conditional_edge_mapping: Optional[Dict[str, str]] = None,
     ) -> None:
@@ -673,15 +701,14 @@
 
 This method adds a conditional entry point.
 What this means is that when the graph is called, it will call the `condition` Callable to decide what node to enter into first.
 
 - `condition`: A function to call to decide what to do next. The input will be the input to the graph. It should return a string that is present in `conditional_edge_mapping` and represents the edge to take.
 - `conditional_edge_mapping`: A mapping of string to string. The keys should be strings that may be returned by `condition`. The values should be the downstream node to call if that condition is returned.
 
-
 #### `.set_finish_point`
 
 ```python
     def set_finish_point(self, key: str) -> None:
 ```
 
 This is the exit point of the graph.
@@ -768,15 +795,15 @@
 
 inputs = {"messages": [HumanMessage(content="какая погода в саратове")]}
 for s in app.stream(inputs):
     print(list(s.values())[0])
     print("----")
 ```
 
-### create_tool_calling_executor
+### chat_agent_executor.create_tool_calling_executor
 
 ```python
 from langgraph.prebuilt import chat_agent_executor
 ```
 
 This is a helper function for creating a graph that works with a chat model that utilizes tool calling.
 Can be created by passing in a model and a list of tools.
@@ -829,7 +856,8 @@
 app = create_agent_executor(agent_runnable, tools)
 
 inputs = {"input": "what is the weather in sf", "chat_history": []}
 for s in app.stream(inputs):
     print(list(s.values())[0])
     print("----")
 ```
+
```

### Comparing `gigagraph-0.0.26/langgraph/channels/any_value.py` & `gigagraph-0.0.34/langgraph/channels/last_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,63 @@
 from contextlib import contextmanager
 from typing import Generator, Generic, Optional, Sequence, Type
 
 from typing_extensions import Self
 
-from langgraph.channels.base import BaseChannel, EmptyChannelError, Value
+from langgraph.channels.base import (
+    BaseChannel,
+    EmptyChannelError,
+    InvalidUpdateError,
+    Value,
+)
 
 
-class AnyValue(Generic[Value], BaseChannel[Value, Value, Value]):
-    """Stores the last value received, assumes that if multiple values are
-    received, they are all equal."""
+class LastValue(Generic[Value], BaseChannel[Value, Value, Value]):
+    """Stores the last value received, can receive at most one value per step."""
 
     def __init__(self, typ: Type[Value]) -> None:
         self.typ = typ
 
     @property
     def ValueType(self) -> Type[Value]:
         """The type of the value stored in the channel."""
         return self.typ
 
     @property
     def UpdateType(self) -> Type[Value]:
         """The type of the update received by the channel."""
         return self.typ
 
+    def checkpoint(self) -> Value:
+        try:
+            return self.value
+        except AttributeError:
+            raise EmptyChannelError()
+
     @contextmanager
-    def empty(self, checkpoint: Optional[Value] = None) -> Generator[Self, None, None]:
+    def from_checkpoint(
+        self, checkpoint: Optional[Value] = None
+    ) -> Generator[Self, None, None]:
         empty = self.__class__(self.typ)
         if checkpoint is not None:
             empty.value = checkpoint
         try:
             yield empty
         finally:
             try:
                 del empty.value
             except AttributeError:
                 pass
 
     def update(self, values: Sequence[Value]) -> None:
         if len(values) == 0:
             return
+        if len(values) != 1:
+            raise InvalidUpdateError("LastValue can only receive one value per step.")
 
         self.value = values[-1]
 
     def get(self) -> Value:
         try:
             return self.value
         except AttributeError:
             raise EmptyChannelError()
-
-    def checkpoint(self) -> Value:
-        try:
-            return self.value
-        except AttributeError:
-            raise EmptyChannelError()
```

### Comparing `gigagraph-0.0.26/langgraph/channels/base.py` & `gigagraph-0.0.34/langgraph/channels/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,57 +41,65 @@
         """The type of the value stored in the channel."""
 
     @property
     @abstractmethod
     def UpdateType(self) -> Any:
         """The type of the update received by the channel."""
 
+    # ser/de methods
+
+    @abstractmethod
+    def checkpoint(self) -> Optional[C]:
+        """Return a serializable representation of the channel's current state.
+        Raises EmptyChannelError if the channel is empty (never updated yet),
+        or doesn't support checkpoints."""
+
     @contextmanager
     @abstractmethod
-    def empty(self, checkpoint: Optional[C] = None) -> Generator[Self, None, None]:
-        """Return a new identical channel, optionally initialized from a checkpoint."""
+    def from_checkpoint(
+        self, checkpoint: Optional[C] = None
+    ) -> Generator[Self, None, None]:
+        """Return a new identical channel, optionally initialized from a checkpoint.
+        If the checkpoint contains complex data structures, they should be copied."""
 
     @asynccontextmanager
-    async def aempty(
+    async def afrom_checkpoint(
         self, checkpoint: Optional[C] = None
     ) -> AsyncGenerator[Self, None]:
-        """Return a new identical channel, optionally initialized from a checkpoint."""
-        with self.empty(checkpoint) as value:
+        """Return a new identical channel, optionally initialized from a checkpoint.
+        If the checkpoint contains complex data structures, they should be copied."""
+        with self.from_checkpoint(checkpoint) as value:
             yield value
 
+    # state methods
+
     @abstractmethod
     def update(self, values: Sequence[Update]) -> None:
         """Update the channel's value with the given sequence of updates.
         The order of the updates in the sequence is arbitrary.
 
         Raises InvalidUpdateError if the sequence of updates is invalid."""
 
     @abstractmethod
     def get(self) -> Value:
         """Return the current value of the channel.
 
         Raises EmptyChannelError if the channel is empty (never updated yet)."""
 
-    @abstractmethod
-    def checkpoint(self) -> Optional[C]:
-        """Return a string representation of the channel's current state.
-
-        Raises EmptyChannelError if the channel is empty (never updated yet),
-        or doesn't supportcheckpoints."""
-
 
 @contextmanager
 def ChannelsManager(
     channels: Mapping[str, BaseChannel],
     checkpoint: Checkpoint,
 ) -> Generator[Mapping[str, BaseChannel], None, None]:
     """Manage channels for the lifetime of a Pregel invocation (multiple steps)."""
     # TODO use https://docs.python.org/3/library/contextlib.html#contextlib.ExitStack
     empty = {
-        k: v.empty(checkpoint["channel_values"].get(k)) for k, v in channels.items()
+        k: v.from_checkpoint(checkpoint["channel_values"].get(k))
+        for k, v in channels.items()
     }
     try:
         yield {k: v.__enter__() for k, v in empty.items()}
     finally:
         for v in empty.values():
             v.__exit__(None, None, None)
 
@@ -99,15 +107,16 @@
 @asynccontextmanager
 async def AsyncChannelsManager(
     channels: Mapping[str, BaseChannel],
     checkpoint: Checkpoint,
 ) -> AsyncGenerator[Mapping[str, BaseChannel], None]:
     """Manage channels for the lifetime of a Pregel invocation (multiple steps)."""
     empty = {
-        k: v.aempty(checkpoint["channel_values"].get(k)) for k, v in channels.items()
+        k: v.afrom_checkpoint(checkpoint["channel_values"].get(k))
+        for k, v in channels.items()
     }
     try:
         yield {k: await v.__aenter__() for k, v in empty.items()}
     finally:
         for v in empty.values():
             await v.__aexit__(None, None, None)
```

### Comparing `gigagraph-0.0.26/langgraph/channels/binop.py` & `gigagraph-0.0.34/langgraph/channels/binop.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,24 @@
         return self.typ
 
     @property
     def UpdateType(self) -> Type[Value]:
         """The type of the update received by the channel."""
         return self.typ
 
+    def checkpoint(self) -> Value:
+        try:
+            return self.value
+        except AttributeError:
+            raise EmptyChannelError()
+
     @contextmanager
-    def empty(self, checkpoint: Optional[Value] = None) -> Generator[Self, None, None]:
+    def from_checkpoint(
+        self, checkpoint: Optional[Value] = None
+    ) -> Generator[Self, None, None]:
         empty = self.__class__(self.typ, self.operator)
         if checkpoint is not None:
             empty.value = checkpoint
         try:
             yield empty
         finally:
             try:
@@ -58,13 +66,7 @@
             self.value = self.operator(self.value, value)
 
     def get(self) -> Value:
         try:
             return self.value
         except AttributeError:
             raise EmptyChannelError()
-
-    def checkpoint(self) -> Value:
-        try:
-            return self.value
-        except AttributeError:
-            raise EmptyChannelError()
```

### Comparing `gigagraph-0.0.26/langgraph/channels/context.py` & `gigagraph-0.0.34/langgraph/channels/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,50 +61,50 @@
         )
 
     @property
     def UpdateType(self) -> Type[None]:
         """The type of the update received by the channel."""
         raise InvalidUpdateError()
 
+    def checkpoint(self) -> None:
+        raise EmptyChannelError()
+
     @contextmanager
-    def empty(self, checkpoint: None = None) -> Generator[Self, None, None]:
+    def from_checkpoint(self, checkpoint: None = None) -> Generator[Self, None, None]:
         if self.ctx is None:
             raise ValueError("Cannot enter sync context manager.")
 
         empty = self.__class__(ctx=self.ctx, actx=self.actx, typ=self.typ)
         # ContextManager doesn't have a checkpoint
         ctx = self.ctx()
         empty.value = ctx.__enter__()
         try:
             yield empty
         finally:
             ctx.__exit__(None, None, None)
 
     @asynccontextmanager
-    async def aempty(
+    async def afrom_checkpoint(
         self, checkpoint: Optional[str] = None
     ) -> AsyncGenerator[Self, None]:
         if self.actx is not None:
             empty = self.__class__(ctx=self.ctx, actx=self.actx, typ=self.typ)
             # ContextManager doesn't have a checkpoint
             actx = self.actx()
             empty.value = await actx.__aenter__()
             try:
                 yield empty
             finally:
                 await actx.__aexit__(None, None, None)
         else:
-            with self.empty() as empty:
+            with self.from_checkpoint() as empty:
                 yield empty
 
     def update(self, values: Sequence[None]) -> None:
         if values:
             raise InvalidUpdateError()
 
     def get(self) -> Value:
         try:
             return self.value
         except AttributeError:
             raise EmptyChannelError()
-
-    def checkpoint(self) -> None:
-        raise EmptyChannelError()
```

### Comparing `gigagraph-0.0.26/langgraph/channels/ephemeral_value.py` & `gigagraph-0.0.34/langgraph/channels/ephemeral_value.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,16 +24,24 @@
         return self.typ
 
     @property
     def UpdateType(self) -> Type[Value]:
         """The type of the update received by the channel."""
         return self.typ
 
+    def checkpoint(self) -> Value:
+        try:
+            return self.value
+        except AttributeError:
+            raise EmptyChannelError()
+
     @contextmanager
-    def empty(self, checkpoint: Optional[Value] = None) -> Generator[Self, None, None]:
+    def from_checkpoint(
+        self, checkpoint: Optional[Value] = None
+    ) -> Generator[Self, None, None]:
         empty = self.__class__(self.typ, self.guard)
         if checkpoint is not None:
             empty.value = checkpoint
         try:
             yield empty
         finally:
             try:
@@ -55,13 +63,7 @@
         self.value = values[-1]
 
     def get(self) -> Value:
         try:
             return self.value
         except AttributeError:
             raise EmptyChannelError()
-
-    def checkpoint(self) -> Value:
-        try:
-            return self.value
-        except AttributeError:
-            raise EmptyChannelError()
```

### Comparing `gigagraph-0.0.26/langgraph/channels/last_value.py` & `gigagraph-0.0.34/langgraph/channels/named_barrier_value.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,55 +7,54 @@
     BaseChannel,
     EmptyChannelError,
     InvalidUpdateError,
     Value,
 )
 
 
-class LastValue(Generic[Value], BaseChannel[Value, Value, Value]):
-    """Stores the last value received, can receive at most one value per step."""
+class NamedBarrierValue(Generic[Value], BaseChannel[Value, Value, set[Value]]):
+    """A channel that waits until all named values are received before making the value available."""
 
-    def __init__(self, typ: Type[Value]) -> None:
+    def __init__(self, typ: Type[Value], names: set[Value]) -> None:
         self.typ = typ
+        self.names = names
+        self.seen = set()
 
     @property
     def ValueType(self) -> Type[Value]:
         """The type of the value stored in the channel."""
         return self.typ
 
     @property
     def UpdateType(self) -> Type[Value]:
         """The type of the update received by the channel."""
         return self.typ
 
+    def checkpoint(self) -> set[Value]:
+        return self.seen
+
     @contextmanager
-    def empty(self, checkpoint: Optional[Value] = None) -> Generator[Self, None, None]:
-        empty = self.__class__(self.typ)
+    def from_checkpoint(
+        self, checkpoint: Optional[set[Value]] = None
+    ) -> Generator[Self, None, None]:
+        empty = self.__class__(self.typ, self.names)
         if checkpoint is not None:
-            empty.value = checkpoint
+            empty.seen = checkpoint.copy()
+
         try:
             yield empty
         finally:
-            try:
-                del empty.value
-            except AttributeError:
-                pass
+            pass
 
     def update(self, values: Sequence[Value]) -> None:
-        if len(values) == 0:
-            return
-        if len(values) != 1:
-            raise InvalidUpdateError("LastValue can only receive one value per step.")
-
-        self.value = values[-1]
+        if self.seen == self.names:
+            self.seen = set()
+        for value in values:
+            if value in self.names:
+                self.seen.add(value)
+            else:
+                raise InvalidUpdateError(f"Value {value} not in {self.names}")
 
     def get(self) -> Value:
-        try:
-            return self.value
-        except AttributeError:
-            raise EmptyChannelError()
-
-    def checkpoint(self) -> Value:
-        try:
-            return self.value
-        except AttributeError:
+        if self.seen != self.names:
             raise EmptyChannelError()
+        return None
```

### Comparing `gigagraph-0.0.26/langgraph/channels/topic.py` & `gigagraph-0.0.34/langgraph/channels/topic.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,22 +45,25 @@
         return Sequence[self.typ]  # type: ignore[name-defined]
 
     @property
     def UpdateType(self) -> Any:
         """The type of the update received by the channel."""
         return Union[self.typ, list[self.typ]]  # type: ignore[name-defined]
 
+    def checkpoint(self) -> tuple[set[Value], list[Value]]:
+        return (self.seen, self.values)
+
     @contextmanager
-    def empty(
+    def from_checkpoint(
         self, checkpoint: Optional[tuple[set[Value], list[Value]]] = None
     ) -> Generator[Self, None, None]:
         empty = self.__class__(self.typ, self.unique, self.accumulate)
         if checkpoint is not None:
-            empty.seen = checkpoint[0]
-            empty.values = checkpoint[1]
+            empty.seen = checkpoint[0].copy()
+            empty.values = checkpoint[1].copy()
         try:
             yield empty
         finally:
             pass
 
     def update(self, values: Sequence[Union[Value, list[Value]]]) -> None:
         if not self.accumulate:
@@ -72,10 +75,7 @@
                         self.seen.add(value)
                         self.values.append(value)
             else:
                 self.values.extend(flat_values)
 
     def get(self) -> Sequence[Value]:
         return list(self.values)
-
-    def checkpoint(self) -> tuple[set[Value], list[Value]]:
-        return (self.seen, self.values)
```

### Comparing `gigagraph-0.0.26/langgraph/graph/graph.py` & `gigagraph-0.0.34/langgraph/graph/graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,113 @@
 import logging
-from asyncio import iscoroutinefunction
 from collections import defaultdict
-from typing import Any, Callable, Dict, NamedTuple, Optional, Sequence
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    NamedTuple,
+    Optional,
+    Sequence,
+    Union,
+    cast,
+)
 
 from langchain_core.runnables import Runnable
-from langchain_core.runnables.base import (
-    RunnableLambda,
-    RunnableLike,
-    coerce_to_runnable,
-)
+from langchain_core.runnables.base import RunnableLike, coerce_to_runnable
 from langchain_core.runnables.config import RunnableConfig
 from langchain_core.runnables.graph import (
     Graph as RunnableGraph,
 )
 from langchain_core.runnables.graph import (
     Node as RunnableGraphNode,
 )
 
 from langgraph.channels.ephemeral_value import EphemeralValue
 from langgraph.checkpoint import BaseCheckpointSaver
+from langgraph.constants import TAG_HIDDEN
 from langgraph.pregel import Channel, Pregel
+from langgraph.pregel.read import PregelNode
+from langgraph.pregel.write import ChannelWrite, ChannelWriteEntry
+from langgraph.utils import RunnableCallable
 
 logger = logging.getLogger(__name__)
 
 START = "__start__"
 END = "__end__"
 
 
 class Branch(NamedTuple):
-    condition: Callable[..., str]
+    condition: Runnable[Any, Union[str, list[str]]]
     ends: Optional[dict[str, str]]
 
-    def runnable(self, input: Any) -> Runnable:
-        result = self.condition(input)
+    def run(
+        self,
+        writer: Callable[[list[str]], Optional[Runnable]],
+        reader: Optional[Callable[[RunnableConfig], Any]] = None,
+    ) -> None:
+        return ChannelWrite.register_writer(
+            RunnableCallable(
+                func=self._route,
+                afunc=self._aroute,
+                writer=writer,
+                reader=reader,
+                name=None,
+                trace=False,
+            )
+        )
+
+    def _route(
+        self,
+        input: Any,
+        config: RunnableConfig,
+        *,
+        reader: Optional[Callable[[], Any]],
+        writer: Callable[[str], Optional[Runnable]],
+    ) -> Runnable:
+        result = self.condition.invoke(reader(config) if reader else input, config)
+        if isinstance(result, str):
+            result = [result]
         if self.ends:
-            destination = self.ends[result]
+            destinations = [self.ends[r] for r in result]
         else:
-            destination = result
-        return Channel.write_to(f"{destination}:inbox" if destination != END else END)
+            destinations = result
+        return writer(destinations) or input
+
+    async def _aroute(
+        self,
+        input: Any,
+        config: RunnableConfig,
+        *,
+        reader: Optional[Callable[[], Any]],
+        writer: Callable[[str], Optional[Runnable]],
+    ) -> Runnable:
+        result = await self.condition.ainvoke(
+            reader(config) if reader else input, config
+        )
+        if isinstance(result, str):
+            result = [result]
+        if self.ends:
+            destinations = [self.ends[r] for r in result]
+        else:
+            destinations = result
+        return writer(destinations) or input
 
 
 class Graph:
     def __init__(self) -> None:
         self.nodes: dict[str, Runnable] = {}
         self.edges = set[tuple[str, str]]()
-        self.branches: defaultdict[str, list[Branch]] = defaultdict(list)
+        self.branches: defaultdict[str, dict[str, Branch]] = defaultdict(dict)
         self.support_multiple_edges = False
         self.compiled = False
-        self.entry_point: Optional[str] = None
-        self.entry_point_branch: Optional[Branch] = None
+
+    @property
+    def _all_edges(self) -> set[tuple[str, str]]:
+        return self.edges
 
     def add_node(self, key: str, action: RunnableLike) -> None:
         if self.compiled:
             logger.warning(
                 "Adding a node to a graph that has already been compiled. This will "
                 "not be reflected in the compiled graph."
             )
@@ -67,108 +122,100 @@
         if self.compiled:
             logger.warning(
                 "Adding an edge to a graph that has already been compiled. This will "
                 "not be reflected in the compiled graph."
             )
         if start_key == END:
             raise ValueError("END cannot be a start node")
-        if start_key not in self.nodes:
+        if end_key == START:
+            raise ValueError("START cannot be an end node")
+        if start_key not in self.nodes and start_key != START:
             raise ValueError(f"Need to add_node `{start_key}` first")
         if end_key not in self.nodes and end_key != END:
             raise ValueError(f"Need to add_node `{end_key}` first")
 
         if not self.support_multiple_edges and start_key in set(
             start for start, _ in self.edges
         ):
-            raise ValueError(f"Already found path for {start_key}")
+            raise ValueError(
+                f"Already found path for node '{start_key}'.\n"
+                "For multiple edges, use StateGraph with an annotated state key."
+            )
 
         self.edges.add((start_key, end_key))
 
     def add_conditional_edges(
         self,
         start_key: str,
-        condition: Callable[..., str],
-        conditional_edge_mapping: Optional[Dict[str, str]] = None,
+        condition: Union[
+            Callable[..., Union[str, list[str]]],
+            Callable[..., Awaitable[Union[str, list[str]]]],
+            Runnable[Any, Union[str, list[str]]],
+        ],
+        conditional_edge_mapping: Optional[dict[str, str]] = None,
     ) -> None:
         if self.compiled:
             logger.warning(
                 "Adding an edge to a graph that has already been compiled. This will "
                 "not be reflected in the compiled graph."
             )
-        if start_key not in self.nodes:
+        # find a name for the condition
+        condition = coerce_to_runnable(condition)
+        name = condition.name or "condition"
+        # validate the condition
+        if start_key not in self.nodes and start_key != START:
             raise ValueError(f"Need to add_node `{start_key}` first")
-        if iscoroutinefunction(condition):
-            raise ValueError("Condition cannot be a coroutine function")
         if conditional_edge_mapping and set(
             conditional_edge_mapping.values()
         ).difference([END]).difference(self.nodes):
             raise ValueError(
                 f"Missing nodes which are in conditional edge mapping. Mapping "
                 f"contains possible destinations: "
                 f"{list(conditional_edge_mapping.values())}. Possible nodes are "
                 f"{list(self.nodes.keys())}."
             )
-
-        self.branches[start_key].append(Branch(condition, conditional_edge_mapping))
+        if name in self.branches[start_key]:
+            raise ValueError(
+                f"Branch with name `{condition.name}` already exists for node "
+                f"`{start_key}`"
+            )
+        # save it
+        self.branches[start_key][name] = Branch(condition, conditional_edge_mapping)
 
     def set_entry_point(self, key: str) -> None:
-        if self.compiled:
-            logger.warning(
-                "Setting the entry point of a graph that has already been compiled. "
-                "This will not be reflected in the compiled graph."
-            )
-        if key not in self.nodes:
-            raise ValueError(f"Need to add_node `{key}` first")
-        self.entry_point = key
+        return self.add_edge(START, key)
 
     def set_conditional_entry_point(
         self,
-        condition: Callable[..., str],
+        condition: Union[
+            Callable[..., str], Callable[..., Awaitable[str]], Runnable[Any, str]
+        ],
         conditional_edge_mapping: Optional[Dict[str, str]] = None,
     ) -> None:
-        if self.compiled:
-            logger.warning(
-                "Setting the entry point of a graph that has already been compiled. "
-                "This will not be reflected in the compiled graph."
-            )
-        if iscoroutinefunction(condition):
-            raise ValueError("Condition cannot be a coroutine function")
-        if conditional_edge_mapping and set(
-            conditional_edge_mapping.values()
-        ).difference([END]).difference(self.nodes):
-            raise ValueError(
-                f"Missing nodes which are in conditional edge mapping. Mapping "
-                f"contains possible destinations: "
-                f"{list(conditional_edge_mapping.values())}. Possible nodes are "
-                f"{list(self.nodes.keys())}."
-            )
-        self.entry_point_branch = Branch(condition, conditional_edge_mapping)
+        return self.add_conditional_edges(START, condition, conditional_edge_mapping)
 
     def set_finish_point(self, key: str) -> None:
         return self.add_edge(key, END)
 
     def validate(self, interrupt: Optional[Sequence[str]] = None) -> None:
-        all_starts = {src for src, _ in self.edges} | {src for src in self.branches}
+        all_starts = {src for src, _ in self._all_edges} | {
+            src for src in self.branches
+        }
         for node in self.nodes:
             if node not in all_starts:
                 raise ValueError(f"Node `{node}` is a dead-end")
 
-        branches = [
-            branch for branch_list in self.branches.values() for branch in branch_list
+        all_branches = [
+            branch
+            for branches in self.branches.values()
+            for branch in branches.values()
         ]
-        if self.entry_point_branch is not None:
-            branches.append(self.entry_point_branch)
-
-        all_hard_ends = {end for _, end in self.edges}
-        if self.entry_point is not None:
-            all_hard_ends.add(self.entry_point)
-
-        if all(branch.ends is not None for branch in branches):
-            all_ends = all_hard_ends | {
-                end for branch in branches for end in branch.ends.values()
+        if all(branch.ends is not None for branch in all_branches):
+            all_ends = {end for _, end in self._all_edges} | {
+                end for branch in all_branches for end in branch.ends.values()
             }
 
             for node in self.nodes:
                 if node not in all_ends:
                     raise ValueError(f"Node `{node}` is not reachable")
 
         if interrupt:
@@ -181,75 +228,104 @@
     def compile(
         self,
         checkpointer: Optional[BaseCheckpointSaver] = None,
         interrupt_before: Optional[Sequence[str]] = None,
         interrupt_after: Optional[Sequence[str]] = None,
         debug: bool = False,
     ) -> "CompiledGraph":
+        # assign default values
         interrupt_before = interrupt_before or []
         interrupt_after = interrupt_after or []
-        self.validate(interrupt=interrupt_before + interrupt_after)
 
-        outgoing_edges = defaultdict(list)
-        for start, end in self.edges:
-            outgoing_edges[start].append(f"{end}:inbox" if end != END else END)
-
-        nodes = {
-            key: (Channel.subscribe_to(f"{key}:inbox") | node | Channel.write_to(key))
-            for key, node in self.nodes.items()
-        }
-        node_outboxes = {
-            # we clear outbox channels after each step
-            key: EphemeralValue(Any)
-            for key in self.nodes
-        }
-
-        for key in self.nodes:
-            outgoing = outgoing_edges[key]
-            edges_key = f"{key}:edges"
-            if outgoing or key in self.branches:
-                nodes[edges_key] = Channel.subscribe_to(key, tags=["langsmith:hidden"])
-            if outgoing:
-                nodes[edges_key] |= Channel.write_to(*[dest for dest in outgoing])
-            if key in self.branches:
-                for branch in self.branches[key]:
-                    nodes[edges_key] |= RunnableLambda(
-                        branch.runnable, name=f"{key}_condition"
-                    )
-
-        if self.entry_point_branch:
-            nodes[f"{START}:edges"] = Channel.subscribe_to(
-                START, tags=["langsmith:hidden"]
-            ) | RunnableLambda(
-                self.entry_point_branch.runnable, name=f"{START}_condition"
-            )
-        elif self.entry_point is None:
-            raise ValueError("No entry point set")
+        # validate the graph
+        self.validate(interrupt=interrupt_before + interrupt_after)
 
-        return CompiledGraph(
+        # create empty compiled graph
+        compiled = CompiledGraph(
             graph=self,
-            nodes=nodes,
-            channels={**node_outboxes},
-            input=f"{self.entry_point}:inbox" if self.entry_point else START,
-            output=END,
-            hidden=[f"{node}:inbox" for node in self.nodes],
-            snapshot_channels=list(self.nodes),
+            nodes={},
+            channels={START: EphemeralValue(Any), END: EphemeralValue(Any)},
+            input_channels=START,
+            output_channels=END,
+            stream_mode="values",
+            stream_channels=[],
             checkpointer=checkpointer,
-            interrupt_before_nodes=[f"{node}:inbox" for node in interrupt_before],
+            interrupt_before_nodes=interrupt_before,
             interrupt_after_nodes=interrupt_after,
+            auto_validate=False,
             debug=debug,
         )
 
+        # attach nodes, edges, and branches
+        for key, node in self.nodes.items():
+            compiled.attach_node(key, node)
+
+        for start, end in self.edges:
+            compiled.attach_edge(start, end)
+
+        for start, branches in self.branches.items():
+            for name, branch in branches.items():
+                compiled.attach_branch(start, name, branch)
+
+        # validate the compiled graph
+        return compiled.validate()
+
 
 class CompiledGraph(Pregel):
     graph: Graph
 
+    def attach_node(self, key: str, node: Runnable) -> None:
+        self.channels[key] = EphemeralValue(Any)
+        self.nodes[key] = (
+            PregelNode(channels=[], triggers=[])
+            | node
+            | ChannelWrite([ChannelWriteEntry(key)], tags=[TAG_HIDDEN])
+        )
+        cast(list[str], self.stream_channels).append(key)
+
+    def attach_edge(self, start: str, end: str) -> None:
+        if end == END:
+            # publish to end channel
+            self.nodes[start].writers.append(
+                ChannelWrite([ChannelWriteEntry(END)], tags=[TAG_HIDDEN])
+            )
+        else:
+            # subscribe to start channel
+            self.nodes[end].triggers.append(start)
+            self.nodes[end].channels.append(start)
+
+    def attach_branch(self, start: str, name: str, branch: Branch) -> None:
+        def branch_writer(ends: list[str]) -> Optional[ChannelWrite]:
+            channels = [
+                f"branch:{start}:{name}:{end}" if end != END else END for end in ends
+            ]
+            return ChannelWrite(
+                [ChannelWriteEntry(ch) for ch in channels], tags=[TAG_HIDDEN]
+            )
+
+        # add hidden start node
+        if start == START and start not in self.nodes:
+            self.nodes[start] = Channel.subscribe_to(START, tags=[TAG_HIDDEN])
+
+        # attach branch writer
+        self.nodes[start] |= branch.run(branch_writer)
+
+        # attach branch readers
+        ends = branch.ends.values() if branch.ends else [node for node in self.nodes]
+        for end in ends:
+            if end != END:
+                channel_name = f"branch:{start}:{name}:{end}"
+                self.channels[channel_name] = EphemeralValue(Any)
+                self.nodes[end].triggers.append(channel_name)
+                self.nodes[end].channels.append(channel_name)
+
     def get_graph(
         self, config: Optional[RunnableConfig] = None, *, xray: bool = False
     ) -> RunnableGraph:
+        """Returns a drawable representation of the computation graph."""
         graph = RunnableGraph()
         start_nodes: dict[str, RunnableGraphNode] = {
             START: graph.add_node(self.get_input_schema(config), START)
         }
         end_nodes: dict[str, RunnableGraphNode] = {
             END: graph.add_node(self.get_output_schema(config), END)
         }
@@ -271,43 +347,22 @@
                     n = graph.add_node(node, key)
                     start_nodes[key] = n
                     end_nodes[key] = n
             else:
                 n = graph.add_node(node, key)
                 start_nodes[key] = n
                 end_nodes[key] = n
-        for start, end in self.graph.edges:
+        for start, end in sorted(self.graph._all_edges):
             graph.add_edge(start_nodes[start], end_nodes[end])
         for start, branches in self.graph.branches.items():
-            for i, branch in enumerate(branches):
-                name = f"{start}_{branch.condition.__name__}"
-                if i > 0:
-                    name += f"_{i}"
-                cond = graph.add_node(
-                    RunnableLambda(branch.runnable, name=branch.condition.__name__),
-                    name,
-                )
+            for name, branch in branches.items():
+                name = f"{start}_{name}"
+                cond = graph.add_node(branch.condition, name)
                 graph.add_edge(start_nodes[start], cond)
                 ends = branch.ends or {
                     **{k: k for k in self.graph.nodes},
                     END: END,
                 }
                 for label, end in ends.items():
                     graph.add_edge(cond, end_nodes[end], label)
-        if self.graph.entry_point_branch:
-            cond = graph.add_node(
-                RunnableLambda(
-                    self.graph.entry_point_branch.runnable,
-                    name=self.graph.entry_point_branch.condition.__name__,
-                ),
-                f"{START}_condition",
-            )
-            graph.add_edge(start_nodes[START], cond)
-            ends = self.graph.entry_point_branch.ends or {
-                k: k for k in self.graph.nodes
-            }
-            for label, end in ends.items():
-                graph.add_edge(cond, end_nodes[end], label)
-        elif self.graph.entry_point:
-            graph.add_edge(start_nodes[START], end_nodes[self.graph.entry_point])
 
         return graph
```

### Comparing `gigagraph-0.0.26/langgraph/prebuilt/agent_executor.py` & `gigagraph-0.0.34/langgraph/prebuilt/agent_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import operator
 from typing import Annotated, Sequence, TypedDict, Union
 
 from langchain_core.agents import AgentAction, AgentFinish
 from langchain_core.messages import BaseMessage
-from langchain_core.runnables import RunnableLambda
 
 from langgraph.graph import END, StateGraph
 from langgraph.prebuilt.tool_executor import ToolExecutor
+from langgraph.utils import RunnableCallable
 
 
 def _get_agent_state(input_schema=None):
     if input_schema is None:
 
         class AgentState(TypedDict):
             # The input string
@@ -68,29 +68,41 @@
         agent_outcome = await agent_runnable.ainvoke(data)
         return {"agent_outcome": agent_outcome}
 
     # Define the function to execute tools
     def execute_tools(data):
         # Get the most recent agent_outcome - this is the key added in the `agent` above
         agent_action = data["agent_outcome"]
-        output = tool_executor.invoke(agent_action)
-        return {"intermediate_steps": [(agent_action, str(output))]}
+        if not isinstance(agent_action, list):
+            agent_action = [agent_action]
+        output = tool_executor.batch(agent_action, return_exceptions=True)
+        return {
+            "intermediate_steps": [
+                (action, str(out)) for action, out in zip(agent_action, output)
+            ]
+        }
 
     async def aexecute_tools(data):
         # Get the most recent agent_outcome - this is the key added in the `agent` above
         agent_action = data["agent_outcome"]
-        output = await tool_executor.ainvoke(agent_action)
-        return {"intermediate_steps": [(agent_action, str(output))]}
+        if not isinstance(agent_action, list):
+            agent_action = [agent_action]
+        output = await tool_executor.abatch(agent_action, return_exceptions=True)
+        return {
+            "intermediate_steps": [
+                (action, str(out)) for action, out in zip(agent_action, output)
+            ]
+        }
 
     # Define a new graph
     workflow = StateGraph(state)
 
     # Define the two nodes we will cycle between
-    workflow.add_node("agent", RunnableLambda(run_agent, arun_agent))
-    workflow.add_node("action", RunnableLambda(execute_tools, aexecute_tools))
+    workflow.add_node("agent", RunnableCallable(run_agent, arun_agent))
+    workflow.add_node("action", RunnableCallable(execute_tools, aexecute_tools))
 
     # Set the entrypoint as `agent`
     # This means that this node is the first one called
     workflow.set_entry_point("agent")
 
     # We now add a conditional edge
     workflow.add_conditional_edges(
```

### Comparing `gigagraph-0.0.26/langgraph/prebuilt/chat_agent_executor.py` & `gigagraph-0.0.34/langgraph/prebuilt/chat_agent_executor.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.26/langgraph/prebuilt/tool_executor.py` & `gigagraph-0.0.34/langgraph/prebuilt/tool_executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Any, Sequence, Union
 
 from langchain_core.load.serializable import Serializable
-from langchain_core.runnables import RunnableBinding, RunnableConfig, RunnableLambda
+from langchain_core.runnables import RunnableConfig
 from langchain_core.tools import BaseTool
 
+from langgraph.utils import RunnableCallable
+
 INVALID_TOOL_MSG_TEMPLATE = (
     "{requested_tool_name} is not a valid tool, "
     "try one of [{available_tool_names_str}]."
 )
 
 
 class ToolInvocationInterface:
@@ -22,53 +24,44 @@
 
     tool: str
     """The name of the Tool to execute."""
     tool_input: Union[str, dict]
     """The input to pass in to the Tool."""
 
 
-class ToolExecutor(RunnableBinding):
-    tools: Sequence[BaseTool]
-    tool_map: dict
-    invalid_tool_msg_template: str
-
+class ToolExecutor(RunnableCallable):
     def __init__(
         self,
         tools: Sequence[BaseTool],
         *,
         invalid_tool_msg_template: str = INVALID_TOOL_MSG_TEMPLATE,
-        **kwargs: Any,
     ) -> None:
-        bound = RunnableLambda(self._execute, afunc=self._aexecute)
-        super().__init__(
-            bound=bound,
-            tools=tools,
-            tool_map={t.name: t for t in tools},
-            invalid_tool_msg_template=invalid_tool_msg_template,
-            **kwargs,
-        )
+        super().__init__(self._execute, afunc=self._aexecute, trace=False)
+        self.tools = tools
+        self.tool_map = {t.name: t for t in tools}
+        self.invalid_tool_msg_template = invalid_tool_msg_template
 
     def _execute(
-        self, tool_invocation: ToolInvocationInterface, *, config: RunnableConfig
+        self, tool_invocation: ToolInvocationInterface, config: RunnableConfig
     ) -> Any:
         if tool_invocation.tool not in self.tool_map:
             return self.invalid_tool_msg_template.format(
                 requested_tool_name=tool_invocation.tool,
                 available_tool_names_str=", ".join([t.name for t in self.tools]),
             )
         else:
             tool = self.tool_map[tool_invocation.tool]
-            output = tool.invoke(tool_invocation.tool_input, config=config)
+            output = tool.invoke(tool_invocation.tool_input, config)
             return output
 
     async def _aexecute(
-        self, tool_invocation: ToolInvocationInterface, *, config: RunnableConfig
+        self, tool_invocation: ToolInvocationInterface, config: RunnableConfig
     ) -> Any:
         if tool_invocation.tool not in self.tool_map:
             return self.invalid_tool_msg_template.format(
                 requested_tool_name=tool_invocation.tool,
                 available_tool_names_str=", ".join([t.name for t in self.tools]),
             )
         else:
             tool = self.tool_map[tool_invocation.tool]
-            output = await tool.ainvoke(tool_invocation.tool_input, config=config)
+            output = await tool.ainvoke(tool_invocation.tool_input, config)
             return output
```

### Comparing `gigagraph-0.0.26/langgraph/pregel/__init__.py` & `gigagraph-0.0.34/langgraph/pregel/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,71 +6,86 @@
 from functools import partial
 from typing import (
     Any,
     AsyncIterator,
     Awaitable,
     Callable,
     Iterator,
+    Literal,
     Mapping,
-    NamedTuple,
     Optional,
     Sequence,
     Type,
     Union,
     cast,
     overload,
 )
 
-from langchain_core.callbacks.manager import (
-    AsyncCallbackManagerForChainRun,
-    CallbackManagerForChainRun,
-)
 from langchain_core.globals import get_debug
+from langchain_core.load.dump import dumpd
 from langchain_core.pydantic_v1 import BaseModel, Field, root_validator
 from langchain_core.runnables import (
     Runnable,
+    RunnableSequence,
     RunnableSerializable,
 )
 from langchain_core.runnables.base import Input, Output, coerce_to_runnable
 from langchain_core.runnables.config import (
     RunnableConfig,
+    ensure_config,
+    get_async_callback_manager_for_config,
+    get_callback_manager_for_config,
     get_executor_for_config,
+    merge_configs,
     patch_config,
 )
 from langchain_core.runnables.utils import (
     ConfigurableFieldSpec,
     create_model,
     get_unique_config_specs,
 )
 from langchain_core.tracers.log_stream import LogStreamCallbackHandler
+from typing_extensions import Self
 
-from langgraph.channels.any_value import AnyValue
 from langgraph.channels.base import (
     AsyncChannelsManager,
     BaseChannel,
     ChannelsManager,
     EmptyChannelError,
     InvalidUpdateError,
     create_checkpoint,
 )
-from langgraph.channels.ephemeral_value import EphemeralValue
 from langgraph.channels.last_value import LastValue
 from langgraph.checkpoint.base import (
     BaseCheckpointSaver,
     Checkpoint,
     CheckpointAt,
     copy_checkpoint,
     empty_checkpoint,
 )
-from langgraph.constants import CONFIG_KEY_READ, CONFIG_KEY_SEND, INTERRUPT
+from langgraph.constants import (
+    CONFIG_KEY_READ,
+    CONFIG_KEY_SEND,
+    INTERRUPT,
+)
 from langgraph.pregel.debug import print_checkpoint, print_step_start
-from langgraph.pregel.io import map_input, map_output
+from langgraph.pregel.io import (
+    map_input,
+    map_output_updates,
+    map_output_values,
+    read_channel,
+    read_channels,
+)
 from langgraph.pregel.log import logger
-from langgraph.pregel.read import ChannelBatch, ChannelInvoke
-from langgraph.pregel.reserved import AllReservedChannels, ReservedChannels
+from langgraph.pregel.read import PregelNode
+from langgraph.pregel.types import (
+    PregelExecutableTask,
+    PregelTaskDescription,
+    StateSnapshot,
+)
 from langgraph.pregel.validate import validate_graph, validate_keys
 from langgraph.pregel.write import ChannelWrite, ChannelWriteEntry
 
 WriteValue = Union[
     Runnable[Input, Output],
     Callable[[Input], Output],
     Callable[[Input], Awaitable[Output]],
@@ -92,137 +107,146 @@
     @overload
     @classmethod
     def subscribe_to(
         cls,
         channels: str,
         *,
         key: Optional[str] = None,
-        when: Optional[Callable[[Any], bool]] = None,
         tags: Optional[list[str]] = None,
-    ) -> ChannelInvoke:
+    ) -> PregelNode:
         ...
 
     @overload
     @classmethod
     def subscribe_to(
         cls,
         channels: Sequence[str],
         *,
         key: None = None,
-        when: Optional[Callable[[Any], bool]] = None,
         tags: Optional[list[str]] = None,
-    ) -> ChannelInvoke:
+    ) -> PregelNode:
         ...
 
     @classmethod
     def subscribe_to(
         cls,
         channels: Union[str, Sequence[str]],
         *,
         key: Optional[str] = None,
-        when: Optional[Callable[[Any], bool]] = None,
         tags: Optional[list[str]] = None,
-    ) -> ChannelInvoke:
+    ) -> PregelNode:
         """Runs process.invoke() each time channels are updated,
         with a dict of the channel values as input."""
         if not isinstance(channels, str) and key is not None:
             raise ValueError(
                 "Can't specify a key when subscribing to multiple channels"
             )
-        return ChannelInvoke(
+        return PregelNode(
             channels=cast(
                 Union[Mapping[None, str], Mapping[str, str]],
                 {key: channels}
+                if isinstance(channels, str) and key is not None
+                else [channels]
                 if isinstance(channels, str)
                 else {chan: chan for chan in channels},
             ),
             triggers=[channels] if isinstance(channels, str) else channels,
-            when=when,
             tags=tags,
         )
 
     @classmethod
-    def subscribe_to_each(cls, inbox: str, key: Optional[str] = None) -> ChannelBatch:
-        """Runs process.batch() with the content of inbox each time it is updated."""
-        return ChannelBatch(channel=inbox, key=key)
-
-    @classmethod
     def write_to(
         cls,
         *channels: str,
         **kwargs: WriteValue,
     ) -> ChannelWrite:
         """Writes to channels the result of the lambda, or None to skip writing."""
         return ChannelWrite(
-            channels=(
-                [ChannelWriteEntry(c, None, False) for c in channels]
-                + [
-                    ChannelWriteEntry(k, _coerce_write_value(v), True)
-                    for k, v in kwargs.items()
-                ]
-            )
+            [ChannelWriteEntry(c) for c in channels]
+            + [
+                ChannelWriteEntry(k, _coerce_write_value(v), True)
+                for k, v in kwargs.items()
+            ]
         )
 
 
-class StateSnapshot(NamedTuple):
-    values: dict[str, Any] | Any
-    """Current values of channels"""
-    next: tuple[str]
-    """Nodes to execute in the next step, if any"""
+StreamMode = Literal["values", "updates"]
 
 
 class Pregel(
     RunnableSerializable[Union[dict[str, Any], Any], Union[dict[str, Any], Any]]
 ):
-    nodes: Mapping[str, Union[ChannelInvoke, ChannelBatch]]
+    nodes: Mapping[str, PregelNode]
 
     channels: Mapping[str, BaseChannel] = Field(default_factory=dict)
 
-    # TODO Rename to `output_channels`
-    output: Union[str, Sequence[str]] = "output"
+    default_channel_cls: Type[BaseChannel] = Field(default=LastValue)
+
+    auto_validate: bool = True
 
-    # TODO Replace with `stream_channels`
-    hidden: Sequence[str] = Field(default_factory=list)
+    stream_mode: StreamMode = "values"
 
-    snapshot_channels: Union[str, Sequence[str]] = Field(default_factory=list)
+    output_channels: Union[str, Sequence[str]] = "output"
+    """Channels to output, defaults to channel named 'output'."""
+
+    stream_channels: Optional[Union[str, Sequence[str]]] = None
+    """Channels to stream, defaults to all channels not in reserved channels"""
 
     interrupt_after_nodes: Sequence[str] = Field(default_factory=list)
 
     interrupt_before_nodes: Sequence[str] = Field(default_factory=list)
 
-    # TODO Rename to `input_channels`
-    input: Union[str, Sequence[str]] = "input"
+    input_channels: Union[str, Sequence[str]] = "input"
 
     step_timeout: Optional[float] = None
 
     debug: bool = Field(default_factory=get_debug)
 
     checkpointer: Optional[BaseCheckpointSaver] = None
 
     name: str = "LangGraph"
 
     class Config:
         arbitrary_types_allowed = True
 
     @root_validator(skip_on_failure=True)
-    def validate_pregel(cls, values: dict[str, Any]) -> dict[str, Any]:
+    def validate_on_init(cls, values: dict[str, Any]) -> dict[str, Any]:
+        if not values["auto_validate"]:
+            return values
         validate_graph(
             values["nodes"],
             values["channels"],
-            values["input"],
-            values["output"],
-            values["hidden"],
+            values["input_channels"],
+            values["output_channels"],
+            values["stream_channels"],
             values["interrupt_after_nodes"],
             values["interrupt_before_nodes"],
+            values["default_channel_cls"],
         )
         if values["interrupt_after_nodes"] or values["interrupt_before_nodes"]:
             if not values["checkpointer"]:
                 raise ValueError("Interrupts require a checkpointer")
         return values
 
+    def validate(self) -> Self:
+        validate_graph(
+            self.nodes,
+            self.channels,
+            self.input_channels,
+            self.output_channels,
+            self.stream_channels,
+            self.interrupt_after_nodes,
+            self.interrupt_before_nodes,
+            self.default_channel_cls,
+        )
+        if self.interrupt_after_nodes or self.interrupt_before_nodes:
+            if not self.checkpointer:
+                raise ValueError("Interrupts require a checkpointer")
+        return self
+
     @property
     def config_specs(self) -> list[ConfigurableFieldSpec]:
         return [
             spec
             for spec in get_unique_config_specs(
                 [spec for node in self.nodes.values() for spec in node.config_specs]
                 + (
@@ -233,267 +257,420 @@
             )
             # these are provided by the Pregel class
             if spec.id not in [CONFIG_KEY_READ, CONFIG_KEY_SEND]
         ]
 
     @property
     def InputType(self) -> Any:
-        if isinstance(self.input, str):
-            return self.channels[self.input].UpdateType
+        if isinstance(self.input_channels, str):
+            return self.channels[self.input_channels].UpdateType
 
     def get_input_schema(
         self, config: Optional[RunnableConfig] = None
     ) -> Type[BaseModel]:
-        if isinstance(self.input, str):
+        if isinstance(self.input_channels, str):
             return super().get_input_schema(config)
         else:
             return create_model(  # type: ignore[call-overload]
                 self.get_name("Input"),
                 **{
                     k: (self.channels[k].UpdateType, None)
-                    for k in self.input or self.channels.keys()
+                    for k in self.input_channels or self.channels.keys()
                 },
             )
 
     @property
     def OutputType(self) -> Any:
-        if isinstance(self.output, str):
-            return self.channels[self.output].ValueType
+        if isinstance(self.output_channels, str):
+            return self.channels[self.output_channels].ValueType
 
     def get_output_schema(
         self, config: Optional[RunnableConfig] = None
     ) -> Type[BaseModel]:
-        if isinstance(self.output, str):
+        if isinstance(self.output_channels, str):
             return super().get_output_schema(config)
         else:
             return create_model(  # type: ignore[call-overload]
                 self.get_name("Output"),
-                **{k: (self.channels[k].ValueType, None) for k in self.output},
+                **{k: (self.channels[k].ValueType, None) for k in self.output_channels},
             )
 
     @property
-    def snapshot_channels_list(self) -> Sequence[str]:
+    def stream_channels_list(self) -> Sequence[str]:
         return (
-            [self.snapshot_channels]
-            if isinstance(self.snapshot_channels, str)
-            else self.snapshot_channels
-            or [k for k in self.channels if k not in AllReservedChannels]
+            [self.stream_channels]
+            if isinstance(self.stream_channels, str)
+            else self.stream_channels or [k for k in self.channels]
         )
 
     def get_state(self, config: RunnableConfig) -> StateSnapshot:
         if not self.checkpointer:
             raise ValueError("No checkpointer set")
 
-        checkpoint = self.checkpointer.get(config)
-        checkpoint = checkpoint or empty_checkpoint()
+        saved = self.checkpointer.get_tuple(config)
+        checkpoint = saved.checkpoint if saved else empty_checkpoint()
+        config = saved.config if saved else config
         with ChannelsManager(self.channels, checkpoint) as channels:
             _, next_tasks = _prepare_next_tasks(
-                checkpoint, self.nodes, channels, update_seen=False
+                checkpoint, self.nodes, channels, for_execution=False
             )
-            values = {
-                k: _read_channel(channels, k)
-                for k in channels
-                if k in self.snapshot_channels_list
-            }
+            values = read_channels(channels, self.stream_channels_list)
             return StateSnapshot(
-                values[self.snapshot_channels]
-                if isinstance(self.snapshot_channels, str)
+                values[self.stream_channels]
+                if isinstance(self.stream_channels, str)
                 else values,
-                tuple(name for _, _, name in next_tasks),
+                tuple(name for name, _ in next_tasks),
+                config,
             )
 
     async def aget_state(self, config: RunnableConfig) -> StateSnapshot:
         if not self.checkpointer:
             raise ValueError("No checkpointer set")
 
-        checkpoint = await self.checkpointer.aget(config)
-        checkpoint = checkpoint or empty_checkpoint()
+        saved = await self.checkpointer.aget_tuple(config)
+        checkpoint = saved.checkpoint if saved else empty_checkpoint()
+        config = saved.config if saved else config
         async with AsyncChannelsManager(self.channels, checkpoint) as channels:
             _, next_tasks = _prepare_next_tasks(
-                checkpoint, self.nodes, channels, update_seen=False
+                checkpoint, self.nodes, channels, for_execution=False
             )
-            values = {
-                k: _read_channel(channels, k)
-                for k in channels
-                if k in self.snapshot_channels_list
-            }
+            values = read_channels(channels, self.stream_channels_list)
             return StateSnapshot(
-                values[self.snapshot_channels]
-                if isinstance(self.snapshot_channels, str)
+                values[self.stream_channels]
+                if isinstance(self.stream_channels, str)
                 else values,
-                tuple(name for _, _, name in next_tasks),
+                tuple(name for name, _ in next_tasks),
+                config,
             )
 
+    def get_state_history(self, config: RunnableConfig) -> Iterator[StateSnapshot]:
+        if not self.checkpointer:
+            raise ValueError("No checkpointer set")
+
+        for config, checkpoint, parent_config in self.checkpointer.list(config):
+            with ChannelsManager(self.channels, checkpoint) as channels:
+                _, next_tasks = _prepare_next_tasks(
+                    checkpoint, self.nodes, channels, for_execution=False
+                )
+                values = read_channels(channels, self.stream_channels_list)
+                yield StateSnapshot(
+                    values[self.stream_channels]
+                    if isinstance(self.stream_channels, str)
+                    else values,
+                    tuple(name for name, _ in next_tasks),
+                    config,
+                    parent_config,
+                )
+
+    async def aget_state_history(
+        self, config: RunnableConfig
+    ) -> AsyncIterator[StateSnapshot]:
+        if not self.checkpointer:
+            raise ValueError("No checkpointer set")
+
+        async for config, checkpoint, parent_config in self.checkpointer.alist(config):
+            async with AsyncChannelsManager(self.channels, checkpoint) as channels:
+                _, next_tasks = _prepare_next_tasks(
+                    checkpoint, self.nodes, channels, for_execution=False
+                )
+                values = read_channels(channels, self.stream_channels_list)
+                yield StateSnapshot(
+                    values[self.stream_channels]
+                    if isinstance(self.stream_channels, str)
+                    else values,
+                    tuple(name for name, _ in next_tasks),
+                    config,
+                    parent_config,
+                )
+
     def update_state(
-        self, config: RunnableConfig, values: dict[str, Any] | Any
-    ) -> None:
+        self,
+        config: RunnableConfig,
+        values: dict[str, Any] | Any,
+        as_node: Optional[str] = None,
+    ) -> RunnableConfig:
+        """Update the state of the graph with the given values, as if they came from
+        node `as_node`. If `as_node` is not provided, it will be set to the last node
+        that updated the state, if not ambiguous.
+        """
         if not self.checkpointer:
             raise ValueError("No checkpointer set")
 
-        values = (
-            {self.snapshot_channels: values}
-            if isinstance(self.snapshot_channels, str)
-            else values
-        )
+        # get last checkpoint
         checkpoint = self.checkpointer.get(config)
         checkpoint = copy_checkpoint(checkpoint) if checkpoint else empty_checkpoint()
+        # find last node that updated the state, if not provided
+        if as_node is None:
+            last_seen_by_node = sorted(
+                (v, n)
+                for n, seen in checkpoint["versions_seen"].items()
+                for v in seen.values()
+            )
+            # if two nodes updated the state at the same time, it's ambiguous
+            if last_seen_by_node:
+                if len(last_seen_by_node) == 1:
+                    as_node = last_seen_by_node[0][1]
+                elif last_seen_by_node[-1][0] != last_seen_by_node[-2][0]:
+                    as_node = last_seen_by_node[-1][1]
+        if as_node is None:
+            raise InvalidUpdateError("Ambiguous update, specify as_node")
+        # update channels
         with ChannelsManager(self.channels, checkpoint) as channels:
-            for k, v in values.items():
-                channels[k].update([v])
-                checkpoint["channel_versions"][k] += 1
-            for k in self.snapshot_channels or self.channels:
-                version = checkpoint["channel_versions"][k]
-                checkpoint["versions_seen"][INTERRUPT][k] = version
-            self.checkpointer.put(config, create_checkpoint(checkpoint, channels))
+            # create task to run all writers of the chosen node
+            writers = self.nodes[as_node].get_writers()
+            if not writers:
+                raise InvalidUpdateError(f"Node {as_node} has no writers")
+            task = PregelExecutableTask(
+                as_node,
+                values,
+                RunnableSequence(*writers) if len(writers) > 1 else writers[0],
+                deque(),
+            )
+            # execute task
+            task.proc.invoke(
+                task.input,
+                patch_config(
+                    config,
+                    run_name=self.name + "UpdateState",
+                    configurable={
+                        # deque.extend is thread-safe
+                        CONFIG_KEY_SEND: task.writes.extend,
+                        CONFIG_KEY_READ: partial(
+                            _local_read, checkpoint, channels, task.writes
+                        ),
+                    },
+                ),
+            )
+            # apply to checkpoint and save
+            _apply_writes(checkpoint, channels, task.writes)
+            return self.checkpointer.put(
+                config, create_checkpoint(checkpoint, channels)
+            )
 
     async def aupdate_state(
-        self, config: RunnableConfig, values: dict[str, Any] | Any
-    ) -> None:
+        self,
+        config: RunnableConfig,
+        values: dict[str, Any] | Any,
+        as_node: Optional[str] = None,
+    ) -> RunnableConfig:
         if not self.checkpointer:
             raise ValueError("No checkpointer set")
 
-        values = (
-            {self.snapshot_channels: values}
-            if isinstance(self.snapshot_channels, str)
-            else values
-        )
+        # get last checkpoint
         checkpoint = await self.checkpointer.aget(config)
         checkpoint = copy_checkpoint(checkpoint) if checkpoint else empty_checkpoint()
+        # find last node that updated the state, if not provided
+        if as_node is None:
+            last_seen_by_node = sorted(
+                (v, n)
+                for n, seen in checkpoint["versions_seen"].items()
+                for v in seen.values()
+            )
+            # if two nodes updated the state at the same time, it's ambiguous
+            if last_seen_by_node:
+                if len(last_seen_by_node) == 1:
+                    as_node = last_seen_by_node[0][1]
+                elif last_seen_by_node[-1][0] != last_seen_by_node[-2][0]:
+                    as_node = last_seen_by_node[-1][1]
+        if as_node is None:
+            raise InvalidUpdateError("Ambiguous update, specify as_node")
+        # update channels, acting as the chosen node
         async with AsyncChannelsManager(self.channels, checkpoint) as channels:
-            for k, v in values.items():
-                channels[k].update([v])
-                checkpoint["channel_versions"][k] += 1
-            for k in self.snapshot_channels or self.channels:
-                version = checkpoint["channel_versions"][k]
-                checkpoint["versions_seen"][INTERRUPT][k] = version
-            await self.checkpointer.aput(
+            # create task to run all writers of the chosen node
+            writers = self.nodes[as_node].get_writers()
+            if not writers:
+                raise InvalidUpdateError(f"Node {as_node} has no writers")
+            task = PregelExecutableTask(
+                as_node,
+                values,
+                RunnableSequence(*writers) if len(writers) > 1 else writers[0],
+                deque(),
+            )
+            # execute task
+            await task.proc.ainvoke(
+                task.input,
+                patch_config(
+                    config,
+                    run_name=self.name + "UpdateState",
+                    configurable={
+                        # deque.extend is thread-safe
+                        CONFIG_KEY_SEND: task.writes.extend,
+                        CONFIG_KEY_READ: partial(
+                            _local_read, checkpoint, channels, task.writes
+                        ),
+                    },
+                ),
+            )
+            # apply to checkpoint and save
+            _apply_writes(checkpoint, channels, task.writes)
+            return await self.checkpointer.aput(
                 config, create_checkpoint(checkpoint, channels)
             )
 
     def _defaults(
         self,
         *,
+        stream_mode: Optional[StreamMode] = None,
         input_keys: Optional[Union[str, Sequence[str]]] = None,
         output_keys: Optional[Union[str, Sequence[str]]] = None,
         interrupt_before_nodes: Optional[Sequence[str]] = None,
         interrupt_after_nodes: Optional[Sequence[str]] = None,
         debug: Optional[bool] = None,
     ) -> tuple[
         bool,
+        StreamMode,
         Union[str, Sequence[str]],
         Union[str, Sequence[str]],
         Optional[Sequence[str]],
         Optional[Sequence[str]],
     ]:
         debug = debug if debug is not None else self.debug
         if output_keys is None:
-            output_keys = [chan for chan in self.channels if chan not in self.hidden]
+            output_keys = (
+                [chan for chan in self.channels]
+                if self.stream_channels is None
+                else self.stream_channels
+            )
         else:
             validate_keys(output_keys, self.channels)
         if input_keys is None:
-            input_keys = self.input
+            input_keys = self.input_channels
         else:
             validate_keys(input_keys, self.channels)
         interrupt_before_nodes = interrupt_before_nodes or self.interrupt_before_nodes
         interrupt_after_nodes = interrupt_after_nodes or self.interrupt_after_nodes
         return (
             debug,
+            stream_mode if stream_mode is not None else self.stream_mode,
             input_keys,
             output_keys,
             interrupt_before_nodes,
             interrupt_after_nodes,
         )
 
-    def _transform(
+    def stream(
         self,
-        input: Iterator[Union[dict[str, Any], Any]],
-        run_manager: CallbackManagerForChainRun,
-        config: RunnableConfig,
-        **kwargs: Any,
+        input: Union[dict[str, Any], Any],
+        config: Optional[RunnableConfig] = None,
+        *,
+        stream_mode: Optional[StreamMode] = None,
+        output_keys: Optional[Union[str, Sequence[str]]] = None,
+        input_keys: Optional[Union[str, Sequence[str]]] = None,
+        interrupt_before_nodes: Optional[Sequence[str]] = None,
+        interrupt_after_nodes: Optional[Sequence[str]] = None,
+        debug: Optional[bool] = None,
     ) -> Iterator[Union[dict[str, Any], Any]]:
+        config = ensure_config(config)
+        callback_manager = get_callback_manager_for_config(config)
+        run_manager = callback_manager.on_chain_start(
+            dumpd(self), input, name=config.get("run_name", self.get_name())
+        )
         try:
             if config["recursion_limit"] < 1:
                 raise ValueError("recursion_limit must be at least 1")
             # assign defaults
             (
                 debug,
+                stream_mode,
                 input_keys,
                 output_keys,
                 interrupt_before_nodes,
                 interrupt_after_nodes,
-            ) = self._defaults(**kwargs)
+            ) = self._defaults(
+                stream_mode=stream_mode,
+                input_keys=input_keys,
+                output_keys=output_keys,
+                interrupt_before_nodes=interrupt_before_nodes,
+                interrupt_after_nodes=interrupt_after_nodes,
+                debug=debug,
+            )
             # copy nodes to ignore mutations during execution
             processes = {**self.nodes}
             # get checkpoint from saver, or create an empty one
-            checkpoint = self.checkpointer.get(config) if self.checkpointer else None
+            checkpoint_config = config
+            checkpoint = (
+                self.checkpointer.get(checkpoint_config) if self.checkpointer else None
+            )
             checkpoint = checkpoint or empty_checkpoint()
             # create channels from checkpoint
             with ChannelsManager(
                 self.channels, checkpoint
             ) as channels, get_executor_for_config(config) as executor:
                 # map inputs to channel updates
-                if input_writes := deque(
-                    w for c in input for w in map_input(input_keys, c)
-                ):
+                if input_writes := deque(map_input(input_keys, input)):
                     # discard any unfinished tasks from previous checkpoint
-                    checkpoint, _ = _prepare_next_tasks(checkpoint, processes, channels)
-                    # apply input writes
-                    _apply_writes(
-                        checkpoint,
-                        channels,
-                        input_writes,
-                        config,
-                        0,
+                    checkpoint, _ = _prepare_next_tasks(
+                        checkpoint, processes, channels, for_execution=True
                     )
-
-                read = partial(_read_channel, channels)
+                    # apply input writes
+                    _apply_writes(checkpoint, channels, input_writes)
+                else:
+                    # if received no input, take that as signal to proceed
+                    # past previous interrupt, if any
+                    checkpoint = copy_checkpoint(checkpoint)
+                    for k in self.stream_channels_list:
+                        version = checkpoint["channel_versions"][k]
+                        checkpoint["versions_seen"][INTERRUPT][k] = version
 
                 # Similarly to Bulk Synchronous Parallel / Pregel model
                 # computation proceeds in steps, while there are channel updates
                 # channel updates from step N are only visible in step N+1
                 # channels are guaranteed to be immutable for the duration of the step,
                 # with channel updates applied only at the transition between steps
                 for step in range(config["recursion_limit"] + 1):
-                    checkpoint, next_tasks = _prepare_next_tasks(
-                        checkpoint, processes, channels
+                    next_checkpoint, next_tasks = _prepare_next_tasks(
+                        checkpoint, processes, channels, for_execution=True
                     )
 
                     # if no more tasks, we're done
                     if not next_tasks:
-                        break
+                        if step == 0:
+                            raise ValueError("No tasks to run in graph.")
+                        else:
+                            break
                     elif step == config["recursion_limit"]:
                         raise GraphRecursionError(
                             f"Recursion limit of {config['recursion_limit']} reached"
-                            "without hitting a stop condition. You can increase the limit"
-                            "by setting the `recursion_limit` config key."
+                            "without hitting a stop condition. You can increase the "
+                            "limit by setting the `recursion_limit` config key."
                         )
 
+                    # before execution, check if we should interrupt
+                    if _should_interrupt(
+                        checkpoint,
+                        interrupt_before_nodes,
+                        self.stream_channels_list,
+                        next_tasks,
+                    ):
+                        break
+                    else:
+                        checkpoint = next_checkpoint
+
                     if debug:
                         print_step_start(step, next_tasks)
 
-                    # collect all writes to channels, without applying them yet
-                    pending_writes = deque[tuple[str, Any]]()
-
                     # prepare tasks with config
                     tasks_w_config = [
                         (
                             proc,
                             input,
                             patch_config(
-                                config,
+                                merge_configs(config, proc_config),
                                 run_name=name,
                                 callbacks=run_manager.get_child(f"graph:step:{step}"),
                                 configurable={
                                     # deque.extend is thread-safe
-                                    CONFIG_KEY_SEND: pending_writes.extend,
-                                    CONFIG_KEY_READ: read,
+                                    CONFIG_KEY_SEND: writes.extend,
+                                    CONFIG_KEY_READ: partial(
+                                        _local_read, checkpoint, channels, writes
+                                    ),
                                 },
                             ),
                         )
-                        for proc, input, name in next_tasks
+                        for name, input, proc, writes, proc_config in next_tasks
                     ]
 
                     futures = [
                         executor.submit(proc.invoke, input, config)
                         for proc, input, config in tasks_w_config
                     ]
 
@@ -504,168 +681,203 @@
                         return_when=concurrent.futures.FIRST_EXCEPTION,
                         timeout=self.step_timeout,
                     )
 
                     # panic on failure or timeout
                     _panic_or_proceed(done, inflight, step)
 
+                    # combine pending writes from all tasks
+                    pending_writes = deque[tuple[str, Any]]()
+                    for _, _, _, writes, _ in next_tasks:
+                        pending_writes.extend(writes)
+
                     # apply writes to channels
-                    _apply_writes(
-                        checkpoint, channels, pending_writes, config, step + 1
-                    )
+                    _apply_writes(checkpoint, channels, pending_writes)
 
                     if debug:
                         print_checkpoint(step, channels)
 
-                    # yield current value and checkpoint view
-                    if step_output := map_output(output_keys, pending_writes, channels):
-                        yield step_output
-                        # we can detect updates when output is multiple channels (ie. dict)
-                        if not isinstance(output_keys, str):
-                            # if view was updated, apply writes to channels
-                            _apply_writes_from_view(checkpoint, channels, step_output)
-
-                    # with previous step's checkpoint
-                    if do_interrupt_before := _should_interrupt(
-                        checkpoint,
-                        interrupt_before_nodes,
-                        self.snapshot_channels_list,
-                        pending_writes,
-                    ):
-                        break
+                    # yield current value or updates
+                    if stream_mode == "values":
+                        if step_output := map_output_values(
+                            output_keys, pending_writes, channels
+                        ):
+                            yield step_output
+                    else:
+                        if step_output := map_output_updates(output_keys, next_tasks):
+                            yield step_output
 
                     # save end of step checkpoint
                     if self.checkpointer is not None and (
                         self.checkpointer.at == CheckpointAt.END_OF_STEP
-                        or interrupt_before_nodes
                     ):
                         checkpoint = create_checkpoint(checkpoint, channels)
-                        self.checkpointer.put(config, checkpoint)
+                        checkpoint_config = self.checkpointer.put(
+                            checkpoint_config, checkpoint
+                        )
 
-                    # with this step's checkpoint,
+                    # after execution, check if we should interrupt
                     if _should_interrupt(
                         checkpoint,
                         interrupt_after_nodes,
-                        self.snapshot_channels_list,
-                        pending_writes,
+                        self.stream_channels_list,
+                        next_tasks,
                     ):
                         break
 
+                # set final channel values as run output
+                run_manager.on_chain_end(read_channels(channels, output_keys))
+
                 # save end of run checkpoint
                 if (
                     self.checkpointer is not None
                     and self.checkpointer.at == CheckpointAt.END_OF_RUN
-                    and not do_interrupt_before
                 ):
                     checkpoint = create_checkpoint(checkpoint, channels)
-                    self.checkpointer.put(config, checkpoint)
+                    self.checkpointer.put(checkpoint_config, checkpoint)
+        except BaseException as e:
+            run_manager.on_chain_error(e)
+            raise
         finally:
             # cancel any pending tasks when generator is interrupted
             try:
                 for task in futures:
                     task.cancel()
             except NameError:
                 pass
 
-    async def _atransform(
+    async def astream(
         self,
-        input: AsyncIterator[Union[dict[str, Any], Any]],
-        run_manager: AsyncCallbackManagerForChainRun,
-        config: RunnableConfig,
-        **kwargs: Any,
+        input: Union[dict[str, Any], Any],
+        config: Optional[RunnableConfig] = None,
+        *,
+        stream_mode: Optional[StreamMode] = None,
+        output_keys: Optional[Union[str, Sequence[str]]] = None,
+        input_keys: Optional[Union[str, Sequence[str]]] = None,
+        interrupt_before_nodes: Optional[Sequence[str]] = None,
+        interrupt_after_nodes: Optional[Sequence[str]] = None,
+        debug: Optional[bool] = None,
     ) -> AsyncIterator[Union[dict[str, Any], Any]]:
+        config = ensure_config(config)
+        callback_manager = get_async_callback_manager_for_config(config)
+        run_manager = await callback_manager.on_chain_start(
+            dumpd(self), input, name=config.get("run_name", self.get_name())
+        )
+        # if running from astream_log() run each proc with streaming
+        do_stream = next(
+            (
+                h
+                for h in run_manager.handlers
+                if isinstance(h, LogStreamCallbackHandler)
+            ),
+            None,
+        )
         try:
             if config["recursion_limit"] < 1:
                 raise ValueError("recursion_limit must be at least 1")
-            # if running from astream_log() run each proc with streaming
-            do_stream = next(
-                (
-                    h
-                    for h in run_manager.handlers
-                    if isinstance(h, LogStreamCallbackHandler)
-                ),
-                None,
-            )
             # assign defaults
             (
                 debug,
+                stream_mode,
                 input_keys,
                 output_keys,
                 interrupt_before_nodes,
                 interrupt_after_nodes,
-            ) = self._defaults(**kwargs)
+            ) = self._defaults(
+                stream_mode=stream_mode,
+                input_keys=input_keys,
+                output_keys=output_keys,
+                interrupt_before_nodes=interrupt_before_nodes,
+                interrupt_after_nodes=interrupt_after_nodes,
+                debug=debug,
+            )
             # copy nodes to ignore mutations during execution
             processes = {**self.nodes}
             # get checkpoint from saver, or create an empty one
+            checkpoint_config = config
             checkpoint = (
-                await self.checkpointer.aget(config) if self.checkpointer else None
+                await self.checkpointer.aget(checkpoint_config)
+                if self.checkpointer
+                else None
             )
             checkpoint = checkpoint or empty_checkpoint()
             # create channels from checkpoint
             async with AsyncChannelsManager(self.channels, checkpoint) as channels:
                 # map inputs to channel updates
-                if input_writes := deque(
-                    [w async for c in input for w in map_input(input_keys, c)]
-                ):
+                if input_writes := deque(map_input(input_keys, input)):
                     # discard any unfinished tasks from previous checkpoint
-                    checkpoint, _ = _prepare_next_tasks(checkpoint, processes, channels)
-                    # apply input writes
-                    _apply_writes(
-                        checkpoint,
-                        channels,
-                        input_writes,
-                        config,
-                        0,
+                    checkpoint, _ = _prepare_next_tasks(
+                        checkpoint, processes, channels, for_execution=True
                     )
-
-                read = partial(_read_channel, channels)
+                    # apply input writes
+                    _apply_writes(checkpoint, channels, input_writes)
+                else:
+                    # if received no input, take that as signal to proceed
+                    # past previous interrupt, if any
+                    checkpoint = copy_checkpoint(checkpoint)
+                    for k in self.stream_channels_list:
+                        version = checkpoint["channel_versions"][k]
+                        checkpoint["versions_seen"][INTERRUPT][k] = version
 
                 # Similarly to Bulk Synchronous Parallel / Pregel model
                 # computation proceeds in steps, while there are channel updates
                 # channel updates from step N are only visible in step N+1,
                 # channels are guaranteed to be immutable for the duration of the step,
                 # channel updates being applied only at the transition between steps
                 for step in range(config["recursion_limit"] + 1):
-                    checkpoint, next_tasks = _prepare_next_tasks(
-                        checkpoint, processes, channels
+                    next_checkpoint, next_tasks = _prepare_next_tasks(
+                        checkpoint, processes, channels, for_execution=True
                     )
 
                     # if no more tasks, we're done
                     if not next_tasks:
-                        break
+                        if step == 0:
+                            raise ValueError("No tasks to run in graph.")
+                        else:
+                            break
                     elif step == config["recursion_limit"]:
                         raise GraphRecursionError(
                             f"Recursion limit of {config['recursion_limit']} reached"
                             "without hitting a stop condition. You can increase the limit"
                             "by setting the `recursion_limit` config key."
                         )
 
+                    # before execution, check if we should interrupt
+                    if _should_interrupt(
+                        checkpoint,
+                        interrupt_before_nodes,
+                        self.stream_channels_list,
+                        next_tasks,
+                    ):
+                        break
+                    else:
+                        checkpoint = next_checkpoint
+
                     if debug:
                         print_step_start(step, next_tasks)
 
-                    # collect all writes to channels, without applying them yet
-                    pending_writes = deque[tuple[str, Any]]()
-
                     # prepare tasks with config
                     tasks_w_config = [
                         (
                             proc,
                             input,
                             patch_config(
-                                config,
+                                merge_configs(config, proc_config),
                                 run_name=name,
                                 callbacks=run_manager.get_child(f"graph:step:{step}"),
                                 configurable={
                                     # deque.extend is thread-safe
-                                    CONFIG_KEY_SEND: pending_writes.extend,
-                                    CONFIG_KEY_READ: read,
+                                    CONFIG_KEY_SEND: writes.extend,
+                                    CONFIG_KEY_READ: partial(
+                                        _local_read, checkpoint, channels, writes
+                                    ),
                                 },
                             ),
                         )
-                        for proc, input, name in next_tasks
+                        for name, input, proc, writes, proc_config in next_tasks
                     ]
 
                     futures = (
                         [
                             asyncio.create_task(_aconsume(proc.astream(input, config)))
                             for proc, input, config in tasks_w_config
                         ]
@@ -683,223 +895,151 @@
                         return_when=asyncio.FIRST_EXCEPTION,
                         timeout=self.step_timeout,
                     )
 
                     # panic on failure or timeout
                     _panic_or_proceed(done, inflight, step)
 
+                    # combine pending writes from all tasks
+                    pending_writes = deque[tuple[str, Any]]()
+                    for _, _, _, writes, _ in next_tasks:
+                        pending_writes.extend(writes)
+
                     # apply writes to channels
-                    _apply_writes(
-                        checkpoint, channels, pending_writes, config, step + 1
-                    )
+                    _apply_writes(checkpoint, channels, pending_writes)
 
                     if debug:
                         print_checkpoint(step, channels)
 
-                    # yield current value and checkpoint view
-                    if step_output := map_output(output_keys, pending_writes, channels):
-                        yield step_output
-                        # we can detect updates when output is multiple channels (ie. dict)
-                        if not isinstance(output_keys, str):
-                            # if view was updated, apply writes to channels
-                            _apply_writes_from_view(checkpoint, channels, step_output)
-
-                    # with previous step's checkpoint
-                    if do_interrupt_before := _should_interrupt(
-                        checkpoint,
-                        interrupt_before_nodes,
-                        self.snapshot_channels_list,
-                        pending_writes,
-                    ):
-                        break
+                    # yield current value or updates
+                    if stream_mode == "values":
+                        if step_output := map_output_values(
+                            output_keys, pending_writes, channels
+                        ):
+                            yield step_output
+                    else:
+                        if step_output := map_output_updates(output_keys, next_tasks):
+                            yield step_output
 
                     # save end of step checkpoint
-                    if (
-                        self.checkpointer is not None
-                        and self.checkpointer.at == CheckpointAt.END_OF_STEP
+                    if self.checkpointer is not None and (
+                        self.checkpointer.at == CheckpointAt.END_OF_STEP
                     ):
                         checkpoint = create_checkpoint(checkpoint, channels)
-                        await self.checkpointer.aput(config, checkpoint)
+                        checkpoint_config = await self.checkpointer.aput(
+                            checkpoint_config, checkpoint
+                        )
 
-                    # with this step's checkpoint
+                    # after execution, check if we should interrupt
                     if _should_interrupt(
                         checkpoint,
                         interrupt_after_nodes,
-                        self.snapshot_channels_list,
-                        pending_writes,
+                        self.stream_channels_list,
+                        next_tasks,
                     ):
                         break
 
+                # set final channel values as run output
+                await run_manager.on_chain_end(read_channels(channels, output_keys))
+
                 # save end of run checkpoint
                 if (
                     self.checkpointer is not None
                     and self.checkpointer.at == CheckpointAt.END_OF_RUN
-                    and not do_interrupt_before
                 ):
                     checkpoint = create_checkpoint(checkpoint, channels)
-                    await self.checkpointer.aput(config, checkpoint)
+                    await self.checkpointer.aput(checkpoint_config, checkpoint)
+        except BaseException as e:
+            await run_manager.on_chain_error(e)
+            raise
         finally:
             # cancel any pending tasks when generator is interrupted
             try:
                 for task in futures:
                     task.cancel()
             except NameError:
                 pass
 
     def invoke(
         self,
         input: Union[dict[str, Any], Any],
         config: Optional[RunnableConfig] = None,
         *,
+        stream_mode: StreamMode = "values",
         output_keys: Optional[Union[str, Sequence[str]]] = None,
         input_keys: Optional[Union[str, Sequence[str]]] = None,
         interrupt_before_nodes: Optional[Sequence[str]] = None,
         interrupt_after_nodes: Optional[Sequence[str]] = None,
         debug: Optional[bool] = None,
         **kwargs: Any,
     ) -> Union[dict[str, Any], Any]:
-        latest: Union[dict[str, Any], Any] = None
+        output_keys = output_keys if output_keys is not None else self.output_channels
+        output_is_dict = not isinstance(output_keys, str)
+        if stream_mode == "values":
+            latest: Union[dict[str, Any], Any] = {} if output_is_dict else None
+        else:
+            chunks = []
         for chunk in self.stream(
             input,
             config,
-            output_keys=output_keys if output_keys is not None else self.output,
-            input_keys=input_keys,
-            interrupt_before_nodes=interrupt_before_nodes,
-            interrupt_after_nodes=interrupt_after_nodes,
-            debug=debug,
-            **kwargs,
-        ):
-            latest = chunk
-        return latest
-
-    def stream(
-        self,
-        input: Union[dict[str, Any], Any],
-        config: Optional[RunnableConfig] = None,
-        *,
-        output_keys: Optional[Union[str, Sequence[str]]] = None,
-        input_keys: Optional[Union[str, Sequence[str]]] = None,
-        interrupt_before_nodes: Optional[Sequence[str]] = None,
-        interrupt_after_nodes: Optional[Sequence[str]] = None,
-        debug: Optional[bool] = None,
-        **kwargs: Any,
-    ) -> Iterator[Union[dict[str, Any], Any]]:
-        return self.transform(
-            iter([input]),
-            config,
-            output_keys=output_keys,
-            input_keys=input_keys,
-            interrupt_before_nodes=interrupt_before_nodes,
-            interrupt_after_nodes=interrupt_after_nodes,
-            debug=debug,
-            **kwargs,
-        )
-
-    def transform(
-        self,
-        input: Iterator[Union[dict[str, Any], Any]],
-        config: Optional[RunnableConfig] = None,
-        *,
-        output_keys: Optional[Union[str, Sequence[str]]] = None,
-        input_keys: Optional[Union[str, Sequence[str]]] = None,
-        interrupt_before_nodes: Optional[Sequence[str]] = None,
-        interrupt_after_nodes: Optional[Sequence[str]] = None,
-        debug: Optional[bool] = None,
-        **kwargs: Any,
-    ) -> Iterator[Union[dict[str, Any], Any]]:
-        for chunk in self._transform_stream_with_config(
-            input,
-            self._transform,
-            config,
+            stream_mode=stream_mode,
             output_keys=output_keys,
             input_keys=input_keys,
             interrupt_before_nodes=interrupt_before_nodes,
             interrupt_after_nodes=interrupt_after_nodes,
             debug=debug,
             **kwargs,
         ):
-            yield chunk
+            if stream_mode == "values":
+                latest = {**latest, **chunk} if output_is_dict else chunk
+            else:
+                chunks.append(chunk)
+        if stream_mode == "values":
+            return latest
+        else:
+            return chunks
 
     async def ainvoke(
         self,
         input: Union[dict[str, Any], Any],
         config: Optional[RunnableConfig] = None,
         *,
+        stream_mode: StreamMode = "values",
         output_keys: Optional[Union[str, Sequence[str]]] = None,
         input_keys: Optional[Union[str, Sequence[str]]] = None,
         interrupt_before_nodes: Optional[Sequence[str]] = None,
         interrupt_after_nodes: Optional[Sequence[str]] = None,
         debug: Optional[bool] = None,
         **kwargs: Any,
     ) -> Union[dict[str, Any], Any]:
-        latest: Union[dict[str, Any], Any] = None
+        output_keys = output_keys if output_keys is not None else self.output_channels
+        output_is_dict = not isinstance(output_keys, str)
+        if stream_mode == "values":
+            latest: Union[dict[str, Any], Any] = {} if output_is_dict else None
+        else:
+            chunks = []
         async for chunk in self.astream(
             input,
             config,
-            output_keys=output_keys if output_keys is not None else self.output,
-            input_keys=input_keys,
-            interrupt_before_nodes=interrupt_before_nodes,
-            interrupt_after_nodes=interrupt_after_nodes,
-            debug=debug,
-            **kwargs,
-        ):
-            latest = chunk
-        return latest
-
-    async def astream(
-        self,
-        input: Union[dict[str, Any], Any],
-        config: Optional[RunnableConfig] = None,
-        *,
-        output_keys: Optional[Union[str, Sequence[str]]] = None,
-        input_keys: Optional[Union[str, Sequence[str]]] = None,
-        interrupt_before_nodes: Optional[Sequence[str]] = None,
-        interrupt_after_nodes: Optional[Sequence[str]] = None,
-        debug: Optional[bool] = None,
-        **kwargs: Any,
-    ) -> AsyncIterator[Union[dict[str, Any], Any]]:
-        async def input_stream() -> AsyncIterator[Union[dict[str, Any], Any]]:
-            yield input
-
-        async for chunk in self.atransform(
-            input_stream(),
-            config,
+            stream_mode=stream_mode,
             output_keys=output_keys,
             input_keys=input_keys,
             interrupt_before_nodes=interrupt_before_nodes,
             interrupt_after_nodes=interrupt_after_nodes,
             debug=debug,
             **kwargs,
         ):
-            yield chunk
-
-    async def atransform(
-        self,
-        input: AsyncIterator[Union[dict[str, Any], Any]],
-        config: Optional[RunnableConfig] = None,
-        *,
-        output_keys: Optional[Union[str, Sequence[str]]] = None,
-        input_keys: Optional[Union[str, Sequence[str]]] = None,
-        interrupt_before_nodes: Optional[Sequence[str]] = None,
-        interrupt_after_nodes: Optional[Sequence[str]] = None,
-        debug: Optional[bool] = None,
-        **kwargs: Any,
-    ) -> AsyncIterator[Union[dict[str, Any], Any]]:
-        async for chunk in self._atransform_stream_with_config(
-            input,
-            self._atransform,
-            config,
-            output_keys=output_keys,
-            input_keys=input_keys,
-            interrupt_before_nodes=interrupt_before_nodes,
-            interrupt_after_nodes=interrupt_after_nodes,
-            debug=debug,
-            **kwargs,
-        ):
-            yield chunk
+            if stream_mode == "values":
+                latest = {**latest, **chunk} if output_is_dict else chunk
+            else:
+                chunks.append(chunk)
+        if stream_mode == "values":
+            return latest
+        else:
+            return chunks
 
 
 def _panic_or_proceed(
     done: Union[set[concurrent.futures.Future[Any]], set[asyncio.Task[Any]]],
     inflight: Union[set[concurrent.futures.Future[Any]], set[asyncio.Task[Any]]],
     step: int,
 ) -> None:
@@ -922,160 +1062,166 @@
         raise TimeoutError(f"Timed out at step {step}")
 
 
 def _should_interrupt(
     checkpoint: Checkpoint,
     interrupt_nodes: Sequence[str],
     snapshot_channels: Sequence[str],
-    pending_writes: Sequence[tuple[str, Any]],
+    tasks: list[PregelExecutableTask],
 ) -> bool:
+    # defaultdicts are mutated on access :( so we need to copy
+    seen = checkpoint["versions_seen"].copy()[INTERRUPT].copy()
     return (
         # interrupt if any of snapshopt_channels has been updated since last interrupt
         any(
-            checkpoint["channel_versions"][chan]
-            > checkpoint["versions_seen"][INTERRUPT][chan]
+            checkpoint["channel_versions"][chan] > seen[chan]
             for chan in snapshot_channels
         )
         # and any channel written to is in interrupt_nodes list
-        and any(chan for chan, _ in pending_writes if chan in interrupt_nodes)
+        and any(node for node, _, _, _, _ in tasks if node in interrupt_nodes)
     )
 
 
-def _read_channel(
-    channels: Mapping[str, BaseChannel], chan: str, catch: bool = True
-) -> Any:
-    try:
-        return channels[chan].get()
-    except EmptyChannelError:
-        if catch:
-            return None
-        else:
-            raise
+def _local_read(
+    checkpoint: Checkpoint,
+    channels: Mapping[str, BaseChannel],
+    writes: Sequence[tuple[str, Any]],
+    select: Union[list[str], str],
+    fresh: bool = False,
+) -> Union[dict[str, Any], Any]:
+    if fresh:
+        checkpoint = create_checkpoint(checkpoint, channels)
+        with ChannelsManager(channels, checkpoint) as channels:
+            _apply_writes(copy_checkpoint(checkpoint), channels, writes)
+            return read_channels(channels, select)
+    else:
+        return read_channels(channels, select)
 
 
 def _apply_writes(
     checkpoint: Checkpoint,
     channels: Mapping[str, BaseChannel],
     pending_writes: Sequence[tuple[str, Any]],
-    config: RunnableConfig,
-    for_step: int,
 ) -> None:
     pending_writes_by_channel: dict[str, list[Any]] = defaultdict(list)
     # Group writes by channel
     for chan, val in pending_writes:
-        if chan in AllReservedChannels:
-            raise ValueError(f"Can't write to reserved channel {chan}")
         pending_writes_by_channel[chan].append(val)
 
-    # Update reserved channels
-    pending_writes_by_channel[ReservedChannels.is_last_step] = [
-        for_step + 1 == config["recursion_limit"]
-    ]
+    # Find the highest version of all channels
+    if checkpoint["channel_versions"]:
+        max_version = max(checkpoint["channel_versions"].values())
+    else:
+        max_version = 0
 
     updated_channels: set[str] = set()
     # Apply writes to channels
     for chan, vals in pending_writes_by_channel.items():
         if chan in channels:
             try:
                 channels[chan].update(vals)
             except InvalidUpdateError as e:
                 raise InvalidUpdateError(
                     f"Invalid update for channel {chan}: {e}"
                 ) from e
-            checkpoint["channel_versions"][chan] += 1
+            checkpoint["channel_versions"][chan] = max_version + 1
             updated_channels.add(chan)
         else:
-            logger.warning(f"Skipping write for channel {chan} which has no readers")
+            logger.warning(f"Skipping write for channel '{chan}' which has no readers")
     # Channels that weren't updated in this step are notified of a new step
     for chan in channels:
         if chan not in updated_channels:
             channels[chan].update([])
 
 
-def _apply_writes_from_view(
-    checkpoint: Checkpoint, channels: Mapping[str, BaseChannel], values: dict[str, Any]
-) -> None:
-    # Apply writes to channels
-    for chan, value in values.items():
-        if value == _read_channel(channels, chan):
-            continue
-
-        assert isinstance(channels[chan], (LastValue, EphemeralValue, AnyValue)), (
-            f"Can't modify channel {chan} of type "
-            f"{channels[chan].__class__.__name__}"
-        )
-        checkpoint["channel_versions"][chan] += 1
-        channels[chan].update([values[chan]])
+@overload
+def _prepare_next_tasks(
+    checkpoint: Checkpoint,
+    processes: Mapping[str, PregelNode],
+    channels: Mapping[str, BaseChannel],
+    for_execution: Literal[False],
+) -> tuple[Checkpoint, list[PregelTaskDescription]]:
+    ...
+
+
+@overload
+def _prepare_next_tasks(
+    checkpoint: Checkpoint,
+    processes: Mapping[str, PregelNode],
+    channels: Mapping[str, BaseChannel],
+    for_execution: Literal[True],
+) -> tuple[Checkpoint, list[PregelExecutableTask]]:
+    ...
 
 
 def _prepare_next_tasks(
     checkpoint: Checkpoint,
-    processes: Mapping[str, Union[ChannelInvoke, ChannelBatch]],
+    processes: Mapping[str, PregelNode],
     channels: Mapping[str, BaseChannel],
-    update_seen: bool = True,
-) -> tuple[Checkpoint, list[tuple[Runnable, Any, str]]]:
-    checkpoint = copy_checkpoint(checkpoint) if update_seen else checkpoint
-    tasks: list[tuple[Runnable, Any, str]] = []
+    *,
+    for_execution: bool,
+) -> tuple[Checkpoint, Union[list[PregelTaskDescription], list[PregelExecutableTask]]]:
+    checkpoint = copy_checkpoint(checkpoint)
+    tasks: Union[list[PregelTaskDescription], list[PregelExecutableTask]] = []
     # Check if any processes should be run in next step
     # If so, prepare the values to be passed to them
     for name, proc in processes.items():
         seen = checkpoint["versions_seen"][name]
-        if isinstance(proc, ChannelInvoke):
-            # If any of the channels read by this process were updated
-            if any(
-                checkpoint["channel_versions"][chan] > seen[chan]
-                for chan in proc.triggers
-            ):
-                # If all trigger channels subscribed by this process are not empty
-                # then invoke the process with the values of all non-empty channels
+        # If any of the channels read by this process were updated
+        if any(
+            checkpoint["channel_versions"][chan] > seen[chan]
+            for chan in proc.triggers
+            if not isinstance(
+                read_channel(channels, chan, return_exception=True), EmptyChannelError
+            )
+        ):
+            # If all trigger channels subscribed by this process are not empty
+            # then invoke the process with the values of all non-empty channels
+            if isinstance(proc.channels, dict):
                 try:
                     val: Any = {
-                        k: _read_channel(
-                            channels, chan, catch=chan not in proc.triggers
-                        )
+                        k: read_channel(channels, chan, catch=chan not in proc.triggers)
                         for k, chan in proc.channels.items()
                     }
                 except EmptyChannelError:
                     continue
-
-                # If the process has a mapper, apply it to the value
-                if proc.mapper is not None:
-                    val = proc.mapper(val)
-
-                # Processes that subscribe to a single keyless channel get
-                # the value directly, instead of a dict
-                if list(proc.channels.keys()) == [None]:
-                    val = val[None]
-
-                # update seen versions
-                if update_seen:
-                    seen.update(
-                        {
-                            chan: checkpoint["channel_versions"][chan]
-                            for chan in proc.triggers
-                        }
-                    )
-
-                # skip if condition is not met
-                if proc.when is None or proc.when(val):
-                    tasks.append((proc, val, name))
-        elif isinstance(proc, ChannelBatch):
-            # If the channel read by this process was updated
-            if checkpoint["channel_versions"][proc.channel] > seen[proc.channel]:
-                # If the channel subscribed by this process is not empty
-                try:
-                    val = channels[proc.channel].get()
-                except EmptyChannelError:
+            elif isinstance(proc.channels, list):
+                for chan in proc.channels:
+                    try:
+                        val = read_channel(channels, chan, catch=False)
+                        break
+                    except EmptyChannelError:
+                        pass
+                else:
                     continue
-                if proc.key is not None:
-                    val = [{proc.key: v} for v in val]
+            else:
+                raise RuntimeError(
+                    "Invalid channels type, expected list or dict, got {proc.channels}"
+                )
 
-                tasks.append((proc, val, name))
-                if update_seen:
-                    seen[proc.channel] = checkpoint["channel_versions"][proc.channel]
+            # If the process has a mapper, apply it to the value
+            if proc.mapper is not None:
+                val = proc.mapper(val)
+
+            # update seen versions
+            if for_execution:
+                seen.update(
+                    {
+                        chan: checkpoint["channel_versions"][chan]
+                        for chan in proc.triggers
+                    }
+                )
+
+            if for_execution:
+                if node := proc.get_node():
+                    tasks.append(
+                        PregelExecutableTask(name, val, node, deque(), proc.config)
+                    )
+            else:
+                tasks.append(PregelTaskDescription(name, val))
     return checkpoint, tasks
 
 
 async def _aconsume(iterator: AsyncIterator[Any]) -> None:
     """Consume an async iterator."""
     async for _ in iterator:
         pass
```

### Comparing `gigagraph-0.0.26/langgraph/pregel/debug.py` & `gigagraph-0.0.34/langgraph/pregel/debug.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from pprint import pformat
 from typing import Any, Iterator, Mapping
 
-from langchain_core.runnables import Runnable
 from langchain_core.utils.input import get_bolded_text, get_colored_text
 
 from langgraph.channels.base import BaseChannel, EmptyChannelError
+from langgraph.pregel.types import PregelExecutableTask
 
 
-def print_step_start(step: int, next_tasks: list[tuple[Runnable, Any, str]]) -> None:
+def print_step_start(step: int, next_tasks: list[PregelExecutableTask]) -> None:
     n_tasks = len(next_tasks)
     print(
-        f"{get_colored_text('[pregel/step]', color='blue')} "
+        f"{get_colored_text('[langgraph/step]', color='blue')} "
         + get_bolded_text(
             f"Starting step {step} with {n_tasks} task{'s' if n_tasks > 1 else ''}. Next tasks:\n"
         )
-        + "\n".join(f"- {name}({pformat(val)})" for _, val, name in next_tasks)
+        + "\n".join(f"- {name}({pformat(val)})" for name, val, _, _, _ in next_tasks)
     )
 
 
 def print_checkpoint(step: int, channels: Mapping[str, BaseChannel]) -> None:
     print(
-        f"{get_colored_text('[pregel/checkpoint]', color='blue')} "
+        f"{get_colored_text('[langgraph/checkpoint]', color='blue')} "
         + get_bolded_text(f"Finishing step {step}. Channel values:\n")
-        + pformat({name: val for name, val in _read_channels(channels)}, depth=1)
+        + pformat({name: val for name, val in _read_channels(channels)}, depth=3)
     )
 
 
 def _read_channels(channels: Mapping[str, BaseChannel]) -> Iterator[tuple[str, Any]]:
     for name, channel in channels.items():
         try:
             yield (name, channel.get())
```

### Comparing `gigagraph-0.0.26/langgraph/pregel/write.py` & `gigagraph-0.0.34/langgraph/pregel/write.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 from __future__ import annotations
 
 import asyncio
-from typing import Any, Callable, NamedTuple, Optional, Sequence, Union
+from typing import Any, Callable, NamedTuple, Optional, Sequence, TypeVar, Union
 
-from langchain_core.runnables import (
-    Runnable,
-    RunnableConfig,
-    RunnablePassthrough,
-)
+from langchain_core.runnables import Runnable, RunnableConfig
 from langchain_core.runnables.utils import ConfigurableFieldSpec
 
 from langgraph.constants import CONFIG_KEY_SEND
+from langgraph.utils import RunnableCallable
 
 TYPE_SEND = Callable[[Sequence[tuple[str, Any]]], None]
+R = TypeVar("R", bound=Runnable)
 
 
 SKIP_WRITE = object()
 
 
 class ChannelWriteEntry(NamedTuple):
     channel: str
-    value: Optional[Union[Any, Runnable]]
-    skip_none: bool
+    value: Optional[Union[Any, Runnable]] = None
+    skip_none: bool = False
 
 
-class ChannelWrite(RunnablePassthrough):
-    channels: Sequence[ChannelWriteEntry]
+class ChannelWrite(RunnableCallable):
+    writes: Sequence[ChannelWriteEntry]
     """
     Sequence of write entries, each of which is a tuple of:
     - channel name
     - runnable to map input, or None to use the input, or any other value to use instead
     - whether to skip writing if the mapped value is None
     """
 
-    class Config:
-        arbitrary_types_allowed = True
-
-    def __init__(self, *, channels: Sequence[ChannelWriteEntry]):
-        super().__init__(func=self._write, afunc=self._awrite, channels=channels)
-        self.name = f"ChannelWrite<{','.join(chan for chan, _, _ in self.channels)}>"
+    def __init__(
+        self, writes: Sequence[ChannelWriteEntry], *, tags: Optional[list[str]] = None
+    ):
+        super().__init__(func=self._write, afunc=self._awrite, name=None, tags=tags)
+        self.writes = writes
 
     def __repr_args__(self) -> Any:
-        return [("channels", self.channels)]
+        return [("writes", self.writes)]
+
+    def get_name(
+        self, suffix: Optional[str] = None, *, name: Optional[str] = None
+    ) -> str:
+        if not name:
+            name = f"ChannelWrite<{','.join(chan for chan, _, _ in self.writes)}>"
+        return super().get_name(suffix, name=name)
 
     @property
     def config_specs(self) -> list[ConfigurableFieldSpec]:
         return [
             ConfigurableFieldSpec(
                 id=CONFIG_KEY_SEND,
                 name=CONFIG_KEY_SEND,
@@ -61,46 +65,60 @@
                 chan,
                 r.invoke(input, config)
                 if isinstance(r, Runnable)
                 else r
                 if r is not None
                 else input,
             )
-            for chan, r, _ in self.channels
+            for chan, r, _ in self.writes
         ]
         values = [
             write
-            for write, (_, _, skip_none) in zip(values, self.channels)
+            for write, (_, _, skip_none) in zip(values, self.writes)
             if not skip_none or write[1] is not None
         ]
-
         self.do_write(config, **dict(values))
+        return input
 
     async def _awrite(self, input: Any, config: RunnableConfig) -> None:
         values = await asyncio.gather(
             *(
                 r.ainvoke(input, config)
                 if isinstance(r, Runnable)
                 else _mk_future(r)
                 if r is not None
                 else _mk_future(input)
-                for _, r, _ in self.channels
+                for _, r, _ in self.writes
             )
         )
         values = [
             (chan, val)
-            for val, (chan, _, skip_none) in zip(values, self.channels)
+            for val, (chan, _, skip_none) in zip(values, self.writes)
             if not skip_none or val is not None
         ]
-
         self.do_write(config, **dict(values))
+        return input
 
     @staticmethod
     def do_write(config: RunnableConfig, **values: Any) -> None:
         write: TYPE_SEND = config["configurable"][CONFIG_KEY_SEND]
         write([(chan, val) for chan, val in values.items() if val is not SKIP_WRITE])
 
+    @staticmethod
+    def is_writer(runnable: Runnable) -> bool:
+        return (
+            isinstance(runnable, ChannelWrite)
+            or getattr(runnable, "_is_channel_writer", False) is True
+        )
+
+    @staticmethod
+    def register_writer(runnable: R) -> R:
+        # using object.__setattr__ to work around objects that override __setattr__
+        # eg. pydantic models and dataclasses
+        object.__setattr__(runnable, "_is_channel_writer", True)
+        return runnable
+
 
 def _mk_future(val: Any) -> asyncio.Future:
     fut = asyncio.Future()
     fut.set_result(val)
     return fut
```

### Comparing `gigagraph-0.0.26/pyproject.toml` & `gigagraph-0.0.34/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "gigagraph"
-version = "0.0.26"
+version = "0.0.34"
 description = "gigagraph"
 authors = []
-license = "LangGraph License"
+license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ai-forever/gigagraph"
 packages = [
     {include = "langgraph"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9.0,<4.0"
-gigachain_core = "^0.1.28"
+gigachain-core = "^0.1.38"
 
 
 [tool.poetry.group.test.dependencies]
 # The only dependencies that should be added are
 # dependencies used for running tests (e.g., pytest, freezegun, response).
 # Any dependencies that do not meet that criteria will be removed.
 pytest = "^7.3.0"
```

### Comparing `gigagraph-0.0.26/PKG-INFO` & `gigagraph-0.0.34/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: gigagraph
-Version: 0.0.26
-Summary: gigagraph
-Home-page: https://github.com/ai-forever/gigagraph
-License: LangGraph License
-Requires-Python: >=3.9.0,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: gigachain_core (>=0.1.28,<0.2.0)
-Project-URL: Repository, https://github.com/ai-forever/gigagraph
-Description-Content-Type: text/markdown
-
 # GigaGraph
 
 ⚡ Разработка языковых агентов в виде графов ⚡
 
 ## Описание
 
 GigaGraph — это библиотека, дающая возможность работать с LLM (большие языковые модели) для создания приложений, которые используют множество взаимодействующих цепочек (акторов) и сохраняют данные о состоянии.
@@ -448,14 +431,26 @@
 For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/persistence.ipynb)
 
 ### Human-in-the-loop
 
 LangGraph comes with built-in support for human-in-the-loop workflows. This is useful when you want to have a human review the current state before proceeding to a particular node.
 For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/human-in-the-loop.ipynb)
 
+### Visualizing the graph
+
+Agents you create with LangGraph can be complex. In order to make it easier to understand what is happening under the hood, we've added methods to print out and visualize the graph.
+This can create both ascii art as well as pngs.
+For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/visualization.ipynb)
+
+### "Time Travel"
+
+With "time travel" functionality you can jump to any point in the graph execution, modify the state, and rerun from there.
+This is useful for both debugging workflows, as well as end user-facing workflows to allow them to correct the state.
+For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/time-travel.ipynb)
+
 
 ## Примеры
 
 ### ChatAgentExecutor: with function calling
 
 ### Исполнитель чат-агента с возможностью вызывать функции
 
@@ -489,31 +484,29 @@
 Примеры небольших изменений, которые можно сделать при разработке исполнителя чат-агента.
 Приведенные вариации основаны на примере [Getting Started Notebook](https://github.com/langchain-ai/langgraph/blob/main/examples/agent_executor/base.ipynb).
 
 - [Human-in-the-loop](https://github.com/langchain-ai/langgraph/blob/main/examples/agent_executor/human-in-the-loop.ipynb). Пример демонстрирует как реализовать подход «человек-в-цикле».
 - [Принудительный вызов инструмента](https://github.com/langchain-ai/langgraph/blob/main/examples/agent_executor/force-calling-a-tool-first.ipynb). Пример демонстрирует как всегда вызывать определенный инструмент в первую очередь.
 - [Управление этапами работы агента](https://github.com/langchain-ai/langgraph/blob/main/examples/agent_executor/managing-agent-steps.ipynb). Пример демонстрирует, как можно более детально управлять промежуточными этапами работы агента.
 
-
 ### Planning Agent Examples
 
 The following notebooks implement agent architectures prototypical of the "plan-and-execute" style, where an LLM planner decomposes a user request into a program, an executor executes the program, and an LLM synthesizes a response (and/or dynamically replans) based on the program outputs.
 
 - [Plan-and-execute](https://github.com/langchain-ai/langgraph/blob/main/examples/plan-and-execute/plan-and-execute.ipynb): a simple agent with a **planner** that generates a multi-step task list, an **executor** that invokes the tools in the plan, and a **replanner** that responds or generates an updated plan. Based on the [Plan-and-solve](https://arxiv.org/abs/2305.04091) paper by Wang, et. al.
 - [Reasoning without Observation](https://github.com/langchain-ai/langgraph/blob/main/examples/rewoo/rewoo.ipynb): planner generates a task list whose observations are saved as **variables**. Variables can be used in subsequent tasks to reduce the need for further re-planning. Based on the [ReWOO](https://arxiv.org/abs/2305.18323) paper by Xu, et. al.
 - [LLMCompiler](https://github.com/langchain-ai/langgraph/blob/main/examples/llm-compiler/LLMCompiler.ipynb): planner generates a **DAG** of tasks with variable responses. Tasks are **streamed** and executed eagerly to minimize tool execution runtime. Based on the [paper](https://arxiv.org/abs/2312.04511) by Kim, et. al.
 
-
 ### Reflection / Self-Critique
 
 When output quality is a major concern, it's common to incorporate some combination of self-critique or reflection and external validation to refine your system's outputs. The following examples demonstrate research that implement this type of design.
 
 - [Basic Reflection](./examples/reflection/reflection.ipynb): add a simple "reflect" step in your graph to prompt your system to revise its outputs.
 - [Reflexion](./examples/reflexion/reflexion.ipynb): critique missing and superflous aspects of the agent's response to guide subsequent steps. Based on [Reflexion](https://arxiv.org/abs/2303.11366), by Shinn, et. al.
-- [Language Agent Tree Search](./examples/lats/lats.ipynb): execute multiple agents in parallel, using reflection and environmental rewards to drive a Monte Carlo Tree Search. Based on [LATS](https://arxiv.org/abs/2310.04406/LanguageAgentTreeSearch/), by Zhou, et. al.
+- [Language Agent Tree Search](./examples/lats/lats.ipynb): execute multiple agents in parallel, using reflection and environmental rewards to drive a Monte Carlo Tree Search. Based on [LATS](https://arxiv.org/abs/2310.04406), by Zhou, et. al.
 
 ### Multi-agent Examples
 ### Примеры с несколькими агентами
 
 - [Совместная работа нескольких агентов](https://github.com/langchain-ai/langgraph/blob/main/examples/multi_agent/multi-agent-collaboration.ipynb). Пример демонстрирует как создать двух агентов, которые работают вместе для решения задачи.
 - [Несколько агентов с «руководителем»](https://github.com/langchain-ai/langgraph/blob/main/examples/multi_agent/agent_supervisor.ipynb). Пример демонстрирует как организовать работу агентов используя LLM в роли «руководителя», который решает как распределять работу.
 - [Иерархичные команды агентов](https://github.com/langchain-ai/langgraph/blob/main/examples/multi_agent/hierarchical_agent_teams.ipynb): пример демонстрирует как организовать «команды» агентов, которые будут взаимодействовать для решения задачи, в виде вложенных графов.
@@ -525,15 +518,16 @@
 - [Оценка чат-бота с помощью симуляции взаимодействия нескольких агентов.](https://github.com/langchain-ai/langgraph/blob/main/examples/chatbot-simulation-evaluation/agent-simulation-evaluation.ipynb). В примере показано как симулировать диалог «виртуального пользователя» с чат-ботом.
 
 ### Асинхронная работа
 
 При работе с асинхронными процессами вам может потребоваться создать с помощью GigaGraph граф с вершинами, которые будут асинхронными по умолчанию.
 [Пример](https://github.com/langchain-ai/langgraph/blob/main/examples/async.ipynb).
 
-### Потоковая передача токенов
+- [Chat bot evaluation as multi-agent simulation](https://github.com/langchain-ai/langgraph/blob/main/examples/chatbot-simulation-evaluation/agent-simulation-evaluation.ipynb): how to simulate a dialogue between a "virtual user" and your chat bot
+- [Evaluating over a dataset](./examples/chatbot-simulation-evaluation/langsmith-agent-simulation-evaluation.ipynb): benchmark your assistant over a LangSmith dataset, which tasks a simulated customer to red-team your chat bot.
 
 Ответ модели может занимать продолжительное время и вам может потребоваться на лету отображать пользователям результат работы модели.
 [Пример](https://github.com/langchain-ai/langgraph/blob/main/examples/streaming-tokens.ipynb).
 
 ### Устойчивость
 
 GigaGraph позволяет сохранять состояние графа в определенный момент времени и потом возобновлять работу с этого состояния.
@@ -674,15 +668,15 @@
 ```
 Точка входа в граф.
 Задает вершину, которая будет вызвана в самом начале.
 Принимает один параметр:
 
 - `key` — название вершины, которую нужно вызывать в первую очередь.
 
-#### `.add_conditional_edges`
+#### `.set_conditional_entry_point`
 
 ```python
     def set_conditional_entry_point(
         self,
         condition: Callable[..., str],
         conditional_edge_mapping: Optional[Dict[str, str]] = None,
     ) -> None:
@@ -690,15 +684,14 @@
 
 This method adds a conditional entry point.
 What this means is that when the graph is called, it will call the `condition` Callable to decide what node to enter into first.
 
 - `condition`: A function to call to decide what to do next. The input will be the input to the graph. It should return a string that is present in `conditional_edge_mapping` and represents the edge to take.
 - `conditional_edge_mapping`: A mapping of string to string. The keys should be strings that may be returned by `condition`. The values should be the downstream node to call if that condition is returned.
 
-
 #### `.set_finish_point`
 
 ```python
     def set_finish_point(self, key: str) -> None:
 ```
 
 This is the exit point of the graph.
@@ -785,15 +778,15 @@
 
 inputs = {"messages": [HumanMessage(content="какая погода в саратове")]}
 for s in app.stream(inputs):
     print(list(s.values())[0])
     print("----")
 ```
 
-### create_tool_calling_executor
+### chat_agent_executor.create_tool_calling_executor
 
 ```python
 from langgraph.prebuilt import chat_agent_executor
 ```
 
 This is a helper function for creating a graph that works with a chat model that utilizes tool calling.
 Can be created by passing in a model and a list of tools.
@@ -846,8 +839,7 @@
 app = create_agent_executor(agent_runnable, tools)
 
 inputs = {"input": "what is the weather in sf", "chat_history": []}
 for s in app.stream(inputs):
     print(list(s.values())[0])
     print("----")
 ```
-
```

