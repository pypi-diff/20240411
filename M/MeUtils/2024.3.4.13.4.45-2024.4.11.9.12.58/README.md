# Comparing `tmp/MeUtils-2024.3.4.13.4.45.tar.gz` & `tmp/MeUtils-2024.4.11.9.12.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeUtils-2024.3.4.13.4.45.tar", last modified: Mon Mar  4 05:04:47 2024, max compression
+gzip compressed data, was "MeUtils-2024.4.11.9.12.58.tar", last modified: Thu Apr 11 01:13:00 2024, max compression
```

## Comparing `MeUtils-2024.3.4.13.4.45.tar` & `MeUtils-2024.4.11.9.12.58.tar`

### file list

```diff
@@ -1,534 +1,542 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.532202 MeUtils-2024.3.4.13.4.45/
--rw-r--r--   0 betterme   (501) staff       (20)    10244 2023-11-30 00:39:46.000000 MeUtils-2024.3.4.13.4.45/.DS_Store
--rw-r--r--   0 betterme   (501) staff       (20)     1204 2023-05-22 06:35:12.000000 MeUtils-2024.3.4.13.4.45/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      331 2023-11-29 08:20:55.000000 MeUtils-2024.3.4.13.4.45/MANIFEST.in
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.495831 MeUtils-2024.3.4.13.4.45/MeUtils.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     5959 2024-03-04 05:04:46.000000 MeUtils-2024.3.4.13.4.45/MeUtils.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)    15583 2024-03-04 05:04:47.000000 MeUtils-2024.3.4.13.4.45/MeUtils.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2024-03-04 05:04:46.000000 MeUtils-2024.3.4.13.4.45/MeUtils.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)      312 2024-03-04 05:04:46.000000 MeUtils-2024.3.4.13.4.45/MeUtils.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1186 2024-03-04 05:04:46.000000 MeUtils-2024.3.4.13.4.45/MeUtils.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)       22 2024-03-04 05:04:46.000000 MeUtils-2024.3.4.13.4.45/MeUtils.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)     5959 2024-03-04 05:04:47.500761 MeUtils-2024.3.4.13.4.45/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2024.3.4.13.4.45/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-07-20 08:15:27.000000 MeUtils-2024.3.4.13.4.45/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.268196 MeUtils-2024.3.4.13.4.45/apps/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2024-01-18 04:10:04.000000 MeUtils-2024.3.4.13.4.45/apps/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      462 2024-01-18 04:20:39.000000 MeUtils-2024.3.4.13.4.45/apps/spider.py
--rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/clear_githis.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      308 2023-08-11 00:53:48.000000 MeUtils-2024.3.4.13.4.45/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.275029 MeUtils-2024.3.4.13.4.45/meutils/
--rw-r--r--   0 betterme   (501) staff       (20)      348 2023-08-17 00:48:50.000000 MeUtils-2024.3.4.13.4.45/meutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2024.3.4.13.4.45/meutils/_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.284413 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 05:51:24.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-11-21 10:11:16.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/adjusted_audio1.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.286706 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/asr/
--rw-r--r--   0 betterme   (501) staff       (20)      825 2023-11-28 10:28:28.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/asr/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3121 2023-11-28 02:24:07.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/asr/fast_asr.py
--rw-r--r--   0 betterme   (501) staff       (20)      514 2023-12-11 10:44:07.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/asr/openai_asr.py
--rw-r--r--   0 betterme   (501) staff       (20)      823 2023-11-28 02:20:46.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/asr/subtitle.srt
--rw-r--r--   0 betterme   (501) staff       (20)     7251 2023-12-01 04:06:03.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/asr/xunfei_asr.py
--rw-r--r--   0 betterme   (501) staff       (20)     1226 2023-11-21 06:01:47.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/asr.py
--rw-r--r--   0 betterme   (501) staff       (20)  2879556 2023-11-27 03:16:45.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/demo.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)     3790 2023-11-24 08:13:08.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/example.srt
--rw-r--r--   0 betterme   (501) staff       (20)     2968 2023-11-21 11:25:44.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/fast_asr.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-11-21 12:22:26.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/new.srt
--rw-r--r--   0 betterme   (501) staff       (20)     9087 2023-11-21 11:36:58.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/subtitles.srt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.288771 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/tts/
--rw-r--r--   0 betterme   (501) staff       (20)     5086 2023-12-26 09:31:08.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/tts/EdgeTTS.py
--rw-r--r--   0 betterme   (501) staff       (20)      405 2023-12-26 05:42:13.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/tts/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-11-21 12:22:26.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/tts/new.srt
--rw-r--r--   0 betterme   (501) staff       (20)     1886 2023-12-26 08:56:03.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/tts/openai_tts.py
--rw-r--r--   0 betterme   (501) staff       (20)     4597 2023-11-03 07:18:48.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/tts/tts_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     2494 2023-11-21 10:39:01.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/tts.py
--rw-r--r--   0 betterme   (501) staff       (20)     1214 2023-11-28 10:28:28.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1898 2023-11-22 09:47:51.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_audio/视频合并.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.300212 MeUtils-2024.3.4.13.4.45/meutils/ai_cv/
--rwxr-xr-x   0 betterme   (501) staff       (20)    20960 2023-08-31 09:02:20.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_cv/1.jpg
--rwxr-xr-x   0 betterme   (501) staff       (20)     8285 2023-08-31 09:27:34.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_cv/197.jpg
--rwxr-xr-x   0 betterme   (501) staff       (20)    27190 2023-08-31 09:02:20.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_cv/2.jpg
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:11:56.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_cv/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2684 2023-09-01 11:12:26.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_cv/doc_prompt.py
--rw-r--r--   0 betterme   (501) staff       (20)    49873 2023-09-25 03:07:24.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_cv/img.png
--rw-r--r--   0 betterme   (501) staff       (20)   335396 2023-08-25 05:34:53.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_cv/invoice.jpg
--rw-r--r--   0 betterme   (501) staff       (20)     1152 2023-11-02 10:12:40.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_cv/latex_ocr.py
--rw-r--r--   0 betterme   (501) staff       (20)      682 2023-10-24 01:58:01.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_cv/ocr.py
--rw-r--r--   0 betterme   (501) staff       (20)     2401 2023-09-25 04:18:07.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_cv/ocr_api.py
--rw-r--r--   0 betterme   (501) staff       (20)   159229 2023-10-24 01:56:18.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_cv/tbl.png
--rw-r--r--   0 betterme   (501) staff       (20)    24809 2023-10-27 03:01:01.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_cv/test.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.306234 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/
--rw-r--r--   0 betterme   (501) staff       (20)     6927 2023-06-30 13:22:13.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/SplitSentence.py
--rw-r--r--   0 betterme   (501) staff       (20)    13489 2023-05-21 05:19:20.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/Untitled-1(1).py
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2295 2023-04-10 08:57:58.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/_lda.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.307262 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/_textsplitter/
--rw-r--r--   0 betterme   (501) staff       (20)      287 2023-05-22 01:52:50.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/_textsplitter/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-05-21 05:10:54.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2282 2023-05-21 05:27:40.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/_textsplitter/text_split.py
--rw-r--r--   0 betterme   (501) staff       (20)      650 2023-12-12 02:19:51.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      329 2023-10-26 01:47:40.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/epub翻译.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-06-06 06:44:28.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/lda.py
--rw-r--r--   0 betterme   (501) staff       (20)     2560 2023-07-25 08:50:49.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/ner.py
--rw-r--r--   0 betterme   (501) staff       (20)     1019 2023-12-12 03:58:07.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/text_transformer.py
--rw-r--r--   0 betterme   (501) staff       (20)     2111 2023-06-30 13:18:15.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     3542 2023-06-05 05:29:27.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.310563 MeUtils-2024.3.4.13.4.45/meutils/ai_video/
--rw-r--r--   0 betterme   (501) staff       (20)      254 2020-12-15 11:24:42.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_video/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1143 2023-11-20 10:32:55.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_video/avmerge.py
--rw-r--r--   0 betterme   (501) staff       (20)      881 2023-11-22 09:38:35.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_video/avmerge_.py
--rw-r--r--   0 betterme   (501) staff       (20)     3470 2023-11-24 07:46:38.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_video/scene_detect.py
--rw-r--r--   0 betterme   (501) staff       (20)     1760 2023-11-24 07:57:00.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_video/test.py
--rw-r--r--   0 betterme   (501) staff       (20)     1727 2023-11-24 08:38:38.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_video/video.py
--rw-r--r--   0 betterme   (501) staff       (20)      902 2023-11-17 08:12:46.000000 MeUtils-2024.3.4.13.4.45/meutils/ai_video/xx.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.315416 MeUtils-2024.3.4.13.4.45/meutils/ann/
--rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/README_gensim.md
--rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/ann.py
--rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/ann_faiss.py
--rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/ann_gensim.py
--rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-05-16 06:47:06.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/ann_inmemory.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-05-19 06:06:57.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/ann_qdrant.py
--rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/ann_service.py
--rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/ann_v1.py
--rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.316049 MeUtils-2024.3.4.13.4.45/meutils/ann/examples/
--rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/examples/client.py
--rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/examples/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/milvus.py
--rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/ann/shake_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.317434 MeUtils-2024.3.4.13.4.45/meutils/api/
--rw-r--r--   0 betterme   (501) staff       (20)      344 2023-12-04 08:54:59.000000 MeUtils-2024.3.4.13.4.45/meutils/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3657 2024-02-05 02:46:19.000000 MeUtils-2024.3.4.13.4.45/meutils/api/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      735 2024-03-01 09:00:39.000000 MeUtils-2024.3.4.13.4.45/meutils/api/deeplx.py
--rw-r--r--   0 betterme   (501) staff       (20)   421916 2023-12-07 02:25:29.000000 MeUtils-2024.3.4.13.4.45/meutils/api/qr.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.319741 MeUtils-2024.3.4.13.4.45/meutils/async_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      284 2023-08-28 05:10:12.000000 MeUtils-2024.3.4.13.4.45/meutils/async_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1523 2024-02-29 11:04:14.000000 MeUtils-2024.3.4.13.4.45/meutils/async_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     8285 2024-01-20 10:30:04.000000 MeUtils-2024.3.4.13.4.45/meutils/cache_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.329194 MeUtils-2024.3.4.13.4.45/meutils/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      784 2024-01-05 03:29:34.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/__test.sh
--rw-r--r--   0 betterme   (501) staff       (20)     4511 2024-01-03 02:50:38.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/browser.py
--rw-r--r--   0 betterme   (501) staff       (20)     3212 2024-02-21 06:58:51.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      319 2024-01-17 03:02:30.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/cloudflare.py
--rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/cron.py
--rw-r--r--   0 betterme   (501) staff       (20)      180 2024-01-03 02:23:43.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek.txt
--rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:24:07.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_13003330042.json
--rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:11:32.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_13003872192.json
--rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:24:42.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_13852263862.json
--rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:24:28.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_13913898681.json
--rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:24:21.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_13962978617.json
--rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:24:16.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_15251801790.json
--rw-r--r--   0 betterme   (501) staff       (20)     2596 2024-01-03 02:24:37.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_15720826383.json
--rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:24:12.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_18395563611.json
--rw-r--r--   0 betterme   (501) staff       (20)     2617 2024-01-03 02:24:32.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_313303303@qq.com.json
--rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/gunicorn.conf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2032 2024-01-05 03:30:04.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/kimi_state.json
--rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      731 2023-08-30 03:57:39.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/nesc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1757 2023-12-27 00:56:08.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/notice.py
--rw-r--r--   0 betterme   (501) staff       (20)     2411 2024-02-27 08:32:53.000000 MeUtils-2024.3.4.13.4.45/meutils/clis/server.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.330989 MeUtils-2024.3.4.13.4.45/meutils/cmds/
--rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/cmds/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/cmds/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/cmds/cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/cmds/hdfs_cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/cmds/subprocess_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.331554 MeUtils-2024.3.4.13.4.45/meutils/coding/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/coding/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/coding/find132.py
--rw-r--r--   0 betterme   (501) staff       (20)    15337 2024-02-06 13:51:23.000000 MeUtils-2024.3.4.13.4.45/meutils/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.332100 MeUtils-2024.3.4.13.4.45/meutils/comp_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/comp_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/comp_utils/reverse_metric.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.343903 MeUtils-2024.3.4.13.4.45/meutils/data/
--rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2024.3.4.13.4.45/meutils/data/SimHei.ttf
--rw-r--r--   0 betterme   (501) staff       (20)       19 2024-03-04 05:04:45.000000 MeUtils-2024.3.4.13.4.45/meutils/data/VERSION
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/data/_FLAG
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/data/_SUCCESS
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/data/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/data/coordinate.py
--rw-r--r--   0 betterme   (501) staff       (20)     2497 2023-09-07 05:50:11.000000 MeUtils-2024.3.4.13.4.45/meutils/date_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.348773 MeUtils-2024.3.4.13.4.45/meutils/db/
--rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/db/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     7637 2024-01-05 00:39:21.000000 MeUtils-2024.3.4.13.4.45/meutils/db/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/db/mongo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/db/neo4j.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.356931 MeUtils-2024.3.4.13.4.45/meutils/decorators/
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1681 2023-05-25 09:49:50.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/__ai.py
--rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2951 2023-12-28 05:10:23.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/cache.py
--rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/catch.py
--rw-r--r--   0 betterme   (501) staff       (20)    10299 2024-01-24 09:24:12.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     1251 2024-01-16 12:50:20.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/contextmanagers.py
--rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/decorator.py
--rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/decorator_demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      710 2023-12-26 09:35:03.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1355 2024-01-09 00:35:44.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/fastapi_decorator.py
--rw-r--r--   0 betterme   (501) staff       (20)     3634 2023-08-24 02:55:32.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)     2976 2024-02-27 09:07:28.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/retry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     2664 2023-11-06 02:17:41.000000 MeUtils-2024.3.4.13.4.45/meutils/decorators/schedulers.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.357332 MeUtils-2024.3.4.13.4.45/meutils/dependencies/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-02 08:27:24.000000 MeUtils-2024.3.4.13.4.45/meutils/dependencies/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3640 2023-05-15 10:32:24.000000 MeUtils-2024.3.4.13.4.45/meutils/dist_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.359173 MeUtils-2024.3.4.13.4.45/meutils/docarray_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2024.3.4.13.4.45/meutils/docarray_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2024.3.4.13.4.45/meutils/docarray_utils/demo_es.py
--rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2024.3.4.13.4.45/meutils/docarray_utils/demo_hnsw.py
--rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2024.3.4.13.4.45/meutils/docarray_utils/in_memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2024.3.4.13.4.45/meutils/docarray_utils/改造下hnsw.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.360268 MeUtils-2024.3.4.13.4.45/meutils/easy_search/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/easy_search/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2425 2023-08-02 06:36:30.000000 MeUtils-2024.3.4.13.4.45/meutils/easy_search/es.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.363321 MeUtils-2024.3.4.13.4.45/meutils/fileparser/
--rw-r--r--   0 betterme   (501) staff       (20)     1975 2023-05-30 05:34:49.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/PDF抽取.py
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-18 08:38:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      284 2023-07-12 04:10:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2792 2023-08-16 04:33:39.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.365397 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/
--rw-r--r--   0 betterme   (501) staff       (20)      223 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      803 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/__main__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2122 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/filetype.py
--rw-r--r--   0 betterme   (501) staff       (20)     2947 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/helpers.py
--rw-r--r--   0 betterme   (501) staff       (20)     3288 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/match.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.369085 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/
--rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      498 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/application.py
--rw-r--r--   0 betterme   (501) staff       (20)    17006 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/archive.py
--rw-r--r--   0 betterme   (501) staff       (20)     4960 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/audio.py
--rw-r--r--   0 betterme   (501) staff       (20)      647 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     7513 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/document.py
--rw-r--r--   0 betterme   (501) staff       (20)     2924 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/font.py
--rw-r--r--   0 betterme   (501) staff       (20)     9130 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/image.py
--rw-r--r--   0 betterme   (501) staff       (20)      958 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/isobmff.py
--rw-r--r--   0 betterme   (501) staff       (20)     5371 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/video.py
--rw-r--r--   0 betterme   (501) staff       (20)     2089 2023-05-18 08:40:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      285 2023-07-15 07:06:30.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype.py
--rw-r--r--   0 betterme   (501) staff       (20)      639 2023-08-10 05:04:53.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4037 2023-07-17 10:15:11.000000 MeUtils-2024.3.4.13.4.45/meutils/fileparser/表格抽取.py
--rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2024.3.4.13.4.45/meutils/hash_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/import_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.370241 MeUtils-2024.3.4.13.4.45/meutils/init/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2024.3.4.13.4.45/meutils/init/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1588 2023-08-07 08:26:31.000000 MeUtils-2024.3.4.13.4.45/meutils/init/evn.py
--rw-r--r--   0 betterme   (501) staff       (20)    12884 2023-07-06 01:18:39.000000 MeUtils-2024.3.4.13.4.45/meutils/init/oo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.374780 MeUtils-2024.3.4.13.4.45/meutils/io/
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2024.3.4.13.4.45/meutils/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/io/file.py
--rw-r--r--   0 betterme   (501) staff       (20)     2574 2023-11-21 02:11:46.000000 MeUtils-2024.3.4.13.4.45/meutils/io/image.py
--rw-r--r--   0 betterme   (501) staff       (20)    49873 2023-09-25 03:07:24.000000 MeUtils-2024.3.4.13.4.45/meutils/io/img.png
--rw-r--r--   0 betterme   (501) staff       (20)     1274 2024-02-05 09:39:04.000000 MeUtils-2024.3.4.13.4.45/meutils/io/minio_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     8605 2023-06-26 01:26:21.000000 MeUtils-2024.3.4.13.4.45/meutils/io/tf_io.py
--rw-r--r--   0 betterme   (501) staff       (20)        2 2024-01-03 06:54:16.000000 MeUtils-2024.3.4.13.4.45/meutils/io/x.yml
--rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/jinja_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.377182 MeUtils-2024.3.4.13.4.45/meutils/logging/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-15 06:07:38.000000 MeUtils-2024.3.4.13.4.45/meutils/logging/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      701 2023-08-21 08:23:51.000000 MeUtils-2024.3.4.13.4.45/meutils/logging/handlers.py
--rw-r--r--   0 betterme   (501) staff       (20)     2937 2023-08-15 01:04:50.000000 MeUtils-2024.3.4.13.4.45/meutils/logging/log_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6183 2024-02-08 00:37:38.000000 MeUtils-2024.3.4.13.4.45/meutils/logging/logger.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.385008 MeUtils-2024.3.4.13.4.45/meutils/notice/
--rw-r--r--   0 betterme   (501) staff       (20)      248 2023-08-30 03:57:39.000000 MeUtils-2024.3.4.13.4.45/meutils/notice/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-10-16 09:04:49.000000 MeUtils-2024.3.4.13.4.45/meutils/notice/emails.py
--rw-r--r--   0 betterme   (501) staff       (20)     2390 2024-02-06 10:38:33.000000 MeUtils-2024.3.4.13.4.45/meutils/notice/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/notice/file_post.py
--rw-r--r--   0 betterme   (501) staff       (20)     7836 2023-09-27 09:38:07.000000 MeUtils-2024.3.4.13.4.45/meutils/notice/img.png
--rw-r--r--   0 betterme   (501) staff       (20)     7331 2023-09-12 01:53:53.000000 MeUtils-2024.3.4.13.4.45/meutils/notice/load_emailfile - 副本.py
--rw-r--r--   0 betterme   (501) staff       (20)      110 2023-09-27 09:39:06.000000 MeUtils-2024.3.4.13.4.45/meutils/notice/todo.md
--rw-r--r--   0 betterme   (501) staff       (20)     4112 2023-11-30 11:34:13.000000 MeUtils-2024.3.4.13.4.45/meutils/notice/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/notice/wechat_.py
--rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/notice/wecom.py
--rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/notice/weekmeet.py
--rw-r--r--   0 betterme   (501) staff       (20)     3559 2023-08-14 09:47:22.000000 MeUtils-2024.3.4.13.4.45/meutils/np_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.389471 MeUtils-2024.3.4.13.4.45/meutils/office_automation/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/office_automation/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2024.3.4.13.4.45/meutils/office_automation/doc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1528 2023-07-25 10:06:46.000000 MeUtils-2024.3.4.13.4.45/meutils/office_automation/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2024.3.4.13.4.45/meutils/office_automation/pdm.py
--rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2024.3.4.13.4.45/meutils/office_automation/pdm_run.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.391249 MeUtils-2024.3.4.13.4.45/meutils/office_automation/report/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/office_automation/report/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/office_automation/投资管理系统O3.2_交易组.pdm
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.393136 MeUtils-2024.3.4.13.4.45/meutils/other/
--rw-r--r--   0 betterme   (501) staff       (20)      996 2023-07-04 01:28:59.000000 MeUtils-2024.3.4.13.4.45/meutils/other/__demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/other/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.395978 MeUtils-2024.3.4.13.4.45/meutils/other/aiomultiprocess/
--rw-r--r--   0 betterme   (501) staff       (20)      416 2023-07-04 01:05:39.000000 MeUtils-2024.3.4.13.4.45/meutils/other/aiomultiprocess/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)       22 2023-07-04 01:01:15.000000 MeUtils-2024.3.4.13.4.45/meutils/other/aiomultiprocess/__version__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7835 2023-07-04 01:01:15.000000 MeUtils-2024.3.4.13.4.45/meutils/other/aiomultiprocess/core.py
--rw-r--r--   0 betterme   (501) staff       (20)    11688 2023-07-04 01:01:15.000000 MeUtils-2024.3.4.13.4.45/meutils/other/aiomultiprocess/pool.py
--rw-r--r--   0 betterme   (501) staff       (20)     2573 2023-07-04 01:01:15.000000 MeUtils-2024.3.4.13.4.45/meutils/other/aiomultiprocess/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1037 2023-07-04 01:01:15.000000 MeUtils-2024.3.4.13.4.45/meutils/other/aiomultiprocess/types.py
--rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/other/besttable.py
--rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2024.3.4.13.4.45/meutils/other/crontab.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.396932 MeUtils-2024.3.4.13.4.45/meutils/pandas_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/pandas_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/pandas_utils/opt.py
--rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/pandas_utils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2024.3.4.13.4.45/meutils/path_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)    10133 2023-11-27 09:25:49.000000 MeUtils-2024.3.4.13.4.45/meutils/pipe.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.400059 MeUtils-2024.3.4.13.4.45/meutils/playwright_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      291 2024-01-02 10:44:47.000000 MeUtils-2024.3.4.13.4.45/meutils/playwright_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)       92 2024-01-02 10:46:56.000000 MeUtils-2024.3.4.13.4.45/meutils/playwright_utils/__test.sh
--rw-r--r--   0 betterme   (501) staff       (20)     2266 2024-01-18 03:09:30.000000 MeUtils-2024.3.4.13.4.45/meutils/playwright_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     2444 2024-01-02 11:08:58.000000 MeUtils-2024.3.4.13.4.45/meutils/playwright_utils/kimi1_cookies.json
--rw-r--r--   0 betterme   (501) staff       (20)     2443 2024-01-02 11:08:57.000000 MeUtils-2024.3.4.13.4.45/meutils/playwright_utils/kimi2_cookies.json
--rw-r--r--   0 betterme   (501) staff       (20)     3334 2024-01-05 03:49:32.000000 MeUtils-2024.3.4.13.4.45/meutils/playwright_utils/kimi_cookies.json
--rw-r--r--   0 betterme   (501) staff       (20)     3145 2024-01-05 03:48:40.000000 MeUtils-2024.3.4.13.4.45/meutils/playwright_utils/reload.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.404031 MeUtils-2024.3.4.13.4.45/meutils/plots/
--rw-r--r--   0 betterme   (501) staff       (20)      276 2023-09-12 02:56:35.000000 MeUtils-2024.3.4.13.4.45/meutils/plots/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2022 2023-09-12 02:59:23.000000 MeUtils-2024.3.4.13.4.45/meutils/plots/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/plots/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/plots/echarts.py
--rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2024.3.4.13.4.45/meutils/plots/embedding_plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2024.3.4.13.4.45/meutils/plots/mecharts.py
--rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/plots/metrics.py
--rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/plots/plot_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.405367 MeUtils-2024.3.4.13.4.45/meutils/queues/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-07-20 02:35:53.000000 MeUtils-2024.3.4.13.4.45/meutils/queues/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1735 2023-12-06 09:14:18.000000 MeUtils-2024.3.4.13.4.45/meutils/queues/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     1562 2024-01-22 05:26:41.000000 MeUtils-2024.3.4.13.4.45/meutils/queues/uniform_queue.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.409006 MeUtils-2024.3.4.13.4.45/meutils/request_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     3375 2023-07-27 05:15:39.000000 MeUtils-2024.3.4.13.4.45/meutils/request_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1894 2023-11-03 02:19:03.000000 MeUtils-2024.3.4.13.4.45/meutils/request_utils/a爬虫.py
--rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2024.3.4.13.4.45/meutils/request_utils/crawler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2024.3.4.13.4.45/meutils/request_utils/download.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/request_utils/results.py
--rw-r--r--   0 betterme   (501) staff       (20)     3057 2023-12-04 10:37:44.000000 MeUtils-2024.3.4.13.4.45/meutils/request_utils/tiangong.py
--rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/request_utils/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)      646 2023-11-22 01:02:28.000000 MeUtils-2024.3.4.13.4.45/meutils/request_utils/公网ip.py
--rw-r--r--   0 betterme   (501) staff       (20)     1735 2024-01-17 05:19:28.000000 MeUtils-2024.3.4.13.4.45/meutils/request_utils/爬虫.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.409714 MeUtils-2024.3.4.13.4.45/meutils/schemas/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-24 06:44:44.000000 MeUtils-2024.3.4.13.4.45/meutils/schemas/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      484 2023-08-25 03:48:09.000000 MeUtils-2024.3.4.13.4.45/meutils/schemas/baidu_api.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.411541 MeUtils-2024.3.4.13.4.45/meutils/serving/
--rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2478 2023-05-11 08:02:45.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/_fastapi.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.414709 MeUtils-2024.3.4.13.4.45/meutils/serving/celery/
--rw-r--r--   0 betterme   (501) staff       (20)      628 2023-08-04 02:38:19.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/celery/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2109 2023-08-04 05:36:36.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/celery/_conf.py
--rw-r--r--   0 betterme   (501) staff       (20)      514 2023-08-04 06:55:40.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/celery/_demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-08-04 06:55:14.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/celery/_run.sh
--rw-r--r--   0 betterme   (501) staff       (20)      415 2023-08-04 07:01:12.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/celery/_run_fastapi.py
--rw-r--r--   0 betterme   (501) staff       (20)     1126 2023-11-08 05:27:33.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/celery/router.py
--rw-r--r--   0 betterme   (501) staff       (20)     1465 2023-08-04 07:31:09.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/celery/tasks.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.419252 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.420356 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/__demo/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-29 01:58:15.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/__demo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1444 2023-06-01 01:17:23.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/__demo/异步任务.py
--rw-r--r--   0 betterme   (501) staff       (20)      290 2023-05-26 07:01:26.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3897 2024-01-18 03:22:23.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.421133 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/dependencies/
--rw-r--r--   0 betterme   (501) staff       (20)      272 2023-12-19 09:14:44.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/dependencies/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      369 2023-12-19 09:14:44.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/dependencies/auth.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.422155 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/exceptions/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/exceptions/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      510 2024-01-08 08:24:52.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/exceptions/http_error.py
--rw-r--r--   0 betterme   (501) staff       (20)      825 2023-05-25 10:51:34.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/exceptions/validation_error.py
--rw-r--r--   0 betterme   (501) staff       (20)     7791 2024-02-22 02:14:50.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/gunicorn.conf.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.424330 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/routers/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-09 00:52:27.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/routers/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      546 2024-01-09 01:09:19.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/routers/_test.py
--rw-r--r--   0 betterme   (501) staff       (20)     1440 2024-01-09 01:03:15.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/routers/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)      544 2024-01-09 01:00:29.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/routers/shutdown.py
--rw-r--r--   0 betterme   (501) staff       (20)     1197 2024-01-18 08:10:48.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/routers/spider.py
--rw-r--r--   0 betterme   (501) staff       (20)     1624 2023-11-28 09:24:09.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.426760 MeUtils-2024.3.4.13.4.45/meutils/serving/gui/
--rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/gui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1690 2024-01-24 01:49:04.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/gui/bar.py
--rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/gui/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/gui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.427119 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.430723 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      889 2023-06-06 10:44:06.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/client.py
--rw-r--r--   0 betterme   (501) staff       (20)    14055 2023-07-24 05:52:25.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/flow.svg
--rw-r--r--   0 betterme   (501) staff       (20)      926 2023-07-24 06:13:28.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/s.py
--rw-r--r--   0 betterme   (501) staff       (20)      953 2023-07-24 06:17:01.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/s2.py
--rw-r--r--   0 betterme   (501) staff       (20)     2113 2023-07-24 06:04:10.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/server.py
--rw-r--r--   0 betterme   (501) staff       (20)     1160 2023-07-19 06:57:16.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/test.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.432952 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/executors/
--rw-r--r--   0 betterme   (501) staff       (20)     1805 2023-06-07 05:33:04.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/executors/SentenceEncoder.py
--rw-r--r--   0 betterme   (501) staff       (20)     1831 2023-07-17 10:23:25.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/executors/SentenceEncoder_.py
--rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-06-06 11:14:22.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/executors/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1093 2023-07-24 06:57:00.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/executors/base.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.433778 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/nlp_serving/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 01:14:50.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/nlp_serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1079 2023-06-06 07:52:01.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/jina/nlp_serving/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.434140 MeUtils-2024.3.4.13.4.45/meutils/serving/rq/
--rw-r--r--   0 betterme   (501) staff       (20)      321 2023-11-08 05:10:21.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/rq/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.438735 MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/
--rw-r--r--   0 betterme   (501) staff       (20)      291 2023-09-20 06:06:45.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      931 2023-12-04 10:19:52.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/_test.py
--rw-r--r--   0 betterme   (501) staff       (20)     3887 2023-11-21 03:52:24.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/chat_latex.py
--rw-r--r--   0 betterme   (501) staff       (20)     6909 2023-11-21 04:02:16.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-05-15 03:46:21.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)     1427 2023-11-03 05:24:48.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)    30236 2023-10-27 02:35:13.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/ocr.png
--rw-r--r--   0 betterme   (501) staff       (20)      300 2023-12-04 10:18:31.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.440956 MeUtils-2024.3.4.13.4.45/meutils/serving/webui/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.441632 MeUtils-2024.3.4.13.4.45/meutils/serving/webui/.streamlit/
--rw-r--r--   0 betterme   (501) staff       (20)     7586 2023-03-24 08:27:34.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/webui/.streamlit/_config.toml
--rw-r--r--   0 betterme   (501) staff       (20)      511 2023-03-24 08:27:34.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/webui/.streamlit/config.toml
--rw-r--r--   0 betterme   (501) staff       (20)     1757 2023-08-23 04:01:26.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/webui/_2_词性标注与实体识别.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-21 09:09:55.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      509 2023-08-23 04:01:26.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/webui/_🏆_主页.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.442947 MeUtils-2024.3.4.13.4.45/meutils/serving/webui/pages/
--rw-r--r--   0 betterme   (501) staff       (20)     1944 2023-08-23 04:01:26.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/webui/pages/_1_分词.py
--rw-r--r--   0 betterme   (501) staff       (20)     1715 2023-08-23 04:01:26.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/webui/pages/_2_词性标注与实体识别.py
--rw-r--r--   0 betterme   (501) staff       (20)     2425 2023-08-23 04:01:26.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/webui/pages/_3_文本匹配.py
--rwxr--r--   0 betterme   (501) staff       (20)      252 2023-05-22 10:17:52.000000 MeUtils-2024.3.4.13.4.45/meutils/serving/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.444071 MeUtils-2024.3.4.13.4.45/meutils/settings/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-21 06:24:50.000000 MeUtils-2024.3.4.13.4.45/meutils/settings/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      264 2023-08-21 06:29:43.000000 MeUtils-2024.3.4.13.4.45/meutils/settings/base.py
--rw-r--r--   0 betterme   (501) staff       (20)      484 2023-08-21 06:31:48.000000 MeUtils-2024.3.4.13.4.45/meutils/settings/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/sftp.py
--rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/sk_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1400 2023-08-25 08:16:40.000000 MeUtils-2024.3.4.13.4.45/meutils/smooth_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.444457 MeUtils-2024.3.4.13.4.45/meutils/spark/
--rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/spark/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.446162 MeUtils-2024.3.4.13.4.45/meutils/str_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/str_utils/Translator.py
--rw-r--r--   0 betterme   (501) staff       (20)     6697 2023-12-22 01:04:55.000000 MeUtils-2024.3.4.13.4.45/meutils/str_utils/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.452298 MeUtils-2024.3.4.13.4.45/meutils/str_utils/__translater/
--rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/str_utils/__translater/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/str_utils/__translater/tencent.py
--rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/str_utils/__translater/translater.py
--rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/str_utils/__translater/youdao.py
--rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-06-12 09:51:25.000000 MeUtils-2024.3.4.13.4.45/meutils/str_utils/json_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1903 2024-01-18 08:09:19.000000 MeUtils-2024.3.4.13.4.45/meutils/str_utils/regular_expression.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.453402 MeUtils-2024.3.4.13.4.45/meutils/tasks/
--rw-r--r--   0 betterme   (501) staff       (20)      280 2023-11-08 05:13:34.000000 MeUtils-2024.3.4.13.4.45/meutils/tasks/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      627 2023-11-08 05:23:51.000000 MeUtils-2024.3.4.13.4.45/meutils/tasks/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.458245 MeUtils-2024.3.4.13.4.45/meutils/templates/
--rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/demo.conf
--rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/demo.j2
--rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/demox.py
--rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/df_html.j2
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.460995 MeUtils-2024.3.4.13.4.45/meutils/templates/dockerfiles/
--rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/dockerfiles/Dockerfile
--rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/dockerfiles/Dockerfile_me
--rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/dockerfiles/Dockerfile_milvus
--rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/dockerfiles/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/dockerfiles/docker_build_push.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/dockerfiles/docker_push.sh
--rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/hegui.py
--rw-r--r--   0 betterme   (501) staff       (20)      540 2023-06-29 07:13:14.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/markmap.html
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.461232 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/
--rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/cookiecutter.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.469452 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.469960 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
--rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 betterme   (501) staff       (20)     1198 2023-05-31 00:59:56.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.474681 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.475003 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
--rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
--rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.475871 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.477050 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.478237 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/tpl.docx
--rw-r--r--   0 betterme   (501) staff       (20)      537 2023-06-29 07:15:57.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/x.html
--rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/templates/合规日报模板.docx
--rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2024.3.4.13.4.45/meutils/todo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.480415 MeUtils-2024.3.4.13.4.45/meutils/tools/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/tools/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/tools/cprint.py
--rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/tools/machine_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/tools/monitor.yml
--rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/tools/seize.py
--rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/tools/service_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/tools/sys_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)     1127 2023-12-11 10:37:26.000000 MeUtils-2024.3.4.13.4.45/meutils/types.py
--rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/meutils/zk_utils.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      550 2024-01-18 04:04:56.000000 MeUtils-2024.3.4.13.4.45/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)      418 2024-01-18 05:41:52.000000 MeUtils-2024.3.4.13.4.45/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       82 2024-01-17 10:32:32.000000 MeUtils-2024.3.4.13.4.45/requirements_ai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/requirements_app.txt
--rw-r--r--   0 betterme   (501) staff       (20)       52 2023-06-02 06:00:11.000000 MeUtils-2024.3.4.13.4.45/requirements_db.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-18 08:43:00.000000 MeUtils-2024.3.4.13.4.45/requirements_fileparser.txt
--rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/requirements_office.txt
--rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/requirements_pd.txt
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/requirements_plot.txt
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/requirements_plus.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.486176 MeUtils-2024.3.4.13.4.45/scripts/
--rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/scripts/demo.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-03-04 05:04:47.495154 MeUtils-2024.3.4.13.4.45/scripts/docker/
--rw-r--r--   0 betterme   (501) staff       (20)      556 2024-01-23 05:42:04.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/api-tokens.sh
--rw-r--r--   0 betterme   (501) staff       (20)     2235 2024-02-23 00:52:20.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/chat.sh
--rw-r--r--   0 betterme   (501) staff       (20)      708 2024-02-27 08:04:33.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/copilot.sh
--rw-r--r--   0 betterme   (501) staff       (20)      288 2024-02-27 08:04:33.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/copilot_config1.json
--rw-r--r--   0 betterme   (501) staff       (20)      283 2024-02-27 08:04:33.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/copilot_config2.json
--rw-r--r--   0 betterme   (501) staff       (20)      286 2024-02-27 08:04:33.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/copilot_config3.json
--rw-r--r--   0 betterme   (501) staff       (20)     1626 2023-12-15 01:03:06.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/docker连接宿主机mysql.md
--rw-r--r--   0 betterme   (501) staff       (20)      483 2024-01-22 16:05:10.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/elasticsearch.yml
--rw-r--r--   0 betterme   (501) staff       (20)     1297 2024-01-22 16:05:10.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/es.sh
--rw-r--r--   0 betterme   (501) staff       (20)      405 2024-01-05 06:04:39.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/kuma监控.sh
--rw-r--r--   0 betterme   (501) staff       (20)      524 2024-01-03 06:37:12.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/minio.sh
--rw-r--r--   0 betterme   (501) staff       (20)     4710 2024-02-19 09:38:11.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/oneapi.sh
--rw-r--r--   0 betterme   (501) staff       (20)      379 2024-02-05 03:27:42.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/文档智能.sh
--rw-r--r--   0 betterme   (501) staff       (20)      335 2023-12-22 11:51:25.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/构建镜像.sh
--rw-r--r--   0 betterme   (501) staff       (20)      366 2023-12-18 04:08:22.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/潘多拉.sh
--rw-r--r--   0 betterme   (501) staff       (20)     1052 2024-01-26 10:23:09.000000 MeUtils-2024.3.4.13.4.45/scripts/docker/镜像自动更新.sh
--rw-r--r--   0 betterme   (501) staff       (20)      640 2024-02-01 12:54:58.000000 MeUtils-2024.3.4.13.4.45/scripts/github代理.sh
--rw-r--r--   0 betterme   (501) staff       (20)      428 2023-12-12 05:47:22.000000 MeUtils-2024.3.4.13.4.45/scripts/hf_download.sh
--rw-r--r--   0 betterme   (501) staff       (20)      501 2024-02-23 02:33:52.000000 MeUtils-2024.3.4.13.4.45/scripts/jupyter.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/scripts/killall.sh
--rw-r--r--   0 betterme   (501) staff       (20)      478 2023-12-13 10:57:04.000000 MeUtils-2024.3.4.13.4.45/scripts/pip.conf
--rw-r--r--   0 betterme   (501) staff       (20)      268 2024-01-18 05:34:10.000000 MeUtils-2024.3.4.13.4.45/scripts/playwright.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/scripts/py_sh.sh
--rw-r--r--   0 betterme   (501) staff       (20)      414 2024-01-17 10:21:40.000000 MeUtils-2024.3.4.13.4.45/scripts/python软连接.sh
--rw-r--r--   0 betterme   (501) staff       (20)      620 2023-12-13 10:53:44.000000 MeUtils-2024.3.4.13.4.45/scripts/startup.sh
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2024.3.4.13.4.45/scripts/yum.sh
--rw-r--r--   0 betterme   (501) staff       (20)       34 2024-01-26 11:37:05.000000 MeUtils-2024.3.4.13.4.45/scripts/模型价格表
--rw-r--r--   0 betterme   (501) staff       (20)       38 2024-03-04 05:04:47.532296 MeUtils-2024.3.4.13.4.45/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2466 2023-11-29 08:25:30.000000 MeUtils-2024.3.4.13.4.45/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.121804 MeUtils-2024.4.11.9.12.58/
+-rw-r--r--   0 betterme   (501) staff       (20)    10244 2023-11-30 00:39:46.000000 MeUtils-2024.4.11.9.12.58/.DS_Store
+-rw-r--r--   0 betterme   (501) staff       (20)     1204 2023-05-22 06:35:12.000000 MeUtils-2024.4.11.9.12.58/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      331 2023-11-29 08:20:55.000000 MeUtils-2024.4.11.9.12.58/MANIFEST.in
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.116852 MeUtils-2024.4.11.9.12.58/MeUtils.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     5960 2024-04-11 01:12:59.000000 MeUtils-2024.4.11.9.12.58/MeUtils.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)    15743 2024-04-11 01:12:59.000000 MeUtils-2024.4.11.9.12.58/MeUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2024-04-11 01:12:59.000000 MeUtils-2024.4.11.9.12.58/MeUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      312 2024-04-11 01:12:59.000000 MeUtils-2024.4.11.9.12.58/MeUtils.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1186 2024-04-11 01:12:59.000000 MeUtils-2024.4.11.9.12.58/MeUtils.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2024-04-11 01:12:59.000000 MeUtils-2024.4.11.9.12.58/MeUtils.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     5960 2024-04-11 01:13:00.121489 MeUtils-2024.4.11.9.12.58/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2024.4.11.9.12.58/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-07-20 08:15:27.000000 MeUtils-2024.4.11.9.12.58/TODO.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:12:59.986809 MeUtils-2024.4.11.9.12.58/apps/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2024-01-18 04:10:04.000000 MeUtils-2024.4.11.9.12.58/apps/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      462 2024-01-18 04:20:39.000000 MeUtils-2024.4.11.9.12.58/apps/spider.py
+-rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/clear_githis.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      308 2023-08-11 00:53:48.000000 MeUtils-2024.4.11.9.12.58/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:12:59.991279 MeUtils-2024.4.11.9.12.58/meutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      348 2023-08-17 00:48:50.000000 MeUtils-2024.4.11.9.12.58/meutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2024.4.11.9.12.58/meutils/_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:12:59.997028 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 05:51:24.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-11-21 10:11:16.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/adjusted_audio1.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:12:59.998175 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/asr/
+-rw-r--r--   0 betterme   (501) staff       (20)      825 2023-11-28 10:28:28.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/asr/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3121 2023-11-28 02:24:07.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/asr/fast_asr.py
+-rw-r--r--   0 betterme   (501) staff       (20)      514 2023-12-11 10:44:07.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/asr/openai_asr.py
+-rw-r--r--   0 betterme   (501) staff       (20)      823 2023-11-28 02:20:46.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/asr/subtitle.srt
+-rw-r--r--   0 betterme   (501) staff       (20)     7251 2023-12-01 04:06:03.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/asr/xunfei_asr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1226 2023-11-21 06:01:47.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/asr.py
+-rw-r--r--   0 betterme   (501) staff       (20)  2879556 2023-11-27 03:16:45.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/demo.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)     3790 2023-11-24 08:13:08.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/example.srt
+-rw-r--r--   0 betterme   (501) staff       (20)     2968 2023-11-21 11:25:44.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/fast_asr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-11-21 12:22:26.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/new.srt
+-rw-r--r--   0 betterme   (501) staff       (20)     9087 2023-11-21 11:36:58.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/subtitles.srt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:12:59.999551 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/tts/
+-rw-r--r--   0 betterme   (501) staff       (20)     5884 2024-03-27 05:35:42.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/tts/EdgeTTS.py
+-rw-r--r--   0 betterme   (501) staff       (20)      405 2023-12-26 05:42:13.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/tts/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-11-21 12:22:26.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/tts/new.srt
+-rw-r--r--   0 betterme   (501) staff       (20)     1755 2024-03-27 06:30:42.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/tts/openai_tts.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4638 2024-03-27 03:35:59.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/tts/tts_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2494 2023-11-21 10:39:01.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/tts.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1214 2023-11-28 10:28:28.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1898 2023-11-22 09:47:51.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_audio/视频合并.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.004327 MeUtils-2024.4.11.9.12.58/meutils/ai_cv/
+-rwxr-xr-x   0 betterme   (501) staff       (20)    20960 2023-08-31 09:02:20.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_cv/1.jpg
+-rwxr-xr-x   0 betterme   (501) staff       (20)     8285 2023-08-31 09:27:34.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_cv/197.jpg
+-rwxr-xr-x   0 betterme   (501) staff       (20)    27190 2023-08-31 09:02:20.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_cv/2.jpg
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:11:56.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_cv/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2684 2023-09-01 11:12:26.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_cv/doc_prompt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    49873 2023-09-25 03:07:24.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_cv/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)   335396 2023-08-25 05:34:53.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_cv/invoice.jpg
+-rw-r--r--   0 betterme   (501) staff       (20)     1152 2023-11-02 10:12:40.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_cv/latex_ocr.py
+-rw-r--r--   0 betterme   (501) staff       (20)      682 2023-10-24 01:58:01.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_cv/ocr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2401 2023-09-25 04:18:07.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_cv/ocr_api.py
+-rw-r--r--   0 betterme   (501) staff       (20)   159229 2023-10-24 01:56:18.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_cv/tbl.png
+-rw-r--r--   0 betterme   (501) staff       (20)    24809 2023-10-27 03:01:01.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_cv/test.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.007309 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/
+-rw-r--r--   0 betterme   (501) staff       (20)     6927 2023-06-30 13:22:13.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/SplitSentence.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13489 2023-05-21 05:19:20.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/Untitled-1(1).py
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2295 2023-04-10 08:57:58.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/_lda.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.008145 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/_textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)      287 2023-05-22 01:52:50.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/_textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-05-21 05:10:54.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2282 2023-05-21 05:27:40.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/_textsplitter/text_split.py
+-rw-r--r--   0 betterme   (501) staff       (20)      650 2023-12-12 02:19:51.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      329 2023-10-26 01:47:40.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/epub翻译.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-06-06 06:44:28.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/lda.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2560 2023-07-25 08:50:49.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/ner.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1019 2023-12-12 03:58:07.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/text_transformer.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2111 2023-06-30 13:18:15.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3542 2023-06-05 05:29:27.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.009821 MeUtils-2024.4.11.9.12.58/meutils/ai_video/
+-rw-r--r--   0 betterme   (501) staff       (20)      254 2020-12-15 11:24:42.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_video/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1143 2023-11-20 10:32:55.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_video/avmerge.py
+-rw-r--r--   0 betterme   (501) staff       (20)      881 2023-11-22 09:38:35.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_video/avmerge_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3470 2023-11-24 07:46:38.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_video/scene_detect.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1760 2023-11-24 07:57:00.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_video/test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1727 2023-11-24 08:38:38.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_video/video.py
+-rw-r--r--   0 betterme   (501) staff       (20)      902 2023-11-17 08:12:46.000000 MeUtils-2024.4.11.9.12.58/meutils/ai_video/xx.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.012598 MeUtils-2024.4.11.9.12.58/meutils/ann/
+-rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/README_gensim.md
+-rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/ann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/ann_faiss.py
+-rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/ann_gensim.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-05-16 06:47:06.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/ann_inmemory.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-05-19 06:06:57.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/ann_qdrant.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/ann_service.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/ann_v1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.012905 MeUtils-2024.4.11.9.12.58/meutils/ann/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/examples/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/examples/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/milvus.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/ann/shake_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.013934 MeUtils-2024.4.11.9.12.58/meutils/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      344 2023-12-04 08:54:59.000000 MeUtils-2024.4.11.9.12.58/meutils/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3657 2024-02-05 02:46:19.000000 MeUtils-2024.4.11.9.12.58/meutils/api/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      735 2024-03-01 09:00:39.000000 MeUtils-2024.4.11.9.12.58/meutils/api/deeplx.py
+-rw-r--r--   0 betterme   (501) staff       (20)   421916 2023-12-07 02:25:29.000000 MeUtils-2024.4.11.9.12.58/meutils/api/qr.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.018417 MeUtils-2024.4.11.9.12.58/meutils/async_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      284 2023-08-28 05:10:12.000000 MeUtils-2024.4.11.9.12.58/meutils/async_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1523 2024-02-29 11:04:14.000000 MeUtils-2024.4.11.9.12.58/meutils/async_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8285 2024-01-20 10:30:04.000000 MeUtils-2024.4.11.9.12.58/meutils/cache_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.025407 MeUtils-2024.4.11.9.12.58/meutils/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      784 2024-01-05 03:29:34.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/__test.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     4511 2024-01-03 02:50:38.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/browser.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3212 2024-02-21 06:58:51.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      319 2024-01-17 03:02:30.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/cloudflare.py
+-rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/cron.py
+-rw-r--r--   0 betterme   (501) staff       (20)      180 2024-01-03 02:23:43.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:24:07.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_13003330042.json
+-rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:11:32.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_13003872192.json
+-rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:24:42.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_13852263862.json
+-rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:24:28.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_13913898681.json
+-rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:24:21.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_13962978617.json
+-rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:24:16.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_15251801790.json
+-rw-r--r--   0 betterme   (501) staff       (20)     2596 2024-01-03 02:24:37.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_15720826383.json
+-rw-r--r--   0 betterme   (501) staff       (20)     2597 2024-01-03 02:24:12.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_18395563611.json
+-rw-r--r--   0 betterme   (501) staff       (20)     2617 2024-01-03 02:24:32.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_313303303@qq.com.json
+-rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/gunicorn.conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2032 2024-01-05 03:30:04.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/kimi_state.json
+-rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      731 2023-08-30 03:57:39.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/nesc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1757 2023-12-27 00:56:08.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/notice.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2411 2024-02-27 08:32:53.000000 MeUtils-2024.4.11.9.12.58/meutils/clis/server.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.026316 MeUtils-2024.4.11.9.12.58/meutils/cmds/
+-rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/cmds/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/cmds/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/cmds/cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/cmds/hdfs_cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/cmds/subprocess_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.026683 MeUtils-2024.4.11.9.12.58/meutils/coding/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/coding/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/coding/find132.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15339 2024-03-22 01:11:55.000000 MeUtils-2024.4.11.9.12.58/meutils/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.027025 MeUtils-2024.4.11.9.12.58/meutils/comp_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/comp_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/comp_utils/reverse_metric.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.039680 MeUtils-2024.4.11.9.12.58/meutils/data/
+-rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2024.4.11.9.12.58/meutils/data/SimHei.ttf
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2024-04-11 01:12:58.000000 MeUtils-2024.4.11.9.12.58/meutils/data/VERSION
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/data/_FLAG
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/data/_SUCCESS
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/data/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/data/coordinate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2497 2023-09-07 05:50:11.000000 MeUtils-2024.4.11.9.12.58/meutils/date_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.042264 MeUtils-2024.4.11.9.12.58/meutils/db/
+-rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/db/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     7637 2024-01-05 00:39:21.000000 MeUtils-2024.4.11.9.12.58/meutils/db/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/db/mongo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/db/neo4j.py
+-rw-r--r--   0 betterme   (501) staff       (20)      265 2024-03-26 03:21:15.000000 MeUtils-2024.4.11.9.12.58/meutils/db/redis_db.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.045797 MeUtils-2024.4.11.9.12.58/meutils/decorators/
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1681 2023-05-25 09:49:50.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/__ai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2951 2023-12-28 05:10:23.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/cache.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/catch.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10644 2024-03-27 05:09:13.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1251 2024-01-16 12:50:20.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/contextmanagers.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/decorator.py
+-rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/decorator_demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      710 2023-12-26 09:35:03.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1355 2024-01-09 00:35:44.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/fastapi_decorator.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3634 2023-08-24 02:55:32.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2976 2024-02-27 09:07:28.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/retry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2664 2023-11-06 02:17:41.000000 MeUtils-2024.4.11.9.12.58/meutils/decorators/schedulers.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.046044 MeUtils-2024.4.11.9.12.58/meutils/dependencies/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-02 08:27:24.000000 MeUtils-2024.4.11.9.12.58/meutils/dependencies/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3640 2023-05-15 10:32:24.000000 MeUtils-2024.4.11.9.12.58/meutils/dist_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.047290 MeUtils-2024.4.11.9.12.58/meutils/docarray_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2024.4.11.9.12.58/meutils/docarray_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2024.4.11.9.12.58/meutils/docarray_utils/demo_es.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2024.4.11.9.12.58/meutils/docarray_utils/demo_hnsw.py
+-rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2024.4.11.9.12.58/meutils/docarray_utils/in_memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2024.4.11.9.12.58/meutils/docarray_utils/改造下hnsw.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.047807 MeUtils-2024.4.11.9.12.58/meutils/easy_search/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/easy_search/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2425 2023-08-02 06:36:30.000000 MeUtils-2024.4.11.9.12.58/meutils/easy_search/es.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.049409 MeUtils-2024.4.11.9.12.58/meutils/fileparser/
+-rw-r--r--   0 betterme   (501) staff       (20)     1975 2023-05-30 05:34:49.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/PDF抽取.py
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-18 08:38:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      284 2023-07-12 04:10:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2792 2023-08-16 04:33:39.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.050680 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/
+-rw-r--r--   0 betterme   (501) staff       (20)      223 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      803 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/__main__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2122 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/filetype.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2947 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/helpers.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3288 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/match.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.052765 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/
+-rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      498 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/application.py
+-rw-r--r--   0 betterme   (501) staff       (20)    17006 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/archive.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4960 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/audio.py
+-rw-r--r--   0 betterme   (501) staff       (20)      647 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7513 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/document.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2924 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/font.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9130 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)      958 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/isobmff.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5371 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/video.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2089 2023-05-18 08:40:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      285 2023-07-15 07:06:30.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype.py
+-rw-r--r--   0 betterme   (501) staff       (20)      639 2023-08-10 05:04:53.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4037 2023-07-17 10:15:11.000000 MeUtils-2024.4.11.9.12.58/meutils/fileparser/表格抽取.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2024.4.11.9.12.58/meutils/hash_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/import_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.053494 MeUtils-2024.4.11.9.12.58/meutils/init/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2024.4.11.9.12.58/meutils/init/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1588 2023-08-07 08:26:31.000000 MeUtils-2024.4.11.9.12.58/meutils/init/evn.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12884 2023-07-06 01:18:39.000000 MeUtils-2024.4.11.9.12.58/meutils/init/oo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.055544 MeUtils-2024.4.11.9.12.58/meutils/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2024.4.11.9.12.58/meutils/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/io/file.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2785 2024-03-13 05:49:08.000000 MeUtils-2024.4.11.9.12.58/meutils/io/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)    49873 2023-09-25 03:07:24.000000 MeUtils-2024.4.11.9.12.58/meutils/io/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)     1274 2024-02-05 09:39:04.000000 MeUtils-2024.4.11.9.12.58/meutils/io/minio_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8605 2023-06-26 01:26:21.000000 MeUtils-2024.4.11.9.12.58/meutils/io/tf_io.py
+-rw-r--r--   0 betterme   (501) staff       (20)        2 2024-01-03 06:54:16.000000 MeUtils-2024.4.11.9.12.58/meutils/io/x.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/jinja_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.056426 MeUtils-2024.4.11.9.12.58/meutils/logging/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-15 06:07:38.000000 MeUtils-2024.4.11.9.12.58/meutils/logging/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      701 2023-08-21 08:23:51.000000 MeUtils-2024.4.11.9.12.58/meutils/logging/handlers.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2937 2023-08-15 01:04:50.000000 MeUtils-2024.4.11.9.12.58/meutils/logging/log_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6183 2024-02-08 00:37:38.000000 MeUtils-2024.4.11.9.12.58/meutils/logging/logger.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.059399 MeUtils-2024.4.11.9.12.58/meutils/notice/
+-rw-r--r--   0 betterme   (501) staff       (20)      248 2023-08-30 03:57:39.000000 MeUtils-2024.4.11.9.12.58/meutils/notice/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-10-16 09:04:49.000000 MeUtils-2024.4.11.9.12.58/meutils/notice/emails.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2411 2024-03-26 07:39:26.000000 MeUtils-2024.4.11.9.12.58/meutils/notice/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/notice/file_post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7836 2023-09-27 09:38:07.000000 MeUtils-2024.4.11.9.12.58/meutils/notice/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)     7331 2023-09-12 01:53:53.000000 MeUtils-2024.4.11.9.12.58/meutils/notice/load_emailfile - 副本.py
+-rw-r--r--   0 betterme   (501) staff       (20)      110 2023-09-27 09:39:06.000000 MeUtils-2024.4.11.9.12.58/meutils/notice/todo.md
+-rw-r--r--   0 betterme   (501) staff       (20)     4207 2024-03-06 06:10:50.000000 MeUtils-2024.4.11.9.12.58/meutils/notice/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/notice/wechat_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/notice/wecom.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/notice/weekmeet.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3559 2023-08-14 09:47:22.000000 MeUtils-2024.4.11.9.12.58/meutils/np_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.061169 MeUtils-2024.4.11.9.12.58/meutils/office_automation/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/office_automation/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2024.4.11.9.12.58/meutils/office_automation/doc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1528 2023-07-25 10:06:46.000000 MeUtils-2024.4.11.9.12.58/meutils/office_automation/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2024.4.11.9.12.58/meutils/office_automation/pdm.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2024.4.11.9.12.58/meutils/office_automation/pdm_run.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.062103 MeUtils-2024.4.11.9.12.58/meutils/office_automation/report/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/office_automation/report/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/office_automation/投资管理系统O3.2_交易组.pdm
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.062741 MeUtils-2024.4.11.9.12.58/meutils/oss/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2024-03-14 09:54:51.000000 MeUtils-2024.4.11.9.12.58/meutils/oss/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4500 2024-03-18 03:06:05.000000 MeUtils-2024.4.11.9.12.58/meutils/oss/minio_oss.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1274 2024-02-05 09:39:04.000000 MeUtils-2024.4.11.9.12.58/meutils/oss/minio_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.063874 MeUtils-2024.4.11.9.12.58/meutils/other/
+-rw-r--r--   0 betterme   (501) staff       (20)      996 2023-07-04 01:28:59.000000 MeUtils-2024.4.11.9.12.58/meutils/other/__demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/other/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.065899 MeUtils-2024.4.11.9.12.58/meutils/other/aiomultiprocess/
+-rw-r--r--   0 betterme   (501) staff       (20)      416 2023-07-04 01:05:39.000000 MeUtils-2024.4.11.9.12.58/meutils/other/aiomultiprocess/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2023-07-04 01:01:15.000000 MeUtils-2024.4.11.9.12.58/meutils/other/aiomultiprocess/__version__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7835 2023-07-04 01:01:15.000000 MeUtils-2024.4.11.9.12.58/meutils/other/aiomultiprocess/core.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11688 2023-07-04 01:01:15.000000 MeUtils-2024.4.11.9.12.58/meutils/other/aiomultiprocess/pool.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2573 2023-07-04 01:01:15.000000 MeUtils-2024.4.11.9.12.58/meutils/other/aiomultiprocess/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1037 2023-07-04 01:01:15.000000 MeUtils-2024.4.11.9.12.58/meutils/other/aiomultiprocess/types.py
+-rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/other/besttable.py
+-rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2024.4.11.9.12.58/meutils/other/crontab.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.066588 MeUtils-2024.4.11.9.12.58/meutils/pandas_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/pandas_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/pandas_utils/opt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/pandas_utils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2024.4.11.9.12.58/meutils/path_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10133 2023-11-27 09:25:49.000000 MeUtils-2024.4.11.9.12.58/meutils/pipe.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.068415 MeUtils-2024.4.11.9.12.58/meutils/playwright_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2024-01-02 10:44:47.000000 MeUtils-2024.4.11.9.12.58/meutils/playwright_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)       92 2024-01-02 10:46:56.000000 MeUtils-2024.4.11.9.12.58/meutils/playwright_utils/__test.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     2266 2024-01-18 03:09:30.000000 MeUtils-2024.4.11.9.12.58/meutils/playwright_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2444 2024-01-02 11:08:58.000000 MeUtils-2024.4.11.9.12.58/meutils/playwright_utils/kimi1_cookies.json
+-rw-r--r--   0 betterme   (501) staff       (20)     2443 2024-01-02 11:08:57.000000 MeUtils-2024.4.11.9.12.58/meutils/playwright_utils/kimi2_cookies.json
+-rw-r--r--   0 betterme   (501) staff       (20)     3334 2024-01-05 03:49:32.000000 MeUtils-2024.4.11.9.12.58/meutils/playwright_utils/kimi_cookies.json
+-rw-r--r--   0 betterme   (501) staff       (20)     3145 2024-01-05 03:48:40.000000 MeUtils-2024.4.11.9.12.58/meutils/playwright_utils/reload.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.070407 MeUtils-2024.4.11.9.12.58/meutils/plots/
+-rw-r--r--   0 betterme   (501) staff       (20)      276 2023-09-12 02:56:35.000000 MeUtils-2024.4.11.9.12.58/meutils/plots/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2022 2023-09-12 02:59:23.000000 MeUtils-2024.4.11.9.12.58/meutils/plots/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/plots/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/plots/echarts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2024.4.11.9.12.58/meutils/plots/embedding_plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2024.4.11.9.12.58/meutils/plots/mecharts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/plots/metrics.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/plots/plot_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.071589 MeUtils-2024.4.11.9.12.58/meutils/queues/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-07-20 02:35:53.000000 MeUtils-2024.4.11.9.12.58/meutils/queues/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1735 2023-12-06 09:14:18.000000 MeUtils-2024.4.11.9.12.58/meutils/queues/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1491 2024-03-22 07:55:29.000000 MeUtils-2024.4.11.9.12.58/meutils/queues/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3269 2024-03-27 04:40:48.000000 MeUtils-2024.4.11.9.12.58/meutils/queues/smooth_queue.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1564 2024-03-22 09:12:23.000000 MeUtils-2024.4.11.9.12.58/meutils/queues/uniform_queue.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.073629 MeUtils-2024.4.11.9.12.58/meutils/request_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     3375 2023-07-27 05:15:39.000000 MeUtils-2024.4.11.9.12.58/meutils/request_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1894 2023-11-03 02:19:03.000000 MeUtils-2024.4.11.9.12.58/meutils/request_utils/a爬虫.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2024.4.11.9.12.58/meutils/request_utils/crawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2024.4.11.9.12.58/meutils/request_utils/download.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/request_utils/results.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3057 2023-12-04 10:37:44.000000 MeUtils-2024.4.11.9.12.58/meutils/request_utils/tiangong.py
+-rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/request_utils/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)      646 2023-11-22 01:02:28.000000 MeUtils-2024.4.11.9.12.58/meutils/request_utils/公网ip.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1735 2024-01-17 05:19:28.000000 MeUtils-2024.4.11.9.12.58/meutils/request_utils/爬虫.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.074132 MeUtils-2024.4.11.9.12.58/meutils/schemas/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-24 06:44:44.000000 MeUtils-2024.4.11.9.12.58/meutils/schemas/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      484 2023-08-25 03:48:09.000000 MeUtils-2024.4.11.9.12.58/meutils/schemas/baidu_api.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.074915 MeUtils-2024.4.11.9.12.58/meutils/serving/
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2478 2023-05-11 08:02:45.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/_fastapi.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.077179 MeUtils-2024.4.11.9.12.58/meutils/serving/celery/
+-rw-r--r--   0 betterme   (501) staff       (20)      628 2023-08-04 02:38:19.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/celery/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2109 2023-08-04 05:36:36.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/celery/_conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      514 2023-08-04 06:55:40.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/celery/_demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-08-04 06:55:14.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/celery/_run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      415 2023-08-04 07:01:12.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/celery/_run_fastapi.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1126 2023-11-08 05:27:33.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/celery/router.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1465 2023-08-04 07:31:09.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/celery/tasks.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.080855 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.081381 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-29 01:58:15.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1444 2023-06-01 01:17:23.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/__demo/异步任务.py
+-rw-r--r--   0 betterme   (501) staff       (20)      290 2023-05-26 07:01:26.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3897 2024-01-18 03:22:23.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.081880 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/dependencies/
+-rw-r--r--   0 betterme   (501) staff       (20)      272 2023-12-19 09:14:44.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/dependencies/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      369 2023-12-19 09:14:44.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/dependencies/auth.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.082537 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/exceptions/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/exceptions/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      509 2024-03-14 10:06:19.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/exceptions/http_error.py
+-rw-r--r--   0 betterme   (501) staff       (20)      825 2023-05-25 10:51:34.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/exceptions/validation_error.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7791 2024-02-22 02:14:50.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/gunicorn.conf.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.084166 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/routers/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-09 00:52:27.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/routers/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      546 2024-01-09 01:09:19.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/routers/_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1440 2024-01-09 01:03:15.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/routers/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      544 2024-01-09 01:00:29.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/routers/shutdown.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1197 2024-01-18 08:10:48.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/routers/spider.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2994 2024-03-14 10:39:22.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.085237 MeUtils-2024.4.11.9.12.58/meutils/serving/gui/
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/gui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1690 2024-01-24 01:49:04.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/gui/bar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/gui/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/gui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.085516 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.087390 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      889 2023-06-06 10:44:06.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14055 2023-07-24 05:52:25.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/flow.svg
+-rw-r--r--   0 betterme   (501) staff       (20)      926 2023-07-24 06:13:28.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/s.py
+-rw-r--r--   0 betterme   (501) staff       (20)      953 2023-07-24 06:17:01.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/s2.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2113 2023-07-24 06:04:10.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/server.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1160 2023-07-19 06:57:16.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/test.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.088367 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/executors/
+-rw-r--r--   0 betterme   (501) staff       (20)     1805 2023-06-07 05:33:04.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/executors/SentenceEncoder.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1831 2023-07-17 10:23:25.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/executors/SentenceEncoder_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-06-06 11:14:22.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/executors/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1093 2023-07-24 06:57:00.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/executors/base.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.088866 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/nlp_serving/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 01:14:50.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/nlp_serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1079 2023-06-06 07:52:01.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/jina/nlp_serving/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.089099 MeUtils-2024.4.11.9.12.58/meutils/serving/rq/
+-rw-r--r--   0 betterme   (501) staff       (20)      321 2023-11-08 05:10:21.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/rq/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.091310 MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2023-09-20 06:06:45.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      931 2023-12-04 10:19:52.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3887 2023-11-21 03:52:24.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/chat_latex.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6930 2024-03-25 05:38:12.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-05-15 03:46:21.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)     1427 2023-11-03 05:24:48.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)    30236 2023-10-27 02:35:13.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/ocr.png
+-rw-r--r--   0 betterme   (501) staff       (20)      300 2023-12-04 10:18:31.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.092424 MeUtils-2024.4.11.9.12.58/meutils/serving/webui/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.093131 MeUtils-2024.4.11.9.12.58/meutils/serving/webui/.streamlit/
+-rw-r--r--   0 betterme   (501) staff       (20)     7586 2023-03-24 08:27:34.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/webui/.streamlit/_config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)      511 2023-03-24 08:27:34.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/webui/.streamlit/config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)     1757 2023-08-23 04:01:26.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/webui/_2_词性标注与实体识别.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-21 09:09:55.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      509 2023-08-23 04:01:26.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/webui/_🏆_主页.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.093991 MeUtils-2024.4.11.9.12.58/meutils/serving/webui/pages/
+-rw-r--r--   0 betterme   (501) staff       (20)     1944 2023-08-23 04:01:26.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/webui/pages/_1_分词.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1715 2023-08-23 04:01:26.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/webui/pages/_2_词性标注与实体识别.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2425 2023-08-23 04:01:26.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/webui/pages/_3_文本匹配.py
+-rwxr--r--   0 betterme   (501) staff       (20)      252 2023-05-22 10:17:52.000000 MeUtils-2024.4.11.9.12.58/meutils/serving/webui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.094845 MeUtils-2024.4.11.9.12.58/meutils/settings/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-21 06:24:50.000000 MeUtils-2024.4.11.9.12.58/meutils/settings/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      264 2023-08-21 06:29:43.000000 MeUtils-2024.4.11.9.12.58/meutils/settings/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)      484 2023-08-21 06:31:48.000000 MeUtils-2024.4.11.9.12.58/meutils/settings/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/sftp.py
+-rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/sk_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1400 2023-08-25 08:16:40.000000 MeUtils-2024.4.11.9.12.58/meutils/smooth_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.095103 MeUtils-2024.4.11.9.12.58/meutils/spark/
+-rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/spark/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.096047 MeUtils-2024.4.11.9.12.58/meutils/str_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/str_utils/Translator.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6697 2023-12-22 01:04:55.000000 MeUtils-2024.4.11.9.12.58/meutils/str_utils/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.096949 MeUtils-2024.4.11.9.12.58/meutils/str_utils/__translater/
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/str_utils/__translater/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/str_utils/__translater/tencent.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/str_utils/__translater/translater.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/str_utils/__translater/youdao.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-06-12 09:51:25.000000 MeUtils-2024.4.11.9.12.58/meutils/str_utils/json_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1903 2024-01-18 08:09:19.000000 MeUtils-2024.4.11.9.12.58/meutils/str_utils/regular_expression.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.097414 MeUtils-2024.4.11.9.12.58/meutils/tasks/
+-rw-r--r--   0 betterme   (501) staff       (20)      280 2023-11-08 05:13:34.000000 MeUtils-2024.4.11.9.12.58/meutils/tasks/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      627 2023-11-08 05:23:51.000000 MeUtils-2024.4.11.9.12.58/meutils/tasks/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.099740 MeUtils-2024.4.11.9.12.58/meutils/templates/
+-rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/demo.conf
+-rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/demo.j2
+-rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/demox.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/df_html.j2
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.101196 MeUtils-2024.4.11.9.12.58/meutils/templates/dockerfiles/
+-rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/dockerfiles/Dockerfile
+-rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/dockerfiles/Dockerfile_me
+-rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/dockerfiles/Dockerfile_milvus
+-rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/dockerfiles/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/dockerfiles/docker_build_push.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/dockerfiles/docker_push.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/hegui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      540 2023-06-29 07:13:14.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/markmap.html
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.101356 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/
+-rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/cookiecutter.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.104852 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.105029 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1198 2023-05-31 00:59:56.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.107283 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.107434 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
+-rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.107764 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.108193 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.108746 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/tpl.docx
+-rw-r--r--   0 betterme   (501) staff       (20)      537 2023-06-29 07:15:57.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/x.html
+-rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/templates/合规日报模板.docx
+-rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2024.4.11.9.12.58/meutils/todo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.109872 MeUtils-2024.4.11.9.12.58/meutils/tools/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/tools/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/tools/cprint.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/tools/machine_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/tools/monitor.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/tools/seize.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/tools/service_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/tools/sys_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1127 2023-12-11 10:37:26.000000 MeUtils-2024.4.11.9.12.58/meutils/types.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/meutils/zk_utils.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      550 2024-01-18 04:04:56.000000 MeUtils-2024.4.11.9.12.58/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      418 2024-01-18 05:41:52.000000 MeUtils-2024.4.11.9.12.58/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       82 2024-01-17 10:32:32.000000 MeUtils-2024.4.11.9.12.58/requirements_ai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/requirements_app.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       52 2023-06-02 06:00:11.000000 MeUtils-2024.4.11.9.12.58/requirements_db.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-18 08:43:00.000000 MeUtils-2024.4.11.9.12.58/requirements_fileparser.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/requirements_office.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/requirements_pd.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/requirements_plot.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/requirements_plus.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.112285 MeUtils-2024.4.11.9.12.58/scripts/
+-rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/scripts/demo.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-11 01:13:00.116521 MeUtils-2024.4.11.9.12.58/scripts/docker/
+-rw-r--r--   0 betterme   (501) staff       (20)      556 2024-01-23 05:42:04.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/api-tokens.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     3726 2024-04-09 09:54:20.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/chat.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     1626 2023-12-15 01:03:06.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/docker连接宿主机mysql.md
+-rw-r--r--   0 betterme   (501) staff       (20)      483 2024-01-22 16:05:10.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/elasticsearch.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1297 2024-01-22 16:05:10.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/es.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      250 2024-04-08 05:55:45.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/gpt.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      405 2024-01-05 06:04:39.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/kuma监控.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      524 2024-01-03 06:37:12.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/minio.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     1021 2024-03-06 03:10:04.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/nineai-docker-compose.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1599 2024-03-26 11:16:33.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/ollama.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     5349 2024-04-09 08:18:48.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/oneapi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      418 2024-04-02 05:49:05.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/导航页.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      379 2024-03-18 07:54:30.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/文档智能.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      335 2024-03-18 09:37:51.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/构建镜像.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      366 2023-12-18 04:08:22.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/潘多拉.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      777 2024-04-01 11:01:49.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/逆向.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     1162 2024-04-02 09:52:07.000000 MeUtils-2024.4.11.9.12.58/scripts/docker/镜像自动更新.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      640 2024-02-01 12:54:58.000000 MeUtils-2024.4.11.9.12.58/scripts/github代理.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      428 2023-12-12 05:47:22.000000 MeUtils-2024.4.11.9.12.58/scripts/hf_download.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      514 2024-03-26 07:19:49.000000 MeUtils-2024.4.11.9.12.58/scripts/jupyter.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/scripts/killall.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      478 2023-12-13 10:57:04.000000 MeUtils-2024.4.11.9.12.58/scripts/pip.conf
+-rw-r--r--   0 betterme   (501) staff       (20)      268 2024-01-18 05:34:10.000000 MeUtils-2024.4.11.9.12.58/scripts/playwright.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/scripts/py_sh.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      414 2024-01-17 10:21:40.000000 MeUtils-2024.4.11.9.12.58/scripts/python软连接.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      620 2023-12-13 10:53:44.000000 MeUtils-2024.4.11.9.12.58/scripts/startup.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2024.4.11.9.12.58/scripts/yum.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       34 2024-01-26 11:37:05.000000 MeUtils-2024.4.11.9.12.58/scripts/模型价格表
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2024-04-11 01:13:00.121870 MeUtils-2024.4.11.9.12.58/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2466 2023-11-29 08:25:30.000000 MeUtils-2024.4.11.9.12.58/setup.py
```

### Comparing `MeUtils-2024.3.4.13.4.45/.DS_Store` & `MeUtils-2024.4.11.9.12.58/.DS_Store`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/.gitignore` & `MeUtils-2024.4.11.9.12.58/.gitignore`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/LICENSE` & `MeUtils-2024.4.11.9.12.58/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/MeUtils.egg-info/PKG-INFO` & `MeUtils-2024.4.11.9.12.58/MeUtils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2024.3.4.13.4.45
+Version: 2024.4.11.9.12.58
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
@@ -98,50 +98,50 @@
 Requires-Dist: sqlalchemy; extra == "db"
 Provides-Extra: pd
 Requires-Dist: dataframe_image; extra == "pd"
 Requires-Dist: pandas-profiling[notebook]; extra == "pd"
 Requires-Dist: pandas_summary; extra == "pd"
 Requires-Dist: polars; extra == "pd"
 Provides-Extra: all
-Requires-Dist: polars; extra == "all"
+Requires-Dist: pymysql; extra == "all"
 Requires-Dist: asyncmy; extra == "all"
+Requires-Dist: pandas_summary; extra == "all"
+Requires-Dist: iteration_utilities; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: pyarrow; extra == "all"
 Requires-Dist: geopy; extra == "all"
 Requires-Dist: pymongo; extra == "all"
-Requires-Dist: missingno; extra == "all"
+Requires-Dist: pretty_errors; extra == "all"
+Requires-Dist: thefuck; extra == "all"
+Requires-Dist: jieba; extra == "all"
+Requires-Dist: filetype; extra == "all"
 Requires-Dist: pymilvus; extra == "all"
-Requires-Dist: redis-py-cluster; extra == "all"
-Requires-Dist: langchain; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: sse_starlette; extra == "all"
-Requires-Dist: pymupd; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: iteration_utilities; extra == "all"
-Requires-Dist: faiss-cpu; extra == "all"
-Requires-Dist: schedule; extra == "all"
 Requires-Dist: reportlab; extra == "all"
 Requires-Dist: fastapi; extra == "all"
-Requires-Dist: jmespath; extra == "all"
+Requires-Dist: pymupd; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: cachetools; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: fastapi[all]; extra == "all"
+Requires-Dist: sqlalchemy; extra == "all"
 Requires-Dist: simplejson; extra == "all"
-Requires-Dist: gunicorn; extra == "all"
-Requires-Dist: pymysql; extra == "all"
 Requires-Dist: openai; extra == "all"
-Requires-Dist: jieba; extra == "all"
+Requires-Dist: langchain; extra == "all"
+Requires-Dist: sse_starlette; extra == "all"
+Requires-Dist: dataframe_image; extra == "all"
 Requires-Dist: streamlit; extra == "all"
+Requires-Dist: polars; extra == "all"
+Requires-Dist: redis-py-cluster; extra == "all"
+Requires-Dist: pandas-profiling[notebook]; extra == "all"
+Requires-Dist: missingno; extra == "all"
+Requires-Dist: jmespath; extra == "all"
+Requires-Dist: gunicorn; extra == "all"
+Requires-Dist: faiss-cpu; extra == "all"
 Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: pandas_summary; extra == "all"
-Requires-Dist: cachetools; extra == "all"
-Requires-Dist: filetype; extra == "all"
-Requires-Dist: dataframe_image; extra == "all"
 Requires-Dist: thriftpy2; extra == "all"
-Requires-Dist: sqlalchemy; extra == "all"
-Requires-Dist: fastapi[all]; extra == "all"
-Requires-Dist: thefuck; extra == "all"
-Requires-Dist: pandas-profiling[notebook]; extra == "all"
-Requires-Dist: pretty_errors; extra == "all"
 
 [![Downloads](http://pepy.tech/badge/meutils)](http://pepy.tech/project/meutils)
 
 <h1 align = "center">:rocket: 常用工具类 :facepunch:</h1>
 
 ## Install
 ```bash
```

### Comparing `MeUtils-2024.3.4.13.4.45/MeUtils.egg-info/SOURCES.txt` & `MeUtils-2024.4.11.9.12.58/MeUtils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,15 @@
 meutils/data/_SUCCESS
 meutils/data/__init__.py
 meutils/data/coordinate.py
 meutils/db/README.md
 meutils/db/__init__.py
 meutils/db/mongo.py
 meutils/db/neo4j.py
+meutils/db/redis_db.py
 meutils/decorators/README.md
 meutils/decorators/__ai.py
 meutils/decorators/__init__.py
 meutils/decorators/cache.py
 meutils/decorators/catch.py
 meutils/decorators/common.py
 meutils/decorators/contextmanagers.py
@@ -238,14 +239,17 @@
 meutils/office_automation/__init__.py
 meutils/office_automation/doc.py
 meutils/office_automation/pdf.py
 meutils/office_automation/pdm.py
 meutils/office_automation/pdm_run.py
 meutils/office_automation/投资管理系统O3.2_交易组.pdm
 meutils/office_automation/report/__init__.py
+meutils/oss/__init__.py
+meutils/oss/minio_oss.py
+meutils/oss/minio_utils.py
 meutils/other/__demo.py
 meutils/other/__init__.py
 meutils/other/besttable.py
 meutils/other/crontab.py
 meutils/other/aiomultiprocess/__init__.py
 meutils/other/aiomultiprocess/__version__.py
 meutils/other/aiomultiprocess/core.py
@@ -268,14 +272,16 @@
 meutils/plots/echarts.py
 meutils/plots/embedding_plot.py
 meutils/plots/mecharts.py
 meutils/plots/metrics.py
 meutils/plots/plot_utils.py
 meutils/queues/__init__.py
 meutils/queues/common.py
+meutils/queues/demo.py
+meutils/queues/smooth_queue.py
 meutils/queues/uniform_queue.py
 meutils/request_utils/__init__.py
 meutils/request_utils/a爬虫.py
 meutils/request_utils/crawler.py
 meutils/request_utils/download.py
 meutils/request_utils/results.py
 meutils/request_utils/tiangong.py
@@ -435,21 +441,22 @@
 scripts/py_sh.sh
 scripts/python软连接.sh
 scripts/startup.sh
 scripts/yum.sh
 scripts/模型价格表
 scripts/docker/api-tokens.sh
 scripts/docker/chat.sh
-scripts/docker/copilot.sh
-scripts/docker/copilot_config1.json
-scripts/docker/copilot_config2.json
-scripts/docker/copilot_config3.json
 scripts/docker/docker连接宿主机mysql.md
 scripts/docker/elasticsearch.yml
 scripts/docker/es.sh
+scripts/docker/gpt.sh
 scripts/docker/kuma监控.sh
 scripts/docker/minio.sh
+scripts/docker/nineai-docker-compose.yml
+scripts/docker/ollama.sh
 scripts/docker/oneapi.sh
+scripts/docker/导航页.sh
 scripts/docker/文档智能.sh
 scripts/docker/构建镜像.sh
 scripts/docker/潘多拉.sh
+scripts/docker/逆向.sh
 scripts/docker/镜像自动更新.sh
```

### Comparing `MeUtils-2024.3.4.13.4.45/MeUtils.egg-info/requires.txt` & `MeUtils-2024.4.11.9.12.58/MeUtils.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -35,50 +35,50 @@
 uvicorn
 gunicorn
 sse_starlette
 openai
 langchain
 
 [all]
-polars
+pymysql
 asyncmy
+pandas_summary
+iteration_utilities
+schedule
+pyarrow
 geopy
 pymongo
-missingno
+pretty_errors
+thefuck
+jieba
+filetype
 pymilvus
-redis-py-cluster
-langchain
-jinja2
-sse_starlette
-pymupd
-pyarrow
-seaborn
-iteration_utilities
-faiss-cpu
-schedule
 reportlab
 fastapi
-jmespath
+pymupd
+jinja2
+cachetools
+seaborn
+fastapi[all]
+sqlalchemy
 simplejson
-gunicorn
-pymysql
 openai
-jieba
+langchain
+sse_starlette
+dataframe_image
 streamlit
+polars
+redis-py-cluster
+pandas-profiling[notebook]
+missingno
+jmespath
+gunicorn
+faiss-cpu
 uvicorn
-pandas_summary
-cachetools
-filetype
-dataframe_image
 thriftpy2
-sqlalchemy
-fastapi[all]
-thefuck
-pandas-profiling[notebook]
-pretty_errors
 
 [ann]
 pymilvus
 faiss-cpu
 
 [app]
 fastapi[all]
```

### Comparing `MeUtils-2024.3.4.13.4.45/PKG-INFO` & `MeUtils-2024.4.11.9.12.58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2024.3.4.13.4.45
+Version: 2024.4.11.9.12.58
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
@@ -98,50 +98,50 @@
 Requires-Dist: sqlalchemy; extra == "db"
 Provides-Extra: pd
 Requires-Dist: dataframe_image; extra == "pd"
 Requires-Dist: pandas-profiling[notebook]; extra == "pd"
 Requires-Dist: pandas_summary; extra == "pd"
 Requires-Dist: polars; extra == "pd"
 Provides-Extra: all
-Requires-Dist: polars; extra == "all"
+Requires-Dist: pymysql; extra == "all"
 Requires-Dist: asyncmy; extra == "all"
+Requires-Dist: pandas_summary; extra == "all"
+Requires-Dist: iteration_utilities; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: pyarrow; extra == "all"
 Requires-Dist: geopy; extra == "all"
 Requires-Dist: pymongo; extra == "all"
-Requires-Dist: missingno; extra == "all"
+Requires-Dist: pretty_errors; extra == "all"
+Requires-Dist: thefuck; extra == "all"
+Requires-Dist: jieba; extra == "all"
+Requires-Dist: filetype; extra == "all"
 Requires-Dist: pymilvus; extra == "all"
-Requires-Dist: redis-py-cluster; extra == "all"
-Requires-Dist: langchain; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: sse_starlette; extra == "all"
-Requires-Dist: pymupd; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: iteration_utilities; extra == "all"
-Requires-Dist: faiss-cpu; extra == "all"
-Requires-Dist: schedule; extra == "all"
 Requires-Dist: reportlab; extra == "all"
 Requires-Dist: fastapi; extra == "all"
-Requires-Dist: jmespath; extra == "all"
+Requires-Dist: pymupd; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: cachetools; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: fastapi[all]; extra == "all"
+Requires-Dist: sqlalchemy; extra == "all"
 Requires-Dist: simplejson; extra == "all"
-Requires-Dist: gunicorn; extra == "all"
-Requires-Dist: pymysql; extra == "all"
 Requires-Dist: openai; extra == "all"
-Requires-Dist: jieba; extra == "all"
+Requires-Dist: langchain; extra == "all"
+Requires-Dist: sse_starlette; extra == "all"
+Requires-Dist: dataframe_image; extra == "all"
 Requires-Dist: streamlit; extra == "all"
+Requires-Dist: polars; extra == "all"
+Requires-Dist: redis-py-cluster; extra == "all"
+Requires-Dist: pandas-profiling[notebook]; extra == "all"
+Requires-Dist: missingno; extra == "all"
+Requires-Dist: jmespath; extra == "all"
+Requires-Dist: gunicorn; extra == "all"
+Requires-Dist: faiss-cpu; extra == "all"
 Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: pandas_summary; extra == "all"
-Requires-Dist: cachetools; extra == "all"
-Requires-Dist: filetype; extra == "all"
-Requires-Dist: dataframe_image; extra == "all"
 Requires-Dist: thriftpy2; extra == "all"
-Requires-Dist: sqlalchemy; extra == "all"
-Requires-Dist: fastapi[all]; extra == "all"
-Requires-Dist: thefuck; extra == "all"
-Requires-Dist: pandas-profiling[notebook]; extra == "all"
-Requires-Dist: pretty_errors; extra == "all"
 
 [![Downloads](http://pepy.tech/badge/meutils)](http://pepy.tech/project/meutils)
 
 <h1 align = "center">:rocket: 常用工具类 :facepunch:</h1>
 
 ## Install
 ```bash
```

### Comparing `MeUtils-2024.3.4.13.4.45/README.md` & `MeUtils-2024.4.11.9.12.58/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/TODO.md` & `MeUtils-2024.4.11.9.12.58/TODO.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/clear_githis.sh` & `MeUtils-2024.4.11.9.12.58/clear_githis.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/adjusted_audio1.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/adjusted_audio1.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/asr/__init__.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/asr/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/asr/fast_asr.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/asr/fast_asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/asr/openai_asr.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/asr/openai_asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/asr/subtitle.srt` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/asr/subtitle.srt`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/asr/xunfei_asr.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/asr/xunfei_asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/asr.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/demo.ipynb` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/demo.ipynb`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/example.srt` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/example.srt`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/fast_asr.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/fast_asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/new.srt` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/new.srt`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/subtitles.srt` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/subtitles.srt`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/tts/EdgeTTS.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/tts/EdgeTTS.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # @Project      : AI.  @by PyCharm
 # @File         : tts
 # @Time         : 2023/11/3 15:21
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  : 增加固定时长的生成
+# https://github.com/rany2/edge-tts/blob/master/examples/streaming_with_subtitles.py
 
 import edge_tts
 
 from meutils.pipe import *
 from meutils.decorators.retry import retrying
 
 
@@ -44,15 +45,15 @@
             self,
             text: str,
             role: str = '云希',
             rate: float = 0,
             volume: float = 0,
             filename: Optional[None] = None,
     ):
-        voices = (await edge_tts.VoicesManager.create()).find(**{'ShortName': role}) or [{}]
+        voices = (await edge_tts.VoicesManager.create()).find(**{'ShortName': role}) or [{}]  # todo: 优化
         voice = voices[0].get('ShortName', 'zh-CN-YunxiNeural')
 
         rate = f"{'+' if rate >= 0 else ''}{rate}%"
         volume = f"{'+' if volume >= 0 else ''}{volume}%"
 
         communicate = edge_tts.Communicate(text, voice=voice, rate=rate, volume=volume)  # todo: 文件流
 
@@ -83,30 +84,43 @@
 
         rate = f"{'+' if rate >= 0 else ''}{rate}%"
         volume = f"{'+' if volume >= 0 else ''}{volume}%"
 
         communicate = edge_tts.Communicate(text, voice=voice, rate=rate, volume=volume)
         async for chunk in communicate.stream():  # 构建生成器，流式输出， todo: 字幕结构体
             # {'type': 'WordBoundary', 'offset': 1000000, 'duration': 6750000, 'text': '你好'} # 断句字幕
+            # https://github.com/rany2/edge-tts/blob/master/examples/streaming_with_subtitles.py
             # if chunk.get('type') == 'WordBoundary':
             #     logger.debug(chunk)
             #     continue
-
             if chunk.get('type') == "audio":
                 yield chunk["data"]
 
     @staticmethod
     @lru_cache
     def find_voices(**kwargs: Any):  # @alru_cache
         """https://speech.platform.bing.com/consumer/speech/synthesize/readaloud/voices/list?trustedclienttoken=6A5AA1D4EAFF4E9FB37E23D68491D6F4
             find_voices(**{"Locale": "en-US"})
             find_voices(**{'ShortName': 'zh-CN-XiaoxiaoNeural'})
         """
         return asyncio.run(edge_tts.VoicesManager.create()).find(**kwargs or {"Locale": "zh-CN"})
 
+    async def acreate_for_openai(
+            self,
+            input: str,
+            model: str = 'edge-tts',
+            voice: str = '云希',  # 男声 女声
+            **kwargs
+    ):
+        data = {
+            "text": input,
+            "voice": voice,
+        }
+        return self.stream_acreate(**data)
+
 
 if __name__ == '__main__':
     # print(EdgeTTS().create(['不知道'] * 10))
 
     cls = EdgeTTS()
     # cls.create('不知道')
     # cls.create('不知道')
@@ -118,7 +132,16 @@
     text = """
     陕西省，简称“陕”或“秦”，中华人民共和国省级行政区，省会西安，位于中国内陆腹地，黄河中游，东邻山西、河南，西连宁夏、甘肃，南抵四川、重庆、湖北，北接内蒙古，介于东经105°29′—111°15′，北纬31°42′—39°35′之间，总面积205624.3平方千米。 [1] [5]截至2022年11月，陕西省下辖10个地级市（其中省会西安为副省级市）、31个市辖区、7个县级市、69个县。 [121]截至2022年末，陕西省常住人口3956万人。
     """
 
     # print(cls.find_voices(Locale="zh-CN"))
     for i in async2sync_generator(cls.stream_acreate(input)):
         print(i)
+
+    # EDGE_TTS_DICT = {
+    #     "用英语": "en-US-AriaNeural",
+    #     "用日语": "ja-JP-NanamiNeural",
+    #     "用法语": "fr-BE-CharlineNeural",
+    #     "用韩语": "ko-KR-SunHiNeural",
+    #     "用德语": "de-AT-JonasNeural",
+    #     # add more here
+    # }
```

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/tts/new.srt` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/tts/new.srt`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/tts/openai_tts.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/tts/openai_tts.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,29 @@
 # @Software     : PyCharm
 # @Description  :
 
 from meutils.pipe import *
 from openai import OpenAI
 
 base_url = os.getenv('OPENAI_API_BASE')
-base_url = 'http://0.0.0.0:8000/v1'
+# base_url = 'http://0.0.0.0:8000/v1'
+# base_url='http://154.3.0.117:39009/tts/v1'
 client = OpenAI(
-    api_key=os.getenv('OPENAI_API_KEY'),
-    base_url=base_url,
-    max_retries=3
+    base_url=base_url
 )
 
 # text = """
 # 陕西省，简称“陕”或“秦”，中华人民共和国省级行政区，省会西安，位于中国内陆腹地，黄河中游，东邻山西、河南，西连宁夏、甘肃，南抵四川、重庆、湖北，北接内蒙古，介于东经105°29′—111°15′，北纬31°42′—39°35′之间，总面积205624.3平方千米。 [1] [5]截至2022年11月，陕西省下辖10个地级市（其中省会西安为副省级市）、31个市辖区、7个县级市、69个县。 [121]截至2022年末，陕西省常住人口3956万人。
 # """
 # # text = "你好哇"*20
 # _ = client.audio.speech.create(input=text, model="tts", voice="晓晓")
 # _.stream_to_file("hi.mp3")
 
 
-# from pathlib import Path
-from openai import OpenAI
-
-client = OpenAI(api_key='sk-TZVGYMoCUYrGSddb56F167A54e544e658aD5F1B8D809CfF4', base_url=base_url)
-
-speech_file_path = "speech_xx.mp3"
+speech_file_path = "speech_tts——xxx.mp3"
 response = client.audio.speech.create(
     input="健身需要注意适度和平衡，过度的锻炼可能会导致身体受伤。因此，进行健身活动前，最好先咨询医生或专业的健身教练，制定一个适合自己的健身计划。一般来说，一周内进行150分钟的适度强度的有氧运动，或者75分钟的高强度有氧运动，加上每周两天的肌肉锻炼，就能达到保持健康的目标。",
-    model="tts",
-    voice="晓晓",
+    model="tts-1",
+    voice="alloy",
 )
-
+# logger.debug(response)
 response.stream_to_file(speech_file_path)
```

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/tts/tts_ui.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/tts/tts_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # @Time         : 2023/10/25 18:21
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  : https://www.qianduan.shop/blogs/detail/140
 # https://baijiahao.baidu.com/s?id=1762431177147996323&wfr=spider&for=pc
 # https://github.com/pndurette/gTTS
+# https://github.com/ycyy/edge-tts-webui
 
 from meutils.pipe import *
 import gradio as gr
 import edge_tts
 import asyncio
 import os
```

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/tts.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/tts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_audio/视频合并.sh` & `MeUtils-2024.4.11.9.12.58/meutils/ai_audio/视频合并.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_cv/1.jpg` & `MeUtils-2024.4.11.9.12.58/meutils/ai_cv/1.jpg`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_cv/197.jpg` & `MeUtils-2024.4.11.9.12.58/meutils/ai_cv/197.jpg`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_cv/2.jpg` & `MeUtils-2024.4.11.9.12.58/meutils/ai_cv/2.jpg`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_cv/doc_prompt.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_cv/doc_prompt.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_cv/img.png` & `MeUtils-2024.4.11.9.12.58/meutils/ai_cv/img.png`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_cv/invoice.jpg` & `MeUtils-2024.4.11.9.12.58/meutils/ai_cv/invoice.jpg`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_cv/latex_ocr.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_cv/latex_ocr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_cv/ocr.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_cv/ocr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_cv/ocr_api.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_cv/ocr_api.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_cv/tbl.png` & `MeUtils-2024.4.11.9.12.58/meutils/ai_cv/tbl.png`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_cv/test.png` & `MeUtils-2024.4.11.9.12.58/meutils/ai_cv/test.png`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/SplitSentence.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/SplitSentence.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/Untitled-1(1).py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/Untitled-1(1).py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/_lda.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/_lda.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/_textsplitter/text_split.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/_textsplitter/text_split.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/demo.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/lda.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/lda.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/ner.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/ner.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/text_transformer.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/text_transformer.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/textsplitter.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/textsplitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_nlp/word_segmentation.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_nlp/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_video/avmerge.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_video/avmerge.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_video/avmerge_.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_video/avmerge_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_video/scene_detect.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_video/scene_detect.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_video/test.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_video/test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_video/video.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_video/video.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ai_video/xx.py` & `MeUtils-2024.4.11.9.12.58/meutils/ai_video/xx.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ann/README.md` & `MeUtils-2024.4.11.9.12.58/meutils/ann/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ann/README_gensim.md` & `MeUtils-2024.4.11.9.12.58/meutils/ann/README_gensim.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ann/ann.py` & `MeUtils-2024.4.11.9.12.58/meutils/ann/ann.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ann/ann_faiss.py` & `MeUtils-2024.4.11.9.12.58/meutils/ann/ann_faiss.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ann/ann_gensim.py` & `MeUtils-2024.4.11.9.12.58/meutils/ann/ann_gensim.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ann/ann_inmemory.py` & `MeUtils-2024.4.11.9.12.58/meutils/ann/ann_inmemory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ann/ann_service.py` & `MeUtils-2024.4.11.9.12.58/meutils/ann/ann_service.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ann/ann_v1.py` & `MeUtils-2024.4.11.9.12.58/meutils/ann/ann_v1.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ann/cli.py` & `MeUtils-2024.4.11.9.12.58/meutils/ann/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ann/examples/client.py` & `MeUtils-2024.4.11.9.12.58/meutils/ann/examples/client.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/ann/shake_demo.py` & `MeUtils-2024.4.11.9.12.58/meutils/ann/shake_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/api/common.py` & `MeUtils-2024.4.11.9.12.58/meutils/api/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/api/deeplx.py` & `MeUtils-2024.4.11.9.12.58/meutils/api/deeplx.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/api/qr.png` & `MeUtils-2024.4.11.9.12.58/meutils/api/qr.png`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/async_utils/common.py` & `MeUtils-2024.4.11.9.12.58/meutils/async_utils/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/cache_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/__test.sh` & `MeUtils-2024.4.11.9.12.58/meutils/clis/__test.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/browser.py` & `MeUtils-2024.4.11.9.12.58/meutils/clis/browser.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/cli.py` & `MeUtils-2024.4.11.9.12.58/meutils/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/conf.py` & `MeUtils-2024.4.11.9.12.58/meutils/clis/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/cron.py` & `MeUtils-2024.4.11.9.12.58/meutils/clis/cron.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_13003330042.json` & `MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_13003330042.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_13003872192.json` & `MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_13003872192.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_13852263862.json` & `MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_13852263862.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_13913898681.json` & `MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_13913898681.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_13962978617.json` & `MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_13962978617.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_15251801790.json` & `MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_15251801790.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_15720826383.json` & `MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_15720826383.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_18395563611.json` & `MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_18395563611.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/deepseek_313303303@qq.com.json` & `MeUtils-2024.4.11.9.12.58/meutils/clis/deepseek_313303303@qq.com.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/demo.py` & `MeUtils-2024.4.11.9.12.58/meutils/clis/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/gunicorn.conf.py` & `MeUtils-2024.4.11.9.12.58/meutils/clis/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/kimi_state.json` & `MeUtils-2024.4.11.9.12.58/meutils/clis/kimi_state.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/monitor.py` & `MeUtils-2024.4.11.9.12.58/meutils/clis/monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/nesc.py` & `MeUtils-2024.4.11.9.12.58/meutils/clis/nesc.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/notice.py` & `MeUtils-2024.4.11.9.12.58/meutils/clis/notice.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/clis/server.py` & `MeUtils-2024.4.11.9.12.58/meutils/clis/server.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/cmds/README.md` & `MeUtils-2024.4.11.9.12.58/meutils/cmds/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/cmds/hdfs_cmd.py` & `MeUtils-2024.4.11.9.12.58/meutils/cmds/hdfs_cmd.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/cmds/subprocess_demo.py` & `MeUtils-2024.4.11.9.12.58/meutils/cmds/subprocess_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/coding/find132.py` & `MeUtils-2024.4.11.9.12.58/meutils/coding/find132.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/common.py` & `MeUtils-2024.4.11.9.12.58/meutils/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 
     i = int(current / total * 100)
     s = f"""\r{i}%|{"█" * (i // 5)}|"""
     print(s, end="", flush=True)
     # sys.stdout.flush()
 
 
-wget.download = partial(wget.download, bar=_bar)
+# wget.download = partial(wget.download, bar=_bar)
 
 
 class BaseConfig(BaseModel):
     """基础配置"""
     _path: str = None
 
     @classmethod
```

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/comp_utils/reverse_metric.py` & `MeUtils-2024.4.11.9.12.58/meutils/comp_utils/reverse_metric.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/data/SimHei.ttf` & `MeUtils-2024.4.11.9.12.58/meutils/data/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/data/coordinate.py` & `MeUtils-2024.4.11.9.12.58/meutils/data/coordinate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/date_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/date_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/db/README.md` & `MeUtils-2024.4.11.9.12.58/meutils/db/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/db/__init__.py` & `MeUtils-2024.4.11.9.12.58/meutils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/db/mongo.py` & `MeUtils-2024.4.11.9.12.58/meutils/db/mongo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/db/neo4j.py` & `MeUtils-2024.4.11.9.12.58/meutils/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/__ai.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/__ai.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/__init__.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/cache.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/cache.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/catch.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/catch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/common.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,32 +73,40 @@
     logger.add(sink, enqueue=True, **logkwargs)
     _ = func(*args, **kwargs)
     logger.info(_)
     return func(*args, **kwargs)
 
 
 @contextmanager
-def timer(task="Task"):
+def timer(task="Task", notice_fn: Optional[Callable] = None):
     """https://www.kaggle.com/lopuhin/mercari-golf-0-3875-cv-in-75-loc-1900-s
         # 其他装饰器可学习这种写法
         with timer() as t:
             time.sleep(3)
 
         @timer()
         def f():
             print('sleeping')
             time.sleep(6)
             return 6
+
+
+        from meutils.notice import feishu
+        feishu.send_message
     """
 
     logger.info(f"{task} started")
     s = time.perf_counter()
     yield
     e = time.perf_counter()
-    logger.info(f"{task} done in {e - s:.3f} s")
+    msg = f"{task} done in {e - s:.3f} s"
+    logger.info(msg)  # feishu
+
+    # notice
+    if notice_fn: notice_fn(msg)
 
 
 @contextmanager
 def tryer(task, is_trace=False):
     try:
         yield
     except Exception as e:
@@ -166,32 +174,35 @@
 
 
 @decorator
 def background_task(func, max_workers=1, *args, **kwargs):
     # pool.shutdown(wait=False)  # 不等待
     # pool.shutdown(wait=True)  # 等待
 
+    # with ThreadPoolExecutor(max_workers=max_workers, thread_name_prefix='🐶') as pool: # 失去异步效果
     pool = ThreadPoolExecutor(max_workers=max_workers, thread_name_prefix='🐶')
     future = pool.submit(func, *args, **kwargs)  # pool.map(fun4, ips)
     future.add_done_callback(
         lambda x: logger.error(f"future.exception()\n{traceback.format_exc()}") if future.exception() else None
     )
     # future.add_done_callback()
 
+    # pool.shutdown(wait=False)  # 不等待
+
     return future.running()  # future.done()
 
 
 background = background_task
 
 
 @decorator
 def background_task_plus(func, *args, **kwargs):
     pool = ThreadPoolExecutor(max_workers=1, thread_name_prefix='🐶')
     future = pool.submit(func, *args, **kwargs)  # pool.map(fun4, ips)
-    future.add_done_callback(lambda x: logger.error(future.exception()) if future.exception() else None)
+    future.add_done_callback(lambda x: logger.error(f"{future.exception()}") if future.exception() else None)
     # 详细错误 traceback.format_exc()
     return future.running()  # future.done()
 
 
 # @backend
 @decorator
 def scheduler(func, scheduler_=schedule.every(2).seconds, stop_func=lambda: False, *args, **kwargs):
@@ -394,14 +405,14 @@
     #
     #
     # f()
     # while 1:
     #     pass
 
     def f():
-        return  1/0
+        return 1 / 0
         # return 1
 
 
     with tryer('try'):
         a = f()
     print(a)
```

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/contextmanagers.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/decorator.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/decorator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/decorator_demo.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/decorator_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/demo.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/fastapi_decorator.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/fastapi_decorator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/feishu.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/retry.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/scheduler.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/decorators/schedulers.py` & `MeUtils-2024.4.11.9.12.58/meutils/decorators/schedulers.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/dist_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/docarray_utils/demo_es.py` & `MeUtils-2024.4.11.9.12.58/meutils/docarray_utils/demo_es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/docarray_utils/demo_hnsw.py` & `MeUtils-2024.4.11.9.12.58/meutils/docarray_utils/demo_hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/docarray_utils/in_memory.py` & `MeUtils-2024.4.11.9.12.58/meutils/docarray_utils/in_memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/docarray_utils/改造下hnsw.py` & `MeUtils-2024.4.11.9.12.58/meutils/docarray_utils/改造下hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/easy_search/es.py` & `MeUtils-2024.4.11.9.12.58/meutils/easy_search/es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/PDF抽取.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/PDF抽取.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/common.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/__main__.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/__main__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/filetype.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/filetype.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/helpers.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/helpers.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/match.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/__init__.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/archive.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/archive.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/audio.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/audio.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/base.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/document.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/document.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/font.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/font.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/image.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/isobmff.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/isobmff.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/types/video.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/types/video.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/filetype/utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/filetype/utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/pdf.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/pdf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/fileparser/表格抽取.py` & `MeUtils-2024.4.11.9.12.58/meutils/fileparser/表格抽取.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/hash_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/import_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/import_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/init/evn.py` & `MeUtils-2024.4.11.9.12.58/meutils/init/evn.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/init/oo.py` & `MeUtils-2024.4.11.9.12.58/meutils/init/oo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/io/__init__.py` & `MeUtils-2024.4.11.9.12.58/meutils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/io/image.py` & `MeUtils-2024.4.11.9.12.58/meutils/io/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,21 @@
 def image_to_base64(image_path, for_image_url: bool = True):
     _ = base64.b64encode(Path(image_path).read_bytes()).decode('utf-8')
     if for_image_url:
         _ = f"data:image/jpeg;base64,{_}"
     return _
 
 
+def file_to_base64(image_path, for_image_url: bool = True):
+    _ = base64.b64encode(Path(image_path).read_bytes()).decode('utf-8')
+    if for_image_url:
+        _ = f"data:image/jpeg;base64,{_}"
+    return _
+
+
 # alias
 base64_to_img = base64_to_image
 
 if __name__ == '__main__':
     url = "https://i1.mifile.cn/f/i/mioffice/img/slogan_5.png?1604383825042"
 
     print(image_read(url))
```

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/io/img.png` & `MeUtils-2024.4.11.9.12.58/meutils/io/img.png`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/io/minio_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/io/minio_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/io/tf_io.py` & `MeUtils-2024.4.11.9.12.58/meutils/io/tf_io.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/jinja_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/logging/handlers.py` & `MeUtils-2024.4.11.9.12.58/meutils/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/logging/log_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/logging/log_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/logging/logger.py` & `MeUtils-2024.4.11.9.12.58/meutils/logging/logger.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/notice/emails.py` & `MeUtils-2024.4.11.9.12.58/meutils/notice/emails.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/notice/feishu.py` & `MeUtils-2024.4.11.9.12.58/meutils/notice/feishu.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,9 +82,9 @@
     # @catch(task_name='这是一个任务名')
     # def f():
     #     time.sleep(3)
     #     1 / 0
     #
     #
     # f()
-
-    send_message("ERROR", title='GitHub Copilot Chat Error')
+    with timer():
+        send_message("ERROR", title='GitHub Copilot Chat Error')
```

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/notice/file_post.py` & `MeUtils-2024.4.11.9.12.58/meutils/notice/file_post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/notice/img.png` & `MeUtils-2024.4.11.9.12.58/meutils/notice/img.png`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/notice/load_emailfile - 副本.py` & `MeUtils-2024.4.11.9.12.58/meutils/notice/load_emailfile - 副本.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/notice/wechat.py` & `MeUtils-2024.4.11.9.12.58/meutils/notice/wechat.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,37 +77,41 @@
     # # 公网测试
     # corp_id = 'wwc18433f3075302e4'
     # secret = 'iL_8JXBoB5vFITCcOk2-EvP6TcOnVCjZI1LRw8vidtEE'
     # agent_id = '1000002'
     # api_base_url = None
     #
     # # 内外AI：
-    # corp_id = 'ww3c6024bb94ecef59'
-    # secret = 'empKNMx-RSgd4tK6uzVA56qCl1QY6eErRdSb7Hr5vyQQ'
-    # agent_id = '1000041'
-    # api_base_url = 'https://qywxlocal.nesc.cn:7443/cgi-bin/'
+    corp_id = 'ww3c6024bb94ecef59'
+    secret = 'empKNMx-RSgd4tK6uzVA56qCl1QY6eErRdSb7Hr5vyQ'
+    agent_id = '1000041'
+    api_base_url = 'https://qywxlocal.nesc.cn:7443/cgi-bin/'
     # # api_base_url = 'https://192.18.27.53:80/cgi-bin/'
     #
-    # wc = WeChatClient(corp_id, secret, api_base_url)
-    # name = '联盟微信群测试1111111111111111xxxxxxxxxxxx'
-    # chat_id = wc.name2id(name)
-    # # wc.appchat.create(chat_id=chat_id, name=name, owner='YuanJie', user_list=['YuanJie', 'yayoYan'])
-    # # _ = wc.appchat.create(chat_id=chat_id, name=name, owner=7683, user_list=[7683, 7689])
+    wc = WeChatClient(corp_id, secret, api_base_url)
+    name = '常态化巡查通知'
+    chat_id = wc.name2id(name)
+    # wc.appchat.create(chat_id=chat_id, name=name, owner='YuanJie', user_list=['YuanJie', 'yayoYan'])
+    # _ = wc.appchat.create(chat_id=chat_id, name=name, owner=7683, user_list=[7683, 9147])
     # # 7560 离职：wechatpy.exceptions.WeChatClientException: Error code: 60111, message: userid not found [logid:]
     #
     # # wc.appchat.create(chat_id=chat_id, name=name, owner=7683, user_list=[7683, 7689])
     # wc.appchat.send_text(chat_id, f"{name}#chat_id: {chat_id}\n{_}")
+    # wc.appchat.send_text(chat_id, f"{name}#chat_id: {chat_id}\n{_}")
+    wc.appchat.send_text(chat_id, '# 我是个机器人🤖')
+
+
     # wc.appchat.update(chat_id, add_user_list=[7838])
     # # wc.appchat.send(chat_id, 'textcard', **{'title': 'Title', 'description': 'description', 'url': 'http://'})
     # # wc.appchat.send_text(chat_id, '# 我是个机器人🤖')
     # # wc.appchat.send(chat_id, 'markdown', content='# 我是个机器人🤖') # 不支持
 
-    corp_id, secret = os.getenv("D_CORP_SECRET").split('|')
-    wc = _WeChatClient(corp_id, secret)
-    name = '🔥火力全开机器人测试群'
+    # corp_id, secret = os.getenv("D_CORP_SECRET").split('|')
+    # wc = _WeChatClient(corp_id, secret)
+    # name = '常态化巡查通知'
     # chat_id = wc.name2id(name)
-    chat_id = 10000
-    _ = wc.appchat.create(chat_id=chat_id, name=name,
-                          owner='Betterme',
-                          # user_list=[7683, 7689]
-                          )
-    wc.appchat.send_text(chat_id, f"{name}#chat_id: {chat_id}\n{_}")
+    # # chat_id = 10000
+    # _ = wc.appchat.create(chat_id=chat_id, name=name,
+    #                       owner='Betterme',
+    #                       # user_list=[7683, 7689]
+    #                       )
+    # wc.appchat.send_text(chat_id, f"{name}#chat_id: {chat_id}\n{_}")
```

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/notice/wechat_.py` & `MeUtils-2024.4.11.9.12.58/meutils/notice/wechat_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/notice/wecom.py` & `MeUtils-2024.4.11.9.12.58/meutils/notice/wecom.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/notice/weekmeet.py` & `MeUtils-2024.4.11.9.12.58/meutils/notice/weekmeet.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/np_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/np_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/office_automation/pdf.py` & `MeUtils-2024.4.11.9.12.58/meutils/office_automation/pdf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/office_automation/pdm.py` & `MeUtils-2024.4.11.9.12.58/meutils/office_automation/pdm.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/office_automation/pdm_run.py` & `MeUtils-2024.4.11.9.12.58/meutils/office_automation/pdm_run.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/office_automation/投资管理系统O3.2_交易组.pdm` & `MeUtils-2024.4.11.9.12.58/meutils/office_automation/投资管理系统O3.2_交易组.pdm`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/other/__demo.py` & `MeUtils-2024.4.11.9.12.58/meutils/other/__demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/other/aiomultiprocess/core.py` & `MeUtils-2024.4.11.9.12.58/meutils/other/aiomultiprocess/core.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/other/aiomultiprocess/pool.py` & `MeUtils-2024.4.11.9.12.58/meutils/other/aiomultiprocess/pool.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/other/aiomultiprocess/scheduler.py` & `MeUtils-2024.4.11.9.12.58/meutils/other/aiomultiprocess/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/other/aiomultiprocess/types.py` & `MeUtils-2024.4.11.9.12.58/meutils/other/aiomultiprocess/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/other/besttable.py` & `MeUtils-2024.4.11.9.12.58/meutils/other/besttable.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/other/crontab.py` & `MeUtils-2024.4.11.9.12.58/meutils/other/crontab.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/pandas_utils/opt.py` & `MeUtils-2024.4.11.9.12.58/meutils/pandas_utils/opt.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/pandas_utils/pd_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/pandas_utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/path_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/path_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/pd_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/pipe.py` & `MeUtils-2024.4.11.9.12.58/meutils/pipe.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/playwright_utils/common.py` & `MeUtils-2024.4.11.9.12.58/meutils/playwright_utils/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/playwright_utils/kimi1_cookies.json` & `MeUtils-2024.4.11.9.12.58/meutils/playwright_utils/kimi1_cookies.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/playwright_utils/kimi2_cookies.json` & `MeUtils-2024.4.11.9.12.58/meutils/playwright_utils/kimi2_cookies.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/playwright_utils/kimi_cookies.json` & `MeUtils-2024.4.11.9.12.58/meutils/playwright_utils/kimi_cookies.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/playwright_utils/reload.py` & `MeUtils-2024.4.11.9.12.58/meutils/playwright_utils/reload.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/plots/common.py` & `MeUtils-2024.4.11.9.12.58/meutils/plots/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/plots/demo.py` & `MeUtils-2024.4.11.9.12.58/meutils/plots/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/plots/echarts.py` & `MeUtils-2024.4.11.9.12.58/meutils/plots/echarts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/plots/embedding_plot.py` & `MeUtils-2024.4.11.9.12.58/meutils/plots/embedding_plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/plots/mecharts.py` & `MeUtils-2024.4.11.9.12.58/meutils/plots/mecharts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/plots/metrics.py` & `MeUtils-2024.4.11.9.12.58/meutils/plots/metrics.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/plots/plot_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/queues/common.py` & `MeUtils-2024.4.11.9.12.58/meutils/queues/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/queues/uniform_queue.py` & `MeUtils-2024.4.11.9.12.58/meutils/queues/uniform_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 from queue import Queue, Empty
 
 
 class UniformQueue(object):
 
     def __init__(self, generator: Generator):
         self.queue = Queue()
+
         self.producer(generator)
 
     def smooth(self, interval: float = 0.05, timeout: float = 30, break_fn: Callable = lambda item: item is None):
         return self.consumer(interval, timeout, break_fn)
 
-    def consumer(self, interval: float = 0.05, timeout: float = 30, break_fn: Callable = lambda item: item is None):
+    def consumer(self, interval: float = 0.066, timeout: float = 10, break_fn: Callable = lambda item: item is None):
         """
 
         :param interval:
         :param timeout:
         :param break_fn: 默认item为None跳出
             lambda line: line.choices[0].finish_reason == 'stop'
         :return:
```

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/request_utils/__init__.py` & `MeUtils-2024.4.11.9.12.58/meutils/request_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/request_utils/a爬虫.py` & `MeUtils-2024.4.11.9.12.58/meutils/request_utils/a爬虫.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/request_utils/crawler.py` & `MeUtils-2024.4.11.9.12.58/meutils/request_utils/crawler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/request_utils/download.py` & `MeUtils-2024.4.11.9.12.58/meutils/request_utils/download.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/request_utils/results.py` & `MeUtils-2024.4.11.9.12.58/meutils/request_utils/results.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/request_utils/tiangong.py` & `MeUtils-2024.4.11.9.12.58/meutils/request_utils/tiangong.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/request_utils/公网ip.py` & `MeUtils-2024.4.11.9.12.58/meutils/request_utils/公网ip.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/request_utils/爬虫.py` & `MeUtils-2024.4.11.9.12.58/meutils/request_utils/爬虫.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/_fastapi.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/_fastapi.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/celery/__init__.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/celery/_conf.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/celery/_conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/celery/_demo.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/celery/_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/celery/router.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/celery/router.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/celery/tasks.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/__demo/异步任务.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/__demo/异步任务.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/common.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/exceptions/validation_error.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/exceptions/validation_error.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/gunicorn.conf.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/routers/_test.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/routers/_test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/routers/scheduler.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/routers/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/routers/shutdown.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/routers/shutdown.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/routers/spider.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/routers/spider.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/fastapi/utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/fastapi/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,17 +4,41 @@
 # @File         : utils
 # @Time         : 2023/11/28 16:51
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  : 
 
-from starlette.requests import Request
 from meutils.pipe import *
 
+from starlette.requests import Request
+from fastapi.security import HTTPBearer, HTTPAuthorizationCredentials
+
+from fastapi import APIRouter, File, UploadFile, Query, Form, BackgroundTasks, Depends, HTTPException as _HTTPException, \
+    Request, status
+
+
+class HTTPException(_HTTPException):
+    message: str = ""
+    type: str = "error"
+    param: Optional[Any] = None
+    code: Optional[Any] = None
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+        self.detail = self.detail or {
+            "error": {
+                "message": self.message,
+                "type": self.type,
+                "param": self.param,
+                "code": self.code or self.status_code,
+            }
+        }
+
 
 def get_ipaddr(request: Request) -> str:
     """
     Returns the ip address for the current request (or 127.0.0.1 if none found)
      based on the X-Forwarded-For headers.
      Note that a more robust method for determining IP address of the client is
      provided by uvicorn's ProxyHeadersMiddleware.
@@ -47,7 +71,30 @@
     """
     from slowapi.errors import RateLimitExceeded
     from slowapi import Limiter, _rate_limit_exceeded_handler
     from slowapi.util import get_remote_address
 
     limiter = Limiter(key_func=get_remote_address)
     return limiter.limit(limit_value=limit_value, error_message=error_message, **kwargs)
+
+
+def check_api_key(auth: HTTPAuthorizationCredentials):
+    api_key = auth and auth.credentials or None
+    if api_key is None:
+        detail = {
+            "error": {
+                "message": "invalid_api_key",
+                "type": "invalid_request_error",
+                "param": None,
+                "code": None,
+            }
+        }
+        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail=detail)
+
+
+if __name__ == '__main__':
+    d = {
+        "error": {
+            "message": "当前分组 chatfire 下对于模型 ERNIE-Bot 无可用渠道 (request id: 20240314180638675032749TVFiqyF1)",
+            "type": "new_api_error"
+        }
+    }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/gui/bar.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/gui/bar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/gui/demo.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/gui/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/client.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/client.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/flow.svg` & `MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/flow.svg`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/s.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/s.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/s2.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/s2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/server.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/server.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/jina/__demo/test.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/jina/__demo/test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/jina/executors/SentenceEncoder.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/jina/executors/SentenceEncoder.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/jina/executors/SentenceEncoder_.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/jina/executors/SentenceEncoder_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/jina/executors/__init__.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/jina/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/jina/executors/base.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/jina/executors/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/jina/nlp_serving/word_segmentation.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/jina/nlp_serving/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/_test.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/_test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/chat_latex.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/chat_latex.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/common.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     """
     from streamlit_extras.streaming_write import write
 
     if fhook: fhook()
 
     with st.chat_message(name=message.name, avatar=message.avatar):
         written_content = write(message.generator, unsafe_allow_html=unsafe_allow_html, **kwargs)
-        message.generator = written_content | xfilter | xjoin('')
+        message.generator = written_content | xfilter(lambda x: x is None) | xjoin('')
 
     if bhook: bhook()
 
     st.session_state.messages = st.session_state.get('messages', [])
     if is_history:
         st.session_state.messages.append(message)
```

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/demo.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/streamlit/ocr.png` & `MeUtils-2024.4.11.9.12.58/meutils/serving/streamlit/ocr.png`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/webui/.streamlit/_config.toml` & `MeUtils-2024.4.11.9.12.58/meutils/serving/webui/.streamlit/_config.toml`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/webui/_2_词性标注与实体识别.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/webui/_2_词性标注与实体识别.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/webui/pages/_1_分词.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/webui/pages/_1_分词.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/webui/pages/_2_词性标注与实体识别.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/webui/pages/_2_词性标注与实体识别.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/serving/webui/pages/_3_文本匹配.py` & `MeUtils-2024.4.11.9.12.58/meutils/serving/webui/pages/_3_文本匹配.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/sftp.py` & `MeUtils-2024.4.11.9.12.58/meutils/sftp.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/sk_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/sk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/smooth_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/smooth_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/spark/__init__.py` & `MeUtils-2024.4.11.9.12.58/meutils/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/str_utils/Translator.py` & `MeUtils-2024.4.11.9.12.58/meutils/str_utils/Translator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/str_utils/__init__.py` & `MeUtils-2024.4.11.9.12.58/meutils/str_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/str_utils/__translater/tencent.py` & `MeUtils-2024.4.11.9.12.58/meutils/str_utils/__translater/tencent.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/str_utils/__translater/translater.py` & `MeUtils-2024.4.11.9.12.58/meutils/str_utils/__translater/translater.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/str_utils/__translater/youdao.py` & `MeUtils-2024.4.11.9.12.58/meutils/str_utils/__translater/youdao.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/str_utils/json_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/str_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/str_utils/regular_expression.py` & `MeUtils-2024.4.11.9.12.58/meutils/str_utils/regular_expression.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/tasks/common.py` & `MeUtils-2024.4.11.9.12.58/meutils/tasks/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/demo.j2` & `MeUtils-2024.4.11.9.12.58/meutils/templates/demo.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/demo.py` & `MeUtils-2024.4.11.9.12.58/meutils/templates/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/demox.py` & `MeUtils-2024.4.11.9.12.58/meutils/templates/demox.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/df_html.j2` & `MeUtils-2024.4.11.9.12.58/meutils/templates/df_html.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/dockerfiles/docker_build_push.py` & `MeUtils-2024.4.11.9.12.58/meutils/templates/dockerfiles/docker_build_push.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/hegui.py` & `MeUtils-2024.4.11.9.12.58/meutils/templates/hegui.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/markmap.html` & `MeUtils-2024.4.11.9.12.58/meutils/templates/markmap.html`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/cookiecutter.json` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py` & `MeUtils-2024.4.11.9.12.58/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/tpl.docx` & `MeUtils-2024.4.11.9.12.58/meutils/templates/tpl.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/x.html` & `MeUtils-2024.4.11.9.12.58/meutils/templates/x.html`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/templates/合规日报模板.docx` & `MeUtils-2024.4.11.9.12.58/meutils/templates/合规日报模板.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/todo.py` & `MeUtils-2024.4.11.9.12.58/meutils/todo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/tools/cprint.py` & `MeUtils-2024.4.11.9.12.58/meutils/tools/cprint.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/tools/machine_monitor.py` & `MeUtils-2024.4.11.9.12.58/meutils/tools/machine_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/tools/monitor.yml` & `MeUtils-2024.4.11.9.12.58/meutils/tools/monitor.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/tools/seize.py` & `MeUtils-2024.4.11.9.12.58/meutils/tools/seize.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/tools/service_monitor.py` & `MeUtils-2024.4.11.9.12.58/meutils/tools/service_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/types.py` & `MeUtils-2024.4.11.9.12.58/meutils/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/meutils/zk_utils.py` & `MeUtils-2024.4.11.9.12.58/meutils/zk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/pypi.sh` & `MeUtils-2024.4.11.9.12.58/pypi.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/scripts/docker/api-tokens.sh` & `MeUtils-2024.4.11.9.12.58/scripts/docker/api-tokens.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/scripts/docker/chat.sh` & `MeUtils-2024.4.11.9.12.58/scripts/docker/chat.sh`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 
 docker run -d -p 39777:3210 \
   -e OPENAI_API_KEY=sk-xxxx \
   -e OPENAI_PROXY_URL=https://api.chatllm.vip/v1 \
   -e ACCESS_CODE=chatllm \
   lobehub/lobe-chat
 
+#
+docker run -d -p 39777:3210 \
+  -e OPENAI_API_KEY=sk-xxxx \
+  -e OPENAI_PROXY_URL=https://api.chatllm.vip/v1 \
+  -e ACCESS_CODE=chatllm \
+  yangclivia/lobe-chat
+
 # https://github.com/ChatGPTNextWeb/ChatGPT-Next-Web
 docker run --name chatgpt-next-web \
   --restart=always \
   -d -p 39771:3000 \
   -e BASE_URL=http://api.chatllm.vip \
   -e CUSTOM_MODELS=+gemini-pro,+kimi,+kimi-32k,+kimi-128k,+kimi-256k,+deepseek,-gpt-3.5-turbo-0301,-gpt-3.5-turbo-0613,-gpt-3.5-turbo-16k-0613,-gpt-4-0314,-gpt-4-0613,-gpt-4-32k-0314,-gpt-4-32k-0613 \
   yidadaa/chatgpt-next-web
@@ -44,8 +51,50 @@
   -e R2_ACCOUNT_ID=d6746affe0c6f033dc6e8aa472d22d87 \
   -e R2_ACCESS_KEY_ID=9b87ee7be319fc4d1a8fe07881dccdbb \
   -e R2_SECRET_ACCESS_KEY=49b86992d3ab45a6eb538fc316fffee964c551f95c1a0a88576ef80b10e93863 \
   -e R2_BUCKET=chatfire \
   -e CUSTOM_MODELS=-all,+gpt-4-all,+dall-e-3,+gpt-4-vision-preview,+gpt-3.5-turbo,+gpt-4-turbo-preview,+deepseek-chat,+deepseek-coder,+kimi \
   gosuto/chatgpt-next-web-langchain
 
+docker run --name chatfire \
+  -p 39999:3000 \
+  -e OPENAI_API_KEY=sk-xxxxx \
+  -e CUSTOM_MODELS="kimi-all,glm-4-all,gpt-4-all" \
+  ydlhero/chatgpt-web-midjourney-proxy
+
+# HIDE_SERVER
+docker run --name chatgpt-web-midjourney-proxy -d \
+  -p 6015:3002 \
+  -v /www/data/uploads:/app/uploads \
+  -e OPENAI_API_BASE_URL=https://api.chatllm.vip \
+  -e OPENAI_API_KEY=sk-xxxxx \
+  -e API_UPLOADER=1 \
+  -e CUSTOM_MODELS=kimi-all,glm-4-all \
+  ydlhero/chatgpt-web-midjourney-proxy
+
+# http://154.3.0.117:6015/openapi/v1/upload
+
+docker run -d -p 3210:3210 \
+  -e OPENAI_API_KEY=sk-xxxx \
+  -e OPENAI_PROXY_URL=https://api.oaifree.com/v1 \
+  -e ACCESS_CODE=lobe66 \
+  -e CUSTOM_MODELS=-gpt-4,-gpt-4-32k,-gpt-3.5-turbo-16k,gpt-3.5-turbo-1106=gpt-3.5-turbo-16k,gpt-4-0125-preview=gpt-4-turbo,gpt-4-vision-preview=gpt-4-vision,gpt-4-mobile=gpt-4-mobile \
+  --name lobe-chat \
+  lobehub/lobe-chat
 
+#https://github.com/Deeptrain-Community/chatnio
+docker run -d --name chatnio \
+  --network host \
+  -p 8000:8094 \
+  -v ~/config:/config \
+  -v ~/logs:/logs \
+  -v ~/storage:/storage \
+  -e MYSQL_HOST=localhost \
+  -e MYSQL_PORT=3306 \
+  -e MYSQL_DB=chatnio \
+  -e MYSQL_USER=root \
+  -e MYSQL_PASSWORD=chatnio123456 \
+  -e REDIS_HOST=localhost \
+  -e REDIS_PORT=6379 \
+  -e SECRET=secret \
+  -e SERVE_STATIC=true \
+  programzmh/chatnio:latest
```

### Comparing `MeUtils-2024.3.4.13.4.45/scripts/docker/docker连接宿主机mysql.md` & `MeUtils-2024.4.11.9.12.58/scripts/docker/docker连接宿主机mysql.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/scripts/docker/es.sh` & `MeUtils-2024.4.11.9.12.58/scripts/docker/es.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/scripts/docker/minio.sh` & `MeUtils-2024.4.11.9.12.58/scripts/docker/minio.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/scripts/docker/oneapi.sh` & `MeUtils-2024.4.11.9.12.58/scripts/docker/oneapi.sh`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # @Author       : betterme
 # @Email        : 313303303@qq.com
 # @Software     : PyCharm
 # @Description  : https://mp.weixin.qq.com/s/uOcaKQkNROTXqFuKA3hznQ
 """
 mysql -u root -p chatllmchatllm
 
-GRANT ALL PRIVILEGES ON oneapi.* TO 'root'@'%' IDENTIFIED BY 'fiaAcdm8SwiPm6wH';
+GRANT ALL PRIVILEGES ON oneapi.* TO 'root'@'%' IDENTIFIED BY 'chatllmchatllm';
 FLUSH PRIVILEGES;
 
 GRANT ALL PRIVILEGES ON gpt3.* TO 'root'@'%' IDENTIFIED BY 'chatllmchatllm';
 FLUSH PRIVILEGES;
 
 GRANT ALL PRIVILEGES ON gpt4.* TO 'root'@'%' IDENTIFIED BY 'chatllmchatllm';
 FLUSH PRIVILEGES;
@@ -92,45 +92,61 @@
 export NAME=gpt4
 docker run --name $NAME \
   -d --restart always \
   -p 4444:3000 \
   --add-host="host.docker.internal:host-gateway" \
   -e SQL_DSN="root:chatllmchatllm@tcp(host.docker.internal:3306)/$NAME" -e TZ=Asia/Shanghai \
   -v /root/data/$NAME:/data \
-  calciumion/new-api:latest
+  calciumion/new-api:v0.2.0.3-alpha.2
 
 # 主站点：负载均衡
-docker run --name api \
+docker run --name master-api \
   -d --restart always \
   -p 38888:3000 \
   -e TZ=Asia/Shanghai \
   -e SESSION_SECRET=chatfire \
   -e GLOBAL_API_RATE_LIMIT=30000 -e GLOBAL_WEB_RATE_LIMIT=300 -e RELAY_TIMEOUT=300 \
   -e MEMORY_CACHE_ENABLED=true \
   -e SQL_DSN="root:chatllmchatllm@tcp(111.173.117.175:3306)/oneapi" -e SYNC_FREQUENCY=60 \
-  -v /root/data/aiapi:/data \
-  calciumion/new-api:latest
+  -e REDIS_CONN_STRING="redis://default:chatfirechatfire@111.173.117.175:6379" \
+  -v /www/data/newapi:/data \
+  calciumion/new-api
 
 ## todo: REDIS_CONN_STRING：设置之后将使用 Redis 作为缓存使用。
-docker run --name api \
+# 美国节点
+docker run --name slave-api \
   -d --restart always \
-  -p 6666:3000 \
+  -p 36666:3000 \
   -e TZ=Asia/Shanghai \
   -e SESSION_SECRET=chatfire -e NODE_TYPE=slave \
   -e GLOBAL_API_RATE_LIMIT=30000 -e GLOBAL_WEB_RATE_LIMIT=300 -e RELAY_TIMEOUT=300 \
   -e MEMORY_CACHE_ENABLED=true \
   -e SQL_DSN="root:chatllmchatllm@tcp(111.173.117.175:3306)/oneapi" -e SYNC_FREQUENCY=60 \
-  --add-host="host.docker.internal:host-gateway" \
-  -e REDIS_CONN_STRING="redis://host.docker.internal:6379" \
-  -v /root/data/aiapi:/data \
-  calciumion/new-api:latest
+  -e REDIS_CONN_STRING="redis://default:chatfirechatfire@154.44.8.149:6379" \
+  -v /www/data/newapi:/data \
+  calciumion/new-api
 
+# 香港节点
 docker run --name slave-api \
   -d --restart always \
-  -p 6666:3000 \
+  -p 36666:3000 \
   -e TZ=Asia/Shanghai \
   -e SESSION_SECRET=chatfire -e NODE_TYPE=slave \
   -e GLOBAL_API_RATE_LIMIT=30000 -e GLOBAL_WEB_RATE_LIMIT=300 -e RELAY_TIMEOUT=300 \
   -e MEMORY_CACHE_ENABLED=true \
   -e SQL_DSN="root:chatllmchatllm@tcp(111.173.117.175:3306)/oneapi" -e SYNC_FREQUENCY=60 \
-  -v /root/data/aiapi:/data \
-  calciumion/new-api:latest
+  -e REDIS_CONN_STRING="redis://default:chatfirechatfire@154.3.0.117:6379" \
+  -v /www/data/newapi:/data \
+  calciumion/new-api
+
+##### new one 结合体
+docker run --name oneapi \
+  -d --restart always \
+  -p 8888:3000 \
+  -e TZ=Asia/Shanghai \
+  -e SESSION_SECRET=chatfire \
+  -e GLOBAL_API_RATE_LIMIT=30000 -e GLOBAL_WEB_RATE_LIMIT=300 -e RELAY_TIMEOUT=300 \
+  -e MEMORY_CACHE_ENABLED=true \
+  -e SQL_DSN="root:chatllmchatllm@tcp(154.44.8.149:3306)/oneapi" -e SYNC_FREQUENCY=60 \
+  -e REDIS_CONN_STRING="redis://default:chatfirechatfire@154.44.8.149:6379" \
+  -v /www/data/chat-api:/data \
+  justsong/one-api
```

### Comparing `MeUtils-2024.3.4.13.4.45/scripts/github代理.sh` & `MeUtils-2024.4.11.9.12.58/scripts/github代理.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/scripts/startup.sh` & `MeUtils-2024.4.11.9.12.58/scripts/startup.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.3.4.13.4.45/setup.py` & `MeUtils-2024.4.11.9.12.58/setup.py`

 * *Files identical despite different names*

