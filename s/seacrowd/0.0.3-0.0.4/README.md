# Comparing `tmp/seacrowd-0.0.3.tar.gz` & `tmp/seacrowd-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seacrowd-0.0.3.tar", last modified: Thu Apr 11 08:42:34 2024, max compression
+gzip compressed data, was "seacrowd-0.0.4.tar", last modified: Thu Apr 11 09:04:26 2024, max compression
```

## Comparing `seacrowd-0.0.3.tar` & `seacrowd-0.0.4.tar`

### file list

```diff
@@ -1,980 +1,980 @@
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:34.510025 seacrowd-0.0.3/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11357 2024-04-04 06:00:44.000000 seacrowd-0.0.3/LICENSE
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-11 08:42:34.506183 seacrowd-0.0.3/PKG-INFO
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5757 2024-04-04 06:00:44.000000 seacrowd-0.0.3/README.md
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:26.990161 seacrowd-0.0.3/seacrowd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      251 2024-04-11 08:41:52.000000 seacrowd-0.0.3/seacrowd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    40451 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/config_helper.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.058292 seacrowd-0.0.3/seacrowd/sea_datasets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/__init__.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.073977 seacrowd-0.0.3/seacrowd/sea_datasets/abui_wordnet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/abui_wordnet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5277 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.096696 seacrowd-0.0.3/seacrowd/sea_datasets/alt_burmese_treebank/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/alt_burmese_treebank/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5692 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.113962 seacrowd-0.0.3/seacrowd/sea_datasets/alt_burmese_treebank/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/alt_burmese_treebank/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2661 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.131010 seacrowd-0.0.3/seacrowd/sea_datasets/ara_close/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ara_close/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8227 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ara_close/ara_close.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.149092 seacrowd-0.0.3/seacrowd/sea_datasets/asr_sindodusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/asr_sindodusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7231 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.167448 seacrowd-0.0.3/seacrowd/sea_datasets/asr_smaldusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/asr_smaldusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7305 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.187746 seacrowd-0.0.3/seacrowd/sea_datasets/asr_stidusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/asr_stidusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6979 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.207589 seacrowd-0.0.3/seacrowd/sea_datasets/audio_keyword_spotting/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/audio_keyword_spotting/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7860 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.227031 seacrowd-0.0.3/seacrowd/sea_datasets/aya_dataset/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/aya_dataset/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7482 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/aya_dataset/aya_dataset.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.245211 seacrowd-0.0.3/seacrowd/sea_datasets/barasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/barasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7224 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/barasa/barasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.262873 seacrowd-0.0.3/seacrowd/sea_datasets/beaye_lexicon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/beaye_lexicon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4357 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.282152 seacrowd-0.0.3/seacrowd/sea_datasets/belebele/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/belebele/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8610 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/belebele/belebele.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.300654 seacrowd-0.0.3/seacrowd/sea_datasets/bible_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bible_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6790 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bible_en_id/bible_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.323393 seacrowd-0.0.3/seacrowd/sea_datasets/bible_jv_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bible_jv_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6856 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.344100 seacrowd-0.0.3/seacrowd/sea_datasets/bible_su_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bible_su_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6632 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bible_su_id/bible_su_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.368107 seacrowd-0.0.3/seacrowd/sea_datasets/bioner_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bioner_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6108 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bioner_id/bioner_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.389548 seacrowd-0.0.3/seacrowd/sea_datasets/bloom_captioning/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bloom_captioning/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8518 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.412349 seacrowd-0.0.3/seacrowd/sea_datasets/bloom_lm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bloom_lm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8430 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bloom_lm/bloom_lm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.431889 seacrowd-0.0.3/seacrowd/sea_datasets/bloom_speech/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bloom_speech/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6922 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bloom_speech/bloom_speech.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.448826 seacrowd-0.0.3/seacrowd/sea_datasets/bloom_vist/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bloom_vist/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9674 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/bloom_vist/bloom_vist.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.467167 seacrowd-0.0.3/seacrowd/sea_datasets/burapha_th/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/burapha_th/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6995 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/burapha_th/burapha_th.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.486256 seacrowd-0.0.3/seacrowd/sea_datasets/burmese_romanize/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/burmese_romanize/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4420 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.511517 seacrowd-0.0.3/seacrowd/sea_datasets/casa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/casa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5635 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/casa/casa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.531704 seacrowd-0.0.3/seacrowd/sea_datasets/cc100/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cc100/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10941 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cc100/cc100.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.551938 seacrowd-0.0.3/seacrowd/sea_datasets/cc_aligned_doc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cc_aligned_doc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6230 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.573230 seacrowd-0.0.3/seacrowd/sea_datasets/cc_aligned_sent/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cc_aligned_sent/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6256 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.592475 seacrowd-0.0.3/seacrowd/sea_datasets/cebuaner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cebuaner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7783 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cebuaner/cebuaner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.620211 seacrowd-0.0.3/seacrowd/sea_datasets/coco_35l/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/coco_35l/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9830 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/coco_35l/coco_35l.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.639381 seacrowd-0.0.3/seacrowd/sea_datasets/cod/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cod/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6239 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cod/cod.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.657482 seacrowd-0.0.3/seacrowd/sea_datasets/code_mixed_jv_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/code_mixed_jv_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8760 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.683561 seacrowd-0.0.3/seacrowd/sea_datasets/codeswitch_reddit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/codeswitch_reddit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9015 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.704738 seacrowd-0.0.3/seacrowd/sea_datasets/commonvoice_120/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/commonvoice_120/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9438 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.729735 seacrowd-0.0.3/seacrowd/sea_datasets/copal/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/copal/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5868 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/copal/copal.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.748011 seacrowd-0.0.3/seacrowd/sea_datasets/covost2/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/covost2/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10329 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/covost2/covost2.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.783308 seacrowd-0.0.3/seacrowd/sea_datasets/creole_rc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.3/seacrowd/sea_datasets/creole_rc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9448 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/creole_rc/creole_rc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.801555 seacrowd-0.0.3/seacrowd/sea_datasets/crosssum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/crosssum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5467 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/crosssum/crosssum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.819659 seacrowd-0.0.3/seacrowd/sea_datasets/cub_bahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cub_bahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14495 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.844628 seacrowd-0.0.3/seacrowd/sea_datasets/culturax/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/culturax/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6383 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/culturax/culturax.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.863321 seacrowd-0.0.3/seacrowd/sea_datasets/cvss/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cvss/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11054 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/cvss/cvss.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.890014 seacrowd-0.0.3/seacrowd/sea_datasets/dengue_filipino/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/dengue_filipino/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4777 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.910613 seacrowd-0.0.3/seacrowd/sea_datasets/emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5522 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/emot/emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.931147 seacrowd-0.0.3/seacrowd/sea_datasets/emotcmt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/emotcmt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4484 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/emotcmt/emotcmt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.955660 seacrowd-0.0.3/seacrowd/sea_datasets/emotes_3k/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/emotes_3k/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9257 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/emotes_3k/emotes_3k.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:27.979029 seacrowd-0.0.3/seacrowd/sea_datasets/emotion_id_opinion/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/emotion_id_opinion/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7315 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.000301 seacrowd-0.0.3/seacrowd/sea_datasets/etos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/etos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7041 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/etos/etos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.032960 seacrowd-0.0.3/seacrowd/sea_datasets/facqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/facqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5788 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/facqa/facqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.063581 seacrowd-0.0.3/seacrowd/sea_datasets/facqa/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/facqa/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      815 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/facqa/utils/facqa_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.084092 seacrowd-0.0.3/seacrowd/sea_datasets/fakenews_ph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/fakenews_ph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4936 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.107488 seacrowd-0.0.3/seacrowd/sea_datasets/filipino_gay_lang/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/filipino_gay_lang/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4808 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.136896 seacrowd-0.0.3/seacrowd/sea_datasets/filipino_hatespeech_tiktok/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/filipino_hatespeech_tiktok/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4697 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.163152 seacrowd-0.0.3/seacrowd/sea_datasets/filipino_slang_norm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/filipino_slang_norm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4967 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.186855 seacrowd-0.0.3/seacrowd/sea_datasets/filipino_words_aoa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/filipino_words_aoa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4965 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.211849 seacrowd-0.0.3/seacrowd/sea_datasets/filwordnet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/filwordnet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/filwordnet/filwordnet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.250182 seacrowd-0.0.3/seacrowd/sea_datasets/fleurs/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/fleurs/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13189 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/fleurs/fleurs.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.277396 seacrowd-0.0.3/seacrowd/sea_datasets/flores200/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/flores200/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13920 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/flores200/flores200.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.305160 seacrowd-0.0.3/seacrowd/sea_datasets/fsl_105/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/fsl_105/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6753 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/fsl_105/fsl_105.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.331941 seacrowd-0.0.3/seacrowd/sea_datasets/gatitos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/gatitos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6624 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/gatitos/gatitos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.365597 seacrowd-0.0.3/seacrowd/sea_datasets/gklmip_newsclass/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/gklmip_newsclass/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6024 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.385951 seacrowd-0.0.3/seacrowd/sea_datasets/gklmip_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/gklmip_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5007 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.411117 seacrowd-0.0.3/seacrowd/sea_datasets/globalwoz/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/globalwoz/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10031 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/globalwoz/globalwoz.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.433140 seacrowd-0.0.3/seacrowd/sea_datasets/glotstorybook/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/glotstorybook/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5878 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/glotstorybook/glotstorybook.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.458281 seacrowd-0.0.3/seacrowd/sea_datasets/hoasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/hoasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6301 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/hoasa/hoasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.488917 seacrowd-0.0.3/seacrowd/sea_datasets/iapp_squad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/iapp_squad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5420 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/iapp_squad/iapp_squad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.516304 seacrowd-0.0.3/seacrowd/sea_datasets/iatf/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/iatf/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5801 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/iatf/iatf.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.535947 seacrowd-0.0.3/seacrowd/sea_datasets/icon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/icon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8351 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/icon/icon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.569968 seacrowd-0.0.3/seacrowd/sea_datasets/id_abusive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_abusive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6540 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_abusive/id_abusive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.589468 seacrowd-0.0.3/seacrowd/sea_datasets/id_abusive_news_comment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_abusive_news_comment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4293 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.606965 seacrowd-0.0.3/seacrowd/sea_datasets/id_am2ico/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_am2ico/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7430 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_am2ico/id_am2ico.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.626022 seacrowd-0.0.3/seacrowd/sea_datasets/id_clickbait/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_clickbait/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5770 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_clickbait/id_clickbait.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.646181 seacrowd-0.0.3/seacrowd/sea_datasets/id_coreference_resolution/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_coreference_resolution/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7576 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.674577 seacrowd-0.0.3/seacrowd/sea_datasets/id_frog_story/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_frog_story/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4524 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_frog_story/id_frog_story.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.694843 seacrowd-0.0.3/seacrowd/sea_datasets/id_google_play_review/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_google_play_review/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6144 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.713085 seacrowd-0.0.3/seacrowd/sea_datasets/id_hatespeech/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_hatespeech/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4450 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.746688 seacrowd-0.0.3/seacrowd/sea_datasets/id_hoax_news/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_hoax_news/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.764489 seacrowd-0.0.3/seacrowd/sea_datasets/id_hsd_nofaaulia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_hsd_nofaaulia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7252 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.792454 seacrowd-0.0.3/seacrowd/sea_datasets/id_msvd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_msvd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5051 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_msvd/id_msvd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.811467 seacrowd-0.0.3/seacrowd/sea_datasets/id_multilabel_hs/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_multilabel_hs/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6021 2024-04-04 06:00:46.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.834443 seacrowd-0.0.3/seacrowd/sea_datasets/id_panl_bppt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_panl_bppt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5616 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.852213 seacrowd-0.0.3/seacrowd/sea_datasets/id_qqp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_qqp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4686 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_qqp/id_qqp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.870274 seacrowd-0.0.3/seacrowd/sea_datasets/id_sent_emo_mobile_apps/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_sent_emo_mobile_apps/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5395 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.891702 seacrowd-0.0.3/seacrowd/sea_datasets/id_sentiment_analysis/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_sentiment_analysis/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5538 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.909592 seacrowd-0.0.3/seacrowd/sea_datasets/id_short_answer_grading/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_short_answer_grading/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9107 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.931693 seacrowd-0.0.3/seacrowd/sea_datasets/id_short_answer_grading/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_short_answer_grading/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1826 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.958036 seacrowd-0.0.3/seacrowd/sea_datasets/id_stance/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_stance/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5114 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_stance/id_stance.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:28.987010 seacrowd-0.0.3/seacrowd/sea_datasets/id_sts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_sts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4308 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_sts/id_sts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.007363 seacrowd-0.0.3/seacrowd/sea_datasets/id_vaccines_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_vaccines_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4329 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.038145 seacrowd-0.0.3/seacrowd/sea_datasets/id_wiki_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_wiki_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6697 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.072305 seacrowd-0.0.3/seacrowd/sea_datasets/id_wsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_wsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6404 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/id_wsd/id_wsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.098078 seacrowd-0.0.3/seacrowd/sea_datasets/identic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/identic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13357 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/identic/identic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.123618 seacrowd-0.0.3/seacrowd/sea_datasets/identifikasi_bahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/identifikasi_bahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5177 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.147230 seacrowd-0.0.3/seacrowd/sea_datasets/idk_mrc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/idk_mrc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9530 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/idk_mrc/idk_mrc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.178597 seacrowd-0.0.3/seacrowd/sea_datasets/idn_tagged_corpus_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/idn_tagged_corpus_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6193 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.202549 seacrowd-0.0.3/seacrowd/sea_datasets/ijelid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ijelid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5403 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ijelid/ijelid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.220080 seacrowd-0.0.3/seacrowd/sea_datasets/imdb_jv/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/imdb_jv/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4894 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/imdb_jv/imdb_jv.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.241406 seacrowd-0.0.3/seacrowd/sea_datasets/indo4b/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo4b/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7236 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo4b/indo4b.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.275154 seacrowd-0.0.3/seacrowd/sea_datasets/indo4b_plus/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo4b_plus/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7417 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.295687 seacrowd-0.0.3/seacrowd/sea_datasets/indo_general_mt_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo_general_mt_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6442 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.315517 seacrowd-0.0.3/seacrowd/sea_datasets/indo_law/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo_law/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5445 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo_law/indo_law.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.335039 seacrowd-0.0.3/seacrowd/sea_datasets/indo_puisi/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo_puisi/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4018 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo_puisi/indo_puisi.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.352100 seacrowd-0.0.3/seacrowd/sea_datasets/indo_religious_mt_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo_religious_mt_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8507 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.369903 seacrowd-0.0.3/seacrowd/sea_datasets/indo_story_cloze/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo_story_cloze/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6563 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.389042 seacrowd-0.0.3/seacrowd/sea_datasets/indocamrest/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indocamrest/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6670 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indocamrest/indocamrest.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.408871 seacrowd-0.0.3/seacrowd/sea_datasets/indocollex/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indocollex/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6949 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indocollex/indocollex.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.435142 seacrowd-0.0.3/seacrowd/sea_datasets/indocoref/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indocoref/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11610 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indocoref/indocoref.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.487466 seacrowd-0.0.3/seacrowd/sea_datasets/indocoref/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indocoref/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9072 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indocoref/utils/feature_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2091 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indocoref/utils/file_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4307 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.508481 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ner_ugm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ner_ugm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6402 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.526230 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_nerui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_nerui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8192 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.544140 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ntp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ntp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5885 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.567389 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12679 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.597209 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_tweet_ordering/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_tweet_ordering/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12454 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.615811 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ud_id_gsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ud_id_gsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8462 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.634913 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ud_id_pud/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ud_id_pud/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8825 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.654670 seacrowd-0.0.3/seacrowd/sea_datasets/indoler/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indoler/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9100 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indoler/indoler.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.672741 seacrowd-0.0.3/seacrowd/sea_datasets/indommlu/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indommlu/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10934 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indommlu/indommlu.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.691061 seacrowd-0.0.3/seacrowd/sea_datasets/indoner_tourism/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indoner_tourism/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8394 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.710105 seacrowd-0.0.3/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5250 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.737040 seacrowd-0.0.3/seacrowd/sea_datasets/indonesian_madurese_bible_translation/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonesian_madurese_bible_translation/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7932 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.769522 seacrowd-0.0.3/seacrowd/sea_datasets/indonesian_news_dataset/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonesian_news_dataset/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4581 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.789239 seacrowd-0.0.3/seacrowd/sea_datasets/indonesiannmt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonesiannmt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9148 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.808709 seacrowd-0.0.3/seacrowd/sea_datasets/indonglish/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonglish/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8339 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonglish/indonglish.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.831063 seacrowd-0.0.3/seacrowd/sea_datasets/indonli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8050 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonli/indonli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.857770 seacrowd-0.0.3/seacrowd/sea_datasets/indonlu_nergrit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonlu_nergrit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5677 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.876803 seacrowd-0.0.3/seacrowd/sea_datasets/indoqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indoqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5422 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indoqa/indoqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.895442 seacrowd-0.0.3/seacrowd/sea_datasets/indosmd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indosmd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13550 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indosmd/indosmd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.914362 seacrowd-0.0.3/seacrowd/sea_datasets/indosum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indosum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6872 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indosum/indosum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.936519 seacrowd-0.0.3/seacrowd/sea_datasets/indotacos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indotacos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indotacos/indotacos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.953374 seacrowd-0.0.3/seacrowd/sea_datasets/indowiki/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indowiki/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7684 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indowiki/indowiki.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:29.980156 seacrowd-0.0.3/seacrowd/sea_datasets/indqner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indqner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6614 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indqner/indqner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.003686 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_digit_cdsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_digit_cdsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9856 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.021765 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_news_ethnicsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_news_ethnicsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8440 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.039178 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_news_lvcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_news_lvcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9432 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.057019 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_news_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_news_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8857 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.075589 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11615 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.094676 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9932 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.114187 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_teldialog_svcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_teldialog_svcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9818 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.133354 seacrowd-0.0.3/seacrowd/sea_datasets/inset_lexicon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/inset_lexicon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4829 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.156956 seacrowd-0.0.3/seacrowd/sea_datasets/jadi_ide/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/jadi_ide/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4404 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/jadi_ide/jadi_ide.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.183347 seacrowd-0.0.3/seacrowd/sea_datasets/jv_id_asr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/jv_id_asr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6236 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.199969 seacrowd-0.0.3/seacrowd/sea_datasets/jv_id_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/jv_id_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7628 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.217567 seacrowd-0.0.3/seacrowd/sea_datasets/kamus_alay/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kamus_alay/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5286 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kamus_alay/kamus_alay.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.249011 seacrowd-0.0.3/seacrowd/sea_datasets/karonese_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/karonese_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4533 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.280387 seacrowd-0.0.3/seacrowd/sea_datasets/kawat/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kawat/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5933 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kawat/kawat.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.310948 seacrowd-0.0.3/seacrowd/sea_datasets/kde4/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kde4/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14408 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kde4/kde4.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.330509 seacrowd-0.0.3/seacrowd/sea_datasets/keps/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/keps/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5066 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/keps/keps.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.366102 seacrowd-0.0.3/seacrowd/sea_datasets/kheng_info/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kheng_info/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3687 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kheng_info/kheng_info.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.388907 seacrowd-0.0.3/seacrowd/sea_datasets/khmer_alt_pos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/khmer_alt_pos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7442 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.409730 seacrowd-0.0.3/seacrowd/sea_datasets/khpos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/khpos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8756 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/khpos/khpos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.442798 seacrowd-0.0.3/seacrowd/sea_datasets/kopi_cc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kopi_cc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10035 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kopi_cc/kopi_cc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.468495 seacrowd-0.0.3/seacrowd/sea_datasets/kopi_cc_news/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kopi_cc_news/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5088 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.488084 seacrowd-0.0.3/seacrowd/sea_datasets/kopi_nllb/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kopi_nllb/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5956 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.508344 seacrowd-0.0.3/seacrowd/sea_datasets/korpus_nusantara/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/korpus_nusantara/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8476 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.539205 seacrowd-0.0.3/seacrowd/sea_datasets/lazada_review_filipino/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/lazada_review_filipino/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4913 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.559618 seacrowd-0.0.3/seacrowd/sea_datasets/librivox_indonesia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/librivox_indonesia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8736 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.578781 seacrowd-0.0.3/seacrowd/sea_datasets/limesoda/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/limesoda/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6775 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/limesoda/limesoda.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.603561 seacrowd-0.0.3/seacrowd/sea_datasets/liputan6/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/liputan6/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7512 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/liputan6/liputan6.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.621658 seacrowd-0.0.3/seacrowd/sea_datasets/local_id_abusive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/local_id_abusive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7530 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.639237 seacrowd-0.0.3/seacrowd/sea_datasets/lr_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/lr_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6160 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/lr_sum/lr_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.664580 seacrowd-0.0.3/seacrowd/sea_datasets/m3exam/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/m3exam/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14637 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/m3exam/m3exam.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.693428 seacrowd-0.0.3/seacrowd/sea_datasets/mabl/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mabl/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8609 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mabl/mabl.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.710680 seacrowd-0.0.3/seacrowd/sea_datasets/malaysia_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/malaysia_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6432 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.729617 seacrowd-0.0.3/seacrowd/sea_datasets/malindo_morph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/malindo_morph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4617 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/malindo_morph/malindo_morph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.746176 seacrowd-0.0.3/seacrowd/sea_datasets/malindo_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/malindo_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6494 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.771379 seacrowd-0.0.3/seacrowd/sea_datasets/massive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/massive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    18420 2024-04-04 06:00:48.000000 seacrowd-0.0.3/seacrowd/sea_datasets/massive/massive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.792228 seacrowd-0.0.3/seacrowd/sea_datasets/mc4_indo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mc4_indo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5510 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mc4_indo/mc4_indo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.811518 seacrowd-0.0.3/seacrowd/sea_datasets/melayu_brunei/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/melayu_brunei/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10682 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.831861 seacrowd-0.0.3/seacrowd/sea_datasets/melayu_sabah/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/melayu_sabah/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5561 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.853214 seacrowd-0.0.3/seacrowd/sea_datasets/melayu_sarawak/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/melayu_sarawak/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6559 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.874139 seacrowd-0.0.3/seacrowd/sea_datasets/melayu_standard_lisan/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/melayu_standard_lisan/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7594 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.895745 seacrowd-0.0.3/seacrowd/sea_datasets/memolon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/memolon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5589 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/memolon/memolon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.915904 seacrowd-0.0.3/seacrowd/sea_datasets/minangnlp_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/minangnlp_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6874 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.934963 seacrowd-0.0.3/seacrowd/sea_datasets/miracl/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/miracl/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13119 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/miracl/miracl.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.952539 seacrowd-0.0.3/seacrowd/sea_datasets/mkqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mkqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8345 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mkqa/mkqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.973702 seacrowd-0.0.3/seacrowd/sea_datasets/mlqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mlqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9825 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mlqa/mlqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:30.995398 seacrowd-0.0.3/seacrowd/sea_datasets/mozilla_pontoon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mozilla_pontoon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6211 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.012728 seacrowd-0.0.3/seacrowd/sea_datasets/mswc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mswc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8048 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mswc/mswc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.046639 seacrowd-0.0.3/seacrowd/sea_datasets/mtop_intent_classification/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mtop_intent_classification/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2654 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mtop_intent_classification/labels.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5662 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.074310 seacrowd-0.0.3/seacrowd/sea_datasets/multilexnorm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/multilexnorm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6223 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/multilexnorm/multilexnorm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.092544 seacrowd-0.0.3/seacrowd/sea_datasets/my_paraphrase/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/my_paraphrase/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8124 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.108614 seacrowd-0.0.3/seacrowd/sea_datasets/myanmar_rakhine_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/myanmar_rakhine_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7223 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.132744 seacrowd-0.0.3/seacrowd/sea_datasets/mypos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mypos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5116 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mypos/mypos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.152996 seacrowd-0.0.3/seacrowd/sea_datasets/mysentence/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mysentence/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7612 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/mysentence/mysentence.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.178690 seacrowd-0.0.3/seacrowd/sea_datasets/myxnli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/myxnli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5096 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/myxnli/myxnli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.203353 seacrowd-0.0.3/seacrowd/sea_datasets/nergrit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nergrit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6322 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nergrit/nergrit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.234228 seacrowd-0.0.3/seacrowd/sea_datasets/nerp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nerp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4852 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nerp/nerp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.259546 seacrowd-0.0.3/seacrowd/sea_datasets/netifier/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/netifier/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4838 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/netifier/netifier.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.280984 seacrowd-0.0.3/seacrowd/sea_datasets/news_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/news_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5003 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/news_en_id/news_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.301144 seacrowd-0.0.3/seacrowd/sea_datasets/newsph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/newsph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3810 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/newsph/newsph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.322315 seacrowd-0.0.3/seacrowd/sea_datasets/nllb_seed/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nllb_seed/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15208 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nllb_seed/nllb_seed.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.341324 seacrowd-0.0.3/seacrowd/sea_datasets/ntrex_128/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ntrex_128/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10971 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ntrex_128/ntrex_128.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.364547 seacrowd-0.0.3/seacrowd/sea_datasets/nusaparagraph_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusaparagraph_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8785 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.402093 seacrowd-0.0.3/seacrowd/sea_datasets/nusaparagraph_rhetoric/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusaparagraph_rhetoric/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8792 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.421722 seacrowd-0.0.3/seacrowd/sea_datasets/nusaparagraph_topic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusaparagraph_topic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8845 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.443483 seacrowd-0.0.3/seacrowd/sea_datasets/nusatranslation_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusatranslation_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.461066 seacrowd-0.0.3/seacrowd/sea_datasets/nusatranslation_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusatranslation_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9156 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.484606 seacrowd-0.0.3/seacrowd/sea_datasets/nusatranslation_senti/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusatranslation_senti/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8285 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.501946 seacrowd-0.0.3/seacrowd/sea_datasets/nusax_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusax_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7578 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusax_mt/nusax_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.530932 seacrowd-0.0.3/seacrowd/sea_datasets/nusax_senti/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusax_senti/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7250 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/nusax_senti/nusax_senti.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.568509 seacrowd-0.0.3/seacrowd/sea_datasets/oil/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/oil/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/oil/oil.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.597071 seacrowd-0.0.3/seacrowd/sea_datasets/ojw/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ojw/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5110 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ojw/ojw.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.615750 seacrowd-0.0.3/seacrowd/sea_datasets/openlid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/openlid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7915 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/openlid/openlid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.640563 seacrowd-0.0.3/seacrowd/sea_datasets/openslr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/openslr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10343 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/openslr/openslr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.671044 seacrowd-0.0.3/seacrowd/sea_datasets/orchid_pos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/orchid_pos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9625 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/orchid_pos/orchid_pos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.697221 seacrowd-0.0.3/seacrowd/sea_datasets/oscar_2201/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/oscar_2201/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    16270 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/oscar_2201/oscar_2201.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.715210 seacrowd-0.0.3/seacrowd/sea_datasets/palito/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/palito/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5930 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/palito/palito.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.742941 seacrowd-0.0.3/seacrowd/sea_datasets/paracotta_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/paracotta_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4768 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/paracotta_id/paracotta_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.760698 seacrowd-0.0.3/seacrowd/sea_datasets/parallel_id_nyo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/parallel_id_nyo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5471 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.792731 seacrowd-0.0.3/seacrowd/sea_datasets/parallel_su_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/parallel_su_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4782 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.813248 seacrowd-0.0.3/seacrowd/sea_datasets/ph_fake_news_corpus/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ph_fake_news_corpus/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4339 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.857767 seacrowd-0.0.3/seacrowd/sea_datasets/pho_ner_covid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/pho_ner_covid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6866 2024-04-04 06:00:49.000000 seacrowd-0.0.3/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.895015 seacrowd-0.0.3/seacrowd/sea_datasets/phomt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/phomt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5141 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/phomt/phomt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.920035 seacrowd-0.0.3/seacrowd/sea_datasets/phost/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/phost/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9498 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/phost/phost.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.939729 seacrowd-0.0.3/seacrowd/sea_datasets/posp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/posp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5990 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/posp/posp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.967332 seacrowd-0.0.3/seacrowd/sea_datasets/postag_su/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/postag_su/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8033 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/postag_su/postag_su.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:31.988350 seacrowd-0.0.3/seacrowd/sea_datasets/prdect_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/prdect_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7572 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/prdect_id/prdect_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.008946 seacrowd-0.0.3/seacrowd/sea_datasets/qasina/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/qasina/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6424 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/qasina/qasina.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.033914 seacrowd-0.0.3/seacrowd/sea_datasets/roots_vi_ted/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/roots_vi_ted/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5065 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.060492 seacrowd-0.0.3/seacrowd/sea_datasets/sampiran/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sampiran/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5024 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sampiran/sampiran.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.082149 seacrowd-0.0.3/seacrowd/sea_datasets/sap_wat/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sap_wat/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7077 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sap_wat/sap_wat.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.107524 seacrowd-0.0.3/seacrowd/sea_datasets/sarawak_malay/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sarawak_malay/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7381 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.127419 seacrowd-0.0.3/seacrowd/sea_datasets/scb_mt_en_th/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/scb_mt_en_th/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7071 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.147310 seacrowd-0.0.3/seacrowd/sea_datasets/sea_bench/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sea_bench/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7206 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sea_bench/sea_bench.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.184852 seacrowd-0.0.3/seacrowd/sea_datasets/sea_madlad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sea_madlad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10051 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sea_madlad/sea_madlad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.210593 seacrowd-0.0.3/seacrowd/sea_datasets/sea_wiki/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sea_wiki/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sea_wiki/sea_wiki.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.230541 seacrowd-0.0.3/seacrowd/sea_datasets/seaeval/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/seaeval/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/seaeval/seaeval.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.248957 seacrowd-0.0.3/seacrowd/sea_datasets/seahorse/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/seahorse/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6884 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/seahorse/seahorse.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.272073 seacrowd-0.0.3/seacrowd/sea_datasets/sentiment_nathasa_review/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sentiment_nathasa_review/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6002 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.287493 seacrowd-0.0.3/seacrowd/sea_datasets/shopee_reviews_tagalog/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/shopee_reviews_tagalog/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4597 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.305403 seacrowd-0.0.3/seacrowd/sea_datasets/singgalang/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/singgalang/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5430 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/singgalang/singgalang.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.335252 seacrowd-0.0.3/seacrowd/sea_datasets/smsa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/smsa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5575 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/smsa/smsa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.360563 seacrowd-0.0.3/seacrowd/sea_datasets/snli_indo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/snli_indo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6244 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/snli_indo/snli_indo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.389056 seacrowd-0.0.3/seacrowd/sea_datasets/spamid_pair/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/spamid_pair/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5524 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/spamid_pair/spamid_pair.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.407001 seacrowd-0.0.3/seacrowd/sea_datasets/squad_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/squad_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5315 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/squad_id/squad_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.429076 seacrowd-0.0.3/seacrowd/sea_datasets/stb_ext/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/stb_ext/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9273 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/stb_ext/stb_ext.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.448796 seacrowd-0.0.3/seacrowd/sea_datasets/stif_indonesia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/stif_indonesia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5135 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.468785 seacrowd-0.0.3/seacrowd/sea_datasets/struct_amb_ind/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/struct_amb_ind/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7724 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.488784 seacrowd-0.0.3/seacrowd/sea_datasets/su_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/su_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4567 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/su_emot/su_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.506782 seacrowd-0.0.3/seacrowd/sea_datasets/su_id_asr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/su_id_asr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5601 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/su_id_asr/su_id_asr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.524536 seacrowd-0.0.3/seacrowd/sea_datasets/su_id_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/su_id_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/su_id_tts/su_id_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.542475 seacrowd-0.0.3/seacrowd/sea_datasets/talpco/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/talpco/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6870 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/talpco/talpco.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.568551 seacrowd-0.0.3/seacrowd/sea_datasets/tatabahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tatabahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5411 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tatabahasa/tatabahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.587853 seacrowd-0.0.3/seacrowd/sea_datasets/tatoeba/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tatoeba/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tatoeba/tatoeba.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.605696 seacrowd-0.0.3/seacrowd/sea_datasets/tcope/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tcope/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6693 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tcope/tcope.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.622952 seacrowd-0.0.3/seacrowd/sea_datasets/ted_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ted_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7105 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ted_en_id/ted_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.642947 seacrowd-0.0.3/seacrowd/sea_datasets/term_a/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/term_a/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5358 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/term_a/term_a.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.661854 seacrowd-0.0.3/seacrowd/sea_datasets/tgl_profanity/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tgl_profanity/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4351 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.683717 seacrowd-0.0.3/seacrowd/sea_datasets/tha_lao_embassy_parcor/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tha_lao_embassy_parcor/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4436 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.712392 seacrowd-0.0.3/seacrowd/sea_datasets/thai_alpaca/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_alpaca/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3943 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.737597 seacrowd-0.0.3/seacrowd/sea_datasets/thai_constitution/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_constitution/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10954 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_constitution/thai_constitution.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.755869 seacrowd-0.0.3/seacrowd/sea_datasets/thai_databricks_dolly/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_databricks_dolly/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4388 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.773859 seacrowd-0.0.3/seacrowd/sea_datasets/thai_depression/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_depression/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5739 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_depression/thai_depression.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.791613 seacrowd-0.0.3/seacrowd/sea_datasets/thai_gpteacher/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_gpteacher/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3960 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.808568 seacrowd-0.0.3/seacrowd/sea_datasets/thai_hh_rlhf/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_hh_rlhf/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5077 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.827031 seacrowd-0.0.3/seacrowd/sea_datasets/thai_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5683 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_sum/thai_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.846171 seacrowd-0.0.3/seacrowd/sea_datasets/thai_toxicity_tweet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_toxicity_tweet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.872311 seacrowd-0.0.3/seacrowd/sea_datasets/tico_19/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tico_19/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12192 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tico_19/tico_19.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.890704 seacrowd-0.0.3/seacrowd/sea_datasets/titml_idn/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/titml_idn/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/titml_idn/titml_idn.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.909729 seacrowd-0.0.3/seacrowd/sea_datasets/tlunified_ner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tlunified_ner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5800 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.931948 seacrowd-0.0.3/seacrowd/sea_datasets/toxicity_200/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/toxicity_200/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5975 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/toxicity_200/toxicity_200.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.959617 seacrowd-0.0.3/seacrowd/sea_datasets/tydiqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tydiqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23881 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/tydiqa/tydiqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.979735 seacrowd-0.0.3/seacrowd/sea_datasets/typhoon_yolanda_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/typhoon_yolanda_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5165 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:32.999643 seacrowd-0.0.3/seacrowd/sea_datasets/ucla_phonetic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ucla_phonetic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6531 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.018272 seacrowd-0.0.3/seacrowd/sea_datasets/ud_id_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ud_id_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9185 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.037619 seacrowd-0.0.3/seacrowd/sea_datasets/ud_jv_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ud_jv_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10052 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.059467 seacrowd-0.0.3/seacrowd/sea_datasets/udhr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/udhr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6030 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/udhr/udhr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.083064 seacrowd-0.0.3/seacrowd/sea_datasets/udhr_lid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/udhr_lid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5190 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/udhr_lid/udhr_lid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.101810 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vicov19qa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vicov19qa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7244 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.119559 seacrowd-0.0.3/seacrowd/sea_datasets/uit_victsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_victsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5311 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_victsd/uit_victsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.153749 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vihsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vihsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5721 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.178273 seacrowd-0.0.3/seacrowd/sea_datasets/uit_viic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_viic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6572 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_viic/uit_viic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.207678 seacrowd-0.0.3/seacrowd/sea_datasets/uit_viocd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_viocd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_viocd/uit_viocd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.226096 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vion/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vion/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5939 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vion/uit_vion.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.253055 seacrowd-0.0.3/seacrowd/sea_datasets/uit_visd4sa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_visd4sa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7034 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.287095 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vsfc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vsfc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8715 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.309268 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vsmec/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vsmec/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4802 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.333069 seacrowd-0.0.3/seacrowd/sea_datasets/unimorph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/unimorph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15492 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/unimorph/unimorph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.359594 seacrowd-0.0.3/seacrowd/sea_datasets/unimorph_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/unimorph_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7445 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/unimorph_id/unimorph_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.380012 seacrowd-0.0.3/seacrowd/sea_datasets/vi_pubmed/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vi_pubmed/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15136 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.419936 seacrowd-0.0.3/seacrowd/sea_datasets/vihealthqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vihealthqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5587 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vihealthqa/vihealthqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.446528 seacrowd-0.0.3/seacrowd/sea_datasets/visobert/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/visobert/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6265 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/visobert/visobert.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.472547 seacrowd-0.0.3/seacrowd/sea_datasets/vispamreviews/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vispamreviews/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7245 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vispamreviews/vispamreviews.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.503193 seacrowd-0.0.3/seacrowd/sea_datasets/vistec_tp_th_21/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vistec_tp_th_21/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6739 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.549485 seacrowd-0.0.3/seacrowd/sea_datasets/vitext2sql/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vitext2sql/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6893 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vitext2sql/vitext2sql.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.572085 seacrowd-0.0.3/seacrowd/sea_datasets/vivos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vivos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7832 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vivos/vivos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.591807 seacrowd-0.0.3/seacrowd/sea_datasets/vivqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vivqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9080 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vivqa/vivqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.613005 seacrowd-0.0.3/seacrowd/sea_datasets/vlsp2016_ner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vlsp2016_ner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5857 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.633787 seacrowd-0.0.3/seacrowd/sea_datasets/vlsp2016_sa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vlsp2016_sa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7134 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.673390 seacrowd-0.0.3/seacrowd/sea_datasets/vndt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vndt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2232 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vndt/utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7852 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/vndt/vndt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.700682 seacrowd-0.0.3/seacrowd/sea_datasets/voxlingua/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/voxlingua/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7980 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/voxlingua/voxlingua.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.728118 seacrowd-0.0.3/seacrowd/sea_datasets/weathub/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/weathub/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7521 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/weathub/weathub.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.756481 seacrowd-0.0.3/seacrowd/sea_datasets/wikiann/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wikiann/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8643 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wikiann/wikiann.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.773634 seacrowd-0.0.3/seacrowd/sea_datasets/wikilingua/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wikilingua/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4984 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wikilingua/wikilingua.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.790875 seacrowd-0.0.3/seacrowd/sea_datasets/wikimatrix/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wikimatrix/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8585 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wikimatrix/wikimatrix.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.810159 seacrowd-0.0.3/seacrowd/sea_datasets/wikitext_tl_39/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wikitext_tl_39/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3663 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.829254 seacrowd-0.0.3/seacrowd/sea_datasets/wili_2018/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wili_2018/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6699 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wili_2018/wili_2018.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.847883 seacrowd-0.0.3/seacrowd/sea_datasets/wisesight_thai_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wisesight_thai_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7027 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.866949 seacrowd-0.0.3/seacrowd/sea_datasets/wit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12057 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wit/wit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.885306 seacrowd-0.0.3/seacrowd/sea_datasets/wongnai_reviews/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wongnai_reviews/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4106 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.903940 seacrowd-0.0.3/seacrowd/sea_datasets/wrete/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wrete/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6113 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/wrete/wrete.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.920626 seacrowd-0.0.3/seacrowd/sea_datasets/x_fact/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/x_fact/__init__.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.939027 seacrowd-0.0.3/seacrowd/sea_datasets/x_fact/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/x_fact/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      473 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/x_fact/utils/x_fact_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/x_fact/x_fact.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.956050 seacrowd-0.0.3/seacrowd/sea_datasets/xcopa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xcopa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7024 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xcopa/xcopa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.973707 seacrowd-0.0.3/seacrowd/sea_datasets/xl_jailbreak/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xl_jailbreak/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6317 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:33.997972 seacrowd-0.0.3/seacrowd/sea_datasets/xl_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xl_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6903 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xl_sum/xl_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:34.032626 seacrowd-0.0.3/seacrowd/sea_datasets/xm3600/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xm3600/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-11 08:39:41.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xm3600/xm3600.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:34.062427 seacrowd-0.0.3/seacrowd/sea_datasets/xnli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xnli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8333 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xnli/xnli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:34.081824 seacrowd-0.0.3/seacrowd/sea_datasets/xpersona_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xpersona_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6550 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xpersona_id/xpersona_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:34.102764 seacrowd-0.0.3/seacrowd/sea_datasets/xquad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xquad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xquad/xquad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:34.122604 seacrowd-0.0.3/seacrowd/sea_datasets/xsid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xsid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9510 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xsid/xsid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:34.141914 seacrowd-0.0.3/seacrowd/sea_datasets/xstorycloze/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xstorycloze/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6794 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/sea_datasets/xstorycloze/xstorycloze.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:34.168649 seacrowd-0.0.3/seacrowd/sea_datasets/yunshan_cup_2020/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/sea_datasets/yunshan_cup_2020/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5828 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:34.205551 seacrowd-0.0.3/seacrowd/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5493 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/common_parser.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      284 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/configs.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12786 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/constants.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:34.442321 seacrowd-0.0.3/seacrowd/utils/schemas/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1485 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      506 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/image_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1101 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/imqa.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2283 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/kb.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      626 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/pairs.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      371 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/pairs_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1007 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/qa.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      206 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/self_supervised_pretraining.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      525 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/seq_label.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      618 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/speech.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      606 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/speech_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      454 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/speech_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      796 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/speech_to_speech.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      311 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      331 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/text_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      444 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/text_to_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3046 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/tod.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3068 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/tree.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      810 2024-04-04 06:00:52.000000 seacrowd-0.0.3/seacrowd/utils/schemas/video.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:34.489841 seacrowd-0.0.3/seacrowd.egg-info/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-11 08:42:25.000000 seacrowd-0.0.3/seacrowd.egg-info/PKG-INFO
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    31277 2024-04-11 08:42:25.000000 seacrowd-0.0.3/seacrowd.egg-info/SOURCES.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-11 08:42:25.000000 seacrowd-0.0.3/seacrowd.egg-info/dependency_links.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      409 2024-04-11 08:42:25.000000 seacrowd-0.0.3/seacrowd.egg-info/requires.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       15 2024-04-11 08:42:25.000000 seacrowd-0.0.3/seacrowd.egg-info/top_level.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      666 2024-04-11 08:42:34.518284 seacrowd-0.0.3/setup.cfg
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       68 2024-04-04 06:00:52.000000 seacrowd-0.0.3/setup.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 08:42:34.476164 seacrowd-0.0.3/tests/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.3/tests/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23314 2024-04-04 06:00:52.000000 seacrowd-0.0.3/tests/test_seacrowd.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    20714 2024-04-04 06:00:52.000000 seacrowd-0.0.3/tests/test_seacrowd_source_only.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.582415 seacrowd-0.0.4/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11357 2024-04-04 06:00:44.000000 seacrowd-0.0.4/LICENSE
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-11 09:04:26.579179 seacrowd-0.0.4/PKG-INFO
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5757 2024-04-04 06:00:44.000000 seacrowd-0.0.4/README.md
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.493566 seacrowd-0.0.4/seacrowd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      251 2024-04-11 09:04:09.000000 seacrowd-0.0.4/seacrowd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    40451 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/config_helper.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.564295 seacrowd-0.0.4/seacrowd/sea_datasets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/__init__.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.582461 seacrowd-0.0.4/seacrowd/sea_datasets/abui_wordnet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/abui_wordnet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5277 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.601288 seacrowd-0.0.4/seacrowd/sea_datasets/alt_burmese_treebank/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/alt_burmese_treebank/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5692 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.619309 seacrowd-0.0.4/seacrowd/sea_datasets/alt_burmese_treebank/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/alt_burmese_treebank/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2661 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.636889 seacrowd-0.0.4/seacrowd/sea_datasets/ara_close/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ara_close/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8227 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ara_close/ara_close.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.656410 seacrowd-0.0.4/seacrowd/sea_datasets/asr_sindodusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/asr_sindodusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7231 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.676687 seacrowd-0.0.4/seacrowd/sea_datasets/asr_smaldusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/asr_smaldusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7305 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.694296 seacrowd-0.0.4/seacrowd/sea_datasets/asr_stidusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/asr_stidusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6979 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.712180 seacrowd-0.0.4/seacrowd/sea_datasets/audio_keyword_spotting/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/audio_keyword_spotting/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7860 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.730532 seacrowd-0.0.4/seacrowd/sea_datasets/aya_dataset/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/aya_dataset/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7482 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/aya_dataset/aya_dataset.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.747243 seacrowd-0.0.4/seacrowd/sea_datasets/barasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/barasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7224 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/barasa/barasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.766327 seacrowd-0.0.4/seacrowd/sea_datasets/beaye_lexicon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/beaye_lexicon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4357 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.790536 seacrowd-0.0.4/seacrowd/sea_datasets/belebele/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/belebele/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8610 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/belebele/belebele.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.807447 seacrowd-0.0.4/seacrowd/sea_datasets/bible_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bible_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6790 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bible_en_id/bible_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.828560 seacrowd-0.0.4/seacrowd/sea_datasets/bible_jv_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bible_jv_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6856 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.845720 seacrowd-0.0.4/seacrowd/sea_datasets/bible_su_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bible_su_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6632 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bible_su_id/bible_su_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.863100 seacrowd-0.0.4/seacrowd/sea_datasets/bioner_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bioner_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6108 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bioner_id/bioner_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.883189 seacrowd-0.0.4/seacrowd/sea_datasets/bloom_captioning/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bloom_captioning/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8518 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.903827 seacrowd-0.0.4/seacrowd/sea_datasets/bloom_lm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bloom_lm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8430 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bloom_lm/bloom_lm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.923303 seacrowd-0.0.4/seacrowd/sea_datasets/bloom_speech/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bloom_speech/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6922 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bloom_speech/bloom_speech.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.941800 seacrowd-0.0.4/seacrowd/sea_datasets/bloom_vist/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bloom_vist/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9674 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/bloom_vist/bloom_vist.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.960869 seacrowd-0.0.4/seacrowd/sea_datasets/burapha_th/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/burapha_th/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6995 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/burapha_th/burapha_th.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.977797 seacrowd-0.0.4/seacrowd/sea_datasets/burmese_romanize/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/burmese_romanize/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4420 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:20.994814 seacrowd-0.0.4/seacrowd/sea_datasets/casa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/casa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5635 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/casa/casa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.012231 seacrowd-0.0.4/seacrowd/sea_datasets/cc100/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cc100/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10941 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cc100/cc100.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.028724 seacrowd-0.0.4/seacrowd/sea_datasets/cc_aligned_doc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cc_aligned_doc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6230 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.045263 seacrowd-0.0.4/seacrowd/sea_datasets/cc_aligned_sent/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cc_aligned_sent/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6256 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.061455 seacrowd-0.0.4/seacrowd/sea_datasets/cebuaner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cebuaner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7783 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cebuaner/cebuaner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.078033 seacrowd-0.0.4/seacrowd/sea_datasets/coco_35l/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/coco_35l/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9830 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/coco_35l/coco_35l.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.095602 seacrowd-0.0.4/seacrowd/sea_datasets/cod/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cod/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6239 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cod/cod.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.114160 seacrowd-0.0.4/seacrowd/sea_datasets/code_mixed_jv_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/code_mixed_jv_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8760 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.131899 seacrowd-0.0.4/seacrowd/sea_datasets/codeswitch_reddit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/codeswitch_reddit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9015 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.148848 seacrowd-0.0.4/seacrowd/sea_datasets/commonvoice_120/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/commonvoice_120/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9438 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.166992 seacrowd-0.0.4/seacrowd/sea_datasets/copal/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/copal/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5868 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/copal/copal.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.183609 seacrowd-0.0.4/seacrowd/sea_datasets/covost2/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/covost2/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10329 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/covost2/covost2.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.201390 seacrowd-0.0.4/seacrowd/sea_datasets/creole_rc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.4/seacrowd/sea_datasets/creole_rc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9448 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/creole_rc/creole_rc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.219372 seacrowd-0.0.4/seacrowd/sea_datasets/crosssum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/crosssum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5467 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/crosssum/crosssum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.240065 seacrowd-0.0.4/seacrowd/sea_datasets/cub_bahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cub_bahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14495 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.256001 seacrowd-0.0.4/seacrowd/sea_datasets/culturax/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/culturax/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6383 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/culturax/culturax.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.272126 seacrowd-0.0.4/seacrowd/sea_datasets/cvss/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cvss/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11054 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/cvss/cvss.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.291331 seacrowd-0.0.4/seacrowd/sea_datasets/dengue_filipino/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/dengue_filipino/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4777 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.309560 seacrowd-0.0.4/seacrowd/sea_datasets/emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5522 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/emot/emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.326448 seacrowd-0.0.4/seacrowd/sea_datasets/emotcmt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/emotcmt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4484 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/emotcmt/emotcmt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.343774 seacrowd-0.0.4/seacrowd/sea_datasets/emotes_3k/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/emotes_3k/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9257 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/emotes_3k/emotes_3k.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.362160 seacrowd-0.0.4/seacrowd/sea_datasets/emotion_id_opinion/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/emotion_id_opinion/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7315 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.378599 seacrowd-0.0.4/seacrowd/sea_datasets/etos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/etos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7041 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/etos/etos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.395294 seacrowd-0.0.4/seacrowd/sea_datasets/facqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/facqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5788 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/facqa/facqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.412926 seacrowd-0.0.4/seacrowd/sea_datasets/facqa/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/facqa/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      815 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/facqa/utils/facqa_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.431181 seacrowd-0.0.4/seacrowd/sea_datasets/fakenews_ph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/fakenews_ph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4936 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.446681 seacrowd-0.0.4/seacrowd/sea_datasets/filipino_gay_lang/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/filipino_gay_lang/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4808 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.464296 seacrowd-0.0.4/seacrowd/sea_datasets/filipino_hatespeech_tiktok/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/filipino_hatespeech_tiktok/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4697 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.481727 seacrowd-0.0.4/seacrowd/sea_datasets/filipino_slang_norm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/filipino_slang_norm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4967 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.499095 seacrowd-0.0.4/seacrowd/sea_datasets/filipino_words_aoa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/filipino_words_aoa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4965 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.515286 seacrowd-0.0.4/seacrowd/sea_datasets/filwordnet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/filwordnet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/filwordnet/filwordnet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.530704 seacrowd-0.0.4/seacrowd/sea_datasets/fleurs/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/fleurs/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13201 2024-04-11 09:01:40.000000 seacrowd-0.0.4/seacrowd/sea_datasets/fleurs/fleurs.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.547647 seacrowd-0.0.4/seacrowd/sea_datasets/flores200/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/flores200/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13920 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/flores200/flores200.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.568133 seacrowd-0.0.4/seacrowd/sea_datasets/fsl_105/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/fsl_105/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6753 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/fsl_105/fsl_105.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.584902 seacrowd-0.0.4/seacrowd/sea_datasets/gatitos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/gatitos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6624 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/gatitos/gatitos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.602575 seacrowd-0.0.4/seacrowd/sea_datasets/gklmip_newsclass/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/gklmip_newsclass/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6024 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.623765 seacrowd-0.0.4/seacrowd/sea_datasets/gklmip_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/gklmip_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5007 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.640123 seacrowd-0.0.4/seacrowd/sea_datasets/globalwoz/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/globalwoz/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10031 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/globalwoz/globalwoz.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.658698 seacrowd-0.0.4/seacrowd/sea_datasets/glotstorybook/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/glotstorybook/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5878 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/glotstorybook/glotstorybook.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.676540 seacrowd-0.0.4/seacrowd/sea_datasets/hoasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/hoasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6301 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/hoasa/hoasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.693432 seacrowd-0.0.4/seacrowd/sea_datasets/iapp_squad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/iapp_squad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5420 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/iapp_squad/iapp_squad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.711222 seacrowd-0.0.4/seacrowd/sea_datasets/iatf/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/iatf/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5801 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/iatf/iatf.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.728546 seacrowd-0.0.4/seacrowd/sea_datasets/icon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/icon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8351 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/icon/icon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.746346 seacrowd-0.0.4/seacrowd/sea_datasets/id_abusive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_abusive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6540 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_abusive/id_abusive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.765608 seacrowd-0.0.4/seacrowd/sea_datasets/id_abusive_news_comment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_abusive_news_comment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4293 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.784145 seacrowd-0.0.4/seacrowd/sea_datasets/id_am2ico/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_am2ico/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7430 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_am2ico/id_am2ico.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.802204 seacrowd-0.0.4/seacrowd/sea_datasets/id_clickbait/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_clickbait/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5770 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_clickbait/id_clickbait.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.822205 seacrowd-0.0.4/seacrowd/sea_datasets/id_coreference_resolution/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_coreference_resolution/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7576 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.839101 seacrowd-0.0.4/seacrowd/sea_datasets/id_frog_story/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_frog_story/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4524 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_frog_story/id_frog_story.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.858188 seacrowd-0.0.4/seacrowd/sea_datasets/id_google_play_review/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_google_play_review/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6144 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.880895 seacrowd-0.0.4/seacrowd/sea_datasets/id_hatespeech/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_hatespeech/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4450 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.898600 seacrowd-0.0.4/seacrowd/sea_datasets/id_hoax_news/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_hoax_news/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.915473 seacrowd-0.0.4/seacrowd/sea_datasets/id_hsd_nofaaulia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_hsd_nofaaulia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7252 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.932561 seacrowd-0.0.4/seacrowd/sea_datasets/id_msvd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_msvd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5051 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_msvd/id_msvd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.956606 seacrowd-0.0.4/seacrowd/sea_datasets/id_multilabel_hs/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_multilabel_hs/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6021 2024-04-04 06:00:46.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.971921 seacrowd-0.0.4/seacrowd/sea_datasets/id_panl_bppt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_panl_bppt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5616 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:21.987850 seacrowd-0.0.4/seacrowd/sea_datasets/id_qqp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_qqp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4686 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_qqp/id_qqp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.004639 seacrowd-0.0.4/seacrowd/sea_datasets/id_sent_emo_mobile_apps/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_sent_emo_mobile_apps/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5395 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.054180 seacrowd-0.0.4/seacrowd/sea_datasets/id_sentiment_analysis/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_sentiment_analysis/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5538 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.073310 seacrowd-0.0.4/seacrowd/sea_datasets/id_short_answer_grading/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_short_answer_grading/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9107 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.091929 seacrowd-0.0.4/seacrowd/sea_datasets/id_short_answer_grading/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_short_answer_grading/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1826 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.108542 seacrowd-0.0.4/seacrowd/sea_datasets/id_stance/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_stance/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5114 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_stance/id_stance.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.126906 seacrowd-0.0.4/seacrowd/sea_datasets/id_sts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_sts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4308 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_sts/id_sts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.142932 seacrowd-0.0.4/seacrowd/sea_datasets/id_vaccines_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_vaccines_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4329 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.161605 seacrowd-0.0.4/seacrowd/sea_datasets/id_wiki_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_wiki_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6697 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.179141 seacrowd-0.0.4/seacrowd/sea_datasets/id_wsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_wsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6404 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/id_wsd/id_wsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.195239 seacrowd-0.0.4/seacrowd/sea_datasets/identic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/identic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13357 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/identic/identic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.212467 seacrowd-0.0.4/seacrowd/sea_datasets/identifikasi_bahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/identifikasi_bahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5177 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.226909 seacrowd-0.0.4/seacrowd/sea_datasets/idk_mrc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/idk_mrc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9530 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/idk_mrc/idk_mrc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.243611 seacrowd-0.0.4/seacrowd/sea_datasets/idn_tagged_corpus_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/idn_tagged_corpus_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6193 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.258515 seacrowd-0.0.4/seacrowd/sea_datasets/ijelid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ijelid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5403 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ijelid/ijelid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.276943 seacrowd-0.0.4/seacrowd/sea_datasets/imdb_jv/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/imdb_jv/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4894 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/imdb_jv/imdb_jv.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.294209 seacrowd-0.0.4/seacrowd/sea_datasets/indo4b/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo4b/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7236 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo4b/indo4b.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.312885 seacrowd-0.0.4/seacrowd/sea_datasets/indo4b_plus/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo4b_plus/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7417 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.331683 seacrowd-0.0.4/seacrowd/sea_datasets/indo_general_mt_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo_general_mt_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6442 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.348776 seacrowd-0.0.4/seacrowd/sea_datasets/indo_law/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo_law/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5445 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo_law/indo_law.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.364376 seacrowd-0.0.4/seacrowd/sea_datasets/indo_puisi/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo_puisi/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4018 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo_puisi/indo_puisi.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.381523 seacrowd-0.0.4/seacrowd/sea_datasets/indo_religious_mt_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo_religious_mt_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8507 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.401333 seacrowd-0.0.4/seacrowd/sea_datasets/indo_story_cloze/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo_story_cloze/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6563 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.420818 seacrowd-0.0.4/seacrowd/sea_datasets/indocamrest/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indocamrest/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6670 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indocamrest/indocamrest.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.440228 seacrowd-0.0.4/seacrowd/sea_datasets/indocollex/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indocollex/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6949 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indocollex/indocollex.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.456485 seacrowd-0.0.4/seacrowd/sea_datasets/indocoref/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indocoref/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11610 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indocoref/indocoref.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.492402 seacrowd-0.0.4/seacrowd/sea_datasets/indocoref/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indocoref/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9072 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indocoref/utils/feature_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2091 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indocoref/utils/file_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4307 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.509939 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ner_ugm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ner_ugm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6402 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.528748 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_nerui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_nerui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8192 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.546272 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ntp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ntp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5885 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.563003 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12679 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.582857 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_tweet_ordering/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_tweet_ordering/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12454 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.602011 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ud_id_gsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ud_id_gsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8462 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.621281 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ud_id_pud/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ud_id_pud/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8825 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.638353 seacrowd-0.0.4/seacrowd/sea_datasets/indoler/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indoler/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9100 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indoler/indoler.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.654767 seacrowd-0.0.4/seacrowd/sea_datasets/indommlu/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indommlu/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10934 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indommlu/indommlu.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.672737 seacrowd-0.0.4/seacrowd/sea_datasets/indoner_tourism/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indoner_tourism/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8394 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.687621 seacrowd-0.0.4/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5250 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.703906 seacrowd-0.0.4/seacrowd/sea_datasets/indonesian_madurese_bible_translation/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonesian_madurese_bible_translation/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7932 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.720143 seacrowd-0.0.4/seacrowd/sea_datasets/indonesian_news_dataset/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonesian_news_dataset/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4581 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.738376 seacrowd-0.0.4/seacrowd/sea_datasets/indonesiannmt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonesiannmt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9148 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.754926 seacrowd-0.0.4/seacrowd/sea_datasets/indonglish/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonglish/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8339 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonglish/indonglish.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.771526 seacrowd-0.0.4/seacrowd/sea_datasets/indonli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8050 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonli/indonli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.789770 seacrowd-0.0.4/seacrowd/sea_datasets/indonlu_nergrit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonlu_nergrit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5677 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.806389 seacrowd-0.0.4/seacrowd/sea_datasets/indoqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indoqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5422 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indoqa/indoqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.823779 seacrowd-0.0.4/seacrowd/sea_datasets/indosmd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indosmd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13550 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indosmd/indosmd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.851438 seacrowd-0.0.4/seacrowd/sea_datasets/indosum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indosum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6872 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indosum/indosum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.868282 seacrowd-0.0.4/seacrowd/sea_datasets/indotacos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indotacos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indotacos/indotacos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.884566 seacrowd-0.0.4/seacrowd/sea_datasets/indowiki/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indowiki/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7684 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indowiki/indowiki.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.906839 seacrowd-0.0.4/seacrowd/sea_datasets/indqner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indqner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6614 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indqner/indqner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.923018 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_digit_cdsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_digit_cdsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9856 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.946619 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_news_ethnicsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_news_ethnicsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8440 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.964781 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_news_lvcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_news_lvcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9432 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:22.988957 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_news_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_news_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8857 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.009079 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11615 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.033349 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9932 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.061680 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_teldialog_svcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_teldialog_svcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9818 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.089820 seacrowd-0.0.4/seacrowd/sea_datasets/inset_lexicon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/inset_lexicon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4829 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.113044 seacrowd-0.0.4/seacrowd/sea_datasets/jadi_ide/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/jadi_ide/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4404 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/jadi_ide/jadi_ide.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.134142 seacrowd-0.0.4/seacrowd/sea_datasets/jv_id_asr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/jv_id_asr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6236 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.154514 seacrowd-0.0.4/seacrowd/sea_datasets/jv_id_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/jv_id_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7628 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.187178 seacrowd-0.0.4/seacrowd/sea_datasets/kamus_alay/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kamus_alay/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5286 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kamus_alay/kamus_alay.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.214964 seacrowd-0.0.4/seacrowd/sea_datasets/karonese_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/karonese_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4533 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.238361 seacrowd-0.0.4/seacrowd/sea_datasets/kawat/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kawat/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5933 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kawat/kawat.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.253407 seacrowd-0.0.4/seacrowd/sea_datasets/kde4/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kde4/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14408 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kde4/kde4.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.276285 seacrowd-0.0.4/seacrowd/sea_datasets/keps/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/keps/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5066 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/keps/keps.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.298191 seacrowd-0.0.4/seacrowd/sea_datasets/kheng_info/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kheng_info/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3687 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kheng_info/kheng_info.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.321029 seacrowd-0.0.4/seacrowd/sea_datasets/khmer_alt_pos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/khmer_alt_pos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7442 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.344369 seacrowd-0.0.4/seacrowd/sea_datasets/khpos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/khpos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8756 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/khpos/khpos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.367096 seacrowd-0.0.4/seacrowd/sea_datasets/kopi_cc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kopi_cc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10035 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kopi_cc/kopi_cc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.389291 seacrowd-0.0.4/seacrowd/sea_datasets/kopi_cc_news/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kopi_cc_news/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5088 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.417723 seacrowd-0.0.4/seacrowd/sea_datasets/kopi_nllb/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kopi_nllb/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5956 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.444452 seacrowd-0.0.4/seacrowd/sea_datasets/korpus_nusantara/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/korpus_nusantara/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8476 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.462373 seacrowd-0.0.4/seacrowd/sea_datasets/lazada_review_filipino/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/lazada_review_filipino/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4913 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.480752 seacrowd-0.0.4/seacrowd/sea_datasets/librivox_indonesia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/librivox_indonesia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8736 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.499602 seacrowd-0.0.4/seacrowd/sea_datasets/limesoda/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/limesoda/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6775 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/limesoda/limesoda.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.525160 seacrowd-0.0.4/seacrowd/sea_datasets/liputan6/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/liputan6/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7512 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/liputan6/liputan6.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.543162 seacrowd-0.0.4/seacrowd/sea_datasets/local_id_abusive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/local_id_abusive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7530 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.560205 seacrowd-0.0.4/seacrowd/sea_datasets/lr_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/lr_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6160 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/lr_sum/lr_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.578273 seacrowd-0.0.4/seacrowd/sea_datasets/m3exam/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/m3exam/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14637 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/m3exam/m3exam.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.595930 seacrowd-0.0.4/seacrowd/sea_datasets/mabl/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mabl/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8609 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mabl/mabl.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.612746 seacrowd-0.0.4/seacrowd/sea_datasets/malaysia_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/malaysia_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6432 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.629805 seacrowd-0.0.4/seacrowd/sea_datasets/malindo_morph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/malindo_morph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4617 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/malindo_morph/malindo_morph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.645898 seacrowd-0.0.4/seacrowd/sea_datasets/malindo_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/malindo_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6494 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.663749 seacrowd-0.0.4/seacrowd/sea_datasets/massive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/massive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    18420 2024-04-04 06:00:48.000000 seacrowd-0.0.4/seacrowd/sea_datasets/massive/massive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.681695 seacrowd-0.0.4/seacrowd/sea_datasets/mc4_indo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mc4_indo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5510 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mc4_indo/mc4_indo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.698992 seacrowd-0.0.4/seacrowd/sea_datasets/melayu_brunei/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/melayu_brunei/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10682 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.717818 seacrowd-0.0.4/seacrowd/sea_datasets/melayu_sabah/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/melayu_sabah/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5561 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.733285 seacrowd-0.0.4/seacrowd/sea_datasets/melayu_sarawak/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/melayu_sarawak/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6559 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.758029 seacrowd-0.0.4/seacrowd/sea_datasets/melayu_standard_lisan/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/melayu_standard_lisan/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7594 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.776048 seacrowd-0.0.4/seacrowd/sea_datasets/memolon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/memolon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5589 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/memolon/memolon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.791790 seacrowd-0.0.4/seacrowd/sea_datasets/minangnlp_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/minangnlp_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6874 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.808242 seacrowd-0.0.4/seacrowd/sea_datasets/miracl/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/miracl/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13119 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/miracl/miracl.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.825668 seacrowd-0.0.4/seacrowd/sea_datasets/mkqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mkqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8345 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mkqa/mkqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.846071 seacrowd-0.0.4/seacrowd/sea_datasets/mlqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mlqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9825 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mlqa/mlqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.863626 seacrowd-0.0.4/seacrowd/sea_datasets/mozilla_pontoon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mozilla_pontoon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6211 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.881650 seacrowd-0.0.4/seacrowd/sea_datasets/mswc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mswc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8048 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mswc/mswc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.910021 seacrowd-0.0.4/seacrowd/sea_datasets/mtop_intent_classification/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mtop_intent_classification/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2654 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mtop_intent_classification/labels.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5662 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.928288 seacrowd-0.0.4/seacrowd/sea_datasets/multilexnorm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/multilexnorm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6223 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/multilexnorm/multilexnorm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.944896 seacrowd-0.0.4/seacrowd/sea_datasets/my_paraphrase/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/my_paraphrase/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8124 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.965365 seacrowd-0.0.4/seacrowd/sea_datasets/myanmar_rakhine_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/myanmar_rakhine_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7223 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:23.983053 seacrowd-0.0.4/seacrowd/sea_datasets/mypos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mypos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5116 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mypos/mypos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.005128 seacrowd-0.0.4/seacrowd/sea_datasets/mysentence/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mysentence/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7612 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/mysentence/mysentence.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.024709 seacrowd-0.0.4/seacrowd/sea_datasets/myxnli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/myxnli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5096 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/myxnli/myxnli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.043096 seacrowd-0.0.4/seacrowd/sea_datasets/nergrit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nergrit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6322 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nergrit/nergrit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.064313 seacrowd-0.0.4/seacrowd/sea_datasets/nerp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nerp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4852 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nerp/nerp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.081075 seacrowd-0.0.4/seacrowd/sea_datasets/netifier/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/netifier/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4838 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/netifier/netifier.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.097939 seacrowd-0.0.4/seacrowd/sea_datasets/news_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/news_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5003 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/news_en_id/news_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.117177 seacrowd-0.0.4/seacrowd/sea_datasets/newsph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/newsph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3810 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/newsph/newsph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.134200 seacrowd-0.0.4/seacrowd/sea_datasets/nllb_seed/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nllb_seed/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15208 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nllb_seed/nllb_seed.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.153575 seacrowd-0.0.4/seacrowd/sea_datasets/ntrex_128/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ntrex_128/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10971 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ntrex_128/ntrex_128.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.171618 seacrowd-0.0.4/seacrowd/sea_datasets/nusaparagraph_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusaparagraph_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8785 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.191630 seacrowd-0.0.4/seacrowd/sea_datasets/nusaparagraph_rhetoric/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusaparagraph_rhetoric/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8792 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.209720 seacrowd-0.0.4/seacrowd/sea_datasets/nusaparagraph_topic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusaparagraph_topic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8845 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.232067 seacrowd-0.0.4/seacrowd/sea_datasets/nusatranslation_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusatranslation_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.250133 seacrowd-0.0.4/seacrowd/sea_datasets/nusatranslation_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusatranslation_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9156 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.269749 seacrowd-0.0.4/seacrowd/sea_datasets/nusatranslation_senti/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusatranslation_senti/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8285 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.287023 seacrowd-0.0.4/seacrowd/sea_datasets/nusax_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusax_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7578 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusax_mt/nusax_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.304363 seacrowd-0.0.4/seacrowd/sea_datasets/nusax_senti/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusax_senti/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7250 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/nusax_senti/nusax_senti.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.318639 seacrowd-0.0.4/seacrowd/sea_datasets/oil/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/oil/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/oil/oil.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.336365 seacrowd-0.0.4/seacrowd/sea_datasets/ojw/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ojw/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5110 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ojw/ojw.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.355300 seacrowd-0.0.4/seacrowd/sea_datasets/openlid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/openlid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7915 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/openlid/openlid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.372398 seacrowd-0.0.4/seacrowd/sea_datasets/openslr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/openslr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10343 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/openslr/openslr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.389824 seacrowd-0.0.4/seacrowd/sea_datasets/orchid_pos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/orchid_pos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9625 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/orchid_pos/orchid_pos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.408023 seacrowd-0.0.4/seacrowd/sea_datasets/oscar_2201/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/oscar_2201/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    16270 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/oscar_2201/oscar_2201.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.427850 seacrowd-0.0.4/seacrowd/sea_datasets/palito/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/palito/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5930 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/palito/palito.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.444259 seacrowd-0.0.4/seacrowd/sea_datasets/paracotta_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/paracotta_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4768 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/paracotta_id/paracotta_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.458819 seacrowd-0.0.4/seacrowd/sea_datasets/parallel_id_nyo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/parallel_id_nyo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5471 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.475161 seacrowd-0.0.4/seacrowd/sea_datasets/parallel_su_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/parallel_su_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4782 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.492795 seacrowd-0.0.4/seacrowd/sea_datasets/ph_fake_news_corpus/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ph_fake_news_corpus/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4339 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.509848 seacrowd-0.0.4/seacrowd/sea_datasets/pho_ner_covid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/pho_ner_covid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6866 2024-04-04 06:00:49.000000 seacrowd-0.0.4/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.527628 seacrowd-0.0.4/seacrowd/sea_datasets/phomt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/phomt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5141 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/phomt/phomt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.545356 seacrowd-0.0.4/seacrowd/sea_datasets/phost/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/phost/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9498 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/phost/phost.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.563150 seacrowd-0.0.4/seacrowd/sea_datasets/posp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/posp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5990 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/posp/posp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.580557 seacrowd-0.0.4/seacrowd/sea_datasets/postag_su/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/postag_su/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8033 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/postag_su/postag_su.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.599657 seacrowd-0.0.4/seacrowd/sea_datasets/prdect_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/prdect_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7572 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/prdect_id/prdect_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.618869 seacrowd-0.0.4/seacrowd/sea_datasets/qasina/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/qasina/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6424 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/qasina/qasina.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.636290 seacrowd-0.0.4/seacrowd/sea_datasets/roots_vi_ted/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/roots_vi_ted/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5065 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.653999 seacrowd-0.0.4/seacrowd/sea_datasets/sampiran/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sampiran/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5024 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sampiran/sampiran.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.672085 seacrowd-0.0.4/seacrowd/sea_datasets/sap_wat/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sap_wat/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7077 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sap_wat/sap_wat.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.691417 seacrowd-0.0.4/seacrowd/sea_datasets/sarawak_malay/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sarawak_malay/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7381 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.708010 seacrowd-0.0.4/seacrowd/sea_datasets/scb_mt_en_th/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/scb_mt_en_th/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7071 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.724656 seacrowd-0.0.4/seacrowd/sea_datasets/sea_bench/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sea_bench/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7206 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sea_bench/sea_bench.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.742625 seacrowd-0.0.4/seacrowd/sea_datasets/sea_madlad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sea_madlad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10051 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sea_madlad/sea_madlad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.758901 seacrowd-0.0.4/seacrowd/sea_datasets/sea_wiki/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sea_wiki/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sea_wiki/sea_wiki.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.778221 seacrowd-0.0.4/seacrowd/sea_datasets/seaeval/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/seaeval/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/seaeval/seaeval.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.796483 seacrowd-0.0.4/seacrowd/sea_datasets/seahorse/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/seahorse/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6884 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/seahorse/seahorse.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.813222 seacrowd-0.0.4/seacrowd/sea_datasets/sentiment_nathasa_review/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sentiment_nathasa_review/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6002 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.830174 seacrowd-0.0.4/seacrowd/sea_datasets/shopee_reviews_tagalog/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/shopee_reviews_tagalog/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4597 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.849634 seacrowd-0.0.4/seacrowd/sea_datasets/singgalang/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/singgalang/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5430 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/singgalang/singgalang.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.867849 seacrowd-0.0.4/seacrowd/sea_datasets/smsa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/smsa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5575 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/smsa/smsa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.886063 seacrowd-0.0.4/seacrowd/sea_datasets/snli_indo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/snli_indo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6244 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/snli_indo/snli_indo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.903223 seacrowd-0.0.4/seacrowd/sea_datasets/spamid_pair/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/spamid_pair/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5524 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/spamid_pair/spamid_pair.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.921438 seacrowd-0.0.4/seacrowd/sea_datasets/squad_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/squad_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5315 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/squad_id/squad_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.938543 seacrowd-0.0.4/seacrowd/sea_datasets/stb_ext/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/stb_ext/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9273 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/stb_ext/stb_ext.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.956407 seacrowd-0.0.4/seacrowd/sea_datasets/stif_indonesia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/stif_indonesia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5135 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.973735 seacrowd-0.0.4/seacrowd/sea_datasets/struct_amb_ind/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/struct_amb_ind/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7724 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:24.991233 seacrowd-0.0.4/seacrowd/sea_datasets/su_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/su_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4567 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/su_emot/su_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.008884 seacrowd-0.0.4/seacrowd/sea_datasets/su_id_asr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/su_id_asr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5601 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/su_id_asr/su_id_asr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.026378 seacrowd-0.0.4/seacrowd/sea_datasets/su_id_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/su_id_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/su_id_tts/su_id_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.041200 seacrowd-0.0.4/seacrowd/sea_datasets/talpco/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/talpco/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6870 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/talpco/talpco.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.059031 seacrowd-0.0.4/seacrowd/sea_datasets/tatabahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tatabahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5411 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tatabahasa/tatabahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.075835 seacrowd-0.0.4/seacrowd/sea_datasets/tatoeba/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tatoeba/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tatoeba/tatoeba.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.093428 seacrowd-0.0.4/seacrowd/sea_datasets/tcope/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tcope/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6693 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tcope/tcope.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.111996 seacrowd-0.0.4/seacrowd/sea_datasets/ted_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ted_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7105 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ted_en_id/ted_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.132335 seacrowd-0.0.4/seacrowd/sea_datasets/term_a/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/term_a/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5358 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/term_a/term_a.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.151390 seacrowd-0.0.4/seacrowd/sea_datasets/tgl_profanity/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tgl_profanity/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4351 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.168410 seacrowd-0.0.4/seacrowd/sea_datasets/tha_lao_embassy_parcor/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tha_lao_embassy_parcor/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4436 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.185970 seacrowd-0.0.4/seacrowd/sea_datasets/thai_alpaca/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_alpaca/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3943 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.201878 seacrowd-0.0.4/seacrowd/sea_datasets/thai_constitution/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_constitution/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10954 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_constitution/thai_constitution.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.220299 seacrowd-0.0.4/seacrowd/sea_datasets/thai_databricks_dolly/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_databricks_dolly/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4388 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.237702 seacrowd-0.0.4/seacrowd/sea_datasets/thai_depression/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_depression/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5739 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_depression/thai_depression.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.256124 seacrowd-0.0.4/seacrowd/sea_datasets/thai_gpteacher/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_gpteacher/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3960 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.272784 seacrowd-0.0.4/seacrowd/sea_datasets/thai_hh_rlhf/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_hh_rlhf/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5077 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.296076 seacrowd-0.0.4/seacrowd/sea_datasets/thai_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5683 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_sum/thai_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.313160 seacrowd-0.0.4/seacrowd/sea_datasets/thai_toxicity_tweet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_toxicity_tweet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.331356 seacrowd-0.0.4/seacrowd/sea_datasets/tico_19/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tico_19/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12192 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tico_19/tico_19.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.348505 seacrowd-0.0.4/seacrowd/sea_datasets/titml_idn/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/titml_idn/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/titml_idn/titml_idn.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.366677 seacrowd-0.0.4/seacrowd/sea_datasets/tlunified_ner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tlunified_ner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5800 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.381940 seacrowd-0.0.4/seacrowd/sea_datasets/toxicity_200/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/toxicity_200/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5975 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/toxicity_200/toxicity_200.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.399685 seacrowd-0.0.4/seacrowd/sea_datasets/tydiqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tydiqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23881 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/tydiqa/tydiqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.420109 seacrowd-0.0.4/seacrowd/sea_datasets/typhoon_yolanda_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/typhoon_yolanda_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5165 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.435764 seacrowd-0.0.4/seacrowd/sea_datasets/ucla_phonetic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ucla_phonetic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6531 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.452189 seacrowd-0.0.4/seacrowd/sea_datasets/ud_id_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ud_id_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9185 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.469703 seacrowd-0.0.4/seacrowd/sea_datasets/ud_jv_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ud_jv_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10052 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.488026 seacrowd-0.0.4/seacrowd/sea_datasets/udhr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/udhr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6030 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/udhr/udhr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.504994 seacrowd-0.0.4/seacrowd/sea_datasets/udhr_lid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/udhr_lid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5190 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/udhr_lid/udhr_lid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.521348 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vicov19qa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vicov19qa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7244 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.537813 seacrowd-0.0.4/seacrowd/sea_datasets/uit_victsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_victsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5311 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_victsd/uit_victsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.552942 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vihsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vihsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5721 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.571379 seacrowd-0.0.4/seacrowd/sea_datasets/uit_viic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_viic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6572 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_viic/uit_viic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.588124 seacrowd-0.0.4/seacrowd/sea_datasets/uit_viocd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_viocd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_viocd/uit_viocd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.603900 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vion/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vion/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5939 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vion/uit_vion.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.622498 seacrowd-0.0.4/seacrowd/sea_datasets/uit_visd4sa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_visd4sa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7034 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.638120 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vsfc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vsfc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8715 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.655036 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vsmec/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vsmec/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4802 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.672324 seacrowd-0.0.4/seacrowd/sea_datasets/unimorph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/unimorph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15492 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/unimorph/unimorph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.689288 seacrowd-0.0.4/seacrowd/sea_datasets/unimorph_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/unimorph_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7445 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/unimorph_id/unimorph_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.707873 seacrowd-0.0.4/seacrowd/sea_datasets/vi_pubmed/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vi_pubmed/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15136 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.722857 seacrowd-0.0.4/seacrowd/sea_datasets/vihealthqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vihealthqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5587 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vihealthqa/vihealthqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.741485 seacrowd-0.0.4/seacrowd/sea_datasets/visobert/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/visobert/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6265 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/visobert/visobert.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.758966 seacrowd-0.0.4/seacrowd/sea_datasets/vispamreviews/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vispamreviews/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7245 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vispamreviews/vispamreviews.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.776175 seacrowd-0.0.4/seacrowd/sea_datasets/vistec_tp_th_21/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vistec_tp_th_21/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6739 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.794479 seacrowd-0.0.4/seacrowd/sea_datasets/vitext2sql/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vitext2sql/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6893 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vitext2sql/vitext2sql.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.811170 seacrowd-0.0.4/seacrowd/sea_datasets/vivos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vivos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7832 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vivos/vivos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.826814 seacrowd-0.0.4/seacrowd/sea_datasets/vivqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vivqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9080 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vivqa/vivqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.843715 seacrowd-0.0.4/seacrowd/sea_datasets/vlsp2016_ner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vlsp2016_ner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5857 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.860860 seacrowd-0.0.4/seacrowd/sea_datasets/vlsp2016_sa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vlsp2016_sa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7134 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.888918 seacrowd-0.0.4/seacrowd/sea_datasets/vndt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vndt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2232 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vndt/utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7852 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/vndt/vndt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.907219 seacrowd-0.0.4/seacrowd/sea_datasets/voxlingua/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/voxlingua/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7980 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/voxlingua/voxlingua.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.924189 seacrowd-0.0.4/seacrowd/sea_datasets/weathub/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/weathub/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7521 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/weathub/weathub.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.940853 seacrowd-0.0.4/seacrowd/sea_datasets/wikiann/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wikiann/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8643 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wikiann/wikiann.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.956858 seacrowd-0.0.4/seacrowd/sea_datasets/wikilingua/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wikilingua/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4984 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wikilingua/wikilingua.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.972444 seacrowd-0.0.4/seacrowd/sea_datasets/wikimatrix/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wikimatrix/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8585 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wikimatrix/wikimatrix.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:25.991433 seacrowd-0.0.4/seacrowd/sea_datasets/wikitext_tl_39/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wikitext_tl_39/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3663 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.008311 seacrowd-0.0.4/seacrowd/sea_datasets/wili_2018/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wili_2018/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6699 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wili_2018/wili_2018.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.025557 seacrowd-0.0.4/seacrowd/sea_datasets/wisesight_thai_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wisesight_thai_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7027 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.043786 seacrowd-0.0.4/seacrowd/sea_datasets/wit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12057 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wit/wit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.060925 seacrowd-0.0.4/seacrowd/sea_datasets/wongnai_reviews/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wongnai_reviews/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4106 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.078159 seacrowd-0.0.4/seacrowd/sea_datasets/wrete/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wrete/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6113 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/wrete/wrete.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.093860 seacrowd-0.0.4/seacrowd/sea_datasets/x_fact/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/x_fact/__init__.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.110118 seacrowd-0.0.4/seacrowd/sea_datasets/x_fact/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/x_fact/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      473 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/x_fact/utils/x_fact_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/x_fact/x_fact.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.128452 seacrowd-0.0.4/seacrowd/sea_datasets/xcopa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xcopa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7024 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xcopa/xcopa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.145867 seacrowd-0.0.4/seacrowd/sea_datasets/xl_jailbreak/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xl_jailbreak/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6317 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.163125 seacrowd-0.0.4/seacrowd/sea_datasets/xl_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xl_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6903 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xl_sum/xl_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.181376 seacrowd-0.0.4/seacrowd/sea_datasets/xm3600/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xm3600/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-11 08:39:41.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xm3600/xm3600.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.199097 seacrowd-0.0.4/seacrowd/sea_datasets/xnli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xnli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8333 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xnli/xnli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.215757 seacrowd-0.0.4/seacrowd/sea_datasets/xpersona_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xpersona_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6550 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xpersona_id/xpersona_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.235263 seacrowd-0.0.4/seacrowd/sea_datasets/xquad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xquad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xquad/xquad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.254917 seacrowd-0.0.4/seacrowd/sea_datasets/xsid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xsid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9510 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xsid/xsid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.274150 seacrowd-0.0.4/seacrowd/sea_datasets/xstorycloze/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xstorycloze/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6794 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/sea_datasets/xstorycloze/xstorycloze.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.292810 seacrowd-0.0.4/seacrowd/sea_datasets/yunshan_cup_2020/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/sea_datasets/yunshan_cup_2020/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5828 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.324565 seacrowd-0.0.4/seacrowd/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5493 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/common_parser.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      284 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/configs.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12786 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/constants.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.522711 seacrowd-0.0.4/seacrowd/utils/schemas/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1485 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      506 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/image_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1101 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/imqa.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2283 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/kb.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      626 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/pairs.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      371 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/pairs_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1007 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/qa.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      206 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/self_supervised_pretraining.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      525 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/seq_label.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      618 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/speech.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      606 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/speech_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      454 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/speech_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      796 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/speech_to_speech.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      311 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      331 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/text_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      444 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/text_to_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3046 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/tod.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3068 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/tree.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      810 2024-04-04 06:00:52.000000 seacrowd-0.0.4/seacrowd/utils/schemas/video.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.561900 seacrowd-0.0.4/seacrowd.egg-info/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-11 09:04:18.000000 seacrowd-0.0.4/seacrowd.egg-info/PKG-INFO
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    31277 2024-04-11 09:04:19.000000 seacrowd-0.0.4/seacrowd.egg-info/SOURCES.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-11 09:04:18.000000 seacrowd-0.0.4/seacrowd.egg-info/dependency_links.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      409 2024-04-11 09:04:18.000000 seacrowd-0.0.4/seacrowd.egg-info/requires.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       15 2024-04-11 09:04:18.000000 seacrowd-0.0.4/seacrowd.egg-info/top_level.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      666 2024-04-11 09:04:26.588944 seacrowd-0.0.4/setup.cfg
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       68 2024-04-04 06:00:52.000000 seacrowd-0.0.4/setup.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:04:26.549103 seacrowd-0.0.4/tests/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.4/tests/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23314 2024-04-04 06:00:52.000000 seacrowd-0.0.4/tests/test_seacrowd.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    20714 2024-04-04 06:00:52.000000 seacrowd-0.0.4/tests/test_seacrowd_source_only.py
```

### Comparing `seacrowd-0.0.3/LICENSE` & `seacrowd-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/PKG-INFO` & `seacrowd-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seacrowd
-Version: 0.0.3
+Version: 0.0.4
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: bioc>=1.3.7
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: datasets>=2.2.0
```

### Comparing `seacrowd-0.0.3/README.md` & `seacrowd-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/config_helper.py` & `seacrowd-0.0.4/seacrowd/config_helper.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/ara_close/ara_close.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/ara_close/ara_close.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/aya_dataset/aya_dataset.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/aya_dataset/aya_dataset.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/barasa/barasa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/barasa/barasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/belebele/belebele.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/belebele/belebele.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/bible_en_id/bible_en_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/bible_en_id/bible_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/bible_su_id/bible_su_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/bible_su_id/bible_su_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/bioner_id/bioner_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/bioner_id/bioner_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/bloom_lm/bloom_lm.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/bloom_lm/bloom_lm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/bloom_speech/bloom_speech.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/bloom_speech/bloom_speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/bloom_vist/bloom_vist.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/bloom_vist/bloom_vist.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/burapha_th/burapha_th.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/burapha_th/burapha_th.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/casa/casa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/casa/casa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/cc100/cc100.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/cc100/cc100.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/cebuaner/cebuaner.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/cebuaner/cebuaner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/coco_35l/coco_35l.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/coco_35l/coco_35l.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/cod/cod.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/cod/cod.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/copal/copal.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/copal/copal.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/covost2/covost2.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/covost2/covost2.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/creole_rc/creole_rc.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/creole_rc/creole_rc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/crosssum/crosssum.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/crosssum/crosssum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/culturax/culturax.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/culturax/culturax.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/cvss/cvss.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/cvss/cvss.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/emot/emot.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/emot/emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/emotcmt/emotcmt.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/emotcmt/emotcmt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/emotes_3k/emotes_3k.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/emotes_3k/emotes_3k.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/etos/etos.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/etos/etos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/facqa/facqa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/facqa/facqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/facqa/utils/facqa_utils.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/facqa/utils/facqa_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/filwordnet/filwordnet.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/filwordnet/filwordnet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/fleurs/fleurs.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/fleurs/fleurs.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,24 +26,25 @@
   doi={10.21437/Interspeech.2022-10007}
 }
 """
 
 logger = datasets.logging.get_logger(__name__)
 
 
-with open(DownloadManager().download_and_extract("seacrowd/sea_datasets/fleurs/lang_config.json"), "r") as f:
-    _LANG_CONFIG = json.load(f)
-
 _LOCAL = False
-_LANGUAGES = list(_LANG_CONFIG.keys())
 
 # since this fleurs source already subsets SEA langs, the names on lang group id is hard-coded
 _LANG_GROUP_ID = ["south_east_asian_sea"]
 
 _DATASETNAME = "fleurs"
+
+with open(DownloadManager().download_and_extract(f"./seacrowd/sea_datasets/{_DATASETNAME}/lang_config.json"), "r") as f:
+    _LANG_CONFIG = json.load(f)
+_LANGUAGES = list(_LANG_CONFIG.keys())
+
 _DESCRIPTION = """\
     Fleurs dataset is a part of XTREME-S benchmark to evaluate universal cross-lingual speech representations in many languages.
     Fleurs is used for two tasks: automatic speech recognition and speech classification.
     Fleurs covers 10 language native to Southeast Asian and other 3 major languages
     mostly spoken in few of Southeast Asia countries (Mandarin Chinese, Portuguese, and Tamil).
 """
```

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/flores200/flores200.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/flores200/flores200.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/fsl_105/fsl_105.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/fsl_105/fsl_105.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/gatitos/gatitos.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/gatitos/gatitos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/globalwoz/globalwoz.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/globalwoz/globalwoz.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/glotstorybook/glotstorybook.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/glotstorybook/glotstorybook.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/hoasa/hoasa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/hoasa/hoasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/iapp_squad/iapp_squad.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/iapp_squad/iapp_squad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/iatf/iatf.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/iatf/iatf.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/icon/icon.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/icon/icon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_abusive/id_abusive.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_abusive/id_abusive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_am2ico/id_am2ico.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_am2ico/id_am2ico.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_clickbait/id_clickbait.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_clickbait/id_clickbait.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_frog_story/id_frog_story.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_frog_story/id_frog_story.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_msvd/id_msvd.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_msvd/id_msvd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_qqp/id_qqp.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_qqp/id_qqp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_stance/id_stance.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_stance/id_stance.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_sts/id_sts.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_sts/id_sts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/id_wsd/id_wsd.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/id_wsd/id_wsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/identic/identic.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/identic/identic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/idk_mrc/idk_mrc.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/idk_mrc/idk_mrc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/ijelid/ijelid.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/ijelid/ijelid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/imdb_jv/imdb_jv.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/imdb_jv/imdb_jv.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indo4b/indo4b.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indo4b/indo4b.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indo_law/indo_law.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indo_law/indo_law.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indo_puisi/indo_puisi.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indo_puisi/indo_puisi.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indocamrest/indocamrest.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indocamrest/indocamrest.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indocollex/indocollex.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indocollex/indocollex.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indocoref/indocoref.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indocoref/indocoref.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indocoref/utils/feature_utils.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indocoref/utils/feature_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indocoref/utils/file_utils.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indocoref/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indoler/indoler.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indoler/indoler.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indommlu/indommlu.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indommlu/indommlu.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indonglish/indonglish.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indonglish/indonglish.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indonli/indonli.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indonli/indonli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indoqa/indoqa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indoqa/indoqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indosmd/indosmd.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indosmd/indosmd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indosum/indosum.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indosum/indosum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indotacos/indotacos.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indotacos/indotacos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indowiki/indowiki.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indowiki/indowiki.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indqner/indqner.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indqner/indqner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/jadi_ide/jadi_ide.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/jadi_ide/jadi_ide.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/kamus_alay/kamus_alay.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/kamus_alay/kamus_alay.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/kawat/kawat.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/kawat/kawat.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/kde4/kde4.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/kde4/kde4.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/keps/keps.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/keps/keps.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/kheng_info/kheng_info.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/kheng_info/kheng_info.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/khpos/khpos.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/khpos/khpos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/kopi_cc/kopi_cc.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/kopi_cc/kopi_cc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/limesoda/limesoda.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/limesoda/limesoda.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/liputan6/liputan6.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/liputan6/liputan6.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/lr_sum/lr_sum.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/lr_sum/lr_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/m3exam/m3exam.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/m3exam/m3exam.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/mabl/mabl.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/mabl/mabl.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/malindo_morph/malindo_morph.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/malindo_morph/malindo_morph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/massive/massive.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/massive/massive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/mc4_indo/mc4_indo.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/mc4_indo/mc4_indo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/memolon/memolon.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/memolon/memolon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/miracl/miracl.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/miracl/miracl.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/mkqa/mkqa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/mkqa/mkqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/mlqa/mlqa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/mlqa/mlqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/mswc/mswc.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/mswc/mswc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/mtop_intent_classification/labels.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/mtop_intent_classification/labels.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/multilexnorm/multilexnorm.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/multilexnorm/multilexnorm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/mypos/mypos.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/mypos/mypos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/mysentence/mysentence.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/mysentence/mysentence.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/myxnli/myxnli.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/myxnli/myxnli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/nergrit/nergrit.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/nergrit/nergrit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/nerp/nerp.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/nerp/nerp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/netifier/netifier.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/netifier/netifier.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/news_en_id/news_en_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/news_en_id/news_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/newsph/newsph.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/newsph/newsph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/nllb_seed/nllb_seed.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/nllb_seed/nllb_seed.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/ntrex_128/ntrex_128.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/ntrex_128/ntrex_128.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/nusax_mt/nusax_mt.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/nusax_mt/nusax_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/nusax_senti/nusax_senti.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/nusax_senti/nusax_senti.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/oil/oil.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/oil/oil.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/ojw/ojw.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/ojw/ojw.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/openlid/openlid.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/openlid/openlid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/openslr/openslr.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/openslr/openslr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/orchid_pos/orchid_pos.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/orchid_pos/orchid_pos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/oscar_2201/oscar_2201.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/oscar_2201/oscar_2201.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/palito/palito.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/palito/palito.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/paracotta_id/paracotta_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/paracotta_id/paracotta_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/phomt/phomt.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/phomt/phomt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/phost/phost.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/phost/phost.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/posp/posp.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/posp/posp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/postag_su/postag_su.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/postag_su/postag_su.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/prdect_id/prdect_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/prdect_id/prdect_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/qasina/qasina.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/qasina/qasina.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/sampiran/sampiran.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/sampiran/sampiran.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/sap_wat/sap_wat.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/sap_wat/sap_wat.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/sea_bench/sea_bench.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/sea_bench/sea_bench.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/sea_madlad/sea_madlad.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/sea_madlad/sea_madlad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/sea_wiki/sea_wiki.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/sea_wiki/sea_wiki.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/seaeval/seaeval.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/seaeval/seaeval.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/seahorse/seahorse.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/seahorse/seahorse.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/singgalang/singgalang.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/singgalang/singgalang.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/smsa/smsa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/smsa/smsa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/snli_indo/snli_indo.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/snli_indo/snli_indo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/spamid_pair/spamid_pair.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/spamid_pair/spamid_pair.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/squad_id/squad_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/squad_id/squad_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/stb_ext/stb_ext.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/stb_ext/stb_ext.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/su_emot/su_emot.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/su_emot/su_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/su_id_asr/su_id_asr.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/su_id_asr/su_id_asr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/su_id_tts/su_id_tts.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/su_id_tts/su_id_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/talpco/talpco.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/talpco/talpco.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/tatabahasa/tatabahasa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/tatabahasa/tatabahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/tatoeba/tatoeba.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/tatoeba/tatoeba.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/tcope/tcope.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/tcope/tcope.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/ted_en_id/ted_en_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/ted_en_id/ted_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/term_a/term_a.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/term_a/term_a.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/thai_constitution/thai_constitution.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/thai_constitution/thai_constitution.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/thai_depression/thai_depression.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/thai_depression/thai_depression.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/thai_sum/thai_sum.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/thai_sum/thai_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/tico_19/tico_19.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/tico_19/tico_19.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/titml_idn/titml_idn.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/titml_idn/titml_idn.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/toxicity_200/toxicity_200.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/toxicity_200/toxicity_200.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/tydiqa/tydiqa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/tydiqa/tydiqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/udhr/udhr.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/udhr/udhr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/udhr_lid/udhr_lid.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/udhr_lid/udhr_lid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/uit_victsd/uit_victsd.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/uit_victsd/uit_victsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/uit_viic/uit_viic.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/uit_viic/uit_viic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/uit_viocd/uit_viocd.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/uit_viocd/uit_viocd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/uit_vion/uit_vion.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/uit_vion/uit_vion.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/unimorph/unimorph.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/unimorph/unimorph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/unimorph_id/unimorph_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/unimorph_id/unimorph_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/vihealthqa/vihealthqa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/vihealthqa/vihealthqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/visobert/visobert.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/visobert/visobert.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/vispamreviews/vispamreviews.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/vispamreviews/vispamreviews.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/vitext2sql/vitext2sql.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/vitext2sql/vitext2sql.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/vivos/vivos.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/vivos/vivos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/vivqa/vivqa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/vivqa/vivqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/vndt/utils.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/vndt/utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/vndt/vndt.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/vndt/vndt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/voxlingua/voxlingua.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/voxlingua/voxlingua.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/weathub/weathub.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/weathub/weathub.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/wikiann/wikiann.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/wikiann/wikiann.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/wikilingua/wikilingua.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/wikilingua/wikilingua.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/wikimatrix/wikimatrix.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/wikimatrix/wikimatrix.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/wili_2018/wili_2018.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/wili_2018/wili_2018.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/wit/wit.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/wit/wit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/wrete/wrete.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/wrete/wrete.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/x_fact/x_fact.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/x_fact/x_fact.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/xcopa/xcopa.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/xcopa/xcopa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/xl_sum/xl_sum.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/xl_sum/xl_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/xm3600/xm3600.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/xm3600/xm3600.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/xnli/xnli.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/xnli/xnli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/xpersona_id/xpersona_id.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/xpersona_id/xpersona_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/xquad/xquad.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/xquad/xquad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/xsid/xsid.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/xsid/xsid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/xstorycloze/xstorycloze.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/xstorycloze/xstorycloze.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py` & `seacrowd-0.0.4/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/common_parser.py` & `seacrowd-0.0.4/seacrowd/utils/common_parser.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/constants.py` & `seacrowd-0.0.4/seacrowd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/schemas/__init__.py` & `seacrowd-0.0.4/seacrowd/utils/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/schemas/imqa.py` & `seacrowd-0.0.4/seacrowd/utils/schemas/imqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/schemas/kb.py` & `seacrowd-0.0.4/seacrowd/utils/schemas/kb.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/schemas/pairs.py` & `seacrowd-0.0.4/seacrowd/utils/schemas/pairs.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/schemas/qa.py` & `seacrowd-0.0.4/seacrowd/utils/schemas/qa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/schemas/seq_label.py` & `seacrowd-0.0.4/seacrowd/utils/schemas/seq_label.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/schemas/speech.py` & `seacrowd-0.0.4/seacrowd/utils/schemas/speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/schemas/speech_multilabel.py` & `seacrowd-0.0.4/seacrowd/utils/schemas/speech_multilabel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/schemas/speech_to_speech.py` & `seacrowd-0.0.4/seacrowd/utils/schemas/speech_to_speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/schemas/tod.py` & `seacrowd-0.0.4/seacrowd/utils/schemas/tod.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/schemas/tree.py` & `seacrowd-0.0.4/seacrowd/utils/schemas/tree.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd/utils/schemas/video.py` & `seacrowd-0.0.4/seacrowd/utils/schemas/video.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/seacrowd.egg-info/PKG-INFO` & `seacrowd-0.0.4/seacrowd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seacrowd
-Version: 0.0.3
+Version: 0.0.4
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: bioc>=1.3.7
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: datasets>=2.2.0
```

### Comparing `seacrowd-0.0.3/seacrowd.egg-info/SOURCES.txt` & `seacrowd-0.0.4/seacrowd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/setup.cfg` & `seacrowd-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/tests/test_seacrowd.py` & `seacrowd-0.0.4/tests/test_seacrowd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.3/tests/test_seacrowd_source_only.py` & `seacrowd-0.0.4/tests/test_seacrowd_source_only.py`

 * *Files identical despite different names*

