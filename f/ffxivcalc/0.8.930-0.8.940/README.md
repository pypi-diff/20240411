# Comparing `tmp/ffxivcalc-0.8.930.tar.gz` & `tmp/ffxivcalc-0.8.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffxivcalc-0.8.930.tar", last modified: Sat Mar 30 20:59:15 2024, max compression
+gzip compressed data, was "ffxivcalc-0.8.940.tar", last modified: Thu Apr 11 01:07:15 2024, max compression
```

## Comparing `ffxivcalc-0.8.930.tar` & `ffxivcalc-0.8.940.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.574914 ffxivcalc-0.8.930/
--rw-rw-rw-   0        0        0     1096 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/License.md
--rw-rw-rw-   0        0        0     8696 2024-03-30 20:59:15.573913 ffxivcalc-0.8.930/PKG-INFO
--rw-rw-rw-   0        0        0     7509 2023-12-05 18:54:48.000000 ffxivcalc-0.8.930/README.md
--rw-rw-rw-   0        0        0       99 2023-12-05 18:34:38.000000 ffxivcalc-0.8.930/pyproject.toml
--rw-rw-rw-   0        0        0       84 2024-03-30 20:59:15.576914 ffxivcalc-0.8.930/setup.cfg
--rw-rw-rw-   0        0        0     1904 2024-03-30 20:57:25.000000 ffxivcalc-0.8.930/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:14.953705 ffxivcalc-0.8.930/src/
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.030792 ffxivcalc-0.8.930/src/ffxivcalc/
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.067800 ffxivcalc-0.8.930/src/ffxivcalc/API/
--rw-rw-rw-   0        0        0     1291 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/API/API.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.081804 ffxivcalc-0.8.930/src/ffxivcalc/API/Model/
--rw-rw-rw-   0        0        0     1331 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/API/Model/ObjectInModel.py
--rw-rw-rw-   0        0        0     1166 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/API/Model/ObjectOutModel.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/API/Model/__init__.py
--rw-rw-rw-   0        0        0      245 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/API/__init__.py
--rw-rw-rw-   0        0        0    11300 2023-08-12 03:23:31.000000 ffxivcalc-0.8.930/src/ffxivcalc/API/library.py
--rw-rw-rw-   0        0        0     8898 2024-03-05 03:10:39.000000 ffxivcalc-0.8.930/src/ffxivcalc/Enemy.py
--rw-rw-rw-   0        0        0    61879 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/Fight.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.102808 ffxivcalc-0.8.930/src/ffxivcalc/GearSolver/
--rw-rw-rw-   0        0        0    25433 2024-01-08 22:21:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/GearSolver/Gear.py
--rw-rw-rw-   0        0        0    60331 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/GearSolver/Solver.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/GearSolver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.143818 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/
--rw-rw-rw-   0        0        0    18461 2024-03-20 21:34:42.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/ActionEnum.py
--rw-rw-rw-   0        0        0    41438 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Base_Spell.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.153820 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.162822 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Blackmage/
--rw-rw-rw-   0        0        0    16913 2024-03-05 23:41:51.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Blackmage/BlackMage_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Blackmage/__init__.py
--rw-rw-rw-   0        0        0     5683 2024-03-20 18:07:50.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Caster_Spell.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.173824 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Redmage/
--rw-rw-rw-   0        0        0    14685 2023-11-22 02:47:02.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Redmage/Redmage_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Redmage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.183826 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Summoner/
--rw-rw-rw-   0        0        0    11920 2024-03-16 17:05:29.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Summoner/Summoner_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Summoner/__init__.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.192828 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.202831 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Astrologian/
--rw-rw-rw-   0        0        0    16171 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Astrologian/Astrologian_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Astrologian/__init__.py
--rw-rw-rw-   0        0        0     3452 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Healer_Spell.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.212833 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Sage/
--rw-rw-rw-   0        0        0     8218 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Sage/Sage_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Sage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.222835 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Scholar/
--rw-rw-rw-   0        0        0    10628 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Scholar/Scholar_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Scholar/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.226837 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Whitemage/
--rw-rw-rw-   0        0        0     7110 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Whitemage/Whitemage_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Whitemage/__init__.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.230838 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.240840 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Dragoon/
--rw-rw-rw-   0        0        0    14354 2023-11-30 18:40:07.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Dragoon/Dragoon_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Dragoon/__init__.py
--rw-rw-rw-   0        0        0     5502 2024-03-20 18:07:12.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Melee_Spell.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.251842 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Monk/
--rw-rw-rw-   0        0        0    17329 2023-11-25 23:09:24.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Monk/Monk_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Monk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.261844 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Ninja/
--rw-rw-rw-   0        0        0    21455 2024-02-10 19:14:06.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Ninja/Ninja_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Ninja/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.272846 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Reaper/
--rw-rw-rw-   0        0        0    16669 2023-11-22 02:47:02.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Reaper/Reaper_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Reaper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.281849 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Samurai/
--rw-rw-rw-   0        0        0    17033 2024-02-07 02:58:18.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Samurai/Samurai_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Samurai/__init__.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/__init__.py
--rw-rw-rw-   0        0        0   147483 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Player.py
--rw-rw-rw-   0        0        0     1299 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/PlayerEnum.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.291852 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.301854 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Bard/
--rw-rw-rw-   0        0        0    21886 2024-03-14 04:10:36.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Bard/Bard_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Bard/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.311856 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Dancer/
--rw-rw-rw-   0        0        0    17215 2024-03-20 21:35:16.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Dancer/Dancer_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Dancer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.320857 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Machinist/
--rw-rw-rw-   0        0        0    15778 2024-03-20 19:51:31.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Machinist/Machinist_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Machinist/__init__.py
--rw-rw-rw-   0        0        0     3367 2024-03-20 18:09:32.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Ranged_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.330859 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.340861 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/DarkKnight/
--rw-rw-rw-   0        0        0    14726 2024-02-10 19:14:06.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/DarkKnight/DarkKnight_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/DarkKnight/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.350864 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Gunbreaker/
--rw-rw-rw-   0        0        0    10822 2024-02-08 00:30:27.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Gunbreaker/Gunbreaker_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Gunbreaker/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.360866 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Paladin/
--rw-rw-rw-   0        0        0    15029 2024-02-08 23:33:24.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Paladin/Paladin_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Paladin/__init__.py
--rw-rw-rw-   0        0        0     7494 2024-03-20 16:27:29.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Tank_Spell.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.371869 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Warrior/
--rw-rw-rw-   0        0        0    11972 2024-02-08 01:51:53.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Warrior/Warrior_Spell.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Warrior/__init__.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/__init__.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Jobs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.428882 ffxivcalc-0.8.930/src/ffxivcalc/Request/
--rw-rw-rw-   0        0        0    31419 2024-03-22 16:37:41.000000 ffxivcalc-0.8.930/src/ffxivcalc/Request/FFLogsAPIRequest.py
--rw-rw-rw-   0        0        0    25158 2024-03-22 20:15:47.000000 ffxivcalc-0.8.930/src/ffxivcalc/Request/FFLogs_api.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Request/__init__.py
--rw-rw-rw-   0        0        0     4683 2024-03-22 16:37:41.000000 ffxivcalc-0.8.930/src/ffxivcalc/Request/custom_columns.py
--rw-rw-rw-   0        0        0     2270 2024-01-02 21:14:00.000000 ffxivcalc-0.8.930/src/ffxivcalc/Request/etro_request.py
--rw-rw-rw-   0        0        0    13370 2024-03-22 20:15:47.000000 ffxivcalc-0.8.930/src/ffxivcalc/Request/ffxivcalcViewTranslator.py
--rw-rw-rw-   0        0        0     6564 2024-03-22 16:37:41.000000 ffxivcalc-0.8.930/src/ffxivcalc/Request/prepull.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.439884 ffxivcalc-0.8.930/src/ffxivcalc/SimulationRecord/
--rw-rw-rw-   0        0        0        0 2023-10-31 05:24:04.000000 ffxivcalc-0.8.930/src/ffxivcalc/SimulationRecord/__init__.py
--rw-rw-rw-   0        0        0    11647 2024-02-22 03:34:11.000000 ffxivcalc-0.8.930/src/ffxivcalc/SimulationRecord/record.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.479893 ffxivcalc-0.8.930/src/ffxivcalc/Tester/
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/Tester/__init__.py
--rw-rw-rw-   0        0        0   929485 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/Tester/testImplementation.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.498897 ffxivcalc-0.8.930/src/ffxivcalc/UI/
--rw-rw-rw-   0        0        0    16152 2023-09-07 03:45:36.000000 ffxivcalc-0.8.930/src/ffxivcalc/UI/SimulationInput.py
--rw-rw-rw-   0        0        0    10335 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/UI/TUI.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/UI/__init__.py
--rw-rw-rw-   0        0        0     3135 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/__init__.py
--rw-rw-rw-   0        0        0     3896 2023-12-04 19:09:48.000000 ffxivcalc-0.8.930/src/ffxivcalc/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.514901 ffxivcalc-0.8.930/src/ffxivcalc/codeParser/
--rw-rw-rw-   0        0        0      175 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/codeParser/__init__.py
--rw-rw-rw-   0        0        0     4176 2023-10-26 17:01:45.000000 ffxivcalc-0.8.930/src/ffxivcalc/codeParser/parser.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.570913 ffxivcalc-0.8.930/src/ffxivcalc/helperCode/
--rw-rw-rw-   0        0        0     3953 2024-01-08 21:47:27.000000 ffxivcalc-0.8.930/src/ffxivcalc/helperCode/Progress.py
--rw-rw-rw-   0        0        0    10212 2024-02-22 03:34:11.000000 ffxivcalc-0.8.930/src/ffxivcalc/helperCode/Vocal.py
--rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/helperCode/__init__.py
--rw-rw-rw-   0        0        0     8323 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/helperCode/exceptions.py
--rw-rw-rw-   0        0        0    30462 2024-03-30 20:55:22.000000 ffxivcalc-0.8.930/src/ffxivcalc/helperCode/helper_backend.py
--rw-rw-rw-   0        0        0      337 2024-01-05 18:36:28.000000 ffxivcalc-0.8.930/src/ffxivcalc/helperCode/helper_math.py
--rw-rw-rw-   0        0        0     7095 2024-03-22 16:37:41.000000 ffxivcalc-0.8.930/src/ffxivcalc/helperCode/lookUpAbilityID.py
--rw-rw-rw-   0        0        0      985 2023-08-08 18:10:05.000000 ffxivcalc-0.8.930/src/ffxivcalc/helperCode/requirementHandler.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:59:15.572913 ffxivcalc-0.8.930/src/ffxivcalc.egg-info/
--rw-rw-rw-   0        0        0     8696 2024-03-30 20:59:14.000000 ffxivcalc-0.8.930/src/ffxivcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3937 2024-03-30 20:59:14.000000 ffxivcalc-0.8.930/src/ffxivcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 20:59:14.000000 ffxivcalc-0.8.930/src/ffxivcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2024-03-30 20:59:14.000000 ffxivcalc-0.8.930/src/ffxivcalc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-30 20:59:14.000000 ffxivcalc-0.8.930/src/ffxivcalc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.874079 ffxivcalc-0.8.940/
+-rw-rw-rw-   0        0        0     1096 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/License.md
+-rw-rw-rw-   0        0        0     6924 2024-04-11 01:07:15.873079 ffxivcalc-0.8.940/PKG-INFO
+-rw-rw-rw-   0        0        0     5737 2024-04-11 01:05:54.000000 ffxivcalc-0.8.940/README.md
+-rw-rw-rw-   0        0        0       99 2023-12-05 18:34:38.000000 ffxivcalc-0.8.940/pyproject.toml
+-rw-rw-rw-   0        0        0       84 2024-04-11 01:07:15.876080 ffxivcalc-0.8.940/setup.cfg
+-rw-rw-rw-   0        0        0     1904 2024-04-11 01:05:06.000000 ffxivcalc-0.8.940/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.286947 ffxivcalc-0.8.940/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.342959 ffxivcalc-0.8.940/src/ffxivcalc/
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.390970 ffxivcalc-0.8.940/src/ffxivcalc/API/
+-rw-rw-rw-   0        0        0     1291 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/API/API.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.401973 ffxivcalc-0.8.940/src/ffxivcalc/API/Model/
+-rw-rw-rw-   0        0        0     1331 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/API/Model/ObjectInModel.py
+-rw-rw-rw-   0        0        0     1166 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/API/Model/ObjectOutModel.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/API/Model/__init__.py
+-rw-rw-rw-   0        0        0      245 2024-03-30 20:55:22.000000 ffxivcalc-0.8.940/src/ffxivcalc/API/__init__.py
+-rw-rw-rw-   0        0        0    11300 2023-08-12 03:23:31.000000 ffxivcalc-0.8.940/src/ffxivcalc/API/library.py
+-rw-rw-rw-   0        0        0     8898 2024-03-05 03:10:39.000000 ffxivcalc-0.8.940/src/ffxivcalc/Enemy.py
+-rw-rw-rw-   0        0        0    61879 2024-03-30 20:55:22.000000 ffxivcalc-0.8.940/src/ffxivcalc/Fight.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.421977 ffxivcalc-0.8.940/src/ffxivcalc/GearSolver/
+-rw-rw-rw-   0        0        0    25433 2024-01-08 22:21:22.000000 ffxivcalc-0.8.940/src/ffxivcalc/GearSolver/Gear.py
+-rw-rw-rw-   0        0        0    60331 2024-03-30 20:55:22.000000 ffxivcalc-0.8.940/src/ffxivcalc/GearSolver/Solver.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/GearSolver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.452984 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/
+-rw-rw-rw-   0        0        0    18461 2024-03-20 21:34:42.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/ActionEnum.py
+-rw-rw-rw-   0        0        0    41438 2024-03-30 20:55:22.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Base_Spell.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.462986 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.471989 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Blackmage/
+-rw-rw-rw-   0        0        0    16913 2024-03-05 23:41:51.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Blackmage/BlackMage_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Blackmage/__init__.py
+-rw-rw-rw-   0        0        0     5683 2024-03-20 18:07:50.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Caster_Spell.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.481991 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Redmage/
+-rw-rw-rw-   0        0        0    14685 2023-11-22 02:47:02.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Redmage/Redmage_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Redmage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.492994 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Summoner/
+-rw-rw-rw-   0        0        0    11920 2024-03-16 17:05:29.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Summoner/Summoner_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Summoner/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.500995 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.510997 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Astrologian/
+-rw-rw-rw-   0        0        0    16171 2024-03-30 20:55:22.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Astrologian/Astrologian_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Astrologian/__init__.py
+-rw-rw-rw-   0        0        0     3452 2024-03-30 20:55:22.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Healer_Spell.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.520999 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Sage/
+-rw-rw-rw-   0        0        0     8218 2024-03-30 20:55:22.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Sage/Sage_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Sage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.530001 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Scholar/
+-rw-rw-rw-   0        0        0    10628 2024-03-30 20:55:22.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Scholar/Scholar_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Scholar/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.533002 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Whitemage/
+-rw-rw-rw-   0        0        0     7110 2024-03-30 20:55:22.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Whitemage/Whitemage_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Whitemage/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.542004 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.552006 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Dragoon/
+-rw-rw-rw-   0        0        0    14354 2023-11-30 18:40:07.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Dragoon/Dragoon_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Dragoon/__init__.py
+-rw-rw-rw-   0        0        0     5502 2024-03-20 18:07:12.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Melee_Spell.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.562008 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Monk/
+-rw-rw-rw-   0        0        0    17329 2023-11-25 23:09:24.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Monk/Monk_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Monk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.572011 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Ninja/
+-rw-rw-rw-   0        0        0    21455 2024-02-10 19:14:06.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Ninja/Ninja_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Ninja/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.581013 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Reaper/
+-rw-rw-rw-   0        0        0    16669 2023-11-22 02:47:02.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Reaper/Reaper_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Reaper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.591015 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Samurai/
+-rw-rw-rw-   0        0        0    17033 2024-02-07 02:58:18.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Samurai/Samurai_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Samurai/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/__init__.py
+-rw-rw-rw-   0        0        0   147878 2024-04-11 00:14:25.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Player.py
+-rw-rw-rw-   0        0        0     1299 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/PlayerEnum.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.594016 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.605018 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Bard/
+-rw-rw-rw-   0        0        0    23577 2024-04-11 01:04:13.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Bard/Bard_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Bard/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.615021 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Dancer/
+-rw-rw-rw-   0        0        0    17215 2024-03-20 21:35:16.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Dancer/Dancer_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Dancer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.625023 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Machinist/
+-rw-rw-rw-   0        0        0    15778 2024-03-20 19:51:31.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Machinist/Machinist_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Machinist/__init__.py
+-rw-rw-rw-   0        0        0     3367 2024-03-20 18:09:32.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Ranged_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.636025 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.646027 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/DarkKnight/
+-rw-rw-rw-   0        0        0    14726 2024-02-10 19:14:06.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/DarkKnight/DarkKnight_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/DarkKnight/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.657030 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Gunbreaker/
+-rw-rw-rw-   0        0        0    10822 2024-02-08 00:30:27.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Gunbreaker/Gunbreaker_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Gunbreaker/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.667032 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Paladin/
+-rw-rw-rw-   0        0        0    15029 2024-02-08 23:33:24.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Paladin/Paladin_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Paladin/__init__.py
+-rw-rw-rw-   0        0        0     7494 2024-03-20 16:27:29.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Tank_Spell.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.677034 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Warrior/
+-rw-rw-rw-   0        0        0    11972 2024-02-08 01:51:53.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Warrior/Warrior_Spell.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Warrior/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Jobs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.729046 ffxivcalc-0.8.940/src/ffxivcalc/Request/
+-rw-rw-rw-   0        0        0    31419 2024-03-22 16:37:41.000000 ffxivcalc-0.8.940/src/ffxivcalc/Request/FFLogsAPIRequest.py
+-rw-rw-rw-   0        0        0    25158 2024-03-22 20:15:47.000000 ffxivcalc-0.8.940/src/ffxivcalc/Request/FFLogs_api.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Request/__init__.py
+-rw-rw-rw-   0        0        0     4683 2024-03-22 16:37:41.000000 ffxivcalc-0.8.940/src/ffxivcalc/Request/custom_columns.py
+-rw-rw-rw-   0        0        0     2270 2024-01-02 21:14:00.000000 ffxivcalc-0.8.940/src/ffxivcalc/Request/etro_request.py
+-rw-rw-rw-   0        0        0    13370 2024-03-22 20:15:47.000000 ffxivcalc-0.8.940/src/ffxivcalc/Request/ffxivcalcViewTranslator.py
+-rw-rw-rw-   0        0        0     6564 2024-03-22 16:37:41.000000 ffxivcalc-0.8.940/src/ffxivcalc/Request/prepull.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.739048 ffxivcalc-0.8.940/src/ffxivcalc/SimulationRecord/
+-rw-rw-rw-   0        0        0        0 2023-10-31 05:24:04.000000 ffxivcalc-0.8.940/src/ffxivcalc/SimulationRecord/__init__.py
+-rw-rw-rw-   0        0        0    11647 2024-02-22 03:34:11.000000 ffxivcalc-0.8.940/src/ffxivcalc/SimulationRecord/record.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.777057 ffxivcalc-0.8.940/src/ffxivcalc/Tester/
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/Tester/__init__.py
+-rw-rw-rw-   0        0        0   937596 2024-04-11 01:04:13.000000 ffxivcalc-0.8.940/src/ffxivcalc/Tester/testImplementation.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.796061 ffxivcalc-0.8.940/src/ffxivcalc/UI/
+-rw-rw-rw-   0        0        0    16152 2023-09-07 03:45:36.000000 ffxivcalc-0.8.940/src/ffxivcalc/UI/SimulationInput.py
+-rw-rw-rw-   0        0        0    10335 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/UI/TUI.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/UI/__init__.py
+-rw-rw-rw-   0        0        0     3265 2024-04-11 01:04:13.000000 ffxivcalc-0.8.940/src/ffxivcalc/__init__.py
+-rw-rw-rw-   0        0        0     3896 2023-12-04 19:09:48.000000 ffxivcalc-0.8.940/src/ffxivcalc/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.805064 ffxivcalc-0.8.940/src/ffxivcalc/codeParser/
+-rw-rw-rw-   0        0        0      175 2024-03-30 20:55:22.000000 ffxivcalc-0.8.940/src/ffxivcalc/codeParser/__init__.py
+-rw-rw-rw-   0        0        0     4176 2023-10-26 17:01:45.000000 ffxivcalc-0.8.940/src/ffxivcalc/codeParser/parser.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.870078 ffxivcalc-0.8.940/src/ffxivcalc/helperCode/
+-rw-rw-rw-   0        0        0     3953 2024-01-08 21:47:27.000000 ffxivcalc-0.8.940/src/ffxivcalc/helperCode/Progress.py
+-rw-rw-rw-   0        0        0    10212 2024-02-22 03:34:11.000000 ffxivcalc-0.8.940/src/ffxivcalc/helperCode/Vocal.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/helperCode/__init__.py
+-rw-rw-rw-   0        0        0     8323 2024-03-30 20:55:22.000000 ffxivcalc-0.8.940/src/ffxivcalc/helperCode/exceptions.py
+-rw-rw-rw-   0        0        0    30462 2024-03-30 20:55:22.000000 ffxivcalc-0.8.940/src/ffxivcalc/helperCode/helper_backend.py
+-rw-rw-rw-   0        0        0      337 2024-01-05 18:36:28.000000 ffxivcalc-0.8.940/src/ffxivcalc/helperCode/helper_math.py
+-rw-rw-rw-   0        0        0     7095 2024-03-22 16:37:41.000000 ffxivcalc-0.8.940/src/ffxivcalc/helperCode/lookUpAbilityID.py
+-rw-rw-rw-   0        0        0      985 2023-08-08 18:10:05.000000 ffxivcalc-0.8.940/src/ffxivcalc/helperCode/requirementHandler.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:07:15.872078 ffxivcalc-0.8.940/src/ffxivcalc.egg-info/
+-rw-rw-rw-   0        0        0     6924 2024-04-11 01:07:15.000000 ffxivcalc-0.8.940/src/ffxivcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3937 2024-04-11 01:07:15.000000 ffxivcalc-0.8.940/src/ffxivcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 01:07:15.000000 ffxivcalc-0.8.940/src/ffxivcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2024-04-11 01:07:15.000000 ffxivcalc-0.8.940/src/ffxivcalc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 01:07:15.000000 ffxivcalc-0.8.940/src/ffxivcalc.egg-info/top_level.txt
```

### Comparing `ffxivcalc-0.8.930/License.md` & `ffxivcalc-0.8.940/License.md`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/PKG-INFO` & `ffxivcalc-0.8.940/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffxivcalc
-Version: 0.8.930
+Version: 0.8.940
 Summary: DPS simulator for Final Fantasy XIV.
 Home-page: https://github.com/IAmPythagoras/FFXIV-Combat-Simulator
 Author: Anthony Desrochers
 Author-email: anthony.desrochers17@gmail.com
 Project-URL: Source, https://github.com/IAmPythagoras/FFXIV-Combat-Simulator
 Project-URL: Site, https://ffxivdpscalc.azurewebsites.net/simulate/
 Project-URL: Documentation, https://iampythagoras.github.io/index.html
@@ -29,46 +29,40 @@
 Requires-Dist: six
 Requires-Dist: coreapi
 Requires-Dist: pandas
 Requires-Dist: python_graphql_client
 
 [![Discord](https://img.shields.io/discord/970724799464738977?color=7289da&label=Discord&logo=discord)](https://discord.gg/mZXKUNy2sw)
 
-# Website
+# Desktop app
 
-The website https://ffxivdpscalc.azurewebsites.net allows an easier time for people without coding knowledge to use the simulator.
-It uses the most up to date version of FFIXV-Combat-Simulator, but has some limitations to keep computation time low.
+You can download the desktop app to use the simulator without having to code : https://github.com/IAmPythagoras/ffxivcalcWebApp .
 
 # Install
 
 You can install this library using pip : 
 
 ```
 pip install ffxivcalc
 ```
 
-or using git (this would let you download from the dev branch "feature/GeneralDev"): 
+Or can download latest unstable version using : 
 
 ```
-pip install ffxiv-combat-simulator@git+https://github.com/IAmPythagoras/FFXIV-Combat-Simulator.git@main
+pip install ffxiv-combat-simulator@git+https://github.com/IAmPythagoras/FFXIV-Combat-Simulator.git@feature/GeneralDev
 ```
 
 *Note that you must have git installed : https://git-scm.com/download/win 
 
 You can find the documentation here : https://iampythagoras.github.io/index.html or join the discord linked above if you have any questions.
 
-If you want to locally use the API. Install the ffxiv-combat-simulator library and also install uvicorn :
+*The unstable version can be removed using
 ```
-pip install uvicorn
+pip uninstall ffxiv-combat-simulator
 ```
-And then run this command:
-```
-python -m uvicorn ffxivcalc.API.API:app
-```
-This will locally launch the API.
 
 # FFXIV-Combat-Simulator (ffxivcalc)
 
 This Python library lets you simulate combat from the game Final Fantasy XIV. It allows for as many players as possible and will simulate the fight in "real time". It
 accurately keeps track of MP, cooldown on abilities, HP, DOTs, raid buffs, personnal buffs, team composition bonus, potions buff, which allows for a dynamic environment that portrays as accurately as possible the real game's environment.
 
 The simulator in its base state will output every player's DPS (Damage Per Second), PPS (Potency Per Second), TP (Total Potency), but it can be customized to output any other metric that could be useful. Furthermore, the simulator is able to output a distribution of the DPS which allows to see the different DPS' percentiles.
@@ -99,51 +93,41 @@
 
 ![image](https://github.com/IAmPythagoras/FFXIV-Combat-Simulator/assets/62820030/88069e5d-8ffa-4783-acc3-b1b02c3ce33e)
 
 This record's goal is to act as a sort of log, but which is more easily understood and contains only the most useful information on the running of the simulation.
 You can also export a text only version of this record.
 # Rotation BiS Solver 
 
-As of ffxivcalc version 0.8.00, this library now has a built in rotation BiS solver. You can use the ffxivcalclayout.py in order to experiment with it.
+As of ffxivcalc version 0.8.00, this library now has a built in rotation BiS solver. You can use the ffxivcalclayout.py in order to experiment with it or download the desktop app.
 
 You can read this PDF [BiS_Solver_Algorithm_Documentation.pdf](https://github.com/IAmPythagoras/FFXIV-Combat-Simulator/files/12580553/BiS_Solver_Algorithm_Documentation.pdf) if you are interested in its
 functionning. 
 
 You can read about the experimental results of this solver here : https://docs.google.com/spreadsheets/d/1yVl-F1tHARYIYvz4ZPxIY6MayakYug3OEqpGnpZllqU/edit?usp=sharing
 
 # Validity of simulator
 
-As of version 0.8.30 I have started adding in depth testing of the simulator. The simulator will still have some flaws, but it is currently being checked by around 430 individual tests. More tests
-will be added with time.
-
-# Discord bot): 
-DISCORD BOT IS CURRENTLY OFFLINE. WILL UPDATE HERE WHEN IT IS AVAILABLE
-I made a disbord bot that uses the python library ffxivcalc in order to simulate fights. Feel free to install it using the link below. As of now, the main bot commands are :
-```
-!Simulate (With a JSON file as a file in the same message)
-!Template <filename> <job1> <job2> ... (Generates a template JSON file used to simulate)
-!Help (for help)
-```
-Use this link to install the bot on your server : 
-```
-https://discord.com/oauth2/authorize?client_id=1071922835011932290&permissions=274878024704&scope=bot
-```
-
-# Currently Working On
-
-Adding code to support multiple enemies at the same time and individual targetting of enemy by the players.
+As of version 0.8.940 I have started adding in depth testing of the simulator. The simulator will still have some flaws, but it is currently being checked by around 800 individual tests. More tests will be added with time.
 
+# Other simulators
 
-# HOW IT WORKS
+Make sure to check out this alternative FFXIV simulator [Amas-FF14-Combat-Sim](https://github.com/Amarantine-xiv/Amas-FF14-Combat-Sim) or join its [Discord](https://discord.gg/8GjA5uRcDX)
 
-The big advantage of this program is that instead of computing the average PPS (potency per second) and then using a damage formula to find the
-DPS (Damage per second), it simulates the fight like it would happen in real time. That way, buffs are accurately taken into account. It is also able to discernate between oGCD and GCD, and will treat them accordingly (for weaving and stuff).The program can also see if a rotation is illegal, and will stop if it is determined to be a rotation that cannot be done in the game.
-
-The time-unit used for the program is by default 0.01s/step, but it can be put at whatever smaller (or bigger) number we prefer. It is also able to know when a certain ability cannot be casted, and using that ability anyway will result in an error that stops the simulation. We could in theory disable this checking if we wanted.
+# If you want to help
 
-Each job in the game is implemented in a relatively similar way. We first create a class JobSpell, which will be an object that will represent a spell/ability/weaponskill of the job. Such an object will have information like casting time, recast time (if GCD), potency, manacost, effect of applying that spell and the requirements of that spell. We then also need to create a class JobPlayer, which will inherit certain traits for its parent class (Healer, Caster, Melee, Ranged or Tank) (This is also the case for spell). This JobPlayer class will contain information like Ability Cooldown, Buff Timer, DOTTimer and other stuff that need to be tracked during the execution of the simulation.
+If you want to help or want to ask questions to me directly, feel free to join the discord linked above:)
 
-And that's about it, the code will take these two new classes (and object of the JobSpell class) and if everything is done correctly the simulator will be able to run without any issues.
+# Update log
 
-# If you want to help
+(Recent only read __init__.py for all update logs)
 
-If you want to help or want to ask questions to me directly, feel free to join the discord linked above:)
+0.9.940:
+    - Oups, forgot to ever implement Army Ethos/Army Muse effect on Bard. This is now fixed.
+    - Other bug fixes.
+
+0.8.930:
+    - Added Player.getPlayerPrePullTime() which returns the length of the prepull (time before first damage action).
+    - Added Fight.getPlayerPrepullLength() which returns the prepull length of all players
+    - added Fight.syncPlayerPrePull() which syncs all player's prepull so they all do damage at the same time.
+    - Added test suite 'Prepull length test suite' that tests the Player.GetPlayerPrePullTime() function.
+    - Removed access to ffxvivcalc.API, ffxivcalc.codeParser and ffxivcalc.Request.FFLogsAPIRequest modules (outdated modules).
+    - Other minor bug fix.
```

### Comparing `ffxivcalc-0.8.930/README.md` & `ffxivcalc-0.8.940/src/ffxivcalc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,68 @@
+Metadata-Version: 2.1
+Name: ffxivcalc
+Version: 0.8.940
+Summary: DPS simulator for Final Fantasy XIV.
+Home-page: https://github.com/IAmPythagoras/FFXIV-Combat-Simulator
+Author: Anthony Desrochers
+Author-email: anthony.desrochers17@gmail.com
+Project-URL: Source, https://github.com/IAmPythagoras/FFXIV-Combat-Simulator
+Project-URL: Site, https://ffxivdpscalc.azurewebsites.net/simulate/
+Project-URL: Documentation, https://iampythagoras.github.io/index.html
+Keywords: ffxiv,xiv,dps,simulator,ffxiv-combat-simulator
+Classifier: Development Status :: 4 - Beta
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: License.md
+Requires-Dist: contourpy
+Requires-Dist: cycler
+Requires-Dist: fonttools
+Requires-Dist: kiwisolver
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: packaging
+Requires-Dist: Pillow
+Requires-Dist: pyparsing
+Requires-Dist: python-dateutil
+Requires-Dist: six
+Requires-Dist: coreapi
+Requires-Dist: pandas
+Requires-Dist: python_graphql_client
+
 [![Discord](https://img.shields.io/discord/970724799464738977?color=7289da&label=Discord&logo=discord)](https://discord.gg/mZXKUNy2sw)
 
-# Website
+# Desktop app
 
-The website https://ffxivdpscalc.azurewebsites.net allows an easier time for people without coding knowledge to use the simulator.
-It uses the most up to date version of FFIXV-Combat-Simulator, but has some limitations to keep computation time low.
+You can download the desktop app to use the simulator without having to code : https://github.com/IAmPythagoras/ffxivcalcWebApp .
 
 # Install
 
 You can install this library using pip : 
 
 ```
 pip install ffxivcalc
 ```
 
-or using git (this would let you download from the dev branch "feature/GeneralDev"): 
+Or can download latest unstable version using : 
 
 ```
-pip install ffxiv-combat-simulator@git+https://github.com/IAmPythagoras/FFXIV-Combat-Simulator.git@main
+pip install ffxiv-combat-simulator@git+https://github.com/IAmPythagoras/FFXIV-Combat-Simulator.git@feature/GeneralDev
 ```
 
 *Note that you must have git installed : https://git-scm.com/download/win 
 
 You can find the documentation here : https://iampythagoras.github.io/index.html or join the discord linked above if you have any questions.
 
-If you want to locally use the API. Install the ffxiv-combat-simulator library and also install uvicorn :
-```
-pip install uvicorn
+*The unstable version can be removed using
 ```
-And then run this command:
+pip uninstall ffxiv-combat-simulator
 ```
-python -m uvicorn ffxivcalc.API.API:app
-```
-This will locally launch the API.
 
 # FFXIV-Combat-Simulator (ffxivcalc)
 
 This Python library lets you simulate combat from the game Final Fantasy XIV. It allows for as many players as possible and will simulate the fight in "real time". It
 accurately keeps track of MP, cooldown on abilities, HP, DOTs, raid buffs, personnal buffs, team composition bonus, potions buff, which allows for a dynamic environment that portrays as accurately as possible the real game's environment.
 
 The simulator in its base state will output every player's DPS (Damage Per Second), PPS (Potency Per Second), TP (Total Potency), but it can be customized to output any other metric that could be useful. Furthermore, the simulator is able to output a distribution of the DPS which allows to see the different DPS' percentiles.
@@ -66,51 +93,41 @@
 
 ![image](https://github.com/IAmPythagoras/FFXIV-Combat-Simulator/assets/62820030/88069e5d-8ffa-4783-acc3-b1b02c3ce33e)
 
 This record's goal is to act as a sort of log, but which is more easily understood and contains only the most useful information on the running of the simulation.
 You can also export a text only version of this record.
 # Rotation BiS Solver 
 
-As of ffxivcalc version 0.8.00, this library now has a built in rotation BiS solver. You can use the ffxivcalclayout.py in order to experiment with it.
+As of ffxivcalc version 0.8.00, this library now has a built in rotation BiS solver. You can use the ffxivcalclayout.py in order to experiment with it or download the desktop app.
 
 You can read this PDF [BiS_Solver_Algorithm_Documentation.pdf](https://github.com/IAmPythagoras/FFXIV-Combat-Simulator/files/12580553/BiS_Solver_Algorithm_Documentation.pdf) if you are interested in its
 functionning. 
 
 You can read about the experimental results of this solver here : https://docs.google.com/spreadsheets/d/1yVl-F1tHARYIYvz4ZPxIY6MayakYug3OEqpGnpZllqU/edit?usp=sharing
 
 # Validity of simulator
 
-As of version 0.8.30 I have started adding in depth testing of the simulator. The simulator will still have some flaws, but it is currently being checked by around 430 individual tests. More tests
-will be added with time.
-
-# Discord bot): 
-DISCORD BOT IS CURRENTLY OFFLINE. WILL UPDATE HERE WHEN IT IS AVAILABLE
-I made a disbord bot that uses the python library ffxivcalc in order to simulate fights. Feel free to install it using the link below. As of now, the main bot commands are :
-```
-!Simulate (With a JSON file as a file in the same message)
-!Template <filename> <job1> <job2> ... (Generates a template JSON file used to simulate)
-!Help (for help)
-```
-Use this link to install the bot on your server : 
-```
-https://discord.com/oauth2/authorize?client_id=1071922835011932290&permissions=274878024704&scope=bot
-```
+As of version 0.8.940 I have started adding in depth testing of the simulator. The simulator will still have some flaws, but it is currently being checked by around 800 individual tests. More tests will be added with time.
 
-# Currently Working On
+# Other simulators
 
-Adding code to support multiple enemies at the same time and individual targetting of enemy by the players.
+Make sure to check out this alternative FFXIV simulator [Amas-FF14-Combat-Sim](https://github.com/Amarantine-xiv/Amas-FF14-Combat-Sim) or join its [Discord](https://discord.gg/8GjA5uRcDX)
 
+# If you want to help
 
-# HOW IT WORKS
-
-The big advantage of this program is that instead of computing the average PPS (potency per second) and then using a damage formula to find the
-DPS (Damage per second), it simulates the fight like it would happen in real time. That way, buffs are accurately taken into account. It is also able to discernate between oGCD and GCD, and will treat them accordingly (for weaving and stuff).The program can also see if a rotation is illegal, and will stop if it is determined to be a rotation that cannot be done in the game.
-
-The time-unit used for the program is by default 0.01s/step, but it can be put at whatever smaller (or bigger) number we prefer. It is also able to know when a certain ability cannot be casted, and using that ability anyway will result in an error that stops the simulation. We could in theory disable this checking if we wanted.
-
-Each job in the game is implemented in a relatively similar way. We first create a class JobSpell, which will be an object that will represent a spell/ability/weaponskill of the job. Such an object will have information like casting time, recast time (if GCD), potency, manacost, effect of applying that spell and the requirements of that spell. We then also need to create a class JobPlayer, which will inherit certain traits for its parent class (Healer, Caster, Melee, Ranged or Tank) (This is also the case for spell). This JobPlayer class will contain information like Ability Cooldown, Buff Timer, DOTTimer and other stuff that need to be tracked during the execution of the simulation.
+If you want to help or want to ask questions to me directly, feel free to join the discord linked above:)
 
-And that's about it, the code will take these two new classes (and object of the JobSpell class) and if everything is done correctly the simulator will be able to run without any issues.
+# Update log
 
-# If you want to help
+(Recent only read __init__.py for all update logs)
 
-If you want to help or want to ask questions to me directly, feel free to join the discord linked above:)
+0.9.940:
+    - Oups, forgot to ever implement Army Ethos/Army Muse effect on Bard. This is now fixed.
+    - Other bug fixes.
+
+0.8.930:
+    - Added Player.getPlayerPrePullTime() which returns the length of the prepull (time before first damage action).
+    - Added Fight.getPlayerPrepullLength() which returns the prepull length of all players
+    - added Fight.syncPlayerPrePull() which syncs all player's prepull so they all do damage at the same time.
+    - Added test suite 'Prepull length test suite' that tests the Player.GetPlayerPrePullTime() function.
+    - Removed access to ffxvivcalc.API, ffxivcalc.codeParser and ffxivcalc.Request.FFLogsAPIRequest modules (outdated modules).
+    - Other minor bug fix.
```

### Comparing `ffxivcalc-0.8.930/setup.py` & `ffxivcalc-0.8.940/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ffxivcalc",  # Required
-    version="0.8.930",  # Required
+    version="0.8.940",  # Required
     description="DPS simulator for Final Fantasy XIV.",
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/IAmPythagoras/FFXIV-Combat-Simulator",  # Optiona
     author="Anthony Desrochers",
     author_email="anthony.desrochers17@gmail.com",
     classifiers=[  # Optional
```

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/API/API.py` & `ffxivcalc-0.8.940/src/ffxivcalc/API/API.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/API/Model/ObjectInModel.py` & `ffxivcalc-0.8.940/src/ffxivcalc/API/Model/ObjectInModel.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/API/Model/ObjectOutModel.py` & `ffxivcalc-0.8.940/src/ffxivcalc/API/Model/ObjectOutModel.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/API/library.py` & `ffxivcalc-0.8.940/src/ffxivcalc/API/library.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Enemy.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Enemy.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Fight.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Fight.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/GearSolver/Gear.py` & `ffxivcalc-0.8.940/src/ffxivcalc/GearSolver/Gear.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/GearSolver/Solver.py` & `ffxivcalc-0.8.940/src/ffxivcalc/GearSolver/Solver.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/ActionEnum.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/ActionEnum.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Base_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Base_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Blackmage/BlackMage_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Blackmage/BlackMage_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Caster_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Caster_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Redmage/Redmage_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Redmage/Redmage_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Caster/Summoner/Summoner_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Caster/Summoner/Summoner_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Astrologian/Astrologian_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Astrologian/Astrologian_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Healer_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Healer_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Sage/Sage_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Sage/Sage_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Scholar/Scholar_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Scholar/Scholar_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Healer/Whitemage/Whitemage_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Healer/Whitemage/Whitemage_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Dragoon/Dragoon_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Dragoon/Dragoon_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Melee_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Melee_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Monk/Monk_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Monk/Monk_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Ninja/Ninja_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Ninja/Ninja_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Reaper/Reaper_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Reaper/Reaper_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Melee/Samurai/Samurai_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Melee/Samurai/Samurai_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Player.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Player.py`

 * *Files 0% similar despite different names*

```diff
@@ -2224,15 +2224,18 @@
         self.UsedRepertoire = 0 #Only relevant for Wanderer and pitch perfect
         self.UsedSoulVoiceGauge = 0
         self.UsedBloodLetterReduction = 0
         self.UsedRepertoireAdd = 0 #This is repertoire stacks we used more than the expected value
         self.UsedTotalWandererRepertoire = 0
         self.UsedShadowbite = 0
 
-
+        # Haste Gained
+        self.hasteGainedFromArmyMuse = 0
+        self.hasteGainedFromArmyPaeon = 0
+        
         #Gauge
         self.SoulVoiceGauge = 0
         self.Repertoire = 0
         self.MaximumRepertoire = 0 #Used for wanderer
         self.MaximumBloodLetterReduction = 0
 
         #Stack
@@ -2273,14 +2276,16 @@
         #Timer
         self.SongTimer = 0
         self.StormbiteDOTTimer = 0
         self.CausticbiteDOTTimer = 0
         self.BattleVoiceTimer = 0
         self.RagingStrikeTimer = 0
         self.RadiantFinaleTimer = 0
+        self.ArmyEthosTimer = 0
+        self.ArmyMuseTimer = 0
 
         #DOT
         self.StormbiteDOT = None
         self.CausticbiteDOT = None
 
 
         #DPSBonus
@@ -2308,14 +2313,18 @@
             
             if (self.SongTimer > 0) : self.SongTimer = max(0,self.SongTimer - time)
             if (self.StormbiteDOTTimer > 0) : self.StormbiteDOTTimer = max(0,self.StormbiteDOTTimer - time)
             if (self.CausticbiteDOTTimer > 0) : self.CausticbiteDOTTimer = max(0,self.CausticbiteDOTTimer - time)
             if (self.BattleVoiceTimer > 0) : self.BattleVoiceTimer = max(0,self.BattleVoiceTimer - time)
             if (self.RagingStrikeTimer > 0) : self.RagingStrikeTimer = max(0,self.RagingStrikeTimer - time)
             if (self.RadiantFinaleTimer > 0) : self.RadiantFinaleTimer = max(0,self.RadiantFinaleTimer - time)
+            if (self.ArmyEthosTimer > 0) : self.ArmyEthosTimer = max(0,self.ArmyEthosTimer - time)
+            if (self.ArmyMuseTimer > 0) : self.ArmyMuseTimer = max(0,self.ArmyMuseTimer - time)
+
+            
 
         # update functions
         self.updateJobTimer = updateTimer
         self.updateJobCD = updateCD
 
     def init_monk(self):
```

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/PlayerEnum.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/PlayerEnum.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Bard/Bard_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Bard/Bard_Spell.py`

 * *Files 6% similar despite different names*

```diff
@@ -214,32 +214,76 @@
 
 def ApplyBloodLetter(Player, Enemy):
     if Player.BloodLetterStack == 3:
         Player.EffectCDList.append(BloodLetterStackCheck)
         Player.BloodLetterCD = 15
     Player.BloodLetterStack -= 1
 
+def armyMuseCheck(Player, Enemy):
+    if Player.ArmyMuseTimer <= 0:
+        Player.hasteChangeValue = -Player.hasteGainedFromArmyMuse
+        Player.Haste -= Player.hasteGainedFromArmyMuse 
+        Player.hasteHasChanged = True
+        Player.EffectToRemove.append(armyMuseCheck)
+
+def _apply_army_muse(Player, Enemy):
+
+    Player.ArmyMuseTimer = 10
+
+    hasteBuff : int = 0
+    repValue : int = int(Player.Repertoire)
+    assert repValue >= 0 and repValue <= 4, "Player Repertoire value is lower than 0 or higher than 4"
+
+    match repValue:
+        case 0: hasteBuff = 0
+        case 1 : hasteBuff = 1
+        case 2 : hasteBuff = 2
+        case 3 : hasteBuff = 4
+        case 4 : hasteBuff = 12
+
+    Player.hasteGainedFromArmyMuse = hasteBuff    
+    Player.hasteChangeValue += hasteBuff
+    Player.Haste = hasteBuff
+    Player.hasteHasChanged = int(Player.hasteChangeValue) != 0 # Should never happend (not zero) but just in case.
+
+    if _apply_army_muse in Player.EffectCDList : Player.EffectToRemove.append(_apply_army_muse)
+    Player.EffectCDList.append(armyMuseCheck)
+
+def checkArmyEthos(Player, Enemy):
+    if Player.ArmyEthosTimer <= 0:
+        Player.EffectToRemove.append(checkArmyEthos)
+        
+def _check_army_muse(Player):
+    if Player.ArmyPaeon:
+                             # Adding end of EffectCDList since ArmyPaeonCheck will remove its effect before it goes through this function.
+        Player.EffectCDList.append(_apply_army_muse)
+    elif checkArmyEthos in Player.EffectCDList:
+        _apply_army_muse(Player, None)
+
+        Player.ArmyEthosTimer = 0
+
+
 def ApplyWanderingMinuet(Player, Enemy):
     Player.WandererCoda = True #Adding Coda
     Player.WanderingMinuetCD = 120
     Player.SongTimer = 45
     Enemy.WanderingMinuet = True
     Player.EffectCDList.append(WandererCheck)
+    _check_army_muse(Player)
     #Removing Current song
     Player.MageBallad = False
     Player.ArmyPaeon = False
     Player.WanderingMinuet = True
 
-                                     # Only doing this if SavePreBakedAction is true
-    #if Player.CurrentFight.SavePreBakedAction:
-    #    fight = Player.CurrentFight
-    #    history = buffHistory(fight.TimeStamp, fight.TimeStamp + 45)
-    #    fight.PlayerList[fight.PlayerIDSavePreBakedAction].WanderingMinuetHistory.append(history)
-
 def ApplyArmyPaeon(Player, Enemy):
+    Player.Repertoire = 0 # Reseting ArmyPaeon repertoire count.
+    Player.ArmyEthosTimer = 0 
+    Player.hasteGainedFromArmyMuse = 0
+    if _check_army_muse in Player.EffectCDList: Player.EffectCDList.remove(_check_army_muse)
+
     Player.ArmyCoda = True #Adding Coda
     Enemy.ArmyPaeon = True # 3% DH
     Player.ArmyPaeonCD = 120
     Player.SongTimer = 45
     Player.EffectCDList.append(ArmyPaeonCheck)
     Player.EffectList.append(ArmyPaeonEffect)
     #Have to remove current song
@@ -249,14 +293,15 @@
 
 def ApplyMageBallad(Player, Enemy):
     Player.MageCoda = True #Adding Coda
     Enemy.buffList.append(MageBalladBuff)
     Player.SongTimer = 45
     Player.MageBalladCD = 120
     Player.EffectCDList.append(MageBalladCheck)
+    _check_army_muse(Player)
     #Have to remove current song
     Player.MageBallad = True
     Player.ArmyPaeon = False
     Player.WanderingMinuet = False
 
 def ApplyBarrage(Player, Enemy):
     Player.EffectList.append(BarrageEffect)
@@ -383,24 +428,29 @@
     #It will add 0.8 repertoire each proc since we have 80% chance for a max of 4 procs
 
     if Player.SongTimer != 45 and (int(Player.SongTimer*100)/100)%3 == 0 and not (Player.Repertoire == 4.0):
         Player.Repertoire += 0.8
         Player.hasteChangeValue = 3.2
         Player.Haste += 3.2
         Player.hasteHasChanged = True
+        Player.hasteGainedFromArmyPaeon += 3.2
 
     if Player.SongTimer <= 0 or not (Player.ArmyPaeon):
         Enemy.ArmyPaeon = False
         Player.ArmyPaeon = False
         Player.EffectToRemove.append(ArmyPaeonCheck)
         Player.EffectList.remove(ArmyPaeonEffect)
-        Player.Haste = 0 # Reseting Haste value since there is no other haste buff from Bard
-        Player.hasteChangeValue = -Player.Haste # Bard only has Haste from Army Paeon, so we simply look what value it was at when it ended.
+        if _apply_army_muse not in Player.EffectCDList : Player.EffectCDList.append(checkArmyEthos)
+        Player.ArmyEthosTimer = 30
+        Player.hasteChangeValue = -Player.hasteGainedFromArmyPaeon
+        Player.Haste -= Player.hasteGainedFromArmyPaeon 
         Player.hasteHasChanged = True
 
+                             # Giving 
+
 def MageBalladCheck(Player, Enemy):
 
     if Player.SongTimer != 45 and (int(Player.SongTimer*100)/100)%3 == 0: #The effect applies each 3 seconds, so we check each such interval 
         Player.ExpectedBloodLetterReduction += 7.5 * 0.8 #Adding expected reduction
         Player.MaximumBloodLetterReduction += 7.5
 
     if Player.SongTimer <= 0 or not (Player.MageBallad):
```

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Dancer/Dancer_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Dancer/Dancer_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Machinist/Machinist_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Machinist/Machinist_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Ranged/Ranged_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Ranged/Ranged_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/DarkKnight/DarkKnight_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/DarkKnight/DarkKnight_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Gunbreaker/Gunbreaker_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Gunbreaker/Gunbreaker_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Paladin/Paladin_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Paladin/Paladin_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Tank_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Tank_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Jobs/Tank/Warrior/Warrior_Spell.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Jobs/Tank/Warrior/Warrior_Spell.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Request/FFLogsAPIRequest.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Request/FFLogsAPIRequest.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Request/FFLogs_api.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Request/FFLogs_api.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Request/custom_columns.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Request/custom_columns.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Request/etro_request.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Request/etro_request.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Request/ffxivcalcViewTranslator.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Request/ffxivcalcViewTranslator.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Request/prepull.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Request/prepull.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/SimulationRecord/record.py` & `ffxivcalc-0.8.940/src/ffxivcalc/SimulationRecord/record.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/Tester/testImplementation.py` & `ffxivcalc-0.8.940/src/ffxivcalc/Tester/testImplementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -4891,15 +4891,15 @@
 
         Event.SimulateFight(0.01, 500, False, PPSGraph=False, showProgress=False,computeGraph=False)
 
         return [MageBalladBuff in Dummy.buffList, round(player.SongTimer,2), player.Haste, Dummy.WanderingMinuet, Dummy.ArmyPaeon]
 
     def brdTest15ValidationFunction(testResults) -> (bool, list):
         passed = True
-        expected = [False,44.99, 0, True,False]   
+        expected = [False,44.99, 1, True,False]   
 
         for i in range(len(testResults)): passed = passed and (expected[i] == testResults[i])
 
         return passed , expected
 
     brdtest15 = test("Song test 10", brdTest15TestFunction, brdTest15ValidationFunction)
     brdTestSuite.addTest(brdtest15)
@@ -4925,15 +4925,15 @@
 
         Event.SimulateFight(0.01, 500, False, PPSGraph=False, showProgress=False,computeGraph=False)
 
         return [MageBalladBuff in Dummy.buffList, round(player.SongTimer,2), player.Haste, Dummy.WanderingMinuet, Dummy.ArmyPaeon]
 
     def brdTest16ValidationFunction(testResults) -> (bool, list):
         passed = True
-        expected = [True,44.99, 0, False, False]   
+        expected = [True,44.99, 1, False, False]   
 
         for i in range(len(testResults)): passed = passed and (expected[i] == testResults[i])
 
         return passed , expected
 
     brdtest16 = test("Song test 11", brdTest16TestFunction, brdTest16ValidationFunction)
     brdTestSuite.addTest(brdtest16)
@@ -4957,15 +4957,15 @@
 
         Event.SimulateFight(0.01, 500, False, PPSGraph=False, showProgress=False,computeGraph=False)
 
         return [MageBalladBuff in Dummy.buffList, round(player.SongTimer,2), player.Haste, Dummy.WanderingMinuet]
 
     def brdTest17ValidationFunction(testResults) -> (bool, list):
         passed = True
-        expected = [True,44.99, 0, False]   
+        expected = [True,44.99, 2, False]   
 
         for i in range(len(testResults)): passed = passed and (expected[i] == testResults[i])
 
         return passed , expected
 
     brdtest17 = test("Song test 12", brdTest17TestFunction, brdTest17ValidationFunction)
     brdTestSuite.addTest(brdtest17)
@@ -5318,14 +5318,238 @@
         for i in range(len(testResults)): passed = passed and (expected[i] == testResults[i])
 
         return passed , expected
 
     brdtest26 = test("Battle Voice test 2", brdTest26TestFunction, brdTest26ValidationFunction)
     brdTestSuite.addTest(brdtest26)
 
+    def brdTest27TestFunction() -> None:
+        """
+        """
+
+        Dummy = Enemy()
+        Event = Fight(Dummy, False)
+        Stat = {'MainStat': 3378, 'WD': 132, 'Det': 1601, 'Ten': 400, 'SS': 400, 'SkS': 400, 'Crit': 2514, 'DH': 1402, 'Piety': 390}
+
+        actionSet = [MageBallad, WanderingMinuet, WaitAbility(5)]
+        player = Player(actionSet, [], Stat, JobEnum.Bard)
+
+        Event.AddPlayer([player])
+
+        Event.RequirementOn = False
+        Event.ShowGraph = False
+        Event.IgnoreMana = True
+
+        Event.SimulateFight(0.01, 500, False, PPSGraph=False, showProgress=False,computeGraph=False)
+
+        return [checkArmyEthos in player.EffectCDList, armyMuseCheck in player.EffectCDList]
+
+    def brdTest27ValidationFunction(testResults) -> (bool, list):
+        passed = True
+        expected = [False, False]   
+
+        for i in range(len(testResults)): passed = passed and (expected[i] == testResults[i])
+
+        return passed , expected
+
+    brdtest27 = test("Army Muse test 1", brdTest27TestFunction, brdTest27ValidationFunction)
+    brdTestSuite.addTest(brdtest27)
+
+    def brdTest28TestFunction() -> None:
+        """
+        """
+
+        Dummy = Enemy()
+        Event = Fight(Dummy, False)
+        Stat = {'MainStat': 3378, 'WD': 132, 'Det': 1601, 'Ten': 400, 'SS': 400, 'SkS': 400, 'Crit': 2514, 'DH': 1402, 'Piety': 390}
+
+        actionSet = [ArmyPaeon, WaitAbility(45),MageBallad, WaitAbility(5)]
+        player = Player(actionSet, [], Stat, JobEnum.Bard)
+
+        Event.AddPlayer([player])
+
+        Event.RequirementOn = False
+        Event.ShowGraph = False
+        Event.IgnoreMana = True
+
+        Event.SimulateFight(0.01, 500, False, PPSGraph=False, showProgress=False,computeGraph=False)
+
+        return [checkArmyEthos in player.EffectCDList, armyMuseCheck in player.EffectCDList, player.Haste]
+
+    def brdTest28ValidationFunction(testResults) -> (bool, list):
+        passed = True
+        expected = [False, True, 12]   
+
+        for i in range(len(testResults)): passed = passed and (expected[i] == testResults[i])
+
+        return passed , expected
+
+    brdtest28 = test("Army Muse test 2", brdTest28TestFunction, brdTest28ValidationFunction)
+    brdTestSuite.addTest(brdtest28)
+
+    def brdTest29TestFunction() -> None:
+        """
+        """
+
+        Dummy = Enemy()
+        Event = Fight(Dummy, False)
+        Stat = {'MainStat': 3378, 'WD': 132, 'Det': 1601, 'Ten': 400, 'SS': 400, 'SkS': 400, 'Crit': 2514, 'DH': 1402, 'Piety': 390}
+
+        actionSet = [ArmyPaeon, WaitAbility(45),MageBallad, WaitAbility(11)]
+        player = Player(actionSet, [], Stat, JobEnum.Bard)
+
+        Event.AddPlayer([player])
+
+        Event.RequirementOn = False
+        Event.ShowGraph = False
+        Event.IgnoreMana = True
+
+        Event.SimulateFight(0.01, 500, False, PPSGraph=False, showProgress=False,computeGraph=False)
+
+        return [checkArmyEthos in player.EffectCDList, armyMuseCheck in player.EffectCDList, player.Haste]
+
+    def brdTest29ValidationFunction(testResults) -> (bool, list):
+        passed = True
+        expected = [False, False, 0]   
+
+        for i in range(len(testResults)): passed = passed and (expected[i] == testResults[i])
+
+        return passed , expected
+
+    brdtest29 = test("Army Muse test 3", brdTest29TestFunction, brdTest29ValidationFunction)
+    brdTestSuite.addTest(brdtest29)
+
+    def brdTest30TestFunction() -> None:
+        """
+        """
+
+        Dummy = Enemy()
+        Event = Fight(Dummy, False)
+        Stat = {'MainStat': 3378, 'WD': 132, 'Det': 1601, 'Ten': 400, 'SS': 400, 'SkS': 400, 'Crit': 2514, 'DH': 1402, 'Piety': 390}
+
+        actionSet = [ArmyPaeon, WaitAbility(45),WanderingMinuet, WaitAbility(5)]
+        player = Player(actionSet, [], Stat, JobEnum.Bard)
+
+        Event.AddPlayer([player])
+
+        Event.RequirementOn = False
+        Event.ShowGraph = False
+        Event.IgnoreMana = True
+
+        Event.SimulateFight(0.01, 500, False, PPSGraph=False, showProgress=False,computeGraph=False)
+
+        return [checkArmyEthos in player.EffectCDList, armyMuseCheck in player.EffectCDList, player.Haste]
+
+    def brdTest30ValidationFunction(testResults) -> (bool, list):
+        passed = True
+        expected = [False, True, 12]   
+
+        for i in range(len(testResults)): passed = passed and (expected[i] == testResults[i])
+
+        return passed , expected
+
+    brdtest30 = test("Army Muse test 4", brdTest30TestFunction, brdTest30ValidationFunction)
+    brdTestSuite.addTest(brdtest30)
+
+    def brdTest31TestFunction() -> None:
+        """
+        """
+
+        Dummy = Enemy()
+        Event = Fight(Dummy, False)
+        Stat = {'MainStat': 3378, 'WD': 132, 'Det': 1601, 'Ten': 400, 'SS': 400, 'SkS': 400, 'Crit': 2514, 'DH': 1402, 'Piety': 390}
+
+        actionSet = [ArmyPaeon, WaitAbility(45),WanderingMinuet, WaitAbility(11)]
+        player = Player(actionSet, [], Stat, JobEnum.Bard)
+
+        Event.AddPlayer([player])
+
+        Event.RequirementOn = False
+        Event.ShowGraph = False
+        Event.IgnoreMana = True
+
+        Event.SimulateFight(0.01, 500, False, PPSGraph=False, showProgress=False,computeGraph=False)
+
+        return [checkArmyEthos in player.EffectCDList, armyMuseCheck in player.EffectCDList, player.Haste]
+
+    def brdTest31ValidationFunction(testResults) -> (bool, list):
+        passed = True
+        expected = [False, False, 0]   
+
+        for i in range(len(testResults)): passed = passed and (expected[i] == testResults[i])
+
+        return passed , expected
+
+    brdtest31 = test("Army Muse test 5", brdTest31TestFunction, brdTest31ValidationFunction)
+    brdTestSuite.addTest(brdtest31)
+
+    def brdTest32TestFunction() -> None:
+        """
+        """
+
+        Dummy = Enemy()
+        Event = Fight(Dummy, False)
+        Stat = {'MainStat': 3378, 'WD': 132, 'Det': 1601, 'Ten': 400, 'SS': 400, 'SkS': 400, 'Crit': 2514, 'DH': 1402, 'Piety': 390}
+
+        actionSet = [ArmyPaeon, WaitAbility(46)]
+        player = Player(actionSet, [], Stat, JobEnum.Bard)
+
+        Event.AddPlayer([player])
+
+        Event.RequirementOn = False
+        Event.ShowGraph = False
+        Event.IgnoreMana = True
+
+        Event.SimulateFight(0.01, 500, False, PPSGraph=False, showProgress=False,computeGraph=False)
+
+        return [checkArmyEthos in player.EffectCDList, armyMuseCheck in player.EffectCDList, player.Haste]
+
+    def brdTest32ValidationFunction(testResults) -> (bool, list):
+        passed = True
+        expected = [True, False, 0]   
+
+        for i in range(len(testResults)): passed = passed and (expected[i] == testResults[i])
+
+        return passed , expected
+
+    brdtest32 = test("Army Muse test 6", brdTest32TestFunction, brdTest32ValidationFunction)
+    brdTestSuite.addTest(brdtest32)
+
+    def brdTest33TestFunction() -> None:
+        """
+        """
+
+        Dummy = Enemy()
+        Event = Fight(Dummy, False)
+        Stat = {'MainStat': 3378, 'WD': 132, 'Det': 1601, 'Ten': 400, 'SS': 400, 'SkS': 400, 'Crit': 2514, 'DH': 1402, 'Piety': 390}
+
+        actionSet = [ArmyPaeon, WaitAbility(46), WaitAbility(30), MageBallad, WaitAbility(0.1)]
+        player = Player(actionSet, [], Stat, JobEnum.Bard)
+
+        Event.AddPlayer([player])
+
+        Event.RequirementOn = False
+        Event.ShowGraph = False
+        Event.IgnoreMana = True
+
+        Event.SimulateFight(0.01, 500, False, PPSGraph=False, showProgress=False,computeGraph=False)
+
+        return [checkArmyEthos in player.EffectCDList, armyMuseCheck in player.EffectCDList, player.Haste]
+
+    def brdTest33ValidationFunction(testResults) -> (bool, list):
+        passed = True
+        expected = [False, False, 0]   
+
+        for i in range(len(testResults)): passed = passed and (expected[i] == testResults[i])
+
+        return passed , expected
+
+    brdtest33 = test("Army Muse test 7", brdTest33TestFunction, brdTest33ValidationFunction)
+    brdTestSuite.addTest(brdtest33)
+
     return brdTestSuite
 
 ######################################
 #           Dancer testSuite           #
 ######################################
 
 def generateDNCTestSuite() -> testSuite:
```

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/UI/SimulationInput.py` & `ffxivcalc-0.8.940/src/ffxivcalc/UI/SimulationInput.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/UI/TUI.py` & `ffxivcalc-0.8.940/src/ffxivcalc/UI/TUI.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/__init__.py` & `ffxivcalc-0.8.940/src/ffxivcalc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-__version__ = '0.8.930'
+__version__ = '0.8.940'
 
 """
 Update history :
 
+0.9.940:
+    - Oups, forgot to ever implement Army Ethos/Army Muse effect on Bard. This is now fixed.
+    - Other bug fixes.
+
 0.8.930:
     - Added Player.getPlayerPrePullTime() which returns the length of the prepull (time before first damage action).
     - Added Fight.getPlayerPrepullLength() which returns the prepull length of all players
     - added Fight.syncPlayerPrePull() which syncs all player's prepull so they all do damage at the same time.
     - Added test suite 'Prepull length test suite' that tests the Player.GetPlayerPrePullTime() function.
     - Removed access to ffxvivcalc.API, ffxivcalc.codeParser and ffxivcalc.Request.FFLogsAPIRequest modules (outdated modules).
     - Other minor bug fix.
```

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/__main__.py` & `ffxivcalc-0.8.940/src/ffxivcalc/__main__.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/codeParser/parser.py` & `ffxivcalc-0.8.940/src/ffxivcalc/codeParser/parser.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/helperCode/Progress.py` & `ffxivcalc-0.8.940/src/ffxivcalc/helperCode/Progress.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/helperCode/Vocal.py` & `ffxivcalc-0.8.940/src/ffxivcalc/helperCode/Vocal.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/helperCode/exceptions.py` & `ffxivcalc-0.8.940/src/ffxivcalc/helperCode/exceptions.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/helperCode/helper_backend.py` & `ffxivcalc-0.8.940/src/ffxivcalc/helperCode/helper_backend.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/helperCode/lookUpAbilityID.py` & `ffxivcalc-0.8.940/src/ffxivcalc/helperCode/lookUpAbilityID.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc/helperCode/requirementHandler.py` & `ffxivcalc-0.8.940/src/ffxivcalc/helperCode/requirementHandler.py`

 * *Files identical despite different names*

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc.egg-info/PKG-INFO` & `ffxivcalc-0.8.940/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,35 @@
-Metadata-Version: 2.1
-Name: ffxivcalc
-Version: 0.8.930
-Summary: DPS simulator for Final Fantasy XIV.
-Home-page: https://github.com/IAmPythagoras/FFXIV-Combat-Simulator
-Author: Anthony Desrochers
-Author-email: anthony.desrochers17@gmail.com
-Project-URL: Source, https://github.com/IAmPythagoras/FFXIV-Combat-Simulator
-Project-URL: Site, https://ffxivdpscalc.azurewebsites.net/simulate/
-Project-URL: Documentation, https://iampythagoras.github.io/index.html
-Keywords: ffxiv,xiv,dps,simulator,ffxiv-combat-simulator
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: License.md
-Requires-Dist: contourpy
-Requires-Dist: cycler
-Requires-Dist: fonttools
-Requires-Dist: kiwisolver
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: packaging
-Requires-Dist: Pillow
-Requires-Dist: pyparsing
-Requires-Dist: python-dateutil
-Requires-Dist: six
-Requires-Dist: coreapi
-Requires-Dist: pandas
-Requires-Dist: python_graphql_client
-
 [![Discord](https://img.shields.io/discord/970724799464738977?color=7289da&label=Discord&logo=discord)](https://discord.gg/mZXKUNy2sw)
 
-# Website
+# Desktop app
 
-The website https://ffxivdpscalc.azurewebsites.net allows an easier time for people without coding knowledge to use the simulator.
-It uses the most up to date version of FFIXV-Combat-Simulator, but has some limitations to keep computation time low.
+You can download the desktop app to use the simulator without having to code : https://github.com/IAmPythagoras/ffxivcalcWebApp .
 
 # Install
 
 You can install this library using pip : 
 
 ```
 pip install ffxivcalc
 ```
 
-or using git (this would let you download from the dev branch "feature/GeneralDev"): 
+Or can download latest unstable version using : 
 
 ```
-pip install ffxiv-combat-simulator@git+https://github.com/IAmPythagoras/FFXIV-Combat-Simulator.git@main
+pip install ffxiv-combat-simulator@git+https://github.com/IAmPythagoras/FFXIV-Combat-Simulator.git@feature/GeneralDev
 ```
 
 *Note that you must have git installed : https://git-scm.com/download/win 
 
 You can find the documentation here : https://iampythagoras.github.io/index.html or join the discord linked above if you have any questions.
 
-If you want to locally use the API. Install the ffxiv-combat-simulator library and also install uvicorn :
-```
-pip install uvicorn
+*The unstable version can be removed using
 ```
-And then run this command:
+pip uninstall ffxiv-combat-simulator
 ```
-python -m uvicorn ffxivcalc.API.API:app
-```
-This will locally launch the API.
 
 # FFXIV-Combat-Simulator (ffxivcalc)
 
 This Python library lets you simulate combat from the game Final Fantasy XIV. It allows for as many players as possible and will simulate the fight in "real time". It
 accurately keeps track of MP, cooldown on abilities, HP, DOTs, raid buffs, personnal buffs, team composition bonus, potions buff, which allows for a dynamic environment that portrays as accurately as possible the real game's environment.
 
 The simulator in its base state will output every player's DPS (Damage Per Second), PPS (Potency Per Second), TP (Total Potency), but it can be customized to output any other metric that could be useful. Furthermore, the simulator is able to output a distribution of the DPS which allows to see the different DPS' percentiles.
@@ -99,51 +60,41 @@
 
 ![image](https://github.com/IAmPythagoras/FFXIV-Combat-Simulator/assets/62820030/88069e5d-8ffa-4783-acc3-b1b02c3ce33e)
 
 This record's goal is to act as a sort of log, but which is more easily understood and contains only the most useful information on the running of the simulation.
 You can also export a text only version of this record.
 # Rotation BiS Solver 
 
-As of ffxivcalc version 0.8.00, this library now has a built in rotation BiS solver. You can use the ffxivcalclayout.py in order to experiment with it.
+As of ffxivcalc version 0.8.00, this library now has a built in rotation BiS solver. You can use the ffxivcalclayout.py in order to experiment with it or download the desktop app.
 
 You can read this PDF [BiS_Solver_Algorithm_Documentation.pdf](https://github.com/IAmPythagoras/FFXIV-Combat-Simulator/files/12580553/BiS_Solver_Algorithm_Documentation.pdf) if you are interested in its
 functionning. 
 
 You can read about the experimental results of this solver here : https://docs.google.com/spreadsheets/d/1yVl-F1tHARYIYvz4ZPxIY6MayakYug3OEqpGnpZllqU/edit?usp=sharing
 
 # Validity of simulator
 
-As of version 0.8.30 I have started adding in depth testing of the simulator. The simulator will still have some flaws, but it is currently being checked by around 430 individual tests. More tests
-will be added with time.
-
-# Discord bot): 
-DISCORD BOT IS CURRENTLY OFFLINE. WILL UPDATE HERE WHEN IT IS AVAILABLE
-I made a disbord bot that uses the python library ffxivcalc in order to simulate fights. Feel free to install it using the link below. As of now, the main bot commands are :
-```
-!Simulate (With a JSON file as a file in the same message)
-!Template <filename> <job1> <job2> ... (Generates a template JSON file used to simulate)
-!Help (for help)
-```
-Use this link to install the bot on your server : 
-```
-https://discord.com/oauth2/authorize?client_id=1071922835011932290&permissions=274878024704&scope=bot
-```
+As of version 0.8.940 I have started adding in depth testing of the simulator. The simulator will still have some flaws, but it is currently being checked by around 800 individual tests. More tests will be added with time.
 
-# Currently Working On
+# Other simulators
 
-Adding code to support multiple enemies at the same time and individual targetting of enemy by the players.
+Make sure to check out this alternative FFXIV simulator [Amas-FF14-Combat-Sim](https://github.com/Amarantine-xiv/Amas-FF14-Combat-Sim) or join its [Discord](https://discord.gg/8GjA5uRcDX)
 
+# If you want to help
 
-# HOW IT WORKS
-
-The big advantage of this program is that instead of computing the average PPS (potency per second) and then using a damage formula to find the
-DPS (Damage per second), it simulates the fight like it would happen in real time. That way, buffs are accurately taken into account. It is also able to discernate between oGCD and GCD, and will treat them accordingly (for weaving and stuff).The program can also see if a rotation is illegal, and will stop if it is determined to be a rotation that cannot be done in the game.
-
-The time-unit used for the program is by default 0.01s/step, but it can be put at whatever smaller (or bigger) number we prefer. It is also able to know when a certain ability cannot be casted, and using that ability anyway will result in an error that stops the simulation. We could in theory disable this checking if we wanted.
-
-Each job in the game is implemented in a relatively similar way. We first create a class JobSpell, which will be an object that will represent a spell/ability/weaponskill of the job. Such an object will have information like casting time, recast time (if GCD), potency, manacost, effect of applying that spell and the requirements of that spell. We then also need to create a class JobPlayer, which will inherit certain traits for its parent class (Healer, Caster, Melee, Ranged or Tank) (This is also the case for spell). This JobPlayer class will contain information like Ability Cooldown, Buff Timer, DOTTimer and other stuff that need to be tracked during the execution of the simulation.
+If you want to help or want to ask questions to me directly, feel free to join the discord linked above:)
 
-And that's about it, the code will take these two new classes (and object of the JobSpell class) and if everything is done correctly the simulator will be able to run without any issues.
+# Update log
 
-# If you want to help
+(Recent only read __init__.py for all update logs)
 
-If you want to help or want to ask questions to me directly, feel free to join the discord linked above:)
+0.9.940:
+    - Oups, forgot to ever implement Army Ethos/Army Muse effect on Bard. This is now fixed.
+    - Other bug fixes.
+
+0.8.930:
+    - Added Player.getPlayerPrePullTime() which returns the length of the prepull (time before first damage action).
+    - Added Fight.getPlayerPrepullLength() which returns the prepull length of all players
+    - added Fight.syncPlayerPrePull() which syncs all player's prepull so they all do damage at the same time.
+    - Added test suite 'Prepull length test suite' that tests the Player.GetPlayerPrePullTime() function.
+    - Removed access to ffxvivcalc.API, ffxivcalc.codeParser and ffxivcalc.Request.FFLogsAPIRequest modules (outdated modules).
+    - Other minor bug fix.
```

### Comparing `ffxivcalc-0.8.930/src/ffxivcalc.egg-info/SOURCES.txt` & `ffxivcalc-0.8.940/src/ffxivcalc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

