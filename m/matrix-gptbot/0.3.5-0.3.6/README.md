# Comparing `tmp/matrix_gptbot-0.3.5.tar.gz` & `tmp/matrix_gptbot-0.3.6.tar.gz`

## Comparing `matrix_gptbot-0.3.5.tar` & `matrix_gptbot-0.3.6.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/.gitlab-ci.yml
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/CHANGELOG.md
--rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/config.dist.ini
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/gptbot-pantalaimon.service
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/gptbot.service
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/pantalaimon.example.conf
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/pantalaimon_first_login.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/.vscode/launch.json
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/__init__.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/__main__.py
--rw-r--r--   0        0        0   190295 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/assets/logo.png
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/callbacks/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/callbacks/invite.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/callbacks/join.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/callbacks/message.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/callbacks/roommember.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/callbacks/sync.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/callbacks/test.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/callbacks/test_response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/classes/__init__.py
--rw-r--r--   0        0        0    45207 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/classes/bot.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/classes/dict.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/classes/logging.py
--rw-r--r--   0        0        0    25750 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/classes/openai.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/classes/trackingmore.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/classes/wolframalpha.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/__init__.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/botinfo.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/calculate.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/chat.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/classify.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/coin.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/custom.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/dice.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/help.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/ignoreolder.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/imagine.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/newroom.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/parcel.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/privacy.py
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/roomsettings.py
--rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/space.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/stats.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/systemmessage.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/tts.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/commands/unknown.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/migrations/__init__.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/migrations/migration_1.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/migrations/migration_2.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/migrations/migration_3.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/migrations/migration_4.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/migrations/migration_5.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/migrations/migration_6.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/migrations/migration_7.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/migrations/migration_8.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/tools/__init__.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/tools/base.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/tools/datetime.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/tools/dice.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/tools/geocode.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/tools/imagedescription.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/tools/imagine.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/tools/newroom.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/tools/weather.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/tools/webrequest.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/tools/websearch.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/src/gptbot/tools/wikipedia.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/LICENSE
--rw-r--r--   0        0        0     8355 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/README.md
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/pyproject.toml
--rw-r--r--   0        0        0    10902 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/CHANGELOG.md
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/config.dist.ini
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/gptbot-pantalaimon.service
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/gptbot.service
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/pantalaimon.example.conf
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/pantalaimon_first_login.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/.vscode/launch.json
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/__init__.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/__main__.py
+-rw-r--r--   0        0        0   190295 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/assets/logo.png
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/invite.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/join.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/message.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/roommember.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/sync.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/test.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/test_response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/__init__.py
+-rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/bot.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/dict.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/logging.py
+-rw-r--r--   0        0        0    25750 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/openai.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/trackingmore.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/wolframalpha.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/__init__.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/botinfo.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/calculate.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/chat.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/classify.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/coin.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/custom.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/dice.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/help.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/ignoreolder.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/imagine.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/newroom.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/parcel.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/privacy.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/roomsettings.py
+-rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/space.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/stats.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/systemmessage.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/tts.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/unknown.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/__init__.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_1.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_2.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_3.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_4.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_5.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_6.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_7.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_8.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/__init__.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/base.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/datetime.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/dice.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/geocode.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/imagedescription.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/imagine.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/newroom.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/weather.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/webrequest.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/websearch.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/wikipedia.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/LICENSE
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/README.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0    10910 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/PKG-INFO
```

### Comparing `matrix_gptbot-0.3.5/config.dist.ini` & `matrix_gptbot-0.3.6/config.dist.ini`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/__main__.py` & `matrix_gptbot-0.3.6/src/gptbot/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 def get_version():
     try:
         package_version = pkg_resources.get_distribution("matrix_gptbot").version
     except pkg_resources.DistributionNotFound:
         return None
     return package_version
 
-
-if __name__ == "__main__":
+def main():
     # Parse command line arguments
     parser = ArgumentParser()
     parser.add_argument(
         "--config",
         "-c",
         help="Path to config file (default: config.ini in working directory)",
         default="config.ini",
@@ -49,7 +48,11 @@
     # Start bot
     try:
         asyncio.run(bot.run())
     except KeyboardInterrupt:
         print("Received KeyboardInterrupt - exiting...")
     except SystemExit:
         print("Received SIGTERM - exiting...")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `matrix_gptbot-0.3.5/src/gptbot/assets/logo.png` & `matrix_gptbot-0.3.6/src/gptbot/assets/logo.png`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/callbacks/__init__.py` & `matrix_gptbot-0.3.6/src/gptbot/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/callbacks/join.py` & `matrix_gptbot-0.3.6/src/gptbot/callbacks/join.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/callbacks/message.py` & `matrix_gptbot-0.3.6/src/gptbot/callbacks/message.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/classes/bot.py` & `matrix_gptbot-0.3.6/src/gptbot/classes/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     RoomMessageImage,
     RoomMessageFile,
     RoomMessageAudio,
     DownloadError,
     DownloadResponse,
     ToDeviceEvent,
     ToDeviceError,
+    RoomGetStateError,
 )
 from nio.store import SqliteStore
 
 
 from typing import Optional, List
 from configparser import ConfigParser
 from datetime import datetime
@@ -316,33 +317,44 @@
         if isinstance(response, RoomMessagesError):
             raise Exception(
                 f"Error fetching messages: {response.message} (status code {response.status_code})",
                 "error",
             )
 
         for event in response.chunk:
-            if len(messages) >= n:
-                break
+            try:
+                event_type = event.type
+            except AttributeError:
+                try:
+                    event_type = event.source["content"]["msgtype"]
+                except KeyError:
+                    self.logger.log(f"Could not process event: {event}", "debug")
+                    continue # This is most likely not a message event
 
-            if event.type.startswith("gptbot"):
+            if event_type.startswith("gptbot"):
                 messages.append(event)
 
             elif isinstance(event, RoomMessageText):
                 if event.body.split() == ["!gptbot", "ignoreolder"]:
                     break
-                if (not event.body.startswith("!")) or (event.body.split()[1] == "custom"):
+                if (not event.body.startswith("!")) or (
+                    event.body.split()[1] == "custom"
+                ):
                     messages.append(event)
 
             elif isinstance(event, RoomMessageNotice):
                 if not ignore_notices:
                     messages.append(event)
 
             elif isinstance(event, RoomMessageMedia):
                 messages.append(event)
 
+            if len(messages) >= n:
+                break
+
         self.logger.log(f"Found {len(messages)} messages (limit: {n})", "debug")
 
         # Reverse the list so that messages are in chronological order
         return messages[::-1]
 
     def _truncate(
         self,
@@ -808,14 +820,30 @@
             room = room.room_id
 
         self.database.execute(
             "INSERT INTO token_usage (message_id, room_id, tokens, api, timestamp) VALUES (?, ?, ?, ?, ?)",
             (message, room, tokens, api, datetime.now()),
         )
 
+    async def get_state_event(
+        self, room: MatrixRoom | str, event_type: str, state_key: Optional[str] = None
+    ):
+        if isinstance(room, MatrixRoom):
+            room = room.room_id
+
+        state = await self.matrix_client.room_get_state(room)
+
+        if isinstance(state, RoomGetStateError):
+            self.logger.log(f"Could not get state for room {room}")
+
+        for event in state.events:
+            if event["type"] == event_type:
+                if state_key is None or event["state_key"] == state_key:
+                    return event
+
     async def run(self):
         """Start the bot."""
 
         # Set up the Matrix client
 
         assert self.matrix_client, "Matrix client not set up"
         assert self.matrix_client.access_token, "Access token not set up"
@@ -886,20 +914,22 @@
                 logo_bio.getvalue(), "logo", Image.MIME[self.logo.format]
             )
             self.logo_uri = uri
 
             asyncio.create_task(self.matrix_client.set_avatar(uri))
 
             for room in self.matrix_client.rooms.keys():
-                self.logger.log(f"Setting avatar for {room}...", "debug")
-                asyncio.create_task(
-                    self.matrix_client.room_put_state(
-                        room, "m.room.avatar", {"url": uri}, ""
+                room_avatar = await self.get_state_event(room, "m.room.avatar")
+                if not room_avatar:
+                    self.logger.log(f"Setting avatar for {room}...", "debug")
+                    asyncio.create_task(
+                        self.matrix_client.room_put_state(
+                            room, "m.room.avatar", {"url": uri}, ""
+                        )
                     )
-                )
 
         # Start syncing events
         self.logger.log("Starting sync loop...", "warning")
         try:
             await self.matrix_client.sync_forever(timeout=30000, full_state=True)
         finally:
             self.logger.log("Syncing one last time...", "warning")
```

### Comparing `matrix_gptbot-0.3.5/src/gptbot/classes/logging.py` & `matrix_gptbot-0.3.6/src/gptbot/classes/logging.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/classes/openai.py` & `matrix_gptbot-0.3.6/src/gptbot/classes/openai.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/classes/trackingmore.py` & `matrix_gptbot-0.3.6/src/gptbot/classes/trackingmore.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/classes/wolframalpha.py` & `matrix_gptbot-0.3.6/src/gptbot/classes/wolframalpha.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/__init__.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/botinfo.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/botinfo.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/calculate.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/calculate.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/classify.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/classify.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/dice.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/dice.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/help.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/help.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/imagine.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/imagine.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/newroom.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/newroom.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/parcel.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/parcel.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/privacy.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/privacy.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/roomsettings.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/roomsettings.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/space.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/space.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/stats.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/stats.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/systemmessage.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/systemmessage.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/commands/tts.py` & `matrix_gptbot-0.3.6/src/gptbot/commands/tts.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/migrations/__init__.py` & `matrix_gptbot-0.3.6/src/gptbot/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/migrations/migration_1.py` & `matrix_gptbot-0.3.6/src/gptbot/migrations/migration_1.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/migrations/migration_3.py` & `matrix_gptbot-0.3.6/src/gptbot/migrations/migration_3.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/migrations/migration_5.py` & `matrix_gptbot-0.3.6/src/gptbot/migrations/migration_5.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/migrations/migration_6.py` & `matrix_gptbot-0.3.6/src/gptbot/migrations/migration_6.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/migrations/migration_7.py` & `matrix_gptbot-0.3.6/src/gptbot/migrations/migration_7.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/migrations/migration_8.py` & `matrix_gptbot-0.3.6/src/gptbot/migrations/migration_8.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/tools/base.py` & `matrix_gptbot-0.3.6/src/gptbot/tools/base.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/tools/dice.py` & `matrix_gptbot-0.3.6/src/gptbot/tools/dice.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/tools/geocode.py` & `matrix_gptbot-0.3.6/src/gptbot/tools/geocode.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/tools/imagine.py` & `matrix_gptbot-0.3.6/src/gptbot/tools/imagine.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/tools/newroom.py` & `matrix_gptbot-0.3.6/src/gptbot/tools/newroom.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/tools/weather.py` & `matrix_gptbot-0.3.6/src/gptbot/tools/weather.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/tools/webrequest.py` & `matrix_gptbot-0.3.6/src/gptbot/tools/webrequest.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/tools/websearch.py` & `matrix_gptbot-0.3.6/src/gptbot/tools/websearch.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/src/gptbot/tools/wikipedia.py` & `matrix_gptbot-0.3.6/src/gptbot/tools/wikipedia.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/LICENSE` & `matrix_gptbot-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.5/README.md` & `matrix_gptbot-0.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 pip install matrix-gptbot[all]
 ```
 
 This will install the latest release of the bot and all required dependencies
 for all available features.
 
-You can also use `pip install git+https://kumig.it/kumitterer/matrix-gptbot.git`
+You can also use `pip install git+https://git.private.coffee/kumi/matrix-gptbot.git`
 to install the latest version from the Git repository.
 
 #### End-to-end encryption
 
 WARNING: Using end-to-end encryption seems to sometimes cause problems with
 file attachments, especially in rooms that are not encrypted, if the same
 user also uses the bot in encrypted rooms.
@@ -76,15 +76,15 @@
 ### Development
 
 Clone the repository and install the requirements to a virtual environment.
 
 ```shell
 # Clone the repository
 
-git clone https://kumig.it/kumitterer/matrix-gptbot.git
+git clone https://git.private.coffee/kumi/matrix-gptbot.git
 cd matrix-gptbot
 
 # If desired, activate a venv first
 
 python -m venv venv
 . venv/bin/activate
```

### Comparing `matrix_gptbot-0.3.5/pyproject.toml` & `matrix_gptbot-0.3.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "matrix-gptbot"
-version = "0.3.5"
+version = "0.3.6"
 
 authors = [
   { name="Kumi Mitterer", email="gptbot@kumi.email" },
 ]
 
 description = "Multifunctional Chatbot for Matrix"
 readme = "README.md"
@@ -65,11 +65,11 @@
 ]
 
 [project.urls]
 "Homepage" = "https://kumig.it/kumitterer/matrix-gptbot"
 "Bug Tracker" = "https://kumig.it/kumitterer/matrix-gptbot/issues"
 
 [project.scripts]
-gptbot = "gptbot:main"
+gptbot = "gptbot.__main__:main"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/gptbot"]
```

### Comparing `matrix_gptbot-0.3.5/PKG-INFO` & `matrix_gptbot-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: matrix-gptbot
-Version: 0.3.5
+Version: 0.3.6
 Summary: Multifunctional Chatbot for Matrix
 Project-URL: Homepage, https://kumig.it/kumitterer/matrix-gptbot
 Project-URL: Bug Tracker, https://kumig.it/kumitterer/matrix-gptbot/issues
 Author-email: Kumi Mitterer <gptbot@kumi.email>
 License: Copyright (c) 2023 Kumi Mitterer <gptbot@kumi.email>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -96,15 +96,15 @@
 
 pip install matrix-gptbot[all]
 ```
 
 This will install the latest release of the bot and all required dependencies
 for all available features.
 
-You can also use `pip install git+https://kumig.it/kumitterer/matrix-gptbot.git`
+You can also use `pip install git+https://git.private.coffee/kumi/matrix-gptbot.git`
 to install the latest version from the Git repository.
 
 #### End-to-end encryption
 
 WARNING: Using end-to-end encryption seems to sometimes cause problems with
 file attachments, especially in rooms that are not encrypted, if the same
 user also uses the bot in encrypted rooms.
@@ -131,15 +131,15 @@
 ### Development
 
 Clone the repository and install the requirements to a virtual environment.
 
 ```shell
 # Clone the repository
 
-git clone https://kumig.it/kumitterer/matrix-gptbot.git
+git clone https://git.private.coffee/kumi/matrix-gptbot.git
 cd matrix-gptbot
 
 # If desired, activate a venv first
 
 python -m venv venv
 . venv/bin/activate
```

