# Comparing `tmp/pytun-pmd3-2.0.4.tar.gz` & `tmp/pytun-pmd3-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytun-pmd3-2.0.4.tar", last modified: Thu Apr 11 06:06:51 2024, max compression
+gzip compressed data, was "pytun-pmd3-2.0.5.tar", last modified: Thu Apr 11 06:45:34 2024, max compression
```

## Comparing `pytun-pmd3-2.0.4.tar` & `pytun-pmd3-2.0.5.tar`

### file list

```diff
@@ -1,135 +1,134 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.100358 pytun-pmd3-2.0.4/
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.058734 pytun-pmd3-2.0.4/.git/
--rw-rw-rw-   0        0        0      127 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/FETCH_HEAD
--rw-rw-rw-   0        0        0       41 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/HEAD
--rw-rw-rw-   0        0        0      378 2024-04-11 06:06:01.000000 pytun-pmd3-2.0.4/.git/config
--rw-rw-rw-   0        0        0       73 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/description
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.058734 pytun-pmd3-2.0.4/.git/hooks/
--rw-rw-rw-   0        0        0      478 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/applypatch-msg.sample
--rw-rw-rw-   0        0        0      896 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/commit-msg.sample
--rw-rw-rw-   0        0        0     4726 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/fsmonitor-watchman.sample
--rw-rw-rw-   0        0        0      189 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/post-update.sample
--rw-rw-rw-   0        0        0      424 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/pre-applypatch.sample
--rw-rw-rw-   0        0        0     1649 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/pre-commit.sample
--rw-rw-rw-   0        0        0      416 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/pre-merge-commit.sample
--rw-rw-rw-   0        0        0     1374 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/pre-push.sample
--rw-rw-rw-   0        0        0     4898 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/pre-rebase.sample
--rw-rw-rw-   0        0        0      544 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/pre-receive.sample
--rw-rw-rw-   0        0        0     1492 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/prepare-commit-msg.sample
--rw-rw-rw-   0        0        0     2783 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/push-to-checkout.sample
--rw-rw-rw-   0        0        0     2308 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/sendemail-validate.sample
--rw-rw-rw-   0        0        0     3650 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/update.sample
--rw-rw-rw-   0        0        0     2271 2024-04-11 06:06:49.000000 pytun-pmd3-2.0.4/.git/index
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/info/
--rw-rw-rw-   0        0        0      240 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/info/exclude
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/logs/
--rw-rw-rw-   0        0        0      191 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/logs/HEAD
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.043113 pytun-pmd3-2.0.4/.git/objects/
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/00/
--r--r--r--   0        0        0   185785 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/objects/00/17794f4638f1a1b4e469619a9824accac6ccea
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/05/
--r--r--r--   0        0        0      644 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/0b/
--r--r--r--   0        0        0      207 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/0b/87183182ca91979436d9e9965719d62cda4b12
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/16/
--r--r--r--   0        0        0     4796 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/16/e6a680fefc2fc02952634fce616297c1725157
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/2a/
--r--r--r--   0        0        0   279805 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/2a/b97dba062208bcb6ffc32bef8347d586751038
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/34/
--r--r--r--   0        0        0       51 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/34/0815e53a01e17a3d4682f7d020696fb3a587da
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/48/
--r--r--r--   0        0        0      113 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/48/2f0e082621cd6d9d699c4cdfa55ba322166de4
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/4d/
--r--r--r--   0        0        0       55 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/4d/76d949a3568d0ff1d0f73fe6858f1dfe6af0a6
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/51/
--r--r--r--   0        0        0      597 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/51/caff11e470f0cfa91e2d07b67ccf52a285824e
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/52/
--r--r--r--   0        0        0       55 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/52/06f67ae5433525c632716e1e595eb02e6856ef
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/55/
--r--r--r--   0        0        0     3227 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/objects/55/d441f4a8017b2ea30eae55137c52f2829dba5f
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/56/
--r--r--r--   0        0        0       53 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/56/d9c426af16617a614e2e17ba6e01afe9b2c9c0
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/5f/
--r--r--r--   0        0        0      128 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/5f/8e3b9fcde01a609d1b1e37c79ecf6b8a50d1e3
--r--r--r--   0        0        0      688 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/5f/b524da018127adcf64a2ffa97bf9be86e9ecb2
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/6f/
--r--r--r--   0        0        0      687 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/6f/8a30c5db31dd360fff4542eef776f4ff397144
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/71/
--r--r--r--   0        0        0       55 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/71/beb6065e5d841f0bb2b7a1d0be99436fe906d4
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/77/
--r--r--r--   0        0        0      898 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/77/b5124b5ab694ecdedd659e0ce18d872174afc3
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/7f/
--r--r--r--   0        0        0      126 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/7f/f8524670c0aed9f1a4439279b78a5e7c137f6f
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/81/
--r--r--r--   0        0        0       55 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/81/7d73b0ac42a4dfc956fd81fd9e130a4ab61aaa
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/83/
--r--r--r--   0        0        0      387 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/83/36f281235488a0f2cca5aeca510a71efc4a7da
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/89/
--r--r--r--   0        0        0     5346 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/89/ee237a05bde1829e0487347488ad23244ebfea
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/ae/
--r--r--r--   0        0        0   209806 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/objects/ae/e04e77bfbd6601adbcd5a46435f059e31cf6e4
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/af/
--r--r--r--   0        0        0       51 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/af/348689d62b32e0021ab0d82c0f8fc156db4728
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/b5/
--r--r--r--   0        0        0      128 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/b5/77e4de768ad66f0d36c258491c30b8f89d64a0
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/bc/
--r--r--r--   0        0        0     2554 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/bc/8d3f0e60565567a8b8598972614dce7d4ffccd
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/c0/
--r--r--r--   0        0        0      107 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/c0/26fe934c3c8d26d252e3541da2d4fe539a7503
--r--r--r--   0        0        0      289 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/objects/c0/93c88fd653a207aea042daeabd98f6666ed72a
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/c5/
--r--r--r--   0        0        0      150 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/c5/8a3c8a6e3b698ea353d97545c477154a0d3e0b
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/d7/
--r--r--r--   0        0        0      151 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/d7/600902847a6ed081b86ebb3ac97ce1c242c4df
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/dc/
--r--r--r--   0        0        0   107745 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/objects/dc/4e4aeeb1400f75fa40bfd4d2503a029c03c52c
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/ed/
--r--r--r--   0        0        0     4088 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/ed/bf62e5089214fd1852188ed807854a0f6693c0
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090305 pytun-pmd3-2.0.4/.git/objects/f4/
--r--r--r--   0        0        0       53 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/f4/2f5d6747f39938e3b2cf67d0dce66b54b1dc73
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/.git/objects/fd/
--r--r--r--   0        0        0     3290 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/fd/f4f4d078cf8140de00025b32a172080017d76d
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.043113 pytun-pmd3-2.0.4/.git/refs/
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/.git/refs/tags/
--rw-rw-rw-   0        0        0       41 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/refs/tags/v2.0.4
--rw-rw-rw-   0        0        0       41 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/shallow
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.058734 pytun-pmd3-2.0.4/.github/
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/.github/workflows/
--rw-rw-rw-   0        0        0     1438 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.github/workflows/python-publish-macos-and-linux.yml
--rw-rw-rw-   0        0        0     1130 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.github/workflows/python-publish-windows.yml
--rw-rw-rw-   0        0        0      142 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.gitignore
--rw-rw-rw-   0        0        0     1074 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/LICENSE
--rw-rw-rw-   0        0        0       44 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2444 2024-04-11 06:06:51.100358 pytun-pmd3-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      130 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/README.md
--rw-rw-rw-   0        0        0      331 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/common.h
--rw-rw-rw-   0        0        0    15301 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/darwin_pytun.c
--rw-rw-rw-   0        0        0    23999 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/linux_pytun.c
--rw-rw-rw-   0        0        0     1529 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/pytun_pmd3/
--rw-rw-rw-   0        0        0      141 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/__init__.py
--rw-rw-rw-   0        0        0      427 2024-04-11 06:06:50.000000 pytun-pmd3-2.0.4/pytun_pmd3/_version.py
--rw-rw-rw-   0        0        0       47 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/pytun_pmd3/wintun/
--rw-rw-rw-   0        0        0     5431 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/LICENSE.txt
--rw-rw-rw-   0        0        0    13916 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.058734 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/amd64/
--rw-rw-rw-   0        0        0   427552 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/amd64/wintun.dll
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/arm/
--rw-rw-rw-   0        0        0   364552 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/arm/wintun.dll
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/arm64/
--rw-rw-rw-   0        0        0   222488 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/arm64/wintun.dll
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/x86/
--rw-rw-rw-   0        0        0   550928 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/x86/wintun.dll
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.100358 pytun-pmd3-2.0.4/pytun_pmd3/wintun/include/
--rw-rw-rw-   0        0        0    10362 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/include/wintun.h
--rw-rw-rw-   0        0        0    10666 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.100358 pytun-pmd3-2.0.4/pytun_pmd3.egg-info/
--rw-rw-rw-   0        0        0     2444 2024-04-11 06:06:50.000000 pytun-pmd3-2.0.4/pytun_pmd3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3101 2024-04-11 06:06:51.000000 pytun-pmd3-2.0.4/pytun_pmd3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 06:06:50.000000 pytun-pmd3-2.0.4/pytun_pmd3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-11 06:06:50.000000 pytun-pmd3-2.0.4/pytun_pmd3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-11 06:06:50.000000 pytun-pmd3-2.0.4/pytun_pmd3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 06:06:51.100358 pytun-pmd3-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0      532 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.668900 pytun-pmd3-2.0.5/
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.622021 pytun-pmd3-2.0.5/.git/
+-rw-rw-rw-   0        0        0      127 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/.git/FETCH_HEAD
+-rw-rw-rw-   0        0        0       41 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/.git/HEAD
+-rw-rw-rw-   0        0        0      378 2024-04-11 06:44:52.000000 pytun-pmd3-2.0.5/.git/config
+-rw-rw-rw-   0        0        0       73 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/description
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/hooks/
+-rw-rw-rw-   0        0        0      478 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/applypatch-msg.sample
+-rw-rw-rw-   0        0        0      896 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/commit-msg.sample
+-rw-rw-rw-   0        0        0     4726 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/fsmonitor-watchman.sample
+-rw-rw-rw-   0        0        0      189 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/post-update.sample
+-rw-rw-rw-   0        0        0      424 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/pre-applypatch.sample
+-rw-rw-rw-   0        0        0     1649 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/pre-commit.sample
+-rw-rw-rw-   0        0        0      416 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/pre-merge-commit.sample
+-rw-rw-rw-   0        0        0     1374 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/pre-push.sample
+-rw-rw-rw-   0        0        0     4898 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/pre-rebase.sample
+-rw-rw-rw-   0        0        0      544 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/pre-receive.sample
+-rw-rw-rw-   0        0        0     1492 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/prepare-commit-msg.sample
+-rw-rw-rw-   0        0        0     2783 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/push-to-checkout.sample
+-rw-rw-rw-   0        0        0     2308 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/sendemail-validate.sample
+-rw-rw-rw-   0        0        0     3650 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/hooks/update.sample
+-rw-rw-rw-   0        0        0     2271 2024-04-11 06:45:33.000000 pytun-pmd3-2.0.5/.git/index
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/info/
+-rw-rw-rw-   0        0        0      240 2024-04-11 06:44:50.000000 pytun-pmd3-2.0.5/.git/info/exclude
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/logs/
+-rw-rw-rw-   0        0        0      190 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/.git/logs/HEAD
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.622021 pytun-pmd3-2.0.5/.git/objects/
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/00/
+-r--r--r--   0        0        0   185785 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/.git/objects/00/17794f4638f1a1b4e469619a9824accac6ccea
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/05/
+-r--r--r--   0        0        0      644 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/0b/
+-r--r--r--   0        0        0      207 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/0b/87183182ca91979436d9e9965719d62cda4b12
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/16/
+-r--r--r--   0        0        0     4796 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/16/e6a680fefc2fc02952634fce616297c1725157
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/24/
+-r--r--r--   0        0        0      151 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/24/37ac7587f2ed14ef7db00fc068613ee4adab69
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/2a/
+-r--r--r--   0        0        0   279805 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/2a/b97dba062208bcb6ffc32bef8347d586751038
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/34/
+-r--r--r--   0        0        0       51 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/34/0815e53a01e17a3d4682f7d020696fb3a587da
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/48/
+-r--r--r--   0        0        0      113 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/48/2f0e082621cd6d9d699c4cdfa55ba322166de4
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/4d/
+-r--r--r--   0        0        0       55 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/4d/76d949a3568d0ff1d0f73fe6858f1dfe6af0a6
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/51/
+-r--r--r--   0        0        0      597 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/51/caff11e470f0cfa91e2d07b67ccf52a285824e
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/52/
+-r--r--r--   0        0        0       55 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/52/06f67ae5433525c632716e1e595eb02e6856ef
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/55/
+-r--r--r--   0        0        0     3227 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/.git/objects/55/d441f4a8017b2ea30eae55137c52f2829dba5f
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/56/
+-r--r--r--   0        0        0       53 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/56/d9c426af16617a614e2e17ba6e01afe9b2c9c0
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/5f/
+-r--r--r--   0        0        0      128 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/5f/8e3b9fcde01a609d1b1e37c79ecf6b8a50d1e3
+-r--r--r--   0        0        0      688 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/5f/b524da018127adcf64a2ffa97bf9be86e9ecb2
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/6f/
+-r--r--r--   0        0        0      687 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/6f/8a30c5db31dd360fff4542eef776f4ff397144
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.637644 pytun-pmd3-2.0.5/.git/objects/71/
+-r--r--r--   0        0        0       55 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/71/beb6065e5d841f0bb2b7a1d0be99436fe906d4
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/77/
+-r--r--r--   0        0        0     3318 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/77/bb9e7e1e55c7963281ea6c2a1551cbe4295097
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/7f/
+-r--r--r--   0        0        0      126 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/7f/f8524670c0aed9f1a4439279b78a5e7c137f6f
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/81/
+-r--r--r--   0        0        0       55 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/81/7d73b0ac42a4dfc956fd81fd9e130a4ab61aaa
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/89/
+-r--r--r--   0        0        0     5346 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/89/ee237a05bde1829e0487347488ad23244ebfea
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/96/
+-r--r--r--   0        0        0     4102 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/96/f5528f89b16112491f01e7cc19ffa7dfbc87d9
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/ae/
+-r--r--r--   0        0        0   209806 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/.git/objects/ae/e04e77bfbd6601adbcd5a46435f059e31cf6e4
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/af/
+-r--r--r--   0        0        0       51 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/af/348689d62b32e0021ab0d82c0f8fc156db4728
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/b5/
+-r--r--r--   0        0        0      128 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/b5/77e4de768ad66f0d36c258491c30b8f89d64a0
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/bc/
+-r--r--r--   0        0        0     2554 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/bc/8d3f0e60565567a8b8598972614dce7d4ffccd
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/c0/
+-r--r--r--   0        0        0      107 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/c0/26fe934c3c8d26d252e3541da2d4fe539a7503
+-r--r--r--   0        0        0      289 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/.git/objects/c0/93c88fd653a207aea042daeabd98f6666ed72a
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/c3/
+-r--r--r--   0        0        0      883 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/c3/a5ea2cdd89353e5c70e2d92f940130d02129a6
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/c5/
+-r--r--r--   0        0        0      150 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/c5/8a3c8a6e3b698ea353d97545c477154a0d3e0b
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/dc/
+-r--r--r--   0        0        0   107745 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/.git/objects/dc/4e4aeeb1400f75fa40bfd4d2503a029c03c52c
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/objects/f4/
+-r--r--r--   0        0        0      388 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/f4/2452538d24c75e06b31f6f3ee59e619b6eef00
+-r--r--r--   0        0        0       53 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/objects/f4/2f5d6747f39938e3b2cf67d0dce66b54b1dc73
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.622021 pytun-pmd3-2.0.5/.git/refs/
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.git/refs/tags/
+-rw-rw-rw-   0        0        0       41 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/.git/refs/tags/v2.0.5
+-rw-rw-rw-   0        0        0       41 2024-04-11 06:44:53.000000 pytun-pmd3-2.0.5/.git/shallow
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.622021 pytun-pmd3-2.0.5/.github/
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/.github/workflows/
+-rw-rw-rw-   0        0        0     1438 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/.github/workflows/python-publish-macos-and-linux.yml
+-rw-rw-rw-   0        0        0     1130 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/.github/workflows/python-publish-windows.yml
+-rw-rw-rw-   0        0        0      142 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/.gitignore
+-rw-rw-rw-   0        0        0     1074 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0       44 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2444 2024-04-11 06:45:34.668900 pytun-pmd3-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      130 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/README.md
+-rw-rw-rw-   0        0        0      331 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/common.h
+-rw-rw-rw-   0        0        0    15375 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/darwin_pytun.c
+-rw-rw-rw-   0        0        0    23999 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/linux_pytun.c
+-rw-rw-rw-   0        0        0     1529 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/pytun_pmd3/
+-rw-rw-rw-   0        0        0      141 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/pytun_pmd3/__init__.py
+-rw-rw-rw-   0        0        0      427 2024-04-11 06:45:34.000000 pytun-pmd3-2.0.5/pytun_pmd3/_version.py
+-rw-rw-rw-   0        0        0       47 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/pytun_pmd3/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/pytun_pmd3/wintun/
+-rw-rw-rw-   0        0        0     5431 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/pytun_pmd3/wintun/LICENSE.txt
+-rw-rw-rw-   0        0        0    13916 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/pytun_pmd3/wintun/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.622021 pytun-pmd3-2.0.5/pytun_pmd3/wintun/bin/
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/pytun_pmd3/wintun/bin/amd64/
+-rw-rw-rw-   0        0        0   427552 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/pytun_pmd3/wintun/bin/amd64/wintun.dll
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.653275 pytun-pmd3-2.0.5/pytun_pmd3/wintun/bin/arm/
+-rw-rw-rw-   0        0        0   364552 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/pytun_pmd3/wintun/bin/arm/wintun.dll
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.668900 pytun-pmd3-2.0.5/pytun_pmd3/wintun/bin/arm64/
+-rw-rw-rw-   0        0        0   222488 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/pytun_pmd3/wintun/bin/arm64/wintun.dll
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.668900 pytun-pmd3-2.0.5/pytun_pmd3/wintun/bin/x86/
+-rw-rw-rw-   0        0        0   550928 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/pytun_pmd3/wintun/bin/x86/wintun.dll
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.668900 pytun-pmd3-2.0.5/pytun_pmd3/wintun/include/
+-rw-rw-rw-   0        0        0    10362 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/pytun_pmd3/wintun/include/wintun.h
+-rw-rw-rw-   0        0        0    10798 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/pytun_pmd3/wintun.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:45:34.668900 pytun-pmd3-2.0.5/pytun_pmd3.egg-info/
+-rw-rw-rw-   0        0        0     2444 2024-04-11 06:45:34.000000 pytun-pmd3-2.0.5/pytun_pmd3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3101 2024-04-11 06:45:34.000000 pytun-pmd3-2.0.5/pytun_pmd3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 06:45:34.000000 pytun-pmd3-2.0.5/pytun_pmd3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-11 06:45:34.000000 pytun-pmd3-2.0.5/pytun_pmd3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-11 06:45:34.000000 pytun-pmd3-2.0.5/pytun_pmd3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 06:45:34.668900 pytun-pmd3-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      532 2024-04-11 06:44:54.000000 pytun-pmd3-2.0.5/setup.py
```

### Comparing `pytun-pmd3-2.0.4/.git/hooks/commit-msg.sample` & `pytun-pmd3-2.0.5/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/hooks/fsmonitor-watchman.sample` & `pytun-pmd3-2.0.5/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/hooks/pre-commit.sample` & `pytun-pmd3-2.0.5/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/hooks/pre-push.sample` & `pytun-pmd3-2.0.5/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/hooks/pre-rebase.sample` & `pytun-pmd3-2.0.5/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/hooks/pre-receive.sample` & `pytun-pmd3-2.0.5/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/hooks/prepare-commit-msg.sample` & `pytun-pmd3-2.0.5/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/hooks/push-to-checkout.sample` & `pytun-pmd3-2.0.5/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/hooks/sendemail-validate.sample` & `pytun-pmd3-2.0.5/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/hooks/update.sample` & `pytun-pmd3-2.0.5/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/objects/00/17794f4638f1a1b4e469619a9824accac6ccea` & `pytun-pmd3-2.0.5/.git/objects/00/17794f4638f1a1b4e469619a9824accac6ccea`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82` & `pytun-pmd3-2.0.5/.git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/objects/16/e6a680fefc2fc02952634fce616297c1725157` & `pytun-pmd3-2.0.5/.git/objects/16/e6a680fefc2fc02952634fce616297c1725157`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/objects/2a/b97dba062208bcb6ffc32bef8347d586751038` & `pytun-pmd3-2.0.5/.git/objects/2a/b97dba062208bcb6ffc32bef8347d586751038`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/objects/51/caff11e470f0cfa91e2d07b67ccf52a285824e` & `pytun-pmd3-2.0.5/.git/objects/51/caff11e470f0cfa91e2d07b67ccf52a285824e`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/objects/55/d441f4a8017b2ea30eae55137c52f2829dba5f` & `pytun-pmd3-2.0.5/.git/objects/55/d441f4a8017b2ea30eae55137c52f2829dba5f`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/objects/5f/b524da018127adcf64a2ffa97bf9be86e9ecb2` & `pytun-pmd3-2.0.5/.git/objects/5f/b524da018127adcf64a2ffa97bf9be86e9ecb2`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/objects/6f/8a30c5db31dd360fff4542eef776f4ff397144` & `pytun-pmd3-2.0.5/.git/objects/6f/8a30c5db31dd360fff4542eef776f4ff397144`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/objects/89/ee237a05bde1829e0487347488ad23244ebfea` & `pytun-pmd3-2.0.5/.git/objects/89/ee237a05bde1829e0487347488ad23244ebfea`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/objects/ae/e04e77bfbd6601adbcd5a46435f059e31cf6e4` & `pytun-pmd3-2.0.5/.git/objects/ae/e04e77bfbd6601adbcd5a46435f059e31cf6e4`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/objects/bc/8d3f0e60565567a8b8598972614dce7d4ffccd` & `pytun-pmd3-2.0.5/.git/objects/bc/8d3f0e60565567a8b8598972614dce7d4ffccd`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.git/objects/dc/4e4aeeb1400f75fa40bfd4d2503a029c03c52c` & `pytun-pmd3-2.0.5/.git/objects/dc/4e4aeeb1400f75fa40bfd4d2503a029c03c52c`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.github/workflows/python-publish-macos-and-linux.yml` & `pytun-pmd3-2.0.5/.github/workflows/python-publish-macos-and-linux.yml`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/.github/workflows/python-publish-windows.yml` & `pytun-pmd3-2.0.5/.github/workflows/python-publish-windows.yml`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/LICENSE` & `pytun-pmd3-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/PKG-INFO` & `pytun-pmd3-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytun-pmd3
-Version: 2.0.4
+Version: 2.0.5
 Summary: python-pytun fork with darwin and windows support (IPv6-ONLY)
 Author-email: doronz88 <doron88@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>
 License: Copyright (c) 2011, montag451.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pytun-pmd3-2.0.4/darwin_pytun.c` & `pytun-pmd3-2.0.5/darwin_pytun.c`

 * *Files 2% similar despite different names*

```diff
@@ -282,19 +282,21 @@
 static PyObject *pytun_tuntap_down(PyObject *self) {
     pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
     struct ifreq req;
 
     memset(&req, 0, sizeof(req));
     strcpy(req.ifr_name, tuntap->name);
     if (ioctl(tuntap->fd, SIOCGIFFLAGS, &req) < 0) {
+        raise_error_from_errno();
         return NULL;
     }
     if (req.ifr_flags & IFF_UP) {
         req.ifr_flags &= ~IFF_UP;
         if (ioctl(tuntap->fd, SIOCSIFFLAGS, &req) < 0) {
+            raise_error_from_errno();
             return NULL;
         }
     }
 
     Py_RETURN_NONE;
 }
```

### Comparing `pytun-pmd3-2.0.4/linux_pytun.c` & `pytun-pmd3-2.0.5/linux_pytun.c`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/pyproject.toml` & `pytun-pmd3-2.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/pytun_pmd3/wintun/LICENSE.txt` & `pytun-pmd3-2.0.5/pytun_pmd3/wintun/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/pytun_pmd3/wintun/README.md` & `pytun-pmd3-2.0.5/pytun_pmd3/wintun/README.md`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/amd64/wintun.dll` & `pytun-pmd3-2.0.5/pytun_pmd3/wintun/bin/amd64/wintun.dll`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/arm/wintun.dll` & `pytun-pmd3-2.0.5/pytun_pmd3/wintun/bin/arm/wintun.dll`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/arm64/wintun.dll` & `pytun-pmd3-2.0.5/pytun_pmd3/wintun/bin/arm64/wintun.dll`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/x86/wintun.dll` & `pytun-pmd3-2.0.5/pytun_pmd3/wintun/bin/x86/wintun.dll`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/pytun_pmd3/wintun/include/wintun.h` & `pytun-pmd3-2.0.5/pytun_pmd3/wintun/include/wintun.h`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.4/pytun_pmd3/wintun.py` & `pytun-pmd3-2.0.5/pytun_pmd3/wintun.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,15 +243,18 @@
         self.ip_interface_entry = row
 
     @property
     def interface_index(self) -> int:
         return self.ip_interface_entry.InterfaceIndex
 
     def close(self) -> None:
-        wintun.WintunCloseAdapter(self.handle)
+        self.down()
+        if self.handle is not None:
+            wintun.WintunCloseAdapter(self.handle)
+        self.handle = None
 
     @property
     def addr(self) -> str:
         return ''
 
     @addr.setter
     def addr(self, value: str) -> None:
@@ -266,15 +269,16 @@
     def name(self) -> str:
         return self._name
 
     def up(self, capacity: int = DEFAULT_RING_CAPCITY) -> None:
         self.session = wintun.WintunStartSession(self.handle, capacity)
 
     def down(self) -> None:
-        wintun.WintunEndSession(self.session)
+        if self.session is not None:
+            wintun.WintunEndSession(self.session)
         self.session = None
 
     def read(self) -> bytes:
         size = DWORD()
         packet_ptr = wintun.WintunReceivePacket(self.session, byref(size))
         if not packet_ptr:
             # No packet was received
```

### Comparing `pytun-pmd3-2.0.4/pytun_pmd3.egg-info/PKG-INFO` & `pytun-pmd3-2.0.5/pytun_pmd3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytun-pmd3
-Version: 2.0.4
+Version: 2.0.5
 Summary: python-pytun fork with darwin and windows support (IPv6-ONLY)
 Author-email: doronz88 <doron88@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>
 License: Copyright (c) 2011, montag451.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pytun-pmd3-2.0.4/pytun_pmd3.egg-info/SOURCES.txt` & `pytun-pmd3-2.0.5/pytun_pmd3.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,44 +29,44 @@
 .git/hooks/update.sample
 .git/info/exclude
 .git/logs/HEAD
 .git/objects/00/17794f4638f1a1b4e469619a9824accac6ccea
 .git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82
 .git/objects/0b/87183182ca91979436d9e9965719d62cda4b12
 .git/objects/16/e6a680fefc2fc02952634fce616297c1725157
+.git/objects/24/37ac7587f2ed14ef7db00fc068613ee4adab69
 .git/objects/2a/b97dba062208bcb6ffc32bef8347d586751038
 .git/objects/34/0815e53a01e17a3d4682f7d020696fb3a587da
 .git/objects/48/2f0e082621cd6d9d699c4cdfa55ba322166de4
 .git/objects/4d/76d949a3568d0ff1d0f73fe6858f1dfe6af0a6
 .git/objects/51/caff11e470f0cfa91e2d07b67ccf52a285824e
 .git/objects/52/06f67ae5433525c632716e1e595eb02e6856ef
 .git/objects/55/d441f4a8017b2ea30eae55137c52f2829dba5f
 .git/objects/56/d9c426af16617a614e2e17ba6e01afe9b2c9c0
 .git/objects/5f/8e3b9fcde01a609d1b1e37c79ecf6b8a50d1e3
 .git/objects/5f/b524da018127adcf64a2ffa97bf9be86e9ecb2
 .git/objects/6f/8a30c5db31dd360fff4542eef776f4ff397144
 .git/objects/71/beb6065e5d841f0bb2b7a1d0be99436fe906d4
-.git/objects/77/b5124b5ab694ecdedd659e0ce18d872174afc3
+.git/objects/77/bb9e7e1e55c7963281ea6c2a1551cbe4295097
 .git/objects/7f/f8524670c0aed9f1a4439279b78a5e7c137f6f
 .git/objects/81/7d73b0ac42a4dfc956fd81fd9e130a4ab61aaa
-.git/objects/83/36f281235488a0f2cca5aeca510a71efc4a7da
 .git/objects/89/ee237a05bde1829e0487347488ad23244ebfea
+.git/objects/96/f5528f89b16112491f01e7cc19ffa7dfbc87d9
 .git/objects/ae/e04e77bfbd6601adbcd5a46435f059e31cf6e4
 .git/objects/af/348689d62b32e0021ab0d82c0f8fc156db4728
 .git/objects/b5/77e4de768ad66f0d36c258491c30b8f89d64a0
 .git/objects/bc/8d3f0e60565567a8b8598972614dce7d4ffccd
 .git/objects/c0/26fe934c3c8d26d252e3541da2d4fe539a7503
 .git/objects/c0/93c88fd653a207aea042daeabd98f6666ed72a
+.git/objects/c3/a5ea2cdd89353e5c70e2d92f940130d02129a6
 .git/objects/c5/8a3c8a6e3b698ea353d97545c477154a0d3e0b
-.git/objects/d7/600902847a6ed081b86ebb3ac97ce1c242c4df
 .git/objects/dc/4e4aeeb1400f75fa40bfd4d2503a029c03c52c
-.git/objects/ed/bf62e5089214fd1852188ed807854a0f6693c0
+.git/objects/f4/2452538d24c75e06b31f6f3ee59e619b6eef00
 .git/objects/f4/2f5d6747f39938e3b2cf67d0dce66b54b1dc73
-.git/objects/fd/f4f4d078cf8140de00025b32a172080017d76d
-.git/refs/tags/v2.0.4
+.git/refs/tags/v2.0.5
 .github/workflows/python-publish-macos-and-linux.yml
 .github/workflows/python-publish-windows.yml
 pytun_pmd3/__init__.py
 pytun_pmd3/_version.py
 pytun_pmd3/exceptions.py
 pytun_pmd3/wintun.py
 pytun_pmd3.egg-info/PKG-INFO
```

### Comparing `pytun-pmd3-2.0.4/setup.py` & `pytun-pmd3-2.0.5/setup.py`

 * *Files identical despite different names*

