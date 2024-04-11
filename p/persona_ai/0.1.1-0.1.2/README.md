# Comparing `tmp/persona_ai-0.1.1.tar.gz` & `tmp/persona_ai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persona_ai-0.1.1.tar", max compression
+gzip compressed data, was "persona_ai-0.1.2.tar", max compression
```

## Comparing `persona_ai-0.1.1.tar` & `persona_ai-0.1.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    11250 2024-04-11 07:56:25.206198 persona_ai-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/code_runners/__init__.py
--rw-r--r--   0        0        0     1239 2024-04-08 14:44:21.457123 persona_ai-0.1.1/persona_ai/code_runners/base.py
--rw-r--r--   0        0        0     2363 2024-04-08 14:39:06.291886 persona_ai-0.1.1/persona_ai/code_runners/local.py
--rw-r--r--   0        0        0      153 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/constants.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/conversation_listeners/__init__.py
--rw-r--r--   0        0        0     5954 2024-04-08 14:44:22.237126 persona_ai-0.1.1/persona_ai/conversation_listeners/terminal.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/conversations/__init__.py
--rw-r--r--   0        0        0     3214 2024-04-11 08:13:50.184451 persona_ai-0.1.1/persona_ai/conversations/manager.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/__init__.py
--rw-r--r--   0        0        0     6372 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/conversations.py
--rw-r--r--   0        0        0      767 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/events.py
--rw-r--r--   0        0        0     1172 2024-04-11 08:14:55.564773 persona_ai-0.1.1/persona_ai/domain/repositories.py
--rw-r--r--   0        0        0       82 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/roles.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/schemas/__init__.py
--rw-r--r--   0        0        0      600 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/schemas/crud.py
--rw-r--r--   0        0        0     2759 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/tasks.py
--rw-r--r--   0        0        0      146 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/domain/utils.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/infrastructure/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/infrastructure/repositories/__init__.py
--rw-r--r--   0        0        0      758 2024-04-08 14:47:42.829922 persona_ai-0.1.1/persona_ai/infrastructure/repositories/base.py
--rw-r--r--   0        0        0     1967 2024-04-11 08:19:46.530087 persona_ai-0.1.1/persona_ai/infrastructure/repositories/in_memory.py
--rw-r--r--   0        0        0     2884 2024-04-08 14:47:42.249920 persona_ai-0.1.1/persona_ai/infrastructure/repositories/mongo.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/initializers/__init__.py
--rw-r--r--   0        0        0     4183 2024-04-11 08:14:57.764784 persona_ai-0.1.1/persona_ai/initializers/env_configurator.py
--rw-r--r--   0        0        0     1012 2024-04-11 08:13:23.084313 persona_ai-0.1.1/persona_ai/initializers/persona_configuration.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/models/__init__.py
--rw-r--r--   0        0        0      870 2024-04-08 14:48:27.882101 persona_ai-0.1.1/persona_ai/models/base.py
--rw-r--r--   0        0        0     2591 2024-04-08 14:48:27.834101 persona_ai-0.1.1/persona_ai/models/code_bison.py
--rw-r--r--   0        0        0    10094 2024-04-08 14:48:35.922133 persona_ai-0.1.1/persona_ai/models/gemini.py
--rw-r--r--   0        0        0     2591 2024-04-08 14:48:36.366135 persona_ai-0.1.1/persona_ai/models/text_bison.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/moderation/__init__.py
--rw-r--r--   0        0        0     2842 2024-04-08 14:50:20.986552 persona_ai-0.1.1/persona_ai/moderation/ai_moderator.py
--rw-r--r--   0        0        0     7345 2024-04-08 14:51:53.450921 persona_ai-0.1.1/persona_ai/moderation/base.py
--rw-r--r--   0        0        0     4475 2024-04-08 14:51:53.978923 persona_ai-0.1.1/persona_ai/moderation/history_moderator.py
--rw-r--r--   0        0        0     4759 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/moderation/history_moderator_fc.py
--rw-r--r--   0        0        0     5580 2024-04-08 14:51:53.474921 persona_ai-0.1.1/persona_ai/moderation/react_moderator.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/personas/__init__.py
--rw-r--r--   0        0        0     6678 2024-04-08 14:54:32.699557 persona_ai-0.1.1/persona_ai/personas/agent.py
--rw-r--r--   0        0        0     4124 2024-04-11 08:16:44.105284 persona_ai-0.1.1/persona_ai/personas/assistant.py
--rw-r--r--   0        0        0     6507 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/personas/base.py
--rw-r--r--   0        0        0     3805 2024-04-11 08:16:44.125284 persona_ai-0.1.1/persona_ai/personas/coder.py
--rw-r--r--   0        0        0    13266 2024-04-08 14:58:31.431608 persona_ai-0.1.1/persona_ai/personas/party.py
--rw-r--r--   0        0        0     3022 2024-04-08 14:58:32.183662 persona_ai-0.1.1/persona_ai/personas/technician.py
--rw-r--r--   0        0        0      760 2024-04-08 15:00:26.392475 persona_ai-0.1.1/persona_ai/personas/terminal.py
--rw-r--r--   0        0        0      860 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/agent.jinja2
--rw-r--r--   0        0        0      413 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/assistant.jinja2
--rw-r--r--   0        0        0     1009 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/coder.jinja2
--rw-r--r--   0        0        0     1076 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/history_moderator.jinja2
--rw-r--r--   0        0        0     1062 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/history_moderator_fc.jinja2
--rw-r--r--   0        0        0     1776 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/react_json_moderator.jinja2
--rw-r--r--   0        0        0     1083 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/react_moderator.jinja2
--rw-r--r--   0        0        0      330 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/refiner.jinja2
--rw-r--r--   0        0        0      946 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2
--rw-r--r--   0        0        0      841 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2
--rw-r--r--   0        0        0      123 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompt_templates/technician.jinja2
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/prompts/__init__.py
--rw-r--r--   0        0        0      238 2024-04-08 14:58:32.179662 persona_ai-0.1.1/persona_ai/prompts/base.py
--rw-r--r--   0        0        0     2207 2024-04-08 15:00:26.384474 persona_ai-0.1.1/persona_ai/prompts/jinja.py
--rw-r--r--   0        0        0      588 2024-04-08 14:58:32.167661 persona_ai-0.1.1/persona_ai/prompts/text.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/refiners/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/refiners/request_refiner.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/task_manager/__init__.py
--rw-r--r--   0        0        0     2263 2024-04-11 08:13:22.660311 persona_ai-0.1.1/persona_ai/task_manager/base.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/tools/__init__.py
--rw-r--r--   0        0        0      469 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/tools/base.py
--rw-r--r--   0        0        0     1746 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/tools/functional.py
--rw-r--r--   0        0        0      730 2024-04-08 15:00:26.376474 persona_ai-0.1.1/persona_ai/tools/manager.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/transport/__init__.py
--rw-r--r--   0        0        0     2576 2024-04-08 15:00:34.632689 persona_ai-0.1.1/persona_ai/transport/local/local_messagebus.py
--rw-r--r--   0        0        0     4022 2024-04-08 14:44:21.469123 persona_ai-0.1.1/persona_ai/transport/messagebus.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/transport/rabbitmq/__init__.py
--rw-r--r--   0        0        0    10002 2024-04-08 15:01:04.409617 persona_ai-0.1.1/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/utils/__init__.py
--rw-r--r--   0        0        0      723 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/utils/crypto.py
--rw-r--r--   0        0        0      750 2024-04-08 06:52:52.049183 persona_ai-0.1.1/persona_ai/utils/extractors.py
--rw-r--r--   0        0        0     1120 2024-04-11 07:37:50.746837 persona_ai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    12755 1970-01-01 00:00:00.000000 persona_ai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11250 2024-04-11 07:56:25.206198 persona_ai-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/code_runners/__init__.py
+-rw-r--r--   0        0        0     1239 2024-04-08 14:44:21.457123 persona_ai-0.1.2/persona_ai/code_runners/base.py
+-rw-r--r--   0        0        0     2363 2024-04-08 14:39:06.291886 persona_ai-0.1.2/persona_ai/code_runners/local.py
+-rw-r--r--   0        0        0      153 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/constants.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/conversation_listeners/__init__.py
+-rw-r--r--   0        0        0     5954 2024-04-08 14:44:22.237126 persona_ai-0.1.2/persona_ai/conversation_listeners/terminal.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/conversations/__init__.py
+-rw-r--r--   0        0        0     3214 2024-04-11 08:13:50.184451 persona_ai-0.1.2/persona_ai/conversations/manager.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/domain/__init__.py
+-rw-r--r--   0        0        0     6372 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/domain/conversations.py
+-rw-r--r--   0        0        0      767 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/domain/events.py
+-rw-r--r--   0        0        0     1172 2024-04-11 08:14:55.564773 persona_ai-0.1.2/persona_ai/domain/repositories.py
+-rw-r--r--   0        0        0       82 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/domain/roles.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/domain/schemas/__init__.py
+-rw-r--r--   0        0        0      600 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/domain/schemas/crud.py
+-rw-r--r--   0        0        0     2759 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/domain/tasks.py
+-rw-r--r--   0        0        0      146 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/domain/utils.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/infrastructure/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/infrastructure/repositories/__init__.py
+-rw-r--r--   0        0        0      758 2024-04-08 14:47:42.829922 persona_ai-0.1.2/persona_ai/infrastructure/repositories/base.py
+-rw-r--r--   0        0        0     1967 2024-04-11 08:19:46.530087 persona_ai-0.1.2/persona_ai/infrastructure/repositories/in_memory.py
+-rw-r--r--   0        0        0     2884 2024-04-08 14:47:42.249920 persona_ai-0.1.2/persona_ai/infrastructure/repositories/mongo.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/initializers/__init__.py
+-rw-r--r--   0        0        0     4130 2024-04-11 08:26:55.195797 persona_ai-0.1.2/persona_ai/initializers/env_configurator.py
+-rw-r--r--   0        0        0     1012 2024-04-11 08:13:23.084313 persona_ai-0.1.2/persona_ai/initializers/persona_configuration.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/models/__init__.py
+-rw-r--r--   0        0        0      870 2024-04-08 14:48:27.882101 persona_ai-0.1.2/persona_ai/models/base.py
+-rw-r--r--   0        0        0     2591 2024-04-08 14:48:27.834101 persona_ai-0.1.2/persona_ai/models/code_bison.py
+-rw-r--r--   0        0        0    10094 2024-04-08 14:48:35.922133 persona_ai-0.1.2/persona_ai/models/gemini.py
+-rw-r--r--   0        0        0     2591 2024-04-08 14:48:36.366135 persona_ai-0.1.2/persona_ai/models/text_bison.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/moderation/__init__.py
+-rw-r--r--   0        0        0     2842 2024-04-08 14:50:20.986552 persona_ai-0.1.2/persona_ai/moderation/ai_moderator.py
+-rw-r--r--   0        0        0     7345 2024-04-08 14:51:53.450921 persona_ai-0.1.2/persona_ai/moderation/base.py
+-rw-r--r--   0        0        0     4475 2024-04-08 14:51:53.978923 persona_ai-0.1.2/persona_ai/moderation/history_moderator.py
+-rw-r--r--   0        0        0     4759 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/moderation/history_moderator_fc.py
+-rw-r--r--   0        0        0     5580 2024-04-08 14:51:53.474921 persona_ai-0.1.2/persona_ai/moderation/react_moderator.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/personas/__init__.py
+-rw-r--r--   0        0        0     6678 2024-04-08 14:54:32.699557 persona_ai-0.1.2/persona_ai/personas/agent.py
+-rw-r--r--   0        0        0     4124 2024-04-11 08:16:44.105284 persona_ai-0.1.2/persona_ai/personas/assistant.py
+-rw-r--r--   0        0        0     6507 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/personas/base.py
+-rw-r--r--   0        0        0     3805 2024-04-11 08:16:44.125284 persona_ai-0.1.2/persona_ai/personas/coder.py
+-rw-r--r--   0        0        0    13266 2024-04-08 14:58:31.431608 persona_ai-0.1.2/persona_ai/personas/party.py
+-rw-r--r--   0        0        0     3022 2024-04-08 14:58:32.183662 persona_ai-0.1.2/persona_ai/personas/technician.py
+-rw-r--r--   0        0        0      760 2024-04-08 15:00:26.392475 persona_ai-0.1.2/persona_ai/personas/terminal.py
+-rw-r--r--   0        0        0      860 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/prompt_templates/agent.jinja2
+-rw-r--r--   0        0        0      413 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/prompt_templates/assistant.jinja2
+-rw-r--r--   0        0        0     1009 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/prompt_templates/coder.jinja2
+-rw-r--r--   0        0        0     1076 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/prompt_templates/history_moderator.jinja2
+-rw-r--r--   0        0        0     1062 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/prompt_templates/history_moderator_fc.jinja2
+-rw-r--r--   0        0        0     1776 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/prompt_templates/react_json_moderator.jinja2
+-rw-r--r--   0        0        0     1083 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/prompt_templates/react_moderator.jinja2
+-rw-r--r--   0        0        0      330 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/prompt_templates/refiner.jinja2
+-rw-r--r--   0        0        0      946 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2
+-rw-r--r--   0        0        0      841 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2
+-rw-r--r--   0        0        0      123 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/prompt_templates/technician.jinja2
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/prompts/__init__.py
+-rw-r--r--   0        0        0      238 2024-04-08 14:58:32.179662 persona_ai-0.1.2/persona_ai/prompts/base.py
+-rw-r--r--   0        0        0     2207 2024-04-08 15:00:26.384474 persona_ai-0.1.2/persona_ai/prompts/jinja.py
+-rw-r--r--   0        0        0      588 2024-04-08 14:58:32.167661 persona_ai-0.1.2/persona_ai/prompts/text.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/refiners/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/refiners/request_refiner.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/task_manager/__init__.py
+-rw-r--r--   0        0        0     2263 2024-04-11 08:13:22.660311 persona_ai-0.1.2/persona_ai/task_manager/base.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/tools/__init__.py
+-rw-r--r--   0        0        0      469 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/tools/base.py
+-rw-r--r--   0        0        0     1746 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/tools/functional.py
+-rw-r--r--   0        0        0      730 2024-04-08 15:00:26.376474 persona_ai-0.1.2/persona_ai/tools/manager.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/transport/__init__.py
+-rw-r--r--   0        0        0     2576 2024-04-08 15:00:34.632689 persona_ai-0.1.2/persona_ai/transport/local/local_messagebus.py
+-rw-r--r--   0        0        0     4022 2024-04-08 14:44:21.469123 persona_ai-0.1.2/persona_ai/transport/messagebus.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/transport/rabbitmq/__init__.py
+-rw-r--r--   0        0        0    10002 2024-04-08 15:01:04.409617 persona_ai-0.1.2/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/utils/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/utils/crypto.py
+-rw-r--r--   0        0        0      750 2024-04-08 06:52:52.049183 persona_ai-0.1.2/persona_ai/utils/extractors.py
+-rw-r--r--   0        0        0     1120 2024-04-11 08:28:16.776105 persona_ai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    12755 1970-01-01 00:00:00.000000 persona_ai-0.1.2/PKG-INFO
```

### Comparing `persona_ai-0.1.1/README.md` & `persona_ai-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/code_runners/base.py` & `persona_ai-0.1.2/persona_ai/code_runners/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/code_runners/local.py` & `persona_ai-0.1.2/persona_ai/code_runners/local.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/conversation_listeners/terminal.py` & `persona_ai-0.1.2/persona_ai/conversation_listeners/terminal.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/conversations/manager.py` & `persona_ai-0.1.2/persona_ai/conversations/manager.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/domain/conversations.py` & `persona_ai-0.1.2/persona_ai/domain/conversations.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/domain/events.py` & `persona_ai-0.1.2/persona_ai/domain/events.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/domain/repositories.py` & `persona_ai-0.1.2/persona_ai/domain/repositories.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/domain/schemas/crud.py` & `persona_ai-0.1.2/persona_ai/domain/schemas/crud.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/domain/tasks.py` & `persona_ai-0.1.2/persona_ai/domain/tasks.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/infrastructure/repositories/base.py` & `persona_ai-0.1.2/persona_ai/infrastructure/repositories/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/infrastructure/repositories/in_memory.py` & `persona_ai-0.1.2/persona_ai/infrastructure/repositories/in_memory.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/infrastructure/repositories/mongo.py` & `persona_ai-0.1.2/persona_ai/infrastructure/repositories/mongo.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/initializers/env_configurator.py` & `persona_ai-0.1.2/persona_ai/initializers/env_configurator.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,51 +55,49 @@
     elif message_bus_type == "local":
         return LocalMessageBus()
     else:
         raise ValueError("Invalid message bus type: {}".format(message_bus_type))
 
 
 def configure_conversations_repository():
-    if os.getenv("REPOSITORIES_TYPE") == "mongodb":
+    if _get_repository_type() == "mongodb":
         return MongoConversationsRepository()
-    elif os.getenv("REPOSITORIES_TYPE") == "in-memory":
+    elif _get_repository_type() == "in-memory":
         return InMemoryConversationsRepository()
     else:
-        raise ValueError(
-            "Invalid repository type: {}".format(os.getenv("REPOSITORIES_TYPE"))
-        )
+        raise ValueError("Invalid repository type: {}".format(_get_repository_type()))
 
 
 def configure_messages_repository():
-    if os.getenv("REPOSITORIES_TYPE") == "mongodb":
+    if _get_repository_type() == "mongodb":
         return MongoMessagesRepository()
-    elif os.getenv("REPOSITORIES_TYPE") == "in-memory":
+    elif _get_repository_type() == "in-memory":
         return InMemoryMessagesRepository()
     else:
-        raise ValueError(
-            "Invalid repository type: {}".format(os.getenv("REPOSITORIES_TYPE"))
-        )
+        raise ValueError("Invalid repository type: {}".format(_get_repository_type()))
 
 
 def configure_conversation_manager():
     return ConversationManager(
         conversations_repository=PersonaAI.conversations_repository,
         messages_repository=PersonaAI.messages_repository,
     )
 
 
 def configure_tasks_repository():
-    if os.getenv("REPOSITORIES_TYPE") == "mongodb":
+    if _get_repository_type() == "mongodb":
         return MongoTasksRepository()
-    elif os.getenv("REPOSITORIES_TYPE") == "in-memory":
+    elif _get_repository_type() == "in-memory":
         return InMemoryTasksRepository()
     else:
-        raise ValueError(
-            "Invalid repository type: {}".format(os.getenv("REPOSITORIES_TYPE"))
-        )
+        raise ValueError("Invalid repository type: {}".format(_get_repository_type()))
+
+
+def _get_repository_type():
+    return os.getenv("REPOSITORIES_TYPE", "in-memory")
 
 
 def configure_persona_from_env():
     """Configure a persona_ai system from environment variables."""
 
     PersonaAI.moderator_model = configure_model("MODERATOR")
     PersonaAI.assistant_model = configure_model("ASSISTANT")
```

### Comparing `persona_ai-0.1.1/persona_ai/initializers/persona_configuration.py` & `persona_ai-0.1.2/persona_ai/initializers/persona_configuration.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/models/base.py` & `persona_ai-0.1.2/persona_ai/models/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/models/code_bison.py` & `persona_ai-0.1.2/persona_ai/models/code_bison.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/models/gemini.py` & `persona_ai-0.1.2/persona_ai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/models/text_bison.py` & `persona_ai-0.1.2/persona_ai/models/text_bison.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/moderation/ai_moderator.py` & `persona_ai-0.1.2/persona_ai/moderation/ai_moderator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/moderation/base.py` & `persona_ai-0.1.2/persona_ai/moderation/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/moderation/history_moderator.py` & `persona_ai-0.1.2/persona_ai/moderation/history_moderator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/moderation/history_moderator_fc.py` & `persona_ai-0.1.2/persona_ai/moderation/history_moderator_fc.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/moderation/react_moderator.py` & `persona_ai-0.1.2/persona_ai/moderation/react_moderator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/personas/agent.py` & `persona_ai-0.1.2/persona_ai/personas/agent.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/personas/assistant.py` & `persona_ai-0.1.2/persona_ai/personas/assistant.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/personas/base.py` & `persona_ai-0.1.2/persona_ai/personas/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/personas/coder.py` & `persona_ai-0.1.2/persona_ai/personas/coder.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/personas/party.py` & `persona_ai-0.1.2/persona_ai/personas/party.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/personas/technician.py` & `persona_ai-0.1.2/persona_ai/personas/technician.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/personas/terminal.py` & `persona_ai-0.1.2/persona_ai/personas/terminal.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/prompt_templates/agent.jinja2` & `persona_ai-0.1.2/persona_ai/prompt_templates/agent.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/prompt_templates/coder.jinja2` & `persona_ai-0.1.2/persona_ai/prompt_templates/coder.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/prompt_templates/history_moderator.jinja2` & `persona_ai-0.1.2/persona_ai/prompt_templates/history_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/prompt_templates/history_moderator_fc.jinja2` & `persona_ai-0.1.2/persona_ai/prompt_templates/history_moderator_fc.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/prompt_templates/react_json_moderator.jinja2` & `persona_ai-0.1.2/persona_ai/prompt_templates/react_json_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/prompt_templates/react_moderator.jinja2` & `persona_ai-0.1.2/persona_ai/prompt_templates/react_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2` & `persona_ai-0.1.2/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2` & `persona_ai-0.1.2/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/prompts/jinja.py` & `persona_ai-0.1.2/persona_ai/prompts/jinja.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/prompts/text.py` & `persona_ai-0.1.2/persona_ai/prompts/text.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/refiners/request_refiner.py` & `persona_ai-0.1.2/persona_ai/refiners/request_refiner.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/task_manager/base.py` & `persona_ai-0.1.2/persona_ai/task_manager/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/tools/functional.py` & `persona_ai-0.1.2/persona_ai/tools/functional.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/tools/manager.py` & `persona_ai-0.1.2/persona_ai/tools/manager.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/transport/local/local_messagebus.py` & `persona_ai-0.1.2/persona_ai/transport/local/local_messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/transport/messagebus.py` & `persona_ai-0.1.2/persona_ai/transport/messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py` & `persona_ai-0.1.2/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/utils/crypto.py` & `persona_ai-0.1.2/persona_ai/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/persona_ai/utils/extractors.py` & `persona_ai-0.1.2/persona_ai/utils/extractors.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.1/pyproject.toml` & `persona_ai-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "persona_ai"
-version = "0.1.1"
+version = "0.1.2"
 description = "Persona is a groundbreaking distributed AI agent system utilizing Google Vertex AI's premier Large Language Models such as Gemini-pro, Text-Bison, and Code-Bison. Developed by Applica Software Guru, Persona is engineered for scalable, high-performance, and intelligent operations across various data sets and applications. It harnesses the power of Google's Vertex AI to deliver unmatched insights and automation capabilities, setting new standards in AI-driven analytics and decision-making processes"
 authors = ["Bruno Fortunato <bruno.fortunato@applica.guru>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `persona_ai-0.1.1/PKG-INFO` & `persona_ai-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persona_ai
-Version: 0.1.1
+Version: 0.1.2
 Summary: Persona is a groundbreaking distributed AI agent system utilizing Google Vertex AI's premier Large Language Models such as Gemini-pro, Text-Bison, and Code-Bison. Developed by Applica Software Guru, Persona is engineered for scalable, high-performance, and intelligent operations across various data sets and applications. It harnesses the power of Google's Vertex AI to deliver unmatched insights and automation capabilities, setting new standards in AI-driven analytics and decision-making processes
 License: MIT
 Author: Bruno Fortunato
 Author-email: bruno.fortunato@applica.guru
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

