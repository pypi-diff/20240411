# Comparing `tmp/battleship_tui-0.9.0.tar.gz` & `tmp/battleship_tui-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battleship_tui-0.9.0.tar", max compression
+gzip compressed data, was "battleship_tui-0.9.1.tar", max compression
```

## Comparing `battleship_tui-0.9.0.tar` & `battleship_tui-0.9.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    18092 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/LICENSE
--rw-r--r--   0        0        0     2866 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/README.md
--rw-r--r--   0        0        0      548 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/__init__.py
--rw-r--r--   0        0        0       69 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/__main__.py
--rw-r--r--   0        0        0       54 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/cli/__init__.py
--rw-r--r--   0        0        0       73 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/cli/__main__.py
--rw-r--r--   0        0        0     2064 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/cli/account.py
--rw-r--r--   0        0        0     2143 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/cli/app.py
--rw-r--r--   0        0        0      638 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/cli/console.py
--rw-r--r--   0        0        0      562 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/cli/di.py
--rw-r--r--   0        0        0      190 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/cli/logging.py
--rw-r--r--   0        0        0     2652 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/cli/play.py
--rw-r--r--   0        0        0      561 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/client/__init__.py
--rw-r--r--   0        0        0      527 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/client/auth.py
--rw-r--r--   0        0        0    15516 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/client/client.py
--rw-r--r--   0        0        0     2267 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/client/credentials.py
--rw-r--r--   0        0        0     1422 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/client/subscriptions.py
--rw-r--r--   0        0        0      119 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/engine/__init__.py
--rw-r--r--   0        0        0     3687 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/engine/ai.py
--rw-r--r--   0        0        0      675 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/engine/api.py
--rw-r--r--   0        0        0    11866 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/engine/domain.py
--rw-r--r--   0        0        0      742 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/engine/errors.py
--rw-r--r--   0        0        0     2474 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/engine/roster.py
--rw-r--r--   0        0        0        0 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/py.typed
--rw-r--r--   0        0        0       71 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/__init__.py
--rw-r--r--   0        0        0     4198 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/app.py
--rw-r--r--   0        0        0     6557 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/auth.py
--rw-r--r--   0        0        0      690 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/config.py
--rw-r--r--   0        0        0       99 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/context.py
--rw-r--r--   0        0        0     7062 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/game.py
--rw-r--r--   0        0        0     5622 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/handlers.py
--rw-r--r--   0        0        0     2455 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/pubsub.py
--rw-r--r--   0        0        0      460 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/repositories/__init__.py
--rw-r--r--   0        0        0     4968 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/repositories/clients.py
--rw-r--r--   0        0        0     1277 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/repositories/observable.py
--rw-r--r--   0        0        0     4169 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/repositories/sessions.py
--rw-r--r--   0        0        0     2286 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/repositories/statistics.py
--rw-r--r--   0        0        0     7036 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/routes.py
--rw-r--r--   0        0        0     3674 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/server/websocket.py
--rw-r--r--   0        0        0        0 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/shared/__init__.py
--rw-r--r--   0        0        0     1421 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/shared/compat.py
--rw-r--r--   0        0        0      995 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/shared/events.py
--rw-r--r--   0        0        0     5836 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/shared/models.py
--rw-r--r--   0        0        0      173 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/tui/__init__.py
--rw-r--r--   0        0        0     8255 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/tui/app.py
--rw-r--r--   0        0        0      363 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/tui/config.py
--rw-r--r--   0        0        0      655 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/tui/format.py
--rw-r--r--   0        0        0      675 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/tui/resources/create_game_help.md
--rw-r--r--   0        0        0      416 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/tui/resources/lobby_help.md
--rw-r--r--   0        0        0      323 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/resources/multiplayer_help.md
--rw-r--r--   0        0        0      350 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/resources/settings_help.md
--rw-r--r--   0        0        0      586 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/resources/singleplayer_help.md
--rw-r--r--   0        0        0      369 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/resources/statistics_help.md
--rw-r--r--   0        0        0      163 2023-12-17 17:46:19.759494 battleship_tui-0.9.0/battleship/tui/resources.py
--rw-r--r--   0        0        0      651 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/screens/__init__.py
--rw-r--r--   0        0        0     1853 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/screens/create_game.py
--rw-r--r--   0        0        0     9455 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/screens/game.py
--rw-r--r--   0        0        0     4468 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/screens/join_game.py
--rw-r--r--   0        0        0     5106 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/screens/lobby.py
--rw-r--r--   0        0        0     1396 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/screens/main_menu.py
--rw-r--r--   0        0        0     5387 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/screens/multiplayer.py
--rw-r--r--   0        0        0     4552 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/screens/settings.py
--rw-r--r--   0        0        0     1948 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/screens/singleplayer.py
--rw-r--r--   0        0        0     1962 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/screens/statistics.py
--rw-r--r--   0        0        0     2453 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/settings.py
--rw-r--r--   0        0        0    10062 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/strategies.py
--rw-r--r--   0        0        0     2862 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/styles.tcss
--rw-r--r--   0        0        0      208 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/widgets/__init__.py
--rw-r--r--   0        0        0     2127 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/widgets/announcement.py
--rw-r--r--   0        0        0      312 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/widgets/battle_log.py
--rw-r--r--   0        0        0    13262 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/widgets/board.py
--rw-r--r--   0        0        0     4117 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/widgets/fleet.py
--rw-r--r--   0        0        0      411 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/widgets/footer.py
--rw-r--r--   0        0        0      674 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/widgets/lobby_header.py
--rw-r--r--   0        0        0     3587 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/widgets/modals.py
--rw-r--r--   0        0        0     3046 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/battleship/tui/widgets/new_game.py
--rw-r--r--   0        0        0     2453 2023-12-17 17:46:19.763494 battleship_tui-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5308 1970-01-01 00:00:00.000000 battleship_tui-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2866 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/README.md
+-rw-r--r--   0        0        0      548 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/__init__.py
+-rw-r--r--   0        0        0       69 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/__main__.py
+-rw-r--r--   0        0        0       54 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/cli/__init__.py
+-rw-r--r--   0        0        0       73 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/cli/__main__.py
+-rw-r--r--   0        0        0     2064 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/cli/account.py
+-rw-r--r--   0        0        0     2143 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/cli/app.py
+-rw-r--r--   0        0        0      638 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/cli/console.py
+-rw-r--r--   0        0        0      562 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/cli/di.py
+-rw-r--r--   0        0        0      190 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/cli/logging.py
+-rw-r--r--   0        0        0     2652 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/cli/play.py
+-rw-r--r--   0        0        0      561 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/client/__init__.py
+-rw-r--r--   0        0        0      527 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/client/auth.py
+-rw-r--r--   0        0        0    15516 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/client/client.py
+-rw-r--r--   0        0        0     2267 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/client/credentials.py
+-rw-r--r--   0        0        0     1422 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/client/subscriptions.py
+-rw-r--r--   0        0        0      119 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/engine/__init__.py
+-rw-r--r--   0        0        0     3687 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/engine/ai.py
+-rw-r--r--   0        0        0      675 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/engine/api.py
+-rw-r--r--   0        0        0    11866 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/engine/domain.py
+-rw-r--r--   0        0        0      742 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/engine/errors.py
+-rw-r--r--   0        0        0     2474 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/engine/roster.py
+-rw-r--r--   0        0        0        0 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/py.typed
+-rw-r--r--   0        0        0       71 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/server/__init__.py
+-rw-r--r--   0        0        0     4198 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/server/app.py
+-rw-r--r--   0        0        0     6557 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/server/auth.py
+-rw-r--r--   0        0        0      690 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/server/config.py
+-rw-r--r--   0        0        0       99 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/server/context.py
+-rw-r--r--   0        0        0     7062 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/server/game.py
+-rw-r--r--   0        0        0     5622 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/server/handlers.py
+-rw-r--r--   0        0        0     2455 2023-12-17 17:54:28.382954 battleship_tui-0.9.1/battleship/server/pubsub.py
+-rw-r--r--   0        0        0      460 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/server/repositories/__init__.py
+-rw-r--r--   0        0        0     4968 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/server/repositories/clients.py
+-rw-r--r--   0        0        0     1277 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/server/repositories/observable.py
+-rw-r--r--   0        0        0     4169 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/server/repositories/sessions.py
+-rw-r--r--   0        0        0     2286 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/server/repositories/statistics.py
+-rw-r--r--   0        0        0     7036 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/server/routes.py
+-rw-r--r--   0        0        0     3674 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/server/websocket.py
+-rw-r--r--   0        0        0        0 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/shared/__init__.py
+-rw-r--r--   0        0        0     1421 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/shared/compat.py
+-rw-r--r--   0        0        0      995 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/shared/events.py
+-rw-r--r--   0        0        0     5836 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/shared/models.py
+-rw-r--r--   0        0        0      173 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/__init__.py
+-rw-r--r--   0        0        0     8255 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/app.py
+-rw-r--r--   0        0        0      363 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/config.py
+-rw-r--r--   0        0        0      655 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/format.py
+-rw-r--r--   0        0        0      675 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/resources/create_game_help.md
+-rw-r--r--   0        0        0      416 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/resources/lobby_help.md
+-rw-r--r--   0        0        0      323 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/resources/multiplayer_help.md
+-rw-r--r--   0        0        0      350 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/resources/settings_help.md
+-rw-r--r--   0        0        0      586 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/resources/singleplayer_help.md
+-rw-r--r--   0        0        0      369 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/resources/statistics_help.md
+-rw-r--r--   0        0        0      163 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/resources.py
+-rw-r--r--   0        0        0      651 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/screens/__init__.py
+-rw-r--r--   0        0        0     1853 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/screens/create_game.py
+-rw-r--r--   0        0        0     9455 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/screens/game.py
+-rw-r--r--   0        0        0     4468 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/screens/join_game.py
+-rw-r--r--   0        0        0     5106 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/screens/lobby.py
+-rw-r--r--   0        0        0     1396 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/screens/main_menu.py
+-rw-r--r--   0        0        0     5387 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/screens/multiplayer.py
+-rw-r--r--   0        0        0     4552 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/screens/settings.py
+-rw-r--r--   0        0        0     1948 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/screens/singleplayer.py
+-rw-r--r--   0        0        0     1962 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/screens/statistics.py
+-rw-r--r--   0        0        0     2482 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/settings.py
+-rw-r--r--   0        0        0    10062 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/strategies.py
+-rw-r--r--   0        0        0     2862 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/styles.tcss
+-rw-r--r--   0        0        0      208 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/widgets/__init__.py
+-rw-r--r--   0        0        0     2127 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/widgets/announcement.py
+-rw-r--r--   0        0        0      312 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/widgets/battle_log.py
+-rw-r--r--   0        0        0    13262 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/widgets/board.py
+-rw-r--r--   0        0        0     4117 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/widgets/fleet.py
+-rw-r--r--   0        0        0      411 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/widgets/footer.py
+-rw-r--r--   0        0        0      674 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/widgets/lobby_header.py
+-rw-r--r--   0        0        0     3587 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/widgets/modals.py
+-rw-r--r--   0        0        0     3046 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/battleship/tui/widgets/new_game.py
+-rw-r--r--   0        0        0     2453 2023-12-17 17:54:28.386954 battleship_tui-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5308 1970-01-01 00:00:00.000000 battleship_tui-0.9.1/PKG-INFO
```

### Comparing `battleship_tui-0.9.0/LICENSE` & `battleship_tui-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/README.md` & `battleship_tui-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/__init__.py` & `battleship_tui-0.9.1/battleship/__init__.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/cli/account.py` & `battleship_tui-0.9.1/battleship/cli/account.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/cli/app.py` & `battleship_tui-0.9.1/battleship/cli/app.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/cli/console.py` & `battleship_tui-0.9.1/battleship/cli/console.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/cli/di.py` & `battleship_tui-0.9.1/battleship/cli/di.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/cli/play.py` & `battleship_tui-0.9.1/battleship/cli/play.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/client/__init__.py` & `battleship_tui-0.9.1/battleship/client/__init__.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/client/auth.py` & `battleship_tui-0.9.1/battleship/client/auth.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/client/client.py` & `battleship_tui-0.9.1/battleship/client/client.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/client/credentials.py` & `battleship_tui-0.9.1/battleship/client/credentials.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/client/subscriptions.py` & `battleship_tui-0.9.1/battleship/client/subscriptions.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/engine/ai.py` & `battleship_tui-0.9.1/battleship/engine/ai.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/engine/api.py` & `battleship_tui-0.9.1/battleship/engine/api.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/engine/domain.py` & `battleship_tui-0.9.1/battleship/engine/domain.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/engine/errors.py` & `battleship_tui-0.9.1/battleship/engine/errors.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/engine/roster.py` & `battleship_tui-0.9.1/battleship/engine/roster.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/server/app.py` & `battleship_tui-0.9.1/battleship/server/app.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/server/auth.py` & `battleship_tui-0.9.1/battleship/server/auth.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/server/config.py` & `battleship_tui-0.9.1/battleship/server/config.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/server/game.py` & `battleship_tui-0.9.1/battleship/server/game.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/server/handlers.py` & `battleship_tui-0.9.1/battleship/server/handlers.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/server/pubsub.py` & `battleship_tui-0.9.1/battleship/server/pubsub.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/server/repositories/clients.py` & `battleship_tui-0.9.1/battleship/server/repositories/clients.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/server/repositories/observable.py` & `battleship_tui-0.9.1/battleship/server/repositories/observable.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/server/repositories/sessions.py` & `battleship_tui-0.9.1/battleship/server/repositories/sessions.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/server/repositories/statistics.py` & `battleship_tui-0.9.1/battleship/server/repositories/statistics.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/server/routes.py` & `battleship_tui-0.9.1/battleship/server/routes.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/server/websocket.py` & `battleship_tui-0.9.1/battleship/server/websocket.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/shared/compat.py` & `battleship_tui-0.9.1/battleship/shared/compat.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/shared/events.py` & `battleship_tui-0.9.1/battleship/shared/events.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/shared/models.py` & `battleship_tui-0.9.1/battleship/shared/models.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/app.py` & `battleship_tui-0.9.1/battleship/tui/app.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/format.py` & `battleship_tui-0.9.1/battleship/tui/format.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/resources/create_game_help.md` & `battleship_tui-0.9.1/battleship/tui/resources/create_game_help.md`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/resources/singleplayer_help.md` & `battleship_tui-0.9.1/battleship/tui/resources/singleplayer_help.md`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/screens/__init__.py` & `battleship_tui-0.9.1/battleship/tui/screens/__init__.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/screens/create_game.py` & `battleship_tui-0.9.1/battleship/tui/screens/create_game.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/screens/game.py` & `battleship_tui-0.9.1/battleship/tui/screens/game.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/screens/join_game.py` & `battleship_tui-0.9.1/battleship/tui/screens/join_game.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/screens/lobby.py` & `battleship_tui-0.9.1/battleship/tui/screens/lobby.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/screens/main_menu.py` & `battleship_tui-0.9.1/battleship/tui/screens/main_menu.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/screens/multiplayer.py` & `battleship_tui-0.9.1/battleship/tui/screens/multiplayer.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/screens/settings.py` & `battleship_tui-0.9.1/battleship/tui/screens/settings.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/screens/singleplayer.py` & `battleship_tui-0.9.1/battleship/tui/screens/singleplayer.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/screens/statistics.py` & `battleship_tui-0.9.1/battleship/tui/screens/statistics.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/settings.py` & `battleship_tui-0.9.1/battleship/tui/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import re
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Annotated, Any
 
-from pydantic import AfterValidator
+from pydantic import AfterValidator, Field
 
 from battleship import config_home
 from battleship.shared.models import BaseModel
 
 hex_color = re.compile(r"^#([0-9a-f]{6})$")
 
 
@@ -20,15 +20,15 @@
     return value
 
 
 HexColor = Annotated[str, AfterValidator(validate_color)]
 
 
 class Settings(BaseModel):
-    player_name: str = "Player"
+    player_name: str = Field("Player", max_length=19)
     fleet_color: HexColor = "#36aa5e"
     enemy_fleet_color: HexColor = "#0065be"
     language: str = "English"
 
     @property
     def language_options(self) -> list[str]:
         return ["English"]
```

### Comparing `battleship_tui-0.9.0/battleship/tui/strategies.py` & `battleship_tui-0.9.1/battleship/tui/strategies.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/styles.tcss` & `battleship_tui-0.9.1/battleship/tui/styles.tcss`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/widgets/announcement.py` & `battleship_tui-0.9.1/battleship/tui/widgets/announcement.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/widgets/board.py` & `battleship_tui-0.9.1/battleship/tui/widgets/board.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/widgets/fleet.py` & `battleship_tui-0.9.1/battleship/tui/widgets/fleet.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/widgets/lobby_header.py` & `battleship_tui-0.9.1/battleship/tui/widgets/lobby_header.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/widgets/modals.py` & `battleship_tui-0.9.1/battleship/tui/widgets/modals.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/battleship/tui/widgets/new_game.py` & `battleship_tui-0.9.1/battleship/tui/widgets/new_game.py`

 * *Files identical despite different names*

### Comparing `battleship_tui-0.9.0/pyproject.toml` & `battleship_tui-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "battleship-tui"
-version = "0.9.0"
+version = "0.9.1"
 description = "Battleship TUI is an implementation of the popular paper-and-pen Battleship game for your terminal."
 authors = ["Roman Vlasenko <klavionik@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/Klavionik/battleship-tui"
 license = "GPL-2.0-or-later"
 keywords = ["battleship", "game", "tui"]
 classifiers = [
```

### Comparing `battleship_tui-0.9.0/PKG-INFO` & `battleship_tui-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battleship-tui
-Version: 0.9.0
+Version: 0.9.1
 Summary: Battleship TUI is an implementation of the popular paper-and-pen Battleship game for your terminal.
 Home-page: https://github.com/Klavionik/battleship-tui
 License: GPL-2.0-or-later
 Keywords: battleship,game,tui
 Author: Roman Vlasenko
 Author-email: klavionik@gmail.com
 Requires-Python: >=3.10,<4.0
```

