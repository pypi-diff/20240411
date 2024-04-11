# Comparing `tmp/senpwai-2.1.7.tar.gz` & `tmp/senpwai-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "senpwai-2.1.7.tar", max compression
+gzip compressed data, was "senpwai-2.1.8.tar", max compression
```

## Comparing `senpwai-2.1.7.tar` & `senpwai-2.1.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    35823 2024-02-27 02:54:57.469943 senpwai-2.1.7/LICENSE
--rw-r--r--   0        0        0     4435 2024-04-02 19:10:28.650268 senpwai-2.1.7/pyproject.toml
--rw-r--r--   0        0        0     6465 2024-02-27 02:54:57.471939 senpwai-2.1.7/README.md
--rw-r--r--   0        0        0        0 2024-02-27 02:54:57.615906 senpwai-2.1.7/senpwai/__init__.py
--rw-r--r--   0        0        0       73 2024-02-27 02:54:57.616904 senpwai-2.1.7/senpwai/__main__.py
--rw-r--r--   0        0        0   167773 2024-02-27 02:54:57.620926 senpwai-2.1.7/senpwai/assets/audio/aqua-crying.mp3
--rw-r--r--   0        0        0    28037 2024-02-27 02:54:57.621905 senpwai-2.1.7/senpwai/assets/audio/bunshin-poof.mp3
--rw-r--r--   0        0        0   257620 2024-02-27 02:54:57.625930 senpwai-2.1.7/senpwai/assets/audio/gigachad.mp3
--rw-r--r--   0        0        0    45701 2024-02-27 02:54:57.628908 senpwai-2.1.7/senpwai/assets/audio/kage-bunshin-no-jutsu.mp3
--rw-r--r--   0        0        0    38481 2024-02-27 02:54:57.630908 senpwai-2.1.7/senpwai/assets/audio/merry-chrismasu.mp3
--rw-r--r--   0        0        0    91267 2024-02-27 02:54:57.632906 senpwai-2.1.7/senpwai/assets/audio/morbin-time.mp3
--rw-r--r--   0        0        0   230876 2024-02-27 02:54:57.636908 senpwai-2.1.7/senpwai/assets/audio/one-piece-real-1.mp3
--rw-r--r--   0        0        0   184032 2024-02-27 02:54:57.639940 senpwai-2.1.7/senpwai/assets/audio/one-piece-real-2.mp3
--rw-r--r--   0        0        0   132304 2024-02-27 02:54:57.642941 senpwai-2.1.7/senpwai/assets/audio/sen-favourite.wav
--rw-r--r--   0        0        0    48659 2024-02-27 02:54:57.645909 senpwai-2.1.7/senpwai/assets/audio/toki-wa-ugoki-dasu.mp3
--rw-r--r--   0        0        0   348653 2024-02-27 02:54:57.653909 senpwai-2.1.7/senpwai/assets/audio/what-da-hell.mp3
--rw-r--r--   0        0        0   463516 2024-02-27 02:54:57.664911 senpwai-2.1.7/senpwai/assets/audio/za-warudo.mp3
--rw-r--r--   0        0        0   348902 2024-02-27 02:54:57.671911 senpwai-2.1.7/senpwai/assets/background-images/about.jpg
--rw-r--r--   0        0        0   617045 2024-02-27 02:54:57.681432 senpwai-2.1.7/senpwai/assets/background-images/chopper-crying.png
--rw-r--r--   0        0        0   392654 2024-02-27 02:54:57.688431 senpwai-2.1.7/senpwai/assets/background-images/chosen-anime.jpg
--rw-r--r--   0        0        0   172353 2024-02-27 02:54:57.692430 senpwai-2.1.7/senpwai/assets/background-images/christmas.jpg
--rw-r--r--   0        0        0   884962 2024-02-27 02:54:57.703431 senpwai-2.1.7/senpwai/assets/background-images/downloads.png
--rw-r--r--   0        0        0   357703 2024-02-27 02:54:57.709432 senpwai-2.1.7/senpwai/assets/background-images/search.jpg
--rw-r--r--   0        0        0   247094 2024-02-27 02:54:57.714432 senpwai-2.1.7/senpwai/assets/background-images/settings.jpg
--rw-r--r--   0        0        0   405642 2024-02-27 02:54:57.721432 senpwai-2.1.7/senpwai/assets/background-images/update.jpg
--rw-r--r--   0        0        0     1227 2024-02-27 02:54:57.722432 senpwai-2.1.7/senpwai/assets/download-icons/cancel.png
--rw-r--r--   0        0        0      757 2024-02-27 02:54:57.723432 senpwai-2.1.7/senpwai/assets/download-icons/down.png
--rw-r--r--   0        0        0      694 2024-02-27 02:54:57.724431 senpwai-2.1.7/senpwai/assets/download-icons/pause.png
--rw-r--r--   0        0        0      920 2024-02-27 02:54:57.725432 senpwai-2.1.7/senpwai/assets/download-icons/resume.png
--rw-r--r--   0        0        0      781 2024-02-27 02:54:57.726437 senpwai-2.1.7/senpwai/assets/download-icons/trash.png
--rw-r--r--   0        0        0      641 2024-02-27 02:54:57.727433 senpwai-2.1.7/senpwai/assets/download-icons/up.png
--rw-r--r--   0        0        0    27409 2024-02-27 02:54:57.729464 senpwai-2.1.7/senpwai/assets/link-icons/discord.png
--rw-r--r--   0        0        0    16226 2024-02-27 02:54:57.730425 senpwai-2.1.7/senpwai/assets/link-icons/github-sponsors.svg
--rw-r--r--   0        0        0    22763 2024-02-27 02:54:57.731426 senpwai-2.1.7/senpwai/assets/link-icons/github.png
--rw-r--r--   0        0        0    17064 2024-02-27 02:54:57.732430 senpwai-2.1.7/senpwai/assets/link-icons/patreon.png
--rw-r--r--   0        0        0    35215 2024-02-27 02:54:57.734432 senpwai-2.1.7/senpwai/assets/link-icons/reddit.png
--rw-r--r--   0        0        0    49259 2024-02-27 02:54:57.736432 senpwai-2.1.7/senpwai/assets/mascots/1.png
--rw-r--r--   0        0        0    69802 2024-02-27 02:54:57.739434 senpwai-2.1.7/senpwai/assets/mascots/2.png
--rw-r--r--   0        0        0     4258 2024-02-27 02:54:57.740433 senpwai-2.1.7/senpwai/assets/misc/folder.png
--rw-r--r--   0        0        0   625301 2024-02-27 02:54:57.754464 senpwai-2.1.7/senpwai/assets/misc/loading.gif
--rw-r--r--   0        0        0    89481 2024-02-27 02:54:57.757459 senpwai-2.1.7/senpwai/assets/misc/sadge-piece.gif
--rw-r--r--   0        0        0    99300 2024-02-27 02:54:57.760429 senpwai-2.1.7/senpwai/assets/misc/senpwai-icon.ico
--rw-r--r--   0        0        0     8044 2024-02-27 02:54:57.761438 senpwai-2.1.7/senpwai/assets/misc/task-complete.png
--rw-r--r--   0        0        0    16336 2024-02-27 02:54:57.763436 senpwai-2.1.7/senpwai/assets/navigation-bar-icons/about.png
--rw-r--r--   0        0        0     7749 2024-02-27 02:54:57.764436 senpwai-2.1.7/senpwai/assets/navigation-bar-icons/downloads.png
--rw-r--r--   0        0        0    19245 2024-02-27 02:54:57.765437 senpwai-2.1.7/senpwai/assets/navigation-bar-icons/search.png
--rw-r--r--   0        0        0    10851 2024-02-27 02:54:57.767439 senpwai-2.1.7/senpwai/assets/navigation-bar-icons/settings.png
--rw-r--r--   0        0        0     6454 2024-02-27 02:54:57.768437 senpwai-2.1.7/senpwai/assets/navigation-bar-icons/update.png
--rw-r--r--   0        0        0    96597 2024-02-27 02:54:57.772439 senpwai-2.1.7/senpwai/assets/reviewer-profile-pics/hentai-addict.png
--rw-r--r--   0        0        0    19936 2024-02-27 02:54:57.773439 senpwai-2.1.7/senpwai/assets/reviewer-profile-pics/morbius-is-peak.png
--rw-r--r--   0        0        0    52908 2024-02-27 02:54:57.774438 senpwai-2.1.7/senpwai/assets/reviewer-profile-pics/sen.png
--rw-r--r--   0        0        0     1710 2024-03-13 02:52:36.375376 senpwai-2.1.7/senpwai/main.py
--rw-r--r--   0        0        0        0 2024-02-27 02:54:57.777958 senpwai-2.1.7/senpwai/scrapers/__init__.py
--rw-r--r--   0        0        0      109 2024-03-05 08:24:06.852246 senpwai-2.1.7/senpwai/scrapers/gogo/__init__.py
--rw-r--r--   0        0        0     1112 2024-03-05 08:24:06.852246 senpwai-2.1.7/senpwai/scrapers/gogo/constants.py
--rw-r--r--   0        0        0     5196 2024-02-27 02:54:57.781957 senpwai-2.1.7/senpwai/scrapers/gogo/hls.py
--rw-r--r--   0        0        0     7747 2024-03-11 19:14:50.991450 senpwai-2.1.7/senpwai/scrapers/gogo/main.py
--rw-r--r--   0        0        0       78 2024-03-05 08:24:06.852246 senpwai-2.1.7/senpwai/scrapers/pahe/__init__.py
--rw-r--r--   0        0        0     1204 2024-03-05 08:24:06.852246 senpwai-2.1.7/senpwai/scrapers/pahe/constants.py
--rw-r--r--   0        0        0    13680 2024-04-02 19:03:05.659479 senpwai-2.1.7/senpwai/scrapers/pahe/main.py
--rw-r--r--   0        0        0    29624 2024-04-02 18:25:35.009961 senpwai-2.1.7/senpwai/scrapers/test.py
--rw-r--r--   0        0        0       81 2024-02-27 02:54:57.788962 senpwai-2.1.7/senpwai/senpcli/__main__.py
--rw-r--r--   0        0        0    23020 2024-03-11 19:14:50.992450 senpwai-2.1.7/senpwai/senpcli/main.py
--rw-r--r--   0        0        0        0 2024-02-27 02:54:57.791960 senpwai-2.1.7/senpwai/utils/__init__.py
--rw-r--r--   0        0        0    14833 2024-03-05 08:24:06.852246 senpwai-2.1.7/senpwai/utils/classes.py
--rw-r--r--   0        0        0    22603 2024-04-02 19:03:15.489710 senpwai-2.1.7/senpwai/utils/scraper.py
--rw-r--r--   0        0        0     9500 2024-04-02 19:10:28.652272 senpwai-2.1.7/senpwai/utils/static.py
--rw-r--r--   0        0        0    25727 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/utils/widgets.py
--rw-r--r--   0        0        0        0 2024-02-27 02:54:57.800965 senpwai-2.1.7/senpwai/windows/__init__.py
--rw-r--r--   0        0        0     8097 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/about.py
--rw-r--r--   0        0        0     2670 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/abstracts.py
--rw-r--r--   0        0        0    20740 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/chosen_anime.py
--rw-r--r--   0        0        0    54375 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/download.py
--rw-r--r--   0        0        0    10393 2024-02-27 02:54:57.808959 senpwai-2.1.7/senpwai/windows/main.py
--rw-r--r--   0        0        0    11995 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/misc.py
--rw-r--r--   0        0        0    18032 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/search.py
--rw-r--r--   0        0        0    27126 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/settings.py
--rw-r--r--   0        0        0     7722 1970-01-01 00:00:00.000000 senpwai-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-02-27 02:54:57.469943 senpwai-2.1.8/LICENSE
+-rw-r--r--   0        0        0     4435 2024-04-11 07:51:23.725066 senpwai-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6578 2024-04-11 07:23:22.981653 senpwai-2.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-02-27 02:54:57.615906 senpwai-2.1.8/senpwai/__init__.py
+-rw-r--r--   0        0        0       73 2024-02-27 02:54:57.616904 senpwai-2.1.8/senpwai/__main__.py
+-rw-r--r--   0        0        0   167773 2024-02-27 02:54:57.620926 senpwai-2.1.8/senpwai/assets/audio/aqua-crying.mp3
+-rw-r--r--   0        0        0    28037 2024-02-27 02:54:57.621905 senpwai-2.1.8/senpwai/assets/audio/bunshin-poof.mp3
+-rw-r--r--   0        0        0   257620 2024-02-27 02:54:57.625930 senpwai-2.1.8/senpwai/assets/audio/gigachad.mp3
+-rw-r--r--   0        0        0    45701 2024-02-27 02:54:57.628908 senpwai-2.1.8/senpwai/assets/audio/kage-bunshin-no-jutsu.mp3
+-rw-r--r--   0        0        0    38481 2024-02-27 02:54:57.630908 senpwai-2.1.8/senpwai/assets/audio/merry-chrismasu.mp3
+-rw-r--r--   0        0        0    91267 2024-02-27 02:54:57.632906 senpwai-2.1.8/senpwai/assets/audio/morbin-time.mp3
+-rw-r--r--   0        0        0   230876 2024-02-27 02:54:57.636908 senpwai-2.1.8/senpwai/assets/audio/one-piece-real-1.mp3
+-rw-r--r--   0        0        0   184032 2024-02-27 02:54:57.639940 senpwai-2.1.8/senpwai/assets/audio/one-piece-real-2.mp3
+-rw-r--r--   0        0        0   132304 2024-02-27 02:54:57.642941 senpwai-2.1.8/senpwai/assets/audio/sen-favourite.wav
+-rw-r--r--   0        0        0    48659 2024-02-27 02:54:57.645909 senpwai-2.1.8/senpwai/assets/audio/toki-wa-ugoki-dasu.mp3
+-rw-r--r--   0        0        0   348653 2024-02-27 02:54:57.653909 senpwai-2.1.8/senpwai/assets/audio/what-da-hell.mp3
+-rw-r--r--   0        0        0   463516 2024-02-27 02:54:57.664911 senpwai-2.1.8/senpwai/assets/audio/za-warudo.mp3
+-rw-r--r--   0        0        0   348902 2024-02-27 02:54:57.671911 senpwai-2.1.8/senpwai/assets/background-images/about.jpg
+-rw-r--r--   0        0        0   617045 2024-02-27 02:54:57.681432 senpwai-2.1.8/senpwai/assets/background-images/chopper-crying.png
+-rw-r--r--   0        0        0   392654 2024-02-27 02:54:57.688431 senpwai-2.1.8/senpwai/assets/background-images/chosen-anime.jpg
+-rw-r--r--   0        0        0   172353 2024-02-27 02:54:57.692430 senpwai-2.1.8/senpwai/assets/background-images/christmas.jpg
+-rw-r--r--   0        0        0   884962 2024-02-27 02:54:57.703431 senpwai-2.1.8/senpwai/assets/background-images/downloads.png
+-rw-r--r--   0        0        0   357703 2024-02-27 02:54:57.709432 senpwai-2.1.8/senpwai/assets/background-images/search.jpg
+-rw-r--r--   0        0        0   247094 2024-02-27 02:54:57.714432 senpwai-2.1.8/senpwai/assets/background-images/settings.jpg
+-rw-r--r--   0        0        0   405642 2024-02-27 02:54:57.721432 senpwai-2.1.8/senpwai/assets/background-images/update.jpg
+-rw-r--r--   0        0        0     1227 2024-02-27 02:54:57.722432 senpwai-2.1.8/senpwai/assets/download-icons/cancel.png
+-rw-r--r--   0        0        0      757 2024-02-27 02:54:57.723432 senpwai-2.1.8/senpwai/assets/download-icons/down.png
+-rw-r--r--   0        0        0      694 2024-02-27 02:54:57.724431 senpwai-2.1.8/senpwai/assets/download-icons/pause.png
+-rw-r--r--   0        0        0      920 2024-02-27 02:54:57.725432 senpwai-2.1.8/senpwai/assets/download-icons/resume.png
+-rw-r--r--   0        0        0      781 2024-02-27 02:54:57.726437 senpwai-2.1.8/senpwai/assets/download-icons/trash.png
+-rw-r--r--   0        0        0      641 2024-02-27 02:54:57.727433 senpwai-2.1.8/senpwai/assets/download-icons/up.png
+-rw-r--r--   0        0        0    27409 2024-02-27 02:54:57.729464 senpwai-2.1.8/senpwai/assets/link-icons/discord.png
+-rw-r--r--   0        0        0    16226 2024-02-27 02:54:57.730425 senpwai-2.1.8/senpwai/assets/link-icons/github-sponsors.svg
+-rw-r--r--   0        0        0    22763 2024-02-27 02:54:57.731426 senpwai-2.1.8/senpwai/assets/link-icons/github.png
+-rw-r--r--   0        0        0    17064 2024-02-27 02:54:57.732430 senpwai-2.1.8/senpwai/assets/link-icons/patreon.png
+-rw-r--r--   0        0        0    35215 2024-02-27 02:54:57.734432 senpwai-2.1.8/senpwai/assets/link-icons/reddit.png
+-rw-r--r--   0        0        0    49259 2024-02-27 02:54:57.736432 senpwai-2.1.8/senpwai/assets/mascots/1.png
+-rw-r--r--   0        0        0    69802 2024-02-27 02:54:57.739434 senpwai-2.1.8/senpwai/assets/mascots/2.png
+-rw-r--r--   0        0        0     4258 2024-02-27 02:54:57.740433 senpwai-2.1.8/senpwai/assets/misc/folder.png
+-rw-r--r--   0        0        0   625301 2024-02-27 02:54:57.754464 senpwai-2.1.8/senpwai/assets/misc/loading.gif
+-rw-r--r--   0        0        0    89481 2024-02-27 02:54:57.757459 senpwai-2.1.8/senpwai/assets/misc/sadge-piece.gif
+-rw-r--r--   0        0        0    99300 2024-02-27 02:54:57.760429 senpwai-2.1.8/senpwai/assets/misc/senpwai-icon.ico
+-rw-r--r--   0        0        0     8044 2024-02-27 02:54:57.761438 senpwai-2.1.8/senpwai/assets/misc/task-complete.png
+-rw-r--r--   0        0        0    16336 2024-02-27 02:54:57.763436 senpwai-2.1.8/senpwai/assets/navigation-bar-icons/about.png
+-rw-r--r--   0        0        0     7749 2024-02-27 02:54:57.764436 senpwai-2.1.8/senpwai/assets/navigation-bar-icons/downloads.png
+-rw-r--r--   0        0        0    19245 2024-02-27 02:54:57.765437 senpwai-2.1.8/senpwai/assets/navigation-bar-icons/search.png
+-rw-r--r--   0        0        0    10851 2024-02-27 02:54:57.767439 senpwai-2.1.8/senpwai/assets/navigation-bar-icons/settings.png
+-rw-r--r--   0        0        0     6454 2024-02-27 02:54:57.768437 senpwai-2.1.8/senpwai/assets/navigation-bar-icons/update.png
+-rw-r--r--   0        0        0    96597 2024-02-27 02:54:57.772439 senpwai-2.1.8/senpwai/assets/reviewer-profile-pics/hentai-addict.png
+-rw-r--r--   0        0        0    19936 2024-02-27 02:54:57.773439 senpwai-2.1.8/senpwai/assets/reviewer-profile-pics/morbius-is-peak.png
+-rw-r--r--   0        0        0    52908 2024-02-27 02:54:57.774438 senpwai-2.1.8/senpwai/assets/reviewer-profile-pics/sen.png
+-rw-r--r--   0        0        0     1711 2024-04-11 00:05:53.611597 senpwai-2.1.8/senpwai/main.py
+-rw-r--r--   0        0        0        0 2024-02-27 02:54:57.777958 senpwai-2.1.8/senpwai/scrapers/__init__.py
+-rw-r--r--   0        0        0      109 2024-04-10 16:10:21.056706 senpwai-2.1.8/senpwai/scrapers/gogo/__init__.py
+-rw-r--r--   0        0        0     1175 2024-04-11 03:49:40.496718 senpwai-2.1.8/senpwai/scrapers/gogo/constants.py
+-rw-r--r--   0        0        0     5196 2024-02-27 02:54:57.781957 senpwai-2.1.8/senpwai/scrapers/gogo/hls.py
+-rw-r--r--   0        0        0     8501 2024-04-11 04:42:36.370908 senpwai-2.1.8/senpwai/scrapers/gogo/main.py
+-rw-r--r--   0        0        0       78 2024-03-05 08:24:06.852246 senpwai-2.1.8/senpwai/scrapers/pahe/__init__.py
+-rw-r--r--   0        0        0     1204 2024-03-05 08:24:06.852246 senpwai-2.1.8/senpwai/scrapers/pahe/constants.py
+-rw-r--r--   0        0        0    13674 2024-04-10 16:16:34.960579 senpwai-2.1.8/senpwai/scrapers/pahe/main.py
+-rw-r--r--   0        0        0    29198 2024-04-11 04:40:38.021786 senpwai-2.1.8/senpwai/scrapers/test.py
+-rw-r--r--   0        0        0       81 2024-02-27 02:54:57.788962 senpwai-2.1.8/senpwai/senpcli/__main__.py
+-rw-r--r--   0        0        0    24218 2024-04-11 07:19:23.047038 senpwai-2.1.8/senpwai/senpcli/main.py
+-rw-r--r--   0        0        0        0 2024-04-09 01:14:15.123895 senpwai-2.1.8/senpwai/utils/__init__.py
+-rw-r--r--   0        0        0    14940 2024-04-11 04:33:27.026164 senpwai-2.1.8/senpwai/utils/classes.py
+-rw-r--r--   0        0        0    23014 2024-04-11 07:39:13.161228 senpwai-2.1.8/senpwai/utils/scraper.py
+-rw-r--r--   0        0        0     9605 2024-04-11 07:51:23.726065 senpwai-2.1.8/senpwai/utils/static.py
+-rw-r--r--   0        0        0    25727 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/utils/widgets.py
+-rw-r--r--   0        0        0        0 2024-02-27 02:54:57.800965 senpwai-2.1.8/senpwai/windows/__init__.py
+-rw-r--r--   0        0        0     8097 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/windows/about.py
+-rw-r--r--   0        0        0     2670 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/windows/abstracts.py
+-rw-r--r--   0        0        0    20740 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/windows/chosen_anime.py
+-rw-r--r--   0        0        0    54312 2024-04-11 04:19:41.774782 senpwai-2.1.8/senpwai/windows/download.py
+-rw-r--r--   0        0        0    10393 2024-02-27 02:54:57.808959 senpwai-2.1.8/senpwai/windows/main.py
+-rw-r--r--   0        0        0    11995 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/windows/misc.py
+-rw-r--r--   0        0        0    18032 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/windows/search.py
+-rw-r--r--   0        0        0    27126 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/windows/settings.py
+-rw-r--r--   0        0        0     7828 1970-01-01 00:00:00.000000 senpwai-2.1.8/PKG-INFO
```

### Comparing `senpwai-2.1.7/LICENSE` & `senpwai-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/pyproject.toml` & `senpwai-2.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "senpwai"
-version = "2.1.7"
+version = "2.1.8"
 description = "A desktop app for tracking and batch downloading anime"
 authors = ["SenZmaKi <senzmaki@gmail.com>"]
 license = "GPL v3"
 readme = "README.md"
 include = ["senpwai/assets"]
 packages = [{ include = "senpwai" }, { include = "senpcli", from = "senpwai" }]
 exclude = ["src/**/test.py"]
```

### Comparing `senpwai-2.1.7/README.md` & `senpwai-2.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,24 +19,31 @@
   <a href="#faq">FAQ</a> •
   <a href="#links">Links</a>
 </p>
 
 <img align="center" src="https://raw.githubusercontent.com/SenZmaKi/Senpwai/master/.github/images/one-piece.png" alt="one-piece-screenshot">
 
 ## Installation
+
 - **Cross-platform (Linux, Mac, Windows 10/11)**
 
 Needs [Python 3.11](https://www.python.org/downloads/release/python-3111) installed.
+
 ```bash
 pip install senpwai
 ```
+
 - **Windows 10/11**
 
 Download [the setup](https://github.com/SenZmaKi/Senpwai/releases/latest/download/Senpwai-setup.exe) then run it.
 
+- **Android**
+
+Check [Senpcli](https://github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md)
+
 - **Other**
 
 [Build from source](#building-from-source).
 
 ## Features
 
 - Download any anime from [Animepahe](https://animepahe.ru) or [Gogoanime](https://anitaku.to).
@@ -60,15 +67,14 @@
 
 1. **Set everything up.**
 
 ```
 git clone https://github.com/SenZmaKi/Senpwai --depth 1 && cd Senpwai && pip install -r dev-requirements.txt && poetry install
 ```
 
-
 2. **Build the app into an executable.**
 
 ```
 poetry run poe build_senpwai_exe
 ```
 
 - The executable will be built in `Senpwai\build\Senpwai`
@@ -82,14 +88,15 @@
 ## Support
 
 - You can support the development of Senpwai through donations on [GitHub Sponsors](https://github.com/sponsors/SenZmaKi) or [Patreon](https://patreon.com/Senpwai).
 - You can also leave a star on the github for more weebs to know about it.
 - Senpwai is open to pull requests, so if you have ideas for improvements, feel free to contribute!
 
 ## Sponsors
+
 <p>
 <a href="https://github.com/Adam1400"><img src="https://github.com/Adam1400.png" width="80px" alt="Adam1400"/></a>&nbsp;&nbsp;<a href="https://github.com/KeithBoehler"><img src="https://github.com/KeithBoehler.png" width="80px" alt="KeithBoehler" /></a>
 </p>
 
 ## FAQ
 
 <details> <summary> Why did you make this? </summary>
```

#### html2text {}

```diff
@@ -4,41 +4,42 @@
               _[_t_e_s_t_-_w_o_r_k_f_l_o_w_-_s_t_a_t_u_s_-_b_a_d_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]/a>
 _I_n_s_t_a_l_l_a_t_i_o_n â¢ _F_e_a_t_u_r_e_s â¢ _C_L_I â¢ _B_u_i_l_d_i_n_g_ _f_r_o_m_ _s_o_u_r_c_e â¢ _S_u_p_p_o_r_t â¢ _F_A_Q
                                    â¢ _L_i_n_k_s
 [one-piece-screenshot]## Installation - **Cross-platform (Linux, Mac, Windows
 10/11)** Needs [Python 3.11](https://www.python.org/downloads/release/python-
 3111) installed. ```bash pip install senpwai ``` - **Windows 10/11** Download
 [the setup](https://github.com/SenZmaKi/Senpwai/releases/latest/download/
-Senpwai-setup.exe) then run it. - **Other** [Build from source](#building-from-
-source). ## Features - Download any anime from [Animepahe](https://
-animepahe.ru) or [Gogoanime](https://anitaku.to). - Keep track of an anime and
-automatically download new episodes when they release. - Download a complete
-season or episodes within a range (e.g., 69-420). - Choose between video
-qualities: 360p, 480p (Gogoanime only), 720p, or 1080p. - Download in sub or
-dub (if available) depending on the user's preference. - Automatically detects
-episodes you already have and avoids re-downloading them. - Robust and graceful
-download error management. - GUI and [CLI](https://github.com/SenZmaKi/Senpwai/
-blob/master/docs/senpcli-guide.md). ## CLI [Senpcli](https://github.com/
-SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md) is a minimalist and
-lightweight CLI alternative for Senpwai. Senpwai is already efficient and
-lightweight, Senpcli basically strips off the GUI while maintaining most of the
-basic functionality. ## Building from Source Ensure you have [Python 3.11]
-(https://www.python.org/downloads/release/python-3111) and [Git](https://
-github.com/git-guides/install-git) installed. Open a terminal and run the
-following commands. 1. **Set everything up.** ``` git clone https://github.com/
-SenZmaKi/Senpwai --depth 1 && cd Senpwai && pip install -r dev-requirements.txt
-&& poetry install ``` 2. **Build the app into an executable.** ``` poetry run
-poe build_senpwai_exe ``` - The executable will be built in
-`Senpwai\build\Senpwai` 3. **Alternatively you can instead run the app directly
-via Python.** ``` poetry run senpwai ``` ## Support - You can support the
-development of Senpwai through donations on [GitHub Sponsors](https://
-github.com/sponsors/SenZmaKi) or [Patreon](https://patreon.com/Senpwai). - You
-can also leave a star on the github for more weebs to know about it. - Senpwai
-is open to pull requests, so if you have ideas for improvements, feel free to
-contribute! ## Sponsors
+Senpwai-setup.exe) then run it. - **Android** Check [Senpcli](https://
+github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md) - **Other**
+[Build from source](#building-from-source). ## Features - Download any anime
+from [Animepahe](https://animepahe.ru) or [Gogoanime](https://anitaku.to). -
+Keep track of an anime and automatically download new episodes when they
+release. - Download a complete season or episodes within a range (e.g., 69-
+420). - Choose between video qualities: 360p, 480p (Gogoanime only), 720p, or
+1080p. - Download in sub or dub (if available) depending on the user's
+preference. - Automatically detects episodes you already have and avoids re-
+downloading them. - Robust and graceful download error management. - GUI and
+[CLI](https://github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md).
+## CLI [Senpcli](https://github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-
+guide.md) is a minimalist and lightweight CLI alternative for Senpwai. Senpwai
+is already efficient and lightweight, Senpcli basically strips off the GUI
+while maintaining most of the basic functionality. ## Building from Source
+Ensure you have [Python 3.11](https://www.python.org/downloads/release/python-
+3111) and [Git](https://github.com/git-guides/install-git) installed. Open a
+terminal and run the following commands. 1. **Set everything up.** ``` git
+clone https://github.com/SenZmaKi/Senpwai --depth 1 && cd Senpwai && pip
+install -r dev-requirements.txt && poetry install ``` 2. **Build the app into
+an executable.** ``` poetry run poe build_senpwai_exe ``` - The executable will
+be built in `Senpwai\build\Senpwai` 3. **Alternatively you can instead run the
+app directly via Python.** ``` poetry run senpwai ``` ## Support - You can
+support the development of Senpwai through donations on [GitHub Sponsors]
+(https://github.com/sponsors/SenZmaKi) or [Patreon](https://patreon.com/
+Senpwai). - You can also leave a star on the github for more weebs to know
+about it. - Senpwai is open to pull requests, so if you have ideas for
+improvements, feel free to contribute! ## Sponsors
 _[_A_d_a_m_1_4_0_0_]  _[_K_e_i_t_h_B_o_e_h_l_e_r_]
 ## FAQ Why did you make this? I couldn't afford wifi so I used my college wifi
 to download anime after class but batch downloading from streaming sites is a
 pain in the ass, you have to click billions of links just to download one
 episode, so I made Senpwai to help me and possibly others that face a similar
 problem. What is HLS mode? HLS mode attempts to fix the unstability of
 Gogoanime normal mode. In HLS mode Gogoanime downloads are guaranteed to work,
```

### Comparing `senpwai-2.1.7/senpwai/assets/audio/aqua-crying.mp3` & `senpwai-2.1.8/senpwai/assets/audio/aqua-crying.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/audio/bunshin-poof.mp3` & `senpwai-2.1.8/senpwai/assets/audio/bunshin-poof.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/audio/gigachad.mp3` & `senpwai-2.1.8/senpwai/assets/audio/gigachad.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/audio/kage-bunshin-no-jutsu.mp3` & `senpwai-2.1.8/senpwai/assets/audio/kage-bunshin-no-jutsu.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/audio/merry-chrismasu.mp3` & `senpwai-2.1.8/senpwai/assets/audio/merry-chrismasu.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/audio/morbin-time.mp3` & `senpwai-2.1.8/senpwai/assets/audio/morbin-time.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/audio/one-piece-real-1.mp3` & `senpwai-2.1.8/senpwai/assets/audio/one-piece-real-1.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/audio/one-piece-real-2.mp3` & `senpwai-2.1.8/senpwai/assets/audio/one-piece-real-2.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/audio/sen-favourite.wav` & `senpwai-2.1.8/senpwai/assets/audio/sen-favourite.wav`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/audio/toki-wa-ugoki-dasu.mp3` & `senpwai-2.1.8/senpwai/assets/audio/toki-wa-ugoki-dasu.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/audio/what-da-hell.mp3` & `senpwai-2.1.8/senpwai/assets/audio/what-da-hell.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/audio/za-warudo.mp3` & `senpwai-2.1.8/senpwai/assets/audio/za-warudo.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/background-images/about.jpg` & `senpwai-2.1.8/senpwai/assets/background-images/about.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/background-images/chopper-crying.png` & `senpwai-2.1.8/senpwai/assets/background-images/chopper-crying.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/background-images/chosen-anime.jpg` & `senpwai-2.1.8/senpwai/assets/background-images/chosen-anime.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/background-images/christmas.jpg` & `senpwai-2.1.8/senpwai/assets/background-images/christmas.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/background-images/downloads.png` & `senpwai-2.1.8/senpwai/assets/background-images/downloads.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/background-images/search.jpg` & `senpwai-2.1.8/senpwai/assets/background-images/search.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/background-images/settings.jpg` & `senpwai-2.1.8/senpwai/assets/background-images/settings.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/background-images/update.jpg` & `senpwai-2.1.8/senpwai/assets/background-images/update.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/download-icons/cancel.png` & `senpwai-2.1.8/senpwai/assets/download-icons/cancel.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/download-icons/down.png` & `senpwai-2.1.8/senpwai/assets/download-icons/down.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/download-icons/pause.png` & `senpwai-2.1.8/senpwai/assets/download-icons/pause.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/download-icons/resume.png` & `senpwai-2.1.8/senpwai/assets/download-icons/resume.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/download-icons/trash.png` & `senpwai-2.1.8/senpwai/assets/download-icons/trash.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/download-icons/up.png` & `senpwai-2.1.8/senpwai/assets/download-icons/up.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/link-icons/discord.png` & `senpwai-2.1.8/senpwai/assets/link-icons/discord.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/link-icons/github-sponsors.svg` & `senpwai-2.1.8/senpwai/assets/link-icons/github-sponsors.svg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/link-icons/github.png` & `senpwai-2.1.8/senpwai/assets/link-icons/github.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/link-icons/patreon.png` & `senpwai-2.1.8/senpwai/assets/link-icons/patreon.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/link-icons/reddit.png` & `senpwai-2.1.8/senpwai/assets/link-icons/reddit.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/mascots/1.png` & `senpwai-2.1.8/senpwai/assets/mascots/1.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/mascots/2.png` & `senpwai-2.1.8/senpwai/assets/mascots/2.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/misc/folder.png` & `senpwai-2.1.8/senpwai/assets/misc/folder.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/misc/loading.gif` & `senpwai-2.1.8/senpwai/assets/misc/loading.gif`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/misc/sadge-piece.gif` & `senpwai-2.1.8/senpwai/assets/misc/sadge-piece.gif`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/misc/senpwai-icon.ico` & `senpwai-2.1.8/senpwai/assets/misc/senpwai-icon.ico`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/misc/task-complete.png` & `senpwai-2.1.8/senpwai/assets/misc/task-complete.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/navigation-bar-icons/about.png` & `senpwai-2.1.8/senpwai/assets/navigation-bar-icons/about.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/navigation-bar-icons/downloads.png` & `senpwai-2.1.8/senpwai/assets/navigation-bar-icons/downloads.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/navigation-bar-icons/search.png` & `senpwai-2.1.8/senpwai/assets/navigation-bar-icons/search.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/navigation-bar-icons/settings.png` & `senpwai-2.1.8/senpwai/assets/navigation-bar-icons/settings.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/navigation-bar-icons/update.png` & `senpwai-2.1.8/senpwai/assets/navigation-bar-icons/update.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/reviewer-profile-pics/hentai-addict.png` & `senpwai-2.1.8/senpwai/assets/reviewer-profile-pics/hentai-addict.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/reviewer-profile-pics/morbius-is-peak.png` & `senpwai-2.1.8/senpwai/assets/reviewer-profile-pics/morbius-is-peak.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/assets/reviewer-profile-pics/sen.png` & `senpwai-2.1.8/senpwai/assets/reviewer-profile-pics/sen.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/main.py` & `senpwai-2.1.8/senpwai/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 import ctypes
 import sys
 
 from PyQt6.QtCore import QCoreApplication, Qt
 from PyQt6.QtGui import QPalette
 from PyQt6.QtWidgets import QApplication
```

### Comparing `senpwai-2.1.7/senpwai/scrapers/gogo/constants.py` & `senpwai-2.1.8/senpwai/scrapers/gogo/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,7 +30,8 @@
     "semigo1458@undewp.com",
     "xojecog864@undewp.com",
     "lobik97135@wanbeiz.com",
 ]
 
 KEYS_REGEX = re.compile(rb"(?:container|videocontent)-(\d+)")
 ENCRYPTED_DATA_REGEX = re.compile(rb'data-value="(.+?)"')
+BASE_URL_REGEX = re.compile(r'(http[s]?://[a-zA-Z0-9\.\-]+)')
```

### Comparing `senpwai-2.1.7/senpwai/scrapers/gogo/hls.py` & `senpwai-2.1.8/senpwai/scrapers/gogo/hls.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/scrapers/gogo/main.py` & `senpwai-2.1.8/senpwai/scrapers/gogo/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from random import choice as random_choice
+import re
 from typing import Callable, cast
 
 from bs4 import BeautifulSoup, ResultSet, Tag
 from requests.cookies import RequestsCookieJar
 from senpwai.utils.scraper import (
     CLIENT,
     IBYTES_TO_MBS_DIVISOR,
     PARSER,
+    RESOURCE_MOVED_STATUS_CODES,
     AnimeMetadata,
     DomainNameError,
     ProgressFunction,
     get_new_home_url_from_readme,
     match_quality,
     sanitise_title,
 )
 from .constants import (
     AJAX_SEARCH_URL,
+    BASE_URL_REGEX,
     DUB_EXTENSION,
     FULL_SITE_NAME,
     AJAX_LOAD_EPS_URL,
     GOGO_HOME_URL,
     REGISTERED_ACCOUNT_EMAILS,
 )
 
 SESSION_COOKIES: RequestsCookieJar | None = None
-FIRST_REQUEST = False
+FIRST_REQUEST = True
 
 
 def search(keyword: str, ignore_dub=True) -> list[tuple[str, str]]:
     search_url = AJAX_SEARCH_URL + keyword
     response = CLIENT.get(search_url)
     content = response.json()["content"]
     soup = BeautifulSoup(content, PARSER)
@@ -127,33 +130,43 @@
             self.resume.wait()
             if self.cancelled:
                 return 0
             progress_update_callback(1)
         return total_size
 
 
-def get_anime_page_content(anime_page_link: str) -> bytes:
+def get_anime_page_content(anime_page_link: str) -> tuple[bytes, str]:
     global FIRST_REQUEST
+    global GOGO_HOME_URL
     if FIRST_REQUEST:
         try:
             FIRST_REQUEST = False
-            return CLIENT.get(
+            response = CLIENT.get(
                 anime_page_link,
-                exceptions_to_raise=(DomainNameError, type(KeyboardInterrupt)),
-            ).content
+                exceptions_to_raise=(DomainNameError, KeyboardInterrupt),
+            )
+            if response.status_code not in RESOURCE_MOVED_STATUS_CODES:
+                return response.content, anime_page_link
+            new_anime_page_link = response.headers.get("Location", GOGO_HOME_URL)
+            # The url in location seems to be in http instead of https but the http one doesn't work
+            if new_anime_page_link != GOGO_HOME_URL:
+                new_anime_page_link = new_anime_page_link.replace("http://", "https://")
+            match = cast(re.Match[str], BASE_URL_REGEX.search(new_anime_page_link))
+            GOGO_HOME_URL = match.group(1)
+            return get_anime_page_content(new_anime_page_link)
         except DomainNameError:
-            global GOGO_HOME_URL
             prev_home_url = GOGO_HOME_URL
             GOGO_HOME_URL = get_new_home_url_from_readme(FULL_SITE_NAME)
             return get_anime_page_content(
                 anime_page_link.replace(prev_home_url, GOGO_HOME_URL)
             )
-    return CLIENT.get(
+    response = CLIENT.get(
         anime_page_link,
-    ).content
+    )
+    return response.content, anime_page_link
 
 
 def extract_anime_metadata(anime_page_content: bytes) -> AnimeMetadata:
     soup = BeautifulSoup(anime_page_content, PARSER)
     poster_link = cast(
         str,
         cast(Tag, cast(Tag, soup.find(class_="anime_info_body_bg")).find("img"))["src"],
```

### Comparing `senpwai-2.1.7/senpwai/scrapers/pahe/constants.py` & `senpwai-2.1.8/senpwai/scrapers/pahe/constants.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/scrapers/pahe/main.py` & `senpwai-2.1.8/senpwai/scrapers/pahe/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         # This is to avoid raising DomainNameError when the something else broke instead
         global FIRST_REQUEST
         if FIRST_REQUEST:
             FIRST_REQUEST = False
             response = CLIENT.get(
                 url,
                 cookies=COOKIES,
-                exceptions_to_raise=(DomainNameError, type(KeyboardInterrupt)),
+                exceptions_to_raise=(DomainNameError, KeyboardInterrupt),
             )
         else:
             response = CLIENT.get(url, cookies=COOKIES)
         COOKIES.update(response.cookies)
     except DomainNameError:
         global PAHE_HOME_URL
         PAHE_HOME_URL = get_new_home_url_from_readme(FULL_SITE_NAME)
```

### Comparing `senpwai-2.1.7/senpwai/scrapers/test.py` & `senpwai-2.1.8/senpwai/scrapers/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,57 +64,54 @@
     raise FailedTest(msg)
 
 
 def pass_test(name: str, execution_time: float):
     conditional_print(f"Passed: {name} Test\nTook: {round(execution_time, 2)}s\n")
 
 
-def test_search(
-    anime_title: str, site: str
-) -> list[tuple[str, str]] | list[tuple[str, str, str]]:
+def test_search(anime_title: str, site: str) -> list[list[str]]:
     test_name = "Search"
     test_start(test_name)
     run_time_getter = get_run_time_later()
     if site == PAHE:
         results = pahe.search(anime_title)
     else:
         results = gogo.search(anime_title)
     rt = run_time_getter()
     if not results:
         fail_if_list_is_empty(results, test_name, "results", rt)
     pass_test(test_name, rt)
     test_name = "Parse search results"
     test_start(test_name)
     c = current_time()
-    parsed_results: list[tuple[str, str]] | list[tuple[str, str, str]] = []
+    parsed_results: list[list[str]] = []
     if site == PAHE:
         parsed_results = [
-            pahe.extract_anime_title_page_link_and_id(r)
+            list(pahe.extract_anime_title_page_link_and_id(r))
             for r in cast(list[dict[str, str]], results)
         ]
     else:
-        parsed_results = cast(list[tuple[str, str]], parsed_results)
         for title, page_link in cast(list[tuple[str, str]], results):
-            parsed_results.append((title, page_link))
+            parsed_results.append([title, page_link])
     run_timer = current_time() - c
     if not parsed_results:
         fail_test(test_name, "List of parsed results", "Empty list", run_timer)
     pass_test(test_name, run_timer)
     return parsed_results
 
 
 def get_run_time_later() -> Callable[[], float]:
     c = current_time()
     return lambda: current_time() - c
 
 
 def test_check_results_for_anime(
     anime_title: str,
-    results: list[tuple[str, str]] | list[tuple[str, str, str]],
-) -> tuple[str, str] | tuple[str, str, str] | None:
+    results: list[list[str]] | list[list[str]],
+) -> list[str] | None:
     test_name = f"Matching results to {anime_title}"
     test_start(test_name)
     run_time = get_run_time_later()
     query = sanitise_title(anime_title, True).lower()
     for r in results:
         title = r[0]
         if query == sanitise_title(title, True).lower():
@@ -126,25 +123,25 @@
         "No match found",
         run_time(),
         f"Anime title was: {anime_title}\nSearch results were: {results}",
     )
 
 
 def test_get_metadata(
-    site: str, target_result: tuple[str, str] | tuple[str, str, str]
+    site: str, target_result: list[str]
 ) -> tuple[AnimeMetadata, bytes]:
     test_name = "Get Metadata"
     test_start(test_name)
     run_time = get_run_time_later()
     page_content = b""
     if site == PAHE:
-        target_result = cast(tuple[str, str, str], target_result)
+        target_result = cast(list[str], target_result)
         metadata = pahe.get_anime_metadata(target_result[2])
     else:
-        page_content = gogo.get_anime_page_content(target_result[1])
+        page_content, target_result[1] = gogo.get_anime_page_content(target_result[1])
         metadata = gogo.extract_anime_metadata(page_content)
     pass_test(test_name, run_time())
     return metadata, page_content
 
 
 def test_get_episode_page_links(
     anime_id: str, anime_page_link: str, start_episode: int, end_episode: int
@@ -517,23 +514,20 @@
                 pass
         if default:
             conditional_print(f"Using default {target_args}: {default}")
             return default
         self.invalid_usage(f"Expected: {target_args}")
 
 
-def test_dub_available(
-    site: str, target_result: tuple[str, str] | tuple[str, str, str]
-) -> tuple[bool, str]:
+def test_dub_available(site: str, target_result: list[str]) -> tuple[bool, str]:
     test_name = "Dub availability checking"
     test_start(test_name)
     runtime_getter = get_run_time_later()
     dub_link = ""
     if site == PAHE:
-        target_result = cast(tuple[str, str, str], target_result)
         dub_available = pahe.dub_available(target_result[1], target_result[2])
     else:
         dub_available, dub_link = gogo.dub_availability_and_link(target_result[0])
     rt = runtime_getter()
     if not isinstance(dub_available, bool):
         fail_test(
             test_name,
@@ -549,15 +543,15 @@
 def run_tests(args: ArgParser):
     was_hls = False
     if args.arg_in_group_was_passed(COMMANDS):
         results = test_search(args.anime_title, args.site)
         if args.verbose:
             conditional_print(f"Search Results: {results}\n")
         target_result = cast(
-            tuple[str, str] | tuple[str, str, str],
+            list[str],
             test_check_results_for_anime(args.anime_title, results),
         )
         if args.verbose:
             conditional_print(f"Target Result: {target_result}\n")
         COMMANDS.remove("search")
         if args.arg_in_group_was_passed(COMMANDS):
             dub_available, dub_link = test_dub_available(args.site, target_result)
@@ -589,21 +583,20 @@
                         )
                     if args.sub_or_dub == "dub" and not dub_available:
                         return print(
                             "Couldn't find Dub for the anime on the specified site"
                         )
                     elif args.site == GOGO and dub_available:
                         metadata, page_content = test_get_metadata(
-                            args.site, ("", dub_link)
+                            args.site, ["", dub_link]
                         )
                         if args.verbose:
                             conditional_print("Dub metadata")
                             print_metadata(metadata)  # type: ignore
                     if args.site == PAHE:
-                        target_result = cast(tuple[str, str, str], target_result)
                         episode_page_links = test_get_episode_page_links(
                             target_result[2],
                             target_result[1],
                             args.start_eps,
                             args.end_eps,
                         )
                         if args.verbose:
```

### Comparing `senpwai-2.1.7/senpwai/senpcli/main.py` & `senpwai-2.1.8/senpwai/senpcli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 import subprocess
 import sys
 from argparse import ArgumentParser, Namespace
 from random import choice as random_choice
 from threading import Event, Lock, Thread
 from typing import Callable, cast
 from queue import Queue
@@ -106,25 +106,27 @@
     "Senpwai: Stand proud Senpcli, you are strong",
     "We are the exception",
     "As the strongest curse Jogoat fought the fraud.. .",
     "Goodbye friend",
 )
 
 
-def parse_args(args: list[str]) -> Namespace:
+def parse_args(args: list[str]) -> tuple[Namespace, ArgumentParser]:
     parser = ArgumentParser(prog=APP_NAME_LOWER, description=DESCRIPTION)
     parser.add_argument("-v", "--version", action="version", version=VERSION)
     parser.add_argument(
-        "-sd",
-        "--sub_or_dub",
-        help="Whether to download the subbed or dubbed version of the anime",
-        choices=[SUB, DUB],
-        default=SETTINGS.sub_or_dub,
+        "title", help="Title of the anime to download", nargs="?", default=None
     )
-    parser.add_argument("title", help="Title of the anime to download")
+    parser.add_argument(
+        "-c",
+        "--config",
+        help="Show config file contents and location",
+        action="store_true",
+    )
+    parser.add_argument("-u", "--update", help="Check for updates", action="store_true")
     parser.add_argument(
         "-s",
         "--site",
         help="Site to download from",
         choices=[PAHE, GOGO],
         default=SETTINGS.auto_download_site,
     )
@@ -146,14 +148,21 @@
         "-q",
         "--quality",
         help="Quality to download the anime in",
         choices=[Q_1080, Q_720, Q_480, Q_360],
         default=SETTINGS.quality,
     )
     parser.add_argument(
+        "-sd",
+        "--sub_or_dub",
+        help="Whether to download the subbed or dubbed version of the anime",
+        choices=[SUB, DUB],
+        default=SETTINGS.sub_or_dub,
+    )
+    parser.add_argument(
         "-hls",
         "--hls",
         help="Use HLS mode to download the anime (Gogo only and requires FFmpeg to be installed)",
         action="store_true",
     )
     parser.add_argument(
         "-sc",
@@ -171,15 +180,15 @@
     parser.add_argument(
         "-msd",
         "--max_simultaneous_downloads",
         type=int,
         help="Maximum number of simultaneous downloads",
         default=SETTINGS.max_simultaneous_downloads,
     )
-    return parser.parse_args(args)
+    return parser.parse_args(args), parser
 
 
 def search(title: str, site: str) -> Anime | None:
     animes = (
         [
             Anime(*pahe.extract_anime_title_page_link_and_id(r))
             for r in pahe.search(title)
@@ -288,17 +297,17 @@
     total_download_size = pahe.calculate_total_download_size(down_info)
     pbar.close()
     print(f"Total download size: {total_download_size} MB")
     return down_page_links
 
 
 def gogo_get_download_page_links(
-    start_episode: int, end_episode: int, anime_page_link: str
+    start_episode: int, end_episode: int, anime_page_content: bytes
 ) -> list[str]:
-    anime_id = gogo.extract_anime_id(gogo.get_anime_page_content(anime_page_link))
+    anime_id = gogo.extract_anime_id(anime_page_content)
     return gogo.get_download_page_links(start_episode, end_episode, anime_id)
 
 
 def gogo_calculate_total_download_size(direct_download_links: list[str]) -> None:
     pbar = tqdm(
         total=len(direct_download_links),
         desc="Calculating total download size",
@@ -502,41 +511,41 @@
     results = gogo.GetHlsSegmentsUrls().get_hls_segments_urls(
         matched_quality_links, pbar.update
     )
     pbar.close()
     return results
 
 
-def handle_pahe(parsed: Namespace, anime: Anime, anime_details: AnimeDetails):
+def handle_pahe(parsed: Namespace, anime_details: AnimeDetails):
     episode_page_links = pahe_get_episode_page_links(
-        parsed.start_episode, parsed.end_episode, cast(str, anime.id), anime.page_link
+        parsed.start_episode,
+        parsed.end_episode,
+        cast(str, anime_details.anime.id),
+        anime_details.anime.page_link,
     )
     if already_has_all_episodes(
         anime_details, parsed.start_episode, parsed.end_episode, episode_page_links
     ):
         return
-    if parsed.sub_or_dub == DUB and not pahe.dub_available(
-        anime.page_link, cast(str, anime.id)
-    ):
-        print("Dub not available for this anime")
-        return
     download_page_links = pahe_get_download_page_links(
         episode_page_links, parsed.quality, parsed.sub_or_dub
     )
     direct_download_links = pahe_get_direct_download_links(download_page_links)
     download_manager(
         direct_download_links, anime_details, False, parsed.max_simultaneous_downloads
     )
 
 
-def handle_gogo(parsed: Namespace, anime: Anime, anime_details: AnimeDetails):
+def handle_gogo(parsed: Namespace, anime_details: AnimeDetails):
     if parsed.hls:
         if install_ffmpeg_prompt():
             download_page_links = gogo_get_download_page_links(
-                parsed.start_episode, parsed.end_episode, anime.page_link
+                parsed.start_episode,
+                parsed.end_episode,
+                anime_details.anime_page_content,
             )
             if already_has_all_episodes(
                 anime_details,
                 parsed.start_episode,
                 parsed.end_episode,
                 download_page_links,
             ):
@@ -550,15 +559,15 @@
                 hls_segments_urls,
                 anime_details,
                 True,
                 parsed.max_simultaneous_downloads,
             )
     else:
         download_page_links = gogo_get_download_page_links(
-            parsed.start_episode, parsed.end_episode, anime.page_link
+            parsed.start_episode, parsed.end_episode, anime_details.anime_page_content
         )
         if already_has_all_episodes(
             anime_details, parsed.start_episode, parsed.end_episode, download_page_links
         ):
             return
         direct_download_links = gogo_get_direct_download_links(
             download_page_links, parsed.quality
@@ -603,71 +612,76 @@
 
 def handle_update_check_result(
     is_available: bool, download_url: str, file_name: str, release_notes: str
 ) -> None:
     if not is_available:
         return
     print(f"\nUpdate available!!!\n\n{release_notes}\n")
-    if IS_PIP_INSTALL:
+    if OS.is_android:
+        print(
+            'To update run:\n"pkg update -y && curl https://raw.githubusercontent.com/SenZmaKi/Senpwai/master/termux/install.sh | bash"'
+        )
+    elif IS_PIP_INSTALL:
         print('Install it by running "pip install senpwai --upgrade"')
         return
-    if SENPWAI_IS_INSTALLED:
+    elif SENPWAI_IS_INSTALLED:
         print("Install it by updating my big sister, Senpwai")
-        return
-    if OS.is_windows:
+    elif OS.is_windows:
         print("Would you like to download and install it? (y/n)")
         if input("> ").lower() == "y":
             download_and_install_update(download_url, file_name)
-        return
-    print(
-        f"A new version is available, but to install it you'll have to build from source\nThere is a guide at: {GITHUB_REPO_URL}"
-    )
+    else:
+        print(
+            f"A new version is available, but to install it you'll have to build from source\nThere is a guide at: {GITHUB_REPO_URL}"
+        )
 
 
 def start_update_check_thread() -> tuple[Thread, Queue[tuple[bool, str, str, str]]]:
     update_check_result_queue: Queue[tuple[bool, str, str, str]] = Queue()
     update_check_thread = Thread(
         target=check_for_update_thread, args=(update_check_result_queue,)
     )
     update_check_thread.start()
     return update_check_thread, update_check_result_queue
 
 
-def get_anime_and_anime_details(parsed) -> tuple[Anime, AnimeDetails] | None:
+def get_anime_details(parsed) -> AnimeDetails | None:
     anime = search(parsed.title, parsed.site)
     if anime is None:
         return None
     if parsed.sub_or_dub == DUB and parsed.site == GOGO:
         dub_available, anime.page_link = gogo.dub_availability_and_link(anime.title)
         if not dub_available:
-            print("Dub not available for this anime")
             return None
     anime_details = AnimeDetails(anime, parsed.site)
+    if parsed.sub_or_dub == DUB:
+        if not anime_details.dub_available:
+            print("Dub not available for this anime")
+            return None
+
     if parsed.start_episode == -1:
         if (
             anime_details.haved_end is not None
             and anime_details.haved_end < anime_details.metadata.episode_count
         ):
             parsed.start_episode = anime_details.haved_end + 1
         else:
             parsed.start_episode = 1
     parsed.start_episode, parsed.end_episode = validate_start_and_end_episode(
         parsed.start_episode, parsed.end_episode, anime_details.metadata.episode_count
     )
-    return anime, anime_details
+    return anime_details
 
 
-def initiate_download_pipeline(
-    parsed: Namespace, anime: Anime, anime_details: AnimeDetails
-):
+def initiate_download_pipeline(parsed: Namespace, anime_details: AnimeDetails):
     print(f"Downloading to: {anime_details.anime_folder_path}")
     if parsed.site == PAHE:
-        handle_pahe(parsed, anime, anime_details)
+        handle_pahe(parsed, anime_details)
     else:
-        handle_gogo(parsed, anime, anime_details)
+        handle_gogo(parsed, anime_details)
     if parsed.open_folder:
         open_folder(anime_details.anime_folder_path)
 
 
 def validate_args(parsed: Namespace) -> bool:
     if parsed.end_episode < parsed.start_episode and parsed.end_episode != -1:
         print("End episode cannot be less than start episode, hontoni baka ga")
@@ -685,22 +699,41 @@
     return True
 
 
 def main():
     try:
         args = sys.argv[1:]
         print(ASCII_APP_NAME)
-        parsed = parse_args(args)
+        parsed, parser = parse_args(args)
+
+        if parsed.config:
+            with open(SETTINGS.settings_json_path) as f:
+                contents = f.read()
+                print(f"{contents}\n\n{SETTINGS.settings_json_path}")
+            return
+        elif parsed.update:
+            update_check_thread, update_check_result_queue = start_update_check_thread()
+            update_check_thread.join()
+            result = update_check_result_queue.get()
+            if not result[0]:
+                print("No update available, already at latest version")
+            handle_update_check_result(*result)
+            return
+        elif parsed.title is None:
+            print(
+                f"{parser.format_usage()}senpcli: error: the following arguments are required: title"
+            )
+            return
         if not validate_args(parsed):
             return
         update_check_thread, update_check_result_queue = start_update_check_thread()
-        anime_and_anime_details = get_anime_and_anime_details(parsed)
-        if anime_and_anime_details is None:
+        anime_details = get_anime_details(parsed)
+        if anime_details is None:
             return
-        initiate_download_pipeline(parsed, *anime_and_anime_details)
+        initiate_download_pipeline(parsed, anime_details)
         update_check_thread.join()
         handle_update_check_result(*update_check_result_queue.get())
 
     except KeyboardInterrupt:
         print("\n\nAborted")
```

### Comparing `senpwai-2.1.7/senpwai/utils/classes.py` & `senpwai-2.1.8/senpwai/utils/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,15 +254,15 @@
         self.haved_episodes: list[int] = []
         (
             self.haved_start,
             self.haved_end,
             self.haved_count,
         ) = self.get_start_end_and_count_of_haved_episodes()
         self.dub_available, self.dub_page_link = self.get_dub_availablilty_status()
-        self.metadata = self.get_metadata()
+        self.metadata, self.anime_page_content = self.get_metadata()
         self.episode_count = self.metadata.episode_count
         self.quality = SETTINGS.quality
         self.sub_or_dub = SETTINGS.sub_or_dub
         self.ddls_or_segs_urls: list[str] | list[list[str]] = []
         self.download_info: list[str] = []
         self.total_download_size: int = 0
         self.lacked_episode_numbers: list[int] = []
@@ -375,14 +375,15 @@
                 self.anime.page_link, cast(str, self.anime.id)
             )
             link = self.anime.page_link
         else:
             dub_available, link = gogo.dub_availability_and_link(self.anime.title)
         return dub_available, link
 
-    def get_metadata(self) -> AnimeMetadata:
+    def get_metadata(self) -> tuple[AnimeMetadata, bytes]:
         if self.site == PAHE:
             metadata = pahe.get_anime_metadata(cast(str, self.anime.id))
+            page_content = b""
         else:
-            page_content = gogo.get_anime_page_content(self.anime.page_link)
+            page_content, self.anime.page_link = gogo.get_anime_page_content(self.anime.page_link)
             metadata = gogo.extract_anime_metadata(page_content)
-        return metadata
+        return metadata, page_content
```

### Comparing `senpwai-2.1.7/senpwai/utils/scraper.py` & `senpwai-2.1.8/senpwai/utils/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import re
 import subprocess
-import sys
 from base64 import b64decode
 from string import ascii_letters, digits, printable
 from threading import Event
 from time import sleep as timesleep
-from typing import  TypeVar, Callable, Iterator, cast
+from typing import TypeVar, Callable, Iterator, cast
 from random import choice as random_choice
 from webbrowser import open_new_tab
 
 import requests
 
 from senpwai.utils.static import log_exception, try_deleting, OS
 
@@ -133,15 +132,15 @@
         headers: dict | None,
         cookies={},
         stream=False,
         data: dict | bytes | None = None,
         json: dict | None = None,
         allow_redirects=False,
         timeout: int | None = None,
-        exceptions_to_ignore: tuple[type[Exception], ...] = (type(KeyboardInterrupt),),
+        exceptions_to_ignore: tuple[type[BaseException], ...] = (KeyboardInterrupt,),
     ) -> requests.Response:
         if not headers:
             headers = self.headers
         if method == "GET":
 
             def callback():
                 return requests.get(
@@ -169,15 +168,15 @@
     def get(
         self,
         url: str,
         stream=False,
         headers: dict | None = None,
         timeout: int | None = None,
         cookies={},
-        exceptions_to_raise: tuple[type[Exception], ...] = (type(KeyboardInterrupt),),
+        exceptions_to_raise: tuple[type[BaseException], ...] = (KeyboardInterrupt,),
     ) -> requests.Response:
         return self.make_request(
             "GET",
             url,
             headers,
             stream=stream,
             timeout=timeout,
@@ -189,15 +188,15 @@
         self,
         url: str,
         data: dict | bytes | None = None,
         json: dict | None = None,
         headers: dict | None = None,
         cookies={},
         allow_redirects=False,
-        exceptions_to_ignore: tuple[type[Exception], ...] = (type(KeyboardInterrupt),),
+        exceptions_to_ignore: tuple[type[BaseException], ...] = (KeyboardInterrupt,),
     ) -> requests.Response:
         return self.make_request(
             "POST",
             url,
             headers,
             data=data,
             json=json,
@@ -205,15 +204,15 @@
             allow_redirects=allow_redirects,
             exceptions_to_ignore=exceptions_to_ignore,
         )
 
     def network_error_retry_wrapper(
         self,
         callback: Callable[[], T],
-        exceptions_to_ignore: tuple[type[Exception], ...] = (type(KeyboardInterrupt),),
+        exceptions_to_ignore: tuple[type[BaseException], ...] = (KeyboardInterrupt,),
     ) -> T:
         while True:
             try:
                 return callback()
             except requests.exceptions.RequestException as e:
                 if isinstance(e, KeyboardInterrupt):
                     raise
@@ -283,15 +282,15 @@
         closest = quality
     return closest[1]
 
 
 def run_process_silently(args: list[str]) -> subprocess.CompletedProcess[bytes]:
     if OS.is_windows:
         return subprocess.run(args, creationflags=subprocess.CREATE_NO_WINDOW)
-    return subprocess.run(args)
+    return subprocess.run(args, capture_output=True)
 
 
 def run_process_in_new_console(
     args: list[str] | str,
 ) -> subprocess.CompletedProcess[bytes]:
     if OS.is_windows:
         return subprocess.run(args, creationflags=subprocess.CREATE_NEW_CONSOLE)
@@ -307,27 +306,40 @@
             pass
         # Incase the installation was scuffed
         if ffmpeg_is_installed():
             return True
         else:
             open_new_tab(FFMPEG_WINDOWS_INSTALLATION_GUIDE)
             return False
-    elif sys.platform == "linux":
+    elif OS.is_linux:
         try:
             run_process_in_new_console(
                 "sudo apt-get update && sudo apt-get install ffmpeg"
             )
         except Exception as _:
             pass
         if ffmpeg_is_installed():
             return True
         else:
             open_new_tab(FFMPEG_LINUX_INSTALLATION_GUIDE)
             return False
 
+    elif OS.is_android:
+        try:
+            run_process_in_new_console("pkg update -y && pkg install ffmpeg -y")
+        except Exception:
+            pass
+        if ffmpeg_is_installed():
+            return True
+        else:
+            print(
+                'Try running "pkg update && pkg install ffmpeg", if it doesn\'t work look up a guide on the internet'
+            )
+            return False
+
     else:
         try:
             run_process_in_new_console("brew install ffmpeg")
         except Exception as _:
             pass
         if ffmpeg_is_installed():
             return True
```

### Comparing `senpwai-2.1.7/senpwai/utils/static.py` & `senpwai-2.1.8/senpwai/utils/static.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 from random import choice as random_choice
 from subprocess import Popen
 from types import TracebackType
 import logging
 
 APP_NAME = "Senpwai"
 APP_NAME_LOWER = "senpwai"
-VERSION = "2.1.7"
+VERSION = "2.1.8"
 DESCRIPTION = "A desktop app for tracking and batch downloading anime"
 
 IS_PIP_INSTALL = False
 APP_EXE_PATH = ""
 
 
 class OS:
-    is_windows = sys.platform == "win32"
-    is_linux = sys.platform == "linux"
-    is_mac = sys.platform == "darwin"
+    is_android = "ANDROID_ROOT" in os.environ 
+    is_windows = sys.platform == "win32" and not is_android
+    is_linux = sys.platform == "linux" and not is_android
+    is_mac = sys.platform == "darwin" and not is_android
 
 
 if getattr(sys, "frozen", False):
     # C:\Users\PC\AppData\Local\Programs\Senpwai
     ROOT_DIRECTORY = os.path.dirname(sys.executable)
     APP_EXE_PATH = sys.executable
     IS_EXECUTABLE = True
```

### Comparing `senpwai-2.1.7/senpwai/utils/widgets.py` & `senpwai-2.1.8/senpwai/utils/widgets.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/windows/about.py` & `senpwai-2.1.8/senpwai/windows/about.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/windows/abstracts.py` & `senpwai-2.1.8/senpwai/windows/abstracts.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/windows/chosen_anime.py` & `senpwai-2.1.8/senpwai/windows/chosen_anime.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/windows/download.py` & `senpwai-2.1.8/senpwai/windows/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -996,16 +996,15 @@
     ):
         super().__init__(download_window)
         self.anime_details = anime_details
         self.hls_finished.connect(callback)
         self.finished.connect(callback)
 
     def run(self):
-        page_content = gogo.get_anime_page_content(self.anime_details.anime.page_link)
-        anime_id = gogo.extract_anime_id(page_content)
+        anime_id = gogo.extract_anime_id(self.anime_details.anime_page_content)
         download_page_links = gogo.get_download_page_links(
             self.anime_details.lacked_episode_numbers[0],
             self.anime_details.lacked_episode_numbers[-1],
             anime_id,
         )
         download_page_links = lacked_episodes(
             self.anime_details.lacked_episode_numbers, download_page_links
```

### Comparing `senpwai-2.1.7/senpwai/windows/main.py` & `senpwai-2.1.8/senpwai/windows/main.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/windows/misc.py` & `senpwai-2.1.8/senpwai/windows/misc.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/windows/search.py` & `senpwai-2.1.8/senpwai/windows/search.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/senpwai/windows/settings.py` & `senpwai-2.1.8/senpwai/windows/settings.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.7/PKG-INFO` & `senpwai-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senpwai
-Version: 2.1.7
+Version: 2.1.8
 Summary: A desktop app for tracking and batch downloading anime
 Home-page: https://github.com/SenZmaKi/Senpwai
 License: GPL v3
 Keywords: anime,app,cli,desktop app,anime downloader,anime cli,anime app,anime tracker,batch anime downloader,bulk anime  downloader,anime desktop app,anime tracker app
 Author: SenZmaKi
 Author-email: senzmaki@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -50,24 +50,31 @@
   <a href="#faq">FAQ</a> •
   <a href="#links">Links</a>
 </p>
 
 <img align="center" src="https://raw.githubusercontent.com/SenZmaKi/Senpwai/master/.github/images/one-piece.png" alt="one-piece-screenshot">
 
 ## Installation
+
 - **Cross-platform (Linux, Mac, Windows 10/11)**
 
 Needs [Python 3.11](https://www.python.org/downloads/release/python-3111) installed.
+
 ```bash
 pip install senpwai
 ```
+
 - **Windows 10/11**
 
 Download [the setup](https://github.com/SenZmaKi/Senpwai/releases/latest/download/Senpwai-setup.exe) then run it.
 
+- **Android**
+
+Check [Senpcli](https://github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md)
+
 - **Other**
 
 [Build from source](#building-from-source).
 
 ## Features
 
 - Download any anime from [Animepahe](https://animepahe.ru) or [Gogoanime](https://anitaku.to).
@@ -91,15 +98,14 @@
 
 1. **Set everything up.**
 
 ```
 git clone https://github.com/SenZmaKi/Senpwai --depth 1 && cd Senpwai && pip install -r dev-requirements.txt && poetry install
 ```
 
-
 2. **Build the app into an executable.**
 
 ```
 poetry run poe build_senpwai_exe
 ```
 
 - The executable will be built in `Senpwai\build\Senpwai`
@@ -113,14 +119,15 @@
 ## Support
 
 - You can support the development of Senpwai through donations on [GitHub Sponsors](https://github.com/sponsors/SenZmaKi) or [Patreon](https://patreon.com/Senpwai).
 - You can also leave a star on the github for more weebs to know about it.
 - Senpwai is open to pull requests, so if you have ideas for improvements, feel free to contribute!
 
 ## Sponsors
+
 <p>
 <a href="https://github.com/Adam1400"><img src="https://github.com/Adam1400.png" width="80px" alt="Adam1400"/></a>&nbsp;&nbsp;<a href="https://github.com/KeithBoehler"><img src="https://github.com/KeithBoehler.png" width="80px" alt="KeithBoehler" /></a>
 </p>
 
 ## FAQ
 
 <details> <summary> Why did you make this? </summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: senpwai Version: 2.1.7 Summary: A desktop app for
+Metadata-Version: 2.1 Name: senpwai Version: 2.1.8 Summary: A desktop app for
 tracking and batch downloading anime Home-page: https://github.com/SenZmaKi/
 Senpwai License: GPL v3 Keywords: anime,app,cli,desktop app,anime
 downloader,anime cli,anime app,anime tracker,batch anime downloader,bulk anime
 downloader,anime desktop app,anime tracker app Author: SenZmaKi Author-email:
 senzmaki@gmail.com Requires-Python: >=3.11,<4.0 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
@@ -23,41 +23,42 @@
               _[_t_e_s_t_-_w_o_r_k_f_l_o_w_-_s_t_a_t_u_s_-_b_a_d_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]/a>
 _I_n_s_t_a_l_l_a_t_i_o_n â¢ _F_e_a_t_u_r_e_s â¢ _C_L_I â¢ _B_u_i_l_d_i_n_g_ _f_r_o_m_ _s_o_u_r_c_e â¢ _S_u_p_p_o_r_t â¢ _F_A_Q
                                    â¢ _L_i_n_k_s
 [one-piece-screenshot]## Installation - **Cross-platform (Linux, Mac, Windows
 10/11)** Needs [Python 3.11](https://www.python.org/downloads/release/python-
 3111) installed. ```bash pip install senpwai ``` - **Windows 10/11** Download
 [the setup](https://github.com/SenZmaKi/Senpwai/releases/latest/download/
-Senpwai-setup.exe) then run it. - **Other** [Build from source](#building-from-
-source). ## Features - Download any anime from [Animepahe](https://
-animepahe.ru) or [Gogoanime](https://anitaku.to). - Keep track of an anime and
-automatically download new episodes when they release. - Download a complete
-season or episodes within a range (e.g., 69-420). - Choose between video
-qualities: 360p, 480p (Gogoanime only), 720p, or 1080p. - Download in sub or
-dub (if available) depending on the user's preference. - Automatically detects
-episodes you already have and avoids re-downloading them. - Robust and graceful
-download error management. - GUI and [CLI](https://github.com/SenZmaKi/Senpwai/
-blob/master/docs/senpcli-guide.md). ## CLI [Senpcli](https://github.com/
-SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md) is a minimalist and
-lightweight CLI alternative for Senpwai. Senpwai is already efficient and
-lightweight, Senpcli basically strips off the GUI while maintaining most of the
-basic functionality. ## Building from Source Ensure you have [Python 3.11]
-(https://www.python.org/downloads/release/python-3111) and [Git](https://
-github.com/git-guides/install-git) installed. Open a terminal and run the
-following commands. 1. **Set everything up.** ``` git clone https://github.com/
-SenZmaKi/Senpwai --depth 1 && cd Senpwai && pip install -r dev-requirements.txt
-&& poetry install ``` 2. **Build the app into an executable.** ``` poetry run
-poe build_senpwai_exe ``` - The executable will be built in
-`Senpwai\build\Senpwai` 3. **Alternatively you can instead run the app directly
-via Python.** ``` poetry run senpwai ``` ## Support - You can support the
-development of Senpwai through donations on [GitHub Sponsors](https://
-github.com/sponsors/SenZmaKi) or [Patreon](https://patreon.com/Senpwai). - You
-can also leave a star on the github for more weebs to know about it. - Senpwai
-is open to pull requests, so if you have ideas for improvements, feel free to
-contribute! ## Sponsors
+Senpwai-setup.exe) then run it. - **Android** Check [Senpcli](https://
+github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md) - **Other**
+[Build from source](#building-from-source). ## Features - Download any anime
+from [Animepahe](https://animepahe.ru) or [Gogoanime](https://anitaku.to). -
+Keep track of an anime and automatically download new episodes when they
+release. - Download a complete season or episodes within a range (e.g., 69-
+420). - Choose between video qualities: 360p, 480p (Gogoanime only), 720p, or
+1080p. - Download in sub or dub (if available) depending on the user's
+preference. - Automatically detects episodes you already have and avoids re-
+downloading them. - Robust and graceful download error management. - GUI and
+[CLI](https://github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md).
+## CLI [Senpcli](https://github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-
+guide.md) is a minimalist and lightweight CLI alternative for Senpwai. Senpwai
+is already efficient and lightweight, Senpcli basically strips off the GUI
+while maintaining most of the basic functionality. ## Building from Source
+Ensure you have [Python 3.11](https://www.python.org/downloads/release/python-
+3111) and [Git](https://github.com/git-guides/install-git) installed. Open a
+terminal and run the following commands. 1. **Set everything up.** ``` git
+clone https://github.com/SenZmaKi/Senpwai --depth 1 && cd Senpwai && pip
+install -r dev-requirements.txt && poetry install ``` 2. **Build the app into
+an executable.** ``` poetry run poe build_senpwai_exe ``` - The executable will
+be built in `Senpwai\build\Senpwai` 3. **Alternatively you can instead run the
+app directly via Python.** ``` poetry run senpwai ``` ## Support - You can
+support the development of Senpwai through donations on [GitHub Sponsors]
+(https://github.com/sponsors/SenZmaKi) or [Patreon](https://patreon.com/
+Senpwai). - You can also leave a star on the github for more weebs to know
+about it. - Senpwai is open to pull requests, so if you have ideas for
+improvements, feel free to contribute! ## Sponsors
 _[_A_d_a_m_1_4_0_0_]  _[_K_e_i_t_h_B_o_e_h_l_e_r_]
 ## FAQ Why did you make this? I couldn't afford wifi so I used my college wifi
 to download anime after class but batch downloading from streaming sites is a
 pain in the ass, you have to click billions of links just to download one
 episode, so I made Senpwai to help me and possibly others that face a similar
 problem. What is HLS mode? HLS mode attempts to fix the unstability of
 Gogoanime normal mode. In HLS mode Gogoanime downloads are guaranteed to work,
```

