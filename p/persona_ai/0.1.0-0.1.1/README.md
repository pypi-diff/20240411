# Comparing `tmp/persona_ai-0.1.0.tar.gz` & `tmp/persona_ai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persona_ai-0.1.0.tar", max compression
+gzip compressed data, was "persona_ai-0.1.1.tar", max compression
```

## Comparing `persona_ai-0.1.0.tar` & `persona_ai-0.1.1.tar`

### file list

```diff
@@ -1,140 +1,79 @@
--rw-r--r--   0        0        0    11242 2024-04-10 10:09:18.359744 persona_ai-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/code_runners/__init__.py
--rw-r--r--   0        0        0      187 2024-04-08 15:22:17.206292 persona_ai-0.1.0/persona_ai/code_runners/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1838 2024-04-08 15:22:17.206292 persona_ai-0.1.0/persona_ai/code_runners/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     2180 2024-04-08 15:22:17.222293 persona_ai-0.1.0/persona_ai/code_runners/__pycache__/local.cpython-310.pyc
--rw-r--r--   0        0        0     1239 2024-04-08 14:44:21.457123 persona_ai-0.1.0/persona_ai/code_runners/base.py
--rw-r--r--   0        0        0     2363 2024-04-08 14:39:06.291886 persona_ai-0.1.0/persona_ai/code_runners/local.py
--rw-r--r--   0        0        0      153 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/constants.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/conversation_listeners/__init__.py
--rw-r--r--   0        0        0      197 2024-04-08 06:53:25.073307 persona_ai-0.1.0/persona_ai/conversation_listeners/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5524 2024-04-08 15:22:17.250293 persona_ai-0.1.0/persona_ai/conversation_listeners/__pycache__/terminal.cpython-310.pyc
--rw-r--r--   0        0        0     5954 2024-04-08 14:44:22.237126 persona_ai-0.1.0/persona_ai/conversation_listeners/terminal.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/conversations/__init__.py
--rw-r--r--   0        0        0      188 2024-04-08 06:53:25.821310 persona_ai-0.1.0/persona_ai/conversations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3331 2024-04-08 15:22:17.258293 persona_ai-0.1.0/persona_ai/conversations/__pycache__/manager.cpython-310.pyc
--rw-r--r--   0        0        0     3161 2024-04-08 14:44:21.465124 persona_ai-0.1.0/persona_ai/conversations/manager.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/domain/__init__.py
--rw-r--r--   0        0        0      181 2024-04-08 06:53:03.629227 persona_ai-0.1.0/persona_ai/domain/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6118 2024-04-08 06:53:03.629227 persona_ai-0.1.0/persona_ai/domain/__pycache__/conversations.cpython-310.pyc
--rw-r--r--   0        0        0      706 2024-04-08 06:53:25.929310 persona_ai-0.1.0/persona_ai/domain/__pycache__/events.cpython-310.pyc
--rw-r--r--   0        0        0     1387 2024-04-08 15:22:17.270294 persona_ai-0.1.0/persona_ai/domain/__pycache__/repositories.cpython-310.pyc
--rw-r--r--   0        0        0      275 2024-04-08 06:53:25.961310 persona_ai-0.1.0/persona_ai/domain/__pycache__/roles.cpython-310.pyc
--rw-r--r--   0        0        0     2740 2024-04-08 06:53:25.825310 persona_ai-0.1.0/persona_ai/domain/__pycache__/tasks.cpython-310.pyc
--rw-r--r--   0        0        0      429 2024-04-08 06:53:03.653227 persona_ai-0.1.0/persona_ai/domain/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     6372 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/domain/conversations.py
--rw-r--r--   0        0        0      767 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/domain/events.py
--rw-r--r--   0        0        0      702 2024-04-08 14:47:42.217919 persona_ai-0.1.0/persona_ai/domain/repositories.py
--rw-r--r--   0        0        0       82 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/domain/roles.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/domain/schemas/__init__.py
--rw-r--r--   0        0        0      189 2024-04-08 15:22:17.282294 persona_ai-0.1.0/persona_ai/domain/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1208 2024-04-08 15:22:17.282294 persona_ai-0.1.0/persona_ai/domain/schemas/__pycache__/crud.cpython-310.pyc
--rw-r--r--   0        0        0      600 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/domain/schemas/crud.py
--rw-r--r--   0        0        0     2759 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/domain/tasks.py
--rw-r--r--   0        0        0      146 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/domain/utils.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/infrastructure/__init__.py
--rw-r--r--   0        0        0      189 2024-04-08 06:53:25.893310 persona_ai-0.1.0/persona_ai/infrastructure/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/infrastructure/repositories/__init__.py
--rw-r--r--   0        0        0      202 2024-04-08 06:53:25.893310 persona_ai-0.1.0/persona_ai/infrastructure/repositories/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1411 2024-04-08 15:22:17.294294 persona_ai-0.1.0/persona_ai/infrastructure/repositories/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     4125 2024-04-08 15:22:17.306294 persona_ai-0.1.0/persona_ai/infrastructure/repositories/__pycache__/mongo.cpython-310.pyc
--rw-r--r--   0        0        0      758 2024-04-08 14:47:42.829922 persona_ai-0.1.0/persona_ai/infrastructure/repositories/base.py
--rw-r--r--   0        0        0     2884 2024-04-08 14:47:42.249920 persona_ai-0.1.0/persona_ai/infrastructure/repositories/mongo.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/initializers/__init__.py
--rw-r--r--   0        0        0      187 2024-04-08 06:53:25.929310 persona_ai-0.1.0/persona_ai/initializers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3084 2024-04-08 06:53:25.929310 persona_ai-0.1.0/persona_ai/initializers/__pycache__/env_configurator.cpython-310.pyc
--rw-r--r--   0        0        0     1371 2024-04-08 15:22:17.318295 persona_ai-0.1.0/persona_ai/initializers/__pycache__/persona_configuration.cpython-310.pyc
--rw-r--r--   0        0        0     3753 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/initializers/env_configurator.py
--rw-r--r--   0        0        0      979 2024-04-08 14:47:42.817922 persona_ai-0.1.0/persona_ai/initializers/persona_configuration.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/models/__init__.py
--rw-r--r--   0        0        0      181 2024-04-08 06:53:03.709227 persona_ai-0.1.0/persona_ai/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1664 2024-04-08 15:22:17.326295 persona_ai-0.1.0/persona_ai/models/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     3239 2024-04-08 15:22:17.330295 persona_ai-0.1.0/persona_ai/models/__pycache__/code_bison.cpython-310.pyc
--rw-r--r--   0        0        0     7272 2024-04-08 15:22:17.330295 persona_ai-0.1.0/persona_ai/models/__pycache__/gemini.cpython-310.pyc
--rw-r--r--   0        0        0     3239 2024-04-08 15:22:17.334295 persona_ai-0.1.0/persona_ai/models/__pycache__/text_bison.cpython-310.pyc
--rw-r--r--   0        0        0      870 2024-04-08 14:48:27.882101 persona_ai-0.1.0/persona_ai/models/base.py
--rw-r--r--   0        0        0     2591 2024-04-08 14:48:27.834101 persona_ai-0.1.0/persona_ai/models/code_bison.py
--rw-r--r--   0        0        0    10094 2024-04-08 14:48:35.922133 persona_ai-0.1.0/persona_ai/models/gemini.py
--rw-r--r--   0        0        0     2591 2024-04-08 14:48:36.366135 persona_ai-0.1.0/persona_ai/models/text_bison.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/moderation/__init__.py
--rw-r--r--   0        0        0      185 2024-04-08 06:53:25.941310 persona_ai-0.1.0/persona_ai/moderation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3192 2024-04-08 15:22:17.338295 persona_ai-0.1.0/persona_ai/moderation/__pycache__/ai_moderator.cpython-310.pyc
--rw-r--r--   0        0        0     8193 2024-04-08 15:22:17.342295 persona_ai-0.1.0/persona_ai/moderation/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     4074 2024-04-08 15:22:17.346295 persona_ai-0.1.0/persona_ai/moderation/__pycache__/history_moderator.cpython-310.pyc
--rw-r--r--   0        0        0     3903 2024-04-08 15:22:17.346295 persona_ai-0.1.0/persona_ai/moderation/__pycache__/history_moderator_fc.cpython-310.pyc
--rw-r--r--   0        0        0     5492 2024-04-08 15:22:17.350295 persona_ai-0.1.0/persona_ai/moderation/__pycache__/react_moderator.cpython-310.pyc
--rw-r--r--   0        0        0     2842 2024-04-08 14:50:20.986552 persona_ai-0.1.0/persona_ai/moderation/ai_moderator.py
--rw-r--r--   0        0        0     7345 2024-04-08 14:51:53.450921 persona_ai-0.1.0/persona_ai/moderation/base.py
--rw-r--r--   0        0        0     4475 2024-04-08 14:51:53.978923 persona_ai-0.1.0/persona_ai/moderation/history_moderator.py
--rw-r--r--   0        0        0     4759 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/moderation/history_moderator_fc.py
--rw-r--r--   0        0        0     5580 2024-04-08 14:51:53.474921 persona_ai-0.1.0/persona_ai/moderation/react_moderator.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/personas/__init__.py
--rw-r--r--   0        0        0      183 2024-04-08 06:53:25.945310 persona_ai-0.1.0/persona_ai/personas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5321 2024-04-08 15:22:17.354296 persona_ai-0.1.0/persona_ai/personas/__pycache__/agent.cpython-310.pyc
--rw-r--r--   0        0        0     3600 2024-04-08 15:22:17.358296 persona_ai-0.1.0/persona_ai/personas/__pycache__/assistant.cpython-310.pyc
--rw-r--r--   0        0        0     5772 2024-04-08 06:53:25.945310 persona_ai-0.1.0/persona_ai/personas/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     3607 2024-04-08 15:22:17.362296 persona_ai-0.1.0/persona_ai/personas/__pycache__/coder.cpython-310.pyc
--rw-r--r--   0        0        0     8471 2024-04-08 15:22:17.378296 persona_ai-0.1.0/persona_ai/personas/__pycache__/party.cpython-310.pyc
--rw-r--r--   0        0        0     2959 2024-04-08 15:22:17.382296 persona_ai-0.1.0/persona_ai/personas/__pycache__/technician.cpython-310.pyc
--rw-r--r--   0        0        0     1257 2024-04-08 15:22:17.382296 persona_ai-0.1.0/persona_ai/personas/__pycache__/terminal.cpython-310.pyc
--rw-r--r--   0        0        0     6678 2024-04-08 14:54:32.699557 persona_ai-0.1.0/persona_ai/personas/agent.py
--rw-r--r--   0        0        0     4165 2024-04-08 14:54:31.839554 persona_ai-0.1.0/persona_ai/personas/assistant.py
--rw-r--r--   0        0        0     6507 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/personas/base.py
--rw-r--r--   0        0        0     3846 2024-04-08 14:54:32.703558 persona_ai-0.1.0/persona_ai/personas/coder.py
--rw-r--r--   0        0        0    13266 2024-04-08 14:58:31.431608 persona_ai-0.1.0/persona_ai/personas/party.py
--rw-r--r--   0        0        0     3022 2024-04-08 14:58:32.183662 persona_ai-0.1.0/persona_ai/personas/technician.py
--rw-r--r--   0        0        0      760 2024-04-08 15:00:26.392475 persona_ai-0.1.0/persona_ai/personas/terminal.py
--rw-r--r--   0        0        0      860 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/prompt_templates/agent.jinja2
--rw-r--r--   0        0        0      413 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/prompt_templates/assistant.jinja2
--rw-r--r--   0        0        0     1009 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/prompt_templates/coder.jinja2
--rw-r--r--   0        0        0     1076 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/prompt_templates/history_moderator.jinja2
--rw-r--r--   0        0        0     1062 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/prompt_templates/history_moderator_fc.jinja2
--rw-r--r--   0        0        0     1776 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/prompt_templates/react_json_moderator.jinja2
--rw-r--r--   0        0        0     1083 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/prompt_templates/react_moderator.jinja2
--rw-r--r--   0        0        0      330 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/prompt_templates/refiner.jinja2
--rw-r--r--   0        0        0      946 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2
--rw-r--r--   0        0        0      841 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2
--rw-r--r--   0        0        0      123 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/prompt_templates/technician.jinja2
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/prompts/__init__.py
--rw-r--r--   0        0        0      182 2024-04-08 06:53:25.929310 persona_ai-0.1.0/persona_ai/prompts/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      652 2024-04-08 15:22:17.390296 persona_ai-0.1.0/persona_ai/prompts/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     2452 2024-04-08 15:22:17.394297 persona_ai-0.1.0/persona_ai/prompts/__pycache__/jinja.cpython-310.pyc
--rw-r--r--   0        0        0     1060 2024-04-08 15:22:17.470298 persona_ai-0.1.0/persona_ai/prompts/__pycache__/text.cpython-310.pyc
--rw-r--r--   0        0        0      238 2024-04-08 14:58:32.179662 persona_ai-0.1.0/persona_ai/prompts/base.py
--rw-r--r--   0        0        0     2207 2024-04-08 15:00:26.384474 persona_ai-0.1.0/persona_ai/prompts/jinja.py
--rw-r--r--   0        0        0      588 2024-04-08 14:58:32.167661 persona_ai-0.1.0/persona_ai/prompts/text.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/refiners/__init__.py
--rw-r--r--   0        0        0      183 2024-04-08 15:22:17.486299 persona_ai-0.1.0/persona_ai/refiners/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1855 2024-04-08 15:22:17.490299 persona_ai-0.1.0/persona_ai/refiners/__pycache__/request_refiner.cpython-310.pyc
--rw-r--r--   0        0        0     1786 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/refiners/request_refiner.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/task_manager/__init__.py
--rw-r--r--   0        0        0      187 2024-04-08 06:53:25.925310 persona_ai-0.1.0/persona_ai/task_manager/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2619 2024-04-08 15:22:17.494299 persona_ai-0.1.0/persona_ai/task_manager/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     2248 2024-04-08 15:00:26.392475 persona_ai-0.1.0/persona_ai/task_manager/base.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/tools/__init__.py
--rw-r--r--   0        0        0      180 2024-04-08 06:53:04.509230 persona_ai-0.1.0/persona_ai/tools/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      759 2024-04-08 06:53:04.513230 persona_ai-0.1.0/persona_ai/tools/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     2334 2024-04-08 06:53:25.965310 persona_ai-0.1.0/persona_ai/tools/__pycache__/functional.cpython-310.pyc
--rw-r--r--   0        0        0     1257 2024-04-08 15:22:17.510299 persona_ai-0.1.0/persona_ai/tools/__pycache__/manager.cpython-310.pyc
--rw-r--r--   0        0        0      469 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/tools/base.py
--rw-r--r--   0        0        0     1746 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/tools/functional.py
--rw-r--r--   0        0        0      730 2024-04-08 15:00:26.376474 persona_ai-0.1.0/persona_ai/tools/manager.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/transport/__init__.py
--rw-r--r--   0        0        0      184 2024-04-08 06:53:25.925310 persona_ai-0.1.0/persona_ai/transport/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4444 2024-04-08 15:22:17.522299 persona_ai-0.1.0/persona_ai/transport/__pycache__/messagebus.cpython-310.pyc
--rw-r--r--   0        0        0     3448 2024-04-09 09:51:04.981993 persona_ai-0.1.0/persona_ai/transport/local/__pycache__/local_messagebus.cpython-310.pyc
--rw-r--r--   0        0        0     2576 2024-04-08 15:00:34.632689 persona_ai-0.1.0/persona_ai/transport/local/local_messagebus.py
--rw-r--r--   0        0        0     4022 2024-04-08 14:44:21.469123 persona_ai-0.1.0/persona_ai/transport/messagebus.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/transport/rabbitmq/__init__.py
--rw-r--r--   0        0        0      193 2024-04-08 06:53:25.933310 persona_ai-0.1.0/persona_ai/transport/rabbitmq/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8768 2024-04-08 15:22:17.530300 persona_ai-0.1.0/persona_ai/transport/rabbitmq/__pycache__/rabbitmq_messagebus.cpython-310.pyc
--rw-r--r--   0        0        0    10002 2024-04-08 15:01:04.409617 persona_ai-0.1.0/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/utils/__init__.py
--rw-r--r--   0        0        0      180 2024-04-08 06:53:04.513230 persona_ai-0.1.0/persona_ai/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1039 2024-04-08 06:53:04.513230 persona_ai-0.1.0/persona_ai/utils/__pycache__/crypto.cpython-310.pyc
--rw-r--r--   0        0        0     1087 2024-04-08 15:22:17.538300 persona_ai-0.1.0/persona_ai/utils/__pycache__/extractors.cpython-310.pyc
--rw-r--r--   0        0        0      723 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/utils/crypto.py
--rw-r--r--   0        0        0      750 2024-04-08 06:52:52.049183 persona_ai-0.1.0/persona_ai/utils/extractors.py
--rw-r--r--   0        0        0     1120 2024-04-09 09:46:14.923905 persona_ai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    12747 1970-01-01 00:00:00.000000 persona_ai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11250 2024-04-11 07:56:25.206198 persona_ai-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/code_runners/__init__.py
+-rw-r--r--   0        0        0     1239 2024-04-08 14:44:21.457123 persona_ai-0.1.1/persona_ai/code_runners/base.py
+-rw-r--r--   0        0        0     2363 2024-04-08 14:39:06.291886 persona_ai-0.1.1/persona_ai/code_runners/local.py
+-rw-r--r--   0        0        0      153 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/constants.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/conversation_listeners/__init__.py
+-rw-r--r--   0        0        0     5954 2024-04-08 14:44:22.237126 persona_ai-0.1.1/persona_ai/conversation_listeners/terminal.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/conversations/__init__.py
+-rw-r--r--   0        0        0     3214 2024-04-11 08:13:50.184451 persona_ai-0.1.1/persona_ai/conversations/manager.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/__init__.py
+-rw-r--r--   0        0        0     6372 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/conversations.py
+-rw-r--r--   0        0        0      767 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/events.py
+-rw-r--r--   0        0        0     1172 2024-04-11 08:14:55.564773 persona_ai-0.1.1/persona_ai/domain/repositories.py
+-rw-r--r--   0        0        0       82 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/roles.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/schemas/__init__.py
+-rw-r--r--   0        0        0      600 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/schemas/crud.py
+-rw-r--r--   0        0        0     2759 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/tasks.py
+-rw-r--r--   0        0        0      146 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/utils.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/infrastructure/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/infrastructure/repositories/__init__.py
+-rw-r--r--   0        0        0      758 2024-04-08 14:47:42.829922 persona_ai-0.1.1/persona_ai/infrastructure/repositories/base.py
+-rw-r--r--   0        0        0     1967 2024-04-11 08:19:46.530087 persona_ai-0.1.1/persona_ai/infrastructure/repositories/in_memory.py
+-rw-r--r--   0        0        0     2884 2024-04-08 14:47:42.249920 persona_ai-0.1.1/persona_ai/infrastructure/repositories/mongo.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/initializers/__init__.py
+-rw-r--r--   0        0        0     4183 2024-04-11 08:14:57.764784 persona_ai-0.1.1/persona_ai/initializers/env_configurator.py
+-rw-r--r--   0        0        0     1012 2024-04-11 08:13:23.084313 persona_ai-0.1.1/persona_ai/initializers/persona_configuration.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/models/__init__.py
+-rw-r--r--   0        0        0      870 2024-04-08 14:48:27.882101 persona_ai-0.1.1/persona_ai/models/base.py
+-rw-r--r--   0        0        0     2591 2024-04-08 14:48:27.834101 persona_ai-0.1.1/persona_ai/models/code_bison.py
+-rw-r--r--   0        0        0    10094 2024-04-08 14:48:35.922133 persona_ai-0.1.1/persona_ai/models/gemini.py
+-rw-r--r--   0        0        0     2591 2024-04-08 14:48:36.366135 persona_ai-0.1.1/persona_ai/models/text_bison.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/moderation/__init__.py
+-rw-r--r--   0        0        0     2842 2024-04-08 14:50:20.986552 persona_ai-0.1.1/persona_ai/moderation/ai_moderator.py
+-rw-r--r--   0        0        0     7345 2024-04-08 14:51:53.450921 persona_ai-0.1.1/persona_ai/moderation/base.py
+-rw-r--r--   0        0        0     4475 2024-04-08 14:51:53.978923 persona_ai-0.1.1/persona_ai/moderation/history_moderator.py
+-rw-r--r--   0        0        0     4759 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/moderation/history_moderator_fc.py
+-rw-r--r--   0        0        0     5580 2024-04-08 14:51:53.474921 persona_ai-0.1.1/persona_ai/moderation/react_moderator.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/personas/__init__.py
+-rw-r--r--   0        0        0     6678 2024-04-08 14:54:32.699557 persona_ai-0.1.1/persona_ai/personas/agent.py
+-rw-r--r--   0        0        0     4124 2024-04-11 08:16:44.105284 persona_ai-0.1.1/persona_ai/personas/assistant.py
+-rw-r--r--   0        0        0     6507 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/personas/base.py
+-rw-r--r--   0        0        0     3805 2024-04-11 08:16:44.125284 persona_ai-0.1.1/persona_ai/personas/coder.py
+-rw-r--r--   0        0        0    13266 2024-04-08 14:58:31.431608 persona_ai-0.1.1/persona_ai/personas/party.py
+-rw-r--r--   0        0        0     3022 2024-04-08 14:58:32.183662 persona_ai-0.1.1/persona_ai/personas/technician.py
+-rw-r--r--   0        0        0      760 2024-04-08 15:00:26.392475 persona_ai-0.1.1/persona_ai/personas/terminal.py
+-rw-r--r--   0        0        0      860 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/agent.jinja2
+-rw-r--r--   0        0        0      413 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/assistant.jinja2
+-rw-r--r--   0        0        0     1009 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/coder.jinja2
+-rw-r--r--   0        0        0     1076 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/history_moderator.jinja2
+-rw-r--r--   0        0        0     1062 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/history_moderator_fc.jinja2
+-rw-r--r--   0        0        0     1776 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/react_json_moderator.jinja2
+-rw-r--r--   0        0        0     1083 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/react_moderator.jinja2
+-rw-r--r--   0        0        0      330 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/refiner.jinja2
+-rw-r--r--   0        0        0      946 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2
+-rw-r--r--   0        0        0      841 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2
+-rw-r--r--   0        0        0      123 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/technician.jinja2
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompts/__init__.py
+-rw-r--r--   0        0        0      238 2024-04-08 14:58:32.179662 persona_ai-0.1.1/persona_ai/prompts/base.py
+-rw-r--r--   0        0        0     2207 2024-04-08 15:00:26.384474 persona_ai-0.1.1/persona_ai/prompts/jinja.py
+-rw-r--r--   0        0        0      588 2024-04-08 14:58:32.167661 persona_ai-0.1.1/persona_ai/prompts/text.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/refiners/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/refiners/request_refiner.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/task_manager/__init__.py
+-rw-r--r--   0        0        0     2263 2024-04-11 08:13:22.660311 persona_ai-0.1.1/persona_ai/task_manager/base.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/tools/__init__.py
+-rw-r--r--   0        0        0      469 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/tools/base.py
+-rw-r--r--   0        0        0     1746 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/tools/functional.py
+-rw-r--r--   0        0        0      730 2024-04-08 15:00:26.376474 persona_ai-0.1.1/persona_ai/tools/manager.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/transport/__init__.py
+-rw-r--r--   0        0        0     2576 2024-04-08 15:00:34.632689 persona_ai-0.1.1/persona_ai/transport/local/local_messagebus.py
+-rw-r--r--   0        0        0     4022 2024-04-08 14:44:21.469123 persona_ai-0.1.1/persona_ai/transport/messagebus.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/transport/rabbitmq/__init__.py
+-rw-r--r--   0        0        0    10002 2024-04-08 15:01:04.409617 persona_ai-0.1.1/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/utils/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/utils/crypto.py
+-rw-r--r--   0        0        0      750 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/utils/extractors.py
+-rw-r--r--   0        0        0     1120 2024-04-11 07:37:50.746837 persona_ai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12755 1970-01-01 00:00:00.000000 persona_ai-0.1.1/PKG-INFO
```

### Comparing `persona_ai-0.1.0/README.md` & `persona_ai-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Introduction
 
-Welcome to the exciting world of Persona AI, a cutting-edge framework designed for the development of generative
+****Welcome to the exciting world of Persona AI, a cutting-edge framework designed for the development of generative
 artificial intelligence applications that span multiple modes of interaction. Persona AI leverages the power of Google
 Vertex AI's generative models, placing it at the forefront of innovation in AI by offering a multimodal platform that
 integrates various forms of AI capabilities, from text to image generation, and beyond.
 
 At its core, Persona AI is a distributed agent system, characterized by its fully asynchronous nature. This means that
 communication among the agents is facilitated through a message bus, allowing for seamless and efficient exchanges of
 information. The agents in Persona AI work collaboratively in what is referred to as a "party," a dynamic group where
@@ -17,15 +17,15 @@
 also selected based on their declared scopes, ensuring that every contribution is meaningful and directed towards the
 collective goal.
 
 This introduction serves as your gateway into the world of Persona AI, where the blend of human ingenuity and artificial
 intelligence opens up new frontiers in technology and application development. Built on the robust and versatile
 foundation of Google Vertex AI's generative models, Persona AI is engineered to harness the capabilities of generative
 AI to create innovative and impactful solutions. Let's embark on this journey together, exploring the vast potentials of
-generative AI with Persona AI.
+generative AI with Persona AI.****
 
 # Party and Moderation in Persona AI
 
 The **Party** and **Moderation** systems within the Persona AI framework are pivotal in orchestrating the collaborative
 and decision-making dynamics essential for managing complex interactions and tasks. These components ensure that
 conversations are not just efficiently managed but also directed towards achieving the most relevant and
 context-appropriate outcomes.
```

### Comparing `persona_ai-0.1.0/persona_ai/code_runners/base.py` & `persona_ai-0.1.1/persona_ai/code_runners/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/code_runners/local.py` & `persona_ai-0.1.1/persona_ai/code_runners/local.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/conversation_listeners/terminal.py` & `persona_ai-0.1.1/persona_ai/conversation_listeners/terminal.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/conversations/manager.py` & `persona_ai-0.1.1/persona_ai/conversations/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from datetime import datetime
 
 from persona_ai.constants import HISTORY_SIZE
 from persona_ai.domain.conversations import Conversation, Message
-from persona_ai.domain.repositories import ConversationsRepository, MessagesRepository
+from persona_ai.domain.repositories import (
+    MongoConversationsRepository,
+    MongoMessagesRepository,
+)
 from persona_ai.domain.utils import create_id
 
 
 class ConversationManager:
     """
     Manages conversations and messages.
     This object is responsible for creating, updating, and retrieving conversations and messages.
@@ -17,37 +20,37 @@
     conversation_manager = ConversationManager()
     conversation = conversation_manager.create_conversation()
     message = Message(conversation_id=conversation.id, sender_id="sender", content="Hello, World!")
     conversation_manager.add_message(message)
     ```
     """
 
-    conversations_repository: ConversationsRepository
+    conversations_repository: MongoConversationsRepository
     """
     The repository for conversations.    
     """
 
-    messages_repository: MessagesRepository
+    messages_repository: MongoMessagesRepository
     """
     The repository for messages.
     """
 
     def __init__(
         self,
-        conversations_repository: ConversationsRepository = None,
-        messages_repository: MessagesRepository = None,
+        conversations_repository: MongoConversationsRepository = None,
+        messages_repository: MongoMessagesRepository = None,
     ):
         self.conversations_repository = (
             conversations_repository
             if conversations_repository
-            else ConversationsRepository()
+            else MongoConversationsRepository()
         )
 
         self.messages_repository = (
-            messages_repository if messages_repository else MessagesRepository()
+            messages_repository if messages_repository else MongoMessagesRepository()
         )
 
     def get_conversation(self, conversation_id: str) -> Conversation | None:
         """
         Get a conversation by its identifier.
         """
         return self.conversations_repository.get_by_id(conversation_id)
```

### Comparing `persona_ai-0.1.0/persona_ai/domain/conversations.py` & `persona_ai-0.1.1/persona_ai/domain/conversations.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/domain/events.py` & `persona_ai-0.1.1/persona_ai/domain/events.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/domain/schemas/crud.py` & `persona_ai-0.1.1/persona_ai/domain/schemas/crud.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/domain/tasks.py` & `persona_ai-0.1.1/persona_ai/domain/tasks.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/infrastructure/repositories/base.py` & `persona_ai-0.1.1/persona_ai/infrastructure/repositories/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/infrastructure/repositories/mongo.py` & `persona_ai-0.1.1/persona_ai/infrastructure/repositories/mongo.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/initializers/env_configurator.py` & `persona_ai-0.1.1/persona_ai/initializers/env_configurator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
 
 from persona_ai.conversations.manager import ConversationManager
 from persona_ai.domain.repositories import (
-    ConversationsRepository,
-    MessagesRepository,
-    TasksRepository,
+    MongoConversationsRepository,
+    MongoMessagesRepository,
+    MongoTasksRepository,
+    InMemoryConversationsRepository,
+    InMemoryMessagesRepository,
+    InMemoryTasksRepository,
 )
 from persona_ai.initializers.persona_configuration import PersonaAI
 from persona_ai.models.code_bison import CodeBisonModel
 from persona_ai.models.gemini import GeminiModel
 from persona_ai.models.text_bison import TextBisonModel
 from persona_ai.transport.local.local_messagebus import LocalMessageBus
 from persona_ai.transport.rabbitmq.rabbitmq_messagebus import RabbitMQMessageBus
@@ -53,24 +56,28 @@
         return LocalMessageBus()
     else:
         raise ValueError("Invalid message bus type: {}".format(message_bus_type))
 
 
 def configure_conversations_repository():
     if os.getenv("REPOSITORIES_TYPE") == "mongodb":
-        return ConversationsRepository()
+        return MongoConversationsRepository()
+    elif os.getenv("REPOSITORIES_TYPE") == "in-memory":
+        return InMemoryConversationsRepository()
     else:
         raise ValueError(
             "Invalid repository type: {}".format(os.getenv("REPOSITORIES_TYPE"))
         )
 
 
 def configure_messages_repository():
     if os.getenv("REPOSITORIES_TYPE") == "mongodb":
-        return MessagesRepository()
+        return MongoMessagesRepository()
+    elif os.getenv("REPOSITORIES_TYPE") == "in-memory":
+        return InMemoryMessagesRepository()
     else:
         raise ValueError(
             "Invalid repository type: {}".format(os.getenv("REPOSITORIES_TYPE"))
         )
 
 
 def configure_conversation_manager():
@@ -78,15 +85,17 @@
         conversations_repository=PersonaAI.conversations_repository,
         messages_repository=PersonaAI.messages_repository,
     )
 
 
 def configure_tasks_repository():
     if os.getenv("REPOSITORIES_TYPE") == "mongodb":
-        return TasksRepository()
+        return MongoTasksRepository()
+    elif os.getenv("REPOSITORIES_TYPE") == "in-memory":
+        return InMemoryTasksRepository()
     else:
         raise ValueError(
             "Invalid repository type: {}".format(os.getenv("REPOSITORIES_TYPE"))
         )
 
 
 def configure_persona_from_env():
```

### Comparing `persona_ai-0.1.0/persona_ai/initializers/persona_configuration.py` & `persona_ai-0.1.1/persona_ai/initializers/persona_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from persona_ai.conversations.manager import ConversationManager
-from persona_ai.domain.repositories import ConversationsRepository, MessagesRepository
+from persona_ai.domain.repositories import (
+    MongoConversationsRepository,
+    MongoMessagesRepository,
+)
 from persona_ai.models.base import GenAIModel
 from persona_ai.prompts.base import Prompt
 from persona_ai.transport.messagebus import MessageBus
 
 
 class PersonaAI:
     """
@@ -14,12 +17,12 @@
     tasks_repository = None
     moderator_model: GenAIModel = None
     assistant_model: GenAIModel = None
     technician_model: GenAIModel = None
     coder_model: GenAIModel = None
     refiner_model: GenAIModel = None
     agent_model: GenAIModel = None
-    conversations_repository: ConversationsRepository = None
-    messages_repository: MessagesRepository = None
+    conversations_repository: MongoConversationsRepository = None
+    messages_repository: MongoMessagesRepository = None
     prompt_manager: Prompt = None
     message_bus: MessageBus = None
     conversation_manager: ConversationManager = None
```

### Comparing `persona_ai-0.1.0/persona_ai/models/base.py` & `persona_ai-0.1.1/persona_ai/models/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/models/code_bison.py` & `persona_ai-0.1.1/persona_ai/models/code_bison.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/models/gemini.py` & `persona_ai-0.1.1/persona_ai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/models/text_bison.py` & `persona_ai-0.1.1/persona_ai/models/text_bison.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/moderation/ai_moderator.py` & `persona_ai-0.1.1/persona_ai/moderation/ai_moderator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/moderation/base.py` & `persona_ai-0.1.1/persona_ai/moderation/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/moderation/history_moderator.py` & `persona_ai-0.1.1/persona_ai/moderation/history_moderator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/moderation/history_moderator_fc.py` & `persona_ai-0.1.1/persona_ai/moderation/history_moderator_fc.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/moderation/react_moderator.py` & `persona_ai-0.1.1/persona_ai/moderation/react_moderator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/personas/agent.py` & `persona_ai-0.1.1/persona_ai/personas/agent.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/personas/assistant.py` & `persona_ai-0.1.1/persona_ai/personas/assistant.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,14 @@
             )
 
     def _render_prompt(self, history, message):
         return self.prompt.render(
             conversation_history=history,
             request=message,
             termination_token=TERMINATION_TOKEN,
-            language=PersonaAI.language,
         )
 
     def _call_model(self, prompt):
         return self.model.generate(prompt)
 
     def _generate_reply(self, body: MessageBody, request: Message) -> Message:
         is_termination_message = False
```

### Comparing `persona_ai-0.1.0/persona_ai/personas/base.py` & `persona_ai-0.1.1/persona_ai/personas/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/personas/coder.py` & `persona_ai-0.1.1/persona_ai/personas/coder.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
         self.code_runner = code_runner if code_runner else LocalCodeRunner()
         self.code_generation_instructions = code_generation_instructions
 
     def _render_template_prompt(self, history, message):
         return self.prompt.render(
             conversation_history=history,
             request=message,
-            language=PersonaAI.language,
             code_generation_instructions=self.code_generation_instructions,
         )
 
     def _generate_reply(self, body: MessageBody, request: Message) -> Message:
         message = super()._generate_reply(body, request)
 
         if message.body.text is not None:
```

### Comparing `persona_ai-0.1.0/persona_ai/personas/party.py` & `persona_ai-0.1.1/persona_ai/personas/party.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/personas/technician.py` & `persona_ai-0.1.1/persona_ai/personas/technician.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/personas/terminal.py` & `persona_ai-0.1.1/persona_ai/personas/terminal.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/prompt_templates/agent.jinja2` & `persona_ai-0.1.1/persona_ai/prompt_templates/agent.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/prompt_templates/coder.jinja2` & `persona_ai-0.1.1/persona_ai/prompt_templates/coder.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/prompt_templates/history_moderator.jinja2` & `persona_ai-0.1.1/persona_ai/prompt_templates/history_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/prompt_templates/history_moderator_fc.jinja2` & `persona_ai-0.1.1/persona_ai/prompt_templates/history_moderator_fc.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/prompt_templates/react_json_moderator.jinja2` & `persona_ai-0.1.1/persona_ai/prompt_templates/react_json_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/prompt_templates/react_moderator.jinja2` & `persona_ai-0.1.1/persona_ai/prompt_templates/react_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2` & `persona_ai-0.1.1/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2` & `persona_ai-0.1.1/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/prompts/jinja.py` & `persona_ai-0.1.1/persona_ai/prompts/jinja.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/prompts/text.py` & `persona_ai-0.1.1/persona_ai/prompts/text.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/refiners/request_refiner.py` & `persona_ai-0.1.1/persona_ai/refiners/request_refiner.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/task_manager/base.py` & `persona_ai-0.1.1/persona_ai/task_manager/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from persona_ai.domain.conversations import Message
-from persona_ai.domain.repositories import TasksRepository
+from persona_ai.domain.repositories import MongoTasksRepository
 from persona_ai.domain.tasks import Task, TaskStatus
 from persona_ai.domain.utils import create_id
 
 
 class TaskManager:
     """
     Task manager is responsible for managing tasks.
     """
 
-    tasks_repository: TasksRepository
+    tasks_repository: MongoTasksRepository
     """
     Repository used to store tasks.        
     """
 
-    def __init__(self, repository: TasksRepository):
+    def __init__(self, repository: MongoTasksRepository):
         self.tasks_repository = repository
 
     def get_pending_task(self, conversation_id: str) -> Task:
         """
         Get the pending task for the given conversation.
         """
         task = next(
```

### Comparing `persona_ai-0.1.0/persona_ai/tools/functional.py` & `persona_ai-0.1.1/persona_ai/tools/functional.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/tools/manager.py` & `persona_ai-0.1.1/persona_ai/tools/manager.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/transport/local/local_messagebus.py` & `persona_ai-0.1.1/persona_ai/transport/local/local_messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/transport/messagebus.py` & `persona_ai-0.1.1/persona_ai/transport/messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py` & `persona_ai-0.1.1/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/utils/crypto.py` & `persona_ai-0.1.1/persona_ai/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/persona_ai/utils/extractors.py` & `persona_ai-0.1.1/persona_ai/utils/extractors.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.0/pyproject.toml` & `persona_ai-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "persona_ai"
-version = "0.1.0"
+version = "0.1.1"
 description = "Persona is a groundbreaking distributed AI agent system utilizing Google Vertex AI's premier Large Language Models such as Gemini-pro, Text-Bison, and Code-Bison. Developed by Applica Software Guru, Persona is engineered for scalable, high-performance, and intelligent operations across various data sets and applications. It harnesses the power of Google's Vertex AI to deliver unmatched insights and automation capabilities, setting new standards in AI-driven analytics and decision-making processes"
 authors = ["Bruno Fortunato <bruno.fortunato@applica.guru>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `persona_ai-0.1.0/PKG-INFO` & `persona_ai-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persona_ai
-Version: 0.1.0
+Version: 0.1.1
 Summary: Persona is a groundbreaking distributed AI agent system utilizing Google Vertex AI's premier Large Language Models such as Gemini-pro, Text-Bison, and Code-Bison. Developed by Applica Software Guru, Persona is engineered for scalable, high-performance, and intelligent operations across various data sets and applications. It harnesses the power of Google's Vertex AI to deliver unmatched insights and automation capabilities, setting new standards in AI-driven analytics and decision-making processes
 License: MIT
 Author: Bruno Fortunato
 Author-email: bruno.fortunato@applica.guru
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
 Requires-Dist: pywhatkit (>=5.4,<6.0)
 Requires-Dist: shortuuid (>=1.0.12,<2.0.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Introduction
 
-Welcome to the exciting world of Persona AI, a cutting-edge framework designed for the development of generative
+****Welcome to the exciting world of Persona AI, a cutting-edge framework designed for the development of generative
 artificial intelligence applications that span multiple modes of interaction. Persona AI leverages the power of Google
 Vertex AI's generative models, placing it at the forefront of innovation in AI by offering a multimodal platform that
 integrates various forms of AI capabilities, from text to image generation, and beyond.
 
 At its core, Persona AI is a distributed agent system, characterized by its fully asynchronous nature. This means that
 communication among the agents is facilitated through a message bus, allowing for seamless and efficient exchanges of
 information. The agents in Persona AI work collaboratively in what is referred to as a "party," a dynamic group where
@@ -44,15 +44,15 @@
 also selected based on their declared scopes, ensuring that every contribution is meaningful and directed towards the
 collective goal.
 
 This introduction serves as your gateway into the world of Persona AI, where the blend of human ingenuity and artificial
 intelligence opens up new frontiers in technology and application development. Built on the robust and versatile
 foundation of Google Vertex AI's generative models, Persona AI is engineered to harness the capabilities of generative
 AI to create innovative and impactful solutions. Let's embark on this journey together, exploring the vast potentials of
-generative AI with Persona AI.
+generative AI with Persona AI.****
 
 # Party and Moderation in Persona AI
 
 The **Party** and **Moderation** systems within the Persona AI framework are pivotal in orchestrating the collaborative
 and decision-making dynamics essential for managing complex interactions and tasks. These components ensure that
 conversations are not just efficiently managed but also directed towards achieving the most relevant and
 context-appropriate outcomes.
```

