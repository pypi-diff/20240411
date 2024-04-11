# Comparing `tmp/PlexTraktSync-0.29.8.tar.gz` & `tmp/PlexTraktSync-0.29.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlexTraktSync-0.29.8.tar", last modified: Sun Mar 17 17:58:52 2024, max compression
+gzip compressed data, was "PlexTraktSync-0.29.9.tar", last modified: Tue Mar 26 22:39:34 2024, max compression
```

## Comparing `PlexTraktSync-0.29.8.tar` & `PlexTraktSync-0.29.9.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.671116 PlexTraktSync-0.29.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    29730 2024-03-17 17:58:52.671116 PlexTraktSync-0.29.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.671116 PlexTraktSync-0.29.8/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29730 2024-03-17 17:58:52.000000 PlexTraktSync-0.29.8/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-03-17 17:58:52.000000 PlexTraktSync-0.29.8/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 17:58:52.000000 PlexTraktSync-0.29.8/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-17 17:58:52.000000 PlexTraktSync-0.29.8/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-17 17:58:52.000000 PlexTraktSync-0.29.8/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-17 17:58:52.000000 PlexTraktSync-0.29.8/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26700 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.651116 PlexTraktSync-0.29.8/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.655116 PlexTraktSync-0.29.8/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.655116 PlexTraktSync-0.29.8/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/config/ServerConfigFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.659116 PlexTraktSync-0.29.8/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.659116 PlexTraktSync-0.29.8/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/logger/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.659116 PlexTraktSync-0.29.8/plextraktsync/media/
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/media/Media.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/media/MediaFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.659116 PlexTraktSync-0.29.8/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/mixin/RichMarkup.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/mixin/SetWindowTitle.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.659116 PlexTraktSync-0.29.8/plextraktsync/plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plan/WalkConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plan/WalkPlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plan/WalkPlanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plan/Walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.663116 PlexTraktSync-0.29.8/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexGuidProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexGuidProviderIMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexGuidProviderLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexGuidProviderMbid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexGuidProviderTMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexGuidProviderTVDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexId.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexIdFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexPlaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexPlaylistCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexSectionPager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/plex/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.663116 PlexTraktSync-0.29.8/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/queue/TraktScrobbleWorker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.663116 PlexTraktSync-0.29.8/plextraktsync/rich/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/rich/RichHighlighter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/rich/RichProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.663116 PlexTraktSync-0.29.8/plextraktsync/sync/
--rw-r--r--   0 runner    (1001) docker     (127)    10783 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/sync/Sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.667116 PlexTraktSync-0.29.8/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10006 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/trakt/TraktUserList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/trakt/TraktUserListCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/trakt/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.667116 PlexTraktSync-0.29.8/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/Rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/util/remove_empty_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.671116 PlexTraktSync-0.29.8/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-17 17:58:50.000000 PlexTraktSync-0.29.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-17 17:58:52.671116 PlexTraktSync-0.29.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 17:58:52.671116 PlexTraktSync-0.29.8/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/tests/test_logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/tests/test_plex_id.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/tests/test_rating.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3584 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-03-17 17:58:48.000000 PlexTraktSync-0.29.8/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.567499 PlexTraktSync-0.29.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    29730 2024-03-26 22:39:34.567499 PlexTraktSync-0.29.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.567499 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29730 2024-03-26 22:39:34.000000 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-03-26 22:39:34.000000 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 22:39:34.000000 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-26 22:39:34.000000 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-26 22:39:34.000000 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-26 22:39:34.000000 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26700 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.547499 PlexTraktSync-0.29.9/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.551499 PlexTraktSync-0.29.9/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.551499 PlexTraktSync-0.29.9/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/ServerConfigFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.551499 PlexTraktSync-0.29.9/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.551499 PlexTraktSync-0.29.9/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/logger/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.551499 PlexTraktSync-0.29.9/plextraktsync/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/media/Media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/media/MediaFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.551499 PlexTraktSync-0.29.9/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/mixin/RichMarkup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/mixin/SetWindowTitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.555499 PlexTraktSync-0.29.9/plextraktsync/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plan/WalkConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plan/WalkPlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plan/WalkPlanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plan/Walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.555499 PlexTraktSync-0.29.9/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderIMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderMbid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderTMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderTVDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexIdFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexPlaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexPlaylistCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexSectionPager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.559499 PlexTraktSync-0.29.9/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/queue/TraktScrobbleWorker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.559499 PlexTraktSync-0.29.9/plextraktsync/rich/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/rich/RichHighlighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/rich/RichProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.559499 PlexTraktSync-0.29.9/plextraktsync/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/sync/Sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.559499 PlexTraktSync-0.29.9/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10006 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktUserList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktUserListCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.563499 PlexTraktSync-0.29.9/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/Rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/remove_empty_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.563499 PlexTraktSync-0.29.9/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-26 22:39:32.000000 PlexTraktSync-0.29.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-26 22:39:34.567499 PlexTraktSync-0.29.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.563499 PlexTraktSync-0.29.9/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_plex_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_rating.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3584 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_walker.py
```

### Comparing `PlexTraktSync-0.29.8/LICENSE` & `PlexTraktSync-0.29.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/PKG-INFO` & `PlexTraktSync-0.29.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.29.8
+Version: 0.29.9
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexTraktSync-0.29.8/PlexTraktSync.egg-info/PKG-INFO` & `PlexTraktSync-0.29.9/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.29.8
+Version: 0.29.9
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexTraktSync-0.29.8/PlexTraktSync.egg-info/SOURCES.txt` & `PlexTraktSync-0.29.9/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/PlexTraktSync.egg-info/requires.txt` & `PlexTraktSync-0.29.9/PlexTraktSync.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/README.md` & `PlexTraktSync-0.29.9/README.md`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/cli.py` & `PlexTraktSync-0.29.9/plextraktsync/cli.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/bug_report.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/cache.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/clear_collections.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/config.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/download.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/imdb_import.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/info.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/inspect.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         print("Subtitles:")
         for index, subtitle in enumerate(pm.subtitle_streams, start=1):
             print(f"  Subtitle {index}: ({subtitle.language}) {subtitle.title} (codec: {subtitle.codec}, selected: {subtitle.selected}, transient: {subtitle.transient})")
 
         print("Parts:")
         for index, part in enumerate(pm.parts, start=1):
-            print(f"  Part {index}: [link=file://{quote_plus(part.file)}]{escape(part.file)}[/link] {part.size} bytes")
+            print(f"  Part {index} (exists: {part.exists}): [link=file://{quote_plus(part.file)}]{escape(part.file)}[/link] {part.size} bytes")
 
         print("Markers:")
         for marker in pm.markers:
             start = millisecondToHumanstr(marker.start)
             end = millisecondToHumanstr(marker.end)
             print(f"  {marker.type}: {start} - {end}")
```

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/login.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/plex_login.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/self_update.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/sync.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/sync.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/trakt_login.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/unmatched.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/unmatched.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/watch.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/commands/watched_shows.py` & `PlexTraktSync-0.29.9/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/config/Config.py` & `PlexTraktSync-0.29.9/plextraktsync/config/Config.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,19 +22,19 @@
         # have a Plex account, they're local users.
         "PLEX_OWNER_TOKEN": True,
         # The account token of the Plex user who have a Plex account but don't
         # own the PMS (use it as shared library).
         # This is stored/used only if user uses a shared PMS.
         # Needed to fetch its watchlist from Plex online servers.
         "PLEX_ACCOUNT_TOKEN": True,
-        # Old keys, Leave comment why deprecated
-        "PLEX_FALLBACKURL": "Legacy, used before 0.18.21",
-        "PLEX_BASEURL": "Unused after 0.24.0, moved to servers.yml",
-        "PLEX_LOCALURL": "Unused after 0.24.0, moved to servers.yml",
-        "PLEX_TOKEN": "Unused after 0.24.0, moved to servers.yml",
+        # Old keys, Do not write to .env anymore
+        "PLEX_FALLBACKURL": False,
+        "PLEX_BASEURL": False,
+        "PLEX_LOCALURL": False,
+        "PLEX_TOKEN": False,
     }
 
     initialized = False
     config_file = config_file
     config_yml = config_yml
     env_file = env_file
 
@@ -153,14 +153,18 @@
             return dump
         print(dump)
 
     def save(self):
         with open(self.env_file, "w") as txt:
             txt.write("# This is .env file for PlexTraktSync\n")
             for key, value in self.env_keys.items():
+                if value is False:
+                    # Skip the item
+                    continue
+
                 if value is not True:
                     # Include deprecation message
                     txt.write(f"# {key}: {value}\n")
 
                 if key in self and self[key] is not None:
                     txt.write(f"{key}={self[key]}\n")
                 else:
```

### Comparing `PlexTraktSync-0.29.8/plextraktsync/config/ConfigLoader.py` & `PlexTraktSync-0.29.9/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/config/HttpCacheConfig.py` & `PlexTraktSync-0.29.9/plextraktsync/config/HttpCacheConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,39 +39,45 @@
         "api.trakt.tv/users/*/collection/shows": "1m",
         "api.trakt.tv/users/*/ratings/episodes": "1m",
         "api.trakt.tv/users/*/ratings/shows": "1m",
         "api.trakt.tv/users/*/ratings/movies": "1m",
         # Trakt search urls
         "api.trakt.tv/search/imdb/tt*?type=movie": "1d",
         "api.trakt.tv/search/imdb/tt*?type=show": "1d",
+        "api.trakt.tv/search/imdb/tt*?type=episode": "1d",
         "api.trakt.tv/search/tmdb/*?type=movie": "1d",
         "api.trakt.tv/search/tmdb/*?type=show": "1d",
+        "api.trakt.tv/search/tmdb/*?type=episode": "1d",
         "api.trakt.tv/search/tvdb/*?type=show": "1d",
+        "api.trakt.tv/search/tvdb/*?type=episode": "1d",
         # Keep watched status cached, but fresh
         "api.trakt.tv/sync/watched/shows": "1s",
         "api.trakt.tv/users/*/watched/movies": "1s",
         # Watchlist better be fresh for next run
         "api.trakt.tv/users/*/watchlist/movies": "1s",
         "api.trakt.tv/users/*/watchlist/shows": "1s",
         "metadata.provider.plex.tv/library/sections/watchlist/all?*includeUserState=0": "1s",
         "metadata.provider.plex.tv/library/sections/watchlist/all": "1s",
         "api.trakt.tv/users/likes/lists": DO_NOT_CACHE,
         "api.trakt.tv/users/me": DO_NOT_CACHE,
+        # Public Lists
+        "api.trakt.tv/lists/*": "1d",
         # Online Plex patterns
         "metadata.provider.plex.tv/library/metadata/*/userState": DO_NOT_CACHE,
         "metadata.provider.plex.tv/library/metadata/*?*includeUserState=1": DO_NOT_CACHE,
         "metadata.provider.plex.tv/library/metadata/*": LONG_EXPIRY,
         "metadata.provider.plex.tv/library/search?query=*&searchTypes=movies&includeMetadata=1": "1h",
         "metadata.provider.plex.tv/library/search?query=*&searchTypes=tv&includeMetadata=1": "1h",
         # https://web.dev/stale-while-revalidate/
         # cache-control: max-age=0,stale-while-revalidate=86400
         "metadata.provider.plex.tv/": 86400,
         # Plex account
         # Cache for some time, this activates 304 responses
         "plex.tv/users/account": "1m",
+        "plex.tv/api/v2/user": "1m",
         # Plex patterns
         # Ratings search
         "*/library/sections/*/all?*userRating%3E%3E=-1*": DO_NOT_CACHE,
         # len(PlexLibrarySection)
         "*/library/sections/*/all?includeCollections=0&X-Plex-Container-Size=0&X-Plex-Container-Start=0": DO_NOT_CACHE,
         # __iter__(PlexLibrarySection)
         "*/library/sections/*/all?includeGuids=1": DO_NOT_CACHE,
```

### Comparing `PlexTraktSync-0.29.8/plextraktsync/config/PlexServerConfig.py` & `PlexTraktSync-0.29.9/plextraktsync/config/PlexServerConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/config/ServerConfigFactory.py` & `PlexTraktSync-0.29.9/plextraktsync/config/ServerConfigFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/config/SyncConfig.py` & `PlexTraktSync-0.29.9/plextraktsync/config/SyncConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/config.default.yml` & `PlexTraktSync-0.29.9/plextraktsync/config.default.yml`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/decorators/rate_limit.py` & `PlexTraktSync-0.29.9/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/decorators/retry.py` & `PlexTraktSync-0.29.9/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/logger/filter.py` & `PlexTraktSync-0.29.9/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/logger/init.py` & `PlexTraktSync-0.29.9/plextraktsync/logger/init.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/media/Media.py` & `PlexTraktSync-0.29.9/plextraktsync/media/Media.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/media/MediaFactory.py` & `PlexTraktSync-0.29.9/plextraktsync/media/MediaFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/mixin/ChangeNotifier.py` & `PlexTraktSync-0.29.9/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plan/WalkConfig.py` & `PlexTraktSync-0.29.9/plextraktsync/plan/WalkConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plan/WalkPlanner.py` & `PlexTraktSync-0.29.9/plextraktsync/plan/WalkPlanner.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plan/Walker.py` & `PlexTraktSync-0.29.9/plextraktsync/plan/Walker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexApi.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexAudioCodec.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexGuid.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexGuidProvider.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProvider.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexGuidProviderMbid.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderMbid.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexGuidProviderTMDB.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderTMDB.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexId.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexId.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexIdFactory.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexIdFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexLibraryItem.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexLibraryItem.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,16 +172,18 @@
             return self.item.markers
         except AttributeError:
             # If not enough access to server, the markers attribute is missing
             return []
 
     @property
     def parts(self) -> list[MediaPart]:
-        item = self.plex.fetch_item(self.item.ratingKey)
-        for media in item.item.media:
+        if self.item.isPartialObject():
+            self.item.reload()
+
+        for media in self.item.media:
             yield from media.parts
 
     @property
     def audio_streams(self):
         return self.item.audioStreams()
 
     @property
@@ -347,16 +349,20 @@
 
         self._show = show
 
     @staticmethod
     def date_value(date) -> datetime.datetime | None:
         if not date:
             return None
-
-        return date.astimezone(datetime.timezone.utc)
+        try:
+            return date.astimezone(datetime.timezone.utc)
+        except OSError:
+            # python on Windows cannot find tz for pre-epoch dates
+            # https://github.com/python/cpython/issues/80940
+            return date
 
     @property
     def title_link(self):
         if self.plex:
             link = self.plex.media_url(self)
 
             return self.markup_link(link, self.title)
```

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexLibrarySection.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexLibrarySection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexPlaylist.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexPlaylist.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexRatings.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexRatings.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexSectionPager.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexSectionPager.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexServerConnection.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexServerConnection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/PlexWatchList.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/plex/SessionCollection.py` & `PlexTraktSync-0.29.9/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/pytrakt_extensions.py` & `PlexTraktSync-0.29.9/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/queue/BackgroundTask.py` & `PlexTraktSync-0.29.9/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/queue/Queue.py` & `PlexTraktSync-0.29.9/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/queue/TraktBatchWorker.py` & `PlexTraktSync-0.29.9/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/queue/TraktMarkWatchedWorker.py` & `PlexTraktSync-0.29.9/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/queue/TraktScrobbleWorker.py` & `PlexTraktSync-0.29.9/plextraktsync/queue/TraktScrobbleWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/rich/RichHighlighter.py` & `PlexTraktSync-0.29.9/plextraktsync/rich/RichHighlighter.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/rich/RichProgressBar.py` & `PlexTraktSync-0.29.9/plextraktsync/rich/RichProgressBar.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/sync/Sync.py` & `PlexTraktSync-0.29.9/plextraktsync/sync/Sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     def sync_collection(self, m: Media, dry_run=False):
         if not self.config.plex_to_trakt["collection"]:
             return
 
         if m.is_collected:
             return
 
-        self.logger.info(f"Adding to collection: {m.title_link}", extra={"markup": True})
+        self.logger.info(f"Adding to Trakt collection: {m.title_link}", extra={"markup": True})
 
         if not dry_run:
             m.add_to_collection()
 
     def sync_ratings(self, m: Media, dry_run=False):
         if not self.config.sync_ratings:
             return
```

### Comparing `PlexTraktSync-0.29.8/plextraktsync/trakt/ScrobblerCollection.py` & `PlexTraktSync-0.29.9/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/trakt/ScrobblerProxy.py` & `PlexTraktSync-0.29.9/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/trakt/TraktApi.py` & `PlexTraktSync-0.29.9/plextraktsync/trakt/TraktApi.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/trakt/TraktLookup.py` & `PlexTraktSync-0.29.9/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/trakt/TraktRatingCollection.py` & `PlexTraktSync-0.29.9/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/trakt/TraktUserList.py` & `PlexTraktSync-0.29.9/plextraktsync/trakt/TraktUserList.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/trakt/TraktUserListCollection.py` & `PlexTraktSync-0.29.9/plextraktsync/trakt/TraktUserListCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/trakt/TraktWatchlist.py` & `PlexTraktSync-0.29.9/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/util/Factory.py` & `PlexTraktSync-0.29.9/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/util/Path.py` & `PlexTraktSync-0.29.9/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/util/Rating.py` & `PlexTraktSync-0.29.9/plextraktsync/util/Rating.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/util/Timer.py` & `PlexTraktSync-0.29.9/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/util/Version.py` & `PlexTraktSync-0.29.9/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/util/local_url.py` & `PlexTraktSync-0.29.9/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/util/openurl.py` & `PlexTraktSync-0.29.9/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/util/packaging.py` & `PlexTraktSync-0.29.9/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/util/remove_empty_values.py` & `PlexTraktSync-0.29.9/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/watch/EventDispatcher.py` & `PlexTraktSync-0.29.9/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/watch/EventFactory.py` & `PlexTraktSync-0.29.9/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/watch/ProgressBar.py` & `PlexTraktSync-0.29.9/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/watch/WatchStateUpdater.py` & `PlexTraktSync-0.29.9/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/watch/WebSocketListener.py` & `PlexTraktSync-0.29.9/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/plextraktsync/watch/events.py` & `PlexTraktSync-0.29.9/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/requirements.txt` & `PlexTraktSync-0.29.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/setup.cfg` & `PlexTraktSync-0.29.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/tests/test_collection_metadata.py` & `PlexTraktSync-0.29.9/tests/test_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/tests/test_config.py` & `PlexTraktSync-0.29.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/tests/test_events.py` & `PlexTraktSync-0.29.9/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/tests/test_new_agent.py` & `PlexTraktSync-0.29.9/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/tests/test_plex_id.py` & `PlexTraktSync-0.29.9/tests/test_plex_id.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/tests/test_rating.py` & `PlexTraktSync-0.29.9/tests/test_rating.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/tests/test_timer.py` & `PlexTraktSync-0.29.9/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/tests/test_trakt_progress.py` & `PlexTraktSync-0.29.9/tests/test_trakt_progress.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/tests/test_tv_lookup.py` & `PlexTraktSync-0.29.9/tests/test_tv_lookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.8/tests/test_walker.py` & `PlexTraktSync-0.29.9/tests/test_walker.py`

 * *Files identical despite different names*

