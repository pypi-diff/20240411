# Comparing `tmp/persona_ai-0.1.5.tar.gz` & `tmp/persona_ai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persona_ai-0.1.5.tar", max compression
+gzip compressed data, was "persona_ai-0.1.6.tar", max compression
```

## Comparing `persona_ai-0.1.5.tar` & `persona_ai-0.1.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    11250 2024-04-11 10:00:15.400629 persona_ai-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/code_runners/__init__.py
--rw-r--r--   0        0        0     1239 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/code_runners/base.py
--rw-r--r--   0        0        0     2363 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/code_runners/local.py
--rw-r--r--   0        0        0      153 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/constants.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/conversation_listeners/__init__.py
--rw-r--r--   0        0        0     5963 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/conversation_listeners/terminal.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/conversations/__init__.py
--rw-r--r--   0        0        0     3214 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/conversations/manager.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/domain/__init__.py
--rw-r--r--   0        0        0     6372 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/domain/conversations.py
--rw-r--r--   0        0        0      767 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/domain/events.py
--rw-r--r--   0        0        0     1172 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/domain/repositories.py
--rw-r--r--   0        0        0       82 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/domain/roles.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/domain/schemas/__init__.py
--rw-r--r--   0        0        0      600 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/domain/schemas/crud.py
--rw-r--r--   0        0        0     2759 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/domain/tasks.py
--rw-r--r--   0        0        0      146 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/domain/utils.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/infrastructure/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/infrastructure/repositories/__init__.py
--rw-r--r--   0        0        0      758 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/infrastructure/repositories/base.py
--rw-r--r--   0        0        0     1967 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/infrastructure/repositories/in_memory.py
--rw-r--r--   0        0        0     2884 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/infrastructure/repositories/mongo.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/initializers/__init__.py
--rw-r--r--   0        0        0     4362 2024-04-11 10:13:24.751773 persona_ai-0.1.5/persona_ai/initializers/env_configurator.py
--rw-r--r--   0        0        0     1012 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/initializers/persona_configuration.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/models/__init__.py
--rw-r--r--   0        0        0      870 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/models/base.py
--rw-r--r--   0        0        0     2591 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/models/code_bison.py
--rw-r--r--   0        0        0    10093 2024-04-11 10:10:57.959178 persona_ai-0.1.5/persona_ai/models/gemini.py
--rw-r--r--   0        0        0     2591 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/models/text_bison.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/moderation/__init__.py
--rw-r--r--   0        0        0     2842 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/moderation/ai_moderator.py
--rw-r--r--   0        0        0     7345 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/moderation/base.py
--rw-r--r--   0        0        0     4475 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/moderation/history_moderator.py
--rw-r--r--   0        0        0     4759 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/moderation/history_moderator_fc.py
--rw-r--r--   0        0        0     5580 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/moderation/react_moderator.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/personas/__init__.py
--rw-r--r--   0        0        0     6678 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/personas/agent.py
--rw-r--r--   0        0        0     4221 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/personas/assistant.py
--rw-r--r--   0        0        0     6507 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/personas/base.py
--rw-r--r--   0        0        0     3805 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/personas/coder.py
--rw-r--r--   0        0        0    13266 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/personas/party.py
--rw-r--r--   0        0        0     3022 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/personas/technician.py
--rw-r--r--   0        0        0      760 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/personas/terminal.py
--rw-r--r--   0        0        0      860 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/prompt_templates/agent.jinja2
--rw-r--r--   0        0        0      413 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/prompt_templates/assistant.jinja2
--rw-r--r--   0        0        0     1009 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/prompt_templates/coder.jinja2
--rw-r--r--   0        0        0     1076 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/prompt_templates/history_moderator.jinja2
--rw-r--r--   0        0        0     1062 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/prompt_templates/history_moderator_fc.jinja2
--rw-r--r--   0        0        0     1776 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/prompt_templates/react_json_moderator.jinja2
--rw-r--r--   0        0        0     1083 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/prompt_templates/react_moderator.jinja2
--rw-r--r--   0        0        0      330 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/prompt_templates/refiner.jinja2
--rw-r--r--   0        0        0      946 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2
--rw-r--r--   0        0        0      841 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2
--rw-r--r--   0        0        0      123 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/prompt_templates/technician.jinja2
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/prompts/__init__.py
--rw-r--r--   0        0        0      238 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/prompts/base.py
--rw-r--r--   0        0        0     2207 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/prompts/jinja.py
--rw-r--r--   0        0        0      588 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/prompts/text.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/refiners/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/refiners/request_refiner.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/task_manager/__init__.py
--rw-r--r--   0        0        0     2263 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/task_manager/base.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/tools/__init__.py
--rw-r--r--   0        0        0      469 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/tools/base.py
--rw-r--r--   0        0        0     1746 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/tools/functional.py
--rw-r--r--   0        0        0      730 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/tools/manager.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/transport/__init__.py
--rw-r--r--   0        0        0     2576 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/transport/local/local_messagebus.py
--rw-r--r--   0        0        0     4022 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/transport/messagebus.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/transport/rabbitmq/__init__.py
--rw-r--r--   0        0        0    10002 2024-04-11 10:00:15.400629 persona_ai-0.1.5/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/utils/__init__.py
--rw-r--r--   0        0        0      723 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/utils/crypto.py
--rw-r--r--   0        0        0      750 2024-04-08 06:52:52.049183 persona_ai-0.1.5/persona_ai/utils/extractors.py
--rw-r--r--   0        0        0     1120 2024-04-11 10:14:15.811981 persona_ai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    12755 1970-01-01 00:00:00.000000 persona_ai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11250 2024-04-11 10:00:15.400629 persona_ai-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/code_runners/__init__.py
+-rw-r--r--   0        0        0     1239 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/code_runners/base.py
+-rw-r--r--   0        0        0     2363 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/code_runners/local.py
+-rw-r--r--   0        0        0      153 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/constants.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/conversation_listeners/__init__.py
+-rw-r--r--   0        0        0     5963 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/conversation_listeners/terminal.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/conversations/__init__.py
+-rw-r--r--   0        0        0     3214 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/conversations/manager.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/domain/__init__.py
+-rw-r--r--   0        0        0     6372 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/domain/conversations.py
+-rw-r--r--   0        0        0      767 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/domain/events.py
+-rw-r--r--   0        0        0     1172 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/domain/repositories.py
+-rw-r--r--   0        0        0       82 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/domain/roles.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/domain/schemas/__init__.py
+-rw-r--r--   0        0        0      600 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/domain/schemas/crud.py
+-rw-r--r--   0        0        0     2759 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/domain/tasks.py
+-rw-r--r--   0        0        0      146 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/domain/utils.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/infrastructure/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/infrastructure/repositories/__init__.py
+-rw-r--r--   0        0        0      758 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/infrastructure/repositories/base.py
+-rw-r--r--   0        0        0     1967 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/infrastructure/repositories/in_memory.py
+-rw-r--r--   0        0        0     2884 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/infrastructure/repositories/mongo.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/initializers/__init__.py
+-rw-r--r--   0        0        0     4362 2024-04-11 10:13:24.751773 persona_ai-0.1.6/persona_ai/initializers/env_configurator.py
+-rw-r--r--   0        0        0     1012 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/initializers/persona_configuration.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/models/__init__.py
+-rw-r--r--   0        0        0      870 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/models/base.py
+-rw-r--r--   0        0        0     2591 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/models/code_bison.py
+-rw-r--r--   0        0        0    10093 2024-04-11 10:10:57.959178 persona_ai-0.1.6/persona_ai/models/gemini.py
+-rw-r--r--   0        0        0     2591 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/models/text_bison.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/moderation/__init__.py
+-rw-r--r--   0        0        0     2842 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/moderation/ai_moderator.py
+-rw-r--r--   0        0        0     7345 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/moderation/base.py
+-rw-r--r--   0        0        0     4475 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/moderation/history_moderator.py
+-rw-r--r--   0        0        0     4759 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/moderation/history_moderator_fc.py
+-rw-r--r--   0        0        0     5580 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/moderation/react_moderator.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/personas/__init__.py
+-rw-r--r--   0        0        0     6678 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/personas/agent.py
+-rw-r--r--   0        0        0     4221 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/personas/assistant.py
+-rw-r--r--   0        0        0     6507 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/personas/base.py
+-rw-r--r--   0        0        0     3805 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/personas/coder.py
+-rw-r--r--   0        0        0    13266 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/personas/party.py
+-rw-r--r--   0        0        0     3022 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/personas/technician.py
+-rw-r--r--   0        0        0      760 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/personas/terminal.py
+-rw-r--r--   0        0        0      860 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/prompt_templates/agent.jinja2
+-rw-r--r--   0        0        0      413 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/prompt_templates/assistant.jinja2
+-rw-r--r--   0        0        0     1009 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/prompt_templates/coder.jinja2
+-rw-r--r--   0        0        0     1076 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/prompt_templates/history_moderator.jinja2
+-rw-r--r--   0        0        0     1062 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/prompt_templates/history_moderator_fc.jinja2
+-rw-r--r--   0        0        0     1776 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/prompt_templates/react_json_moderator.jinja2
+-rw-r--r--   0        0        0     1083 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/prompt_templates/react_moderator.jinja2
+-rw-r--r--   0        0        0      330 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/prompt_templates/refiner.jinja2
+-rw-r--r--   0        0        0      946 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2
+-rw-r--r--   0        0        0      841 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2
+-rw-r--r--   0        0        0      123 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/prompt_templates/technician.jinja2
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/prompts/__init__.py
+-rw-r--r--   0        0        0      238 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/prompts/base.py
+-rw-r--r--   0        0        0     2207 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/prompts/jinja.py
+-rw-r--r--   0        0        0      588 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/prompts/text.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/refiners/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/refiners/request_refiner.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/task_manager/__init__.py
+-rw-r--r--   0        0        0     2263 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/task_manager/base.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/tools/__init__.py
+-rw-r--r--   0        0        0      469 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/tools/base.py
+-rw-r--r--   0        0        0     1746 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/tools/functional.py
+-rw-r--r--   0        0        0      730 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/tools/manager.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/transport/__init__.py
+-rw-r--r--   0        0        0     3475 2024-04-11 10:30:15.213567 persona_ai-0.1.6/persona_ai/transport/local/local_messagebus.py
+-rw-r--r--   0        0        0     4022 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/transport/messagebus.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/transport/rabbitmq/__init__.py
+-rw-r--r--   0        0        0    10002 2024-04-11 10:00:15.400629 persona_ai-0.1.6/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/utils/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/utils/crypto.py
+-rw-r--r--   0        0        0      750 2024-04-08 06:52:52.049183 persona_ai-0.1.6/persona_ai/utils/extractors.py
+-rw-r--r--   0        0        0     1120 2024-04-11 10:29:51.249441 persona_ai-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    12755 1970-01-01 00:00:00.000000 persona_ai-0.1.6/PKG-INFO
```

### Comparing `persona_ai-0.1.5/README.md` & `persona_ai-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/code_runners/base.py` & `persona_ai-0.1.6/persona_ai/code_runners/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/code_runners/local.py` & `persona_ai-0.1.6/persona_ai/code_runners/local.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/conversation_listeners/terminal.py` & `persona_ai-0.1.6/persona_ai/conversation_listeners/terminal.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/conversations/manager.py` & `persona_ai-0.1.6/persona_ai/conversations/manager.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/domain/conversations.py` & `persona_ai-0.1.6/persona_ai/domain/conversations.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/domain/events.py` & `persona_ai-0.1.6/persona_ai/domain/events.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/domain/repositories.py` & `persona_ai-0.1.6/persona_ai/domain/repositories.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/domain/schemas/crud.py` & `persona_ai-0.1.6/persona_ai/domain/schemas/crud.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/domain/tasks.py` & `persona_ai-0.1.6/persona_ai/domain/tasks.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/infrastructure/repositories/base.py` & `persona_ai-0.1.6/persona_ai/infrastructure/repositories/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/infrastructure/repositories/in_memory.py` & `persona_ai-0.1.6/persona_ai/infrastructure/repositories/in_memory.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/infrastructure/repositories/mongo.py` & `persona_ai-0.1.6/persona_ai/infrastructure/repositories/mongo.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/initializers/env_configurator.py` & `persona_ai-0.1.6/persona_ai/initializers/env_configurator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/initializers/persona_configuration.py` & `persona_ai-0.1.6/persona_ai/initializers/persona_configuration.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/models/base.py` & `persona_ai-0.1.6/persona_ai/models/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/models/code_bison.py` & `persona_ai-0.1.6/persona_ai/models/code_bison.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/models/gemini.py` & `persona_ai-0.1.6/persona_ai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/models/text_bison.py` & `persona_ai-0.1.6/persona_ai/models/text_bison.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/moderation/ai_moderator.py` & `persona_ai-0.1.6/persona_ai/moderation/ai_moderator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/moderation/base.py` & `persona_ai-0.1.6/persona_ai/moderation/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/moderation/history_moderator.py` & `persona_ai-0.1.6/persona_ai/moderation/history_moderator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/moderation/history_moderator_fc.py` & `persona_ai-0.1.6/persona_ai/moderation/history_moderator_fc.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/moderation/react_moderator.py` & `persona_ai-0.1.6/persona_ai/moderation/react_moderator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/personas/agent.py` & `persona_ai-0.1.6/persona_ai/personas/agent.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/personas/assistant.py` & `persona_ai-0.1.6/persona_ai/personas/assistant.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/personas/base.py` & `persona_ai-0.1.6/persona_ai/personas/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/personas/coder.py` & `persona_ai-0.1.6/persona_ai/personas/coder.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/personas/party.py` & `persona_ai-0.1.6/persona_ai/personas/party.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/personas/technician.py` & `persona_ai-0.1.6/persona_ai/personas/technician.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/personas/terminal.py` & `persona_ai-0.1.6/persona_ai/personas/terminal.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/prompt_templates/agent.jinja2` & `persona_ai-0.1.6/persona_ai/prompt_templates/agent.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/prompt_templates/coder.jinja2` & `persona_ai-0.1.6/persona_ai/prompt_templates/coder.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/prompt_templates/history_moderator.jinja2` & `persona_ai-0.1.6/persona_ai/prompt_templates/history_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/prompt_templates/history_moderator_fc.jinja2` & `persona_ai-0.1.6/persona_ai/prompt_templates/history_moderator_fc.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/prompt_templates/react_json_moderator.jinja2` & `persona_ai-0.1.6/persona_ai/prompt_templates/react_json_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/prompt_templates/react_moderator.jinja2` & `persona_ai-0.1.6/persona_ai/prompt_templates/react_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2` & `persona_ai-0.1.6/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2` & `persona_ai-0.1.6/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/prompts/jinja.py` & `persona_ai-0.1.6/persona_ai/prompts/jinja.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/prompts/text.py` & `persona_ai-0.1.6/persona_ai/prompts/text.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/refiners/request_refiner.py` & `persona_ai-0.1.6/persona_ai/refiners/request_refiner.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/task_manager/base.py` & `persona_ai-0.1.6/persona_ai/task_manager/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/tools/functional.py` & `persona_ai-0.1.6/persona_ai/tools/functional.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/tools/manager.py` & `persona_ai-0.1.6/persona_ai/tools/manager.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/transport/local/local_messagebus.py` & `persona_ai-0.1.6/persona_ai/transport/local/local_messagebus.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,35 @@
 from typing import List
 
 from persona_ai.domain.conversations import Message
 from persona_ai.transport.messagebus import (
     MessageBus,
     Participant,
     Event,
+    ConversationListener,
 )
 
 
 class LocalSubscription:
     """
     This class represents a local subscription.
     """
 
     participant: Participant
     """The participant."""
+    is_listener: bool = False
+    """Is the participant a listener."""
+    conversation_id: str = None
+    """The conversation ID."""
 
     def __init__(self, participant: Participant):
         self.participant = participant
+        if isinstance(participant, ConversationListener):
+            self.is_listener = True
+            self.conversation_id = participant.conversation_id
 
     def handle_message(self, message: Message):
         self.participant.last_activity = time.time()
         self.participant.receive(message)
 
     def handle_event(self, event: Event):
         self.participant.last_activity = time.time()
@@ -70,19 +78,34 @@
     def stop(self) -> threading.Event:
         self.running = False
         event = threading.Event()
         event.set()
         return event
 
     def publish_message(self, message: Message, recipient_id: str, **kwargs):
+        for subscription in self.subscriptions:
+            if (
+                subscription.is_listener
+                and message.conversation_id == subscription.conversation_id
+            ):
+                subscription.handle_message(message)
+
         subscription = next(
             filter(lambda s: s.participant.id == recipient_id, self.subscriptions),
             None,
         )
         subscription.handle_message(message)
 
     def publish_event(self, event: Event, recipient_id: str | None = None, **kwargs):
-        subscription = next(
-            filter(lambda s: s.participant.id == recipient_id, self.subscriptions),
-            None,
-        )
-        subscription.handle_event(event)
+        if not recipient_id:
+            for subscription in self.subscriptions:
+                if (
+                    subscription.is_listener
+                    and event.conversation_id == subscription.conversation_id
+                ):
+                    subscription.handle_event(event)
+        else:
+            subscription = next(
+                filter(lambda s: s.participant.id == recipient_id, self.subscriptions),
+                None,
+            )
+            subscription.handle_event(event)
```

### Comparing `persona_ai-0.1.5/persona_ai/transport/messagebus.py` & `persona_ai-0.1.6/persona_ai/transport/messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py` & `persona_ai-0.1.6/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/utils/crypto.py` & `persona_ai-0.1.6/persona_ai/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/persona_ai/utils/extractors.py` & `persona_ai-0.1.6/persona_ai/utils/extractors.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.5/pyproject.toml` & `persona_ai-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "persona_ai"
-version = "0.1.5"
+version = "0.1.6"
 description = "Persona is a groundbreaking distributed AI agent system utilizing Google Vertex AI's premier Large Language Models such as Gemini-pro, Text-Bison, and Code-Bison. Developed by Applica Software Guru, Persona is engineered for scalable, high-performance, and intelligent operations across various data sets and applications. It harnesses the power of Google's Vertex AI to deliver unmatched insights and automation capabilities, setting new standards in AI-driven analytics and decision-making processes"
 authors = ["Bruno Fortunato <bruno.fortunato@applica.guru>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `persona_ai-0.1.5/PKG-INFO` & `persona_ai-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persona_ai
-Version: 0.1.5
+Version: 0.1.6
 Summary: Persona is a groundbreaking distributed AI agent system utilizing Google Vertex AI's premier Large Language Models such as Gemini-pro, Text-Bison, and Code-Bison. Developed by Applica Software Guru, Persona is engineered for scalable, high-performance, and intelligent operations across various data sets and applications. It harnesses the power of Google's Vertex AI to deliver unmatched insights and automation capabilities, setting new standards in AI-driven analytics and decision-making processes
 License: MIT
 Author: Bruno Fortunato
 Author-email: bruno.fortunato@applica.guru
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

