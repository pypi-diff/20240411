# Comparing `tmp/xklb-2.5.9.tar.gz` & `tmp/xklb-2.6.1.tar.gz`

## Comparing `xklb-2.5.9.tar` & `xklb-2.6.1.tar`

### file list

```diff
@@ -1,117 +1,122 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.5.9/.gitattributes
--rw-r--r--   0        0        0   203078 2020-02-02 00:00:00.000000 xklb-2.5.9/pdm.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/FUNDING.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/LICENSE
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/Windows.md
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/examples/extract.svg
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/examples/tubeadd.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/__init__.py
--rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/db_media.py
--rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/db_playlists.py
--rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/dl_extract.py
--rw-r--r--   0        0        0    16853 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/fs_extract.py
--rw-r--r--   0        0        0     8133 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/gdl_backend.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/gdl_extract.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/history.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/hn_extract.py
--rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/lb.py
--rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/play_actions.py
--rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/post_actions.py
--rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/readme.py
--rw-r--r--   0        0        0    13292 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/reddit_extract.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/rss_extract.py
--rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/search.py
--rw-r--r--   0        0        0     6810 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/site_extract.py
--rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/tabs_extract.py
--rw-r--r--   0        0        0    19687 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/tube_backend.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/tube_extract.py
--rw-r--r--   0        0        0   111452 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/data/__init__.py
--rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/data/dl_config.py
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/data/wordbank.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/__init__.py
--rw-r--r--   0        0        0     9165 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/av.py
--rw-r--r--   0        0        0     7484 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/books.py
--rw-r--r--   0        0        0    16296 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/dedupe.py
--rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/media_check.py
--rw-r--r--   0        0        0    23526 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/media_player.py
--rw-r--r--   0        0        0     9411 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/media_printer.py
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/subtitle.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scratch/__init__.py
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scratch/javguru.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scratch/javtiful.py
--rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scratch/mam_search.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scratch/mam_slots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     8314 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/big_dirs.py
--rw-r--r--   0        0        0    12252 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/block.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/christen.py
--rw-r--r--   0        0        0    14173 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0    14120 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/dedupe_czkawka.py
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/disk_usage.py
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/eda.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/export_text.py
--rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/history.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/incremental_diff.py
--rw-r--r--   0        0        0    13991 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/links_db.py
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mcda.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/merge_folders.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/move_list.py
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/open_links.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/places_import.py
--rw-r--r--   0        0        0     9972 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/process_audio.py
--rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/rel_mv.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/sample_compare.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/sample_hash.py
--rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/search_db.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/web_add.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     9591 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/extract_text.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/markdown_links.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/substack.py
--rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/tildes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/__init__.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/arg_utils.py
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/consts.py
--rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/db_utils.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/devices.py
--rw-r--r--   0        0        0    15155 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/file_utils.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/gui.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/iterables.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/log_utils.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/mpv_utils.py
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/nums.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/objects.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/path_utils.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/pd_utils.py
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/printing.py
--rw-r--r--   0        0        0     7347 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/processes.py
--rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/sql_utils.py
--rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/strings.py
--rw-r--r--   0        0        0    21269 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/web.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 xklb-2.5.9/.gitignore
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 xklb-2.5.9/pyproject.toml
--rw-r--r--   0        0        0   149845 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/README.md
--rw-r--r--   0        0        0   153606 2020-02-02 00:00:00.000000 xklb-2.5.9/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.6.1/.gitattributes
+-rw-r--r--   0        0        0   197009 2020-02-02 00:00:00.000000 xklb-2.6.1/pdm.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.6.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.6.1/.github/LICENSE
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 xklb-2.6.1/.github/Windows.md
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.6.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.6.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.6.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.6.1/.github/examples/extract.svg
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.6.1/.github/examples/tubeadd.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.6.1/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 xklb-2.6.1/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/__init__.py
+-rw-r--r--   0        0        0    18761 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/db_media.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/db_playlists.py
+-rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/dl_extract.py
+-rw-r--r--   0        0        0    15660 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/fs_extract.py
+-rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/gdl_extract.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/history.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/hn_extract.py
+-rw-r--r--   0        0        0    13607 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/lb.py
+-rw-r--r--   0        0        0    18970 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/play_actions.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/post_actions.py
+-rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/readme.py
+-rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/reddit_extract.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/rss_extract.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/search.py
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/site_extract.py
+-rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    20240 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/tube_extract.py
+-rw-r--r--   0        0        0   115868 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/data/__init__.py
+-rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/data/dl_config.py
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/data/wordbank.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/media/__init__.py
+-rw-r--r--   0        0        0     9128 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/media/av.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/media/books.py
+-rw-r--r--   0        0        0    20846 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/media/dedupe.py
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/media/media_check.py
+-rw-r--r--   0        0        0    23467 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/media/media_player.py
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/media/media_printer.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/media/subtitle.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scratch/__init__.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scratch/javguru.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scratch/javtiful.py
+-rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scratch/mam_search.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scratch/mam_slots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/add_row.py
+-rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/big_dirs.py
+-rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/christen.py
+-rw-r--r--   0        0        0    13461 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0    13762 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/dedupe_czkawka.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/disk_usage.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/eda.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/export_text.py
+-rw-r--r--   0        0        0     6810 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/history.py
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/incremental_diff.py
+-rw-r--r--   0        0        0    10660 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/links_db.py
+-rw-r--r--   0        0        0     8184 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/mcda.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/merge_folders.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0     6751 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/open_links.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/places_import.py
+-rw-r--r--   0        0        0     9944 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/process_ffmpeg.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/process_image.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/rel_mv.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/sample_compare.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/sample_hash.py
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/search_db.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/web_add.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/mining/extract_text.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/mining/markdown_links.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/mining/substack.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/scripts/mining/tildes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/__init__.py
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/arg_utils.py
+-rw-r--r--   0        0        0    17266 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/arggroups.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/argparse_utils.py
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/consts.py
+-rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/db_utils.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/devices.py
+-rw-r--r--   0        0        0    15122 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/file_utils.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/gui.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/iterables.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/log_utils.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/mpv_utils.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/nums.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/objects.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/path_utils.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/pd_utils.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/printing.py
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/processes.py
+-rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/sql_utils.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/strings.py
+-rw-r--r--   0        0        0    22041 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/utils/web.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.6.1/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.6.1/.gitignore
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 xklb-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0   156411 2020-02-02 00:00:00.000000 xklb-2.6.1/.github/README.md
+-rw-r--r--   0        0        0   160172 2020-02-02 00:00:00.000000 xklb-2.6.1/PKG-INFO
```

### Comparing `xklb-2.5.9/pdm.lock` & `xklb-2.6.1/pdm.lock`

 * *Files 2% similar despite different names*

```diff
@@ -454,55 +454,55 @@
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "contourpy"
-version = "1.2.0"
+version = "1.2.1"
 requires_python = ">=3.9"
 summary = "Python library for calculating contours of 2D quadrilateral grids"
 dependencies = [
-    "numpy<2.0,>=1.20",
+    "numpy>=1.20",
 ]
 files = [
-    {file = "contourpy-1.2.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:0274c1cb63625972c0c007ab14dd9ba9e199c36ae1a231ce45d725cbcbfd10a8"},
-    {file = "contourpy-1.2.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:ab459a1cbbf18e8698399c595a01f6dcc5c138220ca3ea9e7e6126232d102bb4"},
-    {file = "contourpy-1.2.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6fdd887f17c2f4572ce548461e4f96396681212d858cae7bd52ba3310bc6f00f"},
-    {file = "contourpy-1.2.0-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:5d16edfc3fc09968e09ddffada434b3bf989bf4911535e04eada58469873e28e"},
-    {file = "contourpy-1.2.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:1c203f617abc0dde5792beb586f827021069fb6d403d7f4d5c2b543d87edceb9"},
-    {file = "contourpy-1.2.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b69303ceb2e4d4f146bf82fda78891ef7bcd80c41bf16bfca3d0d7eb545448aa"},
-    {file = "contourpy-1.2.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:884c3f9d42d7218304bc74a8a7693d172685c84bd7ab2bab1ee567b769696df9"},
-    {file = "contourpy-1.2.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:4a1b1208102be6e851f20066bf0e7a96b7d48a07c9b0cfe6d0d4545c2f6cadab"},
-    {file = "contourpy-1.2.0-cp310-cp310-win32.whl", hash = "sha256:34b9071c040d6fe45d9826cbbe3727d20d83f1b6110d219b83eb0e2a01d79488"},
-    {file = "contourpy-1.2.0-cp310-cp310-win_amd64.whl", hash = "sha256:bd2f1ae63998da104f16a8b788f685e55d65760cd1929518fd94cd682bf03e41"},
-    {file = "contourpy-1.2.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:dd10c26b4eadae44783c45ad6655220426f971c61d9b239e6f7b16d5cdaaa727"},
-    {file = "contourpy-1.2.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:5c6b28956b7b232ae801406e529ad7b350d3f09a4fde958dfdf3c0520cdde0dd"},
-    {file = "contourpy-1.2.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ebeac59e9e1eb4b84940d076d9f9a6cec0064e241818bcb6e32124cc5c3e377a"},
-    {file = "contourpy-1.2.0-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:139d8d2e1c1dd52d78682f505e980f592ba53c9f73bd6be102233e358b401063"},
-    {file = "contourpy-1.2.0-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:1e9dc350fb4c58adc64df3e0703ab076f60aac06e67d48b3848c23647ae4310e"},
-    {file = "contourpy-1.2.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:18fc2b4ed8e4a8fe849d18dce4bd3c7ea637758c6343a1f2bae1e9bd4c9f4686"},
-    {file = "contourpy-1.2.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:16a7380e943a6d52472096cb7ad5264ecee36ed60888e2a3d3814991a0107286"},
-    {file = "contourpy-1.2.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:8d8faf05be5ec8e02a4d86f616fc2a0322ff4a4ce26c0f09d9f7fb5330a35c95"},
-    {file = "contourpy-1.2.0-cp311-cp311-win32.whl", hash = "sha256:67b7f17679fa62ec82b7e3e611c43a016b887bd64fb933b3ae8638583006c6d6"},
-    {file = "contourpy-1.2.0-cp311-cp311-win_amd64.whl", hash = "sha256:99ad97258985328b4f207a5e777c1b44a83bfe7cf1f87b99f9c11d4ee477c4de"},
-    {file = "contourpy-1.2.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:575bcaf957a25d1194903a10bc9f316c136c19f24e0985a2b9b5608bdf5dbfe0"},
-    {file = "contourpy-1.2.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:9e6c93b5b2dbcedad20a2f18ec22cae47da0d705d454308063421a3b290d9ea4"},
-    {file = "contourpy-1.2.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:464b423bc2a009088f19bdf1f232299e8b6917963e2b7e1d277da5041f33a779"},
-    {file = "contourpy-1.2.0-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:68ce4788b7d93e47f84edd3f1f95acdcd142ae60bc0e5493bfd120683d2d4316"},
-    {file = "contourpy-1.2.0-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:3d7d1f8871998cdff5d2ff6a087e5e1780139abe2838e85b0b46b7ae6cc25399"},
-    {file = "contourpy-1.2.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6e739530c662a8d6d42c37c2ed52a6f0932c2d4a3e8c1f90692ad0ce1274abe0"},
-    {file = "contourpy-1.2.0-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:247b9d16535acaa766d03037d8e8fb20866d054d3c7fbf6fd1f993f11fc60ca0"},
-    {file = "contourpy-1.2.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:461e3ae84cd90b30f8d533f07d87c00379644205b1d33a5ea03381edc4b69431"},
-    {file = "contourpy-1.2.0-cp312-cp312-win32.whl", hash = "sha256:1c2559d6cffc94890b0529ea7eeecc20d6fadc1539273aa27faf503eb4656d8f"},
-    {file = "contourpy-1.2.0-cp312-cp312-win_amd64.whl", hash = "sha256:491b1917afdd8638a05b611a56d46587d5a632cabead889a5440f7c638bc6ed9"},
-    {file = "contourpy-1.2.0-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:be16975d94c320432657ad2402f6760990cb640c161ae6da1363051805fa8108"},
-    {file = "contourpy-1.2.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b95a225d4948b26a28c08307a60ac00fb8671b14f2047fc5476613252a129776"},
-    {file = "contourpy-1.2.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:0d7e03c0f9a4f90dc18d4e77e9ef4ec7b7bbb437f7f675be8e530d65ae6ef956"},
-    {file = "contourpy-1.2.0.tar.gz", hash = "sha256:171f311cb758de7da13fc53af221ae47a5877be5a0843a9fe150818c51ed276a"},
+    {file = "contourpy-1.2.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:bd7c23df857d488f418439686d3b10ae2fbf9bc256cd045b37a8c16575ea1040"},
+    {file = "contourpy-1.2.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:5b9eb0ca724a241683c9685a484da9d35c872fd42756574a7cfbf58af26677fd"},
+    {file = "contourpy-1.2.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4c75507d0a55378240f781599c30e7776674dbaf883a46d1c90f37e563453480"},
+    {file = "contourpy-1.2.1-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:11959f0ce4a6f7b76ec578576a0b61a28bdc0696194b6347ba3f1c53827178b9"},
+    {file = "contourpy-1.2.1-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:eb3315a8a236ee19b6df481fc5f997436e8ade24a9f03dfdc6bd490fea20c6da"},
+    {file = "contourpy-1.2.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:39f3ecaf76cd98e802f094e0d4fbc6dc9c45a8d0c4d185f0f6c2234e14e5f75b"},
+    {file = "contourpy-1.2.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:94b34f32646ca0414237168d68a9157cb3889f06b096612afdd296003fdd32fd"},
+    {file = "contourpy-1.2.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:457499c79fa84593f22454bbd27670227874cd2ff5d6c84e60575c8b50a69619"},
+    {file = "contourpy-1.2.1-cp310-cp310-win32.whl", hash = "sha256:ac58bdee53cbeba2ecad824fa8159493f0bf3b8ea4e93feb06c9a465d6c87da8"},
+    {file = "contourpy-1.2.1-cp310-cp310-win_amd64.whl", hash = "sha256:9cffe0f850e89d7c0012a1fb8730f75edd4320a0a731ed0c183904fe6ecfc3a9"},
+    {file = "contourpy-1.2.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:6022cecf8f44e36af10bd9118ca71f371078b4c168b6e0fab43d4a889985dbb5"},
+    {file = "contourpy-1.2.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:ef5adb9a3b1d0c645ff694f9bca7702ec2c70f4d734f9922ea34de02294fdf72"},
+    {file = "contourpy-1.2.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6150ffa5c767bc6332df27157d95442c379b7dce3a38dff89c0f39b63275696f"},
+    {file = "contourpy-1.2.1-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:4c863140fafc615c14a4bf4efd0f4425c02230eb8ef02784c9a156461e62c965"},
+    {file = "contourpy-1.2.1-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:00e5388f71c1a0610e6fe56b5c44ab7ba14165cdd6d695429c5cd94021e390b2"},
+    {file = "contourpy-1.2.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d4492d82b3bc7fbb7e3610747b159869468079fe149ec5c4d771fa1f614a14df"},
+    {file = "contourpy-1.2.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:49e70d111fee47284d9dd867c9bb9a7058a3c617274900780c43e38d90fe1205"},
+    {file = "contourpy-1.2.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:b59c0ffceff8d4d3996a45f2bb6f4c207f94684a96bf3d9728dbb77428dd8cb8"},
+    {file = "contourpy-1.2.1-cp311-cp311-win32.whl", hash = "sha256:7b4182299f251060996af5249c286bae9361fa8c6a9cda5efc29fe8bfd6062ec"},
+    {file = "contourpy-1.2.1-cp311-cp311-win_amd64.whl", hash = "sha256:2855c8b0b55958265e8b5888d6a615ba02883b225f2227461aa9127c578a4922"},
+    {file = "contourpy-1.2.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:62828cada4a2b850dbef89c81f5a33741898b305db244904de418cc957ff05dc"},
+    {file = "contourpy-1.2.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:309be79c0a354afff9ff7da4aaed7c3257e77edf6c1b448a779329431ee79d7e"},
+    {file = "contourpy-1.2.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2e785e0f2ef0d567099b9ff92cbfb958d71c2d5b9259981cd9bee81bd194c9a4"},
+    {file = "contourpy-1.2.1-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:1cac0a8f71a041aa587410424ad46dfa6a11f6149ceb219ce7dd48f6b02b87a7"},
+    {file = "contourpy-1.2.1-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:af3f4485884750dddd9c25cb7e3915d83c2db92488b38ccb77dd594eac84c4a0"},
+    {file = "contourpy-1.2.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9ce6889abac9a42afd07a562c2d6d4b2b7134f83f18571d859b25624a331c90b"},
+    {file = "contourpy-1.2.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:a1eea9aecf761c661d096d39ed9026574de8adb2ae1c5bd7b33558af884fb2ce"},
+    {file = "contourpy-1.2.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:187fa1d4c6acc06adb0fae5544c59898ad781409e61a926ac7e84b8f276dcef4"},
+    {file = "contourpy-1.2.1-cp312-cp312-win32.whl", hash = "sha256:c2528d60e398c7c4c799d56f907664673a807635b857df18f7ae64d3e6ce2d9f"},
+    {file = "contourpy-1.2.1-cp312-cp312-win_amd64.whl", hash = "sha256:1a07fc092a4088ee952ddae19a2b2a85757b923217b7eed584fdf25f53a6e7ce"},
+    {file = "contourpy-1.2.1-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:a31f94983fecbac95e58388210427d68cd30fe8a36927980fab9c20062645609"},
+    {file = "contourpy-1.2.1-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ef2b055471c0eb466033760a521efb9d8a32b99ab907fc8358481a1dd29e3bd3"},
+    {file = "contourpy-1.2.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:b33d2bc4f69caedcd0a275329eb2198f560b325605810895627be5d4b876bf7f"},
+    {file = "contourpy-1.2.1.tar.gz", hash = "sha256:4d8908b3bee1c889e547867ca4cdc54e5ab6be6d3e078556814a22457f49423c"},
 ]
 
 [[package]]
 name = "cryptography"
 version = "42.0.5"
 requires_python = ">=3.7"
 summary = "cryptography is a package which provides cryptographic recipes and primitives to Python developers."
@@ -552,44 +552,44 @@
 files = [
     {file = "cycler-0.12.1-py3-none-any.whl", hash = "sha256:85cef7cff222d8644161529808465972e51340599459b8ac3ccbac5a854e0d30"},
     {file = "cycler-0.12.1.tar.gz", hash = "sha256:88bb128f02ba341da8ef447245a9e138fae777f6a23943da4540077d3601eb1c"},
 ]
 
 [[package]]
 name = "cython"
-version = "3.0.8"
-requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
+version = "3.0.10"
+requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,>=2.7"
 summary = "The Cython compiler for writing C extensions in the Python language."
 files = [
-    {file = "Cython-3.0.8-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:a846e0a38e2b24e9a5c5dc74b0e54c6e29420d88d1dafabc99e0fc0f3e338636"},
-    {file = "Cython-3.0.8-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:45523fdc2b78d79b32834cc1cc12dc2ca8967af87e22a3ee1bff20e77c7f5520"},
-    {file = "Cython-3.0.8-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:baa0b7f3f841fe087410cab66778e2d3fb20ae2d2078a2be3dffe66c6574be39"},
-    {file = "Cython-3.0.8-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e87294e33e40c289c77a135f491cd721bd089f193f956f7b8ed5aa2d0b8c558f"},
-    {file = "Cython-3.0.8-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:a1df7a129344b1215c20096d33c00193437df1a8fcca25b71f17c23b1a44f782"},
-    {file = "Cython-3.0.8-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:13c2a5e57a0358da467d97667297bf820b62a1a87ae47c5f87938b9bb593acbd"},
-    {file = "Cython-3.0.8-cp310-cp310-win32.whl", hash = "sha256:96b028f044f5880e3cb18ecdcfc6c8d3ce9d0af28418d5ab464509f26d8adf12"},
-    {file = "Cython-3.0.8-cp310-cp310-win_amd64.whl", hash = "sha256:8140597a8b5cc4f119a1190f5a2228a84f5ca6d8d9ec386cfce24663f48b2539"},
-    {file = "Cython-3.0.8-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aae26f9663e50caf9657148403d9874eea41770ecdd6caf381d177c2b1bb82ba"},
-    {file = "Cython-3.0.8-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:547eb3cdb2f8c6f48e6865d5a741d9dd051c25b3ce076fbca571727977b28ac3"},
-    {file = "Cython-3.0.8-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5a567d4b9ba70b26db89d75b243529de9e649a2f56384287533cf91512705bee"},
-    {file = "Cython-3.0.8-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:51d1426263b0e82fb22bda8ea60dc77a428581cc19e97741011b938445d383f1"},
-    {file = "Cython-3.0.8-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:c26daaeccda072459b48d211415fd1e5507c06bcd976fa0d5b8b9f1063467d7b"},
-    {file = "Cython-3.0.8-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:289ce7838208211cd166e975865fd73b0649bf118170b6cebaedfbdaf4a37795"},
-    {file = "Cython-3.0.8-cp311-cp311-win32.whl", hash = "sha256:c8aa05f5e17f8042a3be052c24f2edc013fb8af874b0bf76907d16c51b4e7871"},
-    {file = "Cython-3.0.8-cp311-cp311-win_amd64.whl", hash = "sha256:000dc9e135d0eec6ecb2b40a5b02d0868a2f8d2e027a41b0fe16a908a9e6de02"},
-    {file = "Cython-3.0.8-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:90d3fe31db55685d8cb97d43b0ec39ef614fcf660f83c77ed06aa670cb0e164f"},
-    {file = "Cython-3.0.8-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e24791ddae2324e88e3c902a765595c738f19ae34ee66bfb1a6dac54b1833419"},
-    {file = "Cython-3.0.8-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2f020fa1c0552052e0660790b8153b79e3fc9a15dbd8f1d0b841fe5d204a6ae6"},
-    {file = "Cython-3.0.8-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:18bfa387d7a7f77d7b2526af69a65dbd0b731b8d941aaff5becff8e21f6d7717"},
-    {file = "Cython-3.0.8-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:fe81b339cffd87c0069c6049b4d33e28bdd1874625ee515785bf42c9fdff3658"},
-    {file = "Cython-3.0.8-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:80fd94c076e1e1b1ee40a309be03080b75f413e8997cddcf401a118879863388"},
-    {file = "Cython-3.0.8-cp312-cp312-win32.whl", hash = "sha256:85077915a93e359a9b920280d214dc0cf8a62773e1f3d7d30fab8ea4daed670c"},
-    {file = "Cython-3.0.8-cp312-cp312-win_amd64.whl", hash = "sha256:0cb2dcc565c7851f75d496f724a384a790fab12d1b82461b663e66605bec429a"},
-    {file = "Cython-3.0.8-py2.py3-none-any.whl", hash = "sha256:171b27051253d3f9108e9759e504ba59ff06e7f7ba944457f94deaf9c21bf0b6"},
-    {file = "Cython-3.0.8.tar.gz", hash = "sha256:8333423d8fd5765e7cceea3a9985dd1e0a5dfeb2734629e1a2ed2d6233d39de6"},
+    {file = "Cython-3.0.10-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e876272548d73583e90babda94c1299537006cad7a34e515a06c51b41f8657aa"},
+    {file = "Cython-3.0.10-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:adc377aa33c3309191e617bf675fdbb51ca727acb9dc1aa23fc698d8121f7e23"},
+    {file = "Cython-3.0.10-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:401aba1869a57aba2922ccb656a6320447e55ace42709b504c2f8e8b166f46e1"},
+    {file = "Cython-3.0.10-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:541fbe725d6534a90b93f8c577eb70924d664b227a4631b90a6e0506d1469591"},
+    {file = "Cython-3.0.10-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:86998b01f6a6d48398df8467292c7637e57f7e3a2ca68655367f13f66fed7734"},
+    {file = "Cython-3.0.10-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:d092c0ddba7e9e530a5c5be4ac06db8360258acc27675d1fc86294a5dc8994c5"},
+    {file = "Cython-3.0.10-cp310-cp310-win32.whl", hash = "sha256:3cffb666e649dba23810732497442fb339ee67ba4e0be1f0579991e83fcc2436"},
+    {file = "Cython-3.0.10-cp310-cp310-win_amd64.whl", hash = "sha256:9ea31184c7b3a728ef1f81fccb161d8948c05aa86c79f63b74fb6f3ddec860ec"},
+    {file = "Cython-3.0.10-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:051069638abfb076900b0c2bcb6facf545655b3f429e80dd14365192074af5a4"},
+    {file = "Cython-3.0.10-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:712760879600907189c7d0d346851525545484e13cd8b787e94bfd293da8ccf0"},
+    {file = "Cython-3.0.10-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:38d40fa1324ac47c04483d151f5e092406a147eac88a18aec789cf01c089c3f2"},
+    {file = "Cython-3.0.10-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5bd49a3a9fdff65446a3e1c2bfc0ec85c6ce4c3cad27cd4ad7ba150a62b7fb59"},
+    {file = "Cython-3.0.10-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:e8df79b596633b8295eaa48b1157d796775c2bb078f32267d32f3001b687f2fd"},
+    {file = "Cython-3.0.10-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:bcc9795990e525c192bc5c0775e441d7d56d7a7d02210451e9e13c0448dba51b"},
+    {file = "Cython-3.0.10-cp311-cp311-win32.whl", hash = "sha256:09f2000041db482cad3bfce94e1fa3a4c82b0e57390a164c02566cbbda8c4f12"},
+    {file = "Cython-3.0.10-cp311-cp311-win_amd64.whl", hash = "sha256:3919a55ec9b6c7db6f68a004c21c05ed540c40dbe459ced5d801d5a1f326a053"},
+    {file = "Cython-3.0.10-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:8f2864ab5fcd27a346f0b50f901ebeb8f60b25a60a575ccfd982e7f3e9674914"},
+    {file = "Cython-3.0.10-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:407840c56385b9c085826fe300213e0e76ba15d1d47daf4b58569078ecb94446"},
+    {file = "Cython-3.0.10-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5a036d00caa73550a3a976432ef21c1e3fa12637e1616aab32caded35331ae96"},
+    {file = "Cython-3.0.10-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9cc6a0e7e23a96dec3f3c9d39690d4281beabd5297855140d0d30855f950275e"},
+    {file = "Cython-3.0.10-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:a5e14a8c6a8157d2b0cdc2e8e3444905d20a0e78e19d2a097e89fb8b04b51f6b"},
+    {file = "Cython-3.0.10-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:f8a2b8fa0fd8358bccb5f3304be563c4750aae175100463d212d5ea0ec74cbe0"},
+    {file = "Cython-3.0.10-cp312-cp312-win32.whl", hash = "sha256:2d29e617fd23cf4b83afe8f93f2966566c9f565918ad1e86a4502fe825cc0a79"},
+    {file = "Cython-3.0.10-cp312-cp312-win_amd64.whl", hash = "sha256:6c5af936940a38c300977b81598d9c0901158f220a58c177820e17e1774f1cf1"},
+    {file = "Cython-3.0.10-py2.py3-none-any.whl", hash = "sha256:fcbb679c0b43514d591577fd0d20021c55c240ca9ccafbdb82d3fb95e5edfee2"},
+    {file = "Cython-3.0.10.tar.gz", hash = "sha256:dcc96739331fb854dcf503f94607576cfe8488066c61ca50dfd55836f132de99"},
 ]
 
 [[package]]
 name = "decorator"
 version = "5.1.1"
 requires_python = ">=3.5"
 summary = "Decorators for Humans"
@@ -664,74 +664,73 @@
 files = [
     {file = "ffmpeg-python-0.2.0.tar.gz", hash = "sha256:65225db34627c578ef0e11c8b1eb528bb35e024752f6f10b78c011f6f64c4127"},
     {file = "ffmpeg_python-0.2.0-py3-none-any.whl", hash = "sha256:ac441a0404e053f8b6a1113a77c0f452f1cfc62f6344a769475ffdc0f56c23c5"},
 ]
 
 [[package]]
 name = "fiona"
-version = "1.9.5"
+version = "1.9.6"
 requires_python = ">=3.7"
 summary = "Fiona reads and writes spatial data files"
 dependencies = [
     "attrs>=19.2.0",
     "certifi",
     "click-plugins>=1.0",
     "click~=8.0",
     "cligj>=0.5",
-    "setuptools",
     "six",
 ]
 files = [
-    {file = "fiona-1.9.5-cp310-cp310-macosx_10_15_x86_64.whl", hash = "sha256:5f40a40529ecfca5294260316cf987a0420c77a2f0cf0849f529d1afbccd093e"},
-    {file = "fiona-1.9.5-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:374efe749143ecb5cfdd79b585d83917d2bf8ecfbfc6953c819586b336ce9c63"},
-    {file = "fiona-1.9.5-cp310-cp310-manylinux2014_x86_64.whl", hash = "sha256:35dae4b0308eb44617cdc4461ceb91f891d944fdebbcba5479efe524ec5db8de"},
-    {file = "fiona-1.9.5-cp310-cp310-win_amd64.whl", hash = "sha256:5b4c6a3df53bee8f85bb46685562b21b43346be1fe96419f18f70fa1ab8c561c"},
-    {file = "fiona-1.9.5-cp311-cp311-macosx_10_15_x86_64.whl", hash = "sha256:6ad04c1877b9fd742871b11965606c6a52f40706f56a48d66a87cc3073943828"},
-    {file = "fiona-1.9.5-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:9fb9a24a8046c724787719e20557141b33049466145fc3e665764ac7caf5748c"},
-    {file = "fiona-1.9.5-cp311-cp311-manylinux2014_x86_64.whl", hash = "sha256:d722d7f01a66f4ab6cd08d156df3fdb92f0669cf5f8708ddcb209352f416f241"},
-    {file = "fiona-1.9.5-cp311-cp311-win_amd64.whl", hash = "sha256:7ede8ddc798f3d447536080c6db9a5fb73733ad8bdb190cb65eed4e289dd4c50"},
-    {file = "fiona-1.9.5-cp312-cp312-macosx_10_15_x86_64.whl", hash = "sha256:8b098054a27c12afac4f819f98cb4d4bf2db9853f70b0c588d7d97d26e128c39"},
-    {file = "fiona-1.9.5-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:6d9f29e9bcbb33232ff7fa98b4a3c2234db910c1dc6c4147fc36c0b8b930f2e0"},
-    {file = "fiona-1.9.5-cp312-cp312-manylinux2014_x86_64.whl", hash = "sha256:f1af08da4ecea5036cb81c9131946be4404245d1b434b5b24fd3871a1d4030d9"},
-    {file = "fiona-1.9.5-cp312-cp312-win_amd64.whl", hash = "sha256:c521e1135c78dec0d7774303e5a1b4c62e0efb0e602bb8f167550ef95e0a2691"},
-    {file = "fiona-1.9.5.tar.gz", hash = "sha256:99e2604332caa7692855c2ae6ed91e1fffdf9b59449aa8032dd18e070e59a2f7"},
+    {file = "fiona-1.9.6-cp310-cp310-macosx_10_15_x86_64.whl", hash = "sha256:63e528b5ea3d8b1038d788e7c65117835c787ba7fdc94b1b42f09c2cbc0aaff2"},
+    {file = "fiona-1.9.6-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:918bd27d8625416672e834593970f96dff63215108f81efb876fe5c0bc58a3b4"},
+    {file = "fiona-1.9.6-cp310-cp310-manylinux2014_x86_64.whl", hash = "sha256:e313210b30d09ed8f829bf625599e248dadd78622728030221f6526580ff26c5"},
+    {file = "fiona-1.9.6-cp310-cp310-win_amd64.whl", hash = "sha256:89095c2d542325ee45894b8837e8048cdbb2f22274934e1be3b673ca628010d7"},
+    {file = "fiona-1.9.6-cp311-cp311-macosx_10_15_x86_64.whl", hash = "sha256:98cea6f435843b2119731c6b0470e5b7386aa16b6aa7edabbf1ed93aefe029c3"},
+    {file = "fiona-1.9.6-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:f4230eccbd896a79d1ebfa551d84bf90f512f7bcbe1ca61e3f82231321f1a532"},
+    {file = "fiona-1.9.6-cp311-cp311-manylinux2014_x86_64.whl", hash = "sha256:48b6218224e96de5e36b5eb259f37160092260e5de0dcd82ca200b1887aa9884"},
+    {file = "fiona-1.9.6-cp311-cp311-win_amd64.whl", hash = "sha256:c1dd5fbc29b7303bb87eb683455e8451e1a53bb8faf20ef97fdcd843c9e4a7f6"},
+    {file = "fiona-1.9.6-cp312-cp312-macosx_10_15_x86_64.whl", hash = "sha256:42d8a0e5570948d3821c493b6141866d9a4d7a64edad2be4ecbb89f81904baac"},
+    {file = "fiona-1.9.6-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:39819fb8f5ec6d9971cb01b912b4431615a3d3f50c83798565d8ce41917930db"},
+    {file = "fiona-1.9.6-cp312-cp312-manylinux2014_x86_64.whl", hash = "sha256:9b53034efdf93ada9295b081e6a8280af7c75496a20df82d4c2ca46d65b85905"},
+    {file = "fiona-1.9.6-cp312-cp312-win_amd64.whl", hash = "sha256:1dcd6eca7524535baf2a39d7981b4a46d33ae28c313934a7c3eae62eecf9dfa5"},
+    {file = "fiona-1.9.6.tar.gz", hash = "sha256:791b3494f8b218c06ea56f892bd6ba893dfa23525347761d066fb7738acda3b1"},
 ]
 
 [[package]]
 name = "fonttools"
-version = "4.49.0"
+version = "4.51.0"
 requires_python = ">=3.8"
 summary = "Tools to manipulate font files"
 files = [
-    {file = "fonttools-4.49.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:d970ecca0aac90d399e458f0b7a8a597e08f95de021f17785fb68e2dc0b99717"},
-    {file = "fonttools-4.49.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:ac9a745b7609f489faa65e1dc842168c18530874a5f5b742ac3dd79e26bca8bc"},
-    {file = "fonttools-4.49.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0ba0e00620ca28d4ca11fc700806fd69144b463aa3275e1b36e56c7c09915559"},
-    {file = "fonttools-4.49.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:cdee3ab220283057e7840d5fb768ad4c2ebe65bdba6f75d5d7bf47f4e0ed7d29"},
-    {file = "fonttools-4.49.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:ce7033cb61f2bb65d8849658d3786188afd80f53dad8366a7232654804529532"},
-    {file = "fonttools-4.49.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:07bc5ea02bb7bc3aa40a1eb0481ce20e8d9b9642a9536cde0218290dd6085828"},
-    {file = "fonttools-4.49.0-cp310-cp310-win32.whl", hash = "sha256:86eef6aab7fd7c6c8545f3ebd00fd1d6729ca1f63b0cb4d621bccb7d1d1c852b"},
-    {file = "fonttools-4.49.0-cp310-cp310-win_amd64.whl", hash = "sha256:1fac1b7eebfce75ea663e860e7c5b4a8831b858c17acd68263bc156125201abf"},
-    {file = "fonttools-4.49.0-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:edc0cce355984bb3c1d1e89d6a661934d39586bb32191ebff98c600f8957c63e"},
-    {file = "fonttools-4.49.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:83a0d9336de2cba86d886507dd6e0153df333ac787377325a39a2797ec529814"},
-    {file = "fonttools-4.49.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:36c8865bdb5cfeec88f5028e7e592370a0657b676c6f1d84a2108e0564f90e22"},
-    {file = "fonttools-4.49.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:33037d9e56e2562c710c8954d0f20d25b8386b397250d65581e544edc9d6b942"},
-    {file = "fonttools-4.49.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:8fb022d799b96df3eaa27263e9eea306bd3d437cc9aa981820850281a02b6c9a"},
-    {file = "fonttools-4.49.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:33c584c0ef7dc54f5dd4f84082eabd8d09d1871a3d8ca2986b0c0c98165f8e86"},
-    {file = "fonttools-4.49.0-cp311-cp311-win32.whl", hash = "sha256:cbe61b158deb09cffdd8540dc4a948d6e8f4d5b4f3bf5cd7db09bd6a61fee64e"},
-    {file = "fonttools-4.49.0-cp311-cp311-win_amd64.whl", hash = "sha256:fc11e5114f3f978d0cea7e9853627935b30d451742eeb4239a81a677bdee6bf6"},
-    {file = "fonttools-4.49.0-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:d647a0e697e5daa98c87993726da8281c7233d9d4ffe410812a4896c7c57c075"},
-    {file = "fonttools-4.49.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:f3bbe672df03563d1f3a691ae531f2e31f84061724c319652039e5a70927167e"},
-    {file = "fonttools-4.49.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:bebd91041dda0d511b0d303180ed36e31f4f54b106b1259b69fade68413aa7ff"},
-    {file = "fonttools-4.49.0-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4145f91531fd43c50f9eb893faa08399816bb0b13c425667c48475c9f3a2b9b5"},
-    {file = "fonttools-4.49.0-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:ea329dafb9670ffbdf4dbc3b0e5c264104abcd8441d56de77f06967f032943cb"},
-    {file = "fonttools-4.49.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:c076a9e548521ecc13d944b1d261ff3d7825048c338722a4bd126d22316087b7"},
-    {file = "fonttools-4.49.0-cp312-cp312-win32.whl", hash = "sha256:b607ea1e96768d13be26d2b400d10d3ebd1456343eb5eaddd2f47d1c4bd00880"},
-    {file = "fonttools-4.49.0-cp312-cp312-win_amd64.whl", hash = "sha256:a974c49a981e187381b9cc2c07c6b902d0079b88ff01aed34695ec5360767034"},
-    {file = "fonttools-4.49.0-py3-none-any.whl", hash = "sha256:af281525e5dd7fa0b39fb1667b8d5ca0e2a9079967e14c4bfe90fd1cd13e0f18"},
-    {file = "fonttools-4.49.0.tar.gz", hash = "sha256:ebf46e7f01b7af7861310417d7c49591a85d99146fc23a5ba82fdb28af156321"},
+    {file = "fonttools-4.51.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:84d7751f4468dd8cdd03ddada18b8b0857a5beec80bce9f435742abc9a851a74"},
+    {file = "fonttools-4.51.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:8b4850fa2ef2cfbc1d1f689bc159ef0f45d8d83298c1425838095bf53ef46308"},
+    {file = "fonttools-4.51.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b5b48a1121117047d82695d276c2af2ee3a24ffe0f502ed581acc2673ecf1037"},
+    {file = "fonttools-4.51.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:180194c7fe60c989bb627d7ed5011f2bef1c4d36ecf3ec64daec8302f1ae0716"},
+    {file = "fonttools-4.51.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:96a48e137c36be55e68845fc4284533bda2980f8d6f835e26bca79d7e2006438"},
+    {file = "fonttools-4.51.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:806e7912c32a657fa39d2d6eb1d3012d35f841387c8fc6cf349ed70b7c340039"},
+    {file = "fonttools-4.51.0-cp310-cp310-win32.whl", hash = "sha256:32b17504696f605e9e960647c5f64b35704782a502cc26a37b800b4d69ff3c77"},
+    {file = "fonttools-4.51.0-cp310-cp310-win_amd64.whl", hash = "sha256:c7e91abdfae1b5c9e3a543f48ce96013f9a08c6c9668f1e6be0beabf0a569c1b"},
+    {file = "fonttools-4.51.0-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:a8feca65bab31479d795b0d16c9a9852902e3a3c0630678efb0b2b7941ea9c74"},
+    {file = "fonttools-4.51.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:8ac27f436e8af7779f0bb4d5425aa3535270494d3bc5459ed27de3f03151e4c2"},
+    {file = "fonttools-4.51.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0e19bd9e9964a09cd2433a4b100ca7f34e34731e0758e13ba9a1ed6e5468cc0f"},
+    {file = "fonttools-4.51.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b2b92381f37b39ba2fc98c3a45a9d6383bfc9916a87d66ccb6553f7bdd129097"},
+    {file = "fonttools-4.51.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:5f6bc991d1610f5c3bbe997b0233cbc234b8e82fa99fc0b2932dc1ca5e5afec0"},
+    {file = "fonttools-4.51.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:9696fe9f3f0c32e9a321d5268208a7cc9205a52f99b89479d1b035ed54c923f1"},
+    {file = "fonttools-4.51.0-cp311-cp311-win32.whl", hash = "sha256:3bee3f3bd9fa1d5ee616ccfd13b27ca605c2b4270e45715bd2883e9504735034"},
+    {file = "fonttools-4.51.0-cp311-cp311-win_amd64.whl", hash = "sha256:0f08c901d3866a8905363619e3741c33f0a83a680d92a9f0e575985c2634fcc1"},
+    {file = "fonttools-4.51.0-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:4060acc2bfa2d8e98117828a238889f13b6f69d59f4f2d5857eece5277b829ba"},
+    {file = "fonttools-4.51.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:1250e818b5f8a679ad79660855528120a8f0288f8f30ec88b83db51515411fcc"},
+    {file = "fonttools-4.51.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:76f1777d8b3386479ffb4a282e74318e730014d86ce60f016908d9801af9ca2a"},
+    {file = "fonttools-4.51.0-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8b5ad456813d93b9c4b7ee55302208db2b45324315129d85275c01f5cb7e61a2"},
+    {file = "fonttools-4.51.0-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:68b3fb7775a923be73e739f92f7e8a72725fd333eab24834041365d2278c3671"},
+    {file = "fonttools-4.51.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:8e2f1a4499e3b5ee82c19b5ee57f0294673125c65b0a1ff3764ea1f9db2f9ef5"},
+    {file = "fonttools-4.51.0-cp312-cp312-win32.whl", hash = "sha256:278e50f6b003c6aed19bae2242b364e575bcb16304b53f2b64f6551b9c000e15"},
+    {file = "fonttools-4.51.0-cp312-cp312-win_amd64.whl", hash = "sha256:b3c61423f22165541b9403ee39874dcae84cd57a9078b82e1dce8cb06b07fa2e"},
+    {file = "fonttools-4.51.0-py3-none-any.whl", hash = "sha256:15c94eeef6b095831067f72c825eb0e2d48bb4cea0647c1b05c981ecba2bf39f"},
+    {file = "fonttools-4.51.0.tar.gz", hash = "sha256:dc0673361331566d7a663d7ce0f6fdcbfbdc1f59c6e3ed1165ad7202ca183c68"},
 ]
 
 [[package]]
 name = "freezegun"
 version = "1.4.0"
 requires_python = ">=3.7"
 summary = "Let your Python tests travel through time"
@@ -796,46 +795,46 @@
     {file = "frozenlist-1.4.1-cp312-cp312-win_amd64.whl", hash = "sha256:64536573d0a2cb6e625cf309984e2d873979709f2cf22839bf2d61790b448ad5"},
     {file = "frozenlist-1.4.1-py3-none-any.whl", hash = "sha256:04ced3e6a46b4cfffe20f9ae482818e34eba9b5fb0ce4056e4cc9b6e212d09b7"},
     {file = "frozenlist-1.4.1.tar.gz", hash = "sha256:c037a86e8513059a2613aaba4d817bb90b9d9b6b69aace3ce9c877e8c8ed402b"},
 ]
 
 [[package]]
 name = "ftfy"
-version = "6.1.3"
+version = "6.2.0"
 requires_python = ">=3.8,<4"
 summary = "Fixes mojibake and other problems with Unicode, after the fact"
 dependencies = [
     "wcwidth<0.3.0,>=0.2.12",
 ]
 files = [
-    {file = "ftfy-6.1.3-py3-none-any.whl", hash = "sha256:e49c306c06a97f4986faa7a8740cfe3c13f3106e85bcec73eb629817e671557c"},
-    {file = "ftfy-6.1.3.tar.gz", hash = "sha256:693274aead811cff24c1e8784165aa755cd2f6e442a5ec535c7d697f6422a422"},
+    {file = "ftfy-6.2.0-py3-none-any.whl", hash = "sha256:f94a2c34b76e07475720e3096f5ca80911d152406fbde66fdb45c4d0c9150026"},
+    {file = "ftfy-6.2.0.tar.gz", hash = "sha256:5e42143c7025ef97944ca2619d6b61b0619fc6654f98771d39e862c1424c75c0"},
 ]
 
 [[package]]
 name = "future"
 version = "1.0.0"
 requires_python = ">=2.6, !=3.0.*, !=3.1.*, !=3.2.*"
 summary = "Clean single-source support for Python 3 and 2"
 files = [
     {file = "future-1.0.0-py3-none-any.whl", hash = "sha256:929292d34f5872e70396626ef385ec22355a1fae8ad29e1a734c3e43f9fbc216"},
     {file = "future-1.0.0.tar.gz", hash = "sha256:bd2968309307861edae1458a4f8a4f3598c03be43b97521076aebf5d94c07b05"},
 ]
 
 [[package]]
 name = "gallery-dl"
-version = "1.26.8"
+version = "1.26.9"
 requires_python = ">=3.4"
 summary = "Command-line program to download image galleries and collections from several image hosting sites"
 dependencies = [
     "requests>=2.11.0",
 ]
 files = [
-    {file = "gallery_dl-1.26.8-py3-none-any.whl", hash = "sha256:14d0da8b97b8c6d11ad89f4cf3c5f3167f7c86eee46fc9b4b63a2cd88be4dfa3"},
-    {file = "gallery_dl-1.26.8.tar.gz", hash = "sha256:b5f3662a058aaf64c640d82f0bfaa8dbe0ef8a3e0b50bd19cbbee67d371c8b69"},
+    {file = "gallery_dl-1.26.9-py3-none-any.whl", hash = "sha256:cbfce457778a5339e888bca78d339b119318252f0feead6a4cd9b93884738008"},
+    {file = "gallery_dl-1.26.9.tar.gz", hash = "sha256:3e06dfa69c890a9805ba90509e0f0c50f8a16c39a2b780bec569d2cc2272bb99"},
 ]
 
 [[package]]
 name = "geopandas"
 version = "0.14.3"
 requires_python = ">=3.9"
 summary = "Geographic pandas extensions"
@@ -946,32 +945,33 @@
 files = [
     {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
     {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
 ]
 
 [[package]]
 name = "ipython"
-version = "8.22.1"
+version = "8.23.0"
 requires_python = ">=3.10"
 summary = "IPython: Productive Interactive Computing"
 dependencies = [
     "colorama; sys_platform == \"win32\"",
     "decorator",
     "exceptiongroup; python_version < \"3.11\"",
     "jedi>=0.16",
     "matplotlib-inline",
     "pexpect>4.3; sys_platform != \"win32\" and sys_platform != \"emscripten\"",
     "prompt-toolkit<3.1.0,>=3.0.41",
     "pygments>=2.4.0",
     "stack-data",
     "traitlets>=5.13.0",
+    "typing-extensions; python_version < \"3.12\"",
 ]
 files = [
-    {file = "ipython-8.22.1-py3-none-any.whl", hash = "sha256:869335e8cded62ffb6fac8928e5287a05433d6462e3ebaac25f4216474dd6bc4"},
-    {file = "ipython-8.22.1.tar.gz", hash = "sha256:39c6f9efc079fb19bfb0f17eee903978fe9a290b1b82d68196c641cecb76ea22"},
+    {file = "ipython-8.23.0-py3-none-any.whl", hash = "sha256:07232af52a5ba146dc3372c7bf52a0f890a23edf38d77caef8d53f9cdc2584c1"},
+    {file = "ipython-8.23.0.tar.gz", hash = "sha256:7468edaf4f6de3e1b912e57f66c241e6fd3c7099f2ec2136e239e142e800274d"},
 ]
 
 [[package]]
 name = "jedi"
 version = "0.19.1"
 requires_python = ">=3.6"
 summary = "An autocompletion tool for Python that can be used for text editors."
@@ -981,20 +981,20 @@
 files = [
     {file = "jedi-0.19.1-py2.py3-none-any.whl", hash = "sha256:e983c654fe5c02867aef4cdfce5a2fbb4a50adc0af145f70504238f18ef5e7e0"},
     {file = "jedi-0.19.1.tar.gz", hash = "sha256:cf0496f3651bc65d7174ac1b7d043eff454892c708a87d1b683e57b569927ffd"},
 ]
 
 [[package]]
 name = "joblib"
-version = "1.3.2"
-requires_python = ">=3.7"
+version = "1.4.0"
+requires_python = ">=3.8"
 summary = "Lightweight pipelining with Python functions"
 files = [
-    {file = "joblib-1.3.2-py3-none-any.whl", hash = "sha256:ef4331c65f239985f3f2220ecc87db222f08fd22097a3dd5698f693875f8cbb9"},
-    {file = "joblib-1.3.2.tar.gz", hash = "sha256:92f865e621e17784e7955080b6d042489e3b8e294949cc44c6eac304f59772b1"},
+    {file = "joblib-1.4.0-py3-none-any.whl", hash = "sha256:42942470d4062537be4d54c83511186da1fc14ba354961a2114da91efa9a4ed7"},
+    {file = "joblib-1.4.0.tar.gz", hash = "sha256:1eb0dc091919cd384490de890cb5dfd538410a6d4b3b54eef09fb8c50b409b1c"},
 ]
 
 [[package]]
 name = "kaitaistruct"
 version = "0.10"
 requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,>=2.7"
 summary = "Kaitai Struct declarative parser generator for binary data: runtime library for Python"
@@ -1070,20 +1070,20 @@
     {file = "kiwisolver-1.4.5-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:210ef2c3a1f03272649aff1ef992df2e724748918c4bc2d5a90352849eb40bea"},
     {file = "kiwisolver-1.4.5-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:11d011a7574eb3b82bcc9c1a1d35c1d7075677fdd15de527d91b46bd35e935ee"},
     {file = "kiwisolver-1.4.5.tar.gz", hash = "sha256:e57e563a57fb22a142da34f38acc2fc1a5c864bc29ca1517a88abc963e60d6ec"},
 ]
 
 [[package]]
 name = "markdown"
-version = "3.5.2"
+version = "3.6"
 requires_python = ">=3.8"
 summary = "Python implementation of John Gruber's Markdown."
 files = [
-    {file = "Markdown-3.5.2-py3-none-any.whl", hash = "sha256:d43323865d89fc0cb9b20c75fc8ad313af307cc087e84b657d9eec768eddeadd"},
-    {file = "Markdown-3.5.2.tar.gz", hash = "sha256:e1ac7b3dc550ee80e602e71c1d168002f062e49f1b11e26a36264dafd4df2ef8"},
+    {file = "Markdown-3.6-py3-none-any.whl", hash = "sha256:48f276f4d8cfb8ce6527c8f79e2ee29708508bf4d40aa410fbc3b4ee832c850f"},
+    {file = "Markdown-3.6.tar.gz", hash = "sha256:ed4f41f6daecbeeb96e576ce414c41d2d876daa9a16cb35fa8ed8c2ddfad0224"},
 ]
 
 [[package]]
 name = "markdown-it-py"
 version = "3.0.0"
 requires_python = ">=3.8"
 summary = "Python port of markdown-it. Markdown parsing, done right!"
@@ -1093,51 +1093,51 @@
 files = [
     {file = "markdown-it-py-3.0.0.tar.gz", hash = "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"},
     {file = "markdown_it_py-3.0.0-py3-none-any.whl", hash = "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1"},
 ]
 
 [[package]]
 name = "matplotlib"
-version = "3.8.3"
+version = "3.8.4"
 requires_python = ">=3.9"
 summary = "Python plotting package"
 dependencies = [
     "contourpy>=1.0.1",
     "cycler>=0.10",
     "fonttools>=4.22.0",
     "kiwisolver>=1.3.1",
-    "numpy<2,>=1.21",
+    "numpy>=1.21",
     "packaging>=20.0",
     "pillow>=8",
     "pyparsing>=2.3.1",
     "python-dateutil>=2.7",
 ]
 files = [
-    {file = "matplotlib-3.8.3-cp310-cp310-macosx_10_12_x86_64.whl", hash = "sha256:cf60138ccc8004f117ab2a2bad513cc4d122e55864b4fe7adf4db20ca68a078f"},
-    {file = "matplotlib-3.8.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:5f557156f7116be3340cdeef7f128fa99b0d5d287d5f41a16e169819dcf22357"},
-    {file = "matplotlib-3.8.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f386cf162b059809ecfac3bcc491a9ea17da69fa35c8ded8ad154cd4b933d5ec"},
-    {file = "matplotlib-3.8.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b3c5f96f57b0369c288bf6f9b5274ba45787f7e0589a34d24bdbaf6d3344632f"},
-    {file = "matplotlib-3.8.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:83e0f72e2c116ca7e571c57aa29b0fe697d4c6425c4e87c6e994159e0c008635"},
-    {file = "matplotlib-3.8.3-cp310-cp310-win_amd64.whl", hash = "sha256:1c5c8290074ba31a41db1dc332dc2b62def469ff33766cbe325d32a3ee291aea"},
-    {file = "matplotlib-3.8.3-cp311-cp311-macosx_10_12_x86_64.whl", hash = "sha256:5184e07c7e1d6d1481862ee361905b7059f7fe065fc837f7c3dc11eeb3f2f900"},
-    {file = "matplotlib-3.8.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:d7e7e0993d0758933b1a241a432b42c2db22dfa37d4108342ab4afb9557cbe3e"},
-    {file = "matplotlib-3.8.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:04b36ad07eac9740fc76c2aa16edf94e50b297d6eb4c081e3add863de4bb19a7"},
-    {file = "matplotlib-3.8.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7c42dae72a62f14982f1474f7e5c9959fc4bc70c9de11cc5244c6e766200ba65"},
-    {file = "matplotlib-3.8.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:bf5932eee0d428192c40b7eac1399d608f5d995f975cdb9d1e6b48539a5ad8d0"},
-    {file = "matplotlib-3.8.3-cp311-cp311-win_amd64.whl", hash = "sha256:40321634e3a05ed02abf7c7b47a50be50b53ef3eaa3a573847431a545585b407"},
-    {file = "matplotlib-3.8.3-cp312-cp312-macosx_10_12_x86_64.whl", hash = "sha256:09074f8057917d17ab52c242fdf4916f30e99959c1908958b1fc6032e2d0f6d4"},
-    {file = "matplotlib-3.8.3-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:5745f6d0fb5acfabbb2790318db03809a253096e98c91b9a31969df28ee604aa"},
-    {file = "matplotlib-3.8.3-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b97653d869a71721b639714b42d87cda4cfee0ee74b47c569e4874c7590c55c5"},
-    {file = "matplotlib-3.8.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:242489efdb75b690c9c2e70bb5c6550727058c8a614e4c7716f363c27e10bba1"},
-    {file = "matplotlib-3.8.3-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:83c0653c64b73926730bd9ea14aa0f50f202ba187c307a881673bad4985967b7"},
-    {file = "matplotlib-3.8.3-cp312-cp312-win_amd64.whl", hash = "sha256:ef6c1025a570354297d6c15f7d0f296d95f88bd3850066b7f1e7b4f2f4c13a39"},
-    {file = "matplotlib-3.8.3-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:fa93695d5c08544f4a0dfd0965f378e7afc410d8672816aff1e81be1f45dbf2e"},
-    {file = "matplotlib-3.8.3-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e9764df0e8778f06414b9d281a75235c1e85071f64bb5d71564b97c1306a2afc"},
-    {file = "matplotlib-3.8.3-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:5e431a09e6fab4012b01fc155db0ce6dccacdbabe8198197f523a4ef4805eb26"},
-    {file = "matplotlib-3.8.3.tar.gz", hash = "sha256:7b416239e9ae38be54b028abbf9048aff5054a9aba5416bef0bd17f9162ce161"},
+    {file = "matplotlib-3.8.4-cp310-cp310-macosx_10_12_x86_64.whl", hash = "sha256:abc9d838f93583650c35eca41cfcec65b2e7cb50fd486da6f0c49b5e1ed23014"},
+    {file = "matplotlib-3.8.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:8f65c9f002d281a6e904976007b2d46a1ee2bcea3a68a8c12dda24709ddc9106"},
+    {file = "matplotlib-3.8.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ce1edd9f5383b504dbc26eeea404ed0a00656c526638129028b758fd43fc5f10"},
+    {file = "matplotlib-3.8.4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ecd79298550cba13a43c340581a3ec9c707bd895a6a061a78fa2524660482fc0"},
+    {file = "matplotlib-3.8.4-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:90df07db7b599fe7035d2f74ab7e438b656528c68ba6bb59b7dc46af39ee48ef"},
+    {file = "matplotlib-3.8.4-cp310-cp310-win_amd64.whl", hash = "sha256:ac24233e8f2939ac4fd2919eed1e9c0871eac8057666070e94cbf0b33dd9c338"},
+    {file = "matplotlib-3.8.4-cp311-cp311-macosx_10_12_x86_64.whl", hash = "sha256:72f9322712e4562e792b2961971891b9fbbb0e525011e09ea0d1f416c4645661"},
+    {file = "matplotlib-3.8.4-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:232ce322bfd020a434caaffbd9a95333f7c2491e59cfc014041d95e38ab90d1c"},
+    {file = "matplotlib-3.8.4-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6addbd5b488aedb7f9bc19f91cd87ea476206f45d7116fcfe3d31416702a82fa"},
+    {file = "matplotlib-3.8.4-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:cc4ccdc64e3039fc303defd119658148f2349239871db72cd74e2eeaa9b80b71"},
+    {file = "matplotlib-3.8.4-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:b7a2a253d3b36d90c8993b4620183b55665a429da8357a4f621e78cd48b2b30b"},
+    {file = "matplotlib-3.8.4-cp311-cp311-win_amd64.whl", hash = "sha256:8080d5081a86e690d7688ffa542532e87f224c38a6ed71f8fbed34dd1d9fedae"},
+    {file = "matplotlib-3.8.4-cp312-cp312-macosx_10_12_x86_64.whl", hash = "sha256:6485ac1f2e84676cff22e693eaa4fbed50ef5dc37173ce1f023daef4687df616"},
+    {file = "matplotlib-3.8.4-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:c89ee9314ef48c72fe92ce55c4e95f2f39d70208f9f1d9db4e64079420d8d732"},
+    {file = "matplotlib-3.8.4-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:50bac6e4d77e4262c4340d7a985c30912054745ec99756ce213bfbc3cb3808eb"},
+    {file = "matplotlib-3.8.4-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f51c4c869d4b60d769f7b4406eec39596648d9d70246428745a681c327a8ad30"},
+    {file = "matplotlib-3.8.4-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:b12ba985837e4899b762b81f5b2845bd1a28f4fdd1a126d9ace64e9c4eb2fb25"},
+    {file = "matplotlib-3.8.4-cp312-cp312-win_amd64.whl", hash = "sha256:7a6769f58ce51791b4cb8b4d7642489df347697cd3e23d88266aaaee93b41d9a"},
+    {file = "matplotlib-3.8.4-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:c7064120a59ce6f64103c9cefba8ffe6fba87f2c61d67c401186423c9a20fd35"},
+    {file = "matplotlib-3.8.4-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a0e47eda4eb2614300fc7bb4657fced3e83d6334d03da2173b09e447418d499f"},
+    {file = "matplotlib-3.8.4-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:493e9f6aa5819156b58fce42b296ea31969f2aab71c5b680b4ea7a3cb5c07d94"},
+    {file = "matplotlib-3.8.4.tar.gz", hash = "sha256:8aac397d5e9ec158960e31c381c5ffc52ddd52bd9a47717e2a694038167dffea"},
 ]
 
 [[package]]
 name = "matplotlib-inline"
 version = "0.1.6"
 requires_python = ">=3.5"
 summary = "Inline Matplotlib backend for Jupyter"
@@ -1281,20 +1281,20 @@
 files = [
     {file = "outcome-1.3.0.post0-py2.py3-none-any.whl", hash = "sha256:e771c5ce06d1415e356078d3bdd68523f284b4ce5419828922b6871e65eda82b"},
     {file = "outcome-1.3.0.post0.tar.gz", hash = "sha256:9dcf02e65f2971b80047b377468e72a268e15c0af3cf1238e6ff14f7f91143b8"},
 ]
 
 [[package]]
 name = "packaging"
-version = "23.2"
+version = "24.0"
 requires_python = ">=3.7"
 summary = "Core utilities for Python packages"
 files = [
-    {file = "packaging-23.2-py3-none-any.whl", hash = "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"},
-    {file = "packaging-23.2.tar.gz", hash = "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5"},
+    {file = "packaging-24.0-py3-none-any.whl", hash = "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5"},
+    {file = "packaging-24.0.tar.gz", hash = "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"},
 ]
 
 [[package]]
 name = "pandas"
 version = "2.2.1"
 requires_python = ">=3.9"
 summary = "Powerful data structures for data analysis, time series, and statistics"
@@ -1329,20 +1329,20 @@
     {file = "pandas-2.2.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:11940e9e3056576ac3244baef2fedade891977bcc1cb7e5cc8f8cc7d603edc89"},
     {file = "pandas-2.2.1-cp312-cp312-win_amd64.whl", hash = "sha256:4acf681325ee1c7f950d058b05a820441075b0dd9a2adf5c4835b9bc056bf4fb"},
     {file = "pandas-2.2.1.tar.gz", hash = "sha256:0ab90f87093c13f3e8fa45b48ba9f39181046e8f3317d3aadb2fffbb1b978572"},
 ]
 
 [[package]]
 name = "parso"
-version = "0.8.3"
+version = "0.8.4"
 requires_python = ">=3.6"
 summary = "A Python Parser"
 files = [
-    {file = "parso-0.8.3-py2.py3-none-any.whl", hash = "sha256:c001d4636cd3aecdaf33cbb40aebb59b094be2a74c556778ef5576c175e19e75"},
-    {file = "parso-0.8.3.tar.gz", hash = "sha256:8c07be290bb59f03588915921e29e8a50002acaf2cdc5fa0e0114f91709fafa0"},
+    {file = "parso-0.8.4-py2.py3-none-any.whl", hash = "sha256:a418670a20291dacd2dddc80c377c5c3791378ee1e8d12bffc35420643d43f18"},
+    {file = "parso-0.8.4.tar.gz", hash = "sha256:eb3a7b58240fb99099a345571deecc0f9540ea5f4dd2fe14c2a99d6b281ab92d"},
 ]
 
 [[package]]
 name = "pbr"
 version = "6.0.0"
 requires_python = ">=2.6"
 summary = "Python Build Reasonableness"
@@ -1361,65 +1361,66 @@
 files = [
     {file = "pexpect-4.9.0-py2.py3-none-any.whl", hash = "sha256:7236d1e080e4936be2dc3e326cec0af72acf9212a7e1d060210e70a47e253523"},
     {file = "pexpect-4.9.0.tar.gz", hash = "sha256:ee7d41123f3c9911050ea2c2dac107568dc43b2d3b0c7557a33212c398ead30f"},
 ]
 
 [[package]]
 name = "pillow"
-version = "10.2.0"
+version = "10.3.0"
 requires_python = ">=3.8"
 summary = "Python Imaging Library (Fork)"
 files = [
-    {file = "pillow-10.2.0-cp310-cp310-macosx_10_10_x86_64.whl", hash = "sha256:7823bdd049099efa16e4246bdf15e5a13dbb18a51b68fa06d6c1d4d8b99a796e"},
-    {file = "pillow-10.2.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:83b2021f2ade7d1ed556bc50a399127d7fb245e725aa0113ebd05cfe88aaf588"},
-    {file = "pillow-10.2.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6fad5ff2f13d69b7e74ce5b4ecd12cc0ec530fcee76356cac6742785ff71c452"},
-    {file = "pillow-10.2.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:da2b52b37dad6d9ec64e653637a096905b258d2fc2b984c41ae7d08b938a67e4"},
-    {file = "pillow-10.2.0-cp310-cp310-manylinux_2_28_aarch64.whl", hash = "sha256:47c0995fc4e7f79b5cfcab1fc437ff2890b770440f7696a3ba065ee0fd496563"},
-    {file = "pillow-10.2.0-cp310-cp310-manylinux_2_28_x86_64.whl", hash = "sha256:322bdf3c9b556e9ffb18f93462e5f749d3444ce081290352c6070d014c93feb2"},
-    {file = "pillow-10.2.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:51f1a1bffc50e2e9492e87d8e09a17c5eea8409cda8d3f277eb6edc82813c17c"},
-    {file = "pillow-10.2.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:69ffdd6120a4737710a9eee73e1d2e37db89b620f702754b8f6e62594471dee0"},
-    {file = "pillow-10.2.0-cp310-cp310-win32.whl", hash = "sha256:c6dafac9e0f2b3c78df97e79af707cdc5ef8e88208d686a4847bab8266870023"},
-    {file = "pillow-10.2.0-cp310-cp310-win_amd64.whl", hash = "sha256:aebb6044806f2e16ecc07b2a2637ee1ef67a11840a66752751714a0d924adf72"},
-    {file = "pillow-10.2.0-cp310-cp310-win_arm64.whl", hash = "sha256:7049e301399273a0136ff39b84c3678e314f2158f50f517bc50285fb5ec847ad"},
-    {file = "pillow-10.2.0-cp311-cp311-macosx_10_10_x86_64.whl", hash = "sha256:35bb52c37f256f662abdfa49d2dfa6ce5d93281d323a9af377a120e89a9eafb5"},
-    {file = "pillow-10.2.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:9c23f307202661071d94b5e384e1e1dc7dfb972a28a2310e4ee16103e66ddb67"},
-    {file = "pillow-10.2.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:773efe0603db30c281521a7c0214cad7836c03b8ccff897beae9b47c0b657d61"},
-    {file = "pillow-10.2.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:11fa2e5984b949b0dd6d7a94d967743d87c577ff0b83392f17cb3990d0d2fd6e"},
-    {file = "pillow-10.2.0-cp311-cp311-manylinux_2_28_aarch64.whl", hash = "sha256:716d30ed977be8b37d3ef185fecb9e5a1d62d110dfbdcd1e2a122ab46fddb03f"},
-    {file = "pillow-10.2.0-cp311-cp311-manylinux_2_28_x86_64.whl", hash = "sha256:a086c2af425c5f62a65e12fbf385f7c9fcb8f107d0849dba5839461a129cf311"},
-    {file = "pillow-10.2.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:c8de2789052ed501dd829e9cae8d3dcce7acb4777ea4a479c14521c942d395b1"},
-    {file = "pillow-10.2.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:609448742444d9290fd687940ac0b57fb35e6fd92bdb65386e08e99af60bf757"},
-    {file = "pillow-10.2.0-cp311-cp311-win32.whl", hash = "sha256:823ef7a27cf86df6597fa0671066c1b596f69eba53efa3d1e1cb8b30f3533068"},
-    {file = "pillow-10.2.0-cp311-cp311-win_amd64.whl", hash = "sha256:1da3b2703afd040cf65ec97efea81cfba59cdbed9c11d8efc5ab09df9509fc56"},
-    {file = "pillow-10.2.0-cp311-cp311-win_arm64.whl", hash = "sha256:edca80cbfb2b68d7b56930b84a0e45ae1694aeba0541f798e908a49d66b837f1"},
-    {file = "pillow-10.2.0-cp312-cp312-macosx_10_10_x86_64.whl", hash = "sha256:1b5e1b74d1bd1b78bc3477528919414874748dd363e6272efd5abf7654e68bef"},
-    {file = "pillow-10.2.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:0eae2073305f451d8ecacb5474997c08569fb4eb4ac231ffa4ad7d342fdc25ac"},
-    {file = "pillow-10.2.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b7c2286c23cd350b80d2fc9d424fc797575fb16f854b831d16fd47ceec078f2c"},
-    {file = "pillow-10.2.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1e23412b5c41e58cec602f1135c57dfcf15482013ce6e5f093a86db69646a5aa"},
-    {file = "pillow-10.2.0-cp312-cp312-manylinux_2_28_aarch64.whl", hash = "sha256:52a50aa3fb3acb9cf7213573ef55d31d6eca37f5709c69e6858fe3bc04a5c2a2"},
-    {file = "pillow-10.2.0-cp312-cp312-manylinux_2_28_x86_64.whl", hash = "sha256:127cee571038f252a552760076407f9cff79761c3d436a12af6000cd182a9d04"},
-    {file = "pillow-10.2.0-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:8d12251f02d69d8310b046e82572ed486685c38f02176bd08baf216746eb947f"},
-    {file = "pillow-10.2.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:54f1852cd531aa981bc0965b7d609f5f6cc8ce8c41b1139f6ed6b3c54ab82bfb"},
-    {file = "pillow-10.2.0-cp312-cp312-win32.whl", hash = "sha256:257d8788df5ca62c980314053197f4d46eefedf4e6175bc9412f14412ec4ea2f"},
-    {file = "pillow-10.2.0-cp312-cp312-win_amd64.whl", hash = "sha256:154e939c5f0053a383de4fd3d3da48d9427a7e985f58af8e94d0b3c9fcfcf4f9"},
-    {file = "pillow-10.2.0-cp312-cp312-win_arm64.whl", hash = "sha256:f379abd2f1e3dddb2b61bc67977a6b5a0a3f7485538bcc6f39ec76163891ee48"},
-    {file = "pillow-10.2.0-pp310-pypy310_pp73-macosx_10_10_x86_64.whl", hash = "sha256:322209c642aabdd6207517e9739c704dc9f9db943015535783239022002f054a"},
-    {file = "pillow-10.2.0-pp310-pypy310_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3eedd52442c0a5ff4f887fab0c1c0bb164d8635b32c894bc1faf4c618dd89df2"},
-    {file = "pillow-10.2.0-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:cb28c753fd5eb3dd859b4ee95de66cc62af91bcff5db5f2571d32a520baf1f04"},
-    {file = "pillow-10.2.0-pp310-pypy310_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:33870dc4653c5017bf4c8873e5488d8f8d5f8935e2f1fb9a2208c47cdd66efd2"},
-    {file = "pillow-10.2.0-pp310-pypy310_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:3c31822339516fb3c82d03f30e22b1d038da87ef27b6a78c9549888f8ceda39a"},
-    {file = "pillow-10.2.0-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:a2b56ba36e05f973d450582fb015594aaa78834fefe8dfb8fcd79b93e64ba4c6"},
-    {file = "pillow-10.2.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:d8e6aeb9201e655354b3ad049cb77d19813ad4ece0df1249d3c793de3774f8c7"},
-    {file = "pillow-10.2.0-pp39-pypy39_pp73-macosx_10_10_x86_64.whl", hash = "sha256:2247178effb34a77c11c0e8ac355c7a741ceca0a732b27bf11e747bbc950722f"},
-    {file = "pillow-10.2.0-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:15587643b9e5eb26c48e49a7b33659790d28f190fc514a322d55da2fb5c2950e"},
-    {file = "pillow-10.2.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:753cd8f2086b2b80180d9b3010dd4ed147efc167c90d3bf593fe2af21265e5a5"},
-    {file = "pillow-10.2.0-pp39-pypy39_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:7c8f97e8e7a9009bcacbe3766a36175056c12f9a44e6e6f2d5caad06dcfbf03b"},
-    {file = "pillow-10.2.0-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:d1b35bcd6c5543b9cb547dee3150c93008f8dd0f1fef78fc0cd2b141c5baf58a"},
-    {file = "pillow-10.2.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:fe4c15f6c9285dc54ce6553a3ce908ed37c8f3825b5a51a15c91442bb955b868"},
-    {file = "pillow-10.2.0.tar.gz", hash = "sha256:e87f0b2c78157e12d7686b27d63c070fd65d994e8ddae6f328e0dcf4a0cd007e"},
+    {file = "pillow-10.3.0-cp310-cp310-macosx_10_10_x86_64.whl", hash = "sha256:90b9e29824800e90c84e4022dd5cc16eb2d9605ee13f05d47641eb183cd73d45"},
+    {file = "pillow-10.3.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:a2c405445c79c3f5a124573a051062300936b0281fee57637e706453e452746c"},
+    {file = "pillow-10.3.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:78618cdbccaa74d3f88d0ad6cb8ac3007f1a6fa5c6f19af64b55ca170bfa1edf"},
+    {file = "pillow-10.3.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:261ddb7ca91fcf71757979534fb4c128448b5b4c55cb6152d280312062f69599"},
+    {file = "pillow-10.3.0-cp310-cp310-manylinux_2_28_aarch64.whl", hash = "sha256:ce49c67f4ea0609933d01c0731b34b8695a7a748d6c8d186f95e7d085d2fe475"},
+    {file = "pillow-10.3.0-cp310-cp310-manylinux_2_28_x86_64.whl", hash = "sha256:b14f16f94cbc61215115b9b1236f9c18403c15dd3c52cf629072afa9d54c1cbf"},
+    {file = "pillow-10.3.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:d33891be6df59d93df4d846640f0e46f1a807339f09e79a8040bc887bdcd7ed3"},
+    {file = "pillow-10.3.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:b50811d664d392f02f7761621303eba9d1b056fb1868c8cdf4231279645c25f5"},
+    {file = "pillow-10.3.0-cp310-cp310-win32.whl", hash = "sha256:ca2870d5d10d8726a27396d3ca4cf7976cec0f3cb706debe88e3a5bd4610f7d2"},
+    {file = "pillow-10.3.0-cp310-cp310-win_amd64.whl", hash = "sha256:f0d0591a0aeaefdaf9a5e545e7485f89910c977087e7de2b6c388aec32011e9f"},
+    {file = "pillow-10.3.0-cp310-cp310-win_arm64.whl", hash = "sha256:ccce24b7ad89adb5a1e34a6ba96ac2530046763912806ad4c247356a8f33a67b"},
+    {file = "pillow-10.3.0-cp311-cp311-macosx_10_10_x86_64.whl", hash = "sha256:5f77cf66e96ae734717d341c145c5949c63180842a545c47a0ce7ae52ca83795"},
+    {file = "pillow-10.3.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:e4b878386c4bf293578b48fc570b84ecfe477d3b77ba39a6e87150af77f40c57"},
+    {file = "pillow-10.3.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fdcbb4068117dfd9ce0138d068ac512843c52295ed996ae6dd1faf537b6dbc27"},
+    {file = "pillow-10.3.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9797a6c8fe16f25749b371c02e2ade0efb51155e767a971c61734b1bf6293994"},
+    {file = "pillow-10.3.0-cp311-cp311-manylinux_2_28_aarch64.whl", hash = "sha256:9e91179a242bbc99be65e139e30690e081fe6cb91a8e77faf4c409653de39451"},
+    {file = "pillow-10.3.0-cp311-cp311-manylinux_2_28_x86_64.whl", hash = "sha256:1b87bd9d81d179bd8ab871603bd80d8645729939f90b71e62914e816a76fc6bd"},
+    {file = "pillow-10.3.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:81d09caa7b27ef4e61cb7d8fbf1714f5aec1c6b6c5270ee53504981e6e9121ad"},
+    {file = "pillow-10.3.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:048ad577748b9fa4a99a0548c64f2cb8d672d5bf2e643a739ac8faff1164238c"},
+    {file = "pillow-10.3.0-cp311-cp311-win32.whl", hash = "sha256:7161ec49ef0800947dc5570f86568a7bb36fa97dd09e9827dc02b718c5643f09"},
+    {file = "pillow-10.3.0-cp311-cp311-win_amd64.whl", hash = "sha256:8eb0908e954d093b02a543dc963984d6e99ad2b5e36503d8a0aaf040505f747d"},
+    {file = "pillow-10.3.0-cp311-cp311-win_arm64.whl", hash = "sha256:4e6f7d1c414191c1199f8996d3f2282b9ebea0945693fb67392c75a3a320941f"},
+    {file = "pillow-10.3.0-cp312-cp312-macosx_10_10_x86_64.whl", hash = "sha256:e46f38133e5a060d46bd630faa4d9fa0202377495df1f068a8299fd78c84de84"},
+    {file = "pillow-10.3.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:50b8eae8f7334ec826d6eeffaeeb00e36b5e24aa0b9df322c247539714c6df19"},
+    {file = "pillow-10.3.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9d3bea1c75f8c53ee4d505c3e67d8c158ad4df0d83170605b50b64025917f338"},
+    {file = "pillow-10.3.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:19aeb96d43902f0a783946a0a87dbdad5c84c936025b8419da0a0cd7724356b1"},
+    {file = "pillow-10.3.0-cp312-cp312-manylinux_2_28_aarch64.whl", hash = "sha256:74d28c17412d9caa1066f7a31df8403ec23d5268ba46cd0ad2c50fb82ae40462"},
+    {file = "pillow-10.3.0-cp312-cp312-manylinux_2_28_x86_64.whl", hash = "sha256:ff61bfd9253c3915e6d41c651d5f962da23eda633cf02262990094a18a55371a"},
+    {file = "pillow-10.3.0-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:d886f5d353333b4771d21267c7ecc75b710f1a73d72d03ca06df49b09015a9ef"},
+    {file = "pillow-10.3.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:4b5ec25d8b17217d635f8935dbc1b9aa5907962fae29dff220f2659487891cd3"},
+    {file = "pillow-10.3.0-cp312-cp312-win32.whl", hash = "sha256:51243f1ed5161b9945011a7360e997729776f6e5d7005ba0c6879267d4c5139d"},
+    {file = "pillow-10.3.0-cp312-cp312-win_amd64.whl", hash = "sha256:412444afb8c4c7a6cc11a47dade32982439925537e483be7c0ae0cf96c4f6a0b"},
+    {file = "pillow-10.3.0-cp312-cp312-win_arm64.whl", hash = "sha256:798232c92e7665fe82ac085f9d8e8ca98826f8e27859d9a96b41d519ecd2e49a"},
+    {file = "pillow-10.3.0-pp310-pypy310_pp73-macosx_10_10_x86_64.whl", hash = "sha256:6b02471b72526ab8a18c39cb7967b72d194ec53c1fd0a70b050565a0f366d355"},
+    {file = "pillow-10.3.0-pp310-pypy310_pp73-macosx_11_0_arm64.whl", hash = "sha256:8ab74c06ffdab957d7670c2a5a6e1a70181cd10b727cd788c4dd9005b6a8acd9"},
+    {file = "pillow-10.3.0-pp310-pypy310_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:048eeade4c33fdf7e08da40ef402e748df113fd0b4584e32c4af74fe78baaeb2"},
+    {file = "pillow-10.3.0-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9e2ec1e921fd07c7cda7962bad283acc2f2a9ccc1b971ee4b216b75fad6f0463"},
+    {file = "pillow-10.3.0-pp310-pypy310_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:4c8e73e99da7db1b4cad7f8d682cf6abad7844da39834c288fbfa394a47bbced"},
+    {file = "pillow-10.3.0-pp310-pypy310_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:16563993329b79513f59142a6b02055e10514c1a8e86dca8b48a893e33cf91e3"},
+    {file = "pillow-10.3.0-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:dd78700f5788ae180b5ee8902c6aea5a5726bac7c364b202b4b3e3ba2d293170"},
+    {file = "pillow-10.3.0-pp39-pypy39_pp73-macosx_10_10_x86_64.whl", hash = "sha256:aff76a55a8aa8364d25400a210a65ff59d0168e0b4285ba6bf2bd83cf675ba32"},
+    {file = "pillow-10.3.0-pp39-pypy39_pp73-macosx_11_0_arm64.whl", hash = "sha256:b7bc2176354defba3edc2b9a777744462da2f8e921fbaf61e52acb95bafa9828"},
+    {file = "pillow-10.3.0-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:793b4e24db2e8742ca6423d3fde8396db336698c55cd34b660663ee9e45ed37f"},
+    {file = "pillow-10.3.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d93480005693d247f8346bc8ee28c72a2191bdf1f6b5db469c096c0c867ac015"},
+    {file = "pillow-10.3.0-pp39-pypy39_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:c83341b89884e2b2e55886e8fbbf37c3fa5efd6c8907124aeb72f285ae5696e5"},
+    {file = "pillow-10.3.0-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:1a1d1915db1a4fdb2754b9de292642a39a7fb28f1736699527bb649484fb966a"},
+    {file = "pillow-10.3.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:a0eaa93d054751ee9964afa21c06247779b90440ca41d184aeb5d410f20ff591"},
+    {file = "pillow-10.3.0.tar.gz", hash = "sha256:9d2455fbf44c914840c793e89aa82d0e1763a14253a000743719ae5946814b2d"},
 ]
 
 [[package]]
 name = "pluggy"
 version = "1.4.0"
 requires_python = ">=3.8"
 summary = "plugin and hook calling mechanisms for python"
@@ -1467,25 +1468,25 @@
 files = [
     {file = "prompt_toolkit-3.0.43-py3-none-any.whl", hash = "sha256:a11a29cb3bf0a28a387fe5122cdb649816a957cd9261dcedf8c9f1fef33eacf6"},
     {file = "prompt_toolkit-3.0.43.tar.gz", hash = "sha256:3527b7af26106cbc65a040bcc84839a3566ec1b051bb0bfe953631e704b0ff7d"},
 ]
 
 [[package]]
 name = "protobuf"
-version = "4.25.3"
+version = "5.26.1"
 requires_python = ">=3.8"
 summary = ""
 files = [
-    {file = "protobuf-4.25.3-cp310-abi3-win32.whl", hash = "sha256:d4198877797a83cbfe9bffa3803602bbe1625dc30d8a097365dbc762e5790faa"},
-    {file = "protobuf-4.25.3-cp310-abi3-win_amd64.whl", hash = "sha256:209ba4cc916bab46f64e56b85b090607a676f66b473e6b762e6f1d9d591eb2e8"},
-    {file = "protobuf-4.25.3-cp37-abi3-macosx_10_9_universal2.whl", hash = "sha256:f1279ab38ecbfae7e456a108c5c0681e4956d5b1090027c1de0f934dfdb4b35c"},
-    {file = "protobuf-4.25.3-cp37-abi3-manylinux2014_aarch64.whl", hash = "sha256:e7cb0ae90dd83727f0c0718634ed56837bfeeee29a5f82a7514c03ee1364c019"},
-    {file = "protobuf-4.25.3-cp37-abi3-manylinux2014_x86_64.whl", hash = "sha256:7c8daa26095f82482307bc717364e7c13f4f1c99659be82890dcfc215194554d"},
-    {file = "protobuf-4.25.3-py3-none-any.whl", hash = "sha256:f0700d54bcf45424477e46a9f0944155b46fb0639d69728739c0e47bab83f2b9"},
-    {file = "protobuf-4.25.3.tar.gz", hash = "sha256:25b5d0b42fd000320bd7830b349e3b696435f3b329810427a6bcce6a5492cc5c"},
+    {file = "protobuf-5.26.1-cp310-abi3-win32.whl", hash = "sha256:3c388ea6ddfe735f8cf69e3f7dc7611e73107b60bdfcf5d0f024c3ccd3794e23"},
+    {file = "protobuf-5.26.1-cp310-abi3-win_amd64.whl", hash = "sha256:e6039957449cb918f331d32ffafa8eb9255769c96aa0560d9a5bf0b4e00a2a33"},
+    {file = "protobuf-5.26.1-cp37-abi3-macosx_10_9_universal2.whl", hash = "sha256:38aa5f535721d5bb99861166c445c4105c4e285c765fbb2ac10f116e32dcd46d"},
+    {file = "protobuf-5.26.1-cp37-abi3-manylinux2014_aarch64.whl", hash = "sha256:fbfe61e7ee8c1860855696e3ac6cfd1b01af5498facc6834fcc345c9684fb2ca"},
+    {file = "protobuf-5.26.1-cp37-abi3-manylinux2014_x86_64.whl", hash = "sha256:f7417703f841167e5a27d48be13389d52ad705ec09eade63dfc3180a959215d7"},
+    {file = "protobuf-5.26.1-py3-none-any.whl", hash = "sha256:da612f2720c0183417194eeaa2523215c4fcc1a1949772dc65f05047e08d5932"},
+    {file = "protobuf-5.26.1.tar.gz", hash = "sha256:8ca2a1d97c290ec7b16e4e5dff2e5ae150cc1582f55b5ab300d45cb0dfa90e51"},
 ]
 
 [[package]]
 name = "ptyprocess"
 version = "0.7.0"
 summary = "Run a subprocess in a pseudo terminal"
 files = [
@@ -1509,20 +1510,20 @@
 files = [
     {file = "puremagic-1.21-py3-none-any.whl", hash = "sha256:8fe85c05800fe1eacdd5aa943b9e7fdbee66bc41a17aacf80efd6c668c63df45"},
     {file = "puremagic-1.21.tar.gz", hash = "sha256:31ef09b37a6ad2f7f2b09b5bd6b8c4a07187a01af4025f5f1368889bdfc6d779"},
 ]
 
 [[package]]
 name = "pyasn1"
-version = "0.5.1"
-requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7"
+version = "0.6.0"
+requires_python = ">=3.8"
 summary = "Pure-Python implementation of ASN.1 types and DER/BER/CER codecs (X.208)"
 files = [
-    {file = "pyasn1-0.5.1-py2.py3-none-any.whl", hash = "sha256:4439847c58d40b1d0a573d07e3856e95333f1976294494c325775aeca506eb58"},
-    {file = "pyasn1-0.5.1.tar.gz", hash = "sha256:6d391a96e59b23130a5cfa74d6fd7f388dbbe26cc8f1edf39fdddf08d9d6676c"},
+    {file = "pyasn1-0.6.0-py2.py3-none-any.whl", hash = "sha256:cca4bb0f2df5504f02f6f8a775b6e416ff9b0b3b16f7ee80b5a3153d9b804473"},
+    {file = "pyasn1-0.6.0.tar.gz", hash = "sha256:3a35ab2c4b5ef98e17dfdec8ab074046fbda76e281c5a706ccd82328cfc8f64c"},
 ]
 
 [[package]]
 name = "pychromecast"
 version = "13.1.0"
 summary = "Python module to talk to Google Chromecast."
 dependencies = [
@@ -1533,20 +1534,20 @@
 files = [
     {file = "PyChromecast-13.1.0-py2.py3-none-any.whl", hash = "sha256:cac3c6d740deb2d4fd5ac4101a1f8fd2404eab1a32cf40292ea9477075315663"},
     {file = "PyChromecast-13.1.0.tar.gz", hash = "sha256:08e61a8b54bd2119d3c9ab1ec0136d3d8563aa97e0a3b57841588b9be60c2676"},
 ]
 
 [[package]]
 name = "pycparser"
-version = "2.21"
-requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
+version = "2.22"
+requires_python = ">=3.8"
 summary = "C parser in Python"
 files = [
-    {file = "pycparser-2.21-py2.py3-none-any.whl", hash = "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9"},
-    {file = "pycparser-2.21.tar.gz", hash = "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"},
+    {file = "pycparser-2.22-py3-none-any.whl", hash = "sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc"},
+    {file = "pycparser-2.22.tar.gz", hash = "sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6"},
 ]
 
 [[package]]
 name = "pycryptodomex"
 version = "3.20.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
 summary = "Cryptographic library for Python"
@@ -1617,60 +1618,60 @@
 files = [
     {file = "pymcdm-1.2.0-py3-none-any.whl", hash = "sha256:e4c4e1168e8bace889b9453a3e58b9b571264fab5d068e66e49313dddb626f41"},
     {file = "pymcdm-1.2.0.tar.gz", hash = "sha256:eeb69029f1fdbb7a01a18ac58c3f100e7cbf4b51c0fe198e9a2c173470bc7bc0"},
 ]
 
 [[package]]
 name = "pyobjc-core"
-version = "10.1"
+version = "10.2"
 requires_python = ">=3.8"
 summary = "Python<->ObjC Interoperability Module"
 files = [
-    {file = "pyobjc-core-10.1.tar.gz", hash = "sha256:1844f1c8e282839e6fdcb9a9722396c1c12fb1e9331eb68828a26f28a3b2b2b1"},
-    {file = "pyobjc_core-10.1-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:2a72a88222539ad07b5c8be411edc52ff9147d7cef311a2c849869d7bb9603fd"},
-    {file = "pyobjc_core-10.1-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:fe1b9987b7b0437685fb529832876c2a8463500114960d4e76bb8ae96b6bf208"},
-    {file = "pyobjc_core-10.1-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:9f628779c345d3abd0e20048fb0e256d894c22254577a81a6dcfdb92c3647682"},
+    {file = "pyobjc-core-10.2.tar.gz", hash = "sha256:0153206e15d0e0d7abd53ee8a7fbaf5606602a032e177a028fc8589516a8771c"},
+    {file = "pyobjc_core-10.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:b8eab50ce7f17017a0f1d68c3b7e88bb1bb033415fdff62b8e0a9ee4ab72f242"},
+    {file = "pyobjc_core-10.2-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:f2115971463073426ab926416e17e5c16de5b90d1a1f2a2d8724637eb1c21308"},
+    {file = "pyobjc_core-10.2-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:a70546246177c23acb323c9324330e37638f1a0a3d13664abcba3bb75e43012c"},
 ]
 
 [[package]]
 name = "pyobjc-framework-cocoa"
-version = "10.1"
+version = "10.2"
 requires_python = ">=3.8"
 summary = "Wrappers for the Cocoa frameworks on macOS"
 dependencies = [
-    "pyobjc-core>=10.1",
+    "pyobjc-core>=10.2",
 ]
 files = [
-    {file = "pyobjc-framework-Cocoa-10.1.tar.gz", hash = "sha256:8faaf1292a112e488b777d0c19862d993f3f384f3927dc6eca0d8d2221906a14"},
-    {file = "pyobjc_framework_Cocoa-10.1-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:2e82c2e20b89811d92a7e6e487b6980f360b7c142e2576e90f0e7569caf8202b"},
-    {file = "pyobjc_framework_Cocoa-10.1-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:0860a9beb7e5c72a1f575679a6d1428a398fa19ad710fb116df899972912e304"},
-    {file = "pyobjc_framework_Cocoa-10.1-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:34b791ea740e1afce211f19334e45469fea9a48d8fce5072e146199fd19ff49f"},
+    {file = "pyobjc-framework-Cocoa-10.2.tar.gz", hash = "sha256:6383141379636b13855dca1b39c032752862b829f93a49d7ddb35046abfdc035"},
+    {file = "pyobjc_framework_Cocoa-10.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:f9227b4f271fda2250f5a88cbc686ff30ae02c0f923bb7854bb47972397496b2"},
+    {file = "pyobjc_framework_Cocoa-10.2-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:6a6042b7703bdc33b7491959c715c1e810a3f8c7a560c94b36e00ef321480797"},
+    {file = "pyobjc_framework_Cocoa-10.2-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:18886d5013cd7dc7ecd6e0df5134c767569b5247fc10a5e293c72ee3937b217b"},
 ]
 
 [[package]]
 name = "pyopenssl"
-version = "24.0.0"
+version = "24.1.0"
 requires_python = ">=3.7"
 summary = "Python wrapper module around the OpenSSL library"
 dependencies = [
     "cryptography<43,>=41.0.5",
 ]
 files = [
-    {file = "pyOpenSSL-24.0.0-py3-none-any.whl", hash = "sha256:ba07553fb6fd6a7a2259adb9b84e12302a9a8a75c44046e8bb5d3e5ee887e3c3"},
-    {file = "pyOpenSSL-24.0.0.tar.gz", hash = "sha256:6aa33039a93fffa4563e655b61d11364d01264be8ccb49906101e02a334530bf"},
+    {file = "pyOpenSSL-24.1.0-py3-none-any.whl", hash = "sha256:17ed5be5936449c5418d1cd269a1a9e9081bc54c17aed272b45856a3d3dc86ad"},
+    {file = "pyOpenSSL-24.1.0.tar.gz", hash = "sha256:cabed4bfaa5df9f1a16c0ef64a0cb65318b5cd077a7eda7d6970131ca2f41a6f"},
 ]
 
 [[package]]
 name = "pyparsing"
-version = "3.1.1"
+version = "3.1.2"
 requires_python = ">=3.6.8"
 summary = "pyparsing module - Classes and methods to define and execute parsing grammars"
 files = [
-    {file = "pyparsing-3.1.1-py3-none-any.whl", hash = "sha256:32c7c0b711493c72ff18a981d24f28aaf9c1fb7ed5e9667c9e84e3db623bdbfb"},
-    {file = "pyparsing-3.1.1.tar.gz", hash = "sha256:ede28a1a32462f5a9705e07aea48001a08f7cf81a021585011deba701581a0db"},
+    {file = "pyparsing-3.1.2-py3-none-any.whl", hash = "sha256:f9db75911801ed778fe61bb643079ff86601aca99fcae6345aa67292038fb742"},
+    {file = "pyparsing-3.1.2.tar.gz", hash = "sha256:a1bac0ce561155ecc3ed78ca94d3c9378656ad4c94c1270de543f621420f94ad"},
 ]
 
 [[package]]
 name = "pyproj"
 version = "3.6.1"
 requires_python = ">=3.9"
 summary = "Python interface to PROJ (cartographic projections and coordinate transformations library)"
@@ -1730,41 +1731,41 @@
 files = [
     {file = "pysubs2-1.6.1-py3-none-any.whl", hash = "sha256:1f96d9dfb5f859a54a00e04621beb20ff21ea1d788821b2f4935c5c0ef8dc68e"},
     {file = "pysubs2-1.6.1.tar.gz", hash = "sha256:0261611e71735ff7763972c519c72593c8063efcb9039c54af65f31b81cec116"},
 ]
 
 [[package]]
 name = "pytest"
-version = "8.0.2"
+version = "8.1.1"
 requires_python = ">=3.8"
 summary = "pytest: simple powerful testing with Python"
 dependencies = [
     "colorama; sys_platform == \"win32\"",
     "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
     "iniconfig",
     "packaging",
-    "pluggy<2.0,>=1.3.0",
-    "tomli>=1.0.0; python_version < \"3.11\"",
+    "pluggy<2.0,>=1.4",
+    "tomli>=1; python_version < \"3.11\"",
 ]
 files = [
-    {file = "pytest-8.0.2-py3-none-any.whl", hash = "sha256:edfaaef32ce5172d5466b5127b42e0d6d35ebbe4453f0e3505d96afd93f6b096"},
-    {file = "pytest-8.0.2.tar.gz", hash = "sha256:d4051d623a2e0b7e51960ba963193b09ce6daeb9759a451844a21e4ddedfc1bd"},
+    {file = "pytest-8.1.1-py3-none-any.whl", hash = "sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7"},
+    {file = "pytest-8.1.1.tar.gz", hash = "sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044"},
 ]
 
 [[package]]
 name = "python-dateutil"
-version = "2.8.2"
+version = "2.9.0.post0"
 requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,>=2.7"
 summary = "Extensions to the standard Python datetime module"
 dependencies = [
     "six>=1.5",
 ]
 files = [
-    {file = "python-dateutil-2.8.2.tar.gz", hash = "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86"},
-    {file = "python_dateutil-2.8.2-py2.py3-none-any.whl", hash = "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"},
+    {file = "python-dateutil-2.9.0.post0.tar.gz", hash = "sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3"},
+    {file = "python_dateutil-2.9.0.post0-py2.py3-none-any.whl", hash = "sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427"},
 ]
 
 [[package]]
 name = "python-mpv-jsonipc"
 version = "1.2.0"
 requires_python = ">=3.6"
 summary = "Python API to MPV using JSON IPC"
@@ -1789,20 +1790,20 @@
 files = [
     {file = "PyVirtualDisplay-3.0-py3-none-any.whl", hash = "sha256:40d4b8dfe4b8de8552e28eb367647f311f88a130bf837fe910e7f180d5477f0e"},
     {file = "PyVirtualDisplay-3.0.tar.gz", hash = "sha256:09755bc3ceb6eb725fb07eca5425f43f2358d3bf08e00d2a9b792a1aedd16159"},
 ]
 
 [[package]]
 name = "rarfile"
-version = "4.1"
+version = "4.2"
 requires_python = ">=3.6"
 summary = "RAR archive reader for Python"
 files = [
-    {file = "rarfile-4.1-py3-none-any.whl", hash = "sha256:17d7554c93c776ceae677e9d927051267d4c5eba38bf64b9cc89a415d9a5f901"},
-    {file = "rarfile-4.1.tar.gz", hash = "sha256:db60b3b5bc1c4bdeb941427d50b606d51df677353385255583847639473eda48"},
+    {file = "rarfile-4.2-py3-none-any.whl", hash = "sha256:8757e1e3757e32962e229cab2432efc1f15f210823cc96ccba0f6a39d17370c9"},
+    {file = "rarfile-4.2.tar.gz", hash = "sha256:8e1c8e72d0845ad2b32a47ab11a719bc2e41165ec101fd4d3fe9e92aa3f469ef"},
 ]
 
 [[package]]
 name = "rebulk"
 version = "3.2.0"
 summary = "Rebulk - Define simple search patterns in bulk to perform advanced matching on any string."
 files = [
@@ -1893,35 +1894,35 @@
 files = [
     {file = "rich-13.7.1-py3-none-any.whl", hash = "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222"},
     {file = "rich-13.7.1.tar.gz", hash = "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"},
 ]
 
 [[package]]
 name = "ruff"
-version = "0.2.2"
+version = "0.3.5"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter and code formatter, written in Rust."
 files = [
-    {file = "ruff-0.2.2-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:0a9efb032855ffb3c21f6405751d5e147b0c6b631e3ca3f6b20f917572b97eb6"},
-    {file = "ruff-0.2.2-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:d450b7fbff85913f866a5384d8912710936e2b96da74541c82c1b458472ddb39"},
-    {file = "ruff-0.2.2-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ecd46e3106850a5c26aee114e562c329f9a1fbe9e4821b008c4404f64ff9ce73"},
-    {file = "ruff-0.2.2-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:5e22676a5b875bd72acd3d11d5fa9075d3a5f53b877fe7b4793e4673499318ba"},
-    {file = "ruff-0.2.2-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1695700d1e25a99d28f7a1636d85bafcc5030bba9d0578c0781ba1790dbcf51c"},
-    {file = "ruff-0.2.2-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:b0c232af3d0bd8f521806223723456ffebf8e323bd1e4e82b0befb20ba18388e"},
-    {file = "ruff-0.2.2-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:f63d96494eeec2fc70d909393bcd76c69f35334cdbd9e20d089fb3f0640216ca"},
-    {file = "ruff-0.2.2-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:6a61ea0ff048e06de273b2e45bd72629f470f5da8f71daf09fe481278b175001"},
-    {file = "ruff-0.2.2-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5e1439c8f407e4f356470e54cdecdca1bd5439a0673792dbe34a2b0a551a2fe3"},
-    {file = "ruff-0.2.2-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:940de32dc8853eba0f67f7198b3e79bc6ba95c2edbfdfac2144c8235114d6726"},
-    {file = "ruff-0.2.2-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:0c126da55c38dd917621552ab430213bdb3273bb10ddb67bc4b761989210eb6e"},
-    {file = "ruff-0.2.2-py3-none-musllinux_1_2_i686.whl", hash = "sha256:3b65494f7e4bed2e74110dac1f0d17dc8e1f42faaa784e7c58a98e335ec83d7e"},
-    {file = "ruff-0.2.2-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:1ec49be4fe6ddac0503833f3ed8930528e26d1e60ad35c2446da372d16651ce9"},
-    {file = "ruff-0.2.2-py3-none-win32.whl", hash = "sha256:d920499b576f6c68295bc04e7b17b6544d9d05f196bb3aac4358792ef6f34325"},
-    {file = "ruff-0.2.2-py3-none-win_amd64.whl", hash = "sha256:cc9a91ae137d687f43a44c900e5d95e9617cb37d4c989e462980ba27039d239d"},
-    {file = "ruff-0.2.2-py3-none-win_arm64.whl", hash = "sha256:c9d15fc41e6054bfc7200478720570078f0b41c9ae4f010bcc16bd6f4d1aacdd"},
-    {file = "ruff-0.2.2.tar.gz", hash = "sha256:e62ed7f36b3068a30ba39193a14274cd706bc486fad521276458022f7bccb31d"},
+    {file = "ruff-0.3.5-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:aef5bd3b89e657007e1be6b16553c8813b221ff6d92c7526b7e0227450981eac"},
+    {file = "ruff-0.3.5-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:89b1e92b3bd9fca249153a97d23f29bed3992cff414b222fcd361d763fc53f12"},
+    {file = "ruff-0.3.5-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5e55771559c89272c3ebab23326dc23e7f813e492052391fe7950c1a5a139d89"},
+    {file = "ruff-0.3.5-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:dabc62195bf54b8a7876add6e789caae0268f34582333cda340497c886111c39"},
+    {file = "ruff-0.3.5-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3a05f3793ba25f194f395578579c546ca5d83e0195f992edc32e5907d142bfa3"},
+    {file = "ruff-0.3.5-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:dfd3504e881082959b4160ab02f7a205f0fadc0a9619cc481982b6837b2fd4c0"},
+    {file = "ruff-0.3.5-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:87258e0d4b04046cf1d6cc1c56fadbf7a880cc3de1f7294938e923234cf9e498"},
+    {file = "ruff-0.3.5-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:712e71283fc7d9f95047ed5f793bc019b0b0a29849b14664a60fd66c23b96da1"},
+    {file = "ruff-0.3.5-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a532a90b4a18d3f722c124c513ffb5e5eaff0cc4f6d3aa4bda38e691b8600c9f"},
+    {file = "ruff-0.3.5-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:122de171a147c76ada00f76df533b54676f6e321e61bd8656ae54be326c10296"},
+    {file = "ruff-0.3.5-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:d80a6b18a6c3b6ed25b71b05eba183f37d9bc8b16ace9e3d700997f00b74660b"},
+    {file = "ruff-0.3.5-py3-none-musllinux_1_2_i686.whl", hash = "sha256:a7b6e63194c68bca8e71f81de30cfa6f58ff70393cf45aab4c20f158227d5936"},
+    {file = "ruff-0.3.5-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:a759d33a20c72f2dfa54dae6e85e1225b8e302e8ac655773aff22e542a300985"},
+    {file = "ruff-0.3.5-py3-none-win32.whl", hash = "sha256:9d8605aa990045517c911726d21293ef4baa64f87265896e491a05461cae078d"},
+    {file = "ruff-0.3.5-py3-none-win_amd64.whl", hash = "sha256:dc56bb16a63c1303bd47563c60482a1512721053d93231cf7e9e1c6954395a0e"},
+    {file = "ruff-0.3.5-py3-none-win_arm64.whl", hash = "sha256:faeeae9905446b975dcf6d4499dc93439b131f1443ee264055c5716dd947af55"},
+    {file = "ruff-0.3.5.tar.gz", hash = "sha256:a067daaeb1dc2baf9b82a32dae67d154d95212080c80435eb052d95da647763d"},
 ]
 
 [[package]]
 name = "scikit-learn"
 version = "1.4.1.post1"
 requires_python = ">=3.9"
 summary = "A set of python modules for machine learning and data mining"
@@ -1948,40 +1949,40 @@
     {file = "scikit_learn-1.4.1.post1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:712c1c69c45b58ef21635360b3d0a680ff7d83ac95b6f9b82cf9294070cda710"},
     {file = "scikit_learn-1.4.1.post1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1754b0c2409d6ed5a3380512d0adcf182a01363c669033a2b55cca429ed86a81"},
     {file = "scikit_learn-1.4.1.post1-cp312-cp312-win_amd64.whl", hash = "sha256:1d491ef66e37f4e812db7e6c8286520c2c3fc61b34bf5e59b67b4ce528de93af"},
 ]
 
 [[package]]
 name = "scipy"
-version = "1.12.0"
+version = "1.13.0"
 requires_python = ">=3.9"
 summary = "Fundamental algorithms for scientific computing in Python"
 dependencies = [
-    "numpy<1.29.0,>=1.22.4",
+    "numpy<2.3,>=1.22.4",
 ]
 files = [
-    {file = "scipy-1.12.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:78e4402e140879387187f7f25d91cc592b3501a2e51dfb320f48dfb73565f10b"},
-    {file = "scipy-1.12.0-cp310-cp310-macosx_12_0_arm64.whl", hash = "sha256:f5f00ebaf8de24d14b8449981a2842d404152774c1a1d880c901bf454cb8e2a1"},
-    {file = "scipy-1.12.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e53958531a7c695ff66c2e7bb7b79560ffdc562e2051644c5576c39ff8efb563"},
-    {file = "scipy-1.12.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5e32847e08da8d895ce09d108a494d9eb78974cf6de23063f93306a3e419960c"},
-    {file = "scipy-1.12.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:4c1020cad92772bf44b8e4cdabc1df5d87376cb219742549ef69fc9fd86282dd"},
-    {file = "scipy-1.12.0-cp310-cp310-win_amd64.whl", hash = "sha256:75ea2a144096b5e39402e2ff53a36fecfd3b960d786b7efd3c180e29c39e53f2"},
-    {file = "scipy-1.12.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:408c68423f9de16cb9e602528be4ce0d6312b05001f3de61fe9ec8b1263cad08"},
-    {file = "scipy-1.12.0-cp311-cp311-macosx_12_0_arm64.whl", hash = "sha256:5adfad5dbf0163397beb4aca679187d24aec085343755fcdbdeb32b3679f254c"},
-    {file = "scipy-1.12.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c3003652496f6e7c387b1cf63f4bb720951cfa18907e998ea551e6de51a04467"},
-    {file = "scipy-1.12.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8b8066bce124ee5531d12a74b617d9ac0ea59245246410e19bca549656d9a40a"},
-    {file = "scipy-1.12.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:8bee4993817e204d761dba10dbab0774ba5a8612e57e81319ea04d84945375ba"},
-    {file = "scipy-1.12.0-cp311-cp311-win_amd64.whl", hash = "sha256:a24024d45ce9a675c1fb8494e8e5244efea1c7a09c60beb1eeb80373d0fecc70"},
-    {file = "scipy-1.12.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:e7e76cc48638228212c747ada851ef355c2bb5e7f939e10952bc504c11f4e372"},
-    {file = "scipy-1.12.0-cp312-cp312-macosx_12_0_arm64.whl", hash = "sha256:f7ce148dffcd64ade37b2df9315541f9adad6efcaa86866ee7dd5db0c8f041c3"},
-    {file = "scipy-1.12.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9c39f92041f490422924dfdb782527a4abddf4707616e07b021de33467f917bc"},
-    {file = "scipy-1.12.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a7ebda398f86e56178c2fa94cad15bf457a218a54a35c2a7b4490b9f9cb2676c"},
-    {file = "scipy-1.12.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:95e5c750d55cf518c398a8240571b0e0782c2d5a703250872f36eaf737751338"},
-    {file = "scipy-1.12.0-cp312-cp312-win_amd64.whl", hash = "sha256:e646d8571804a304e1da01040d21577685ce8e2db08ac58e543eaca063453e1c"},
-    {file = "scipy-1.12.0.tar.gz", hash = "sha256:4bf5abab8a36d20193c698b0f1fc282c1d083c94723902c447e5d2f1780936a3"},
+    {file = "scipy-1.13.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:ba419578ab343a4e0a77c0ef82f088238a93eef141b2b8017e46149776dfad4d"},
+    {file = "scipy-1.13.0-cp310-cp310-macosx_12_0_arm64.whl", hash = "sha256:22789b56a999265431c417d462e5b7f2b487e831ca7bef5edeb56efe4c93f86e"},
+    {file = "scipy-1.13.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:05f1432ba070e90d42d7fd836462c50bf98bd08bed0aa616c359eed8a04e3922"},
+    {file = "scipy-1.13.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b8434f6f3fa49f631fae84afee424e2483289dfc30a47755b4b4e6b07b2633a4"},
+    {file = "scipy-1.13.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:dcbb9ea49b0167de4167c40eeee6e167caeef11effb0670b554d10b1e693a8b9"},
+    {file = "scipy-1.13.0-cp310-cp310-win_amd64.whl", hash = "sha256:1d2f7bb14c178f8b13ebae93f67e42b0a6b0fc50eba1cd8021c9b6e08e8fb1cd"},
+    {file = "scipy-1.13.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:0fbcf8abaf5aa2dc8d6400566c1a727aed338b5fe880cde64907596a89d576fa"},
+    {file = "scipy-1.13.0-cp311-cp311-macosx_12_0_arm64.whl", hash = "sha256:5e4a756355522eb60fcd61f8372ac2549073c8788f6114449b37e9e8104f15a5"},
+    {file = "scipy-1.13.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b5acd8e1dbd8dbe38d0004b1497019b2dbbc3d70691e65d69615f8a7292865d7"},
+    {file = "scipy-1.13.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9ff7dad5d24a8045d836671e082a490848e8639cabb3dbdacb29f943a678683d"},
+    {file = "scipy-1.13.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:4dca18c3ffee287ddd3bc8f1dabaf45f5305c5afc9f8ab9cbfab855e70b2df5c"},
+    {file = "scipy-1.13.0-cp311-cp311-win_amd64.whl", hash = "sha256:a2f471de4d01200718b2b8927f7d76b5d9bde18047ea0fa8bd15c5ba3f26a1d6"},
+    {file = "scipy-1.13.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:d0de696f589681c2802f9090fff730c218f7c51ff49bf252b6a97ec4a5d19e8b"},
+    {file = "scipy-1.13.0-cp312-cp312-macosx_12_0_arm64.whl", hash = "sha256:b2a3ff461ec4756b7e8e42e1c681077349a038f0686132d623fa404c0bee2551"},
+    {file = "scipy-1.13.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6bf9fe63e7a4bf01d3645b13ff2aa6dea023d38993f42aaac81a18b1bda7a82a"},
+    {file = "scipy-1.13.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1e7626dfd91cdea5714f343ce1176b6c4745155d234f1033584154f60ef1ff42"},
+    {file = "scipy-1.13.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:109d391d720fcebf2fbe008621952b08e52907cf4c8c7efc7376822151820820"},
+    {file = "scipy-1.13.0-cp312-cp312-win_amd64.whl", hash = "sha256:8930ae3ea371d6b91c203b1032b9600d69c568e537b7988a3073dfe4d4774f21"},
+    {file = "scipy-1.13.0.tar.gz", hash = "sha256:58569af537ea29d3f78e5abd18398459f195546bb3be23d16677fb26616cc11e"},
 ]
 
 [[package]]
 name = "screeninfo"
 version = "0.8.1"
 requires_python = ">=3.6.2,<4.0.0"
 summary = "Fetch location and size of physical screens."
@@ -1992,27 +1993,27 @@
 files = [
     {file = "screeninfo-0.8.1-py3-none-any.whl", hash = "sha256:e97d6b173856edcfa3bd282f81deb528188aff14b11ec3e195584e7641be733c"},
     {file = "screeninfo-0.8.1.tar.gz", hash = "sha256:9983076bcc7e34402a1a9e4d7dabf3729411fd2abb3f3b4be7eba73519cd2ed1"},
 ]
 
 [[package]]
 name = "selenium"
-version = "4.18.1"
+version = "4.19.0"
 requires_python = ">=3.8"
 summary = ""
 dependencies = [
     "certifi>=2021.10.8",
     "trio-websocket~=0.9",
     "trio~=0.17",
     "typing-extensions>=4.9.0",
     "urllib3[socks]<3,>=1.26",
 ]
 files = [
-    {file = "selenium-4.18.1-py3-none-any.whl", hash = "sha256:b24a3cdd2d47c29832e81345bfcde0c12bb608738013e53c781b211b418df241"},
-    {file = "selenium-4.18.1.tar.gz", hash = "sha256:a11f67afa8bfac6b77e148c987b33f6b14eb1cae4d352722a75de1f26e3f0ae2"},
+    {file = "selenium-4.19.0-py3-none-any.whl", hash = "sha256:5b4f49240d61e687a73f7968ae2517d403882aae3550eae2a229c745e619f1d9"},
+    {file = "selenium-4.19.0.tar.gz", hash = "sha256:d9dfd6d0b021d71d0a48b865fe7746490ba82b81e9c87b212360006629eb1853"},
 ]
 
 [[package]]
 name = "selenium-wire"
 version = "5.1.0"
 requires_python = ">=3.6"
 summary = "Extends Selenium to give you the ability to inspect requests made by the browser."
@@ -2034,24 +2035,14 @@
 ]
 files = [
     {file = "selenium-wire-5.1.0.tar.gz", hash = "sha256:b1cd4eae44d9959381abe3bb186472520d063c658e279f98555def3d4e6dd29b"},
     {file = "selenium_wire-5.1.0-py3-none-any.whl", hash = "sha256:fbf930d9992f8b6d24bb16b3e6221bab596a41f6ae7548270b7d5a92f3402622"},
 ]
 
 [[package]]
-name = "setuptools"
-version = "69.1.1"
-requires_python = ">=3.8"
-summary = "Easily download, build, install, upgrade, and uninstall Python packages"
-files = [
-    {file = "setuptools-69.1.1-py3-none-any.whl", hash = "sha256:02fa291a0471b3a18b2b2481ed902af520c69e8ae0919c13da936542754b4c56"},
-    {file = "setuptools-69.1.1.tar.gz", hash = "sha256:5c0806c7d9af348e6dd3777b4f4dbb42c7ad85b190104837488eab9a7c945cf8"},
-]
-
-[[package]]
 name = "sgmllib3k"
 version = "1.0.0"
 summary = "Py3k port of sgmllib."
 files = [
     {file = "sgmllib3k-1.0.0.tar.gz", hash = "sha256:7868fb1c8bfa764c1ac563d3cf369c381d1325d36124933a726f29fcdaa812e9"},
 ]
 
@@ -2214,20 +2205,20 @@
 files = [
     {file = "tabulate-0.9.0-py3-none-any.whl", hash = "sha256:024ca478df22e9340661486f85298cff5f6dcdba14f3813e8830015b9ed1948f"},
     {file = "tabulate-0.9.0.tar.gz", hash = "sha256:0095b12bf5966de529c0feb1fa08671671b3368eec77d7ef7ab114be2c068b3c"},
 ]
 
 [[package]]
 name = "threadpoolctl"
-version = "3.3.0"
+version = "3.4.0"
 requires_python = ">=3.8"
 summary = "threadpoolctl"
 files = [
-    {file = "threadpoolctl-3.3.0-py3-none-any.whl", hash = "sha256:6155be1f4a39f31a18ea70f94a77e0ccd57dced08122ea61109e7da89883781e"},
-    {file = "threadpoolctl-3.3.0.tar.gz", hash = "sha256:5dac632b4fa2d43f42130267929af3ba01399ef4bd1882918e92dbc30365d30c"},
+    {file = "threadpoolctl-3.4.0-py3-none-any.whl", hash = "sha256:8f4c689a65b23e5ed825c8436a92b818aac005e0f3715f6a1664d7c7ee29d262"},
+    {file = "threadpoolctl-3.4.0.tar.gz", hash = "sha256:f11b491a03661d6dd7ef692dd422ab34185d982466c49c8f98c8f716b5c93196"},
 ]
 
 [[package]]
 name = "tinytag"
 version = "1.10.1"
 requires_python = ">=2.7"
 summary = "Read music meta data and length of MP3, OGG, OPUS, MP4, M4A, FLAC, WMA and Wave files"
@@ -2244,39 +2235,39 @@
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "traitlets"
-version = "5.14.1"
+version = "5.14.2"
 requires_python = ">=3.8"
 summary = "Traitlets Python configuration system"
 files = [
-    {file = "traitlets-5.14.1-py3-none-any.whl", hash = "sha256:2e5a030e6eff91737c643231bfcf04a65b0132078dad75e4936700b213652e74"},
-    {file = "traitlets-5.14.1.tar.gz", hash = "sha256:8585105b371a04b8316a43d5ce29c098575c2e477850b62b848b964f1444527e"},
+    {file = "traitlets-5.14.2-py3-none-any.whl", hash = "sha256:fcdf85684a772ddeba87db2f398ce00b40ff550d1528c03c14dbf6a02003cd80"},
+    {file = "traitlets-5.14.2.tar.gz", hash = "sha256:8cdd83c040dab7d1dee822678e5f5d100b514f7b72b01615b26fc5718916fdf9"},
 ]
 
 [[package]]
 name = "trio"
-version = "0.24.0"
+version = "0.25.0"
 requires_python = ">=3.8"
 summary = "A friendly Python library for async concurrency and I/O"
 dependencies = [
-    "attrs>=20.1.0",
+    "attrs>=23.2.0",
     "cffi>=1.14; os_name == \"nt\" and implementation_name != \"pypy\"",
     "exceptiongroup; python_version < \"3.11\"",
     "idna",
     "outcome",
     "sniffio>=1.3.0",
     "sortedcontainers",
 ]
 files = [
-    {file = "trio-0.24.0-py3-none-any.whl", hash = "sha256:c3bd3a4e3e3025cd9a2241eae75637c43fe0b9e88b4c97b9161a55b9e54cd72c"},
-    {file = "trio-0.24.0.tar.gz", hash = "sha256:ffa09a74a6bf81b84f8613909fb0beaee84757450183a7a2e0b47b455c0cac5d"},
+    {file = "trio-0.25.0-py3-none-any.whl", hash = "sha256:e6458efe29cc543e557a91e614e2b51710eba2961669329ce9c862d50c6e8e81"},
+    {file = "trio-0.25.0.tar.gz", hash = "sha256:9b41f5993ad2c0e5f62d0acca320ec657fdb6b2a2c22b8c7aed6caf154475c4e"},
 ]
 
 [[package]]
 name = "trio-websocket"
 version = "0.11.1"
 requires_python = ">=3.7"
 summary = "WebSocket library for Trio"
@@ -2288,20 +2279,20 @@
 files = [
     {file = "trio-websocket-0.11.1.tar.gz", hash = "sha256:18c11793647703c158b1f6e62de638acada927344d534e3c7628eedcb746839f"},
     {file = "trio_websocket-0.11.1-py3-none-any.whl", hash = "sha256:520d046b0d030cf970b8b2b2e00c4c2245b3807853ecd44214acd33d74581638"},
 ]
 
 [[package]]
 name = "typing-extensions"
-version = "4.10.0"
+version = "4.11.0"
 requires_python = ">=3.8"
 summary = "Backported and Experimental Type Hints for Python 3.8+"
 files = [
-    {file = "typing_extensions-4.10.0-py3-none-any.whl", hash = "sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475"},
-    {file = "typing_extensions-4.10.0.tar.gz", hash = "sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb"},
+    {file = "typing_extensions-4.11.0-py3-none-any.whl", hash = "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"},
+    {file = "typing_extensions-4.11.0.tar.gz", hash = "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0"},
 ]
 
 [[package]]
 name = "tzdata"
 version = "2024.1"
 requires_python = ">=2"
 summary = "Provider of IANA time zone data"
@@ -2494,79 +2485,44 @@
     {file = "yarl-1.9.4-cp312-cp312-win_amd64.whl", hash = "sha256:a9bd00dc3bc395a662900f33f74feb3e757429e545d831eef5bb280252631984"},
     {file = "yarl-1.9.4-py3-none-any.whl", hash = "sha256:928cecb0ef9d5a7946eb6ff58417ad2fe9375762382f1bf5c55e61645f2c43ad"},
     {file = "yarl-1.9.4.tar.gz", hash = "sha256:566db86717cf8080b99b58b083b773a908ae40f06681e87e589a976faf8246bf"},
 ]
 
 [[package]]
 name = "yt-dlp"
-version = "2023.12.30"
+version = "2024.3.10"
 requires_python = ">=3.8"
 summary = "A youtube-dl fork with additional features and patches"
 dependencies = [
     "brotli; implementation_name == \"cpython\"",
     "brotlicffi; implementation_name != \"cpython\"",
     "certifi",
     "mutagen",
     "pycryptodomex",
     "requests<3,>=2.31.0",
     "urllib3<3,>=1.26.17",
     "websockets>=12.0",
 ]
 files = [
-    {file = "yt-dlp-2023.12.30.tar.gz", hash = "sha256:a11862e57721b0a0f0883dfeb5a4d79ba213a2d4c45e1880e9fd70f8e6570c38"},
-    {file = "yt_dlp-2023.12.30-py2.py3-none-any.whl", hash = "sha256:c00d9a71d64472ad441bcaa1ec0c3797d6e60c9f934f270096a96fe51657e7b3"},
+    {file = "yt_dlp-2024.3.10-py3-none-any.whl", hash = "sha256:bbe66b9a3aa23b6378ccca3ea20f5aadf385fa21a993513a105d73c827a86ed4"},
+    {file = "yt_dlp-2024.3.10.tar.gz", hash = "sha256:6e74cb14a69dbeb872c8ef4e0b8bbed2ee846ec633513cf3124a74c1faedc07b"},
 ]
 
 [[package]]
 name = "zeroconf"
-version = "0.131.0"
-requires_python = ">=3.7,<4.0"
+version = "0.132.0"
+requires_python = "<4.0,>=3.8"
 summary = "A pure python implementation of multicast DNS service discovery"
 dependencies = [
     "async-timeout>=3.0.0; python_version < \"3.11\"",
     "ifaddr>=0.1.7",
 ]
 files = [
-    {file = "zeroconf-0.131.0-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:3bc16228495e67ec990668970e815b341160258178c21b7716400c5e7a78976a"},
-    {file = "zeroconf-0.131.0-cp310-cp310-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:e0d1357940b590466bc72ac605e6ad3f7f05b2e1475b6896ec8e4c61e4d23034"},
-    {file = "zeroconf-0.131.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:434344df3037df08bad7422d5d36a415f30ddcc29ac1ad0cc0160b4976b782b5"},
-    {file = "zeroconf-0.131.0-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:c75bb2c1e472723067c7ec986ea510350c335bf8e73ad12617fc6a9ec765dc4b"},
-    {file = "zeroconf-0.131.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:18ff5b28e8935e5399fe47ece323e15816bc2ea4111417c41fc09726ff056cd2"},
-    {file = "zeroconf-0.131.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:3a49aaff22bc576680b4bcb3c7de896587f6ab4adaa788bedbc468dd0ad28cce"},
-    {file = "zeroconf-0.131.0-cp310-cp310-win32.whl", hash = "sha256:c3f0f87e47e4d5a9bcfcfc1ce29d0e9127a5cab63e839cc6f845c563f29d765c"},
-    {file = "zeroconf-0.131.0-cp310-cp310-win_amd64.whl", hash = "sha256:52b65e5eeacae121695bcea347cc9ad7da5556afcd3765c461e652ca3e8a84e9"},
-    {file = "zeroconf-0.131.0-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:6a041468c428622798193f0006831237aa749ee23e26b5b79e457618484457ef"},
-    {file = "zeroconf-0.131.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9a7f3b9a580af6bf74a7c435b80925dfeb065c987dffaf4d957d578366a80b2c"},
-    {file = "zeroconf-0.131.0-cp311-cp311-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:cc7a76103b03f47d2aa02206f74cc8b2120f4bac02936ccee5d6f29290f5bde5"},
-    {file = "zeroconf-0.131.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5d777b177cb472f7996b9d696b81337bfb846dbe454b8a34a8e33704d3a435b0"},
-    {file = "zeroconf-0.131.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:b843d5e2d2e576efeab59e382907bca1302f20eb33ee1a0a485e90d017b1088a"},
-    {file = "zeroconf-0.131.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:08eb87b0500ddc7c148fe3db3913e9d07d5495d756d7d75683f2dee8d7a09dc5"},
-    {file = "zeroconf-0.131.0-cp311-cp311-win32.whl", hash = "sha256:3b167b9e47f3fec8cc28a8f73a9e47c563ceb6681c16dcbe2c7d41e084cee755"},
-    {file = "zeroconf-0.131.0-cp311-cp311-win_amd64.whl", hash = "sha256:f74149a22a6a27e4c039f6477188dcbcb910acd60529dab5c114ff6265d40ba7"},
-    {file = "zeroconf-0.131.0-cp312-cp312-macosx_11_0_x86_64.whl", hash = "sha256:4865ef65b7eb7eee1a38c05bf7e91dd8182ef2afb1add65440f99e8dd43836d2"},
-    {file = "zeroconf-0.131.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:38bfd08c9191716d65e6ac52741442ee918bfe2db43993aa4d3b365966c0ab48"},
-    {file = "zeroconf-0.131.0-cp312-cp312-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:2389e3a61e99bf74796da7ebc3001b90ecd4e6286f392892b1211748e5b19853"},
-    {file = "zeroconf-0.131.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:194cf1465a756c3090e23ef2a5bd3341caa8d36eef486054daa8e532a4e24ac8"},
-    {file = "zeroconf-0.131.0-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:2907784c8c88795bf1b74cc9b6a4051e37a519ae2caaa7307787d466bc57884c"},
-    {file = "zeroconf-0.131.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:ce67d8dab4d88bcd1e5975d08235590fc5b9f31b2e2b7993ee1680810e67e56d"},
-    {file = "zeroconf-0.131.0-cp312-cp312-win32.whl", hash = "sha256:9dfa3d8827efffebec61b108162eeb76b0fe170a8379f9838be441f61b4557fd"},
-    {file = "zeroconf-0.131.0-cp312-cp312-win_amd64.whl", hash = "sha256:8642d374481d8cc7be9e364b82bcd11bda4a095c24c5f9f5754017a118496b77"},
-    {file = "zeroconf-0.131.0-pp310-pypy310_pp73-macosx_11_0_x86_64.whl", hash = "sha256:d4baa0450b9b0f1bd8acc25c2970d4e49e54726cbc437b81ffb65e5ffb6bd321"},
-    {file = "zeroconf-0.131.0-pp310-pypy310_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:3768ab13a8d7f0df85e40e766edd9e2aef28710a350dc4b15e1f2c5dd1326f00"},
-    {file = "zeroconf-0.131.0-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c10158396d6875f790bfb5600391d44edcbf52ac4d148e19baab3e8bb7825f76"},
-    {file = "zeroconf-0.131.0-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:28d906fc0779badb2183f5b20dbcc7e508cce53a13e63ba4d9477381c9f77463"},
-    {file = "zeroconf-0.131.0-pp38-pypy38_pp73-macosx_11_0_x86_64.whl", hash = "sha256:7c4235f45defd43bb2402ff8d3c7ff5d740e671bfd926852541c282ebef992bc"},
-    {file = "zeroconf-0.131.0-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:d08170123f5c04480bd7a82122b46c5afdb91553a9cef7d686d3fb9c369a9204"},
-    {file = "zeroconf-0.131.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1a57e0c4a94276ec690d2ecf1edeea158aaa3a7f38721af6fa572776dda6c8ad"},
-    {file = "zeroconf-0.131.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:0251034ed1d57eeb4e08782b22cc51e2455da7552b592bfad69a5761e69241c7"},
-    {file = "zeroconf-0.131.0-pp39-pypy39_pp73-macosx_11_0_x86_64.whl", hash = "sha256:34c3379d899361cd9d6b573ea9ac1eba53e2306eb28f94353b58c4703f0e74ae"},
-    {file = "zeroconf-0.131.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:d5d92987c3669edbfa9f911a8ef1c46cfd2c3e51971fc80c215f99212b81d4b1"},
-    {file = "zeroconf-0.131.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a613827f97ca49e2b4b6d6eb7e61a0485afe23447978a60f42b981a45c2b25fd"},
-    {file = "zeroconf-0.131.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:24b0a46c5f697cd6a0b27678ea65a3222b95f1804be6b38c6f5f1a7ce8b5cded"},
-    {file = "zeroconf-0.131.0.tar.gz", hash = "sha256:90c431e99192a044a5e0217afd7ca0ca9824af93190332e6f7baf4da5375f331"},
+    {file = "zeroconf-0.132.0-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:fb0a91b58b10d3a31b8324b2a8548e59c547a5c37055344c12d929f86c063d4e"},
+    {file = "zeroconf-0.132.0.tar.gz", hash = "sha256:e2dddb9b8e6a9de3c43f943d8547300e6bd49b2043fd719ae830cfe0f2908a5c"},
 ]
 
 [[package]]
 name = "zstandard"
 version = "0.22.0"
 requires_python = ">=3.8"
 summary = "Zstandard bindings for Python"
```

### Comparing `xklb-2.5.9/.github/LICENSE` & `xklb-2.6.1/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.5.9/.github/Windows.md` & `xklb-2.6.1/.github/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.5.9/.github/examples/extract.svg` & `xklb-2.6.1/.github/examples/extract.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.5.9/.github/examples/tubeadd.svg` & `xklb-2.6.1/.github/examples/tubeadd.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.5.9/.github/workflows/push.yaml` & `xklb-2.6.1/.github/workflows/push.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -12,21 +12,21 @@
       matrix:
         nv: [ {os: windows-latest, py: "3.10"}, {os: macos-latest, py: "3.11"}, {os: ubuntu-latest, py: "3.12"} ]
 
     runs-on: ${{ matrix.nv.os }}
     timeout-minutes: 20
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.nv.py }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.nv.py }}
 
-      - uses: FedericoCarboni/setup-ffmpeg@v2
+      - uses: FedericoCarboni/setup-ffmpeg@v3
 
       - name: Install Dependencies
         run: |
           python -m pip install pdm
 
       - name: Run missing modules test
         run: |
@@ -41,18 +41,18 @@
   publish:
     needs: test
     runs-on: ubuntu-latest
     timeout-minutes: 20
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.10"
 
       - name: Install pdm
         run: python -m pip install pdm
 
       - name: Build and publish
```

### Comparing `xklb-2.5.9/xklb/db_media.py` & `xklb-2.6.1/xklb/db_media.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse, os, sqlite3
+from collections.abc import Collection
 from datetime import datetime
 from pathlib import Path
-from typing import Collection, Dict, List, Optional
 
 from dateutil import parser
 
 from xklb import fs_extract
 from xklb.utils import consts, db_utils, iterables, nums, objects, processes, strings
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import log
@@ -43,15 +43,15 @@
 
     if "playlists" in tables:
         known_playlists.update(d["path"] for d in args.db.query("SELECT path from playlists"))
 
     return known_playlists
 
 
-def consolidate(v: dict) -> Optional[dict]:
+def consolidate(v: dict) -> dict | None:
     if v.get("title") in ("[Deleted video]", "[Private video]"):
         return None
 
     v = objects.flatten_dict(v, passthrough_keys=["automatic_captions", "http_headers", "subtitles"])
 
     upload_date = iterables.safe_unpack(
         v.pop("upload_date", None),
@@ -82,15 +82,15 @@
     )
     cv["path"] = iterables.safe_unpack(v.pop("path", None), v.pop("local_path", None), cv["webpath"])
     size_bytes = iterables.safe_unpack(v.pop("filesize_approx", None), v.pop("size", None))
     cv["size"] = 0 if not size_bytes else int(size_bytes)
     duration = v.pop("duration", None)
     cv["duration"] = 0 if not duration else int(duration)
     cv["time_uploaded"] = upload_date
-    cv["time_created"] = consts.now()
+    cv["time_created"] = iterables.safe_unpack(v.pop("time_created", None), consts.now())
     cv["time_modified"] = 0  # this should be 0 if the file has never been downloaded
     cv["time_deleted"] = 0
     cv["time_downloaded"] = 0
     language = v.pop("language", None)
     cv["tags"] = strings.combine(
         "language:" + language if language else None,
         v.pop("description", None),
@@ -109,15 +109,15 @@
     cv["longitude"] = iterables.safe_unpack(
         v.pop("longitude", None),
         v.pop("long", None),
         v.pop("lng", None),
     )
 
     # extractor_key should only be in playlist table
-    cv["extractor_id"] = v.pop("id", None)
+    cv["extractor_id"] = iterables.safe_unpack(v.pop("extractor_id", None), v.pop("id", None))
     cv["title"] = iterables.safe_unpack(v.pop("title", None), v.get("playlist_title"))
     cv["width"] = v.pop("width", None)
     cv["height"] = v.pop("height", None)
     fps = v.pop("fps", None)
     cv["fps"] = 0 if not fps else int(fps)
     cv["live_status"] = v.pop("live_status", None)
     cv["age_limit"] = iterables.safe_unpack(
@@ -166,29 +166,30 @@
 
     v = {
         k: v
         for k, v in v.items()
         if not (k.startswith(("_", "reblogged_")) or k in consts.MEDIA_KNOWN_KEYS or v is None)
     }
     if v != {}:
-        log.info("Extra media data %s", v)
+        log.debug("Extra media data %s", v)
         # breakpoint()
 
     return objects.dict_filter_bool(cv)
 
 
 def add(args, entry):
     if "path" not in entry:
         entry["path"] = entry.get("webpath")
     if not entry.get("path"):
         log.warning('Skipping insert: no "path" in entry %s', entry)
         return
 
     tags = entry.pop("tags", None) or ""
     chapters = entry.pop("chapters", None) or []
+    subtitles = entry.pop("subtitles", None) or []
     entry.pop("description", None)
 
     media_id = args.db.pop("select id from media where path = ?", [entry["path"]])
     try:
         if media_id:
             entry["id"] = media_id
 
@@ -200,20 +201,22 @@
         log.error("media_id %s: %s", media_id, entry)
         raise
 
     if tags:
         args.db["captions"].insert({"media_id": media_id, "time": 0, "text": tags}, alter=True)
     for chapter in chapters:
         args.db["captions"].insert({"media_id": media_id, **chapter}, alter=True)
+    if len(subtitles) > 0:
+        args.db["captions"].insert_all([{**d, "media_id": media_id} for d in subtitles], alter=True)
 
 
 def playlist_media_add(
     args,
     webpath: str,
-    info: Optional[dict] = None,
+    info: dict | None = None,
     error=None,
     unrecoverable_error=False,
 ) -> None:
     if not info:
         info = {"path": webpath}
 
     consolidated_entry = consolidate(info) or {}
@@ -226,30 +229,31 @@
     }
     add(args, entry)
 
 
 def download_add(
     args,
     webpath: str,
-    info: Optional[dict] = None,
+    info: dict | None = None,
     local_path=None,
     error=None,
     unrecoverable_error=False,
 ) -> None:
     if local_path and Path(local_path).exists():
         local_path = str(Path(local_path).resolve())
         fs_args = argparse.Namespace(
             profile=args.profile,
             scan_subtitles=args.profile == DBType.video,
             ocr=False,
             speech_recognition=False,
             delete_unplayable=False,
             check_corrupt=False,
         )
-        fs_tags = objects.dict_filter_bool(fs_extract.extract_metadata(fs_args, local_path), keep_0=False) or {}
+        fs_tags = fs_extract.extract_metadata(fs_args, local_path)
+        fs_tags = objects.dict_filter_bool(fs_tags, keep_0=False) or {}
         fs_extract.clean_up_temp_dirs()
     else:
         fs_tags = {"time_modified": consts.now()}
 
     if not info:  # not downloaded or already downloaded
         info = {"path": webpath}
 
@@ -289,23 +293,25 @@
     return modified_row_count
 
 
 def filter_args_sql(args, m_columns):
     return f"""
         {'and path like "http%"' if getattr(args, 'safe', False) else ''}
         {f'and path not like "{args.keep_dir}%"' if getattr(args, 'keep_dir', False) and Path(args.keep_dir).exists() else ''}
-        {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in m_columns and "deleted" not in (getattr(args, 'sort_groups_by',None) or '') and "time_deleted" not in args.where else ''}
+        {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in m_columns and "deleted" not in (getattr(args, 'sort_groups_by',None) or '') and "time_deleted" not in " ".join(args.where) else ''}
         {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
         {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
+        {'AND path not like "http%"' if args.local_media_only and 'time_downloaded' not in m_columns else ''}
+        {'AND path like "http%"' if args.online_media_only and 'time_downloaded' not in m_columns else ''}
         {'AND COALESCE(time_downloaded,0) = 0' if args.online_media_only and 'time_downloaded' in m_columns else ''}
         {'AND COALESCE(time_downloaded,1)!= 0 AND path not like "http%"' if args.local_media_only and 'time_downloaded' in m_columns else ''}
     """
 
 
-def get_dir_media(args, dirs: Collection, include_subdirs=False, limit=2_000) -> List[Dict]:
+def get_dir_media(args, dirs: Collection, include_subdirs=False, limit=2_000) -> list[dict]:
     if len(dirs) == 0:
         return processes.no_media_found()
 
     m_columns = db_utils.columns(args, "media")
 
     if include_subdirs:
         filter_paths = "AND (" + " OR ".join([f"path LIKE :subpath{i}" for i in range(len(dirs))]) + ")"
@@ -358,18 +364,18 @@
         log.debug("get_dir_media[0] %s", media[0:1])
 
     return media
 
 
 def get_sibling_media(args, media):
     if args.fetch_siblings in ("always", "all"):
-        dirs = set(str(Path(d["path"]).parent) + os.sep for d in media)
+        dirs = {str(Path(d["path"]).parent) + os.sep for d in media}
         media = get_dir_media(args, dirs)
     elif args.fetch_siblings == "each":
-        parents = set(str(Path(d["path"]).parent) + os.sep for d in media)
+        parents = {str(Path(d["path"]).parent) + os.sep for d in media}
         media = []
         for parent in parents:
             media.extend(get_dir_media(args, [parent], limit=1)[0:1])
     elif args.fetch_siblings == "if-audiobook":
         new_media = []
         seen = set()
         for d in media:
@@ -449,15 +455,15 @@
     else:
         media = natsorted(media, key=func_sort_key(alg), alg=NS_OPTS | ns.DEFAULT, reverse=reverse)
 
     log.debug("natsort[0] %s", media[0:1])
     return media
 
 
-def get_related_media(args, m: Dict) -> List[Dict]:
+def get_related_media(args, m: dict) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
     m_columns.update(rank=int)
 
     m = get(args, m["path"])
     words = set(
         iterables.conform(
             strings.extract_words(m.get(k)) for k in m if k in db_utils.config["media"]["search_columns"]
@@ -472,15 +478,15 @@
         exclude=args.exclude,
         flexible=True,
     )
     args.filter_bindings = {**args.filter_bindings, **search_bindings}
 
     select_sql = "\n        , ".join(args.select)
     limit_sql = "LIMIT " + str(args.limit - 1) if args.limit else ""
-    offset_sql = f"OFFSET {args.skip}" if args.skip and limit_sql else ""
+    offset_sql = f"OFFSET {args.offset}" if args.offset and limit_sql else ""
     query = f"""WITH m as (
             SELECT
                 SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                 , MIN(h.time_played) time_first_played
                 , MAX(h.time_played) time_last_played
                 , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
                 , {select_sql}
```

### Comparing `xklb-2.5.9/xklb/db_playlists.py` & `xklb-2.6.1/xklb/db_playlists.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os, sqlite3
 from datetime import datetime
-from typing import List, Optional
 
 from xklb.utils import consts, db_utils, iterables, nums, objects
 from xklb.utils.log_utils import log
 
 """
 playlists table
     profile = Type of extractor -- consts.DBType
@@ -92,27 +91,27 @@
         log.debug(e)
         return False
     if known is None:
         return False
     return True
 
 
-def get_parentpath_playlists_id(args, playlist_path) -> Optional[int]:
+def get_parentpath_playlists_id(args, playlist_path) -> int | None:
     try:
         known = args.db.pop(
             "select id from playlists where ? like path || '%' and path != ?",
             [str(playlist_path), str(playlist_path)],
         )
     except sqlite3.OperationalError as e:
         log.debug(e)
         return None
     return known
 
 
-def delete_subpath_playlists(args, playlist_path) -> Optional[int]:
+def delete_subpath_playlists(args, playlist_path) -> int | None:
     try:
         with args.db.conn:
             args.db.conn.execute(
                 f"""
                 DELETE from playlists
                 WHERE COALESCE(time_deleted, 0)=0
                     AND path LIKE ?
@@ -207,15 +206,15 @@
         try:
             with args.db.conn:
                 args.db.conn.execute("ALTER TABLE playlists ADD COLUMN hours_update_delay INTEGER DEFAULT 70")
         except Exception:
             raise e
 
 
-def get_all(args, cols="path, extractor_config", sql_filters=None, order_by="random()") -> List[dict]:
+def get_all(args, cols="path, extractor_config", sql_filters=None, order_by="random()") -> list[dict]:
     pl_columns = db_utils.columns(args, "playlists")
     if sql_filters is None:
         sql_filters = []
     if "time_deleted" in pl_columns:
         sql_filters.append("AND COALESCE(time_deleted,0) = 0")
     if "hours_update_delay" in pl_columns and not getattr(args, "force", False):
         sql_filters.append("AND (cast(STRFTIME('%s', 'now') as int) - time_modified) >= (hours_update_delay * 60 * 60)")
```

### Comparing `xklb-2.5.9/xklb/fs_extract.py` & `xklb-2.6.1/xklb/fs_extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,54 @@
 import argparse, json, math, os, sys
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from functools import partial
 from multiprocessing import TimeoutError as mp_TimeoutError
 from pathlib import Path
 from shutil import which
 from timeit import default_timer as timer
-from typing import Dict, List, Optional
 
 from xklb import db_media, db_playlists, usage
 from xklb.media import av, books
-from xklb.scripts import playlists, process_audio, sample_hash
-from xklb.utils import arg_utils, consts, db_utils, file_utils, iterables, nums, objects, path_utils
+from xklb.scripts import playlists, process_ffmpeg, process_image, sample_hash
+from xklb.utils import arg_utils, arggroups, consts, db_utils, file_utils, iterables, nums, objects, path_utils
 from xklb.utils.consts import SC, DBType
 from xklb.utils.log_utils import log
 
 
 def parse_args(action, usage):
     parser = argparse.ArgumentParser(prog="library " + action, usage=usage)
-
-    profiles = parser.add_argument_group()
-    profiles.add_argument(
-        "--audio",
-        "-A",
-        action="append_const",
-        dest="profiles",
-        const=DBType.audio,
-        help="Extract audio metadata",
-    )
-    profiles.add_argument(
-        "--filesystem",
-        "--fs",
-        "-F",
-        action="append_const",
-        dest="profiles",
-        const=DBType.filesystem,
-        help="Extract filesystem metadata",
-    )
-    profiles.add_argument(
-        "--video",
-        "-V",
-        action="append_const",
-        dest="profiles",
-        const=DBType.video,
-        help="Extract video metadata",
-    )
-    profiles.add_argument(
-        "--text",
-        "-T",
-        action="append_const",
-        dest="profiles",
-        const=DBType.text,
-        help="Extract text metadata",
-    )
-    profiles.add_argument(
-        "--image",
-        "-I",
-        action="append_const",
-        dest="profiles",
-        const=DBType.image,
-        help="Extract image metadata",
-    )
-    parser.add_argument("--scan-all-files", "-a", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--ext", action=arg_utils.ArgparseList)
+    arggroups.db_profiles(parser)
 
     parser.add_argument(
         "--io-multiplier",
         type=float,
         default=1.0,
         help="Especially useful for text, image, filesystem db types",
     )
     parser.add_argument("--ocr", "--OCR", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--speech-recognition", "--speech", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--scan-subtitles", "--scan-subtitle", action="store_true", help=argparse.SUPPRESS)
 
-    parser.add_argument("--delete-unplayable", action="store_true")
     parser.add_argument("--hash", action="store_true")
-    parser.add_argument("--process", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--move")
 
+    parser.add_argument("--process", action="store_true", help=argparse.SUPPRESS)
+    arggroups.process_ffmpeg(parser)
+    parser.add_argument("--delete-unplayable", action="store_true")
+
     parser.add_argument("--check-corrupt", "--check-corruption", action="store_true")
+    arggroups.media_check(parser)
+    parser.set_defaults(gap="0.10")
+
     parser.add_argument(
-        "--chunk-size",
-        type=float,
-        help="Duration to decode per segment (default 0.5 second). If set, recommended to use >0.1 seconds",
-        default=0.5,
-    )
-    parser.add_argument(
-        "--gap",
-        default="0.1",
-        help="Width between chunks to skip (default 10%%). Values greater than 1 are treated as number of seconds",
-    )
-    parser.add_argument(
-        "--delete-corrupt",
-        "--delete-corruption",
-        help="delete media that is more corrupt or equal to this threshold. Values greater than 1 are treated as number of seconds",
-    )
-    parser.add_argument(
-        "--full-scan-if-corrupt",
-        "--full-scan-if-corruption",
-        help="full scan as second pass if initial scan result more corruption or equal to this threshold. Values greater than 1 are treated as number of seconds",
+        "--force", "-f", action="store_true", help="Mark all subpath files as deleted if no files found"
     )
-    parser.add_argument("--full-scan", action="store_true")
-
-    parser.add_argument("--force", "-f", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     if action == SC.fsadd:
         parser.add_argument("paths", nargs="+")
     args = parser.parse_intermixed_args()
 
     if not args.profiles:
         args.profiles = [DBType.video]
 
@@ -119,31 +57,32 @@
 
     args.gap = nums.float_from_percent(args.gap)
     if args.delete_corrupt:
         args.delete_corrupt = nums.float_from_percent(args.delete_corrupt)
     if args.full_scan_if_corrupt:
         args.full_scan_if_corrupt = nums.float_from_percent(args.full_scan_if_corrupt)
 
-    if args.db:
-        args.database = args.db
+    args.split_longer_than = nums.human_to_seconds(args.split_longer_than)
+    args.min_split_segment = nums.human_to_seconds(args.min_split_segment)
+
     Path(args.database).touch()
     args.db = db_utils.connect(args)
 
     if hasattr(args, "paths"):
         args.paths = iterables.conform(args.paths)
     log.info(objects.dict_filter_bool(args.__dict__))
 
     if not which("ffprobe") and (DBType.audio in args.profiles or DBType.video in args.profiles):
         log.error("ffmpeg is not installed. Install it with your package manager.")
         raise SystemExit(3)
 
     return args, parser
 
 
-def extract_metadata(mp_args, path) -> Optional[Dict[str, int]]:
+def extract_metadata(mp_args, path) -> dict[str, int] | None:
     try:
         path.encode()
     except UnicodeEncodeError:
         log.error("Could not encode file path as UTF-8. Skipping %s", path)
         return None
 
     try:
@@ -166,20 +105,21 @@
         "time_downloaded": consts.APPLICATION_START,
         "time_deleted": 0,
     }
 
     ext = path.rsplit(".", 1)[-1].lower()
     is_scan_all_files = getattr(mp_args, "scan_all_files", False)
 
+    if media["type"] == "directory":
+        return None
+
     if not Path(path).exists():
         return media
 
-    if objects.is_profile(mp_args, DBType.audio) and (
-        ext in (consts.AUDIO_ONLY_EXTENSIONS | consts.VIDEO_EXTENSIONS) or is_scan_all_files
-    ):
+    if objects.is_profile(mp_args, DBType.audio) and (ext in consts.AUDIO_ONLY_EXTENSIONS or is_scan_all_files):
         media |= av.munge_av_tags(mp_args, path)
     elif objects.is_profile(mp_args, DBType.video) and (ext in consts.VIDEO_EXTENSIONS or is_scan_all_files):
         media |= av.munge_av_tags(mp_args, path)
 
     if not Path(path).exists():  # av.munge_av_tags might delete if unplayable or corruption exceeds threshold
         return media
 
@@ -196,29 +136,46 @@
             else:
                 media |= books.munge_book_tags_fast(path)
         except mp_TimeoutError:
             log.warning(f"Timed out trying to read file. {path}")
         else:
             log.debug(f"{timer()-start} {path}")
 
-    if getattr(mp_args, "hash", False):
-        # TODO: it would be better if this was saved to and checked against an external global file
+    if getattr(mp_args, "hash", False) and media["type"] != "directory" and media["size"] > 0:
         media["hash"] = sample_hash.sample_hash_file(path)
 
-    if getattr(mp_args, "process", False):
-        if objects.is_profile(mp_args, DBType.audio) and Path(path).suffix not in [".opus", ".mka"]:
-            path = media["path"] = process_audio.process_path(
-                path, split_longer_than=2160 if "audiobook" in path.lower() else None
-            )
-
     if getattr(mp_args, "move", False) and not file_utils.is_file_open(path):
         dest_path = bytes(Path(mp_args.move) / Path(path).relative_to(mp_args.playlist_path))
         dest_path = path_utils.clean_path(dest_path)
         file_utils.rename_move_file(path, dest_path)
-        media["path"] = dest_path
+        path = media["path"] = dest_path
+
+    if getattr(mp_args, "process", False):
+        if objects.is_profile(mp_args, DBType.audio) and Path(path).suffix not in [".opus", ".mka"]:
+            result = process_ffmpeg.process_path(
+                mp_args,
+                path,
+                split_longer_than=2160 if "audiobook" in path.lower() else None,
+            )
+            if result is None:
+                return None
+            path = media["path"] = str(result)
+        elif objects.is_profile(mp_args, DBType.video) and Path(path).suffix not in [".av1.mkv"]:
+            result = process_ffmpeg.process_path(mp_args, path)
+            if result is None:
+                return None
+            path = media["path"] = str(result)
+        elif objects.is_profile(mp_args, DBType.image) and Path(path).suffix not in [".avif", ".avifs"]:
+            result = process_image.process_path(
+                path,
+                delete_unplayable=getattr(mp_args, "delete_unplayable", False),
+            )
+            if result is None:
+                return None
+            path = media["path"] = str(result)
 
     return media
 
 
 def clean_up_temp_dirs():
     temp_subs_path = Path(consts.SUB_TEMP_DIR)
     if temp_subs_path.exists():
@@ -281,17 +238,17 @@
                     (*chunk_paths,),
                 )
                 modified_row_count += cursor.rowcount
 
     return modified_row_count
 
 
-def find_new_files(args, path) -> List[str]:
+def find_new_files(args, path) -> list[str]:
     if path.is_file():
-        scanned_set = set([str(path)])
+        scanned_set = {str(path)}
     else:
         for s in args.profiles:
             if getattr(DBType, s, None) is None:
                 msg = f"fs_extract for profile {s}"
                 raise NotImplementedError(msg)
 
         exts = args.ext
@@ -358,15 +315,15 @@
     except Exception as e:
         log.debug(e)
         new_files = list(scanned_set)
     else:
         new_files = list(scanned_set - existing_set)
 
         deleted_files = list(existing_set - scanned_set)
-        if not new_files and len(deleted_files) >= len(existing_set) and not args.force:
+        if not scanned_set and len(deleted_files) >= len(existing_set) and not args.force:
             print(f"[{path}] Path empty or device not mounted. Rerun with -f to mark all subpaths as deleted.")
             return []  # if path not mounted or all files deleted
         deleted_count = db_media.mark_media_deleted(args, deleted_files)
         if deleted_count > 0:
             print(f"[{path}] Marking", deleted_count, "orphaned metadata records as deleted")
 
     new_files.sort(key=len, reverse=True)
```

### Comparing `xklb-2.5.9/xklb/gdl_backend.py` & `xklb-2.6.1/xklb/gdl_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,16 +182,15 @@
                 if cls:
                     extr = cls.from_url(url)
                 else:
                     extr = self.extractor.find(url)
 
                 if extr:
                     job = self.__class__(extr, self)
-                    for webpath, info in job.run():
-                        yield (webpath, info)
+                    yield from job.run()
             else:
                 raise TypeError
 
     def handle_url(self, url, kwdict):
         self.dispatched = True
 
     def handle_queue(self, url, kwdict):
```

### Comparing `xklb-2.5.9/xklb/gdl_extract.py` & `xklb-2.6.1/xklb/gdl_extract.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,43 @@
 import argparse, sys
 from pathlib import Path
 
 from xklb import db_media, db_playlists, gdl_backend, usage
-from xklb.utils import arg_utils, consts, db_utils, iterables, objects, path_utils, processes
+from xklb.utils import arggroups, argparse_utils, consts, db_utils, iterables, objects, path_utils, processes
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library " + action,
         usage=usage,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
+    arggroups.extractor(parser)
+    arggroups.download(parser)
+    parser.set_defaults(download_archive=str(Path("~/.local/share/gallerydl.sqlite3").expanduser().resolve()))
 
-    parser.add_argument(
-        "--extractor-config",
-        "-extractor-config",
-        nargs=1,
-        action=arg_utils.ArgparseDict,
-        default={},
-        metavar="KEY=VALUE",
-        help="Add key/value pairs to override or extend default downloader configuration",
-    )
-    parser.add_argument("--download-archive", default="~/.local/share/gallerydl.sqlite3")
-    parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
-    parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
-    parser.add_argument(
-        "--force",
-        "-f",
-        action="store_true",
-        help="Fetch metadata for paths even if they are already in the media table",
-    )
-
-    parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true", help=argparse.SUPPRESS)
-
-    parser.add_argument("--timeout", "-T", help="Quit after x minutes")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     if action == SC.galleryadd:
-        parser.add_argument("--insert-only", action="store_true")
-        parser.add_argument("--insert-only-playlists", action="store_true")
-        parser.add_argument("playlists", nargs="*", default=arg_utils.STDIN_DASH, action=arg_utils.ArgparseArgsOrStdin)
+        parser.add_argument(
+            "playlists", nargs="*", default=argparse_utils.STDIN_DASH, action=argparse_utils.ArgparseArgsOrStdin
+        )
 
     args = parser.parse_intermixed_args()
     args.action = action
 
-    if args.db:
-        args.database = args.db
     if action == SC.galleryadd:
         Path(args.database).touch()
     args.db = db_utils.connect(args)
 
     if hasattr(args, "playlists"):
-        args.playlists = list(set(s.strip() for s in args.playlists))
+        args.playlists = list({s.strip() for s in args.playlists})
         if not args.no_sanitize:
             args.playlists = [path_utils.sanitize_url(args, p) for p in args.playlists]
         args.playlists = iterables.conform(args.playlists)
 
     processes.timeout(args.timeout)
 
     args.profile = consts.DBType.image
```

### Comparing `xklb-2.5.9/xklb/history.py` & `xklb-2.6.1/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.9/xklb/hn_extract.py` & `xklb-2.6.1/xklb/hn_extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse, asyncio, queue, sqlite3, threading
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import db_utils, objects, web
+from xklb.utils import arggroups, db_utils, objects, web
 from xklb.utils.log_utils import log
 
 """
 My understanding of aiohttp is stolen
 from ashish01's excellent https://github.com/ashish01/hn-data-dumps/blob/main/hn_async2.py
 
 MIT License
@@ -32,23 +32,19 @@
 SOFTWARE.
 """
 
 
 def parse_args(prog, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog, usage)
     parser.add_argument("--oldest", action="store_true")
-
-    parser.add_argument("--verbose", "-v", action="count", default=0)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
-
-    parser.add_argument("database")
+    arggroups.requests(parser)
+    arggroups.debug(parser)
+    arggroups.database(parser)
     args = parser.parse_args()
 
-    if args.db:
-        args.database = args.db
     Path(args.database).touch()
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
 
     return args
```

### Comparing `xklb-2.5.9/xklb/lb.py` & `xklb-2.6.1/xklb/lb.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         "siteadd": "Auto-scrape website data to SQLITE",
         "redditadd": "Create a reddit database; Add subreddits",
         "pushshift": "Convert pushshift data to reddit.db format (stdin)",
         "hnadd": "Create / Update a Hacker News database",
         "substack": "Backup substack articles",
         "tildes": "Backup tildes comments and topics",
         "places_import": "Import places of interest (POIs)",
+        "add_row": "Add arbitrary data to SQLITE",
     },
     "Update database subcommands": {
         "fsupdate": "Update local media",
         "tubeupdate": "Update online video media",
         "webupdate": "Update open-directory media",
         "galleryupdate": "Update online gallery media",
         "links_update": "Update a link-scraping database",
@@ -83,18 +84,21 @@
     },
     "Single database enrichment subcommands": {
         "dedupe_db": "Dedupe SQLITE tables",
         "dedupe_media": "Dedupe similar media",
         "merge_online_local": "Merge online and local data",
         "mpv_watchlater": "Import mpv watchlater files to history",
         "reddit_selftext": "Copy selftext links to media table",
+        "tabs_shuffle": "Randomize tabs.db a bit",
     },
     "Misc subcommands": {
         "export_text": "Export HTML files from SQLite databases",
-        "process_audio": "Shrink audio by converting to Opus format",
+        "process_audio": "Shrink audio by converting to Opus format (.mka)",
+        "process_image": "Shrink images by converting to AV1 image format (.avif)",
+        "process_video": "Shrink videos by converting to AV1 video format (.av1.mkv)",
         "dedupe_czkawka": "Process czkawka diff output",
         "nouns": "Unstructured text -> compound nouns (stdin)",
     },
 }
 
 
 def usage() -> str:
@@ -174,14 +178,15 @@
     add_parser(subparsers, "xklb.play_actions.filesystem", ["fs", "open"])
     add_parser(subparsers, "xklb.play_actions.listen", ["lt", "tubelisten", "tl"])
     add_parser(subparsers, "xklb.play_actions.read", ["books", "docs"])
     add_parser(subparsers, "xklb.play_actions.view", ["image", "see", "look"])
     add_parser(subparsers, "xklb.play_actions.watch", ["wt", "tubewatch", "tw", "entries"])
     add_parser(subparsers, "xklb.reddit_extract.reddit_add", ["ra"])
     add_parser(subparsers, "xklb.reddit_extract.reddit_update", ["ru"])
+    add_parser(subparsers, "xklb.scripts.add_row.add_row")
     add_parser(subparsers, "xklb.scripts.big_dirs.big_dirs", ["large-folders"])
     add_parser(subparsers, "xklb.scripts.block.block")
     add_parser(subparsers, "xklb.scripts.christen.christen")
     add_parser(subparsers, "xklb.scripts.cluster_sort.cluster_sort", ["cs"])
     add_parser(subparsers, "xklb.scripts.copy_play_counts.copy_play_counts")
     add_parser(subparsers, "xklb.scripts.dedupe_czkawka.czkawka_dedupe", ["dedupe-czkawka"])
     add_parser(subparsers, "xklb.scripts.dedupe_db.dedupe_db", ["dedupe-dbs"])
@@ -211,28 +216,30 @@
     add_parser(subparsers, "xklb.scripts.optimize_db.optimize_db", ["optimize"])
     add_parser(subparsers, "xklb.scripts.places_import.places_import")
     add_parser(subparsers, "xklb.scripts.playback_control.playback_next", ["next"])
     add_parser(subparsers, "xklb.scripts.playback_control.playback_now", ["now"])
     add_parser(subparsers, "xklb.scripts.playback_control.playback_pause", ["pause", "play"])
     add_parser(subparsers, "xklb.scripts.playback_control.playback_stop", ["stop"])
     add_parser(subparsers, "xklb.scripts.playlists.playlists", ["pl", "folders"])
-    add_parser(subparsers, "xklb.scripts.process_audio.process_audio")
+    add_parser(subparsers, "xklb.scripts.process_ffmpeg.process_ffmpeg", ["process-video", "process-audio"])
+    add_parser(subparsers, "xklb.scripts.process_image.process_image")
     add_parser(subparsers, "xklb.scripts.redownload.redownload", ["re-dl", "re-download"])
     add_parser(subparsers, "xklb.scripts.rel_mv.rel_mv", ["relmv", "mv-rel", "mvrel"])
     add_parser(subparsers, "xklb.scripts.sample_hash.sample_hash", ["hash", "hash-file"])
     add_parser(subparsers, "xklb.scripts.sample_compare.sample_compare", ["cmp"])
     add_parser(subparsers, "xklb.scripts.scatter.scatter")
     add_parser(subparsers, "xklb.scripts.search_db.search_db", ["s", "sdb", "search-dbs"])
     add_parser(subparsers, "xklb.scripts.streaming_tab_loader.streaming_tab_loader", ["surf"])
     add_parser(subparsers, "xklb.scripts.web_add.web_add", ["web-dir-add"])
     add_parser(subparsers, "xklb.scripts.web_update.web_update", ["web-dir-update"])
     add_parser(subparsers, "xklb.search.search", ["sc", "search-captions"])
     add_parser(subparsers, "xklb.site_extract.site_add", ["sa", "sql-site", "site-sql"])
     add_parser(subparsers, "xklb.tabs_actions.tabs", ["tb"])
     add_parser(subparsers, "xklb.tabs_extract.tabs_add")
+    add_parser(subparsers, "xklb.tabs_extract.tabs_shuffle")
     add_parser(subparsers, "xklb.tube_extract.tube_add", ["ta", "dladd", "da"])
     add_parser(subparsers, "xklb.tube_extract.tube_update", ["dlupdate", "tu"])
     add_parser(subparsers, "xklb.utils.devices.mount_stats", ["mu", "mount-usage"])
 
     parser.add_argument("--version", "-V", action="store_true")
 
     return parser
```

### Comparing `xklb-2.5.9/xklb/post_actions.py` & `xklb-2.6.1/xklb/post_actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         if src_size > dst_size:
             log.warning("Source (%s) is larger than destination (%s) %s", src_size_str, dst_size_str, diff_size_str)
         elif src_size < dst_size:
             log.warning("Source (%s) is smaller than destination (%s) %s", src_size_str, dst_size_str, diff_size_str)
         else:
             log.warning("Source and destination are the same size %s", src_size_str)
         if args.post_action.upper().startswith("ASK_"):
-            if getattr(args, "move_replace", False) or devices.confirm("Replace destination file?"):
+            if devices.clobber_confirm(args):
                 new_path.unlink()
                 new_path = str(shutil.move(media_file, keep_path))
             else:
                 return media_file
         else:
             raise
 
@@ -137,15 +137,24 @@
 
 
 def external_action(args, log_action, media_file, player_exit_code, player_process):
     player_exit_code_cmd = f"cmd{player_exit_code}"
     cmd = getattr(args, player_exit_code_cmd, None)
     if cmd:
         log_action(player_exit_code_cmd.upper())
-        if "{}" in cmd:
+        if cmd in ["pass", "mark-watched"]:
+            pass
+        elif cmd in ["soft-delete", "mark-deleted"]:
+            db_media.mark_media_deleted(args, media_file)
+        elif cmd in ["delete"]:
+            if media_file.startswith("http"):
+                db_media.mark_media_deleted(args, media_file)
+            else:
+                delete_media(args, media_file)
+        elif "{}" in cmd:
             processes.cmd_detach(media_file if s == "{}" else s for s in shlex.split(cmd))
         else:
             processes.cmd_detach(shlex.split(cmd), media_file)
     else:
         if 0 < player_exit_code and not args.ignore_errors and not (args.delete_unplayable and player_exit_code == 2):
             processes.player_exit(player_process)
```

### Comparing `xklb-2.5.9/xklb/readme.py` & `xklb-2.6.1/xklb/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.9/xklb/reddit_extract.py` & `xklb-2.6.1/xklb/reddit_extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import argparse
 import datetime as dt
 import sys
 from functools import partial
 from itertools import takewhile
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import TYPE_CHECKING, Any
 
 import prawcore
 
 from xklb import db_media, db_playlists, usage
-from xklb.utils import consts, db_utils, iterables, objects
+from xklb.utils import arggroups, consts, db_utils, iterables, objects
 from xklb.utils.log_utils import log
 
 PRAW_SETUP_INSTRUCTIONS = r"""
 You will need your Reddit user login info, client id, and secret.
 See https://www.reddit.com/wiki/api for client id / secret.
 
 Then create a praw.ini file:
@@ -50,27 +50,23 @@
     parser.add_argument("--limit", default=1000, type=int)
     parser.add_argument("--lookback", default=4, type=int, help="Number of days to look back")
     parser.add_argument("--praw-site", default="bot1")
 
     parser.add_argument("--subreddits", action="store_true")
     parser.add_argument("--redditors", action="store_true")
 
-    parser.add_argument("--verbose", "-v", action="count", default=0)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
-
-    parser.add_argument("database")
+    arggroups.debug(parser)
+    arggroups.database(parser)
     if action == "redditadd":
         parser.add_argument("paths", nargs="+")
     args = parser.parse_intermixed_args()
 
     if action == "redditadd":
         args.paths = iterables.conform(args.paths)
 
-    if args.db:
-        args.database = args.db
     Path(args.database).touch()
     args.db = db_utils.connect(args)
 
     try:
         import praw
 
         args.reddit = praw.Reddit(args.praw_site, config_interpolation="basic")
@@ -110,15 +106,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 
-def created_since(row, target_sec_utc: Optional[int]) -> bool:
+def created_since(row, target_sec_utc: int | None) -> bool:
     result = (not target_sec_utc) or (row.created_utc >= target_sec_utc)
     return result
 
 
 def legalize(val):
     import praw
 
@@ -127,28 +123,28 @@
     if isinstance(val, praw.models.reddit.poll.PollData):  # type: ignore
         d = val.__dict__
         d.pop("_reddit", None)
         return d
     return val
 
 
-def _parent_ids_interpreted(dct: Dict[str, Any]) -> Dict[str, Any]:
+def _parent_ids_interpreted(dct: dict[str, Any]) -> dict[str, Any]:
     if not dct.get("parent_id"):
         return dct
 
     prefix = dct["parent_id"][:3]
     dct["parent_clean_id"] = dct["parent_id"][3:]
     if prefix == "t1_":
         dct["parent_comment_id"] = dct["parent_clean_id"]
     elif prefix == "t3_":
         dct["parent_post_id"] = dct["parent_clean_id"]
     return dct
 
 
-def saveable(item) -> Dict[str, Any]:
+def saveable(item) -> dict[str, Any]:
     result = {k: legalize(v) for k, v in item.__dict__.items() if not k.startswith("_")}
     return _parent_ids_interpreted(result)
 
 
 def slim_post_data(d: dict, subreddit=None) -> dict:
     skip_domains = ["linktr.ee", "twitter.com", "t.me", "patreon", "onlyfans", "fans.ly", "file-upload", "file-link"]
     url = d.get("url")
```

### Comparing `xklb-2.5.9/xklb/rss_extract.py` & `xklb-2.6.1/xklb/rss_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.9/xklb/search.py` & `xklb-2.6.1/xklb/scripts/eda.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,200 +1,213 @@
-import argparse, textwrap
-from copy import deepcopy
-from itertools import groupby
-from typing import Tuple
-
-from xklb import db_media, usage
-from xklb.media import media_player, media_printer
-from xklb.utils import arg_utils, consts, db_utils, iterables, objects, printing, processes
-from xklb.utils.log_utils import log
+import argparse
 
+from xklb import usage
+from xklb.utils import arggroups, file_utils, nums
+from xklb.utils.consts import DEFAULT_FILE_ROWS_READ_LIMIT
+from xklb.utils.log_utils import log
+from xklb.utils.printing import print_df, print_series
 
-def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library search", usage=usage.search)
-    parser.add_argument("--open", "--play", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--duration", "-d", action="append", help=argparse.SUPPRESS)
-    parser.add_argument("--overlap", type=int, default=8, help=argparse.SUPPRESS)
-    parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--flexible-search", "--or", "--flex", action="store_true")
-    parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--sort", "-u", nargs="+", default=["path", "time"], help=argparse.SUPPRESS)
-    parser.add_argument("--table", action="store_true")
-    parser.add_argument("--limit", "-L", "-l", help=argparse.SUPPRESS)
 
+def parse_args():
+    parser = argparse.ArgumentParser(description="Perform EDA on one or more files", usage=usage.eda)
     parser.add_argument("--print", "-p", default="p", const="p", nargs="?", help=argparse.SUPPRESS)
-    parser.add_argument("--cols", "-cols", "-col", nargs="*", help="Include a column when printing")
-    parser.add_argument("--action", default="search", help=argparse.SUPPRESS)
-    parser.add_argument("--folder", action="store_true", help="Experimental escape hatch to open folder")
+
+    parser.add_argument("--groupby", "--group-by", "-g", action="store_true")
+    arggroups.table_like(parser)
+
+    parser.add_argument("--sort", "-u", default="random()")
+    parser.add_argument("--repl", "-r", action="store_true")
+    arggroups.debug(parser)
+
     parser.add_argument(
-        "--folder-glob",
-        "--folderglob",
-        type=int,
-        default=False,
-        const=10,
-        nargs="?",
-        help="Experimental escape hatch to open a folder glob limited to x number of files",
+        "paths",
+        metavar="path",
+        nargs="+",
+        help="path to one or more files",
     )
+    args = parser.parse_args()
 
-    parser.add_argument("--ignore-errors", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--online-media-only", "--online", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--local-media-only", "--local", action="store_true", help=argparse.SUPPRESS)
-
-    parser.add_argument("--loop", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--override-player", "--player", "-player", help=argparse.SUPPRESS)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
-
-    parser.add_argument("database")
-    parser.add_argument("search", nargs="*")
-    args = parser.parse_intermixed_args()
-    args.include += args.search
-
-    if args.cols:
-        args.cols = list(iterables.flatten([s.split(",") for s in args.cols]))
-
-    sort = [arg_utils.override_sort(s) for s in args.sort]
-    sort = "\n        , ".join(sort)
-    args.sort = sort.replace(",,", ",")
-
-    if args.db:
-        args.database = args.db
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
+    if args.end_row.lower() in ("inf", "none", "all"):
+        args.end_row = None
+    else:
+        args.end_row = int(args.end_row)
 
     return args
 
 
-def printer(args, captions) -> None:
-    captions = iterables.list_dict_filter_bool(captions)
-    if not captions:
-        processes.no_media_found()
-
-    tbl = deepcopy(captions)
-    printing.col_hhmmss(tbl, "time")
-
-    if args.print == "p":
-        print(f"{len(captions)} captions")
-        for path, path_group in groupby(tbl, key=lambda x: x["path"]):
-            path_group = list(path_group)
-            title = path_group[0].get("title")
-            print(" - ".join(iterables.concat(title, path)))
-            for caption in path_group:
-                for line in textwrap.wrap(caption["text"], subsequent_indent=" " * 9, initial_indent=f"{caption['time']} ", width=consts.TERMINAL_SIZE.columns - 2):  # type: ignore
-                    print(line)
-            print()
+def df_column_values(df, column_name) -> dict:
+    total = len(df)
+
+    null = df[column_name].isnull().sum()
+    zero = (df[column_name] == 0).sum()
+    empty = (df[column_name] == "").sum()
+    values = total - empty - zero - null
+
+    return {
+        "values_count": values,
+        "null_count": null,
+        "zero_count": zero,
+        "empty_string_count": empty,
+        "column": column_name,
+        "null": f"{null} ({nums.percent(null, total):.1f}%)",
+        "zero": f"{zero} ({nums.percent(zero, total):.1f}%)",
+        "empty_string": f"{empty} ({nums.percent(empty, total):.1f}%)",
+        "values": f"{values} ({nums.percent(values, total):.1f}%)",
+    }
+
+
+def print_info(args, df):
+    import pandas as pd
+
+    if df.shape == (0, 0):
+        print(f"Table [{df.name}] empty")
+        return
+
+    if args.end_row is None:
+        partial_dataset_msg = ""
+    elif args.end_row == DEFAULT_FILE_ROWS_READ_LIMIT:
+        partial_dataset_msg = f"(limited by default --end-row {args.end_row})"
     else:
-        media_printer.media_printer(args, captions, units="captions")
+        partial_dataset_msg = f"(limited by --end-row {args.end_row})"
+    if args.end_row is not None and args.end_row not in df.shape:
+        partial_dataset_msg = ""
+    print("### Shape")
+    print()
+    print(df.shape, partial_dataset_msg)
+    print()
+
+    print("### Sample of rows")
+    if len(df) > 6:
+        print_df(pd.concat([df.head(3), df.tail(3)]))
+    else:
+        print_df(df.head(6))
 
+    print("### Summary statistics")
+    print_df(df.describe())
 
-def construct_query(args) -> Tuple[str, dict]:
-    m_columns = db_utils.columns(args, "media")
-    c_columns = db_utils.columns(args, "captions")
-    args.filter_sql = []
-    args.filter_bindings = {}
-
-    args.filter_sql.extend([" and " + w for w in args.where])
-
-    table = "captions"
-    if args.db["captions"].detect_fts():
-        if args.include:
-            args.table, search_bindings = db_utils.fts_search_sql(
-                "captions",
-                fts_table=args.db["captions"].detect_fts(),
-                include=args.include,
-                exclude=args.exclude,
-                flexible=args.flexible_search,
-            )
-            args.filter_bindings = {**args.filter_bindings, **search_bindings}
-            c_columns = {**c_columns, "rank": int}
-        elif args.exclude:
-            db_utils.construct_search_bindings(args, ["text"])
-    else:
-        db_utils.construct_search_bindings(args, ["text"])
+    converted = df.convert_dtypes()
+    same_dtypes = []
+    diff_dtypes = []
+    for col in df.columns:
+        if df.dtypes[col] == converted.dtypes[col]:
+            same_dtypes.append((col, df.dtypes[col]))
+        else:
+            diff_dtypes.append((col, df.dtypes[col], converted.dtypes[col]))
+    if len(same_dtypes) > 0:
+        print("### Pandas columns with 'original' dtypes")
+        same_dtypes = pd.DataFrame(same_dtypes, columns=["column", "dtype"])
+        print_df(same_dtypes.set_index("column"))
+    if len(diff_dtypes) > 0:
+        print("### Pandas columns with 'converted' dtypes")
+        diff_dtypes = pd.DataFrame(diff_dtypes, columns=["column", "original_dtype", "converted_dtype"])
+        print_df(diff_dtypes.set_index("column"))
+
+    if len(df) > 15:
+        numeric_columns = df.select_dtypes("number").columns.to_list()
+        if numeric_columns:
+            print("### Numerical columns")
+            print()
+            print("#### Bins")
+            print()
+            for col in numeric_columns:
+                try:
+                    bins = pd.cut(df[col], bins=6)
+                    print_df(bins.value_counts().sort_index())
+                except TypeError:  # putmask: first argument must be an array
+                    log.warning("Could not calculate bins for col %s", col)
+
+        categorical_columns = [s for s in df.columns.to_list() if s not in numeric_columns]
+        if categorical_columns:
+            high_cardinality_cols = set()
+            low_cardinality_cols = set()
 
-    cols = args.cols or ["path", "text", "time", "rank", "title"]
-    args.select = [c for c in cols if c in {**c_columns, **m_columns, **{"*": "Any"}}]
+            print("### Categorical columns")
+            print()
+            for col in categorical_columns:
+                vc = df[col].value_counts()
+                vc = vc[vc > (len(df) * 0.005)]
+                if len(vc) > 0:
+                    low_cardinality_cols.add(col)
+                    print(f"#### common values of {col} column")
+                    vc = pd.DataFrame({"Count": vc, "Percentage": (vc / len(df)) * 100}).sort_values(
+                        by="Count", ascending=False
+                    )
+                    print_df(vc.head(30))
+
+                    if args.groupby:
+                        groups = df.groupby(col).size()
+                        groups = groups[groups >= 15]
+                        if len(groups) > 0:
+                            print(f"#### group by {col}")
+                            print_df(df[df[col].isin(groups.index)].groupby(col).describe())
+
+                unique_count = df[col].nunique()
+                if unique_count >= (len(df) * 0.2):
+                    high_cardinality_cols.add(col)
+
+            med_cardinality_cols = low_cardinality_cols.intersection(high_cardinality_cols)
+            low_cardinality_cols = low_cardinality_cols - med_cardinality_cols
+            high_cardinality_cols = high_cardinality_cols - med_cardinality_cols
+
+            if high_cardinality_cols:
+                print("#### High cardinality (many unique values)")
+                print_series(high_cardinality_cols)
+            if med_cardinality_cols:
+                print("#### Medium cardinality (many unique but also many similar values)")
+                print_series(med_cardinality_cols)
+            if low_cardinality_cols:
+                print("#### Low cardinality (many similar values)")
+                print_series(low_cardinality_cols)
+
+    print("### Missing values")
+    print()
+    nan_col_sums = df.isna().sum()
+    print(
+        f"{nan_col_sums.sum():,} nulls/NaNs",
+        f"({(nan_col_sums.sum() / (df.shape[0] * df.shape[1])):.1%} dataset values missing)",
+    )
+    print()
 
-    select_sql = "\n        , ".join(args.select)
-    limit_sql = "LIMIT " + str(args.limit) if args.limit else ""
-    query = f"""WITH c as (
-        SELECT id, * FROM {table}
-        WHERE 1=1
-            {db_media.filter_args_sql(args, c_columns)}
+    if nan_col_sums.sum():
+        no_nas = df.columns[df.notnull().all()]
+        if len(no_nas) > 0:
+            print(f"#### {len(no_nas)} columns with no missing values")
+            print_series(no_nas)
+
+        all_nas = df.columns[df.isnull().all()]
+        if len(all_nas) > 0:
+            print(f"#### {len(all_nas)} columns with all missing values")
+            print_series(all_nas)
+
+        print("#### Value stats")
+        column_report = pd.DataFrame(df_column_values(df, col) for col in df.columns).set_index("column")
+        column_report = column_report.sort_values(["empty_string_count", "zero_count", "null_count"])
+        print_df(column_report[["values", "null", "zero", "empty_string"]])
+
+
+def file_eda(args, path):
+    dfs = file_utils.read_file_to_dataframes(
+        path,
+        table_name=args.table_name,
+        table_index=args.table_index,
+        start_row=args.start_row,
+        end_row=args.end_row,
+        order_by=args.sort,
+        encoding=args.encoding,
+        mimetype=args.mimetype,
     )
-    SELECT
-        {select_sql}
-    FROM c
-    JOIN media m on m.id = c.media_id
-    WHERE 1=1
-        {" ".join(args.filter_sql)}
-    ORDER BY 1=1
-        , {args.sort}
-    {limit_sql}
-    """
-
-    return query, args.filter_bindings
-
-
-def merge_captions(args, captions):
-    def get_end(caption):
-        return caption["time"] + (len(caption["text"]) / 4.2 / 220 * 60)
-
-    merged_captions = []
-    for path, group in groupby(
-        captions,
-        key=lambda x: x["path"],
-    ):  # group by only does contiguous items with the same key
-        group = list(group)
-        merged_group = {"path": path, "title": group[0]["title"], "time": group[0]["time"], "end": get_end(group[0]), "text": group[0]["text"]}  # type: ignore
-        for i in range(1, len(group)):
-            end = get_end(group[i])
-
-            if (
-                abs(group[i]["time"] - merged_group["end"]) <= args.overlap  # type: ignore
-                or abs(group[i]["time"] - merged_group["time"]) <= args.overlap  # type: ignore
-            ):
-                merged_group["end"] = end
-                if group[i]["text"] not in merged_group["text"]:  # type: ignore
-                    merged_group["text"] += ". " + group[i]["text"]  # type: ignore
-            else:
-                merged_captions.append(merged_group)
-                merged_group = {
-                    "path": path,
-                    "time": group[i]["time"],  # type: ignore
-                    "end": end,
-                    "text": group[i]["text"],  # type: ignore
-                }
-        merged_captions.append(merged_group)
+    if getattr(args, "repl", False):
+        breakpoint()
 
-    return merged_captions
+    for df in dfs:
+        print(f"## {path}:{df.name}")
+        print_info(args, df)
 
 
-def search() -> None:
+def eda():
     args = parse_args()
-    query, bindings = construct_query(args)
-    captions = list(args.db.query(query, bindings))
-    merged_captions = merge_captions(args, captions)
-
-    if args.open:
-        pl = media_player.MediaPrefetcher(args, merged_captions)
-        pl.fetch()
-        while pl.remaining:
-            d = pl.get_m()
-            if d:
-                print(d["text"])
-                m = args.db.pop_dict("select * from media where path = ?", [d["path"]])
-                m["player"].extend([f'--start={d["time"] - 2}', f'--end={int(d["end"] + 1.5)}'])
-                r = media_player.single_player(args, m)
-                if r.returncode != 0:
-                    log.warning("Player exited with code %s", r.returncode)
-                    if args.ignore_errors:
-                        return
-                    else:
-                        raise SystemExit(r.returncode)
-    else:
-        printer(args, merged_captions)
+    for path in args.paths:
+        file_eda(args, path)
 
 
 if __name__ == "__main__":
-    search()
+    eda()
```

### Comparing `xklb-2.5.9/xklb/site_extract.py` & `xklb-2.6.1/xklb/site_extract.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 import argparse, json
 from collections import defaultdict
 from io import StringIO
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arg_utils, consts, db_utils, iterables, objects, web
+from xklb.utils import arg_utils, arggroups, consts, db_utils, iterables, objects, web
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library site-add", usage=usage.siteadd)
-    parser.add_argument("--auto-pager", "--autopager", action="store_true")
-    parser.add_argument("--poke", action="store_true")
-    parser.add_argument("--chrome", action="store_true")
+    arggroups.selenium(parser)
+    parser.set_defaults(selenium=True)
+
     parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
-    parser.add_argument("--file", "-f", help="File with one URL per line")
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
 
-    parser.add_argument("database")
-    parser.add_argument("paths", nargs="+")
+    arggroups.debug(parser)
+    arggroups.database(parser)
+    arggroups.paths_or_stdin(parser)
     args = parser.parse_intermixed_args()
 
-    if args.db:
-        args.database = args.db
-
     Path(args.database).touch()
     args.db = db_utils.connect(args)
 
     log.info(objects.dict_filter_bool(args.__dict__))
 
     return args
```

### Comparing `xklb-2.5.9/xklb/tabs_actions.py` & `xklb-2.6.1/xklb/scripts/open_links.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,210 +1,215 @@
-import argparse, math, webbrowser
+import argparse, shlex, webbrowser
 from pathlib import Path
 from time import sleep
-from typing import Dict, List, Tuple
 
-from xklb import history, usage
+from xklb import db_media, history, usage
 from xklb.media import media_printer
-from xklb.utils import arg_utils, consts, db_utils, iterables, objects, processes
+from xklb.utils import arg_utils, arggroups, consts, db_utils, iterables, objects, processes, web
 from xklb.utils.log_utils import log
 
 
-def parse_args(action) -> argparse.Namespace:
+def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        prog="library tabs",
+        prog="library open-links",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        usage=usage.tabs,
+        usage=usage.open_links,
     )
+    arggroups.sql_fs(parser)
 
-    parser.add_argument("--sort", "-u", nargs="+")
-    parser.add_argument("--where", "-w", nargs="+", action="extend", default=[])
-    parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[])
-    parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[])
-    parser.add_argument("--exact", action="store_true")
-    parser.add_argument("--print", "-p", default="", const="p", nargs="?")
-    parser.add_argument("--cols", "-cols", "-col", nargs="*", help="Include a column when printing")
-    parser.add_argument(
-        "--delete",
-        "--remove",
-        "--erase",
-        "--rm",
-        "-rm",
-        action="store_true",
-        help="Delete matching rows",
-    )
-    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue")
-    parser.add_argument("--skip")
+    parser.add_argument("--path", action="store_true")
+    parser.add_argument("--title", "-S", action="store_true")
+    parser.add_argument("--title-prefix", "--prefix", nargs="+", action="extend")
+
+    parser.add_argument("--online-media-only", "--online", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--local-media-only", "--local", action="store_true", help=argparse.SUPPRESS)
+
+    parser.add_argument("--category", "-c")
+    arggroups.capability_delete(parser)
 
-    parser.add_argument("--db", "-db")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.operation_cluster(parser)
+    arggroups.operation_related(parser)
 
-    parser.add_argument("database")
+    parser.add_argument("--browser")
+    arggroups.debug(parser)
+
+    arggroups.database(parser)
     parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
-    args.action = action
+    args.action = consts.SC.open_links
+    args.defaults = []
+
+    arg_utils.parse_args_limit(args)
 
     args.include += args.search
     if args.include == ["."]:
         args.include = [str(Path().cwd().resolve())]
 
-    if args.db:
-        args.database = args.db
+    if not args.title_prefix:
+        args.title_prefix = ["https://www.google.com/search?q=%"]
+    args.title_prefix = [s if "%" in s else s + "%" for s in args.title_prefix]
+
+    if args.browser:
+        args.browser = shlex.split(args.browser)
 
     if args.sort:
         args.sort = [arg_utils.override_sort(s) for s in args.sort]
         args.sort = " ".join(args.sort)
 
     if args.cols:
         args.cols = list(iterables.flatten([s.split(",") for s in args.cols]))
 
     if args.delete:
         args.print += "d"
 
-    if args.db:
-        args.database = args.db
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
 
     return args
 
 
-def tabs_include_sql(x) -> str:
+def links_include_sql(x) -> str:
     return f"""and (
     path like :include{x}
-    OR category like :include{x}
-    OR frequency like :include{x}
+    OR title like :include{x}
 )"""
 
 
-def tabs_exclude_sql(x) -> str:
+def links_exclude_sql(x) -> str:
     return f"""and (
     path not like :exclude{x}
-    AND category not like :exclude{x}
-    AND frequency not like :exclude{x}
+    AND title not like :exclude{x}
 )"""
 
 
-def construct_tabs_query(args) -> Tuple[str, dict]:
+def construct_links_query(args) -> tuple[str, dict]:
+    m_columns = db_utils.columns(args, "media")
+
     args.filter_sql = []
     args.filter_bindings = {}
 
     args.filter_sql.extend([" and " + w for w in args.where])
 
     for idx, inc in enumerate(args.include):
-        args.filter_sql.append(tabs_include_sql(idx))
+        args.filter_sql.append(links_include_sql(idx))
         if args.exact:
             args.filter_bindings[f"include{idx}"] = inc
         else:
             args.filter_bindings[f"include{idx}"] = "%" + inc.replace(" ", "%").replace("%%", " ") + "%"
     for idx, exc in enumerate(args.exclude):
-        args.filter_sql.append(tabs_exclude_sql(idx))
+        args.filter_sql.append(links_exclude_sql(idx))
         if args.exact:
             args.filter_bindings[f"exclude{idx}"] = exc
         else:
             args.filter_bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
 
-    LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
-    OFFSET = f"OFFSET {args.skip}" if args.skip else ""
+    if args.category:
+        args.filter_sql.append("AND category like :category")
+        if args.exact:
+            args.filter_bindings[f"category"] = args.category
+        else:
+            args.filter_bindings[f"category"] = "%" + args.category.replace(" ", "%").replace("%%", " ") + "%"
+
+    limit_sql = "LIMIT " + str(args.limit) if args.limit and not args.cluster_sort else ""
+    offset_sql = f"OFFSET {args.offset}" if args.offset and limit_sql else ""
+
+    args.select = ["path"]
+    if args.cols:
+        args.select.extend(args.cols)
+    for s in ["title", "hostname", "category"]:
+        if s in m_columns:
+            args.select.append(s)
 
     query = f"""WITH m as (
             SELECT
-                path
-                , frequency
+                {', '.join(args.select) if args.select else ''}
                 , COALESCE(MAX(h.time_played), 0) time_last_played
                 , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                 , time_deleted
-                , hostname
-                , category
             FROM media
             LEFT JOIN history h on h.media_id = media.id
             WHERE COALESCE(time_deleted, 0)=0
             GROUP BY media.id
         )
-        SELECT path
-        , frequency
+        SELECT
+        {', '.join(args.select) if args.select else ''}
         {", time_last_played" if args.print else ''}
-        , CASE
-            WHEN frequency = 'daily' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+1 Day', '-5 minutes' )) as int)
-            WHEN frequency = 'weekly' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+7 Days', '-5 minutes' )) as int)
-            WHEN frequency = 'monthly' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+1 Month', '-5 minutes' )) as int)
-            WHEN frequency = 'quarterly' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+3 Months', '-5 minutes' )) as int)
-            WHEN frequency = 'yearly' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+1 Year', '-5 minutes' )) as int)
-        END time_valid
-        {', ' + ', '.join(args.cols) if args.cols else ''}
     FROM m
     WHERE 1=1
+        AND COALESCE(time_deleted, 0)=0
+        {'AND path like "http%"' if args.online_media_only else ''}
+        {'AND path not like "http%"' if args.local_media_only else ''}
         {" ".join(args.filter_sql)}
-        {f"and time_valid < {consts.today_stamp()}" if not args.print else ''}
     ORDER BY 1=1
         {', ' + args.sort if args.sort else ''}
-        {', time_last_played, time_valid, path' if args.print else ''}
         , play_count
-        , frequency = 'daily' desc
-        , frequency = 'weekly' desc
-        , frequency = 'monthly' desc
-        , frequency = 'quarterly' desc
-        , frequency = 'yearly' desc
-        , ROW_NUMBER() OVER ( PARTITION BY
-            play_count
-            , frequency
-            , hostname
-            , category
-        ) -- prefer to spread hostname, category over time
+        {', ROW_NUMBER() OVER ( PARTITION BY hostname )' if 'hostname' in m_columns else ''}
+        {', ROW_NUMBER() OVER ( PARTITION BY category )' if 'category' in m_columns else ''}
         , random()
-    {LIMIT} {OFFSET}
+    {limit_sql} {offset_sql}
     """
 
     return query, args.filter_bindings
 
 
-def play(args, m: Dict) -> None:
-    media_file = m["path"]
+def play(args, path, url) -> None:
+    if args.browser:
+        processes.cmd(*args.browser, url)
+    else:
+        webbrowser.open(url, 2, autoraise=False)
+    history.add(args, [path], time_played=consts.today_stamp(), mark_done=True)
 
-    webbrowser.open(media_file, 2, autoraise=False)
-    history.add(args, [media_file], time_played=consts.today_stamp(), mark_done=True)
 
+def make_souffle(args, media):
+    pan = []
 
-def frequency_filter(counts, media: List[Dict]) -> List[dict]:
-    mapper = {
-        "daily": 1,
-        "weekly": 7,
-        "monthly": 30,
-        "quarterly": 91,
-        "yearly": 365,
-    }
-    filtered_media = []
-    for freq, freq_count in counts:
-        num_days = mapper.get(freq, 365)
-        num_tabs = max(1, math.ceil(freq_count / num_days))
-        log.debug(f"freq_count {freq_count} / num_days {num_days} = num_tabs {num_tabs}")
+    urls = set()
+    for m in media:
+        m_urls = set()
+        if args.title:
+            for engine in args.title_prefix:
+                suffix = m.get("title") or m["path"]
+                m_urls.add(suffix if suffix.startswith("http") else web.construct_search(engine, suffix))
+
+        if not args.title or args.path:
+            if not m["path"].startswith("http"):
+                for engine in args.title_prefix:
+                    m_urls.add(web.construct_search(engine, m["path"]))
+            else:
+                m_urls.add(m["path"])
 
-        filtered_media.extend([m for m in media if m["frequency"] == freq][:num_tabs])
+        pan.extend([{**m, "url": url} for url in m_urls if url not in urls])
+        urls |= m_urls
 
-    return filtered_media
+    return pan
 
 
-def open_tabs(args, media):
-    for m in media:
-        play(args, m)
-        if len(media) >= consts.MANY_LINKS:
-            sleep(0.3)
+def open_links() -> None:
+    args = parse_args()
+    history.create(args)
 
+    query, bindings = construct_links_query(args)
+    media = list(args.db.query(query, bindings))
 
-def tabs() -> None:
-    args = parse_args(consts.SC.tabs)
-    history.create(args)
+    if args.related >= consts.RELATED:
+        media = db_media.get_related_media(args, media[0])
 
-    query, bindings = construct_tabs_query(args)
+    if args.cluster_sort:
+        from xklb.scripts.cluster_sort import cluster_dicts
+
+        media = cluster_dicts(args, media)[: args.limit]
+
+    media = make_souffle(args, media)
 
     if args.print:
-        media_printer.printer(args, query, bindings)
+        media_printer.media_printer(args, media)
         return
 
-    media = list(args.db.query(query, bindings))
     if not media:
         processes.no_media_found()
 
-    counts = args.db.execute("select frequency, count(*) from media group by 1").fetchall()
-    media = frequency_filter(counts, media)
+    for m in media:
+        play(args, m["path"], m["url"])
 
-    open_tabs(args, media)
+        sleep(0.1)
+        if len(media) >= consts.MANY_LINKS:
+            sleep(0.7)
```

### Comparing `xklb-2.5.9/xklb/tube_backend.py` & `xklb-2.6.1/xklb/tube_backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import json, sqlite3, sys
+import json, sys
 from copy import deepcopy
 from pathlib import Path
+from pprint import pprint
 from types import ModuleType
-from typing import Dict, List, Optional, Tuple
 
 from xklb import db_media, db_playlists
 from xklb.data.dl_config import (
     prefix_unrecoverable_errors,
     yt_meaningless_errors,
     yt_recoverable_errors,
     yt_unrecoverable_errors,
@@ -24,15 +24,15 @@
     global yt_dlp
 
     if yt_dlp is None:
         import yt_dlp
     return yt_dlp
 
 
-def tube_opts(args, func_opts=None, playlist_opts: Optional[str] = None) -> dict:
+def tube_opts(args, func_opts=None, playlist_opts: str | None = None) -> dict:
     if playlist_opts is None or playlist_opts == "":
         playlist_opts = "{}"
     if func_opts is None:
         func_opts = {}
     cli_opts = {}
     if hasattr(args, "extractor_config"):
         cli_opts = args.extractor_config
@@ -46,15 +46,14 @@
         "lazy_playlist": True,
         "noplaylist": False,
         "extract_flat": True,
         "dynamic_mpd": False,
         "youtube_include_dash_manifest": False,
         "youtube_include_hls_manifest": False,
         "no_check_certificate": True,
-        "check_formats": False,
         "ignore_no_formats_error": True,
         "skip_playlist_after_errors": 21,
         "clean_infojson": False,
         "playlistend": 20000,
     }
 
     all_opts = {
@@ -98,15 +97,15 @@
     yt_dlp = load_module_level_yt_dlp()
     t = Timer()
 
     class ExistingPlaylistVideoReached(yt_dlp.DownloadCancelled):
         pass
 
     class AddToArchivePP(yt_dlp.postprocessor.PostProcessor):
-        def run(self, info) -> Tuple[list, dict]:  # pylint: disable=arguments-renamed
+        def run(self, info) -> tuple[list, dict]:  # pylint: disable=arguments-renamed
             global added_media_count
 
             if info:
                 webpath = iterables.safe_unpack(info.get("webpage_url"), info.get("url"), info.get("original_url"))
                 extractor_key = "ydl_" + (
                     iterables.safe_unpack(info.get("ie_key"), info.get("extractor_key"), info.get("extractor")) or ""
                 )
@@ -175,60 +174,81 @@
         if args.action == consts.SC.tubeupdate:
             if added_media_count > count_before_extract:
                 db_playlists.decrease_update_delay(args, playlist_path)
             else:
                 db_playlists.increase_update_delay(args, playlist_path)
 
 
-def get_extra_metadata(args, playlist_path, playlist_dl_opts=None) -> Optional[List[Dict]]:
+def yt_subs_config(args):
+    if args.subs:
+        return {"writesubtitles": True, "writeautomaticsub": True}
+    elif args.auto_subs:
+        return {"writesubtitles": False, "writeautomaticsub": True}
+    return {}
+
+
+def get_extra_metadata(args, playlist_path, playlist_dl_opts=None) -> list[dict] | None:
     yt_dlp = load_module_level_yt_dlp()
 
+    tables = args.db.table_names()
     m_columns = db_utils.columns(args, "media")
 
     with yt_dlp.YoutubeDL(
         tube_opts(
             args,
             func_opts={
                 "subtitlesformat": "srt/best",
-                "writesubtitles": args.subs,
-                "writeautomaticsub": args.auto_subs,
+                **yt_subs_config(args),
                 "subtitleslangs": args.subtitle_languages,
                 "extract_flat": False,
                 "lazy_playlist": False,
                 "check_formats": False,
                 "skip_download": True,
                 "outtmpl": {
                     "default": str(
                         Path(f"{consts.SUB_TEMP_DIR}/%(id).60B.%(ext)s"),
                     ),
                 },
                 "ignoreerrors": True,
             },
             playlist_opts=playlist_dl_opts,
-        ),
+        )
     ) as ydl:
-        try:
-            videos = args.db.execute(
+        videos = set(
+            args.db.execute(
                 f"""
                 SELECT
-                id
-                , path
-                , playlists_id
+                    id
+                    , path
+                    , null as playlists_id
                 FROM media
-                WHERE 1=1
-                    AND COALESCE(time_deleted, 0)=0
+                WHERE COALESCE(time_deleted, 0)=0
+                    AND path = ?
                     {'and width is null' if 'width' in m_columns else ''}
-                    and path not like '%playlist%'
-                    and playlists_id = (select id from playlists where path = ?)
-                ORDER by random()
                 """,
                 [playlist_path],
             ).fetchall()
-        except sqlite3.OperationalError:
-            videos = []
+        )
+
+        if "playlists" in tables:
+            videos |= set(
+                args.db.execute(
+                    f"""
+                    SELECT
+                        id
+                        , path
+                        , playlists_id
+                    FROM media
+                    WHERE COALESCE(time_deleted, 0)=0
+                        AND playlists_id = (select id from playlists where path = ?)
+                        {'AND width is null' if 'width' in m_columns else ''}
+                    """,
+                    [playlist_path],
+                ).fetchall()
+            )
 
         current_video_count = 0
         for id, path, playlists_id in videos:
             entry = ydl.extract_info(path)
             if entry is None:
                 continue
 
@@ -263,15 +283,15 @@
 
             db_media.playlist_media_add(args, path, entry)
 
             current_video_count += 1
             printing.print_overwrite(f"[{playlist_path}] {current_video_count} of {len(videos)} extra metadata fetched")
 
 
-def get_video_metadata(args, playlist_path) -> Optional[Dict]:
+def get_video_metadata(args, playlist_path) -> dict | None:
     yt_dlp = load_module_level_yt_dlp()
 
     with yt_dlp.YoutubeDL(
         tube_opts(
             args,
             func_opts={
                 "skip_download": True,
@@ -319,45 +339,46 @@
     def out_dir(p):
         return str(Path(args.prefix, "%(extractor_key,extractor)s", p))
 
     func_opts = {
         "ignoreerrors": ignoreerrors,
         "extractor_args": {"youtube": {"skip": ["authcheck"]}},
         "logger": DictLogger(),
-        "skip_download": bool(consts.PYTEST_RUNNING),
+        "skip_download": False,
         "postprocessors": [{"key": "FFmpegMetadata"}],
         "restrictfilenames": True,
         "extract_flat": False,
         "lazy_playlist": True,
         "noplaylist": True,
         "playlist_items": "1",
         "playlist_end": None,
         "extractor_retries": 3,
         "retries": 12,
         "retry_sleep_functions": {
             "extractor": lambda n: 0.2 * n,
-            "http": lambda n: 0.1 * (2**n),
+            "http": lambda n: 0.08 * (2**n),
             "fragment": lambda n: 0.04 * (2**n),
         },
         "outtmpl": {
             "default": out_dir("%(uploader,uploader_id)s/%(title).200B_%(view_count)3.2D_[%(id).60B].%(ext)s"),
             "chapter": out_dir(
                 "%(uploader,uploader_id)s/%(title).200B_%(section_number)03d_%(section_title)s_%(view_count)3.2D_[%(id).60B].%(ext)s",
             ),
         },
     }
 
     if args.verbose >= consts.LOG_DEBUG:
-        func_opts["progress_hooks"] = [lambda d: log.debug(f"downloading {d['_percent_str']} {d['_speed_str']}")]
+        func_opts["progress_hooks"] = [
+            lambda d: log.debug(f"downloading {d['_percent_str']} {d['_speed_str']} {d['downloaded_bytes']} bytes")
+        ]
 
     if args.profile != DBType.audio:
         func_opts["subtitlesformat"] = "srt/best"
         func_opts["subtitleslangs"] = args.subtitle_languages
-        func_opts["writesubtitles"] = args.subs
-        func_opts["writeautomaticsub"] = args.auto_subs
+        func_opts |= yt_subs_config(args)
         func_opts["postprocessors"].append({"key": "FFmpegEmbedSubtitle"})
 
     def yt_cli_to_api(opts):
         default = yt_dlp.parse_options([]).ydl_opts
         supplied = yt_dlp.parse_options(opts).ydl_opts
         diff = {k: v for k, v in supplied.items() if default[k] != v}
         if diff.get("postprocessors"):
@@ -375,25 +396,22 @@
     match_filters = ["live_status=?not_live"]
     if match_filter_user_config is not None:
         match_filters.append(match_filter_user_config)
 
     if args.small:
         if match_filter_user_config is None:
             match_filters.append("duration >? 59 & duration <? 14399")
-        ydl_opts[
-            "format"
-        ] = "bestvideo[height<=576][filesize<2G]+bestaudio/best[height<=576][filesize<2G]/bestvideo[height<=576]+bestaudio/best[height<=576]/best"
+        ydl_opts["format_sort"] = ["res:576"]
+        ydl_opts["format"] = "bestvideo[filesize<2G]+bestaudio/best[filesize<2G]/bestvideo*+bestaudio/best"
 
     if args.profile == DBType.audio:
         ydl_opts[
             "format"
-        ] = "bestaudio[ext=opus]/bestaudio[ext=webm]/bestaudio[ext=ogg]/bestaudio[ext=oga]/bestaudio/best"
-        if args.ext is None:
-            args.ext = "opus"
-        ydl_opts["postprocessors"].append({"key": "FFmpegExtractAudio", "preferredcodec": args.ext})
+        ] = "bestaudio[ext=opus]/bestaudio[ext=mka]/bestaudio[ext=webm]/bestaudio[ext=ogg]/bestaudio[ext=oga]/bestaudio/best"
+        ydl_opts["postprocessors"].append({"key": "FFmpegExtractAudio", "preferredcodec": "opus"})
 
     def blocklist_check(info, *pargs, incomplete):
         if getattr(args, "blocklist_rules", False):
             media_entry = db_media.consolidate(deepcopy(info))
             if sql_utils.is_blocked_dict_like_sql(media_entry or {}, args.blocklist_rules):
                 raise yt_dlp.utils.RejectedVideoReached("Video matched library blocklist")
         ytdlp_match_filter = yt_dlp.utils.match_filter_func(" & ".join(match_filters).split(" | "))
@@ -461,43 +479,45 @@
             info = {**m, **info}
             local_path = info.get("local_path", None)
             if args.profile == DBType.audio:
                 local_path = ydl.prepare_filename({**info, "ext": args.ext})
             else:
                 local_path = ydl.prepare_filename(info)
 
-    ydl_errors = ydl_log["error"] + ydl_log["warning"]
-    ydl_errors = "\n".join([line for line in ydl_errors if not yt_meaningless_errors.match(line)])
     ydl_full_log = ydl_log["error"] + ydl_log["warning"] + ydl_log["info"]
+    ydl_errors = [
+        line for log_entry in ydl_full_log for line in log_entry.splitlines() if not yt_meaningless_errors.match(line)
+    ]
+    ydl_errors_txt = "\n".join(ydl_errors)
 
     if args.verbose >= consts.LOG_DEBUG_SQL:
         log.debug("\n".join(ydl_full_log))
 
-    if not ydl_log["error"] and info and local_path:
+    if not ydl_log["error"] and info and local_path and Path(local_path).exists():
         try:
             info["corruption"] = int(
                 media_check.calculate_corruption(local_path, threads=1, full_scan_if_corrupt=True) * 100
             )
         except RuntimeError:
             info["corruption"] = 50
         if info["corruption"] > 7:
-            log.debug("[%s]: Media check failed (will try again later)", webpath)
+            log.info("[%s]: Media check failed (will try again later)", webpath)
             db_media.download_add(args, webpath, info, local_path, error="Media check failed")
         else:
-            log.debug("[%s]: No news is good news", webpath)
+            log.info("[%s]: Downloaded to %s", webpath, local_path)
             db_media.download_add(args, webpath, info, local_path)
-    elif any(yt_recoverable_errors.match(line) for line in ydl_full_log):
-        log.info("[%s]: Recoverable error matched (will try again later). %s", webpath, ydl_errors)
-        db_media.download_add(args, webpath, info, local_path, error=ydl_errors)
-    elif any(yt_unrecoverable_errors.match(line) for line in ydl_full_log):
+    elif any(yt_recoverable_errors.match(line) for line in ydl_errors):
+        log.info("[%s]: Recoverable error matched (will try again later). %s", webpath, ydl_errors_txt)
+        db_media.download_add(args, webpath, info, local_path, error=ydl_errors_txt)
+    elif any(yt_unrecoverable_errors.match(line) for line in ydl_errors):
         matched_error = [
-            m.string for m in iterables.conform([yt_unrecoverable_errors.match(line) for line in ydl_full_log])
+            m.string for m in iterables.conform([yt_unrecoverable_errors.match(line) for line in ydl_errors])
         ]
-        log.debug("[%s]: Unrecoverable error matched. %s", webpath, ydl_errors or strings.combine(matched_error))
-        db_media.download_add(args, webpath, info, local_path, error=ydl_errors, unrecoverable_error=True)
-    elif any(prefix_unrecoverable_errors.match(line) for line in ydl_full_log):
-        log.warning("[%s]: Prefix error. %s", webpath, ydl_errors)
+        log.info("[%s]: Unrecoverable error matched. %s", webpath, ydl_errors_txt or strings.combine(matched_error))
+        db_media.download_add(args, webpath, info, local_path, error=ydl_errors_txt, unrecoverable_error=True)
+    elif any(prefix_unrecoverable_errors.match(line) for line in ydl_errors):
+        log.warning("[%s]: Prefix error. %s", webpath, ydl_errors_txt)
         raise SystemExit(28)
     else:
-        if ydl_errors != "":
-            log.error("[%s]: Unknown error. %s", webpath, ydl_errors)
-        db_media.download_add(args, webpath, info, local_path, error=ydl_errors)
+        log.error("[%s]: Unknown error. %s", webpath, ydl_errors_txt)
+        pprint([yt_meaningless_errors.match(line) for line in ydl_full_log])
+        db_media.download_add(args, webpath, info, local_path, error=ydl_errors_txt)
```

### Comparing `xklb-2.5.9/xklb/tube_extract.py` & `xklb-2.6.1/xklb/scripts/disk_usage.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,141 +1,168 @@
-import argparse, sys
+import argparse, os
 from pathlib import Path
 
-from xklb import db_media, db_playlists, tube_backend, usage
-from xklb.utils import arg_utils, consts, db_utils, iterables, objects, path_utils, processes
-from xklb.utils.consts import SC
+from xklb import usage
+from xklb.media import media_printer
+from xklb.utils import arggroups, consts, db_utils, file_utils, nums, objects, processes, sql_utils
 from xklb.utils.log_utils import log
 
 
-def parse_args(action, usage) -> argparse.Namespace:
+def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        prog="library " + action,
-        usage=usage,
+        prog="library disk_usage",
+        usage=usage.disk_usage,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
+    arggroups.sql_fs(parser)
+    arggroups.operation_group_folders(parser)
+    parser.set_defaults(limit="4000", depth=0)
 
-    parser.add_argument(
-        "--extractor-config",
-        "-extractor-config",
-        nargs=1,
-        action=arg_utils.ArgparseDict,
-        default={},
-        metavar="KEY=VALUE",
-        help="Add key/value pairs to override or extend default downloader configuration",
-    )
-    parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
-    parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
-    parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
-    parser.add_argument("--extra", "-extra", action="store_true", help="Get full metadata (takes a lot longer)")
-    parser.add_argument("--no-optimize", action="store_true", help=argparse.SUPPRESS)
-
-    parser.add_argument(
-        "--force",
-        "-f",
-        action="store_true",
-        help="Fetch metadata for paths even if they are already in the media table",
-    )
-    parser.add_argument("--subs", action="store_true")
-    parser.add_argument("--auto-subs", "--autosubs", action="store_true")
-    parser.add_argument("--subtitle-languages", "--subtitle-language", "--sl", action=arg_utils.ArgparseList)
-
-    parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true", help=argparse.SUPPRESS)
-
-    parser.add_argument("--timeout", "-T", help="Quit after x minutes")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
-
-    parser.add_argument("database")
-    if action == SC.tubeadd:
-        parser.add_argument("--insert-only", action="store_true")
-        parser.add_argument("--insert-only-playlists", action="store_true")
-        parser.add_argument("playlists", nargs="*", default=arg_utils.STDIN_DASH, action=arg_utils.ArgparseArgsOrStdin)
+    parser.add_argument("--folders-only", "-td", action="store_true", help="Only print folders")
+    parser.add_argument("--files-only", "-tf", action="store_true", help="Only print files")
 
-    args = parser.parse_intermixed_args()
-    args.action = action
+    arggroups.debug(parser)
 
-    if args.db:
-        args.database = args.db
-    if action == SC.tubeadd:
-        Path(args.database).touch()
+    arggroups.database(parser)
+    parser.add_argument("working_directory", nargs="*", default=os.sep)
+    args = parser.parse_intermixed_args()
     args.db = db_utils.connect(args)
 
-    if hasattr(args, "playlists"):
-        args.playlists = list(set(s.strip() for s in args.playlists))
-        if not args.no_sanitize:
-            args.playlists = [path_utils.sanitize_url(args, p) for p in args.playlists]
-        args.playlists = iterables.conform(args.playlists)
+    args.include += args.working_directory
+    if args.include == ["."]:
+        args.include = [str(Path().cwd().resolve())]
 
-    processes.timeout(args.timeout)
+    if len(args.include) == 1 and os.sep in args.include[0]:
+        args.include = [file_utils.resolve_absolute_path(args.include[0])]
 
+    if args.sort_groups_by:
+        args.sort_groups_by = " ".join(args.sort_groups_by)
+
+    if args.size:
+        args.size = sql_utils.parse_human_to_sql(nums.human_to_bytes, "size", args.size)
+
+    args.action = consts.SC.diskusage
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def tube_add(args=None) -> None:
-    if args:
-        sys.argv = ["tubeadd", *args]
-
-    args = parse_args(SC.tubeadd, usage=usage.tubeadd)
-
-    if args.insert_only:
-        args.db["media"].insert_all(
-            [{"path": p, "time_created": consts.APPLICATION_START} for p in args.playlists],
-            alter=True,
-            ignore=True,
-            pk="path",
-        )
-    elif args.insert_only_playlists:
-        args.db["playlists"].insert_all(
-            [{"path": p, "time_created": consts.APPLICATION_START} for p in args.playlists],
-            alter=True,
-            ignore=True,
-            pk="path",
-        )
-    else:
-        known_playlists = set()
-        if not args.force and len(args.playlists) > 9:
-            known_playlists = db_media.get_paths(args)
-
-        for path in args.playlists:
-            if args.safe and not tube_backend.is_supported(path):
-                log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
-                continue
+def sort_by(args):
+    if args.sort_groups_by:
+        return lambda x: x.get(args.sort_groups_by) or 0
 
-            if path in known_playlists:
-                log.info("[%s]: Already added. Skipping!", path)
+    return lambda x: (x["size"] / (x.get("count") or 1), x["size"], x.get("count") or 1)
+
+
+def get_subset(args, level=None, prefix=None) -> list[dict]:
+    d = {}
+    excluded_files = set()
+
+    for m in args.data:
+        if prefix is not None and not m["path"].startswith(prefix):
+            continue
+
+        p = m["path"].split(os.sep)
+        if level is not None and len(p) == level and not m["path"].endswith(os.sep):
+            d[m["path"]] = m
+
+        while len(p) >= 2:
+            p.pop()
+            if p == [""]:
                 continue
 
-            tube_backend.get_playlist_metadata(args, path, tube_backend.tube_opts(args))
+            parent = os.sep.join(p) + os.sep
+            if level is not None and len(p) != level:
+                excluded_files.add(parent)
+
+            if parent not in d:
+                d[parent] = {"size": 0, "count": 0}
+            d[parent]["size"] += m.get("size") or 0
+            d[parent]["count"] += 1
+
+    reverse = True
+    if args.sort_groups_by and " desc" in args.sort_groups_by:
+        args.sort_groups_by = args.sort_groups_by.replace(" desc", "")
+        reverse = False
+
+    return sorted(
+        [{"path": k, **v} for k, v in d.items() if k not in excluded_files],
+        key=sort_by(args),
+        reverse=reverse,
+    )
+
 
-            if args.extra:
-                log.warning("[%s]: Getting extra metadata", path)
-                tube_backend.get_extra_metadata(args, path)
+def load_subset(args):
+    level = args.depth
+    if args.depth == 0:
+        while len(args.subset) < 2:
+            level += 1
+            args.subset = get_subset(args, level=level, prefix=args.cwd)
+    else:
+        args.subset = get_subset(args, level=level, prefix=args.cwd)
+
+    if not args.subset:
+        processes.no_media_found()
 
-    if not args.no_optimize and not args.db["media"].detect_fts():
-        db_utils.optimize(args)
+    args.cwd = os.sep.join(args.subset[0]["path"].split(os.sep)[: level - 1]) + os.sep
+    return args.cwd, args.subset
 
 
-def tube_update(args=None) -> None:
-    if args:
-        sys.argv = ["tubeupdate", *args]
+def get_data(args) -> list[dict]:
+    m_columns = db_utils.columns(args, "media")
+    args.filter_sql = []
+    args.filter_bindings = {}
 
-    args = parse_args(SC.tubeupdate, usage=usage.tubeupdate)
-    tube_playlists = db_playlists.get_all(
+    if args.size:
+        args.filter_sql.append(" and size IS NOT NULL " + args.size)
+    db_utils.construct_search_bindings(
         args,
-        sql_filters=["AND extractor_key NOT IN ('Local', 'reddit_praw_redditor', 'reddit_praw_subreddit')"],
+        [f"{k}" for k in m_columns if k in db_utils.config["media"]["search_columns"]],
+    )
+
+    media = list(
+        args.db.query(
+            f"""
+        SELECT
+            path
+            , size
+        FROM media m
+        WHERE 1=1
+            and size > 0
+            {'and coalesce(time_deleted, 0) = 0' if 'time_deleted' in m_columns else ''}
+            {'and coalesce(is_dir, 0) = 0' if 'is_dir' in m_columns else ''}
+            {" ".join(args.filter_sql)}
+        ORDER BY path
+        """,
+            args.filter_bindings,
+        ),
     )
-    for d in tube_playlists:
-        tube_backend.get_playlist_metadata(
-            args,
-            d["path"],
-            tube_backend.tube_opts(
-                args,
-                playlist_opts=d.get("extractor_config", "{}"),
-                func_opts={"ignoreerrors": "only_download"},
-            ),
-        )
-
-        if args.extra:
-            log.warning("[%s]: Getting extra metadata", d["path"])
-            tube_backend.get_extra_metadata(args, d["path"], playlist_dl_opts=d.get("extractor_config", "{}"))
+
+    if not media:
+        processes.no_media_found()
+    return media
+
+
+def disk_usage():
+    args = parse_args()
+    args.data = get_data(args)
+    args.subset = []
+    args.cwd = None
+
+    load_subset(args)
+
+    num_folders = sum(1 for d in args.subset if d.get("count"))
+    num_files = sum(1 for d in args.subset if not d.get("count"))
+
+    if args.folders_only:
+        args.subset = [d for d in args.subset if d.get("count")]
+    elif args.files_only:
+        args.subset = [d for d in args.subset if not d.get("count")]
+
+    media_printer.media_printer(
+        args,
+        args.subset,
+        units=f"paths at current depth ({num_folders} folders, {num_files} files)",
+    )
+
+
+if __name__ == "__main__":
+    disk_usage()
```

### Comparing `xklb-2.5.9/xklb/usage.py` & `xklb-2.6.1/xklb/usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
     Files will be saved to <lb download prefix>/<extractor>/. If prefix is not specified the current working directory will be used
 
     By default things will download in a random order
 
         library download dl.db --prefix ~/output/path/root/
 
+    But you can sort; eg. oldest first
+
+        library download dl.db -u m.time_modified,m.time_created
+
     Limit downloads to a specified playlist URLs or substring (TODO: https://github.com/chapmanjacobd/library/issues/31)
 
         library download dl.db https://www.youtube.com/c/BlenderFoundation/videos
 
     Limit downloads to a specified video URLs or substring
 
         library download dl.db --include https://www.youtube.com/watch?v=YE7VzlLtp-4
@@ -379,15 +383,15 @@
 
         You may also want to restrict the play queue.
         For example, when you only want 1000 random files:
         library {action} -u random -L 1000
 
     Offset the play queue:
         You can also offset the queue. For example if you want to skip one or ten media:
-        library {action} --skip 10        # offset ten from the top of an ordered query
+        library {action} --offset 10      # offset ten from the top of an ordered query
 
     Repeat
         library {action}                  # listen to 120 random songs (DEFAULT_PLAY_QUEUE)
         library {action} --limit 5        # listen to FIVE songs
         library {action} -l inf -u random # listen to random songs indefinitely
         library {action} -s infinite      # listen to songs from the band infinite
 
@@ -533,14 +537,35 @@
 
         Playback multiple files at once
         library {action} --multiple-playback    # one per display; or two if only one display detected
         library {action} --multiple-playback 4  # play four media at once, divide by available screens
         library {action} -m 4 --screen-name eDP # play four media at once on specific screen
         library {action} -m 4 --loop --crop     # play four cropped videos on a loop
         library {action} -m 4 --hstack          # use hstack style
+
+        When using `--multiple-playback` it may be helpful to set simple window focus rules to prevent keys from accidentally being entered in the wrong mpv window (as new windows are created and capture the cursor focus).
+        You can set and restore your previous mouse focus setting by wrapping the command like this:
+
+            focus-under-mouse
+            library watch ... --multiple-playback 4
+            focus-follows-mouse
+
+        For example in KDE:
+
+            function focus-under-mouse
+                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusUnderMouse
+                qdbus-qt5 org.kde.KWin /KWin reconfigure
+            end
+
+            function focus-follows-mouse
+                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusFollowsMouse
+                kwriteconfig5 --file kwinrc --group Windows --key NextFocusPrefersMouse true
+                qdbus-qt5 org.kde.KWin /KWin reconfigure
+            end
+
 """
 
 
 watch = play("watch")
 
 
 redditadd = """library redditadd [--lookback N_DAYS] [--praw-site bot1] DATABASE URLS ...
@@ -876,14 +901,25 @@
 
     Importing from a line-delimitated file:
 
         library tabsadd -f yearly -c reddit tabs.db (cat ~/mc/yearly-subreddit.cron)
 
 """
 
+tabs_shuffle = """library tabs-shuffle DATABASE
+
+    Moves each tab to a random day-of-the-week by default
+
+    It may also be useful to shuffle monthly tabs, etc. You can accomplish this like so:
+
+        library tabs-shuffle tabs.db -d  31 -f monthly
+        library tabs-shuffle tabs.db -d  90 -f quarterly
+        library tabs-shuffle tabs.db -d 365 -f yearly
+"""
+
 tubeadd = r"""library tubeadd [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
 
     Create a dl database / add links to an existing database
 
         library tubeadd dl.db https://www.youdl.com/c/BranchEducation/videos
 
     Add links from a line-delimited file
@@ -984,15 +1020,15 @@
 
 """
 
 christen = """library christen DATABASE [--run]
 
     Rename files to be somewhat normalized
 
-    Default mode is dry-run
+    Default mode is simulate
 
         library christen fs.db
 
     To actually do stuff use the run flag
 
         library christen audio.db --run
 
@@ -1035,27 +1071,43 @@
 
     Auto-sort images into directories
 
         echo 'image1.jpg
         image2.jpg
         image3.jpg' | library cluster-sort --image --move-groups
 
+    Print similar paths
+
+        library fs 0day.db -pa --cluster --print-groups
+
 """
 
 copy_play_counts = """library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
 
     Copy play count information between databases
 
         library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
 """
-dedupe_media = """library [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
+dedupe_media = """library dedupe-media [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
 
     Dedupe your files (not to be confused with the dedupe-db subcommand)
 
-    library dedupe video.db / http
+    Exact file matches
+
+        library dedupe-media --fs video.db
+
+    Dedupe based on duration and file basename or dirname similarity
+
+        library dedupe-media video.db --duration --basename -s release_group  # pre-filter with a specific text substring
+        library dedupe-media video.db --duration --basename -u m1.size  # sort such that small files are treated as originals and larger files are deleted
+        library dedupe-media video.db --duration --basename -u 'm1.size desc'  # sort such that large files are treated as originals and smaller files are deleted
+
+    Dedupe online against local media
+
+        library dedupe-media video.db / http
 """
 
 dedupe_db = """library dedupe-dbs DATABASE TABLE --bk BUSINESS_KEYS [--pk PRIMARY_KEYS] [--only-columns COLUMNS]
 
     Dedupe your database (not to be confused with the dedupe subcommand)
 
     It should not need to be said but *backup* your database before trying this tool!
@@ -1101,15 +1153,15 @@
      To skip copying primary-keys from the source table(s) use --business-keys instead of --primary-keys
 
      Split DBs using --where
 
          library merge-dbs --pk path specific-site.db big.db -v --only-new-rows -t media,playlists -w 'path like "https://specific-site%"'
 """
 
-merge_folders = """library merge-folders [--replace] [--skip] [--simulate] SOURCES ... DESTINATION
+merge_folders = """library merge-folders [--replace] [--no-replace] [--simulate] SOURCES ... DESTINATION
 
     Merge multiple folders with the same file tree into a single folder.
 
     https://github.com/chapmanjacobd/journal/blob/main/programming/linux/misconceptions.md#mv-src-vs-mv-src
 
     Trumps are new or replaced files from an earlier source which now conflict with a later source.
     If you only have one source then the count of trumps will always be zero.
@@ -1163,27 +1215,27 @@
         ...
 
     ...or between two timestamps inclusive:
 
         library redownload city.db 2023-01-26T19:54:42 2023-01-26T20:45:24
 """
 
-relmv = """library relmv [--dry-run] SOURCE ... DEST
+relmv = """library relmv [--simulate] SOURCE ... DEST
 
     Move files/folders without losing hierarchy metadata
 
     Move fresh music to your phone every Sunday:
 
         # move last week music back to their source folders
-        library relmv /mnt/d/80_Now_Listening/ /mnt/d/
+        library mv /mnt/d/sync/weekly/ /mnt/d/check/audio/
 
         # move new music for this week
         library relmv (
             library listen audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
-        ) /mnt/d/80_Now_Listening/
+        ) /mnt/d/sync/weekly/
 """
 
 mv_list = """library mv-list [--limit LIMIT] [--lower LOWER] [--upper UPPER] MOUNT_POINT DATABASE
 
     Free up space on a specific disk. Find candidates for moving data to a different mount point
 
 
@@ -1237,15 +1289,15 @@
 
     After you are done selecting folders you can press ctrl-d and it will save the list to a tmp file:
 
         Paste a path: done
 
             Folder list saved to /tmp/tmp7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
 
-                rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmp7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
+                rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmp7x_75l8 -r --relative -vv --simulate / jim:/free/real/estate/
 """
 
 scatter = """library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --targets TARGETS DATABASE RELATIVE_PATH ...
 
     Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
 
     Scatter filesystem folder trees (without mountpoints; limited functionality; good for balancing fs inodes)
@@ -1456,15 +1508,16 @@
 
 incremental_diff = """library incremental-diff PATH1 PATH2 [--join-keys JOIN_KEYS] [--table1 TABLE1] [--table2 TABLE2] [--table1-index TABLE1_INDEX] [--table2-index TABLE2_INDEX] [--start-row START_ROW] [--batch-size BATCH_SIZE]
 
     See data differences in an incremental way to quickly see how two different files differ.
 
     Data (PATH1, PATH2) can be two different files of different file formats (CSV, Excel) or it could even be the same file with different tables.
 
-    If files are unsorted you may need to use `--join-keys id,name` to specify ID columns. Rows that have the same ID will then be compared. If you are comparing SQLITE files you may be able to use `--sort id,name` to achieve the same effect.
+    If files are unsorted you may need to use `--join-keys id,name` to specify ID columns. Rows that have the same ID will then be compared.
+    If you are comparing SQLITE files you may be able to use `--sort id,name` to achieve the same effect.
 
     To diff everything at once run with `--batch-size inf`
 """
 
 extract_links = """library extract-links PATH ... [--case-sensitive] [--scroll] [--download] [--verbose] [--local-html] [--file FILE] [--path-include ...] [--text-include ...] [--after-include ...] [--before-include ...] [--path-exclude ...] [--text-exclude ...] [--after-exclude ...] [--before-exclude ...]
 
     Extract links from within local HTML fragments, files, or remote pages; filtering on link text and nearby plain-text
@@ -1597,29 +1650,36 @@
     Extract data from website requests to a database
 
         library siteadd jobs.st.db --poke https://hk.jobsdb.com/hk/search-jobs/python/
 
     Run with `-vv` to see and interact with the browser
 """
 
-process_audio = """library process-audio PATH ... [--always-split] [--split-longer-than DURATION] [--min-split-segment SECONDS] [--dry-run]
+process_ffmpeg = """library process-ffmpeg PATH ... [--always-split] [--split-longer-than DURATION] [--min-split-segment SECONDS] [--simulate]
+
+    Resize videos to max 1440x960px AV1 and/or Opus to save space
 
     Convert audio to Opus. Optionally split up long tracks into multiple files.
 
-        fd -tf -eDTS -eAAC -eWAV -eAIF -eAIFF -eFLAC -eAIFF -eM4A -eMP3 -eOGG -eMP4 -eWMA -j4 -x library process-audio
+        fd -tf -eDTS -eAAC -eWAV -eAIF -eAIFF -eFLAC -eAIFF -eM4A -eMP3 -eOGG -eMP4 -eWMA -j4 -x library process --audio
 
     Use --always-split to _always_ split files if silence is detected
 
         library process-audio --always-split audiobook.m4a
 
     Use --split-longer-than to _only_ detect silence for files in excess of a specific duration
 
         library process-audio --split-longer-than 36mins audiobook.m4b audiobook2.mp3
 """
 
+process_image = """library process-image PATH ...
+
+    Resize images to max 2400x2400px and format AVIF to save space
+"""
+
 sample_hash = """library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
 
     Calculate hashes for large files by reading only small segments of each file
 
         library sample-hash ./my_file.mkv
 
     The threads flag seems to be faster for rotational media but slower on SSDs
@@ -1632,31 +1692,36 @@
 
 media_check = """library media-check [--chunk-size SECONDS] [--gap SECONDS OR 0.0-1.0*DURATION] [--delete-corrupt >0-100] [--full-scan] [--audio-scan] PATH ...
 
     Defaults to decode 0.5 second per 10%% of each file
 
         library media-check ./video.mp4
 
-    Decode all the frames of each file to evaluate how corrupt it is (very slow; about 150 seconds for an hour-long file)
+    Decode all the frames of each file to evaluate how corrupt it is
+    (scantime is very slow; about 150 seconds for an hour-long file)
 
         library media-check --full-scan ./video.mp4
 
-    Decode all the packets of each file to evaluate how corrupt it is (about one second of each file but only accurate for formats where 1 packet == 1 frame)
+    Decode all the packets of each file to evaluate how corrupt it is
+    (scantime is about one second of each file but only accurate for formats where 1 packet == 1 frame)
 
         library media-check --full-scan --gap 0 ./video.mp4
 
-    Decode all audio of each file to evaluate how corrupt it is (about four seconds per file)
+    Decode all audio of each file to evaluate how corrupt it is
+    (scantime is about four seconds per file)
 
         library media-check --full-scan --audio ./video.mp4
 
-    Decode at least one frame at the start and end of each file to evaluate how corrupt it is (takes about one second per file)
+    Decode at least one frame at the start and end of each file to evaluate how corrupt it is
+    (scantime is about one second per file)
 
         library media-check --chunk-size 5%% --gap 99.9%% ./video.mp4
 
-    Decode 3s every 5%% of a file to evaluate how corrupt it is (takes about three seconds per file)
+    Decode 3s every 5%% of a file to evaluate how corrupt it is
+    (scantime is about three seconds per file)
 
         library media-check --chunk-size 3 --gap 5%% ./video.mp4
 
     Delete the file if 20 percent or more of checks fail
 
         library media-check --delete-corrupt 20%% ./video.mp4
 
@@ -1695,16 +1760,69 @@
         [ 91.0 .. 100.0] [141] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
 """
 
 webadd = """library web-add [(--filesystem) | --video | --audio | --image | --text] DATABASE URL ...
 
     Scan open directories
 
-    library download open_dir.db --fs --prefix ~/d/dump/video/ --relative -vv -s factory -p
+        library web-add open_dir.db --video http://1.1.1.1/
+
+    Check download size of all videos matching some criteria
+
+        library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'height<720' -E preview -pa
+
+        path         count  download_duration                  size    avg_size
+        ---------  -------  ----------------------------  ---------  ----------
+        Aggregate     5694  2 years, 7 months and 5 days  724.4 GiB   130.3 MiB
+
+    Download all videos matching some criteria
+
+        library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'height<720' -E preview
+
+    Stream directly to mpv
+
+        library watch open_dir.db
+
+    Check videos before downloading
+
+        library watch open_dir.db --online-media-only --loop --exit-code-confirm -i --action ask-keep -m 4  --start 35%% --volume=0 -w 'height<720' -E preview
+
+        Assuming you have bound in mpv input.conf a key to 'quit' and another key to 'quit 4',
+        using the ask-keep action will mark a video as deleted when you 'quit 4' and it will mark a video as watched when you 'quit'.
+
+        For example, here I bind "'" to "KEEP" and  "j" to "DELETE"
+
+            ' quit
+            j quit 4
+
+        This is pretty intuitive after you use it a few times but writing this out I realize this might seem a bit opaque.
+        Instead of using built-in post-actions (example above) you could also do something like
+            `--cmd5 'echo {} >> keep.txt' --cmd6 'echo {} >> rejected.txt'`
+
+        But you will still bind keys in mpv input.conf:
+
+            k quit 5  # goes to keep.txt
+            r quit 6  # goes to rejected.txt
+
+    Download checked videos
+
+        library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'id in (select media_id from history)'
 
 """
 
 webupdate = """library web-update DATABASE
 
     Update saved open directories
 
 """
+
+add_row = """library add-row DATABASE [--table-name TABLE_NAME]
+
+    Add a row to sqlite
+
+        library add-row t.db --test_b 1 --test-a 2
+
+        ### media (1 rows)
+        |   test_b |   test_a |
+        |----------|----------|
+        |        1 |        2 |
+"""
```

### Comparing `xklb-2.5.9/xklb/data/dl_config.py` & `xklb-2.6.1/xklb/data/dl_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,42 +63,35 @@
 .*copyright claim""".splitlines(),
     ),
 )
 
 
 yt_meaningless_errors = re.compile(
     "|".join(
-        r"""^\[info\]
-^\[redirect\]
-^\[Merger\]
-^\[dashsegments\]
-^Found
-.*hidden
+        r""".*hidden
 .*timed out
 .*Timeout
 .*Timed
 .*Connection reset
 .*ConnectionReset
 .*Unable to extract
-.*Unauthorized
-.*Forbidden
 .*Traceback
 .*Invalid argument
 .*KeyboardInterrupt
 .*Fatal Python error
 .*list index out of range
 .*Extract.* cookies
-.*File .*, line .*, in
-.*Requested format is not available.
+.*File .*, line .*,
+.*Requested format is not available
 .*This channel does not have
 .*fragment_filename_sanitized
 .*no suitable InfoExtractor for URL
-.*File name too long
 .*No such file or directory
 .*Name or service not known
+.*Extracting URL
 .*: Downloading webpage
 .*: Extracting information
 .*: Requesting header
 .*mismatched tag
 .*Fail.* parse
 .*Downloading .* metadata
 .*Downloading .* information
@@ -141,14 +134,15 @@
     ),
 )
 
 yt_unrecoverable_errors = re.compile(
     "|".join(
         r""".*repetitive or misleading metadata
 .*It is not available
+.*does not pass filter
 .*has already been recorded in the archive
 .*ideo.*is private
 .*already ended
 .*id.*was not found
 .*No video player ID
 .*has been removed
 .*from a suspended account
@@ -239,27 +233,28 @@
 .*This video doesn't exist.
 .*Track not found
 .*Not found.
 .*Can't find object media for
 .*No video formats found
 .*certificate is not valid
 .*CERTIFICATE_VERIFY_FAILED
-.*HTTP Error 403: Forbidden
+.*Forbidden
 .*code -404
 .*HTTP Error 404
 .*HTTPError 404
 .*HTTP Error 410
 .*HTTPError 410
 .*stopping due to --break-match-filter""".splitlines(),
     ),
 )
 
 
 prefix_unrecoverable_errors = re.compile(
     "|".join(
         r""".*unable to write data:
 .*No space left on device
+.*File name too long
 .*Transport endpoint is not connected
 .*unable to create directory
 .*Permission denied""".splitlines(),
     ),
 )
```

### Comparing `xklb-2.5.9/xklb/data/wordbank.py` & `xklb-2.6.1/xklb/data/wordbank.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.9/xklb/media/av.py` & `xklb-2.6.1/xklb/media/av.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from datetime import datetime
 from pathlib import Path
-from typing import Dict, Optional
 
 from xklb.media import media_check, subtitle
 from xklb.utils import consts, file_utils, iterables, nums, objects, processes, strings
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import log
 
 
@@ -32,15 +31,15 @@
         "attachment_count": attachment_count,
         "subtitles": subtitles,
     }
 
     return video_tags
 
 
-def parse_tags(mu: Dict, ti: Dict) -> dict:
+def parse_tags(mu: dict, ti: dict) -> dict:
     tags = {
         "mood": strings.combine(
             mu.get("albummood"),
             mu.get("MusicMatch_Situation"),
             mu.get("Songs-DB_Occasion"),
             mu.get("albumgrouping"),
         ),
@@ -195,15 +194,15 @@
         )
 
     if format_ != {}:
         log.info("Extra data %s", format_)
 
     streams = probe.streams
 
-    def parse_framerate(string) -> Optional[float]:
+    def parse_framerate(string) -> float | None:
         top, bot = string.split("/")
         bot = float(bot)
         if bot == 0:
             return None
         return float(top) / bot
 
     fps = iterables.safe_unpack(
```

### Comparing `xklb-2.5.9/xklb/media/books.py` & `xklb-2.6.1/xklb/media/books.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os, re
-from typing import List
 
 from xklb.utils import iterables, processes, strings
 from xklb.utils.log_utils import log
 
 REGEX_SENTENCE_ENDS = re.compile(r";|,|\.|\*|\n|\t")
 
 
@@ -221,15 +220,15 @@
 
     if e != {}:
         log.info("Extra data %s", e)
 
     return m
 
 
-def extract_image_metadata_chunk(metadata: List[dict]) -> List[dict]:
+def extract_image_metadata_chunk(metadata: list[dict]) -> list[dict]:
     try:
         import exiftool
     except ModuleNotFoundError:
         print(
             "exiftool and PyExifTool are required for image database creation: sudo dnf install perl-Image-ExifTool && pip install PyExifTool",
         )
         raise
```

### Comparing `xklb-2.5.9/xklb/media/dedupe.py` & `xklb-2.6.1/xklb/media/dedupe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-import argparse, os, re, tempfile
+import argparse, difflib, os, re, shlex, tempfile
+from collections import defaultdict
+from concurrent.futures import ThreadPoolExecutor
 from copy import deepcopy
 from pathlib import Path
-from typing import List
 
 import humanize
 
 from xklb import db_media, usage
 from xklb.media import media_printer
-from xklb.utils import consts, db_utils, devices, file_utils, iterables, objects, strings
+from xklb.scripts import sample_compare, sample_hash
+from xklb.utils import arggroups, consts, db_utils, devices, file_utils, iterables, objects, processes, strings
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library dedupe-media", usage=usage.dedupe_media)
 
+    arggroups.sql_fs(parser)
+
     profile = parser.add_mutually_exclusive_group()
     profile.add_argument(
         "--audio",
         action="store_const",
         dest="profile",
         const=DBType.audio,
         help="Dedupe database by artist + album + title",
@@ -50,14 +54,15 @@
         action="store_const",
         dest="profile",
         const="fts",
         help=argparse.SUPPRESS,
     )
     profile.add_argument(
         "--filesystem",
+        "--fs",
         action="store_const",
         dest="profile",
         const=DBType.filesystem,
         help="Dedupe filesystem database",
     )
     profile.add_argument(
         "--text",
@@ -73,29 +78,41 @@
         dest="profile",
         const=DBType.image,
         help=argparse.SUPPRESS,
         # "Dedupe image database",
     )
     profile.set_defaults(profile="audio")
 
-    parser.add_argument("--only-soft-delete", action="store_true")
+    parser.set_defaults(limit="100")
+
+    parser.add_argument("--no-delete", "--soft-delete", "--mark-deleted", action="store_true")
+    parser.add_argument("--dedupe-cmd", help=argparse.SUPPRESS)
     parser.add_argument("--force", "-f", action="store_true")
-    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default=100)
-    parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--flexible-search", "--or", "--flex", action="store_true")
-    parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--print", "-p", default="", const="p", nargs="?")
-    parser.add_argument("--cols", "-cols", "-col", nargs="*", help="Include a column when printing")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
 
-    parser.add_argument("database")
+    parser.add_argument("--basename", action="store_true")
+    parser.add_argument("--dirname", action="store_true")
+    parser.add_argument(
+        "--min-similarity-ratio",
+        type=float,
+        default=consts.DEFAULT_DIFFLIB_RATIO,
+        help="Filter out matches with less than this ratio. A sane value is in the range of 0.7~0.9",
+    )
+
+    arggroups.debug(parser)
+
+    arggroups.database(parser)
     parser.add_argument("paths", nargs="*")
     args = parser.parse_intermixed_args()
     args.db = db_utils.connect(args)
 
+    args.action = consts.SC.dedupe
+
+    args.sort = "\n        , ".join(filter(bool, args.sort))
+    args.sort = args.sort.replace(",,", ",")
+
     args.filter_sql = []
     args.filter_bindings = {}
 
     COMPARE_DIRS = False
     if len(args.include + args.paths) == 2:
         COMPARE_DIRS = True
         if len(args.include) == 2:
@@ -132,20 +149,19 @@
         )
         for idx, path in enumerate(args.paths):
             args.filter_bindings[f"path{idx}"] = path.replace(" ", "%").replace("%%", " ") + "%"
 
     if not COMPARE_DIRS:
         args.table2 = args.table
 
-    args.action = consts.SC.dedupe
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def get_rows(args) -> List[dict]:
+def get_rows(args) -> list[dict]:
     query = f"""
     SELECT
         {', '.join(db_utils.config["media"]["search_columns"])}
     FROM
         {args.table}
     WHERE 1=1
         and time_deleted = 0
@@ -163,15 +179,15 @@
         , duration DESC
         , path DESC
     """
 
     return args.db.query(query, args.filter_bindings)
 
 
-def get_music_duplicates(args) -> List[dict]:
+def get_music_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
     query = f"""
     SELECT
         m1.path keep_path
         -- , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) num_slash
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
@@ -189,17 +205,18 @@
     WHERE 1=1
         and coalesce(m1.time_deleted,0) = 0 and coalesce(m2.time_deleted,0) = 0
         and m1.title != ''
         {"and m1.artist != ''" if 'artist' in m_columns else ''}
         {"and m1.album != ''" if 'album' in m_columns else ''}
         {" ".join(args.filter_sql)}
     ORDER BY 1=1
+        {', m1.audio_count > 0 DESC' if 'audio_count' in m_columns else ''}
+        {', ' + args.sort if args.sort else ''}
         {', m1.video_count > 0 DESC' if 'video_count' in m_columns else ''}
         {', m1.subtitle_count > 0 DESC' if 'subtitle_count' in m_columns else ''}
-        {', m1.audio_count > 0 DESC' if 'audio_count' in m_columns else ''}
         {', m1.uploader IS NOT NULL DESC' if 'uploader' in m_columns else ''}
         , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) DESC
         , length(m1.path)-length(REPLACE(m1.path, '.', ''))
         , length(m1.path)
         , m1.size DESC
         , m1.time_modified DESC
         , m1.time_created DESC
@@ -208,15 +225,15 @@
     """
 
     media = list(args.db.query(query, args.filter_bindings))
 
     return media
 
 
-def get_id_duplicates(args) -> List[dict]:
+def get_id_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
     query = f"""
     SELECT
         m1.path keep_path
         -- , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) num_slash
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
@@ -231,14 +248,16 @@
         and m2.path != m1.path
     WHERE 1=1
         and coalesce(m1.time_deleted,0) = 0 and coalesce(m2.time_deleted,0) = 0
         and m1.extractor_id != ''
         {" ".join(args.filter_sql)}
     ORDER BY 1=1
         , m1.video_count > 0 DESC
+        , m1.audio_count > 0 DESC
+        {', ' + args.sort if args.sort else ''}
         {', m1.subtitle_count > 0 DESC' if 'subtitle_count' in m_columns else ''}
         , m1.audio_count DESC
         , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) DESC
         , length(m1.path)-length(REPLACE(m1.path, '.', ''))
         , length(m1.path)
         , m1.size DESC
         , m1.time_modified DESC
@@ -248,15 +267,15 @@
     """
 
     media = list(args.db.query(query, args.filter_bindings))
 
     return media
 
 
-def get_title_duplicates(args) -> List[dict]:
+def get_title_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
     query = f"""
     SELECT
         m1.path keep_path
         -- , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) num_slash
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
@@ -270,17 +289,19 @@
         and m1.duration <= m2.duration + 4
     WHERE 1=1
         and coalesce(m1.time_deleted,0) = 0 and coalesce(m2.time_deleted,0) = 0
         and m1.title != '' and m1.title = m2.title
         {" ".join(args.filter_sql)}
     ORDER BY 1=1
         , m1.video_count > 0 DESC
+        , m1.audio_count > 0 DESC
+        {', ' + args.sort if args.sort else ''}
         {', m1.subtitle_count > 0 DESC' if 'subtitle_count' in m_columns else ''}
         , m1.audio_count DESC
-        , m1.uploader IS NOT NULL DESC
+        {', m1.uploader IS NOT NULL DESC' if 'uploader' in m_columns else ''}
         , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) DESC
         , length(m1.path)-length(REPLACE(m1.path, '.', ''))
         , length(m1.path)
         , m1.size DESC
         , m1.time_modified DESC
         , m1.time_created DESC
         , m1.duration DESC
@@ -288,15 +309,15 @@
     """
 
     media = list(args.db.query(query, args.filter_bindings))
 
     return media
 
 
-def get_duration_duplicates(args) -> List[dict]:
+def get_duration_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
     query = f"""
     SELECT
         m1.path keep_path
         -- , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) num_slash
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
@@ -310,17 +331,19 @@
         and m1.duration <= m2.duration + 4
     WHERE 1=1
         and coalesce(m1.time_deleted,0) = 0 and coalesce(m2.time_deleted,0) = 0
         and m1.duration = m2.duration
         {" ".join(args.filter_sql)}
     ORDER BY 1=1
         , m1.video_count > 0 DESC
+        , m1.audio_count > 0 DESC
+        {', ' + args.sort if args.sort else ''}
         {', m1.subtitle_count > 0 DESC' if 'subtitle_count' in m_columns else ''}
         , m1.audio_count DESC
-        , m1.uploader IS NOT NULL DESC
+        {', m1.uploader IS NOT NULL DESC' if 'uploader' in m_columns else ''}
         , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) DESC
         , length(m1.path)-length(REPLACE(m1.path, '.', ''))
         , length(m1.path)
         , m1.size DESC
         , m1.time_modified DESC
         , m1.time_created DESC
         , m1.duration DESC
@@ -328,14 +351,104 @@
     """
 
     media = list(args.db.query(query, args.filter_bindings))
 
     return media
 
 
+def get_fs_duplicates(args) -> list[dict]:
+    m_columns = db_utils.columns(args, "media")
+    query = f"""
+    SELECT
+        path
+        , size
+        {', hash' if 'hash' in m_columns else ''}
+    FROM
+        {args.table} m1
+    WHERE 1=1
+        and coalesce(m1.time_deleted,0) = 0
+        and m1.size > 0
+        {"and type != 'directory'" if 'type' in m_columns else ''}
+        {" ".join(args.filter_sql)}
+    ORDER BY 1=1
+        , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) DESC
+        , length(m1.path)-length(REPLACE(m1.path, '.', ''))
+        , length(m1.path)
+        , m1.size DESC
+        , m1.time_modified DESC
+        , m1.time_created DESC
+        , m1.path DESC
+    """
+    media = list(args.db.query(query, args.filter_bindings))
+
+    size_groups = defaultdict(list)
+    for m in media:
+        size_groups[m["size"]].append(m)
+    size_groups = [l for l in size_groups.values() if len(l) > 1]
+
+    size_paths = {d["path"] for g in size_groups for d in g}
+    media = [d for d in media if d["path"] in size_paths]
+    log.info(
+        "Got %s size duplicates (%s groups). Doing sample-hash comparison...",
+        len(size_paths),
+        len(size_groups),
+    )
+
+    path_media_map = {d["path"]: d for d in media}
+
+    need_sample_hash_paths = [d["path"] for d in media if not d.get("hash")]
+    if need_sample_hash_paths:
+        with ThreadPoolExecutor(max_workers=20) as pool:
+            hash_results = list(pool.map(sample_hash.sample_hash_file, need_sample_hash_paths))
+
+        for path, hash in zip(need_sample_hash_paths, hash_results):
+            if hash is None:
+                del path_media_map[path]
+            else:
+                path_media_map[path]["hash"] = hash
+                args.db["media"].upsert(path_media_map[path], pk=["path"], alter=True)  # save sample-hash back to db
+        media = [path_media_map[d["path"]] for d in media if d["path"] in path_media_map]
+
+    sample_hash_groups = defaultdict(set)
+    for m in media:
+        sample_hash_groups[m["hash"]].add(m["path"])
+    sample_hash_groups = [l for l in sample_hash_groups.values() if len(l) > 1]
+
+    sample_hash_paths = set().union(*sample_hash_groups)
+    log.info(
+        "Got %s sample-hash duplicates (%s groups). Doing full hash comparison...",
+        len(sample_hash_paths),
+        len(sample_hash_groups),
+    )
+
+    with ThreadPoolExecutor(max_workers=20) as pool:
+        path_hash_map = {
+            k: v for k, v in zip(sample_hash_paths, pool.map(sample_compare.full_hash_file, sample_hash_paths))
+        }
+
+    full_hash_groups = defaultdict(list)
+    for path, hash in path_hash_map.items():
+        if hash is not None:
+            full_hash_groups[hash].append(path)
+    full_hash_groups = [l for l in full_hash_groups.values() if len(l) > 1]
+
+    dup_media = []
+    for hash_group_paths in full_hash_groups:
+        paths = [d["path"] for d in media if d["path"] in hash_group_paths]  # get the correct order from media
+        keep_path = paths[0]
+        dup_media.extend(
+            {"keep_path": keep_path, "duplicate_path": p, "duplicate_size": path_media_map[keep_path]["size"]}
+            for p in paths[1:]
+        )
+
+    # TODO: update false-positive sample-hash matches? probably no because then future sample-hash duplicates won't match
+
+    return dup_media
+
+
 def filter_split_files(paths):
     pattern = r"\.\d{3,5}\."
     return filter(lambda x: not re.search(pattern, x), paths)
 
 
 def dedupe_media() -> None:
     args = parse_args()
@@ -345,22 +458,15 @@
     elif args.profile == "extractor_id":
         duplicates = get_id_duplicates(args)
     elif args.profile == "title":
         duplicates = get_title_duplicates(args)
     elif args.profile == "duration":
         duplicates = get_duration_duplicates(args)
     elif args.profile == DBType.filesystem:
-        print(
-            """
-        You should use `rmlint` instead:
-
-            $ rmlint --progress --partial-hidden --rank-by dOma
-        """,
-        )
-        return
+        duplicates = get_fs_duplicates(args)
     elif args.profile == DBType.image:
         print(
             """
         You should use `czkawka` or `cbird` instead:
 
             $ czkawka image -d (pwd) > dupes.txt
             $ wget https://raw.githubusercontent.com/chapmanjacobd/computer/main/bin/czkawka_output_dupdelete.py
@@ -424,14 +530,34 @@
         return
     else:
         raise NotImplementedError
 
     deletion_candidates = []
     deletion_paths = []
     for d in duplicates:
+        if args.dirname and (
+            difflib.SequenceMatcher(
+                None,
+                os.path.dirname(d["keep_path"]),
+                os.path.dirname(d["duplicate_path"]),
+            ).ratio()
+            < args.min_similarity_ratio
+        ):
+            continue
+
+        if args.basename and (
+            difflib.SequenceMatcher(
+                None,
+                os.path.basename(d["keep_path"]),
+                os.path.basename(d["duplicate_path"]),
+            ).ratio()
+            < args.min_similarity_ratio
+        ):
+            continue
+
         if any(
             [
                 d["keep_path"] in deletion_paths or d["duplicate_path"] in deletion_paths,
                 d["keep_path"] == d["duplicate_path"],
                 not Path(d["keep_path"]).resolve().exists(),
             ],
         ):
@@ -461,14 +587,19 @@
     duplicates_size = sum(filter(None, [d["duplicate_size"] for d in duplicates]))
     print(f"Approx. space savings: {humanize.naturalsize(duplicates_size // 2, binary=True)}")
 
     if duplicates and (args.force or devices.confirm("Delete duplicates?")):  # type: ignore
         log.info("Deleting...")
         for d in duplicates:
             path = d["duplicate_path"]
-            if not path.startswith("http") and not args.only_soft_delete:
-                file_utils.trash(path, detach=False)
+            if not path.startswith("http") and not args.no_delete:
+                if args.dedupe_cmd:
+                    processes.cmd(
+                        *shlex.split(args.dedupe_cmd), d["duplicate_path"], d["keep_path"]
+                    )  # follows rmlint interface
+                else:
+                    file_utils.trash(path, detach=False)
             db_media.mark_media_deleted(args, path)
 
 
 if __name__ == "__main__":
     dedupe_media()
```

### Comparing `xklb-2.5.9/xklb/media/media_player.py` & `xklb-2.6.1/xklb/media/media_player.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 from collections import deque
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from platform import system
 from random import randrange
 from shutil import which
 from time import sleep
-from typing import Dict, List, Optional, Tuple
 
 from xklb import db_media, history
 from xklb.media import subtitle
 from xklb.post_actions import post_act
 from xklb.scripts import playback_control
 from xklb.utils import consts, db_utils, devices, iterables, log_utils, mpv_utils, path_utils, processes
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
-def watch_chromecast(args, m: dict, subtitles_file=None) -> Optional[subprocess.CompletedProcess]:
+def watch_chromecast(args, m: dict, subtitles_file=None) -> subprocess.CompletedProcess | None:
     if "vlc" in m["player"]:
         subtitles = ["--sub-file=" + subtitles_file] if subtitles_file else []
         catt_log = processes.cmd(
             "vlc",
             "--sout",
             "#chromecast",
             f"--sout-chromecast-ip={args.cc_ip}",
@@ -42,15 +41,15 @@
                 m["path"],
             )
         else:
             catt_log = args.cc.play_url(m["path"], resolve=True, block=True)
     return catt_log
 
 
-def calculate_duration(args, m) -> Tuple[int, int]:
+def calculate_duration(args, m) -> tuple[int, int]:
     start = 0
     end = m.get("duration") or 0
 
     if args.interdimensional_cable:
         start = randrange(int(start), int(end - args.interdimensional_cable + 1))
         end = start + args.interdimensional_cable
         log.debug("calculate_duration: %s -- %s", start, end)
@@ -85,15 +84,15 @@
         else:
             end = int(args.end)
 
     log.debug("calculate_duration: %s -- %s", start, end)
     return start, end
 
 
-def listen_chromecast(args, m: dict) -> Optional[subprocess.CompletedProcess]:
+def listen_chromecast(args, m: dict) -> subprocess.CompletedProcess | None:
     Path(consts.CAST_NOW_PLAYING).write_text(m["path"])
     catt = which("catt") or "catt"
     start, end = calculate_duration(args, m)
 
     if args.cast_with_local:
         cast_process = subprocess.Popen(
             [
@@ -209,54 +208,54 @@
         with args.db.conn:
             args.db.conn.execute("UPDATE media SET path = ? where path = ?", [transcode_dest, path])
         return transcode_dest
     else:
         return path
 
 
-def get_browser() -> Optional[str]:
+def get_browser() -> str | None:
     default_application = processes.cmd("xdg-mime", "query", "default", "text/html").stdout
     return which(default_application.replace(".desktop", ""))
 
 
-def find_xdg_application(media_file) -> Optional[str]:
+def find_xdg_application(media_file) -> str | None:
     if media_file.startswith("http"):
         return get_browser()
 
     mimetype = processes.cmd("xdg-mime", "query", "filetype", media_file).stdout
     default_application = processes.cmd("xdg-mime", "query", "default", mimetype).stdout
     return which(default_application.replace(".desktop", ""))
 
 
-def generic_player() -> List[str]:
+def generic_player() -> list[str]:
     if platform.system() == "Linux":
         player = ["xdg-open"]
     elif any(p in platform.system() for p in ("Windows", "_NT-", "MSYS")):
         player = ["cygstart"] if shutil.which("cygstart") else ["start", ""]
     else:
         player = ["open"]
     return player
 
 
-def geom_walk(display, v=1, h=1) -> List[List[int]]:
+def geom_walk(display, v=1, h=1) -> list[list[int]]:
     va = display.width // v
     ha = display.height // h
 
     geoms = []
     for v_idx in range(v):
         for h_idx in range(h):
             x = int(va * v_idx)
             y = int(ha * h_idx)
             log.debug("geom_walk %s", {"va": va, "ha": ha, "v_idx": v_idx, "h_idx": h_idx, "x": x, "y": y})
             geoms.append([va, ha, x, y])
 
     return geoms
 
 
-def grid_stack(display, qty, swap=False) -> List[Tuple]:
+def grid_stack(display, qty, swap=False) -> list[tuple]:
     if qty == 1:
         return [("--fs", f'--screen-name="{display.name}"', f'--fs-screen-name="{display.name}"')]
     else:
         dv = sorted(iterables.divisors_upto_sqrt(qty))
         if not dv:
             vh = (qty, 1)
             log.debug("not dv %s", {"dv": dv, "vh": vh})
@@ -330,15 +329,15 @@
                 display.height -= dock_height
 
         return display
     except Exception:
         return display
 
 
-def get_multiple_player_template(args) -> List[Tuple[str, str]]:
+def get_multiple_player_template(args) -> list[tuple[str, str]]:
     import screeninfo
 
     displays = screeninfo.get_monitors()
     if args.screen_name:
         displays = get_display_by_name(displays, args.screen_name)
 
     if args.multiple_playback == consts.DEFAULT_MULTIPLE_PLAYBACK and len(displays) == 1:
@@ -366,15 +365,15 @@
 
     log.debug(players)
 
     return players
 
 
 class MediaPrefetcher:
-    def __init__(self, args, media: List[Dict]):
+    def __init__(self, args, media: list[dict]):
         self.args = argparse.Namespace(**{k: v for k, v in args.__dict__.items() if k not in {"db"}})
         self.media = media
         self.media.reverse()
         self.remaining = len(media)
         self.ignore_paths = set()
         self.futures = deque()
 
@@ -389,15 +388,15 @@
                     future = executor.submit(self.prep_media, m)  # if self.args.prefetch > 1 else []
                     self.ignore_paths.add(m["path"])
                     self.futures.append(future)
                     log.debug("fill prefetch")
                 log.debug("prefetch full")
         return self
 
-    def infer_command(self, m) -> Tuple[List[str], bool]:
+    def infer_command(self, m) -> tuple[list[str], bool]:
         args = self.args
 
         player = generic_player()
         player_need_sleep = True
 
         if getattr(args, "override_player", False):
             player = [*args.override_player]
@@ -465,15 +464,15 @@
 
                 if getattr(args, "interdimensional_cable", False):
                     player.extend(["--save-position-on-quit=no", "--resume-playback=no"])
 
         log.debug("player: %s", player)
         return player, player_need_sleep
 
-    def prep_media(self, m: Dict):
+    def prep_media(self, m: dict):
         t = log_utils.Timer()
         self.args.db = db_utils.connect(self.args)
         log.debug("db.connect: %s", t.elapsed())
 
         m["original_path"] = m["path"]
         if not m["path"].startswith("http"):
             media_path = Path(self.args.prefix + m["path"]).resolve() if self.args.prefix else Path(m["path"])
```

### Comparing `xklb-2.5.9/xklb/media/media_printer.py` & `xklb-2.6.1/xklb/media/media_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import csv, json, os, shlex, statistics
 from copy import deepcopy
 from io import StringIO
 from numbers import Number
 from pathlib import Path
-from typing import Union
 
 from tabulate import tabulate
 
 from xklb import db_media, history
-from xklb.utils import consts, iterables, printing, processes, sql_utils, strings
+from xklb.utils import consts, db_utils, iterables, printing, processes, sql_utils, strings
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def filter_deleted(media):
     http_list = []
     local_list = []
@@ -61,15 +60,15 @@
             historical_hourly = history[0]["total_duration"]
         except IndexError:
             return None
 
     return int(duration / historical_hourly * 60 * 60)
 
 
-def moved_media(args, moved_files: Union[str, list], base_from, base_to) -> int:
+def moved_media(args, moved_files: str | list, base_from, base_to) -> int:
     moved_files = iterables.conform(moved_files)
     modified_row_count = 0
     if moved_files:
         df_chunked = iterables.chunks(moved_files, consts.SQLITE_PARAM_LIMIT)
         for chunk_paths in df_chunked:
             with args.db.conn:
                 cursor = args.db.conn.execute(
@@ -88,42 +87,47 @@
 def media_printer(args, data, units=None, media_len=None) -> None:
     if units is None:
         units = "media"
 
     action = getattr(args, "action", "")
     print_args = getattr(args, "print", "")
     cols = getattr(args, "cols", [])
+    m_columns = db_utils.columns(args, "media")
 
     media = deepcopy(data)
 
     if args.verbose >= consts.LOG_DEBUG and cols and "*" in cols:
         breakpoint()
 
     if not media:
         processes.no_media_found()
 
     if "f" not in print_args and "limit" in getattr(args, "defaults", []):
         media.reverse()
 
+    tables = args.db.table_names()
+
     duration = sum(m.get("duration") or 0 for m in media)
     if "a" in print_args and ("Aggregate" not in media[0].get("path") or ""):
         if "count" in media[0]:
             D = {"path": "Aggregate", "count": sum(d.get("count") or 0 for d in media)}
+        elif "exists" in media[0]:
+            D = {"path": "Aggregate", "count": sum(d.get("exists") or 0 for d in media)}
         elif action == SC.download_status and "never_downloaded" in media[0]:
             potential_downloads = sum(d["never_downloaded"] + d["retry_queued"] for d in media)
             D = {"path": "Aggregate", "count": potential_downloads}
         else:
             D = {"path": "Aggregate", "count": len(media)}
 
         if "duration" in media[0] and action not in (SC.download_status):
             D["duration"] = duration
             D["avg_duration"] = duration / len(media)
 
-        if hasattr(args, "action"):
-            if action in (SC.download, SC.download_status):
+        if hasattr(args, "action") and "history" in tables:
+            if action in (SC.download, SC.download_status) and "time_downloaded" in m_columns:
                 D["download_duration"] = cadence_adjusted_items(args, D["count"], time_column="time_downloaded")
             else:
                 if duration > 0:
                     D["cadence_adj_duration"] = cadence_adjusted_duration(args, duration)
                 else:
                     D["cadence_adj_duration"] = cadence_adjusted_items(args, D["count"])
 
@@ -146,15 +150,20 @@
             marked = db_media.mark_media_deleted(args, [d["path"] for d in media])
             log.warning(f"Marked {marked} metadata records as deleted")
 
         if "w" in print_args:
             marked = history.add(args, [d["path"] for d in media])
             log.warning(f"Marked {marked} metadata records as watched")
 
-    if "a" not in print_args and action == SC.download_status:
+    if (
+        "a" not in print_args
+        and "history" in tables
+        and action == SC.download_status
+        and "time_downloaded" in m_columns
+    ):
         for m in media:
             m["download_duration"] = cadence_adjusted_items(
                 args, m["never_downloaded"] + m["retry_queued"], time_column="time_downloaded"
             )  # TODO where= p.extractor_key, or try to use SQL
 
     for k, v in list(media[0].items()):
         if k.endswith("size"):
```

### Comparing `xklb-2.5.9/xklb/media/subtitle.py` & `xklb-2.6.1/xklb/media/subtitle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import re, tempfile
 from pathlib import Path
-from typing import List, Optional
 
 import ffmpeg
 
 from xklb.utils import db_utils, iterables, processes, strings
 from xklb.utils.consts import SUB_TEMP_DIR
 from xklb.utils.log_utils import log
 
 SUBTITLE_FORMATS = "vtt|srt|ssa|ass|jss|aqt|mpl2|mpsub|pjs|rt|sami|smi|stl|xml|txt|psb|ssf|usf"
 IMAGE_SUBTITLE_CODECS = ["dvbsub", "dvdsub", "pgssub", "xsub", "dvb_subtitle", "dvd_subtitle", "hdmv_pgs_subtitle"]
 SUBSTATION_OVERRIDE_TAG = re.compile(r"{[^}]*}")
 
 
-def extract_from_video(path, stream_index) -> Optional[str]:
+def extract_from_video(path, stream_index) -> str | None:
     Path(SUB_TEMP_DIR).mkdir(parents=True, exist_ok=True)
     temp_srt = tempfile.mktemp(".srt", dir=SUB_TEMP_DIR)
 
     stream_id = "0:" + str(stream_index)
 
     try:
         ffmpeg.input(path).output(temp_srt, map=stream_id).global_args("-nostdin").run(quiet=True)
@@ -93,48 +92,48 @@
         return read_sub_unsafe(convert_to_srt(path))
 
 
 def is_text_subtitle_stream(s) -> bool:
     return s.get("codec_type") == "subtitle" and s.get("codec_name") not in IMAGE_SUBTITLE_CODECS
 
 
-def externalize_internal_subtitles(path, streams=None) -> List[str]:
+def externalize_internal_subtitles(path, streams=None) -> list[str]:
     if streams is None:
         streams = processes.FFProbe(path).streams
 
     external_paths = iterables.conform(
         [extract_from_video(path, s["index"]) for s in streams if is_text_subtitle_stream(s)],
     )
 
     return external_paths
 
 
-def get_external(file) -> List[str]:
+def get_external(file) -> list[str]:
     p = Path(file)
 
     subtitles = [
         str(sub_p) for sub_p in p.parent.glob(p.stem + "*") if sub_p.suffix[1:].lower() in SUBTITLE_FORMATS.split("|")
     ]
 
     if subtitles:
         return subtitles
 
     return []
 
 
-def get_subtitle_paths(path) -> List[str]:
+def get_subtitle_paths(path) -> list[str]:
     internal_subtitles = externalize_internal_subtitles(path)
     if len(internal_subtitles) > 0:
         return internal_subtitles
 
     external_subtitles = get_external(path)
     return external_subtitles
 
 
-def get_sub_index(args, path) -> Optional[int]:
+def get_sub_index(args, path) -> int | None:
     probe = processes.FFProbe(path)
     temp_db = db_utils.connect(args, memory=True)
     temp_db["streams"].insert_all(probe.streams, pk="index")  # type: ignore
     subtitle_index = temp_db.pop(
         f"""select "index" from streams
             where codec_type = "subtitle"
               and codec_name not in ({",".join(['?'] * len(IMAGE_SUBTITLE_CODECS))})
```

### Comparing `xklb-2.5.9/xklb/scratch/javguru.py` & `xklb-2.6.1/xklb/scratch/javguru.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import argparse, time
 from pathlib import Path
 from urllib.parse import urljoin
 
 from xklb.media import media_check
-from xklb.utils import file_utils, path_utils, processes, web
+from xklb.utils import arggroups, file_utils, path_utils, processes, web
 
 
 def jav_guru() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument("--chrome", action="store_true")
     parser.add_argument("--small", action="store_true")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
     parser.add_argument("path", help="JAV.GURU URL")
     args = parser.parse_args()
 
     from selenium.common.exceptions import NoSuchElementException
     from selenium.webdriver.common.by import By
```

### Comparing `xklb-2.5.9/xklb/scratch/javtiful.py` & `xklb-2.6.1/xklb/scratch/javtiful.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import argparse, time
 from pathlib import Path
 
 from xklb.media import media_check
-from xklb.utils import file_utils, path_utils, processes, web
+from xklb.utils import arggroups, file_utils, path_utils, processes, web
 
 
 def javtiful() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument("--chrome", action="store_true")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
     parser.add_argument("path")
     args = parser.parse_args()
 
     from selenium.webdriver.common.by import By
 
     def process_url(line):
```

### Comparing `xklb-2.5.9/xklb/scratch/mam_search.py` & `xklb-2.6.1/xklb/scratch/mam_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import argparse, json, time
 from pathlib import Path
 from sqlite3 import IntegrityError
 
-from xklb.utils import db_utils, nums, objects, web
+from xklb.utils import arggroups, db_utils, nums, objects, web
 from xklb.utils.log_utils import log
 
 
 def parse_args():
     parser = argparse.ArgumentParser()
-    parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--base-url", default="https://www.myanonamouse.net")
     parser.add_argument("--no-title", action="store_false")
     parser.add_argument("--no-author", action="store_false")
     parser.add_argument("--narrator", action="store_true")
     parser.add_argument("--series", action="store_true")
     parser.add_argument("--description", action="store_true")
 
@@ -22,18 +21,18 @@
     parser.add_argument("--cookbooks", action="store_true")
     parser.add_argument("--musicology", action="store_true")
     parser.add_argument("--radio", action="store_true")
 
     parser.add_argument("--search-in", default="torrents")
 
     parser.add_argument("--cookie", required=True)
-    parser.add_argument("--cookies", help="path to a Netscape formatted cookies file")
-    parser.add_argument("--cookies-from-browser", metavar="BROWSER[+KEYRING][:PROFILE][::CONTAINER]")
+    arggroups.requests(parser)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     parser.add_argument("search_text", nargs="+")
     args = parser.parse_intermixed_args()
 
     Path(args.database).touch()
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
```

### Comparing `xklb-2.5.9/xklb/scratch/mam_slots.py` & `xklb-2.6.1/xklb/scratch/mam_slots.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import argparse
 
-from xklb.utils import objects, web
+from xklb.utils import arggroups, objects, web
 from xklb.utils.log_utils import log
 
 
 def parse_args():
     parser = argparse.ArgumentParser()
-    parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--base-url", default="https://www.myanonamouse.net")
     parser.add_argument("--max", type=int, default=150)
 
     parser.add_argument("--cookie", required=True)
-    parser.add_argument("--cookies", help="path to a Netscape formatted cookies file")
-    parser.add_argument("--cookies-from-browser", metavar="BROWSER[+KEYRING][:PROFILE][::CONTAINER]")
+    arggroups.requests(parser)
+    arggroups.debug(parser)
+
     args = parser.parse_args()
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def get_unsat(args):
```

### Comparing `xklb-2.5.9/xklb/scripts/big_dirs.py` & `xklb-2.6.1/xklb/scripts/big_dirs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,54 @@
 import argparse, os
 from pathlib import Path
-from typing import Dict, List
 
 from xklb import history, usage
 from xklb.media import media_printer
 from xklb.scripts import mcda
-from xklb.utils import arg_utils, consts, db_utils, file_utils, nums, objects, sql_utils
+from xklb.utils import arg_utils, arggroups, consts, db_utils, file_utils, nums, objects, sql_utils
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library big_dirs",
         usage=usage.big_dirs,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument("--sort-groups-by", "--sort-groups", "--sort-by", "--sort", "-u", nargs="+")
-    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="4000")
-    parser.add_argument("--depth", "-d", default=0, type=int, help="Depth of folders")
-    parser.add_argument("--lower", type=int, default=4, help="Minimum number of files per folder")
-    parser.add_argument("--upper", type=int, help="Maximum number of files per folder")
-    parser.add_argument(
-        "--folder-size",
-        "--foldersize",
-        "-Z",
-        action="append",
-        help="Only include folders of specific sizes (uses the same syntax as fd-find)",
-    )
-    parser.add_argument(
-        "--size",
-        "-S",
-        action="append",
-        help="Only include files of specific sizes (uses the same syntax as fd-find)",
-    )
-    parser.add_argument("--include", "-s", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--cluster-sort", action="store_true", help="Cluster by filename instead of grouping by folder")
-    parser.add_argument("--clusters", "--n-clusters", "-c", type=int, help="Number of KMeans clusters")
-    parser.add_argument("--print", "-p", default="", const="p", nargs="?")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.sql_fs(parser)
+    arggroups.operation_cluster(parser)
+    arggroups.operation_group_folders(parser)
+    parser.set_defaults(limit="4000", lower=4, depth=0)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
     args.db = db_utils.connect(args)
 
-    if args.sort_groups_by:
-        args.sort_groups_by = arg_utils.parse_ambiguous_sort(args.sort_groups_by)
-        args.sort_groups_by = ",".join(args.sort_groups_by)
-
     args.include += args.search
     if args.include == ["."]:
         args.include = [str(Path().cwd().resolve())]
 
     if len(args.include) == 1 and os.sep in args.include[0]:
         args.include = [file_utils.resolve_absolute_path(args.include[0])]
 
+    if args.sort_groups_by:
+        args.sort_groups_by = arg_utils.parse_ambiguous_sort(args.sort_groups_by)
+        args.sort_groups_by = ",".join(args.sort_groups_by)
+
     if args.size:
         args.size = sql_utils.parse_human_to_sql(nums.human_to_bytes, "size", args.size)
 
     args.action = consts.SC.bigdirs
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def group_files_by_folder(args, media) -> List[Dict]:
+def group_files_by_folder(args, media) -> list[dict]:
     p_media = {}
     for m in media:
         p = m["path"].split(os.sep)
         while len(p) >= 2:
             p.pop()
             parent = os.sep.join(p) + os.sep
 
@@ -97,15 +77,15 @@
                 d.pop(path)
             elif args.upper and pdict["exists"] > args.upper:
                 d.pop(path)
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
-def folder_depth(args, folders) -> List[Dict]:
+def folder_depth(args, folders) -> list[dict]:
     d = {}
     for f in folders:
         p = f["path"].split(os.sep)
         p.pop()
 
         depth = 1 + args.depth
         parent = os.sep.join(p[:depth]) + os.sep
@@ -126,15 +106,15 @@
             d.pop(path)
         elif args.upper is not None and pdict["exists"] > args.upper:
             d.pop(path)
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
-def get_table(args) -> List[dict]:
+def get_table(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
     args.filter_sql = []
     args.filter_bindings = {}
 
     if args.size:
         args.filter_sql.append(" and size IS NOT NULL " + args.size)
     db_utils.construct_search_bindings(
@@ -160,15 +140,15 @@
         """,
             args.filter_bindings,
         ),
     )
     return media
 
 
-def process_big_dirs(args, folders) -> List[Dict]:
+def process_big_dirs(args, folders) -> list[dict]:
     folders = [d for d in folders if d["total"] != d["deleted"]]  # remove folders where all deleted
 
     if args.depth:
         folders = folder_depth(args, folders)
     if args.folder_size:
         args.folder_size = sql_utils.parse_human_to_lambda(nums.human_to_bytes, args.folder_size)
         folders = [d for d in folders if args.folder_size(d["size"])]
```

### Comparing `xklb-2.5.9/xklb/scripts/block.py` & `xklb-2.6.1/xklb/scripts/block.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,41 @@
 import argparse, sys
 
 import humanize
 
 from xklb import post_actions, tube_backend, usage
 from xklb.media import media_printer
-from xklb.utils import consts, db_utils, devices, iterables, objects
+from xklb.utils import arggroups, consts, db_utils, devices, iterables, objects
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         prog="library block",
         usage=usage.block,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument("--print", "-p", default="", const="p", nargs="?", help=argparse.SUPPRESS)
-    parser.add_argument("--cols", "-cols", "-col", nargs="*", help="Include a column when printing")
-    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", help=argparse.SUPPRESS)
+    arggroups.sql_fs(parser)
+
     parser.add_argument("--match-column", "-c", default="path", help="Column to block media if text matches")
 
     parser.add_argument("--cluster", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--min-tried", default=0, type=int, help=argparse.SUPPRESS)
     parser.add_argument("--no-confirm", "--yes", "-y", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--force", "-f", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument(
-        "--delete",
-        "--remove",
-        "--erase",
-        "--rm",
-        "-rm",
-        action="store_true",
-        help="Delete matching rows",
-    )
+    arggroups.capability_delete(parser)
     parser.add_argument("--offline", "--no-tube", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
-    parser.add_argument("database", help=argparse.SUPPRESS)
-    parser.add_argument("playlists", nargs="*", help=argparse.SUPPRESS)
+    arggroups.database(parser)
+    parser.add_argument("playlists", nargs="*")
     args = parser.parse_intermixed_args()
 
-    if args.db:
-        args.database = args.db
     args.db = db_utils.connect(args)
 
     args.playlists = iterables.conform(args.playlists)
 
     args.action = SC.block
     log.info(objects.dict_filter_bool(args.__dict__))
 
@@ -71,15 +59,15 @@
     args = parse_args()
     m_columns = db_utils.columns(args, "media")
     if args.match_column not in m_columns:
         raise ValueError(
             "Match column does not exist in the media table. You may need to run tubeadd first or check your spelling",
         )
 
-    columns = set(["path", "webpath", args.match_column, "size", "playlist_path", "time_deleted"])
+    columns = {"path", "webpath", args.match_column, "size", "playlist_path", "time_deleted"}
     select_sql = ", ".join(s for s in columns if s in m_columns)
 
     if not args.playlists:
         if "blocklist" in args.db.table_names():
             deleted_count = 0
             blocklist = [(d["key"], d["value"]) for d in args.db["blocklist"].rows if d["key"] in m_columns]
             # TODO: add support for playlists table block rules
```

### Comparing `xklb-2.5.9/xklb/scripts/christen.py` & `xklb-2.6.1/xklb/scripts/christen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import argparse, shutil
 from os import fsdecode
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import objects, path_utils
+from xklb.utils import arggroups, objects, path_utils
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library christen", usage=usage.christen)
     parser.add_argument("--dot-space", action="store_true")
     parser.add_argument("--case-insensitive", action="store_true")
     parser.add_argument("--lowercase-folders", action="store_true")
     parser.add_argument("--overwrite", "-f", action="store_true")
     parser.add_argument("--run", "-r", action="store_true")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
     parser.add_argument("paths", nargs="*")
     args = parser.parse_args()
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
```

### Comparing `xklb-2.5.9/xklb/scripts/cluster_sort.py` & `xklb-2.6.1/xklb/scripts/cluster_sort.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import argparse, difflib, json, os.path, sys
 from collections import Counter
 from pathlib import Path
-from typing import Dict, List
 
 from xklb import usage
 from xklb.data import wordbank
 from xklb.scripts import eda, mcda
-from xklb.utils import consts, db_utils, file_utils, iterables, nums, objects, printing, strings
+from xklb.utils import arggroups, consts, db_utils, file_utils, iterables, nums, objects, printing, strings
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import Timer, log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library cluster-sort", usage=usage.cluster_sort)
 
@@ -52,25 +51,17 @@
         action="store_const",
         dest="profile",
         const=DBType.text,
         help="Read text data",
     )
     parser.set_defaults(profile="lines")
 
-    parser.add_argument("--stop-words", "--ignore-words", "--ignore", "-i", nargs="+", action="append")
-
-    parser.add_argument("--clusters", "--n-clusters", "-c", type=int, help="Number of KMeans clusters")
-    parser.add_argument("--near-duplicates", "--similar-only", action="store_true", help="Re-group by difflib ratio")
-    parser.add_argument(
-        "--unique-only", action="store_true", help="Include only 'unique' lines (not including originals or duplicates)"
-    )
-    parser.add_argument("--exclude-unique", "--no-unique", action="store_true", help="Exclude 'unique' lines")
-    parser.add_argument("--print-groups", "--groups", "-g", action="store_true", help="Print groups")
-    parser.add_argument("--move-groups", "-M", action="store_true", help="Move groups into subfolders")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.operation_cluster(parser)
+    parser.set_defaults(cluster_sort=True)
+    arggroups.debug(parser)
 
     parser.add_argument("input_path", nargs="?", type=argparse.FileType("r"), default=sys.stdin)
     parser.add_argument("output_path", nargs="?")
     args = parser.parse_args()
 
     if args.stop_words is None:
         args.stop_words = wordbank.stop_words
@@ -229,15 +220,15 @@
                 s for d in groups for s in d["grouped_paths"] if not bool(media_keyed[s].get("time_deleted"))
             )
     else:
         sorted_paths = iterables.flatten(
             s for d in groups for s in d["grouped_paths"] if not bool(media_keyed[s].get("time_deleted"))
         )
 
-    if args.print_groups:
+    if getattr(args, "print_groups", False):
         print_groups(groups)
 
     media = [media_keyed[p] for p in sorted_paths]
     return media
 
 
 def cluster_images(paths, n_clusters=None):
@@ -306,27 +297,27 @@
         }
         result.append(metadata)
     log.info("common_prefix %s", t.elapsed())
 
     return result
 
 
-def filter_near_duplicates(groups: List[Dict]) -> List[Dict]:
+def filter_near_duplicates(groups: list[dict]) -> list[dict]:
     regrouped_data = []
 
     for group in groups:
-        temp_groups: Dict[str, List[str]] = {}
+        temp_groups: dict[str, list[str]] = {}
         for curr in group["grouped_paths"]:
             curr = curr.strip()
             if not curr or curr in ["'", '"']:
                 continue
 
             is_duplicate = False
             for prev in temp_groups.keys():
-                if difflib.SequenceMatcher(None, curr, prev).ratio() > 0.73:
+                if difflib.SequenceMatcher(None, curr, prev).ratio() > consts.DEFAULT_DIFFLIB_RATIO:
                     temp_groups[prev].append(curr)
                     is_duplicate = True
                     break
             if not is_duplicate:
                 temp_groups[curr] = []
 
         sorted_temp_groups = sorted(temp_groups.items(), key=lambda t: len(t[1]))
@@ -355,15 +346,15 @@
         groups = filter_near_duplicates(groups)
 
     if args.exclude_unique:
         groups = [d for d in groups if len(d["grouped_paths"]) > 1]
     elif args.unique_only:
         groups = [d for d in groups if len(d["grouped_paths"]) == 1]
 
-    if args.print_groups:
+    if getattr(args, "print_groups", False):
         print_groups(groups)
     elif args.move_groups:
         min_len = len(str(len(groups) + 1))
 
         if args.profile == "lines":
             if args.output_path:
                 output_parent = Path(args.output_path).parent
```

### Comparing `xklb-2.5.9/xklb/scripts/copy_play_counts.py` & `xklb-2.6.1/xklb/scripts/copy_play_counts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import argparse
 from pathlib import Path
 
 from xklb import history, usage
 from xklb.scripts.dedupe_db import dedupe_rows
-from xklb.utils import db_utils, objects
+from xklb.utils import arggroups, db_utils, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library copy-play-counts", usage=usage.copy_play_counts)
-    parser.add_argument("database")
-    parser.add_argument("source_dbs", nargs="+")
     parser.add_argument("--source-prefix", default="")
     parser.add_argument("--target-prefix", default="")
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
+
+    arggroups.database(parser)
+    parser.add_argument("source_dbs", nargs="+")
     args = parser.parse_intermixed_args()
 
-    if args.db:
-        args.database = args.db
     Path(args.database).touch()
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
 
     return args
```

### Comparing `xklb-2.5.9/xklb/scripts/dedupe_czkawka.py` & `xklb-2.6.1/xklb/scripts/dedupe_czkawka.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,41 +3,39 @@
 from pathlib import Path
 
 import humanize
 from screeninfo import get_monitors
 
 from xklb import post_actions
 from xklb.media import media_player
-from xklb.utils import consts, devices, file_utils, iterables, mpv_utils, processes
+from xklb.utils import arggroups, consts, devices, file_utils, iterables, mpv_utils, processes
 from xklb.utils.log_utils import log
 
 left_mpv_socket = str(Path(consts.TEMP_SCRIPT_DIR) / f"mpv_socket_{consts.random_string()}")
 right_mpv_socket = str(Path(consts.TEMP_SCRIPT_DIR) / f"mpv_socket_{consts.random_string()}")
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Choose which duplicate to keep by opening both side-by-side in mpv")
+    arggroups.playback(parser)
+    arggroups.capability_clobber(parser)
+    arggroups.post_actions(parser)
+    parser.set_defaults(start="15%", volume="70")
+
     parser.add_argument(
         "--auto-select-min-ratio",
         type=float,
         default=1.0,
         help="Automatically select largest file if files have similar basenames. A sane value is in the range of 0.7~0.9",
     )
-    parser.add_argument("--start", default="15%")
-    parser.add_argument("--volume", default="70", type=float)
-    parser.add_argument("--keep-dir", "--keepdir", help=argparse.SUPPRESS)
-    parser.add_argument("--exit-code-confirm", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--gui", action="store_true")
-    parser.add_argument("--auto-seek", action="store_true")
-    parser.add_argument("--override-player", "--player", "-player", help=argparse.SUPPRESS)
     parser.add_argument("--all-keep", action="store_true")
     parser.add_argument("--all-left", action="store_true")
     parser.add_argument("--all-right", action="store_true")
     parser.add_argument("--all-delete", action="store_true")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
     parser.add_argument("file_path", help="Path to the text file containing the file list.")
     args = parser.parse_args()
     return args
 
 
 def backup_and_read_file(file_path):
```

### Comparing `xklb-2.5.9/xklb/scripts/dedupe_db.py` & `xklb-2.6.1/xklb/scripts/dedupe_db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import argparse
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arg_utils, db_utils, objects
+from xklb.utils import arggroups, argparse_utils, db_utils, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library dedupe-dbs", usage=usage.dedupe_db)
     parser.add_argument("--skip-upsert", action="store_true")
     parser.add_argument("--skip-0", action="store_true")
-    parser.add_argument("--only-columns", action=arg_utils.ArgparseList, help="Comma separated column names to upsert")
-    parser.add_argument("--primary-keys", "--pk", action=arg_utils.ArgparseList, help="Comma separated primary keys")
+    parser.add_argument(
+        "--only-columns", action=argparse_utils.ArgparseList, help="Comma separated column names to upsert"
+    )
+    parser.add_argument(
+        "--primary-keys", "--pk", action=argparse_utils.ArgparseList, help="Comma separated primary keys"
+    )
     parser.add_argument(
         "--business-keys",
         "--bk",
-        action=arg_utils.ArgparseList,
+        action=argparse_utils.ArgparseList,
         required=True,
         help="Comma separated business keys",
     )
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     parser.add_argument("table")
     args = parser.parse_intermixed_args()
 
-    if args.db:
-        args.database = args.db
     Path(args.database).touch()
     args.db = db_utils.connect(args)
 
     log.info(objects.dict_filter_bool(args.__dict__))
 
     return args
```

### Comparing `xklb-2.5.9/xklb/scripts/download_status.py` & `xklb-2.6.1/xklb/scripts/download_status.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,34 @@
 import argparse
 
 from xklb import dl_extract, tube_backend, usage
 from xklb.media import media_printer
-from xklb.utils import arg_utils, consts, db_utils, objects, sql_utils
+from xklb.utils import arg_utils, arggroups, consts, db_utils, objects, sql_utils
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         "library download-status",
         usage=usage.download_status,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument("--print", "-p", default="p", const="p", nargs="?", help=argparse.SUPPRESS)
-    parser.add_argument("--cols", "-cols", "-col", nargs="*", help="Include a column when printing")
-    parser.add_argument("--sort", "-u", nargs="+", help=argparse.SUPPRESS)
-    parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--duration", "-d", action="append", help=argparse.SUPPRESS)
-    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", help=argparse.SUPPRESS)
-    parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
-    parser.add_argument(
-        "--retry-delay",
-        "-r",
-        default="14 days",
-        help="Must be specified in SQLITE Modifiers format: N hours, days, months, or years",
-    )
 
-    parser.add_argument("-v", "--verbose", action="count", default=0)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
+    arggroups.sql_fs(parser)
+    arggroups.sql_media(parser)
+
+    parser.set_defaults(print="p")
+
+    arggroups.download(parser)
 
-    parser.add_argument("database")
+    arggroups.debug(parser)
+    arggroups.database(parser)
     args = parser.parse_args()
     args.defaults = []
 
-    if args.db:
-        args.database = args.db
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
 
     args.action = consts.SC.download_status
     return args
```

### Comparing `xklb-2.5.9/xklb/scripts/eda.py` & `xklb-2.6.1/xklb/scripts/mcda.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,179 @@
 import argparse
-from typing import Dict
+from pathlib import Path
 
 from xklb import usage
-from xklb.utils import file_utils, nums
+from xklb.utils import arggroups, argparse_utils, file_utils, iterables, objects, pd_utils, sql_utils
 from xklb.utils.consts import DEFAULT_FILE_ROWS_READ_LIMIT
 from xklb.utils.log_utils import log
 from xklb.utils.printing import print_df, print_series
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(description="Perform EDA on one or more files", usage=usage.eda)
-    parser.add_argument("--groupby", "--group-by", "-g", action="store_true")
-    parser.add_argument("--mimetype", "--filetype")
-    parser.add_argument("--encoding")
-    parser.add_argument("--table-name", "--table", "-t")
-    parser.add_argument("--table-index", type=int)
-    parser.add_argument("--start-row", "--skiprows", type=int, default=None)
-    parser.add_argument("--end-row", "--nrows", "--limit", "-L", default=str(DEFAULT_FILE_ROWS_READ_LIMIT))
+    parser = argparse.ArgumentParser(description="Perform MCDA on one or more files", usage=usage.mcda)
+    arggroups.table_like(parser)
+    parser.add_argument(
+        "--minimize-columns",
+        "--minimize-cols",
+        "--minimize",
+        "--min",
+        nargs="*",
+        action=argparse_utils.ArgparseList,
+        default=[],
+    )
+    parser.add_argument(
+        "--columns-exclude",
+        "--exclude-columns",
+        "--ignore-columns",
+        nargs="*",
+        action=argparse_utils.ArgparseList,
+        default=[],
+    )
+    parser.add_argument(
+        "--columns-include",
+        "--include-columns",
+        "--columns",
+        "--cols",
+        nargs="*",
+        action=argparse_utils.ArgparseList,
+        default=[],
+    )
+    parser.add_argument("--words-nums-map")
+    parser.add_argument("--mcda-method")
+    parser.add_argument("--nodata", type=int, default=0)
+    parser.add_argument("--clean", action="store_true")
     parser.add_argument("--sort", "-u", default="random()")
-    parser.add_argument("--repl", "-r", action="store_true")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
     parser.add_argument(
         "paths",
         metavar="path",
         nargs="+",
         help="path to one or more files",
     )
     args = parser.parse_args()
 
     if args.end_row.lower() in ("inf", "none", "all"):
         args.end_row = None
     else:
         args.end_row = int(args.end_row)
 
-    return args
+    if args.words_nums_map:
+        Path(args.words_nums_map).touch()
 
+    log.info(objects.dict_filter_bool(args.__dict__))
+    return args
 
-def df_column_values(df, column_name) -> Dict:
-    total = len(df)
 
-    null = df[column_name].isnull().sum()
-    zero = (df[column_name] == 0).sum()
-    empty = (df[column_name] == "").sum()
-    values = total - empty - zero - null
-
-    return {
-        "values_count": values,
-        "null_count": null,
-        "zero_count": zero,
-        "empty_string_count": empty,
-        "column": column_name,
-        "null": f"{null} ({nums.percent(null, total):.1f}%)",
-        "zero": f"{zero} ({nums.percent(zero, total):.1f}%)",
-        "empty_string": f"{empty} ({nums.percent(empty, total):.1f}%)",
-        "values": f"{values} ({nums.percent(values, total):.1f}%)",
+def words_to_numbers(args, words):
+    default = {
+        "high": 5,
+        "above average": 4,
+        "average": 3,
+        "below average": 2,
+        "low": 1,
     }
 
+    numbers = []
+    with objects.json_shelve(args.words_nums_map, default) as mappings:
+        for word in words:
+            word = word.lower()
 
-def print_info(args, df):
+            try:
+                number = mappings[word]
+            except KeyError:  # word not in mappings
+                number = int(input(f"Enter a number for '{word}': "))
+                mappings[word] = number  # save it for the future
+
+            numbers.append(number)
+
+    return numbers
+
+
+def borda(df, weights):
+    import numpy as np
+
+    m, n = df.shape
+    matrix = np.array(df)
+    borda_matrix = np.empty((m, n))
+    for i in range(n):
+        borda_matrix[:, i] = m - matrix[:, i]
+    w_borda_matrix = borda_matrix * weights
+
+    borda_points = np.sum(w_borda_matrix, axis=1)
+    return borda_points
+
+
+def auto_mcda(args, df, alternatives, minimize_cols):
+    import numpy as np
     import pandas as pd
+    from pymcdm import weights as w
+    from pymcdm.methods import MABAC, SPOTIS, TOPSIS
+
+    goal_directions = np.array([-1 if col in minimize_cols else 1 for col in alternatives.columns])
+    alternatives_np = alternatives.fillna(getattr(args, "nodata", None) or 0).to_numpy()
+    methods = [TOPSIS(), MABAC(), SPOTIS(SPOTIS.make_bounds(alternatives_np))]
+    method_names = ["TOPSIS", "MABAC", "SPOTIS"]
+    votes = []
+    for method in methods:
+        # TODO: --weights flag to override
+        weights = w.entropy_weights(alternatives_np)
+        pref = method(alternatives_np, weights, goal_directions)
+        votes.append(pref)
+    votes_df = pd.DataFrame(zip(*votes), columns=method_names)
+    borda_points = borda(votes_df, weights=[1] * len(votes))
+    borda_df = pd.DataFrame({"BORDA": borda_points}, index=df.index)
+
+    # TODO: PCA option and warning if a criterion accounts for less than 3% of variance
+
+    df = pd.concat((df, votes_df, borda_df), axis=1)
+    df = df.sort_values(getattr(args, "mcda_method", None) or "TOPSIS", ascending=False)
+    return df
+
+
+def sort(args, df, values):
+    columns = []
+    if isinstance(values, str):
+        columns.extend(values.split(","))
+    else:
+        columns.extend(iterables.flatten(s.split(",") for s in values))
 
+    if columns:
+        included_columns = [s.lstrip("-") for s in columns]
+        alternatives = df[included_columns]
+    else:
+        alternatives = df.select_dtypes("number")
+
+    df = auto_mcda(args, df, alternatives, minimize_cols={s.lstrip("-") for s in columns if s.startswith("-")})
+    return df
+
+
+def group_sort_by(args, folders):
+    if args.sort_groups_by is None:
+        sort_func = lambda x: x["size"] / x["exists"]
+    elif args.sort_groups_by.startswith("mcda "):
+        import pandas as pd
+
+        if not isinstance(folders, pd.DataFrame):
+            folders = pd.DataFrame(folders)
+        values = args.sort_groups_by.replace("mcda ", "", 1)
+        df = sort(args, folders, values)
+        return df.drop(columns=["TOPSIS", "MABAC", "SPOTIS", "BORDA"]).to_dict(orient="records")
+    else:
+        if args.sort_groups_by == "played_ratio":
+            sort_func = lambda x: x["played"] / x["deleted"] if x["deleted"] else 0
+        elif args.sort_groups_by == "deleted_ratio":
+            sort_func = lambda x: x["deleted"] / x["played"] if x["played"] else 0
+        else:
+            sort_func = sql_utils.sort_like_sql(args.sort_groups_by)
+
+    return sorted(folders, key=sort_func)
+
+
+def print_info(args, df):
     if df.shape == (0, 0):
         print(f"Table [{df.name}] empty")
         return
 
     if args.end_row is None:
         partial_dataset_msg = ""
     elif args.end_row == DEFAULT_FILE_ROWS_READ_LIMIT:
@@ -74,143 +183,85 @@
     if args.end_row is not None and args.end_row not in df.shape:
         partial_dataset_msg = ""
     print("### Shape")
     print()
     print(df.shape, partial_dataset_msg)
     print()
 
-    print("### Sample of rows")
-    if len(df) > 6:
-        print_df(pd.concat([df.head(3), df.tail(3)]))
-    else:
-        print_df(df.head(6))
-
-    print("### Summary statistics")
-    print_df(df.describe())
-
-    converted = df.convert_dtypes()
-    same_dtypes = []
-    diff_dtypes = []
-    for col in df.columns:
-        if df.dtypes[col] == converted.dtypes[col]:
-            same_dtypes.append((col, df.dtypes[col]))
-        else:
-            diff_dtypes.append((col, df.dtypes[col], converted.dtypes[col]))
-    if len(same_dtypes) > 0:
-        print("### Pandas columns with 'original' dtypes")
-        same_dtypes = pd.DataFrame(same_dtypes, columns=["column", "dtype"])
-        print_df(same_dtypes.set_index("column"))
-    if len(diff_dtypes) > 0:
-        print("### Pandas columns with 'converted' dtypes")
-        diff_dtypes = pd.DataFrame(diff_dtypes, columns=["column", "original_dtype", "converted_dtype"])
-        print_df(diff_dtypes.set_index("column"))
-
-    if len(df) > 15:
-        numeric_columns = df.select_dtypes("number").columns.to_list()
-        if numeric_columns:
-            print("### Numerical columns")
-            print()
-            print("#### Bins")
-            print()
-            for col in numeric_columns:
-                try:
-                    bins = pd.cut(df[col], bins=6)
-                    print_df(bins.value_counts().sort_index())
-                except TypeError:  # putmask: first argument must be an array
-                    log.warning("Could not calculate bins for col %s", col)
-
-        categorical_columns = [s for s in df.columns.to_list() if s not in numeric_columns]
-        if categorical_columns:
-            high_cardinality_cols = set()
-            low_cardinality_cols = set()
-
-            print("### Categorical columns")
-            print()
-            for col in categorical_columns:
-                vc = df[col].value_counts()
-                vc = vc[vc > (len(df) * 0.005)]
-                if len(vc) > 0:
-                    low_cardinality_cols.add(col)
-                    print(f"#### common values of {col} column")
-                    vc = pd.DataFrame({"Count": vc, "Percentage": (vc / len(df)) * 100}).sort_values(
-                        by="Count", ascending=False
-                    )
-                    print_df(vc.head(30))
-
-                    if args.groupby:
-                        groups = df.groupby(col).size()
-                        groups = groups[groups >= 15]
-                        if len(groups) > 0:
-                            print(f"#### group by {col}")
-                            print_df(df[df[col].isin(groups.index)].groupby(col).describe())
-
-                unique_count = df[col].nunique()
-                if unique_count >= (len(df) * 0.2):
-                    high_cardinality_cols.add(col)
-
-            med_cardinality_cols = low_cardinality_cols.intersection(high_cardinality_cols)
-            low_cardinality_cols = low_cardinality_cols - med_cardinality_cols
-            high_cardinality_cols = high_cardinality_cols - med_cardinality_cols
-
-            if high_cardinality_cols:
-                print("#### High cardinality (many unique values)")
-                print_series(high_cardinality_cols)
-            if med_cardinality_cols:
-                print("#### Medium cardinality (many unique but also many similar values)")
-                print_series(med_cardinality_cols)
-            if low_cardinality_cols:
-                print("#### Low cardinality (many similar values)")
-                print_series(low_cardinality_cols)
+    if args.columns_include:
+        args.minimize_columns += [s.lstrip("-") for s in args.columns_include if s.startswith("-")]
+        columns_include = [s.lstrip("-") for s in args.columns_include]
+
+        # TODO: convert str categories like easy, hard, good, bad
+        # if columns_include and the col is not numeric
+        #     col.apply(words_to_numbers(args, words))
+        alternatives = df[columns_include]
+    else:
+        alternatives = df.select_dtypes("number")
+    alternatives = alternatives.drop(columns=args.columns_exclude)
 
-    print("### Missing values")
-    print()
-    nan_col_sums = df.isna().sum()
-    print(
-        f"{nan_col_sums.sum():,} nulls/NaNs",
-        f"({(nan_col_sums.sum() / (df.shape[0] * df.shape[1])):.1%} dataset values missing)",
-    )
+    if alternatives.empty:
+        print("No alternatives could be identified. The data likely needs to be cleaned...")
+        print("You can try running with --clean but compare the output with the original data:")
+        print_df(df.head(5))
+        return
+
+    minimize_cols = set(args.minimize_columns)
+    maximize_cols = set(alternatives.columns) - minimize_cols
+
+    print("### Goals")
     print()
+    if maximize_cols:
+        print("#### Maximize")
+        print_series(maximize_cols)
+    if minimize_cols:
+        print("#### Minimize")
+        print_series(minimize_cols)
+
+    # TODO: add --pairwise flag
+    """
+    from pymcdm.methods import COMET
+    from pymcdm.methods.comet_tools import TriadSupportExpert
+
+    cvalues = [
+            [0, 500, 1000],
+            [1, 5]
+            ]
+
+    expert_function = TriadSupportExpert(
+            criteria_names=['Price [$]', 'Profit [grade]'],
+            filename='mej.csv',
+            )
+
+    comet = COMET(cvalues, expert_function)
+    """
 
-    if nan_col_sums.sum():
-        no_nas = df.columns[df.notnull().all()]
-        if len(no_nas) > 0:
-            print(f"#### {len(no_nas)} columns with no missing values")
-            print_series(no_nas)
-
-        all_nas = df.columns[df.isnull().all()]
-        if len(all_nas) > 0:
-            print(f"#### {len(all_nas)} columns with all missing values")
-            print_series(all_nas)
-
-        print("#### Value stats")
-        column_report = pd.DataFrame(df_column_values(df, col) for col in df.columns).set_index("column")
-        column_report = column_report.sort_values(["empty_string_count", "zero_count", "null_count"])
-        print_df(column_report[["values", "null", "zero", "empty_string"]])
+    data = auto_mcda(args, df, alternatives, minimize_cols)
+    print_df(data)
 
 
-def file_eda(args, path):
+def file_mcda(args, path):
     dfs = file_utils.read_file_to_dataframes(
         path,
         table_name=args.table_name,
         table_index=args.table_index,
         start_row=args.start_row,
         end_row=args.end_row,
         order_by=args.sort,
         encoding=args.encoding,
         mimetype=args.mimetype,
     )
-    if getattr(args, "repl", False):
-        breakpoint()
 
     for df in dfs:
         print(f"## {path}:{df.name}")
+        df = pd_utils.convert_dtypes(df, clean=args.clean)
         print_info(args, df)
 
 
-def eda():
+def mcda():
     args = parse_args()
     for path in args.paths:
-        file_eda(args, path)
+        file_mcda(args, path)
 
 
 if __name__ == "__main__":
-    eda()
+    mcda()
```

### Comparing `xklb-2.5.9/xklb/scripts/export_text.py` & `xklb-2.6.1/xklb/scripts/export_text.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import argparse
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import db_utils, objects
+from xklb.utils import arggroups, db_utils, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library export-text", usage=usage.export_text)
     parser.add_argument("--format", default="html")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     args = parser.parse_args()
 
     Path(args.database).touch()
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
```

### Comparing `xklb-2.5.9/xklb/scripts/history.py` & `xklb-2.6.1/xklb/scripts/history.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,47 @@
 import argparse
 
 from xklb import usage
 from xklb.history import create
 from xklb.media import media_printer
-from xklb.utils import consts, db_utils, objects, sql_utils, strings
+from xklb.utils import arggroups, consts, db_utils, objects, sql_utils, strings
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         "library history",
         usage=usage.history,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument(
-        "--frequency",
-        "--freqency",
-        "-f",
-        metavar="frequency",
-        default="monthly",
-        const="monthly",
-        type=str.lower,
-        nargs="?",
-        help=f"One of: {', '.join(consts.frequency)} (default: %(default)s)",
-    )
 
-    parser.add_argument("--print", "-p", default="p", const="p", nargs="?", help=argparse.SUPPRESS)
-    parser.add_argument("--cols", "-cols", "-col", nargs="*", help="Include a column when printing")
-    parser.add_argument("--sort", "-u", nargs="+", help=argparse.SUPPRESS)
-    parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--duration", "-d", action="append", help=argparse.SUPPRESS)
-    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue")
-    parser.add_argument("--hide-deleted", action="store_true")
-    parser.add_argument("--played", "--opened", action="store_true")
-    parser.add_argument("-v", "--verbose", action="count", default=0)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
+    arggroups.sql_fs(parser)
+    arggroups.sql_media(parser)
 
+    arggroups.frequency(parser)
     parser.add_argument(
         "facet",
         metavar="facet",
         type=str.lower,
         default="watched",
         const="watched",
         nargs="?",
         help=f"One of: {', '.join(consts.time_facets)} (default: %(default)s)",
     )
-    parser.add_argument("database")
+    parser.add_argument("--hide-deleted", action="store_true")
+    parser.add_argument("--played", "--opened", action="store_true")
+
+    arggroups.debug(parser)
+
+    arggroups.database(parser)
     args = parser.parse_intermixed_args()
 
     args.facet = strings.partial_startswith(args.facet, consts.time_facets)
     args.frequency = strings.partial_startswith(args.frequency, consts.frequency)
 
-    if args.db:
-        args.database = args.db
     args.db = db_utils.connect(args)
 
     args.action = consts.SC.history
     log.info(objects.dict_filter_bool(args.__dict__))
 
     args.filter_bindings = {}
```

### Comparing `xklb-2.5.9/xklb/scripts/incremental_diff.py` & `xklb-2.6.1/xklb/scripts/incremental_diff.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import argparse
 
 from xklb import usage
-from xklb.utils import arg_utils, consts, file_utils
+from xklb.utils import arggroups, consts, file_utils
+from xklb.utils.argparse_utils import ArgparseList
 from xklb.utils.log_utils import log
 from xklb.utils.printing import print_df
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Diff two table-like files", usage=usage.incremental_diff)
+    parser.add_argument("--print", "-p", default="p", const="p", nargs="?", help=argparse.SUPPRESS)
     parser.add_argument("--mimetype1", "--filetype1")
     parser.add_argument("--encoding1")
     parser.add_argument("--mimetype2", "--filetype2")
     parser.add_argument("--encoding2")
     parser.add_argument("--table1-name", "--table1", "-t1")
     parser.add_argument("--table2-name", "--table2", "-t2")
     parser.add_argument("--table1-index", type=int)
     parser.add_argument("--table2-index", type=int)
     parser.add_argument("--start-row", "--skiprows", type=int, default=None)
     parser.add_argument("--batch-size", "--batch-rows", default=str(consts.DEFAULT_FILE_ROWS_READ_LIMIT))
-    parser.add_argument("--join-keys", action=arg_utils.ArgparseList, help="Comma separated join keys")
+    parser.add_argument("--join-keys", action=ArgparseList, help="Comma separated join keys")
     parser.add_argument("--sort", "-u")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
     parser.add_argument("path1", help="path to dataset 1")
     parser.add_argument("path2", help="path to dataset 2")
     args = parser.parse_intermixed_args()
 
     # TODO: add an option to load from df2 where ids (select ids from df1)
 
@@ -59,16 +61,16 @@
             order_by=args.sort,
             encoding=args.encoding2,
             mimetype=args.mimetype2,
         )
 
         # TODO: https://github.com/ICRAR/ijson
 
-        tables1 = set(df.name for df in dfs1)
-        tables2 = set(df.name for df in dfs2)
+        tables1 = {df.name for df in dfs1}
+        tables2 = {df.name for df in dfs2}
         common_tables = tables1.intersection(tables2)
         dfs1 = sorted(dfs1, key=lambda df: (df.name in common_tables, df.name), reverse=True)
         dfs2 = sorted(dfs2, key=lambda df: (df.name in common_tables, df.name), reverse=True)
 
         empty_dfs = set()
         for df_idx in range(len(dfs1)):
             df1 = dfs1[df_idx]
```

### Comparing `xklb-2.5.9/xklb/scripts/links_db.py` & `xklb-2.6.1/xklb/scripts/links_db.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import argparse, json, random, time
 from pathlib import Path
 from urllib.parse import parse_qs, urlencode, urlparse, urlunparse
 
 from xklb import db_media, db_playlists, usage
 from xklb.scripts.mining import extract_links
-from xklb.utils import arg_utils, consts, db_utils, objects, printing, strings, web
+from xklb.utils import arg_utils, arggroups, consts, db_utils, objects, printing, strings, web
 from xklb.utils.log_utils import log
 
 
 def parse_args(**kwargs):
     parser = argparse.ArgumentParser(**kwargs)
     parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
-    parser.add_argument("--no-extract", "--skip-extract", action="store_true")
 
     parser.add_argument("--max-pages", type=int)
     parser.add_argument("--fixed-pages", type=int)
     parser.add_argument("--backfill-pages", "--backfill", type=int)
 
     parser.add_argument("--stop-pages-no-match", "--stop-no-match", type=int, default=4)
     parser.add_argument("--stop-pages-no-new", "--stop-no-new", type=int, default=10)
@@ -24,105 +23,26 @@
     parser.add_argument("--stop-link")
 
     parser.add_argument("--page-replace")
     parser.add_argument("--page-key", default="page")
     parser.add_argument("--page-step", "--step", "-S", type=int, default=1)
     parser.add_argument("--page-start", "--start-page", "--start", type=int)
 
-    parser.add_argument(
-        "--path-include",
-        "--include-path",
-        "--include",
-        "-s",
-        nargs="*",
-        default=[],
-        help="path substrings for inclusion (all must match to include)",
-    )
-    parser.add_argument(
-        "--text-include",
-        "--include-text",
-        nargs="*",
-        default=[],
-        help="link text substrings for inclusion (all must match to include)",
-    )
-    parser.add_argument(
-        "--after-include",
-        "--include-after",
-        nargs="*",
-        default=[],
-        help="plain text substrings after URL for inclusion (all must match to include)",
-    )
-    parser.add_argument(
-        "--before-include",
-        "--include-before",
-        nargs="*",
-        default=[],
-        help="plain text substrings before URL for inclusion (all must match to include)",
-    )
-    parser.add_argument(
-        "--path-exclude",
-        "--exclude-path",
-        "--exclude",
-        "-E",
-        nargs="*",
-        default=["javascript:", "mailto:", "tel:"],
-        help="path substrings for exclusion (any must match to exclude)",
-    )
-    parser.add_argument(
-        "--text-exclude",
-        "--exclude-text",
-        nargs="*",
-        default=[],
-        help="link text substrings for exclusion (any must match to exclude)",
-    )
-    parser.add_argument(
-        "--after-exclude",
-        "--exclude-after",
-        nargs="*",
-        default=[],
-        help="plain text substrings after URL for exclusion (any must match to exclude)",
-    )
-    parser.add_argument(
-        "--before-exclude",
-        "--exclude-before",
-        nargs="*",
-        default=[],
-        help="plain text substrings before URL for exclusion (any must match to exclude)",
-    )
-
-    parser.add_argument("--strict-include", action="store_true", help="All include args must resolve true")
-    parser.add_argument("--strict-exclude", action="store_true", help="All exclude args must resolve true")
-    parser.add_argument("--case-sensitive", action="store_true", help="Filter with case sensitivity")
-    parser.add_argument(
-        "--no-url-decode",
-        "--skip-url-decode",
-        action="store_true",
-        help="Skip URL-decode for --path-include/--path-exclude",
-    )
-
-    parser.add_argument("--cookies", help="path to a Netscape formatted cookies file")
-    parser.add_argument("--cookies-from-browser", metavar="BROWSER[+KEYRING][:PROFILE][::CONTAINER]")
-
-    parser.add_argument("--selenium", action="store_true")
-    parser.add_argument("--manual", action="store_true", help="Confirm manually in shell before exiting the browser")
-    parser.add_argument("--scroll", action="store_true", help="Scroll down the page; infinite scroll")
-    parser.add_argument("--auto-pager", "--autopager", action="store_true")
-    parser.add_argument("--poke", action="store_true")
-    parser.add_argument("--chrome", action="store_true")
-    parser.add_argument("--force", action="store_true")
+    arggroups.filter_links(parser)
+
+    arggroups.requests(parser)
+    arggroups.selenium(parser)
 
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    parser.add_argument("--force", action="store_true")
 
-    parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
-    parser.add_argument("--file", "-f", help="File with one URL per line")
+    arggroups.debug(parser)
 
-    parser.add_argument("database", help=argparse.SUPPRESS)
+    arggroups.database(parser)
     if "add" in kwargs["prog"]:
-        parser.add_argument("paths", nargs="*", action=arg_utils.ArgparseArgsOrStdin, help=argparse.SUPPRESS)
+        arggroups.paths_or_stdin(parser)
     args = parser.parse_intermixed_args()
 
     if args.auto_pager:
         args.fixed_pages = 1
 
     if args.scroll:
         args.selenium = True
@@ -137,16 +57,14 @@
         args.text_exclude = [s.lower() for s in args.text_exclude]
         args.after_exclude = [s.lower() for s in args.after_exclude]
 
     if not args.no_url_decode:
         args.path_include = [web.url_decode(s) for s in args.path_include]
         args.path_exclude = [web.url_decode(s) for s in args.path_exclude]
 
-    if args.db:
-        args.database = args.db
     Path(args.database).touch()
     args.db = db_utils.connect(args)
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args, parser
```

### Comparing `xklb-2.5.9/xklb/scripts/merge_dbs.py` & `xklb-2.6.1/xklb/scripts/merge_dbs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 import argparse
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arg_utils, db_utils, objects
+from xklb.utils import arggroups, argparse_utils, db_utils, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library merge-dbs", usage=usage.merge_dbs)
 
-    parser.add_argument("--only-tables", "-t", action=arg_utils.ArgparseList, help="Comma separated specific table(s)")
-
-    parser.add_argument("--primary-keys", "--pk", action=arg_utils.ArgparseList, help="Comma separated primary keys")
-    parser.add_argument("--business-keys", "--bk", action=arg_utils.ArgparseList, help="Comma separated business keys")
+    parser.add_argument(
+        "--only-tables", "-t", action=argparse_utils.ArgparseList, help="Comma separated specific table(s)"
+    )
+
+    parser.add_argument(
+        "--primary-keys", "--pk", action=argparse_utils.ArgparseList, help="Comma separated primary keys"
+    )
+    parser.add_argument(
+        "--business-keys", "--bk", action=argparse_utils.ArgparseList, help="Comma separated business keys"
+    )
 
     parser.add_argument("--upsert", action="store_true")
     parser.add_argument("--ignore", "--only-new-rows", action="store_true")
 
     parser.add_argument("--only-target-columns", action="store_true")
-    parser.add_argument("--skip-columns", action=arg_utils.ArgparseList)
+    parser.add_argument("--skip-columns", action=argparse_utils.ArgparseList)
 
     parser.add_argument("--where", "-w", nargs="+", action="extend", help=argparse.SUPPRESS)
 
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     parser.add_argument("source_dbs", nargs="+")
     args = parser.parse_intermixed_args()
 
     if args.where:
         args.where = " and ".join(args.where)
 
-    if args.db:
-        args.database = args.db
     Path(args.database).touch()
     args.db = db_utils.connect(args)
 
     log.info(objects.dict_filter_bool(args.__dict__))
 
     return args
```

### Comparing `xklb-2.5.9/xklb/scripts/merge_folders.py` & `xklb-2.6.1/xklb/scripts/merge_folders.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import argparse, json, os
 from pathlib import Path
-from typing import List
 
 from xklb import usage
-from xklb.utils import arg_utils, devices, objects, printing
+from xklb.utils import arg_utils, arggroups, devices, file_utils, objects, printing
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library merge-folders", usage=usage.merge_folders)
-    parser.add_argument("--replace", "--delete", action="store_true")
-    parser.add_argument("--skip", "--no-replace", "--no-clobber", action="store_true")
-    parser.add_argument("--simulate", "--dry-run", action="store_true")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.capability_clobber(parser)
+    arggroups.capability_simulate(parser)
+    arggroups.debug(parser)
 
     parser.add_argument("sources", nargs="+")
     parser.add_argument("destination")
     args = parser.parse_intermixed_args()
 
     args.destination = arg_utils.split_folder_glob(args.destination)
 
@@ -66,72 +64,54 @@
             log.info("%s conflicts with %s", source_file, renamed_file)
         else:
             log.debug("%s can be renamed cleanly to %s", source_file, renamed_file)
         source_rename_data.append((is_conflict, source_file, renamed_file))
     return source_rename_data
 
 
-def same_filesystem(path1, path2):
-    stat1 = os.stat(path1)
-    stat2 = os.stat(path2)
-    return stat1.st_dev == stat2.st_dev
-
-
-def filter_valid_sources(args, destination_folder):
-    valid_sources = []
-    for source in args.sources:
-        if same_filesystem(source, destination_folder):
-            valid_sources.append(source)
-        else:
-            print(f"Skipping {source}. Source not on same filesystem as destination.")
-
-    if not valid_sources:
-        print("No valid sources found. Sources and destination must be on the same filesystem.")
-        raise SystemExit(1)
-
-    return valid_sources
-
-
 def get_clobber(args):
     choice = None
     if args.replace:
         choice = "replace"
-    elif args.skip:
-        choice = "skip"
+    elif args.no_replace:
+        choice = "no-replace"
     else:
-        choice = devices.prompt(choices=["replace", "skip", "simulate-replace", "quit"])
+        choice = devices.prompt(choices=["replace", "no-replace", "simulate-replace", "quit"])
 
     if choice == "quit":
         raise SystemExit(130)
     if choice == "simulate-replace":
         args.simulate = True
         choice = "replace"
 
-    assert choice in ["replace", "skip"]
+    assert choice in ["replace", "no-replace"]
     return choice == "replace"
 
 
 def apply_merge(args, empty_folder_data, rename_data, clobber):
     def print_mv(t):
         if t[0]:  ## file exists in destination already
             if not clobber:
                 log.info("[%s]: Skipping due to existing file %s", t[1], t[2])
             else:
                 printing.pipe_print("mv", t[1], t[2])
         else:
             printing.pipe_print("mv", t[1], t[2])
 
     def mv(t):
+        mv_fn = os.renames
         if t[0]:  ## file exists in destination already
+            mv_fn = os.replace
             if not clobber:
                 log.info("[%s]: Skipping due to existing file %s", t[1], t[2])
-            else:
-                os.replace(t[1], t[2])
-        else:  ## file does not exist in destination already
-            os.renames(t[1], t[2])
+                return
+        try:
+            mv_fn(t[1], t[2])
+        except Exception:
+            file_utils.rename_move_file(t[1], t[2])
 
     if args.simulate:
         for p in empty_folder_data:
             print("mkdir", p)
 
         for t in rename_data:
             print_mv(t)
@@ -158,24 +138,23 @@
 
 def merge_folders() -> None:
     args = parse_args()
 
     print("Destination:")
     destination_folder, destination_glob = args.destination
     destination_folder.mkdir(parents=True, exist_ok=True)
-    args.sources = filter_valid_sources(args, destination_folder)  # TODO: add cross-fs support
     destination_files, destination_folders_dict = existing_stats(destination_folder, destination_glob)
 
     destination_folders = (
         destination_folders_dict["file"] | destination_folders_dict["folder"] | destination_folders_dict["empty"]
     )
 
     all_source_folders = set()
     empty_folder_data: set[Path] = set()
-    rename_data: List[tuple[bool, Path, Path]] = []
+    rename_data: list[tuple[bool, Path, Path]] = []
     clobber = False
     print("Sources:")
     for source in args.sources:
         source_folder, source_glob = arg_utils.split_folder_glob(source)
         source_files, source_folders_dict = existing_stats(source_folder, source_glob)
         source_folders = source_folders_dict["file"] | source_folders_dict["folder"] | source_folders_dict["empty"]
```

### Comparing `xklb-2.5.9/xklb/scripts/merge_online_local.py` & `xklb-2.6.1/xklb/scripts/merge_online_local.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import argparse, os
 from copy import deepcopy
-from typing import List
 
 from xklb import db_media, usage
 from xklb.media import media_printer
-from xklb.utils import consts, db_utils, devices, objects
+from xklb.utils import arggroups, consts, db_utils, devices, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library merge-online-local", usage=usage.merge_online_local)
     parser.add_argument("--no-confirm", "--yes", "-y", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default=100)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="100")
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     args = parser.parse_args()
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def get_duplicates(args) -> List[dict]:
+def get_duplicates(args) -> list[dict]:
     query = f"""
     WITH m1 as (
         SELECT
             *
         FROM
             media
         WHERE 1=1
```

### Comparing `xklb-2.5.9/xklb/scripts/move_list.py` & `xklb-2.6.1/xklb/scripts/move_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import argparse, shutil, tempfile
 from copy import deepcopy
 from pathlib import Path
-from typing import Dict, List, Tuple
 
 import humanize
 from tabulate import tabulate
 
 from xklb import usage
-from xklb.utils import consts, db_utils, devices, iterables, objects, printing
+from xklb.utils import arggroups, consts, db_utils, devices, iterables, objects, printing
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library mv-list",
         usage=usage.mv_list,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="25")
-    parser.add_argument("--lower", default=4, type=int, help="Number of files per folder lower limit")
-    parser.add_argument("--upper", default=4000, type=int, help="Number of files per folder upper limit")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.sql_fs(parser)
+    arggroups.operation_group_folders(parser)
+    parser.set_defaults(limit="25", lower=4, upper=4000)
+    arggroups.debug(parser)
 
     parser.add_argument("mount_point")
-    parser.add_argument("database")
+    arggroups.database(parser)
     args = parser.parse_intermixed_args()
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def group_by_folder(args, media) -> List[Dict]:
+def group_by_folder(args, media) -> list[dict]:
     d = {}
     for m in media:
         if m["path"].startswith("http"):
             continue
 
         p = m["path"].split("/")
         while len(p) >= 3:
@@ -53,15 +52,15 @@
     for path, pdict in list(d.items()):
         if any([pdict["count"] < args.lower, pdict["count"] > args.upper]):
             d.pop(path)
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
-def get_table(args) -> List[dict]:
+def get_table(args) -> list[dict]:
     media = list(
         args.db.query(
             """
         select
             path
             , size
         from media
@@ -73,15 +72,15 @@
         ),
     )
 
     folders = group_by_folder(args, media)
     return sorted(folders, key=lambda x: x["size"] / x["count"])
 
 
-def iterate_and_show_options(args, tbl) -> Tuple[List[Dict], List[Dict]]:
+def iterate_and_show_options(args, tbl) -> tuple[list[dict], list[dict]]:
     vew = tbl[-int(args.limit) :] if args.limit else tbl
 
     vew = iterables.list_dict_filter_bool(vew, keep_0=False)
     vew = printing.col_resize_percent(vew, "path", 60)
     vew = printing.col_naturalsize(vew, "size")
     print(tabulate(vew, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
     print(len(tbl) - len(vew), "other folders not shown")
```

### Comparing `xklb-2.5.9/xklb/scripts/places_import.py` & `xklb-2.6.1/xklb/scripts/places_import.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import argparse
 from pathlib import Path
 
 from xklb import db_media, usage
-from xklb.utils import consts, db_utils, nums, objects
+from xklb.utils import arggroups, consts, db_utils, nums, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library places-import", usage=usage.places_import)
-    parser.add_argument("database")
+    arggroups.database(parser)
     parser.add_argument("paths", nargs="+")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
     args = parser.parse_intermixed_args()
 
     Path(args.database).touch()
     args.db = db_utils.connect(args)
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
```

### Comparing `xklb-2.5.9/xklb/scripts/playback_control.py` & `xklb-2.6.1/xklb/scripts/playback_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse, platform, textwrap
 from copy import deepcopy
 from pathlib import Path
 
-from xklb.utils import consts, file_utils, iterables, mpv_utils, nums, objects, printing, processes
+from xklb.utils import arggroups, consts, file_utils, iterables, mpv_utils, nums, objects, printing, processes
 from xklb.utils.log_utils import log
 
 
 def parse_args(action) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog=f"library {action}",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -16,20 +16,19 @@
 
     if action == "next":
         parser.add_argument(
             "--delete",
             "--remove",
             "--erase",
             "--rm",
-            "-rm",
             action="store_true",
-            help="Delete currently playing media",
+            help="Delete currently playing media from the filesystem",
         )
 
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
     args = parser.parse_args()
 
     args.mpv = mpv_utils.connect_mpv(args.mpv_socket)
 
     log.info(objects.dict_filter_bool(args.__dict__))
 
     return args
@@ -48,15 +47,15 @@
     try:
         probe = processes.FFProbe(path)
     except Exception:
         log.exception(f"Failed reading header. {path}")
         return path
 
     codec_types = [s.get("codec_type") for s in probe.streams]
-    audio_count = sum(1 for s in codec_types if s == "audio")
+    audio_count = sum((1 for s in codec_types if s == "audio"))
 
     excluded_keys = [
         "encoder",
         "major_brand",
         "minor_version",
         "compatible_brands",
         "software",
```

### Comparing `xklb-2.5.9/xklb/scripts/playlists.py` & `xklb-2.6.1/xklb/scripts/playlists.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,49 @@
 import argparse, os, sqlite3
-from typing import Tuple
 
 from xklb import usage
 from xklb.media import media_printer
-from xklb.utils import consts, db_utils, objects
+from xklb.utils import arggroups, consts, db_utils, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         "library playlists",
         usage.playlists,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument("--sort", "-u", nargs="+", help=argparse.SUPPRESS)
-    parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--flexible-search", "--or", "--flex", action="store_true")
-    parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--duration", "-d", action="append", help=argparse.SUPPRESS)
-    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", help=argparse.SUPPRESS)
-    parser.add_argument("--online-media-only", "--online", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--local-media-only", "--local", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
-    parser.add_argument("--print", "-p", default="p", const="p", nargs="?", help=argparse.SUPPRESS)
-    parser.add_argument("--cols", "-cols", "-col", nargs="*", help="Include a column when printing")
+
+    arggroups.sql_fs(parser)
+    arggroups.sql_media(parser)
+
     parser.add_argument(
         "--delete",
         "--remove",
-        "--erase",
         "--rm",
-        "-rm",
         action="store_true",
         help="Delete matching playlists and playlist media",
     )
 
-    parser.add_argument("-v", "--verbose", action="count", default=0)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
 
-    if args.search:
-        args.include += args.search
+    args.include += args.search
 
-    if args.db:
-        args.database = args.db
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
 
     args.action = consts.SC.playlists
     return args
 
 
-def construct_query(args) -> Tuple[str, dict]:
+def construct_query(args) -> tuple[str, dict]:
     pl_columns = db_utils.columns(args, "playlists")
     args.filter_sql = []
     args.filter_bindings = {}
 
     args.filter_sql.extend([" and " + w for w in args.where])
 
     args.table = "playlists"
```

### Comparing `xklb-2.5.9/xklb/scripts/process_audio.py` & `xklb-2.6.1/xklb/scripts/process_ffmpeg.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,162 +1,204 @@
 import argparse, json, shlex, subprocess
 from pathlib import Path
-from typing import List
 
 from xklb import usage
-from xklb.utils import nums, objects
+from xklb.utils import arggroups, nums, objects, path_utils, processes, web
+from xklb.utils.arg_utils import kwargs_overwrite
 from xklb.utils.log_utils import log
 
-DEFAULT_MIN_SPLIT = "20s"
-
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library process-audio", usage=usage.process_audio)
-    parser.add_argument("--always-split", action="store_true")
-    parser.add_argument("--split-longer-than")
-    parser.add_argument("--min-split-segment", default=DEFAULT_MIN_SPLIT)
-    parser.add_argument("--delete-video", action="store_true")
-    parser.add_argument("--dry-run", action="store_true")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    parser = argparse.ArgumentParser(prog="library process-ffmpeg", usage=usage.process_ffmpeg)
+    arggroups.capability_simulate(parser)
+    arggroups.process_ffmpeg(parser)
+    parser.add_argument("--delete-unplayable", action="store_true")
+    arggroups.debug(parser)
 
     parser.add_argument("paths", nargs="+")
     args = parser.parse_args()
 
     args.split_longer_than = nums.human_to_seconds(args.split_longer_than)
     args.min_split_segment = nums.human_to_seconds(args.min_split_segment)
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def process_path(
-    path,
-    always_split=False,
-    split_longer_than=None,
-    min_split_segment=nums.human_to_seconds(DEFAULT_MIN_SPLIT),
-    dry_run=False,
-    delete_video=False,
-):
+def process_path(args, path, **kwargs):
+    args = kwargs_overwrite(args, kwargs)
+
+    output_path = Path(web.url_to_local_path(path) if path.startswith("http") else path)
+    output_path = Path(path_utils.clean_path(bytes(output_path), max_name_len=251))
+
     path = Path(path)
+
     ffprobe_cmd = ["ffprobe", "-v", "error", "-print_format", "json", "-show_format", "-show_streams", path]
-    result = subprocess.run(ffprobe_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    result = subprocess.run(ffprobe_cmd, capture_output=True)
     info = json.loads(result.stdout)
 
     if "streams" not in info:
-        print("No stream found:", path)
+        log.error("No media streams found: %s", path)
         return path
-    audio_stream = next((stream for stream in info["streams"] if stream["codec_type"] == "audio"), None)
     video_stream = next((stream for stream in info["streams"] if stream["codec_type"] == "video"), None)
+    audio_stream = next((stream for stream in info["streams"] if stream["codec_type"] == "audio"), None)
+    if not video_stream:
+        log.warning("No video stream found: %s", path)
+        if args.delete_no_video:
+            path.unlink()
+            return None
     if not audio_stream:
-        print("No audio stream found:", path)
+        log.warning("No audio stream found: %s", path)
+        if args.delete_no_audio:
+            path.unlink()
+            return None
+
+    if video_stream and not args.audio_only:
+        output_suffix = ".av1.mkv"
+    elif not video_stream and not audio_stream:
+        output_suffix = ".mkv"
+    else:
+        output_suffix = ".mka"
+    output_path = output_path.with_suffix(output_suffix)
+
+    if path == output_path:
+        log.error("Input and output files have the same names %s", path)
         return path
 
-    channels = audio_stream.get("channels") or 2
-    bitrate = int(audio_stream.get("bit_rate") or info["format"].get("bit_rate") or 256000)
-    source_rate = int(audio_stream.get("sample_rate") or 44100)
-    duration = float(audio_stream.get("duration") or info["format"].get("duration") or 0)
-
-    assert bitrate > 0
-    assert channels > 0
-    assert source_rate > 0
-
-    ff_opts: List[str] = []
-    if channels == 1:
-        ff_opts.extend(["-ac 1"])
-    else:
-        ff_opts.extend(["-ac 2"])
+    ff_opts: list[str] = []
 
-    if bitrate >= 256000:
-        ff_opts.extend(["-b:a 128k"])
-    else:
-        ff_opts.extend(["-b:a 64k", "-frame_duration 40"])
+    if video_stream:
+        ff_opts.extend(["-c:v libsvtav1", "-preset 8 -crf 44"])
 
-    if source_rate >= 44100:
-        opus_rate = 48000
-    elif source_rate >= 22050:
-        opus_rate = 24000
-    else:
-        opus_rate = 16000
-    ff_opts.extend([f"-ar {opus_rate}"])
+        width = int(video_stream.get("width"))
+        height = int(video_stream.get("height"))
+
+        if width > (args.max_width * (1 + args.max_width_buffer)):
+            ff_opts.extend([f"-vf 'scale=-2:min(iw\\,{args.max_width})'"])
+        elif height > (args.max_height * (1 + args.max_height_buffer)):
+            ff_opts.extend([f"-vf 'scale=-2:min(ih\\,{args.max_height})'"])
+
+    is_split = bool(audio_stream)
+    if audio_stream:
+        channels = audio_stream.get("channels") or 2
+        bitrate = int(audio_stream.get("bit_rate") or info["format"].get("bit_rate") or 256000)
+        source_rate = int(audio_stream.get("sample_rate") or 44100)
+
+        duration = float(audio_stream.get("duration") or info["format"].get("duration") or 0)
+        is_split = args.always_split or (args.split_longer_than and duration > args.split_longer_than)
+
+        try:
+            assert bitrate > 0
+            assert channels > 0
+            assert source_rate > 0
+        except AssertionError:
+            log.exception("Broken file or audio format misdetected: %s", path)
+            if args.delete_no_audio:
+                path.unlink()
+                return None
+        else:
+            if channels == 1:
+                ff_opts.extend(["-ac 1"])
+            else:
+                ff_opts.extend(["-ac 2"])
+
+            if bitrate >= 256000:
+                ff_opts.extend(["-b:a 128k"])
+            else:
+                ff_opts.extend(["-b:a 64k", "-frame_duration 40"])
+
+            if source_rate >= 44100:
+                opus_rate = 48000
+            elif source_rate >= 22050:
+                opus_rate = 24000
+            else:
+                opus_rate = 16000
+            ff_opts.extend(["-c:a libopus", f"-ar {opus_rate}", "-filter:a loudnorm=i=-18:tp=-3:lra=17"])
 
-    output_path = path.with_suffix(".mka")
-    is_split = always_split or (split_longer_than and duration > split_longer_than)
-    if is_split:
-        splits = (
-            subprocess.check_output(
-                [
-                    "ffmpeg",
-                    "-v",
-                    "warning",
-                    "-i",
-                    path,
-                    "-af",
-                    "silencedetect=-55dB:d=0.3,ametadata=mode=print:file=-:key=lavfi.silence_start",
-                    "-vn",
-                    "-sn",
-                    "-f",
-                    "s16le",
-                    "-y",
-                    "/dev/null",
-                ]
-            )
-            .decode()
-            .split("\n")
-        )
-
-        splits = [line.split("=")[1] for line in splits if "lavfi.silence_start" in line]
-
-        prev = 0.0
-        final_splits = []
-        for split in splits:
-            split = float(split)
-            if (split - prev) >= min_split_segment:  # type: ignore
-                final_splits.append(str(split))
-                prev = split
-
-        if final_splits:
-            output_path = path.with_suffix(".%03d.mka")
-            final_splits = ",".join(final_splits)
-            print(f"Splitting {path} at points: {final_splits}")
-            ff_opts.extend(["-f segment", f"-segment_times {final_splits}"])
+        if is_split:
+            try:
+                result = subprocess.check_output(
+                    [
+                        "ffmpeg",
+                        "-v",
+                        "warning",
+                        "-i",
+                        path,
+                        "-af",
+                        "silencedetect=-55dB:d=0.3,ametadata=mode=print:file=-:key=lavfi.silence_start",
+                        "-vn",
+                        "-sn",
+                        "-f",
+                        "s16le",
+                        "-y",
+                        "/dev/null",
+                    ]
+                )
+            except subprocess.CalledProcessError:
+                log.exception("Splits could not be identified. Likely broken file: %s", path)
+                if args.delete_broken:
+                    path.unlink()
+                    return None
+                raise
+
+            splits = result.decode().split("\n")
+            splits = [line.split("=")[1] for line in splits if "lavfi.silence_start" in line]
+
+            prev = 0.0
+            final_splits = []
+            for split in splits:
+                split = float(split)
+                if (split - prev) >= args.min_split_segment:  # type: ignore
+                    final_splits.append(str(split))
+                    prev = split
+
+            if final_splits:
+                output_path = path.with_suffix(".%03d" + output_suffix)
+                final_splits = ",".join(final_splits)
+                print(f"Splitting {path} at points: {final_splits}")
+                ff_opts.extend(["-f segment", f"-segment_times {final_splits}"])
+            else:
+                is_split = False
 
-    cmd = f'ffmpeg -nostdin -hide_banner -loglevel warning -y -i {shlex.quote(str(path))} -vn -c:a libopus {" ".join(ff_opts)} -filter:a loudnorm=i=-18:tp=-3:lra=17 {shlex.quote(str(output_path))}'
-    if dry_run:
+    cmd = f'ffmpeg -nostdin -hide_banner -loglevel warning -y -i {shlex.quote(str(path))} {" ".join(ff_opts)} {shlex.quote(str(output_path))}'
+    if args.simulate:
         print(cmd)
     else:
-        subprocess.check_call(cmd, shell=True)
-        if video_stream:
-            if delete_video:
-                path.unlink()  # Remove original
+        try:
+            processes.cmd(cmd, shell=True)
+        except subprocess.CalledProcessError:
+            log.exception("Could not transcode: %s", path)
+            if args.delete_broken:
+                path.unlink()
+                return None
+            else:
+                raise
+
+        if video_stream and (not args.audio_only or (args.audio_only and args.no_preserve_video)):
+            path.unlink()  # Remove original
         elif is_split:
             path.unlink()  # Remove original
+            return path.with_suffix(".000" + output_suffix)  # TODO: return multiple paths...
+        elif output_path.stat().st_size > path.stat().st_size:
+            output_path.unlink()  # Remove transcode
+            return path
         else:
-            if output_path.stat().st_size > path.stat().st_size:
-                output_path.unlink()  # Remove transcode
-                return path
-            else:
-                path.unlink()  # Remove original
+            path.unlink()  # Remove original
     return output_path
 
 
-def process_audio():
+def process_ffmpeg():
     args = parse_args()
 
     for path in args.paths:
-        path = str(Path(path).resolve())
+        if not path.startswith("http"):
+            path = str(Path(path).resolve())
 
         try:
-            process_path(
-                path,
-                always_split=args.always_split,
-                split_longer_than=args.split_longer_than,
-                min_split_segment=args.min_split_segment,
-                delete_video=args.delete_video,
-                dry_run=args.dry_run,
-            )
+            process_path(args, path)
         except Exception:
             print(path)
             raise
 
 
 if __name__ == "__main__":
-    process_audio()
+    process_ffmpeg()
```

### Comparing `xklb-2.5.9/xklb/scripts/redownload.py` & `xklb-2.6.1/xklb/scripts/redownload.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 import argparse, json, tempfile
 from copy import deepcopy
 from pathlib import Path
-from typing import List
 
 from xklb import usage
 from xklb.media import media_printer
-from xklb.utils import consts, db_utils, devices, file_utils, iterables, objects
+from xklb.utils import arggroups, consts, db_utils, devices, file_utils, iterables, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library redownload",
         usage=usage.redownload,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
-    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default=100)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    parser.add_argument("--download-archive", default=str(Path("~/.local/share/yt_archive.txt").expanduser().resolve()))
+    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="100")
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     parser.add_argument("deleted_at", nargs="?")
     parser.add_argument("deleted_to", nargs="?")
     args = parser.parse_args()
 
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def list_deletions(args) -> List[dict]:
+def list_deletions(args) -> list[dict]:
     query = """
         SELECT
             strftime('%Y-%m-%dT%H:%M:%S', time_deleted, 'unixepoch', 'localtime') as time_deleted
             , COUNT(*) as count
         FROM media
         WHERE time_deleted > 0
           AND time_downloaded > 0
@@ -43,15 +42,15 @@
         LIMIT ?
     """
     media = list(args.db.query(query, [args.limit]))
     media = list(reversed(media))
     return media
 
 
-def get_non_tube_media(args, paths) -> List[dict]:
+def get_non_tube_media(args, paths) -> list[dict]:
     media = []
     paths = iterables.conform(paths)
     if paths:
         for p in iterables.chunks(paths, consts.SQLITE_PARAM_LIMIT):
             with args.db.conn:
                 media.extend(
                     list(
@@ -60,15 +59,15 @@
                             (*p,),
                         ),
                     ),
                 )
     return media
 
 
-def get_deleted_media(args) -> List[dict]:
+def get_deleted_media(args) -> list[dict]:
     if all([args.deleted_at, args.deleted_to]):
         # use timestamps between inclusive, converting from localtime to UTC
         query = """
             SELECT *
             FROM media
             WHERE time_deleted >= strftime('%s', ?, 'utc') AND time_deleted <= strftime('%s', ?, 'utc')
             AND time_downloaded > 0
```

### Comparing `xklb-2.5.9/xklb/scripts/rel_mv.py` & `xklb-2.6.1/xklb/scripts/rel_mv.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import argparse, shlex
 from os.path import commonprefix
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arg_utils, file_utils, objects, path_utils, processes
+from xklb.utils import arggroups, argparse_utils, file_utils, objects, path_utils, processes
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library relmv", usage=usage.relmv)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
-    parser.add_argument("--dry-run", action="store_true")
-    parser.add_argument("--ext", "-e", action=arg_utils.ArgparseList)
+    arggroups.capability_simulate(parser)
+    parser.add_argument("--ext", "-e", default=[], action=argparse_utils.ArgparseList)
+    arggroups.debug(parser)
 
     parser.add_argument("sources", nargs="+", help="one or more source files or directories to move")
     parser.add_argument("dest", help="destination directory")
     args = parser.parse_args()
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def rel_move(sources, dest, dry_run=False, relative_from=None):
+def rel_move(sources, dest, simulate=False, relative_from=None):
     if relative_from:
         relative_from = Path(relative_from).expanduser().resolve()
 
     new_paths = []
     for source in sources:
         abspath = Path(source).expanduser().resolve()
 
@@ -40,44 +40,44 @@
                     relpath = str(abspath.relative_to(Path(rel_prefix).parent))
                 except ValueError:
                     relpath = str(source)
 
         target_dir = (dest / relpath).parent
         target_dir = path_utils.dedupe_path_parts(target_dir)
 
-        if dry_run:
+        if simulate:
             log.warning("mv %s %s", shlex.quote(str(abspath)), shlex.quote(str(target_dir)))
             continue
 
         target_dir.mkdir(parents=True, exist_ok=True)
         new_path = target_dir / abspath.name
         try:
             log.info("%s -> %s", abspath, new_path)
             abspath.rename(new_path)
             new_paths.append(new_path)
         except OSError as e:
-            if e.errno == 18:  # cross-device move
-                log.info("%s ->d %s", abspath, target_dir)
-                processes.cmd_interactive("mv", abspath, target_dir)
-                new_paths.append(new_path)
+            if e.errno == 2:  # FileNotFoundError
+                log.error("%s not found", abspath)
             elif e.errno == 39:  # target dir not empty
                 log.info("%s ->m %s", abspath, dest)
-                new_paths.extend(rel_move(abspath.glob("*"), dest, dry_run=dry_run))
-            elif e.errno == 2:  # FileNotFoundError
-                log.error("%s not found", abspath)
+                new_paths.extend(rel_move(abspath.glob("*"), dest, simulate=simulate))
+            elif e.errno == 18:  # cross-device move
+                log.info("%s ->d %s", abspath, target_dir)
+                processes.cmd_interactive("mv", str(abspath), str(target_dir))
+                new_paths.append(new_path)
             else:
                 raise
     return new_paths
 
 
 def rel_mv() -> None:
     args = parse_args()
 
     dest = Path(args.dest).expanduser().resolve()
 
     if args.ext:
         args.sources = [p for source in args.sources for p in file_utils.rglob(source, args.ext)[0]]
-    rel_move(args.sources, dest, dry_run=args.dry_run)
+    rel_move(args.sources, dest, simulate=args.simulate)
 
 
 if __name__ == "__main__":
     rel_mv()
```

### Comparing `xklb-2.5.9/xklb/scripts/sample_compare.py` & `xklb-2.6.1/xklb/scripts/sample_compare.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import argparse, hashlib
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 
 from xklb import usage
 from xklb.scripts import sample_hash
-from xklb.utils import nums, objects
+from xklb.utils import arggroups, nums, objects
 from xklb.utils.log_utils import log
 
 
 def full_hash_file(path):
     sha256_hash = hashlib.sha256()
 
-    with open(path, "rb") as file:
-        for byte_block in iter(lambda: file.read(1048576), b""):
-            sha256_hash.update(byte_block)
+    try:
+        with open(path, "rb") as file:
+            for byte_block in iter(lambda: file.read(1048576), b""):
+                sha256_hash.update(byte_block)
+    except FileNotFoundError:
+        return None
 
     return sha256_hash.hexdigest()
 
 
 def full_hash_compare(paths):
     with ThreadPoolExecutor(max_workers=4) as pool:
         hash_results = list(pool.map(full_hash_file, paths))
@@ -71,28 +74,18 @@
         log.error("Files are not equal:\n%s", paths_str)
 
     return is_equal
 
 
 def sample_compare() -> None:
     parser = argparse.ArgumentParser(prog="library sample-compare", usage=usage.sample_compare)
-    parser.add_argument("--threads", default=1, const=10, nargs="?")
-    parser.add_argument(
-        "--chunk-size",
-        type=int,
-        help="Chunk size in bytes (default is 1%%~0.2%% dependent on file size). If set, recommended to use at least 1048576 (for performance)",
-    )
-    parser.add_argument(
-        "--gap",
-        default="0.1",
-        help="Width between chunks to skip (default 10%%). Values greater than 1 are treated as number of bytes",
-    )
+    arggroups.sample_hash_bytes(parser)
     parser.add_argument("--ignore-holes", "--ignore-sparse", action="store_true")
     parser.add_argument("--skip-full-hash", action="store_true")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
     parser.add_argument("paths", nargs="+")
     args = parser.parse_args()
 
     args.gap = nums.float_from_percent(args.gap)
 
     log.info(objects.dict_filter_bool(args.__dict__))
```

### Comparing `xklb-2.5.9/xklb/scripts/sample_hash.py` & `xklb-2.6.1/xklb/scripts/sample_hash.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse, hashlib, shlex
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import nums, objects
+from xklb.utils import arggroups, nums, objects
 from xklb.utils.log_utils import log
 
 
 def single_thread_read(path, segments, chunk_size):
     with open(path, "rb") as f:
         for start in segments:
             f.seek(start)
@@ -25,15 +25,19 @@
         futures = [pool.submit(open_seek_read, path, start, chunk_size) for start in segments]
 
         for future in futures:
             yield future.result()
 
 
 def sample_hash_file(path, threads=1, gap=0.1, chunk_size=None):
-    file_stats = Path(path).stat()
+    try:
+        file_stats = Path(path).stat()
+    except FileNotFoundError:
+        return None
+
     disk_usage = (
         file_stats.st_blocks * 512
     )  # https://github.com/python/cpython/blob/main/Doc/library/os.rst#files-and-directories
     if file_stats.st_size > disk_usage:
         log.warning(f"File has holes %s", path)
 
     if chunk_size is None:
@@ -51,26 +55,16 @@
         file_hash.update(d)
     file_hash_hex = file_hash.hexdigest()
     return file_hash_hex
 
 
 def sample_hash() -> None:
     parser = argparse.ArgumentParser(prog="library sample-hash", usage=usage.sample_hash)
-    parser.add_argument("--threads", default=1, const=10, nargs="?")
-    parser.add_argument(
-        "--chunk-size",
-        type=int,
-        help="Chunk size in bytes (default is 1%%~0.2%% dependent on file size). If set, recommended to use at least 1048576 (for performance)",
-    )
-    parser.add_argument(
-        "--gap",
-        default="0.1",
-        help="Width between chunks to skip (default 10%%). Values greater than 1 are treated as number of bytes",
-    )
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.sample_hash_bytes(parser)
+    arggroups.debug(parser)
 
     parser.add_argument("paths", nargs="+")
     args = parser.parse_args()
 
     args.gap = nums.float_from_percent(args.gap)
 
     log.info(objects.dict_filter_bool(args.__dict__))
```

### Comparing `xklb-2.5.9/xklb/scripts/scatter.py` & `xklb-2.6.1/xklb/scripts/scatter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import argparse, math, random, sys, tempfile
 from collections import Counter
 from pathlib import Path
-from typing import Dict, List, Tuple, Union
 
 from humanize import naturalsize
 from tabulate import tabulate
 
 from xklb import usage
-from xklb.utils import consts, db_utils, devices, file_utils, iterables, nums, objects, printing
+from xklb.utils import arggroups, consts, db_utils, devices, file_utils, iterables, nums, objects, printing
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library scatter",
         usage=usage.scatter,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue")
     parser.add_argument("--max-files-per-folder", "--max-files-per-directory", type=int)
     parser.add_argument("--policy", "-p")
     parser.add_argument("--group", "-g")
     parser.add_argument("--sort", "-s", default="random()", help="Sort files before moving")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--targets", "--srcmounts", "-m", help="Colon separated destinations eg. /mnt/d1:/mnt/d2")
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     parser.add_argument(
         "relative_paths",
         nargs="+",
         help="Paths to scatter; if using -m any path substring is valid (relative to the root of your mergerfs mount)",
     )
     args = parser.parse_intermixed_args()
     args.db = db_utils.connect(args)
@@ -59,15 +58,15 @@
     args.relative_paths = file_utils.resolve_absolute_paths(args.relative_paths)
     args.targets = file_utils.resolve_absolute_paths(args.targets)
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def get_table(args) -> List[dict]:
+def get_table(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
     or_paths = [f"path like :path_{i}" for i, _path in enumerate(args.relative_paths)]
 
     media = list(
         args.db.query(
             f"""
         select
@@ -91,15 +90,15 @@
             },
         ),
     )
 
     return media
 
 
-def get_path_stats(args, data) -> List[Dict]:
+def get_path_stats(args, data) -> list[dict]:
     read_only_mounts = [
         s for s in args.relative_paths if Path(s).is_absolute() and not any(m in s for m in args.targets)
     ]
     result = []
     for srcmount in args.targets + read_only_mounts:
         disk_files = [d for d in data if d["path"].startswith(srcmount)]
         if disk_files:
@@ -123,15 +122,15 @@
     tbl = printing.col_naturalsize(tbl, "median_size")
     for t in consts.EPOCH_COLUMNS:
         printing.col_naturaldate(tbl, t)
 
     print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
 
 
-def rebin_files(args, disk_stats, all_files) -> Tuple[List, List]:
+def rebin_files(args, disk_stats, all_files) -> tuple[list, list]:
     total_size = sum(d["size"] or 0 for d in all_files)
 
     untouched = []
     to_rebin = []
     full_disks = []
 
     read_only_mounts = [
@@ -191,15 +190,15 @@
         file["from_path"] = file["path"]
         file["path"] = file["path"].replace(file["mount"], new_mount)
         rebinned.append(file)
 
     return untouched, rebinned
 
 
-def get_rel_stats(parents, files) -> List[Dict[str, Union[float, str]]]:
+def get_rel_stats(parents, files) -> list[dict[str, float | str]]:
     mount_space = []
     total_used = 1
     for parent in parents:
         used = sum([file["size"] for file in files if file["path"].startswith(parent)])
         total_used += used
         mount_space.append([parent, used])
```

### Comparing `xklb-2.5.9/xklb/scripts/search_db.py` & `xklb-2.6.1/xklb/scripts/search_db.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,28 @@
 import argparse, json
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import consts, db_utils, objects
+from xklb.utils import arggroups, consts, db_utils, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library search-db", usage=usage.search_db)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
-    parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--exact", action="store_true")
-    parser.add_argument("--flexible-search", "--or", "--flex", action="store_true")
-    parser.add_argument(
-        "--delete",
-        "--remove",
-        "--erase",
-        "--rm",
-        "-rm",
-        action="store_true",
-        help="Delete matching rows",
-    )
-    parser.add_argument("--soft-delete", action="store_true", help="Mark matching rows as deleted")
+    arggroups.sql_fs(parser)
+    arggroups.capability_delete(parser)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     parser.add_argument("table")
     parser.add_argument("search", nargs="+")
     args = parser.parse_intermixed_args()
 
     args.include += args.search
-    if args.db:
-        args.database = args.db
+
     Path(args.database).touch()
     args.db = db_utils.connect(args)
 
     log.info(objects.dict_filter_bool(args.__dict__))
 
     return args
 
@@ -78,15 +64,15 @@
         with args.db.conn:
             cursor = args.db.conn.execute(
                 f"DELETE FROM {args.table} WHERE 1=1 " + " ".join(args.filter_sql),
                 args.filter_bindings,
             )
             deleted_count += cursor.rowcount
         print(f"Deleted {deleted_count} rows")
-    elif args.soft_delete:
+    elif args.mark_deleted:
         modified_row_count = 0
         with args.db.conn:
             cursor = args.db.conn.execute(
                 f"UPDATE {args.table} SET time_deleted={consts.APPLICATION_START} WHERE 1=1 "
                 + " ".join(args.filter_sql),
                 args.filter_bindings,
             )
```

### Comparing `xklb-2.5.9/xklb/scripts/streaming_tab_loader.py` & `xklb-2.6.1/xklb/scripts/streaming_tab_loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import argparse, logging, sys
 from time import sleep
-from typing import List
 
 from xklb import usage
 from xklb.media import media_player
-from xklb.utils import db_utils, objects, processes
+from xklb.utils import arggroups, db_utils, objects, processes
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library surf",
         usage=usage.surf,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("--count", "-n", default=2, type=int)
     parser.add_argument("--target-hosts", "--target", default=None, help="Target hosts IP:Port")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     args = parser.parse_args()
 
     if args.database:
         args.db = db_utils.connect(args)
         log.error("Currently only stdin is supported")
         raise NotImplementedError
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def list_tabs(args) -> List:
+def list_tabs(args) -> list:
     return args.bt_api.list_tabs([])
 
 
 def open_tabs(_args, urls) -> None:
     for url in urls:
         processes.cmd(media_player.get_browser(), url)
```

### Comparing `xklb-2.5.9/xklb/scripts/mining/extract_links.py` & `xklb-2.6.1/xklb/scripts/mining/extract_links.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,30 @@
 import argparse
 
 from xklb import usage
-from xklb.utils import arg_utils, consts, devices, iterables, printing, strings, web
+from xklb.utils import arg_utils, arggroups, consts, devices, iterables, printing, strings, web
 from xklb.utils.log_utils import log
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         prog="library extract-links",
         usage=usage.extract_links,
     )
-    parser.add_argument(
-        "--path-include",
-        "--include-path",
-        "--include",
-        "-s",
-        nargs="*",
-        default=[],
-        help="path substrings for inclusion (all must match to include)",
-    )
-    parser.add_argument(
-        "--text-include",
-        "--include-text",
-        nargs="*",
-        default=[],
-        help="link text substrings for inclusion (all must match to include)",
-    )
-    parser.add_argument(
-        "--after-include",
-        "--include-after",
-        nargs="*",
-        default=[],
-        help="plain text substrings after URL for inclusion (all must match to include)",
-    )
-    parser.add_argument(
-        "--before-include",
-        "--include-before",
-        nargs="*",
-        default=[],
-        help="plain text substrings before URL for inclusion (all must match to include)",
-    )
-    parser.add_argument(
-        "--path-exclude",
-        "--exclude-path",
-        "--exclude",
-        "-E",
-        nargs="*",
-        default=["javascript:", "mailto:", "tel:"],
-        help="path substrings for exclusion (any must match to exclude)",
-    )
-    parser.add_argument(
-        "--text-exclude",
-        "--exclude-text",
-        nargs="*",
-        default=[],
-        help="link text substrings for exclusion (any must match to exclude)",
-    )
-    parser.add_argument(
-        "--after-exclude",
-        "--exclude-after",
-        nargs="*",
-        default=[],
-        help="plain text substrings after URL for exclusion (any must match to exclude)",
-    )
-    parser.add_argument(
-        "--before-exclude",
-        "--exclude-before",
-        nargs="*",
-        default=[],
-        help="plain text substrings before URL for exclusion (any must match to exclude)",
-    )
-
-    parser.add_argument("--strict-include", action="store_true", help="All include args must resolve true")
-    parser.add_argument("--strict-exclude", action="store_true", help="All exclude args must resolve true")
-    parser.add_argument("--case-sensitive", action="store_true", help="Filter with case sensitivity")
-    parser.add_argument(
-        "--no-url-decode",
-        "--skip-url-decode",
-        action="store_true",
-        help="Skip URL-decode for --path-include/--path-exclude",
-    )
+    arggroups.extractor(parser)
+    arggroups.requests(parser)
+    arggroups.selenium(parser)
+    arggroups.filter_links(parser)
 
     parser.add_argument("--print-link-text", "--print-title", action="store_true")
-    parser.add_argument("--cookies", help="path to a Netscape formatted cookies file")
-    parser.add_argument("--cookies-from-browser", metavar="BROWSER[+KEYRING][:PROFILE][::CONTAINER]")
-    parser.add_argument("--selenium", action="store_true")
-    parser.add_argument("--manual", action="store_true", help="Confirm manually in shell before exiting the browser")
-    parser.add_argument("--scroll", action="store_true", help="Scroll down the page; infinite scroll")
-    parser.add_argument("--auto-pager", "--autopager", action="store_true")
-    parser.add_argument("--poke", action="store_true")
-    parser.add_argument("--chrome", action="store_true")
     parser.add_argument("--download", action="store_true", help="Download filtered links")
-    parser.add_argument("--verbose", "-v", action="count", default=0)
-
-    parser.add_argument("--no-extract", "--skip-extract", action="store_true")
     parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
-    parser.add_argument("--file", "-f", help="File with one URL per line")
 
-    parser.add_argument("paths", nargs="*")
+    arggroups.debug(parser)
+    arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
 
     if args.scroll:
         args.selenium = True
 
     if not args.case_sensitive:
         args.before_include = [s.lower() for s in args.before_include]
@@ -200,15 +123,15 @@
                 markup = web.selenium_extract_html(args.driver)
                 yield from parse_inner_urls(args, url, markup)
         else:
             for markup in web.infinite_scroll(args.driver):
                 yield from parse_inner_urls(args, url, markup)
     else:
         if args.local_file:
-            with open(url, "r") as f:
+            with open(url) as f:
                 markup = f.read()
             url = "file://" + url
         else:
             r = web.requests_session(args).get(url, timeout=120)
             if r.status_code == 404:
                 log.warning("404 Not Found Error: %s", url)
                 is_error = True
```

### Comparing `xklb-2.5.9/xklb/scripts/mining/extract_text.py` & `xklb-2.6.1/xklb/scripts/mining/extract_text.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 import argparse, re
+from pathlib import Path
 
 from bs4 import BeautifulSoup, NavigableString
 
 from xklb import usage
-from xklb.utils import arg_utils, devices, iterables, printing, strings, web
+from xklb.utils import arg_utils, arggroups, devices, iterables, printing, strings, web
 from xklb.utils.log_utils import log
 
 
 def parse_args():
     parser = argparse.ArgumentParser(prog="library extract-text", usage=usage.extract_text)
-    parser.add_argument("--skip-links", action="store_true")
-
-    parser.add_argument("--cookies", help="path to a Netscape formatted cookies file")
-    parser.add_argument("--cookies-from-browser", metavar="BROWSER[+KEYRING][:PROFILE][::CONTAINER]")
-    parser.add_argument("--selenium", action="store_true")
-    parser.add_argument("--manual", action="store_true", help="Confirm manually in shell before exiting the browser")
-    parser.add_argument("--scroll", action="store_true", help="Scroll down the page; infinite scroll")
-    parser.add_argument("--auto-pager", "--autopager", action="store_true")
-    parser.add_argument("--poke", action="store_true")
-    parser.add_argument("--chrome", action="store_true")
-
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.requests(parser)
+    arggroups.selenium(parser)
 
+    parser.add_argument("--skip-links", action="store_true")
+    parser.add_argument("--download", "--save", "--write", action="store_true")
     parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
-    parser.add_argument("--file", "-f", help="File with one URL per line")
 
-    parser.add_argument("paths", nargs="*")
+    arggroups.debug(parser)
+    arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
 
     if args.scroll:
         args.selenium = True
 
     return args
 
@@ -70,15 +63,15 @@
                 markup = web.selenium_extract_html(args.driver)
                 yield from parse_text(args, markup)
         else:
             for markup in web.infinite_scroll(args.driver):
                 yield from parse_text(args, markup)
     else:
         if args.local_file:
-            with open(url, "r") as f:
+            with open(url) as f:
                 markup = f.read()
             url = "file://" + url
         else:
             r = web.requests_session(args).get(url, timeout=120)
             if r.status_code == 404:
                 log.warning("404 Not Found Error: %s", url)
                 is_error = True
@@ -95,20 +88,29 @@
 def extract_text() -> None:
     args = parse_args()
 
     if args.selenium:
         web.load_selenium(args)
     try:
         for url in arg_utils.gen_paths(args):
+            output_lines = []
             for s in iterables.return_unique(get_text)(args, url):
                 if s is None:
                     break
 
-                printing.pipe_print(s)
+                if args.download:
+                    output_lines.append(s)
+                else:
+                    printing.pipe_print(s)
 
+            if args.download:
+                save_path = web.url_to_local_path(url)
+                Path(save_path).parent.mkdir(exist_ok=True, parents=True)
+                with open(save_path, "w") as f:
+                    f.writelines(s + "\n" for s in output_lines)
     finally:
         if args.selenium:
             web.quit_selenium(args)
 
 
 if __name__ == "__main__":
     extract_text()
```

### Comparing `xklb-2.5.9/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.6.1/xklb/scripts/mining/mpv_watchlater.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import argparse
 from pathlib import Path
 
 from xklb import history, usage
-from xklb.utils import consts, db_utils, mpv_utils, nums, objects
+from xklb.utils import arggroups, consts, db_utils, mpv_utils, nums, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library mpv-watchlater", usage=usage.mpv_watchlater)
     parser.add_argument("--watch-later-directory", default=consts.DEFAULT_MPV_WATCH_LATER, help=argparse.SUPPRESS)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     args = parser.parse_args()
 
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
```

### Comparing `xklb-2.5.9/xklb/scripts/mining/nouns.py` & `xklb-2.6.1/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.9/xklb/scripts/mining/pushshift.py` & `xklb-2.6.1/xklb/scripts/mining/pushshift.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import argparse, sys
 from pathlib import Path
 
 from xklb import usage
 from xklb.reddit_extract import slim_post_data
-from xklb.utils import db_utils, objects, printing
+from xklb.utils import arggroups, db_utils, objects, printing
 from xklb.utils.log_utils import log
 
 try:
     import orjson
 except ModuleNotFoundError:
     import json as orjson
 
 
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library " + action, usage=usage)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     args = parser.parse_args()
 
-    if args.db:
-        args.database = args.db
     Path(args.database).touch()
     args.db = db_utils.connect(args)
 
     log.info(objects.dict_filter_bool(args.__dict__))
 
     return args
```

### Comparing `xklb-2.5.9/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.6.1/xklb/scripts/mining/reddit_selftext.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import argparse, html
-from typing import Set, Tuple
 from urllib.parse import urlparse
 
 from xklb import db_media, usage
-from xklb.utils import db_utils, log_utils, objects
+from xklb.utils import arggroups, db_utils, log_utils, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library reddit-selftext", usage=usage.reddit_selftext)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     args = parser.parse_args()
 
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def get_page_links(path, text) -> Tuple[Set, Set]:
+def get_page_links(path, text) -> tuple[set, set]:
     from bs4 import BeautifulSoup
 
     soup = BeautifulSoup(html.unescape(text), "lxml")
     internal_links = set()
     external_links = set()
 
     for a in soup.findAll("a", attrs={"href": True}):
```

### Comparing `xklb-2.5.9/xklb/scripts/mining/substack.py` & `xklb-2.6.1/xklb/scripts/mining/substack.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import argparse
 from pathlib import Path
 
 from bs4 import BeautifulSoup
 
 from xklb import db_media, usage
-from xklb.utils import db_utils, nums, objects, web
+from xklb.utils import arggroups, db_utils, nums, objects, web
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library substack", usage=usage.substack)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
-    parser.add_argument("--cookies", help="path to a Netscape formatted cookies file")
-    parser.add_argument("--cookies-from-browser", metavar="BROWSER[+KEYRING][:PROFILE][::CONTAINER]")
+    arggroups.requests(parser)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     parser.add_argument("paths", nargs="+", help="Substack path to extract article for")
     args = parser.parse_intermixed_args()
 
     Path(args.database).touch()
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
```

### Comparing `xklb-2.5.9/xklb/scripts/mining/tildes.py` & `xklb-2.6.1/xklb/scripts/mining/tildes.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 from pathlib import Path
 from time import sleep
 
 from bs4 import BeautifulSoup
 from dateutil import parser
 
 from xklb import db_media, usage
-from xklb.utils import db_utils, nums, objects, web
+from xklb.utils import arggroups, db_utils, nums, objects, web
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library tildes", usage=usage.tildes)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
-    parser.add_argument("--cookies", help="path to a Netscape formatted cookies file")
-    parser.add_argument("--cookies-from-browser", metavar="BROWSER[+KEYRING][:PROFILE][::CONTAINER]")
+    arggroups.requests(parser)
+    arggroups.debug(parser)
 
-    parser.add_argument("database")
+    arggroups.database(parser)
     parser.add_argument("username", help="Tildes.net user to extract comments for")
     args = parser.parse_intermixed_args()
 
     Path(args.database).touch()
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
```

### Comparing `xklb-2.5.9/xklb/utils/arg_utils.py` & `xklb-2.6.1/xklb/utils/arg_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,39 @@
-import argparse, operator, random, sys
-from ast import literal_eval
+import argparse, operator, random
 from pathlib import Path
 
-from xklb.utils import consts, db_utils, iterables
+from xklb.utils import arggroups, consts, db_utils, iterables
 from xklb.utils.consts import SC
-from xklb.utils.iterables import flatten
-
-STDIN_DASH = ["-"]
-
-
-class ArgparseList(argparse.Action):
-    def __call__(self, parser, namespace, values, option_string=None):
-        items = getattr(namespace, self.dest, None) or []
-
-        if isinstance(values, str):
-            items.extend(values.split(","))  # type: ignore
-        else:
-            items.extend(flatten(s.split(",") for s in values))  # type: ignore
-
-        setattr(namespace, self.dest, items)
-
-
-class ArgparseDict(argparse.Action):
-    def __call__(self, parser, args, values, option_string=None):
-        try:
-            d = {}
-            k_eq_v = list(flatten([val.split(" ") for val in values]))
-            for s in k_eq_v:
-                k, v = s.split("=", 1)
-                if any(sym in v for sym in (" [", " {")):
-                    d[k] = literal_eval(v)
-                elif v.strip() in ("True", "False"):
-                    d[k] = bool(v.strip())
-                else:
-                    d[k] = v
-
-        except ValueError as ex:
-            msg = f'Could not parse argument "{values}" as k1=1 k2=2 format {ex}'
-            raise argparse.ArgumentError(self, msg) from ex
-        setattr(args, self.dest, d)
-
-
-class ArgparseArgsOrStdin(argparse.Action):
-    def __call__(self, parser, namespace, values, option_string=None):
-        if values == STDIN_DASH:
-            lines = sys.stdin.readlines()
-            if not lines or (len(lines) == 1 and lines[0].strip() == ""):
-                lines = None
-            else:
-                lines = [s.strip() for s in lines]
-        else:
-            lines = values
-        setattr(namespace, self.dest, lines)
 
 
 def is_sqlite(path):
     try:
         with open(path, "rb") as f:
             header = f.read(16)
         return header == b"SQLite format 3\000"
-    except IOError:
+    except OSError:
         return False
 
 
 def gen_paths(args):
     if args.file:
-        with open(args.file, "r") as f:
+        with open(args.file) as f:
             for line in f:
                 path = line.rstrip("\n")
                 if path.strip():
                     yield path
     else:
         for path in args.paths:
             if path.strip():
                 yield path
 
 
 def stdarg():
     parser = argparse.ArgumentParser()
-    parser.add_argument("--file", "-f", help="File with one URL per line")
-    parser.add_argument("paths", nargs="*", default=STDIN_DASH, action=ArgparseArgsOrStdin)
+    arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
     return gen_paths(args)
 
 
 def override_sort(sort_expression: str) -> str:
     def year_month_sql(var):
         return f"cast(strftime('%Y%m', datetime({var}, 'unixepoch')) as int)"
@@ -155,15 +105,15 @@
         f"subtitle_count {subtitle_count} desc"
         if "subtitle_count" in m_columns
         and args.action == SC.watch
         and not any(
             [
                 args.print,
                 consts.PYTEST_RUNNING,
-                "subtitle_count" in args.where,
+                "subtitle_count" in " ".join(args.where),
                 args.limit != consts.DEFAULT_PLAY_QUEUE,
             ],
         )
         else None,
         *(args.sort or []),
         "duration desc" if args.action in (SC.listen, SC.watch) and args.include else None,
         "size desc" if args.action in (SC.listen, SC.watch) and args.include else None,
@@ -216,13 +166,19 @@
 def override_config(parser, extractor_config, args):
     default_args = {key: parser.get_default(key) for key in vars(args)}
     overridden_args = {k: v for k, v in args.__dict__.items() if default_args.get(k) != v}
     args_env = argparse.Namespace(**{**default_args, **extractor_config, **overridden_args})
     return args_env
 
 
+def kwargs_overwrite(namespace, kwargs):
+    namespace_dict = vars(namespace)
+    namespace_dict.update(kwargs)
+    return argparse.Namespace(**namespace_dict)
+
+
 ops = {"<": operator.lt, "<=": operator.le, "==": operator.eq, "!=": operator.ne, ">=": operator.ge, ">": operator.gt}
 
 
 def cmp(arg1, op, arg2):
     operation = ops.get(op)
-    return operation(arg1, arg2)
+    return operation(arg1, arg2)  # type: ignore
```

### Comparing `xklb-2.5.9/xklb/utils/consts.py` & `xklb-2.6.1/xklb/utils/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,16 @@
     ),
 )
 REGEX_V_REDD_IT = re.compile("https?://v.redd.it/(?:[^/?#&]+)")
 APPLICATION_START = now()
 TERMINAL_SIZE = shutil.get_terminal_size(fallback=(80, 60))
 MOBILE_TERMINAL = TERMINAL_SIZE.columns < 80
 TABULATE_STYLE = "simple"
+DEFAULT_DIFFLIB_RATIO = 0.73
+DEFAULT_MIN_SPLIT = "20s"
 
 EPOCH_COLUMNS = (
     "time_downloaded",  # APPLICATION_START time local file known to exist / time scanned
     "time_deleted",  # APPLICATION_START time local file known to not exist
     "time_created",  # earliest valid time of media creation
     "time_modified",  # time of attempted download, file modification
     "time_played",  # -- history table --
@@ -127,47 +129,48 @@
     return mapper[frequency]
 
 
 SKIP_MEDIA_CHECK = [".iso", ".img", ".vob"]
 
 SPEECH_RECOGNITION_EXTENSIONS = set("mp3|ogg|wav".split("|"))
 OCR_EXTENSIONS = set("gif|jpg|jpeg|png|tif|tff|tiff".split("|"))
-AUDIO_ONLY_EXTENSIONS = set("opus|oga|ogg|mp3|mpga|m2a|m4a|flac|wav|wma|aac|aa3|ac3|ape|mid|midi".split("|"))
+AUDIO_ONLY_EXTENSIONS = set("mka|opus|oga|ogg|mp3|mpga|m2a|m4a|m4b|flac|wav|wma|aac|aa3|ac3|ape|mid|midi".split("|"))
 VIDEO_EXTENSIONS = set(
     (
         "str|aa|aax|acm|adf|adp|dtk|ads|ss2|adx|aea|afc|aix|al|apl"
         "|mac|aptx|aptxhd|aqt|ast|obu|avi|avr|avs|avs2|avs3|bfstm|bcstm|binka"
         "|bit|bmv|brstm|cdg|cdxl|xl|c2|302|daud|str|adp|dav|dss|dts|dtshd|dv"
         "|dif|divx|cdata|eac3|paf|fap|flm|flv|fsb|fwse|g722|722|tco|rco"
         "|g723_1|g729|genh|gsm|h261|h26l|h264|264|avc|mts|m2ts|hca|hevc|h265|265|idf"
         "|ifv|cgi|ipu|sf|ircam|ivr|kux|669|abc|amf|ams|dbm|dmf|dsm|far|it|mdl"
         "|med|mod|mt2|mtm|okt|psm|ptm|s3m|stm|ult|umx|xm|itgz|itr|itz|iso|img"
         "|mdgz|mdr|mdz|s3gz|s3r|s3z|xmgz|xmr|xmz|669|amf|ams|dbm|digi|dmf"
         "|dsm|dtm|far|gdm|ice|imf|it|j2b|m15|mdl|med|mmcmp|mms|mo3|mod|mptm"
         "|mt2|mtm|nst|okt|ogm|ogv|plm|ppm|psm|pt36|ptm|s3m|sfx|sfx2|st26|stk|stm"
-        "|stp|ult|umx|wow|xm|xpk|flv|dat|lvf|m4v|mkv|ts|tp|mk3d|mka|mks|webm|mca|mcc"
-        "|mjpg|mjpeg|mpg|mpeg|mpo|j2k|mlp|mods|moflex|mov|mp4|3gp|3g2|mj2|psp|m4b"
+        "|stp|ult|umx|wow|xm|xpk|flv|dat|lvf|m4v|mkv|ts|tp|mk3d|webm|mca|mcc"
+        "|mjpg|mjpeg|mpg|mpeg|mpo|j2k|mlp|mods|moflex|mov|mp4|3g2|3gp2|3gp|3gpp|3g2|mj2|psp"
         "|ism|ismv|isma|f4v|mp2|mpa|mpc|mjpg|mpl2|msf|mtaf|ul|musx|mvi|mxg"
         "|v|nist|sph|nsp|nut|obu|oma|omg|pjs|pvf|yuv|cif|qcif|rgb|rt|rsd|rmvb|rm"
         "|rsd|rso|sw|sb|sami|sbc|msbc|sbg|scc|sdr2|sds|sdx|ser|sga|shn|vb|son|imx"
         "|sln|mjpg|stl|sup|svag|svs|tak|thd|tta|ans|art|asc|diz|ice|vt|ty|ty+|uw|ub"
         "|v210|yuv10|vag|vc1|rcv|vob|viv|vpk|vqf|vql|vqe|wmv|wsd|xmv|xvag|yop|y4m"
     ).split("|")
 )
+SUBTITLE_EXTENSIONS = set("srt|vtt|mks".split("|"))
 TEXTRACT_EXTENSIONS = set(
     "csv|tab|tsv|doc|docx|eml|epub|json|htm|html|msg|odt|pdf|pptx|ps|rtf|txt|log|xlsx|xls".split("|")
 )
 IMAGE_EXTENSIONS = set(
     (
         "pdf|ai|ait|png|jng|mng|arq|arw|cr2|cs1|dcp|dng|eps|epsf|ps|erf|exv|fff"
         "|gpr|hdp|wdp|jxr|iiq|insp|jpeg|jpg|jpe|mef|mie|mos|mpo|mrw|nef|nrw|orf"
         "|ori|pef|psd|psb|psdt|raf|raw|rw2|rwl|sr2|srw|thm|tiff|tif|x3f|flif|gif"
         "|icc|icm|avif|heic|heif|hif|jp2|jpf|jpm|jpx|j2c|j2k|jpc|3fr|btf|dcr|k25"
         "|kdc|miff|mif|rwz|srf|xcf|bpg|doc|dot|fla|fpx|max|ppt|pps|pot|vsd|xls"
-        "|xlt|pict|pct|360|3g2|3gp2|3gp|3gpp|aax|dvb|f4a|f4b|f4p|f4v|lrv|m4b"
+        "|xlt|pict|pct|360|aax|dvb|f4a|f4b|f4p|f4v|lrv|m4b"
         "|m4p|m4v|mov|qt|mqv|qtif|qti|qif|cr3|crm|jxl|crw|ciff|ind|indd|indt"
         "|nksc|vrd|xmp|la|ofr|pac|riff|rif|wav|webp|wv|asf|divx|djvu|djv|dvr-ms"
         "|flv|insv|inx|swf|wma|wmv|exif|eip|psp|pspimage"
     ).split("|")
 )
```

### Comparing `xklb-2.5.9/xklb/utils/db_utils.py` & `xklb-2.6.1/xklb/utils/db_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import itertools, sqlite3
+from collections.abc import Iterable
 from pathlib import Path
 from textwrap import dedent
-from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Union
+from typing import TYPE_CHECKING, Any
 
 from xklb.utils import consts, iterables, nums, strings
 from xklb.utils.log_utils import log
 
 if TYPE_CHECKING:
     from sqlite_utils import Database
 
@@ -17,15 +18,15 @@
 
 def connect(args, conn=None, **kwargs):
     from sqlite_utils import Database
 
     sqlite3.enable_callback_tracebacks(True)  # noqa: FBT003
 
     class DB(Database):
-        def pop(self, sql: str, params: Optional[Union[Iterable, dict]] = None, ignore_errors=None) -> Optional[Any]:
+        def pop(self, sql: str, params: Iterable | dict | None = None, ignore_errors=None) -> Any | None:
             if ignore_errors is None:
                 ignore_errors = ["no such table"]
             try:
                 curs = self.execute(sql, params)
                 data = curs.fetchone()
             except sqlite3.OperationalError as exc:
                 if any(e in str(exc) for e in ignore_errors):
@@ -34,17 +35,17 @@
             if data is None or len(data) == 0:
                 return None
             return data[0]
 
         def pop_dict(
             self,
             sql: str,
-            params: Optional[Union[Iterable, dict]] = None,
+            params: Iterable | dict | None = None,
             ignore_errors=None,
-        ) -> Optional[Dict]:
+        ) -> dict | None:
             if ignore_errors is None:
                 ignore_errors = ["no such table"]
             try:
                 dg = self.query(sql, params)
                 d = next(dg, None)
             except sqlite3.OperationalError as e:
                 if any(ignore_error in str(e) for ignore_error in ignore_errors):
@@ -135,15 +136,15 @@
         ignore_columns = table_config.get("ignore_columns") or []
         search_columns = table_config.get("search_columns") or []
 
         fts_columns = [c for c in search_columns if c in table_columns]
         int_columns = [k for k, v in table_columns.items() if v == int and k not in search_columns + ignore_columns]
         str_columns = [k for k, v in table_columns.items() if v == str and k not in search_columns + ignore_columns]
         if "path" in table_columns:
-            str_columns = list(set([*str_columns, "path"]))
+            str_columns = list({*str_columns, "path"})
 
         optimized_column_order = list(iterables.ordered_set([*int_columns, *(table_config.get("column_order") or [])]))
         compare_order = zip(table_columns, optimized_column_order)
         was_transformed = False
         if not all(x == y for x, y in compare_order):
             log.info("Transforming column order: %s", optimized_column_order)
             db[table].transform(column_order=optimized_column_order)  # type: ignore
@@ -183,15 +184,15 @@
 
     log.info("Running VACUUM")
     db.vacuum()
     log.info("Running ANALYZE")
     db.analyze()
 
 
-def fts_quote(query: List[str]) -> List[str]:
+def fts_quote(query: list[str]) -> list[str]:
     fts_words = [" NOT ", " AND ", " OR ", "*", ":", "NEAR("]
     return [s if any(r in s for r in fts_words) else '"' + s + '"' for s in query]
 
 
 def fts_search_sql(table, fts_table, include, exclude=None, flexible=False):
     param_key = "FTS" + consts.random_string()
     table = f"""(
```

### Comparing `xklb-2.5.9/xklb/utils/devices.py` & `xklb-2.6.1/xklb/utils/devices.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse, os, platform, random, shutil, sys
-from typing import Dict, List, Union
 
+from xklb.utils import arggroups
 from xklb.utils.log_utils import log
 
 
 def get_ip_of_chromecast(device_name) -> str:
     from pychromecast import discovery
 
     cast_infos, browser = discovery.discover_listed_chromecasts(friendly_names=[device_name])
@@ -41,14 +41,22 @@
 def confirm(*args, **kwargs) -> bool:
     from rich.prompt import Confirm
 
     clear_input()
     return Confirm.ask(*args, **kwargs, default=False)
 
 
+def clobber_confirm(args) -> bool:
+    if getattr(args, "replace", False):
+        return True
+    elif getattr(args, "no_replace", False):
+        return False
+    return confirm("Replace destination file?")
+
+
 def prompt(*args, **kwargs) -> str:
     from rich.prompt import Prompt
 
     clear_input()
     return Prompt.ask(*args, **kwargs)
 
 
@@ -79,15 +87,15 @@
 
     readline.set_completer(create_completer(list_))
     readline.set_completer_delims("\t")
     readline.parse_and_bind("tab: complete")
     return
 
 
-def get_mount_stats(src_mounts) -> List[Dict[str, Union[str, int]]]:
+def get_mount_stats(src_mounts) -> list[dict[str, str | int]]:
     mount_space = []
     total_used = 1
     total_free = 1
     grand_total = 1
     for src_mount in src_mounts:
         total, used, free = shutil.disk_usage(src_mount)
         total_used += used
@@ -99,15 +107,15 @@
         {"mount": mount, "used": used / total_used, "free": free / total_free, "total": total / grand_total}
         for mount, used, free, total in mount_space
     ]
 
 
 def mount_stats() -> None:
     parser = argparse.ArgumentParser(add_help=False)
-    parser.add_argument("-v", "--verbose", action="count", default=0)
+    arggroups.debug(parser)
 
     parser.add_argument("mounts", nargs="+")
     args = parser.parse_args()
 
     space = get_mount_stats(args.mounts)
 
     print("Relative disk dependence:")
```

### Comparing `xklb-2.5.9/xklb/utils/file_utils.py` & `xklb-2.6.1/xklb/utils/file_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import errno, mimetypes, os, shlex, shutil, tempfile, time
 from collections import Counter
+from collections.abc import Iterable
 from functools import wraps
 from io import StringIO
 from pathlib import Path
 from shutil import which
-from typing import Iterable, Set, Tuple, Union
 
 import urllib3
 
 from xklb.utils import consts, file_utils, printing, processes, web
 from xklb.utils.log_utils import log
 
 
 def scan_stats(files, filtered_files, folders):
     return (
         f"""Files: {len(files)}{f" [{len(filtered_files)} ignored]" if filtered_files else ''}"""
         f" Folders: {len(folders)}"
     )
 
 
-def rglob(base_dir: str, extensions: Union[None, Iterable[str]] = None) -> Tuple[Set[str], Set[str], Set[str]]:
+def rglob(base_dir: str, extensions: None | Iterable[str] = None) -> tuple[set[str], set[str], set[str]]:
     files = set()
     filtered_files = set()
     folders = set()
     stack = [base_dir]
     while stack:
         current_dir = stack.pop()
         try:
@@ -61,15 +61,15 @@
         shutil.copyfileobj(fo_src, fo_dest)
     fo_dest.seek(0)
     fname = fo_dest.name
     fo_dest.close()
     return fname
 
 
-def trash(path: Union[Path, str], detach=True) -> None:
+def trash(path: Path | str, detach=True) -> None:
     if Path(path).exists():
         trash_put = which("trash-put") or which("trash")
         if trash_put is not None:
             if not detach:
                 processes.cmd(trash_put, path, strict=False)
                 return
             try:
@@ -92,15 +92,15 @@
         for proc in os.listdir("/proc"):
             try:
                 fd_dir = os.path.join("/proc", proc, "fd")
                 for fd in os.listdir(fd_dir):
                     link = os.readlink(os.path.join(fd_dir, fd))
                     if link.startswith("/") and link == path:
                         open_files.add(link)
-            except (OSError, IOError):
+            except OSError:
                 continue
         return path in open_files
 
 
 def filter_file(path, sieve) -> None:
     with open(path) as fr:
         lines = fr.readlines()
```

### Comparing `xklb-2.5.9/xklb/utils/gui.py` & `xklb-2.6.1/xklb/utils/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import NoReturn, Tuple
+from typing import NoReturn
 
 base_folder = Path(__file__).resolve().parent
 
 
 class MrSuperDialogue:
     def __init__(self, path, qty, geom_data=None, true_action="keep", false_action="delete") -> None:
         from tkinter import PhotoImage, Tk
@@ -125,15 +125,15 @@
 
         x_coordinate = x_coordinate + int((s_width / 2) - (s_width / 2))
         y_coordinate = y_coordinate + int((s_height / 2) - (s_height / 2))
         self.root.geometry(f"{s_width}x{s_height}+{x_coordinate}+{y_coordinate}")
         self.root.wm_attributes("-alpha", 1)
 
     @staticmethod
-    def _get_coord_offset_from_monitor(screeninfo_monitor) -> Tuple[int, int]:
+    def _get_coord_offset_from_monitor(screeninfo_monitor) -> tuple[int, int]:
         # TODO: assuming screeninfo returns monitors in the same order that Tk is expecting it should
         # be possible to figure out where the monitor sits in the framebuffer then add up the preceding
         # monitors to find the pixel offset within the framebuffer for the window to show up in
         # that monitor but I have some doubts about whether this will work at all as well as
         # the portability of this solution. I cycle through five different monitors throughout
         # the day but I never use more than one simultaneously so I will stop over-optimizing here:
         raise NotImplementedError
```

### Comparing `xklb-2.5.9/xklb/utils/iterables.py` & `xklb-2.6.1/xklb/utils/iterables.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import math
-from collections.abc import Iterable
+from collections.abc import Iterable, Iterator
 from functools import wraps
-from typing import Any, Iterator, List, Optional, Union
+from typing import Any
 
 from xklb.utils import objects
 
 
 def flatten(xs: Iterable) -> Iterator:
     for x in xs:
         if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
             yield from flatten(x)
         elif isinstance(x, bytes):
             yield x.decode("utf-8")
         else:
             yield x
 
 
-def conform(list_: Union[str, Iterable]) -> List:
+def conform(list_: str | Iterable) -> list:
     if not list_:
         return []
     if not isinstance(list_, list):
         list_ = [list_]
     list_ = flatten(list_)
     list_ = list(filter(bool, list_))
     return list_
 
 
-def safe_unpack(*list_, idx=0, keep_0=True) -> Optional[Any]:
+def safe_unpack(*list_, idx=0, keep_0=True) -> Any | None:
     list_ = conform(list_)
     if not list_:
         return None
 
     try:
         value = list_[idx]
         return value if keep_0 or value != 0 else None
     except IndexError:
         return None
 
 
-def safe_pop(list_, idx=-1) -> Optional[Any]:
+def safe_pop(list_, idx=-1) -> Any | None:
     if not list_:
         return None
     return list_[idx]
 
 
 def get_all_lists(nested_dict):
     list_ = []
@@ -58,15 +58,15 @@
 
 def get_list_with_most_items(nested_dict):
     list_ = get_all_lists(nested_dict)
     list_ = sorted(list_, key=len)
     return safe_pop(list_)
 
 
-def safe_sum(*list_, keep_0=False) -> Optional[Any]:
+def safe_sum(*list_, keep_0=False) -> Any | None:
     list_ = conform(list_)
     if not list_:
         return None
     value = sum(list_)
     return value if keep_0 or value != 0 else None
 
 
@@ -90,37 +90,37 @@
                 break
         if is_key_none:
             none_keys.append(key)
 
     return none_keys
 
 
-def list_dict_filter_bool(media: List[dict], keep_0=True) -> List[dict]:
+def list_dict_filter_bool(media: list[dict], keep_0=True) -> list[dict]:
     keys_to_remove = find_none_keys(media, keep_0=keep_0)
     return [d for d in [{k: v for k, v in m.items() if k not in keys_to_remove} for m in media] if d]
 
 
-def list_dict_filter_keys(media: List[dict], keys) -> List[dict]:
+def list_dict_filter_keys(media: list[dict], keys) -> list[dict]:
     return [d for d in [objects.dict_filter_keys(d, keys) for d in media] if d]
 
 
-def list_dict_filter_unique(data: List[dict]) -> List[dict]:
+def list_dict_filter_unique(data: list[dict]) -> list[dict]:
     if len(data) == 0:
         return []
 
     unique_values = {}
     for key in set.intersection(*(set(d.keys()) for d in data)):
         values = {d[key] for d in data if key in d}
         if len(values) > 1:
             unique_values[key] = values
     filtered_data = [{k: v for k, v in d.items() if k in unique_values} for d in data]
     return filtered_data
 
 
-def list_dict_unique(data: List[dict], unique_keys: List[str]) -> List[dict]:
+def list_dict_unique(data: list[dict], unique_keys: list[str]) -> list[dict]:
     seen = set()
     list_ = []
     for d in data:
         t = tuple(d[key] for key in unique_keys)
 
         if t not in seen:
             seen.add(t)
```

### Comparing `xklb-2.5.9/xklb/utils/log_utils.py` & `xklb-2.6.1/xklb/utils/log_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import argparse, logging, os, sys
 from functools import wraps
 from timeit import default_timer
 
 from IPython.core import ultratb
 from IPython.terminal import debugger
 
+from xklb.utils import arggroups
+
 sys.breakpointhook = debugger.set_trace
 
 
 def clamp_index(arr, idx):
     return arr[min(max(idx, 0), len(arr) - 1)]
 
 
@@ -24,15 +26,15 @@
     f.has_run = False
     return wrapper
 
 
 @run_once
 def argparse_log() -> logging.Logger:
     parser = argparse.ArgumentParser(add_help=False)
-    parser.add_argument("-v", "--verbose", action="count", default=0)
+    arggroups.debug(parser)
     args, _unknown = parser.parse_known_args()
 
     try:
         if args.verbose > 0 and os.getpgrp() == os.tcgetpgrp(sys.stdout.fileno()):
             sys.excepthook = ultratb.FormattedTB(
                 mode="Verbose" if args.verbose > 1 else "Context",
                 color_scheme="Neutral",
```

### Comparing `xklb-2.5.9/xklb/utils/mpv_utils.py` & `xklb-2.6.1/xklb/utils/mpv_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import hashlib, random, time
 from pathlib import Path
-from typing import Optional
 
 from xklb.utils import nums
 from xklb.utils.log_utils import log
 
 
 def path_to_mpv_watchlater_md5(path: str) -> str:
     return hashlib.md5(path.encode("utf-8")).hexdigest().upper()
 
 
-def mpv_watchlater_value(path, key) -> Optional[str]:
+def mpv_watchlater_value(path, key) -> str | None:
     data = Path(path).read_text().splitlines()
     for s in data:
         if s.startswith(key + "="):
             return s.split("=")[1]
     return None
 
 
@@ -41,17 +40,17 @@
         time.sleep(random.uniform(0.8, 1.2))
 
 
 def get_playhead(
     args,
     path: str,
     start_time: float,
-    existing_playhead: Optional[int] = None,
-    media_duration: Optional[int] = None,
-) -> Optional[int]:
+    existing_playhead: int | None = None,
+    media_duration: int | None = None,
+) -> int | None:
     end_time = time.time()
     session_duration = int(end_time - start_time)
     python_playhead = session_duration
     if existing_playhead:
         python_playhead += existing_playhead
 
     md5 = path_to_mpv_watchlater_md5(path)
```

### Comparing `xklb-2.5.9/xklb/utils/nums.py` & `xklb-2.6.1/xklb/utils/nums.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import math, re, statistics
 from datetime import timezone
-from typing import Optional
 
 
 def percent(value, total):
     if total == 0:
         return 0
     return (value / total) * 100
 
@@ -17,24 +16,36 @@
     return v
 
 
 def to_timestamp(dt_object):
     return int(dt_object.replace(tzinfo=timezone.utc).timestamp())
 
 
-def safe_int(s) -> Optional[int]:
+def safe_int(s) -> int | None:
     if not s:
         return None
     try:
         return int(float(s))
     except Exception:
         return None
 
 
-def safe_median(l) -> Optional[float]:
+def safe_int_float_str(s):
+    try:
+        return int(s)
+    except ValueError:
+        pass
+
+    try:
+        return float(s)
+    except ValueError:
+        return s
+
+
+def safe_median(l) -> float | None:
     if not l:
         return None
     try:
         return statistics.median(l)
     except statistics.StatisticsError:
         return None
```

### Comparing `xklb-2.5.9/xklb/utils/objects.py` & `xklb-2.6.1/xklb/utils/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import json, types
 from contextlib import contextmanager
 from functools import wraps
-from typing import Dict, Optional
-
-from xklb.utils.log_utils import log
 
 
 class NoneSpace(types.SimpleNamespace):
     def __getattr__(self, name):
         return None
 
 
@@ -82,46 +79,44 @@
         return obj
 
 
 def lower_keys(input_dict):
     output_dict = {}
     for key, value in input_dict.items():
         lowercase_key = key.lower().strip()
-        if lowercase_key in output_dict:
-            log.info("Overriding key %s: %s -> %s", lowercase_key, output_dict[lowercase_key], value)
         output_dict[lowercase_key] = value
     return output_dict
 
 
-def dict_filter_bool(kwargs, keep_0=True) -> Optional[dict]:
+def dict_filter_bool(kwargs, keep_0=True) -> dict | None:
     if kwargs is None:
         return None
 
     if keep_0:
         filtered_dict = {k: v for k, v in kwargs.items() if v is not None and v != "" and v is not False}
     else:
         filtered_dict = {k: v for k, v in kwargs.items() if v}
 
     if len(filtered_dict) == 0:
         return None
     return filtered_dict
 
 
-def dict_filter_keys(kwargs, keys) -> Optional[dict]:
+def dict_filter_keys(kwargs, keys) -> dict | None:
     filtered_dict = {k: v for k, v in kwargs.items() if k not in keys}
     if len(filtered_dict) == 0:
         return None
     return filtered_dict
 
 
 def dumbcopy(d):
     return {i: j.copy() if type(j) == dict else j for i, j in d.items()}
 
 
-def filter_namespace(args, config_opts) -> Optional[Dict]:
+def filter_namespace(args, config_opts) -> dict | None:
     return dict_filter_bool({k: v for k, v in args.__dict__.items() if k in config_opts})
 
 
 @contextmanager
 def json_shelve(filename, default):
     try:
         with open(filename) as f:
```

### Comparing `xklb-2.5.9/xklb/utils/path_utils.py` & `xklb-2.6.1/xklb/utils/path_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             for i in range(len(segments)):
                 segments[i] = segments[i][:-1]
 
     segments[-1] += extension
     return str(Path(*segments))
 
 
-def clean_path(b, max_name_len=1024, dot_space=False, case_insensitive=False, lowercase_folders=False) -> str:
+def clean_path(b, max_name_len=255, dot_space=False, case_insensitive=False, lowercase_folders=False) -> str:
     import ftfy
 
     p = b.decode("utf-8", "backslashreplace")
     p = ftfy.fix_text(p, explain=False)
     path = Path(p)
     ext = path.suffix
 
@@ -65,21 +65,21 @@
             if any(x in p[1:-1] for x in (" ", "_", ".")):
                 return p.title()
             else:
                 return p.lower()
 
         parent = [case_insensitive_r(p) for p in parent]
 
-    ffmpeg_limit = max_name_len - len(ext.encode()) - len("...")
-    if len(stem.encode()) > ffmpeg_limit:
-        start = stem[: ffmpeg_limit // 2]
-        end = stem[-ffmpeg_limit // 2 :]
-        while len(start.encode()) > ffmpeg_limit // 2:
+    fs_limit = max_name_len - len(ext.encode()) - len("...")
+    if len(stem.encode()) > fs_limit:
+        start = stem[: fs_limit // 2]
+        end = stem[-fs_limit // 2 :]
+        while len(start.encode()) > fs_limit // 2:
             start = start[:-1]
-        while len(end.encode()) > ffmpeg_limit // 2:
+        while len(end.encode()) > fs_limit // 2:
             end = end[1:]
         stem = start + "..." + end
 
     p = str(Path(*parent) / stem)
 
     if dot_space:
         p = p.replace(" ", ".")
```

### Comparing `xklb-2.5.9/xklb/utils/pd_utils.py` & `xklb-2.6.1/xklb/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.9/xklb/utils/printing.py` & `xklb-2.6.1/xklb/utils/printing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import csv, math, os, platform, sys, textwrap
 from datetime import datetime, timedelta
-from typing import Dict, List
 
 import humanize
 
 from xklb.utils import consts
 
 
 def print_overwrite(*text):
@@ -103,68 +102,68 @@
                 lines.append(current_line)
                 current_line = ""
     if current_line:
         lines.append(current_line)
     return "\n".join(lines)
 
 
-def col_resize(tbl: List[Dict], col: str, width) -> List[Dict]:
+def col_resize(tbl: list[dict], col: str, width) -> list[dict]:
     for idx, _d in enumerate(tbl):
         if tbl[idx].get(col) is not None:
             tbl[idx][col] = path_fill(tbl[idx][col], width=width)
 
     return tbl
 
 
-def col_resize_percent(tbl: List[Dict], col: str, percent=10) -> List[Dict]:
+def col_resize_percent(tbl: list[dict], col: str, percent=10) -> list[dict]:
     for idx, _d in enumerate(tbl):
         if tbl[idx].get(col) is not None:
             tbl[idx][col] = path_fill(tbl[idx][col], percent=percent)
 
     return tbl
 
 
-def col_naturaldate(tbl: List[Dict], col: str) -> List[Dict]:
+def col_naturaldate(tbl: list[dict], col: str) -> list[dict]:
     for idx, _d in enumerate(tbl):
         val = tbl[idx].get(col)
         if val is not None:
             val = int(val)
             if val == 0:
                 tbl[idx][col] = None
             else:
                 tbl[idx][col] = humanize.naturaldate(datetime.fromtimestamp(val))
 
     return tbl
 
 
-def col_naturaltime(tbl: List[Dict], col: str) -> List[Dict]:
+def col_naturaltime(tbl: list[dict], col: str) -> list[dict]:
     for idx, _d in enumerate(tbl):
         val = tbl[idx].get(col)
         if val is not None:
             val = int(val)
             if val == 0:
                 tbl[idx][col] = None
             else:
                 tbl[idx][col] = human_time(val)
 
     return tbl
 
 
-def col_naturalsize(tbl: List[Dict], col: str) -> List[Dict]:
+def col_naturalsize(tbl: list[dict], col: str) -> list[dict]:
     for idx, _d in enumerate(tbl):
         if tbl[idx].get(col) is not None:
             if tbl[idx][col] == 0:
                 tbl[idx][col] = None
             else:
                 tbl[idx][col] = humanize.naturalsize(tbl[idx][col], binary=True)
 
     return tbl
 
 
-def col_duration(tbl: List[Dict], col: str) -> List[Dict]:
+def col_duration(tbl: list[dict], col: str) -> list[dict]:
     for idx, _d in enumerate(tbl):
         if tbl[idx].get(col) is not None:
             tbl[idx][col] = human_duration(tbl[idx][col])
     return tbl
 
 
 def wrap_paragraphs(text, width=80):
@@ -225,15 +224,15 @@
     formatted_time = f"{hours:>2}:{minutes:02d}:{seconds:02d}"
     if hours == 0:
         formatted_time = f"   {minutes:>2}:{seconds:02d}"
 
     return formatted_time
 
 
-def col_hhmmss(tbl: List[Dict], col: str) -> List[Dict]:
+def col_hhmmss(tbl: list[dict], col: str) -> list[dict]:
     for idx, _d in enumerate(tbl):
         if tbl[idx].get(col) is not None:
             tbl[idx][col] = seconds_to_hhmmss(tbl[idx][col])
     return tbl
 
 
 def print_df(df):
```

### Comparing `xklb-2.5.9/xklb/utils/processes.py` & `xklb-2.6.1/xklb/utils/processes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import functools, json, multiprocessing, os, platform, re, shlex, signal, subprocess, sys
-from typing import Dict, NoReturn
+from typing import NoReturn
 
 from xklb.utils import iterables
 from xklb.utils.log_utils import log
 
 
 def exit_nicely(_signal, _frame) -> NoReturn:
     log.warning("\nExiting... (Ctrl+C)")
@@ -48,15 +48,15 @@
                 pool.close()
 
         return inner
 
     return decorator
 
 
-def os_bg_kwargs() -> Dict:
+def os_bg_kwargs() -> dict:
     # prevent ctrl-c from affecting subprocesses first
 
     if hasattr(os, "setpgrp"):
         return {"start_new_session": True}
     else:
         # CREATE_NEW_PROCESS_GROUP = 0x00000200
         # DETACHED_PROCESS = 0x00000008
```

### Comparing `xklb-2.5.9/xklb/utils/sql_utils.py` & `xklb-2.6.1/xklb/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.9/xklb/utils/strings.py` & `xklb-2.6.1/xklb/utils/strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import html, re
 from copy import deepcopy
-from typing import Optional
 
 from xklb.data import wordbank
 from xklb.utils import iterables, nums
 from xklb.utils.log_utils import log
 
 
 def repeat_until_same(fn):  # noqa: ANN201
@@ -157,15 +156,15 @@
 
     return s
 
 
 _RE_COMBINE_WHITESPACE = re.compile(r"\s+")
 
 
-def combine(*list_) -> Optional[str]:
+def combine(*list_) -> str | None:
     list_ = iterables.conform(list_)
     if not list_:
         return None
 
     no_comma = sum((str(s).split(",") for s in list_), [])
     no_semicolon = sum((s.split(";") for s in no_comma), [])
     no_double_space = [_RE_COMBINE_WHITESPACE.sub(" ", s).strip() for s in no_semicolon]
@@ -219,14 +218,14 @@
     while len(remove_chars) < 1:
         remove_chars += remove_groups[-number_of_groups]
         number_of_groups += 1
 
     return remove_chars
 
 
-def safe_percent(v) -> Optional[str]:
+def safe_percent(v) -> str | None:
     if v in [None, ""]:
         return None
     try:
         return f"{v:.2%}"
     except Exception:
         return None
```

### Comparing `xklb-2.5.9/xklb/utils/web.py` & `xklb-2.6.1/xklb/utils/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse, datetime, functools, os, re, tempfile, time, urllib.error, urllib.parse, urllib.request
+from email.message import Message
 from pathlib import Path
 from shutil import which
 from urllib.parse import parse_qs, parse_qsl, quote, unquote, urlencode, urljoin, urlparse, urlunparse
 
 import requests
 from idna import decode as puny_decode
 
@@ -79,14 +80,20 @@
         cookie_file = getattr(args, "cookies", None)
         cookies_from_browser = getattr(args, "cookies_from_browser", None)
 
         session = requests.Session()
         session.mount("http", _get_retry_adapter(http_max_retries))  # also includes https
         session.request = functools.partial(session.request, headers=headers, timeout=(4, 45))  # type: ignore
 
+        if getattr(args, "allow_insecure", False):
+            from urllib3.exceptions import InsecureRequestWarning
+
+            requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)  # type: ignore
+            session.verify = False
+
         if cookie_file or cookies_from_browser:
             from yt_dlp.cookies import load_cookies
 
             if cookies_from_browser:
                 cookies_from_browser = parse_cookies_from_browser(cookies_from_browser)
             cookie_jar = load_cookies(cookie_file, cookies_from_browser, ydl=None)
             session.cookies = cookie_jar  # type: ignore
@@ -301,51 +308,114 @@
     if consts.LOG_DEBUG > args.verbose and not getattr(args, "manual", False):
         try:
             args.driver_display.stop()
         except Exception:
             pass
 
 
-def set_output_path(url, output_path, output_prefix, relative, response):
-    if output_path is None:
-        content_d = response.headers.get("Content-Disposition")
-        if content_d:
-            filename = content_d.split("filename=")[1].replace("/", "-")
-        else:
-            filename = url.split("/")[-1]
+def safe_unquote(url):
+    # https://en.wikipedia.org/wiki/Internationalized_Resource_Identifier
+    # we aren't writing HTML so we can unquote
+
+    try:
+        parsed_url = urlparse(url)
+    except UnicodeDecodeError:
+        return url
+
+    def selective_unquote(component, restricted_chars):
+        try:
+            unquoted = unquote(component, errors="strict")
+        except UnicodeDecodeError:
+            return component
+        # re-quote restricted chars
+        return "".join(quote(char, safe="") if char in restricted_chars else char for char in unquoted)
+
+    def unquote_query_params(query):
+        query_pairs = parse_qsl(query, keep_blank_values=True)
+        return "&".join(
+            selective_unquote(key, "=&#") + "=" + selective_unquote(value, "=&#") for key, value in query_pairs
+        )
+
+    unquoted_path = selective_unquote(parsed_url.path, ";?#")
+    unquoted_params = selective_unquote(parsed_url.params, "?#")
+    unquoted_query = unquote_query_params(parsed_url.query)
+    unquoted_fragment = selective_unquote(parsed_url.fragment, "")
+
+    new_url = urlunparse(
+        (parsed_url.scheme, parsed_url.netloc, unquoted_path, unquoted_params, unquoted_query, unquoted_fragment)
+    )
+
+    return new_url
+
+
+def url_decode(href):
+    href = safe_unquote(href)
+    up = urlparse(href)
+    if up.netloc:
+        try:
+            href = href.replace(up.netloc, puny_decode(up.netloc), 1)
+        except Exception:
+            pass
+    return href
+
+
+def path_tuple_from_url(url):
+    url = url_decode(url)
+    parsed_url = urlparse(url)
+    relative_path = os.path.join(parsed_url.netloc, parsed_url.path.lstrip("/"))
+    base_path = os.path.dirname(relative_path)
+    filename = os.path.basename(parsed_url.path)
+    return base_path, filename
+
+
+def filename_from_content_disposition(response):
+    content_disposition = response.headers.get("Content-Disposition", "")
+    if "filename=" in content_disposition:
+        msg = Message()
+        msg["content-disposition"] = content_disposition
+        filename = msg.get_filename()
+        if filename:
+            return filename
+    return None
 
-        base_path = "."
-        if relative:
-            parsed_url = urlparse(url)
-            relative_path = parsed_url.netloc + "/" + parsed_url.path.lstrip("/")
-            base_path = os.path.dirname(relative_path)
 
-        output_path = os.path.join(base_path, filename)
-        output_path = path_utils.clean_path(output_path.encode())
+def url_to_local_path(url, response=None, output_path=None, output_prefix=None):
+    base_path, filename = path_tuple_from_url(url)
+
+    if response:
+        filename_from_site = filename_from_content_disposition(response)
+        if filename_from_site:
+            filename = filename_from_site
+
+    if not output_path:
+        output_path = filename
+        if base_path:
+            output_path = os.path.join(base_path, filename)
+
+    output_path = path_utils.clean_path(output_path.encode())
 
     if output_prefix:
         output_path = os.path.join(output_prefix, output_path)
+
     return output_path
 
 
-def download_url(
-    url, output_path=None, output_prefix=None, relative=False, chunk_size=8 * 1024 * 1024, retry_num=0, max_retries=10
-):
+def download_url(url, output_path=None, output_prefix=None, chunk_size=8 * 1024 * 1024, retry_num=0, max_retries=10):
     if retry_num > max_retries:
         raise RuntimeError(f"Max retries exceeded for {url}")
 
     session = requests_session()
     r = session.get(url, stream=True)
 
     if not 200 <= r.status_code < 400:
         log.error(f"Error {r.status_code} {url}")
 
     remote_size = nums.safe_int(r.headers.get("Content-Length"))
 
-    output_path = set_output_path(url, output_path, output_prefix, relative, r)
+    output_path = url_to_local_path(url, response=r, output_path=output_path, output_prefix=output_prefix)
     if output_path == ".":
         log.warning("Skipping directory %s", url)
         return
     else:
         log.info("Saving %s to %s", url, output_path)
 
     p = Path(output_path)
@@ -380,15 +450,15 @@
                 raise RuntimeError(msg)
     except OSError:
         raise
     except Exception:
         retry_num += 1
         log.info("Retry #%s %s", retry_num, url)
         time.sleep(retry_num)
-        return download_url(url, output_path, output_prefix, relative, chunk_size, retry_num)
+        return download_url(url, output_path, output_prefix, chunk_size, retry_num)
 
     set_timestamp(r.headers, output_path)
     return output_path
 
 
 def get_elements_forward(start, end):
     elements = []
@@ -534,60 +604,14 @@
 
 
 def construct_search(engine, s):
     s = urllib.parse.quote(s, safe="")
     return engine.replace("%", s, 1)
 
 
-def safe_unquote(url):
-    # https://en.wikipedia.org/wiki/Internationalized_Resource_Identifier
-    # we aren't writing HTML so we can unquote
-
-    try:
-        parsed_url = urlparse(url)
-    except UnicodeDecodeError:
-        return url
-
-    def selective_unquote(component, restricted_chars):
-        try:
-            unquoted = unquote(component, errors="strict")
-        except UnicodeDecodeError:
-            return component
-        # re-quote restricted chars
-        return "".join(quote(char, safe="") if char in restricted_chars else char for char in unquoted)
-
-    def unquote_query_params(query):
-        query_pairs = parse_qsl(query, keep_blank_values=True)
-        return "&".join(
-            selective_unquote(key, "=&#") + "=" + selective_unquote(value, "=&#") for key, value in query_pairs
-        )
-
-    unquoted_path = selective_unquote(parsed_url.path, ";?#")
-    unquoted_params = selective_unquote(parsed_url.params, "?#")
-    unquoted_query = unquote_query_params(parsed_url.query)
-    unquoted_fragment = selective_unquote(parsed_url.fragment, "")
-
-    new_url = urlunparse(
-        (parsed_url.scheme, parsed_url.netloc, unquoted_path, unquoted_params, unquoted_query, unquoted_fragment)
-    )
-
-    return new_url
-
-
-def url_decode(href):
-    href = safe_unquote(href)
-    up = urlparse(href)
-    if up.netloc:
-        try:
-            href = href.replace(up.netloc, puny_decode(up.netloc), 1)
-        except Exception:
-            pass
-    return href
-
-
 def construct_absolute_url(base_url, href):
     href = safe_unquote(href)
 
     up = urlparse(href)
     if up.scheme and up.scheme not in ("https", "http", "ftp"):
         return href
```

### Comparing `xklb-2.5.9/xklb/assets/kotobago.png` & `xklb-2.6.1/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.5.9/.gitignore` & `xklb-2.6.1/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+/.mutmut-cache
+/tests/data/Youtube/
 /TODO
 /.ruff_cache/
 /__pypackages__/
 /.pdm-python
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
```

### Comparing `xklb-2.5.9/pyproject.toml` & `xklb-2.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.5.9/.github/README.md` & `xklb-2.6.1/.github/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.5.009)
+    xk media library subcommands (v2.6.001)
 
     Create database subcommands:
     ╭───────────────┬────────────────────────────────────────────────────╮
     │ fsadd         │ Add local media                                    │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ tubeadd       │ Add online video media (yt-dlp)                    │
     ├───────────────┼────────────────────────────────────────────────────┤
@@ -120,14 +120,16 @@
     │ hnadd         │ Create / Update a Hacker News database             │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ substack      │ Backup substack articles                           │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ tildes        │ Backup tildes comments and topics                  │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ places-import │ Import places of interest (POIs)                   │
+    ├───────────────┼────────────────────────────────────────────────────┤
+    │ add-row       │ Add arbitrary data to SQLITE                       │
     ╰───────────────┴────────────────────────────────────────────────────╯
 
     Update database subcommands:
     ╭───────────────┬─────────────────────────────────╮
     │ fsupdate      │ Update local media              │
     ├───────────────┼─────────────────────────────────┤
     │ tubeupdate    │ Update online video media       │
@@ -243,26 +245,37 @@
     │ dedupe-media       │ Dedupe similar media                   │
     ├────────────────────┼────────────────────────────────────────┤
     │ merge-online-local │ Merge online and local data            │
     ├────────────────────┼────────────────────────────────────────┤
     │ mpv-watchlater     │ Import mpv watchlater files to history │
     ├────────────────────┼────────────────────────────────────────┤
     │ reddit-selftext    │ Copy selftext links to media table     │
+    ├────────────────────┼────────────────────────────────────────┤
+    │ tabs-shuffle       │ Randomize tabs.db a bit                │
     ╰────────────────────┴────────────────────────────────────────╯
 
     Misc subcommands:
-    ╭────────────────┬─────────────────────────────────────────────╮
-    │ export-text    │ Export HTML files from SQLite databases     │
-    ├────────────────┼─────────────────────────────────────────────┤
-    │ process-audio  │ Shrink audio by converting to Opus format   │
-    ├────────────────┼─────────────────────────────────────────────┤
-    │ dedupe-czkawka │ Process czkawka diff output                 │
-    ├────────────────┼─────────────────────────────────────────────┤
-    │ nouns          │ Unstructured text -> compound nouns (stdin) │
-    ╰────────────────┴─────────────────────────────────────────────╯
+    ╭────────────────┬────────────────────────────────────────────────────────────╮
+    │ export-text    │ Export HTML files from SQLite databases                    │
+    ├────────────────┼────────────────────────────────────────────────────────────┤
+    │ process-audio  │ Shrink audio by converting to Opus format (.mka)           │
+    ├────────────────┼────────────────────────────────────────────────────────────┤
+    │ process-image  │ Shrink images by converting to AV1 image format (.avif)    │
+    ├────────────────┼────────────────────────────────────────────────────────────┤
+    │ process-video  │ Shrink videos by converting to AV1 video format (.av1.mkv) │
+    ├────────────────┼────────────────────────────────────────────────────────────┤
+    │ dedupe-czkawka │ Process czkawka diff output                                │
+    ├────────────────┼────────────────────────────────────────────────────────────┤
+    │ nouns          │ Unstructured text -> compound nouns (stdin)                │
+    ╰────────────────┴────────────────────────────────────────────────────────────╯
+
+    Other subcommands:
+    ╭────────────────┬────────────────╮
+    │ process-ffmpeg │ process_ffmpeg │
+    ╰────────────────┴────────────────╯
 
 
 </details>
 
 ## Examples
 
 ### Watch online media on your PC
@@ -592,15 +605,56 @@
 <details><summary>Add open-directory media</summary>
 
     $ library webadd -h
     usage: library web-add [(--filesystem) | --video | --audio | --image | --text] DATABASE URL ...
 
     Scan open directories
 
-    library download open_dir.db --fs --prefix ~/d/dump/video/ --relative -vv -s factory -p
+        library web-add open_dir.db --video http://1.1.1.1/
+
+    Check download size of all videos matching some criteria
+
+        library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'height<720' -E preview -pa
+
+        path         count  download_duration                  size    avg_size
+        ---------  -------  ----------------------------  ---------  ----------
+        Aggregate     5694  2 years, 7 months and 5 days  724.4 GiB   130.3 MiB
+
+    Download all videos matching some criteria
+
+        library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'height<720' -E preview
+
+    Stream directly to mpv
+
+        library watch open_dir.db
+
+    Check videos before downloading
+
+        library watch open_dir.db --online-media-only --loop --exit-code-confirm -i --action ask-keep -m 4  --start 35% --volume=0 -w 'height<720' -E preview
+
+        Assuming you have bound in mpv input.conf a key to 'quit' and another key to 'quit 4',
+        using the ask-keep action will mark a video as deleted when you 'quit 4' and it will mark a video as watched when you 'quit'.
+
+        For example, here I bind "'" to "KEEP" and  "j" to "DELETE"
+
+            ' quit
+            j quit 4
+
+        This is pretty intuitive after you use it a few times but writing this out I realize this might seem a bit opaque.
+        Instead of using built-in post-actions (example above) you could also do something like
+            `--cmd5 'echo {} >> keep.txt' --cmd6 'echo {} >> rejected.txt'`
+
+        But you will still bind keys in mpv input.conf:
+
+            k quit 5  # goes to keep.txt
+            r quit 6  # goes to rejected.txt
+
+    Download checked videos
+
+        library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'id in (select media_id from history)'
 
 
 
 </details>
 
 ###### galleryadd
 
@@ -878,14 +932,33 @@
     usage: library places-import DATABASE PATH ...
 
     Load POIs from Google Maps Google Takeout
 
 
 </details>
 
+###### add-row
+
+<details><summary>Add arbitrary data to SQLITE</summary>
+
+    $ library add-row -h
+    usage: library add-row DATABASE [--table-name TABLE_NAME]
+
+    Add a row to sqlite
+
+        library add-row t.db --test_b 1 --test-a 2
+
+        ### media (1 rows)
+        |   test_b |   test_a |
+        |----------|----------|
+        |        1 |        2 |
+
+
+</details>
+
 ### Update database subcommands
 
 ###### fsupdate
 
 <details><summary>Update local media</summary>
 
     $ library fsupdate -h
@@ -1181,15 +1254,15 @@
 
         You may also want to restrict the play queue.
         For example, when you only want 1000 random files:
         library watch -u random -L 1000
 
     Offset the play queue:
         You can also offset the queue. For example if you want to skip one or ten media:
-        library watch --skip 10        # offset ten from the top of an ordered query
+        library watch --offset 10      # offset ten from the top of an ordered query
 
     Repeat
         library watch                  # listen to 120 random songs (DEFAULT_PLAY_QUEUE)
         library watch --limit 5        # listen to FIVE songs
         library watch -l inf -u random # listen to random songs indefinitely
         library watch -s infinite      # listen to songs from the band infinite
 
@@ -1336,14 +1409,35 @@
         Playback multiple files at once
         library watch --multiple-playback    # one per display; or two if only one display detected
         library watch --multiple-playback 4  # play four media at once, divide by available screens
         library watch -m 4 --screen-name eDP # play four media at once on specific screen
         library watch -m 4 --loop --crop     # play four cropped videos on a loop
         library watch -m 4 --hstack          # use hstack style
 
+        When using `--multiple-playback` it may be helpful to set simple window focus rules to prevent keys from accidentally being entered in the wrong mpv window (as new windows are created and capture the cursor focus).
+        You can set and restore your previous mouse focus setting by wrapping the command like this:
+
+            focus-under-mouse
+            library watch ... --multiple-playback 4
+            focus-follows-mouse
+
+        For example in KDE:
+
+            function focus-under-mouse
+                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusUnderMouse
+                qdbus-qt5 org.kde.KWin /KWin reconfigure
+            end
+
+            function focus-follows-mouse
+                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusFollowsMouse
+                kwriteconfig5 --file kwinrc --group Windows --key NextFocusPrefersMouse true
+                qdbus-qt5 org.kde.KWin /KWin reconfigure
+            end
+
+
 
 </details>
 
 ###### open-links
 
 <details><summary>Open links from link dbs</summary>
 
@@ -1589,14 +1683,18 @@
 
     Files will be saved to <lb download prefix>/<extractor>/. If prefix is not specified the current working directory will be used
 
     By default things will download in a random order
 
         library download dl.db --prefix ~/output/path/root/
 
+    But you can sort; eg. oldest first
+
+        library download dl.db -u m.time_modified,m.time_created
+
     Limit downloads to a specified playlist URLs or substring (TODO: https://github.com/chapmanjacobd/library/issues/31)
 
         library download dl.db https://www.youtube.com/c/BlenderFoundation/videos
 
     Limit downloads to a specified video URLs or substring
 
         library download dl.db --include https://www.youtube.com/watch?v=YE7VzlLtp-4
@@ -1921,14 +2019,18 @@
 
     Auto-sort images into directories
 
         echo 'image1.jpg
         image2.jpg
         image3.jpg' | library cluster-sort --image --move-groups
 
+    Print similar paths
+
+        library fs 0day.db -pa --cluster --print-groups
+
 
 
 </details>
 
 ###### extract-links
 
 <details><summary>Extract inner links from lists of web links</summary>
@@ -2043,15 +2145,16 @@
     $ library incremental-diff -h
     usage: library incremental-diff PATH1 PATH2 [--join-keys JOIN_KEYS] [--table1 TABLE1] [--table2 TABLE2] [--table1-index TABLE1_INDEX] [--table2-index TABLE2_INDEX] [--start-row START_ROW] [--batch-size BATCH_SIZE]
 
     See data differences in an incremental way to quickly see how two different files differ.
 
     Data (PATH1, PATH2) can be two different files of different file formats (CSV, Excel) or it could even be the same file with different tables.
 
-    If files are unsorted you may need to use `--join-keys id,name` to specify ID columns. Rows that have the same ID will then be compared. If you are comparing SQLITE files you may be able to use `--sort id,name` to achieve the same effect.
+    If files are unsorted you may need to use `--join-keys id,name` to specify ID columns. Rows that have the same ID will then be compared.
+    If you are comparing SQLITE files you may be able to use `--sort id,name` to achieve the same effect.
 
     To diff everything at once run with `--batch-size inf`
 
 
 </details>
 
 ###### media-check
@@ -2061,31 +2164,36 @@
     $ library media-check -h
     usage: library media-check [--chunk-size SECONDS] [--gap SECONDS OR 0.0-1.0*DURATION] [--delete-corrupt >0-100] [--full-scan] [--audio-scan] PATH ...
 
     Defaults to decode 0.5 second per 10% of each file
 
         library media-check ./video.mp4
 
-    Decode all the frames of each file to evaluate how corrupt it is (very slow; about 150 seconds for an hour-long file)
+    Decode all the frames of each file to evaluate how corrupt it is
+    (scantime is very slow; about 150 seconds for an hour-long file)
 
         library media-check --full-scan ./video.mp4
 
-    Decode all the packets of each file to evaluate how corrupt it is (about one second of each file but only accurate for formats where 1 packet == 1 frame)
+    Decode all the packets of each file to evaluate how corrupt it is
+    (scantime is about one second of each file but only accurate for formats where 1 packet == 1 frame)
 
         library media-check --full-scan --gap 0 ./video.mp4
 
-    Decode all audio of each file to evaluate how corrupt it is (about four seconds per file)
+    Decode all audio of each file to evaluate how corrupt it is
+    (scantime is about four seconds per file)
 
         library media-check --full-scan --audio ./video.mp4
 
-    Decode at least one frame at the start and end of each file to evaluate how corrupt it is (takes about one second per file)
+    Decode at least one frame at the start and end of each file to evaluate how corrupt it is
+    (scantime is about one second per file)
 
         library media-check --chunk-size 5% --gap 99.9% ./video.mp4
 
-    Decode 3s every 5% of a file to evaluate how corrupt it is (takes about three seconds per file)
+    Decode 3s every 5% of a file to evaluate how corrupt it is
+    (scantime is about three seconds per file)
 
         library media-check --chunk-size 3 --gap 5% ./video.mp4
 
     Delete the file if 20 percent or more of checks fail
 
         library media-check --delete-corrupt 20% ./video.mp4
 
@@ -2157,15 +2265,15 @@
 ### Folder subcommands
 
 ###### merge-folders
 
 <details><summary>Merge two or more file trees</summary>
 
     $ library merge-folders -h
-    usage: library merge-folders [--replace] [--skip] [--simulate] SOURCES ... DESTINATION
+    usage: library merge-folders [--replace] [--no-replace] [--simulate] SOURCES ... DESTINATION
 
     Merge multiple folders with the same file tree into a single folder.
 
     https://github.com/chapmanjacobd/journal/blob/main/programming/linux/misconceptions.md#mv-src-vs-mv-src
 
     Trumps are new or replaced files from an earlier source which now conflict with a later source.
     If you only have one source then the count of trumps will always be zero.
@@ -2175,27 +2283,27 @@
 </details>
 
 ###### relmv
 
 <details><summary>Move files preserving parent folder hierarchy</summary>
 
     $ library relmv -h
-    usage: library relmv [--dry-run] SOURCE ... DEST
+    usage: library relmv [--simulate] SOURCE ... DEST
 
     Move files/folders without losing hierarchy metadata
 
     Move fresh music to your phone every Sunday:
 
         # move last week music back to their source folders
-        library relmv /mnt/d/80_Now_Listening/ /mnt/d/
+        library mv /mnt/d/sync/weekly/ /mnt/d/check/audio/
 
         # move new music for this week
         library relmv (
             library listen audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
-        ) /mnt/d/80_Now_Listening/
+        ) /mnt/d/sync/weekly/
 
 
 </details>
 
 ###### mv-list
 
 <details><summary>Find specific folders to move to different disks</summary>
@@ -2256,15 +2364,15 @@
 
     After you are done selecting folders you can press ctrl-d and it will save the list to a tmp file:
 
         Paste a path: done
 
             Folder list saved to /tmp/tmp7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
 
-                rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmp7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
+                rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmp7x_75l8 -r --relative -vv --simulate / jim:/free/real/estate/
 
 
 </details>
 
 ###### scatter
 
 <details><summary>Scatter files between folders or disks</summary>
@@ -2405,15 +2513,15 @@
 <details><summary>Clean filenames</summary>
 
     $ library christen -h
     usage: library christen DATABASE [--run]
 
     Rename files to be somewhat normalized
 
-    Default mode is dry-run
+    Default mode is simulate
 
         library christen fs.db
 
     To actually do stuff use the run flag
 
         library christen audio.db --run
 
@@ -2538,19 +2646,31 @@
 </details>
 
 ###### dedupe-media
 
 <details><summary>Dedupe similar media</summary>
 
     $ library dedupe-media -h
-    usage: library [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
+    usage: library dedupe-media [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
 
     Dedupe your files (not to be confused with the dedupe-db subcommand)
 
-    library dedupe video.db / http
+    Exact file matches
+
+        library dedupe-media --fs video.db
+
+    Dedupe based on duration and file basename or dirname similarity
+
+        library dedupe-media video.db --duration --basename -s release_group  # pre-filter with a specific text substring
+        library dedupe-media video.db --duration --basename -u m1.size  # sort such that small files are treated as originals and larger files are deleted
+        library dedupe-media video.db --duration --basename -u 'm1.size desc'  # sort such that large files are treated as originals and smaller files are deleted
+
+    Dedupe online against local media
+
+        library dedupe-media video.db / http
 
 
 </details>
 
 ###### merge-online-local
 
 <details><summary>Merge online and local data</summary>
@@ -2585,38 +2705,72 @@
     usage: library reddit-selftext DATABASE
 
     Extract URLs from reddit selftext from the reddit_posts table to the media table
 
 
 </details>
 
+###### tabs-shuffle
+
+<details><summary>Randomize tabs.db a bit</summary>
+
+    $ library tabs-shuffle -h
+    usage: library tabs-shuffle DATABASE
+
+    Moves each tab to a random day-of-the-week by default
+
+    It may also be useful to shuffle monthly tabs, etc. You can accomplish this like so:
+
+        library tabs-shuffle tabs.db -d  31 -f monthly
+        library tabs-shuffle tabs.db -d  90 -f quarterly
+        library tabs-shuffle tabs.db -d 365 -f yearly
+
+
+</details>
+
 ### Misc subcommands
 
 ###### export-text
 
 <details><summary>Export HTML files from SQLite databases</summary>
 
     $ library export-text -h
     usage: library export-text DATABASE
 
     Generate HTML files from SQLite databases
 
 
 </details>
 
-###### process-audio
+###### process-image
+
+<details><summary>Shrink images by converting to AV1 image format (.avif)</summary>
+
+    $ library process-image -h
+    usage: library process-image PATH ...
+
+    Resize images to max 2400x2400px and format AVIF to save space
+
+
+</details>
+
+### Other subcommands
+
+###### process-ffmpeg
+
+<details><summary>process_ffmpeg</summary>
 
-<details><summary>Shrink audio by converting to Opus format</summary>
+    $ library process-ffmpeg -h
+    usage: library process-ffmpeg PATH ... [--always-split] [--split-longer-than DURATION] [--min-split-segment SECONDS] [--simulate]
 
-    $ library process-audio -h
-    usage: library process-audio PATH ... [--always-split] [--split-longer-than DURATION] [--min-split-segment SECONDS] [--dry-run]
+    Resize videos to max 1440x960px AV1 and/or Opus to save space
 
     Convert audio to Opus. Optionally split up long tracks into multiple files.
 
-        fd -tf -eDTS -eAAC -eWAV -eAIF -eAIFF -eFLAC -eAIFF -eM4A -eMP3 -eOGG -eMP4 -eWMA -j4 -x library process-audio
+        fd -tf -eDTS -eAAC -eWAV -eAIF -eAIFF -eFLAC -eAIFF -eM4A -eMP3 -eOGG -eMP4 -eWMA -j4 -x library process --audio
 
     Use --always-split to _always_ split files if silence is detected
 
         library process-audio --always-split audiobook.m4a
 
     Use --split-longer-than to _only_ detect silence for files in excess of a specific duration
```

### Comparing `xklb-2.5.9/PKG-INFO` & `xklb-2.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: xklb
-Version: 2.5.9
+Version: 2.6.1
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -179,15 +179,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.5.009)
+    xk media library subcommands (v2.6.001)
 
     Create database subcommands:
     ╭───────────────┬────────────────────────────────────────────────────╮
     │ fsadd         │ Add local media                                    │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ tubeadd       │ Add online video media (yt-dlp)                    │
     ├───────────────┼────────────────────────────────────────────────────┤
@@ -208,14 +208,16 @@
     │ hnadd         │ Create / Update a Hacker News database             │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ substack      │ Backup substack articles                           │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ tildes        │ Backup tildes comments and topics                  │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ places-import │ Import places of interest (POIs)                   │
+    ├───────────────┼────────────────────────────────────────────────────┤
+    │ add-row       │ Add arbitrary data to SQLITE                       │
     ╰───────────────┴────────────────────────────────────────────────────╯
 
     Update database subcommands:
     ╭───────────────┬─────────────────────────────────╮
     │ fsupdate      │ Update local media              │
     ├───────────────┼─────────────────────────────────┤
     │ tubeupdate    │ Update online video media       │
@@ -331,26 +333,37 @@
     │ dedupe-media       │ Dedupe similar media                   │
     ├────────────────────┼────────────────────────────────────────┤
     │ merge-online-local │ Merge online and local data            │
     ├────────────────────┼────────────────────────────────────────┤
     │ mpv-watchlater     │ Import mpv watchlater files to history │
     ├────────────────────┼────────────────────────────────────────┤
     │ reddit-selftext    │ Copy selftext links to media table     │
+    ├────────────────────┼────────────────────────────────────────┤
+    │ tabs-shuffle       │ Randomize tabs.db a bit                │
     ╰────────────────────┴────────────────────────────────────────╯
 
     Misc subcommands:
-    ╭────────────────┬─────────────────────────────────────────────╮
-    │ export-text    │ Export HTML files from SQLite databases     │
-    ├────────────────┼─────────────────────────────────────────────┤
-    │ process-audio  │ Shrink audio by converting to Opus format   │
-    ├────────────────┼─────────────────────────────────────────────┤
-    │ dedupe-czkawka │ Process czkawka diff output                 │
-    ├────────────────┼─────────────────────────────────────────────┤
-    │ nouns          │ Unstructured text -> compound nouns (stdin) │
-    ╰────────────────┴─────────────────────────────────────────────╯
+    ╭────────────────┬────────────────────────────────────────────────────────────╮
+    │ export-text    │ Export HTML files from SQLite databases                    │
+    ├────────────────┼────────────────────────────────────────────────────────────┤
+    │ process-audio  │ Shrink audio by converting to Opus format (.mka)           │
+    ├────────────────┼────────────────────────────────────────────────────────────┤
+    │ process-image  │ Shrink images by converting to AV1 image format (.avif)    │
+    ├────────────────┼────────────────────────────────────────────────────────────┤
+    │ process-video  │ Shrink videos by converting to AV1 video format (.av1.mkv) │
+    ├────────────────┼────────────────────────────────────────────────────────────┤
+    │ dedupe-czkawka │ Process czkawka diff output                                │
+    ├────────────────┼────────────────────────────────────────────────────────────┤
+    │ nouns          │ Unstructured text -> compound nouns (stdin)                │
+    ╰────────────────┴────────────────────────────────────────────────────────────╯
+
+    Other subcommands:
+    ╭────────────────┬────────────────╮
+    │ process-ffmpeg │ process_ffmpeg │
+    ╰────────────────┴────────────────╯
 
 
 </details>
 
 ## Examples
 
 ### Watch online media on your PC
@@ -680,15 +693,56 @@
 <details><summary>Add open-directory media</summary>
 
     $ library webadd -h
     usage: library web-add [(--filesystem) | --video | --audio | --image | --text] DATABASE URL ...
 
     Scan open directories
 
-    library download open_dir.db --fs --prefix ~/d/dump/video/ --relative -vv -s factory -p
+        library web-add open_dir.db --video http://1.1.1.1/
+
+    Check download size of all videos matching some criteria
+
+        library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'height<720' -E preview -pa
+
+        path         count  download_duration                  size    avg_size
+        ---------  -------  ----------------------------  ---------  ----------
+        Aggregate     5694  2 years, 7 months and 5 days  724.4 GiB   130.3 MiB
+
+    Download all videos matching some criteria
+
+        library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'height<720' -E preview
+
+    Stream directly to mpv
+
+        library watch open_dir.db
+
+    Check videos before downloading
+
+        library watch open_dir.db --online-media-only --loop --exit-code-confirm -i --action ask-keep -m 4  --start 35% --volume=0 -w 'height<720' -E preview
+
+        Assuming you have bound in mpv input.conf a key to 'quit' and another key to 'quit 4',
+        using the ask-keep action will mark a video as deleted when you 'quit 4' and it will mark a video as watched when you 'quit'.
+
+        For example, here I bind "'" to "KEEP" and  "j" to "DELETE"
+
+            ' quit
+            j quit 4
+
+        This is pretty intuitive after you use it a few times but writing this out I realize this might seem a bit opaque.
+        Instead of using built-in post-actions (example above) you could also do something like
+            `--cmd5 'echo {} >> keep.txt' --cmd6 'echo {} >> rejected.txt'`
+
+        But you will still bind keys in mpv input.conf:
+
+            k quit 5  # goes to keep.txt
+            r quit 6  # goes to rejected.txt
+
+    Download checked videos
+
+        library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'id in (select media_id from history)'
 
 
 
 </details>
 
 ###### galleryadd
 
@@ -966,14 +1020,33 @@
     usage: library places-import DATABASE PATH ...
 
     Load POIs from Google Maps Google Takeout
 
 
 </details>
 
+###### add-row
+
+<details><summary>Add arbitrary data to SQLITE</summary>
+
+    $ library add-row -h
+    usage: library add-row DATABASE [--table-name TABLE_NAME]
+
+    Add a row to sqlite
+
+        library add-row t.db --test_b 1 --test-a 2
+
+        ### media (1 rows)
+        |   test_b |   test_a |
+        |----------|----------|
+        |        1 |        2 |
+
+
+</details>
+
 ### Update database subcommands
 
 ###### fsupdate
 
 <details><summary>Update local media</summary>
 
     $ library fsupdate -h
@@ -1269,15 +1342,15 @@
 
         You may also want to restrict the play queue.
         For example, when you only want 1000 random files:
         library watch -u random -L 1000
 
     Offset the play queue:
         You can also offset the queue. For example if you want to skip one or ten media:
-        library watch --skip 10        # offset ten from the top of an ordered query
+        library watch --offset 10      # offset ten from the top of an ordered query
 
     Repeat
         library watch                  # listen to 120 random songs (DEFAULT_PLAY_QUEUE)
         library watch --limit 5        # listen to FIVE songs
         library watch -l inf -u random # listen to random songs indefinitely
         library watch -s infinite      # listen to songs from the band infinite
 
@@ -1424,14 +1497,35 @@
         Playback multiple files at once
         library watch --multiple-playback    # one per display; or two if only one display detected
         library watch --multiple-playback 4  # play four media at once, divide by available screens
         library watch -m 4 --screen-name eDP # play four media at once on specific screen
         library watch -m 4 --loop --crop     # play four cropped videos on a loop
         library watch -m 4 --hstack          # use hstack style
 
+        When using `--multiple-playback` it may be helpful to set simple window focus rules to prevent keys from accidentally being entered in the wrong mpv window (as new windows are created and capture the cursor focus).
+        You can set and restore your previous mouse focus setting by wrapping the command like this:
+
+            focus-under-mouse
+            library watch ... --multiple-playback 4
+            focus-follows-mouse
+
+        For example in KDE:
+
+            function focus-under-mouse
+                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusUnderMouse
+                qdbus-qt5 org.kde.KWin /KWin reconfigure
+            end
+
+            function focus-follows-mouse
+                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusFollowsMouse
+                kwriteconfig5 --file kwinrc --group Windows --key NextFocusPrefersMouse true
+                qdbus-qt5 org.kde.KWin /KWin reconfigure
+            end
+
+
 
 </details>
 
 ###### open-links
 
 <details><summary>Open links from link dbs</summary>
 
@@ -1677,14 +1771,18 @@
 
     Files will be saved to <lb download prefix>/<extractor>/. If prefix is not specified the current working directory will be used
 
     By default things will download in a random order
 
         library download dl.db --prefix ~/output/path/root/
 
+    But you can sort; eg. oldest first
+
+        library download dl.db -u m.time_modified,m.time_created
+
     Limit downloads to a specified playlist URLs or substring (TODO: https://github.com/chapmanjacobd/library/issues/31)
 
         library download dl.db https://www.youtube.com/c/BlenderFoundation/videos
 
     Limit downloads to a specified video URLs or substring
 
         library download dl.db --include https://www.youtube.com/watch?v=YE7VzlLtp-4
@@ -2009,14 +2107,18 @@
 
     Auto-sort images into directories
 
         echo 'image1.jpg
         image2.jpg
         image3.jpg' | library cluster-sort --image --move-groups
 
+    Print similar paths
+
+        library fs 0day.db -pa --cluster --print-groups
+
 
 
 </details>
 
 ###### extract-links
 
 <details><summary>Extract inner links from lists of web links</summary>
@@ -2131,15 +2233,16 @@
     $ library incremental-diff -h
     usage: library incremental-diff PATH1 PATH2 [--join-keys JOIN_KEYS] [--table1 TABLE1] [--table2 TABLE2] [--table1-index TABLE1_INDEX] [--table2-index TABLE2_INDEX] [--start-row START_ROW] [--batch-size BATCH_SIZE]
 
     See data differences in an incremental way to quickly see how two different files differ.
 
     Data (PATH1, PATH2) can be two different files of different file formats (CSV, Excel) or it could even be the same file with different tables.
 
-    If files are unsorted you may need to use `--join-keys id,name` to specify ID columns. Rows that have the same ID will then be compared. If you are comparing SQLITE files you may be able to use `--sort id,name` to achieve the same effect.
+    If files are unsorted you may need to use `--join-keys id,name` to specify ID columns. Rows that have the same ID will then be compared.
+    If you are comparing SQLITE files you may be able to use `--sort id,name` to achieve the same effect.
 
     To diff everything at once run with `--batch-size inf`
 
 
 </details>
 
 ###### media-check
@@ -2149,31 +2252,36 @@
     $ library media-check -h
     usage: library media-check [--chunk-size SECONDS] [--gap SECONDS OR 0.0-1.0*DURATION] [--delete-corrupt >0-100] [--full-scan] [--audio-scan] PATH ...
 
     Defaults to decode 0.5 second per 10% of each file
 
         library media-check ./video.mp4
 
-    Decode all the frames of each file to evaluate how corrupt it is (very slow; about 150 seconds for an hour-long file)
+    Decode all the frames of each file to evaluate how corrupt it is
+    (scantime is very slow; about 150 seconds for an hour-long file)
 
         library media-check --full-scan ./video.mp4
 
-    Decode all the packets of each file to evaluate how corrupt it is (about one second of each file but only accurate for formats where 1 packet == 1 frame)
+    Decode all the packets of each file to evaluate how corrupt it is
+    (scantime is about one second of each file but only accurate for formats where 1 packet == 1 frame)
 
         library media-check --full-scan --gap 0 ./video.mp4
 
-    Decode all audio of each file to evaluate how corrupt it is (about four seconds per file)
+    Decode all audio of each file to evaluate how corrupt it is
+    (scantime is about four seconds per file)
 
         library media-check --full-scan --audio ./video.mp4
 
-    Decode at least one frame at the start and end of each file to evaluate how corrupt it is (takes about one second per file)
+    Decode at least one frame at the start and end of each file to evaluate how corrupt it is
+    (scantime is about one second per file)
 
         library media-check --chunk-size 5% --gap 99.9% ./video.mp4
 
-    Decode 3s every 5% of a file to evaluate how corrupt it is (takes about three seconds per file)
+    Decode 3s every 5% of a file to evaluate how corrupt it is
+    (scantime is about three seconds per file)
 
         library media-check --chunk-size 3 --gap 5% ./video.mp4
 
     Delete the file if 20 percent or more of checks fail
 
         library media-check --delete-corrupt 20% ./video.mp4
 
@@ -2245,15 +2353,15 @@
 ### Folder subcommands
 
 ###### merge-folders
 
 <details><summary>Merge two or more file trees</summary>
 
     $ library merge-folders -h
-    usage: library merge-folders [--replace] [--skip] [--simulate] SOURCES ... DESTINATION
+    usage: library merge-folders [--replace] [--no-replace] [--simulate] SOURCES ... DESTINATION
 
     Merge multiple folders with the same file tree into a single folder.
 
     https://github.com/chapmanjacobd/journal/blob/main/programming/linux/misconceptions.md#mv-src-vs-mv-src
 
     Trumps are new or replaced files from an earlier source which now conflict with a later source.
     If you only have one source then the count of trumps will always be zero.
@@ -2263,27 +2371,27 @@
 </details>
 
 ###### relmv
 
 <details><summary>Move files preserving parent folder hierarchy</summary>
 
     $ library relmv -h
-    usage: library relmv [--dry-run] SOURCE ... DEST
+    usage: library relmv [--simulate] SOURCE ... DEST
 
     Move files/folders without losing hierarchy metadata
 
     Move fresh music to your phone every Sunday:
 
         # move last week music back to their source folders
-        library relmv /mnt/d/80_Now_Listening/ /mnt/d/
+        library mv /mnt/d/sync/weekly/ /mnt/d/check/audio/
 
         # move new music for this week
         library relmv (
             library listen audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
-        ) /mnt/d/80_Now_Listening/
+        ) /mnt/d/sync/weekly/
 
 
 </details>
 
 ###### mv-list
 
 <details><summary>Find specific folders to move to different disks</summary>
@@ -2344,15 +2452,15 @@
 
     After you are done selecting folders you can press ctrl-d and it will save the list to a tmp file:
 
         Paste a path: done
 
             Folder list saved to /tmp/tmp7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
 
-                rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmp7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
+                rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmp7x_75l8 -r --relative -vv --simulate / jim:/free/real/estate/
 
 
 </details>
 
 ###### scatter
 
 <details><summary>Scatter files between folders or disks</summary>
@@ -2493,15 +2601,15 @@
 <details><summary>Clean filenames</summary>
 
     $ library christen -h
     usage: library christen DATABASE [--run]
 
     Rename files to be somewhat normalized
 
-    Default mode is dry-run
+    Default mode is simulate
 
         library christen fs.db
 
     To actually do stuff use the run flag
 
         library christen audio.db --run
 
@@ -2626,19 +2734,31 @@
 </details>
 
 ###### dedupe-media
 
 <details><summary>Dedupe similar media</summary>
 
     $ library dedupe-media -h
-    usage: library [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
+    usage: library dedupe-media [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
 
     Dedupe your files (not to be confused with the dedupe-db subcommand)
 
-    library dedupe video.db / http
+    Exact file matches
+
+        library dedupe-media --fs video.db
+
+    Dedupe based on duration and file basename or dirname similarity
+
+        library dedupe-media video.db --duration --basename -s release_group  # pre-filter with a specific text substring
+        library dedupe-media video.db --duration --basename -u m1.size  # sort such that small files are treated as originals and larger files are deleted
+        library dedupe-media video.db --duration --basename -u 'm1.size desc'  # sort such that large files are treated as originals and smaller files are deleted
+
+    Dedupe online against local media
+
+        library dedupe-media video.db / http
 
 
 </details>
 
 ###### merge-online-local
 
 <details><summary>Merge online and local data</summary>
@@ -2673,38 +2793,72 @@
     usage: library reddit-selftext DATABASE
 
     Extract URLs from reddit selftext from the reddit_posts table to the media table
 
 
 </details>
 
+###### tabs-shuffle
+
+<details><summary>Randomize tabs.db a bit</summary>
+
+    $ library tabs-shuffle -h
+    usage: library tabs-shuffle DATABASE
+
+    Moves each tab to a random day-of-the-week by default
+
+    It may also be useful to shuffle monthly tabs, etc. You can accomplish this like so:
+
+        library tabs-shuffle tabs.db -d  31 -f monthly
+        library tabs-shuffle tabs.db -d  90 -f quarterly
+        library tabs-shuffle tabs.db -d 365 -f yearly
+
+
+</details>
+
 ### Misc subcommands
 
 ###### export-text
 
 <details><summary>Export HTML files from SQLite databases</summary>
 
     $ library export-text -h
     usage: library export-text DATABASE
 
     Generate HTML files from SQLite databases
 
 
 </details>
 
-###### process-audio
+###### process-image
+
+<details><summary>Shrink images by converting to AV1 image format (.avif)</summary>
+
+    $ library process-image -h
+    usage: library process-image PATH ...
+
+    Resize images to max 2400x2400px and format AVIF to save space
+
+
+</details>
+
+### Other subcommands
+
+###### process-ffmpeg
+
+<details><summary>process_ffmpeg</summary>
 
-<details><summary>Shrink audio by converting to Opus format</summary>
+    $ library process-ffmpeg -h
+    usage: library process-ffmpeg PATH ... [--always-split] [--split-longer-than DURATION] [--min-split-segment SECONDS] [--simulate]
 
-    $ library process-audio -h
-    usage: library process-audio PATH ... [--always-split] [--split-longer-than DURATION] [--min-split-segment SECONDS] [--dry-run]
+    Resize videos to max 1440x960px AV1 and/or Opus to save space
 
     Convert audio to Opus. Optionally split up long tracks into multiple files.
 
-        fd -tf -eDTS -eAAC -eWAV -eAIF -eAIFF -eFLAC -eAIFF -eM4A -eMP3 -eOGG -eMP4 -eWMA -j4 -x library process-audio
+        fd -tf -eDTS -eAAC -eWAV -eAIF -eAIFF -eFLAC -eAIFF -eM4A -eMP3 -eOGG -eMP4 -eWMA -j4 -x library process --audio
 
     Use --always-split to _always_ split files if silence is detected
 
         library process-audio --always-split audiobook.m4a
 
     Use --split-longer-than to _only_ detect silence for files in excess of a specific duration
```

