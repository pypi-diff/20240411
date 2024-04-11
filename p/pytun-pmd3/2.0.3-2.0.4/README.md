# Comparing `tmp/pytun-pmd3-2.0.3.tar.gz` & `tmp/pytun-pmd3-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytun-pmd3-2.0.3.tar", last modified: Wed Apr 10 18:58:16 2024, max compression
+gzip compressed data, was "pytun-pmd3-2.0.4.tar", last modified: Thu Apr 11 06:06:51 2024, max compression
```

## Comparing `pytun-pmd3-2.0.3.tar` & `pytun-pmd3-2.0.4.tar`

### file list

```diff
@@ -1,144 +1,135 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.749223 pytun-pmd3-2.0.3/.git/
--rw-rw-rw-   0        0        0      127 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/FETCH_HEAD
--rw-rw-rw-   0        0        0       41 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/HEAD
--rw-rw-rw-   0        0        0      378 2024-04-10 18:57:29.000000 pytun-pmd3-2.0.3/.git/config
--rw-rw-rw-   0        0        0       73 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/description
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/hooks/
--rw-rw-rw-   0        0        0      478 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/applypatch-msg.sample
--rw-rw-rw-   0        0        0      896 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/commit-msg.sample
--rw-rw-rw-   0        0        0     4726 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/fsmonitor-watchman.sample
--rw-rw-rw-   0        0        0      189 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/post-update.sample
--rw-rw-rw-   0        0        0      424 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/pre-applypatch.sample
--rw-rw-rw-   0        0        0     1649 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/pre-commit.sample
--rw-rw-rw-   0        0        0      416 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/pre-merge-commit.sample
--rw-rw-rw-   0        0        0     1374 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/pre-push.sample
--rw-rw-rw-   0        0        0     4898 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/pre-rebase.sample
--rw-rw-rw-   0        0        0      544 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/pre-receive.sample
--rw-rw-rw-   0        0        0     1492 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/prepare-commit-msg.sample
--rw-rw-rw-   0        0        0     2783 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/push-to-checkout.sample
--rw-rw-rw-   0        0        0     2308 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/sendemail-validate.sample
--rw-rw-rw-   0        0        0     3650 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/hooks/update.sample
--rw-rw-rw-   0        0        0     2460 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/index
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/info/
--rw-rw-rw-   0        0        0      240 2024-04-10 18:57:25.000000 pytun-pmd3-2.0.3/.git/info/exclude
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/logs/
--rw-rw-rw-   0        0        0      190 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/logs/HEAD
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.749223 pytun-pmd3-2.0.3/.git/objects/
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/00/
--r--r--r--   0        0        0   185785 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/00/17794f4638f1a1b4e469619a9824accac6ccea
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/05/
--r--r--r--   0        0        0      644 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/0b/
--r--r--r--   0        0        0      207 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/0b/87183182ca91979436d9e9965719d62cda4b12
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/16/
--r--r--r--   0        0        0     4796 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/16/e6a680fefc2fc02952634fce616297c1725157
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/2a/
--r--r--r--   0        0        0   279805 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/2a/b97dba062208bcb6ffc32bef8347d586751038
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/30/
--r--r--r--   0        0        0      107 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/30/b9ae6f25de9828b7a1473270fe3154cbbb67f8
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/34/
--r--r--r--   0        0        0       51 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/34/0815e53a01e17a3d4682f7d020696fb3a587da
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/3f/
--r--r--r--   0        0        0      416 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/3f/6f4a46b79728f3726b519a2a6a9ff5cd80947a
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/48/
--r--r--r--   0        0        0      113 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/48/2f0e082621cd6d9d699c4cdfa55ba322166de4
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/4d/
--r--r--r--   0        0        0       55 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/4d/76d949a3568d0ff1d0f73fe6858f1dfe6af0a6
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/51/
--r--r--r--   0        0        0      597 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/51/caff11e470f0cfa91e2d07b67ccf52a285824e
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/52/
--r--r--r--   0        0        0       55 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/52/06f67ae5433525c632716e1e595eb02e6856ef
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/55/
--r--r--r--   0        0        0     3227 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/55/d441f4a8017b2ea30eae55137c52f2829dba5f
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/56/
--r--r--r--   0        0        0       53 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/56/d9c426af16617a614e2e17ba6e01afe9b2c9c0
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/5f/
--r--r--r--   0        0        0      688 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/5f/b524da018127adcf64a2ffa97bf9be86e9ecb2
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/71/
--r--r--r--   0        0        0       55 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/71/beb6065e5d841f0bb2b7a1d0be99436fe906d4
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/7f/
--r--r--r--   0        0        0      126 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/7f/f8524670c0aed9f1a4439279b78a5e7c137f6f
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/81/
--r--r--r--   0        0        0       55 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/81/7d73b0ac42a4dfc956fd81fd9e130a4ab61aaa
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/89/
--r--r--r--   0        0        0     5346 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/89/ee237a05bde1829e0487347488ad23244ebfea
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/8d/
--r--r--r--   0        0        0     1024 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/8d/e62c37cc8fcf845ecd68838240936924cf9906
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/9d/
--r--r--r--   0        0        0      151 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/9d/c66440808b749982929c6dd762241cf8018032
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/a6/
--r--r--r--   0        0        0      627 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/a6/1e7914203018dfa21514b06f0646981d71d067
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/a9/
--r--r--r--   0        0        0     1058 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/a9/de0cc5100692d182a38a2e85ee739bdd771c7a
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/ae/
--r--r--r--   0        0        0   209806 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/ae/e04e77bfbd6601adbcd5a46435f059e31cf6e4
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/af/
--r--r--r--   0        0        0       51 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/af/348689d62b32e0021ab0d82c0f8fc156db4728
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/b4/
--r--r--r--   0        0        0       83 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/b4/9ac67e351cffd016971fe56eb32564da10b8da
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.764854 pytun-pmd3-2.0.3/.git/objects/b5/
--r--r--r--   0        0        0      128 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/b5/77e4de768ad66f0d36c258491c30b8f89d64a0
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/.git/objects/bc/
--r--r--r--   0        0        0     2554 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/bc/8d3f0e60565567a8b8598972614dce7d4ffccd
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/.git/objects/c0/
--r--r--r--   0        0        0      107 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/c0/26fe934c3c8d26d252e3541da2d4fe539a7503
--r--r--r--   0        0        0      289 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/c0/93c88fd653a207aea042daeabd98f6666ed72a
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/.git/objects/c5/
--r--r--r--   0        0        0      150 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/c5/8a3c8a6e3b698ea353d97545c477154a0d3e0b
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/.git/objects/d4/
--r--r--r--   0        0        0     3292 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/d4/cb4438b5bf15e244a6c5873db243ab511cac0b
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/.git/objects/dc/
--r--r--r--   0        0        0   107745 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/dc/4e4aeeb1400f75fa40bfd4d2503a029c03c52c
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/.git/objects/e4/
--r--r--r--   0        0        0      174 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/e4/a5cdad357c9b4d558acba154c6279163cbfa98
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/.git/objects/ed/
--r--r--r--   0        0        0     4088 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/ed/bf62e5089214fd1852188ed807854a0f6693c0
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/.git/objects/f4/
--r--r--r--   0        0        0       53 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/objects/f4/2f5d6747f39938e3b2cf67d0dce66b54b1dc73
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.749223 pytun-pmd3-2.0.3/.git/refs/
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/.git/refs/tags/
--rw-rw-rw-   0        0        0       41 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/refs/tags/v2.0.3
--rw-rw-rw-   0        0        0       41 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.git/shallow
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.749223 pytun-pmd3-2.0.3/.github/
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/.github/workflows/
--rw-rw-rw-   0        0        0     1438 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.github/workflows/python-publish-macos-and-linux.yml
--rw-rw-rw-   0        0        0     1130 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.github/workflows/python-publish-windows.yml
--rw-rw-rw-   0        0        0      118 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/.gitignore
--rw-rw-rw-   0        0        0     1074 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/LICENSE
--rw-rw-rw-   0        0        0       44 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2444 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      130 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/README.md
--rw-rw-rw-   0        0        0      331 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/common.h
--rw-rw-rw-   0        0        0    15301 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/darwin_pytun.c
--rw-rw-rw-   0        0        0    23999 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/linux_pytun.c
--rw-rw-rw-   0        0        0     1355 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/pytun_pmd3/
--rw-rw-rw-   0        0        0      141 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/pytun_pmd3/__init__.py
--rw-rw-rw-   0        0        0       47 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/pytun_pmd3/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/pytun_pmd3/wintun/
--rw-rw-rw-   0        0        0     5431 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/pytun_pmd3/wintun/LICENSE.txt
--rw-rw-rw-   0        0        0    13916 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/pytun_pmd3/wintun/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.749223 pytun-pmd3-2.0.3/pytun_pmd3/wintun/bin/
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/pytun_pmd3/wintun/bin/amd64/
--rw-rw-rw-   0        0        0   427552 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/pytun_pmd3/wintun/bin/amd64/wintun.dll
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/pytun_pmd3/wintun/bin/arm/
--rw-rw-rw-   0        0        0   364552 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/pytun_pmd3/wintun/bin/arm/wintun.dll
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/pytun_pmd3/wintun/bin/arm64/
--rw-rw-rw-   0        0        0   222488 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/pytun_pmd3/wintun/bin/arm64/wintun.dll
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/pytun_pmd3/wintun/bin/x86/
--rw-rw-rw-   0        0        0   550928 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/pytun_pmd3/wintun/bin/x86/wintun.dll
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/pytun_pmd3/wintun/include/
--rw-rw-rw-   0        0        0    10362 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/pytun_pmd3/wintun/include/wintun.h
--rw-rw-rw-   0        0        0    10682 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/pytun_pmd3/wintun.py
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/pytun_pmd3.egg-info/
--rw-rw-rw-   0        0        0     2444 2024-04-10 18:58:16.000000 pytun-pmd3-2.0.3/pytun_pmd3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3277 2024-04-10 18:58:16.000000 pytun-pmd3-2.0.3/pytun_pmd3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 18:58:16.000000 pytun-pmd3-2.0.3/pytun_pmd3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 18:58:16.000000 pytun-pmd3-2.0.3/pytun_pmd3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-10 18:58:16.000000 pytun-pmd3-2.0.3/pytun_pmd3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      532 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 18:58:16.780480 pytun-pmd3-2.0.3/test/
--rw-rw-rw-   0        0        0     3160 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/test/test_tap.py
--rw-rw-rw-   0        0        0     3348 2024-04-10 18:57:31.000000 pytun-pmd3-2.0.3/test/test_tun.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.100358 pytun-pmd3-2.0.4/
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.058734 pytun-pmd3-2.0.4/.git/
+-rw-rw-rw-   0        0        0      127 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/FETCH_HEAD
+-rw-rw-rw-   0        0        0       41 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/HEAD
+-rw-rw-rw-   0        0        0      378 2024-04-11 06:06:01.000000 pytun-pmd3-2.0.4/.git/config
+-rw-rw-rw-   0        0        0       73 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/description
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.058734 pytun-pmd3-2.0.4/.git/hooks/
+-rw-rw-rw-   0        0        0      478 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/applypatch-msg.sample
+-rw-rw-rw-   0        0        0      896 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/commit-msg.sample
+-rw-rw-rw-   0        0        0     4726 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/fsmonitor-watchman.sample
+-rw-rw-rw-   0        0        0      189 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/post-update.sample
+-rw-rw-rw-   0        0        0      424 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/pre-applypatch.sample
+-rw-rw-rw-   0        0        0     1649 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/pre-commit.sample
+-rw-rw-rw-   0        0        0      416 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/pre-merge-commit.sample
+-rw-rw-rw-   0        0        0     1374 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/pre-push.sample
+-rw-rw-rw-   0        0        0     4898 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/pre-rebase.sample
+-rw-rw-rw-   0        0        0      544 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/pre-receive.sample
+-rw-rw-rw-   0        0        0     1492 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/prepare-commit-msg.sample
+-rw-rw-rw-   0        0        0     2783 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/push-to-checkout.sample
+-rw-rw-rw-   0        0        0     2308 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/sendemail-validate.sample
+-rw-rw-rw-   0        0        0     3650 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/hooks/update.sample
+-rw-rw-rw-   0        0        0     2271 2024-04-11 06:06:49.000000 pytun-pmd3-2.0.4/.git/index
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/info/
+-rw-rw-rw-   0        0        0      240 2024-04-11 06:05:57.000000 pytun-pmd3-2.0.4/.git/info/exclude
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/logs/
+-rw-rw-rw-   0        0        0      191 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/logs/HEAD
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.043113 pytun-pmd3-2.0.4/.git/objects/
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/00/
+-r--r--r--   0        0        0   185785 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/objects/00/17794f4638f1a1b4e469619a9824accac6ccea
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/05/
+-r--r--r--   0        0        0      644 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/0b/
+-r--r--r--   0        0        0      207 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/0b/87183182ca91979436d9e9965719d62cda4b12
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/16/
+-r--r--r--   0        0        0     4796 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/16/e6a680fefc2fc02952634fce616297c1725157
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/2a/
+-r--r--r--   0        0        0   279805 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/2a/b97dba062208bcb6ffc32bef8347d586751038
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/34/
+-r--r--r--   0        0        0       51 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/34/0815e53a01e17a3d4682f7d020696fb3a587da
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/48/
+-r--r--r--   0        0        0      113 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/48/2f0e082621cd6d9d699c4cdfa55ba322166de4
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/4d/
+-r--r--r--   0        0        0       55 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/4d/76d949a3568d0ff1d0f73fe6858f1dfe6af0a6
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/51/
+-r--r--r--   0        0        0      597 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/51/caff11e470f0cfa91e2d07b67ccf52a285824e
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/52/
+-r--r--r--   0        0        0       55 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/52/06f67ae5433525c632716e1e595eb02e6856ef
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/55/
+-r--r--r--   0        0        0     3227 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/objects/55/d441f4a8017b2ea30eae55137c52f2829dba5f
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/56/
+-r--r--r--   0        0        0       53 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/56/d9c426af16617a614e2e17ba6e01afe9b2c9c0
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/5f/
+-r--r--r--   0        0        0      128 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/5f/8e3b9fcde01a609d1b1e37c79ecf6b8a50d1e3
+-r--r--r--   0        0        0      688 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/5f/b524da018127adcf64a2ffa97bf9be86e9ecb2
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/6f/
+-r--r--r--   0        0        0      687 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/6f/8a30c5db31dd360fff4542eef776f4ff397144
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/71/
+-r--r--r--   0        0        0       55 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/71/beb6065e5d841f0bb2b7a1d0be99436fe906d4
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/77/
+-r--r--r--   0        0        0      898 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/77/b5124b5ab694ecdedd659e0ce18d872174afc3
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/7f/
+-r--r--r--   0        0        0      126 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/7f/f8524670c0aed9f1a4439279b78a5e7c137f6f
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/81/
+-r--r--r--   0        0        0       55 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/81/7d73b0ac42a4dfc956fd81fd9e130a4ab61aaa
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/83/
+-r--r--r--   0        0        0      387 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/83/36f281235488a0f2cca5aeca510a71efc4a7da
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/89/
+-r--r--r--   0        0        0     5346 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/89/ee237a05bde1829e0487347488ad23244ebfea
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/ae/
+-r--r--r--   0        0        0   209806 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/objects/ae/e04e77bfbd6601adbcd5a46435f059e31cf6e4
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/af/
+-r--r--r--   0        0        0       51 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/af/348689d62b32e0021ab0d82c0f8fc156db4728
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/b5/
+-r--r--r--   0        0        0      128 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/b5/77e4de768ad66f0d36c258491c30b8f89d64a0
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/bc/
+-r--r--r--   0        0        0     2554 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/bc/8d3f0e60565567a8b8598972614dce7d4ffccd
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/c0/
+-r--r--r--   0        0        0      107 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/c0/26fe934c3c8d26d252e3541da2d4fe539a7503
+-r--r--r--   0        0        0      289 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/objects/c0/93c88fd653a207aea042daeabd98f6666ed72a
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/c5/
+-r--r--r--   0        0        0      150 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/c5/8a3c8a6e3b698ea353d97545c477154a0d3e0b
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/d7/
+-r--r--r--   0        0        0      151 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/d7/600902847a6ed081b86ebb3ac97ce1c242c4df
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/dc/
+-r--r--r--   0        0        0   107745 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/objects/dc/4e4aeeb1400f75fa40bfd4d2503a029c03c52c
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.074359 pytun-pmd3-2.0.4/.git/objects/ed/
+-r--r--r--   0        0        0     4088 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/ed/bf62e5089214fd1852188ed807854a0f6693c0
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090305 pytun-pmd3-2.0.4/.git/objects/f4/
+-r--r--r--   0        0        0       53 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/f4/2f5d6747f39938e3b2cf67d0dce66b54b1dc73
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/.git/objects/fd/
+-r--r--r--   0        0        0     3290 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/objects/fd/f4f4d078cf8140de00025b32a172080017d76d
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.043113 pytun-pmd3-2.0.4/.git/refs/
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/.git/refs/tags/
+-rw-rw-rw-   0        0        0       41 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.git/refs/tags/v2.0.4
+-rw-rw-rw-   0        0        0       41 2024-04-11 06:06:03.000000 pytun-pmd3-2.0.4/.git/shallow
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.058734 pytun-pmd3-2.0.4/.github/
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/.github/workflows/
+-rw-rw-rw-   0        0        0     1438 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.github/workflows/python-publish-macos-and-linux.yml
+-rw-rw-rw-   0        0        0     1130 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.github/workflows/python-publish-windows.yml
+-rw-rw-rw-   0        0        0      142 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/.gitignore
+-rw-rw-rw-   0        0        0     1074 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0       44 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2444 2024-04-11 06:06:51.100358 pytun-pmd3-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      130 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/README.md
+-rw-rw-rw-   0        0        0      331 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/common.h
+-rw-rw-rw-   0        0        0    15301 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/darwin_pytun.c
+-rw-rw-rw-   0        0        0    23999 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/linux_pytun.c
+-rw-rw-rw-   0        0        0     1529 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/pytun_pmd3/
+-rw-rw-rw-   0        0        0      141 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/__init__.py
+-rw-rw-rw-   0        0        0      427 2024-04-11 06:06:50.000000 pytun-pmd3-2.0.4/pytun_pmd3/_version.py
+-rw-rw-rw-   0        0        0       47 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/pytun_pmd3/wintun/
+-rw-rw-rw-   0        0        0     5431 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/LICENSE.txt
+-rw-rw-rw-   0        0        0    13916 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.058734 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/amd64/
+-rw-rw-rw-   0        0        0   427552 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/amd64/wintun.dll
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/arm/
+-rw-rw-rw-   0        0        0   364552 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/arm/wintun.dll
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/arm64/
+-rw-rw-rw-   0        0        0   222488 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/arm64/wintun.dll
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.090841 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/x86/
+-rw-rw-rw-   0        0        0   550928 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/x86/wintun.dll
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.100358 pytun-pmd3-2.0.4/pytun_pmd3/wintun/include/
+-rw-rw-rw-   0        0        0    10362 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun/include/wintun.h
+-rw-rw-rw-   0        0        0    10666 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/pytun_pmd3/wintun.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:06:51.100358 pytun-pmd3-2.0.4/pytun_pmd3.egg-info/
+-rw-rw-rw-   0        0        0     2444 2024-04-11 06:06:50.000000 pytun-pmd3-2.0.4/pytun_pmd3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3101 2024-04-11 06:06:51.000000 pytun-pmd3-2.0.4/pytun_pmd3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 06:06:50.000000 pytun-pmd3-2.0.4/pytun_pmd3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-11 06:06:50.000000 pytun-pmd3-2.0.4/pytun_pmd3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-11 06:06:50.000000 pytun-pmd3-2.0.4/pytun_pmd3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 06:06:51.100358 pytun-pmd3-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      532 2024-04-11 06:06:04.000000 pytun-pmd3-2.0.4/setup.py
```

### Comparing `pytun-pmd3-2.0.3/.git/hooks/commit-msg.sample` & `pytun-pmd3-2.0.4/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/hooks/fsmonitor-watchman.sample` & `pytun-pmd3-2.0.4/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/hooks/pre-commit.sample` & `pytun-pmd3-2.0.4/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/hooks/pre-push.sample` & `pytun-pmd3-2.0.4/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/hooks/pre-rebase.sample` & `pytun-pmd3-2.0.4/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/hooks/pre-receive.sample` & `pytun-pmd3-2.0.4/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/hooks/prepare-commit-msg.sample` & `pytun-pmd3-2.0.4/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/hooks/push-to-checkout.sample` & `pytun-pmd3-2.0.4/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/hooks/sendemail-validate.sample` & `pytun-pmd3-2.0.4/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/hooks/update.sample` & `pytun-pmd3-2.0.4/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/objects/00/17794f4638f1a1b4e469619a9824accac6ccea` & `pytun-pmd3-2.0.4/.git/objects/00/17794f4638f1a1b4e469619a9824accac6ccea`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82` & `pytun-pmd3-2.0.4/.git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/objects/16/e6a680fefc2fc02952634fce616297c1725157` & `pytun-pmd3-2.0.4/.git/objects/16/e6a680fefc2fc02952634fce616297c1725157`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/objects/2a/b97dba062208bcb6ffc32bef8347d586751038` & `pytun-pmd3-2.0.4/.git/objects/2a/b97dba062208bcb6ffc32bef8347d586751038`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/objects/51/caff11e470f0cfa91e2d07b67ccf52a285824e` & `pytun-pmd3-2.0.4/.git/objects/51/caff11e470f0cfa91e2d07b67ccf52a285824e`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/objects/55/d441f4a8017b2ea30eae55137c52f2829dba5f` & `pytun-pmd3-2.0.4/.git/objects/55/d441f4a8017b2ea30eae55137c52f2829dba5f`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/objects/5f/b524da018127adcf64a2ffa97bf9be86e9ecb2` & `pytun-pmd3-2.0.4/.git/objects/5f/b524da018127adcf64a2ffa97bf9be86e9ecb2`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/objects/89/ee237a05bde1829e0487347488ad23244ebfea` & `pytun-pmd3-2.0.4/.git/objects/89/ee237a05bde1829e0487347488ad23244ebfea`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/objects/ae/e04e77bfbd6601adbcd5a46435f059e31cf6e4` & `pytun-pmd3-2.0.4/.git/objects/ae/e04e77bfbd6601adbcd5a46435f059e31cf6e4`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/objects/bc/8d3f0e60565567a8b8598972614dce7d4ffccd` & `pytun-pmd3-2.0.4/.git/objects/bc/8d3f0e60565567a8b8598972614dce7d4ffccd`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/objects/dc/4e4aeeb1400f75fa40bfd4d2503a029c03c52c` & `pytun-pmd3-2.0.4/.git/objects/dc/4e4aeeb1400f75fa40bfd4d2503a029c03c52c`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.git/objects/ed/bf62e5089214fd1852188ed807854a0f6693c0` & `pytun-pmd3-2.0.4/.git/objects/ed/bf62e5089214fd1852188ed807854a0f6693c0`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.github/workflows/python-publish-macos-and-linux.yml` & `pytun-pmd3-2.0.4/.github/workflows/python-publish-macos-and-linux.yml`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/.github/workflows/python-publish-windows.yml` & `pytun-pmd3-2.0.4/.github/workflows/python-publish-windows.yml`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/LICENSE` & `pytun-pmd3-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/PKG-INFO` & `pytun-pmd3-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytun-pmd3
-Version: 2.0.3
+Version: 2.0.4
 Summary: python-pytun fork with darwin and windows support (IPv6-ONLY)
 Author-email: doronz88 <doron88@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>
 License: Copyright (c) 2011, montag451.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pytun-pmd3-2.0.3/darwin_pytun.c` & `pytun-pmd3-2.0.4/darwin_pytun.c`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/linux_pytun.c` & `pytun-pmd3-2.0.4/linux_pytun.c`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/pyproject.toml` & `pytun-pmd3-2.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [project]
 name = "pytun-pmd3"
-version = "2.0.3"
 description = "python-pytun fork with darwin and windows support (IPv6-ONLY)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["tun", "tuntap", "darwin", "pymobiledevice3", "macos", "windows"]
 authors = [
     { name = "doronz88", email = "doron88@gmail.com" }
@@ -19,24 +18,31 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
 ]
+dynamic = ["version"]
 
 [project.optional-dependencies]
 test = ["pytest"]
 
 [project.urls]
 "Homepage" = "https://github.com/doronz88/pytun-pmd3"
 "Bug Reports" = "https://github.com/doronz88/pytun-pmd3/issues"
 
 [tool.setuptools]
 package-data = { "pytun_pmd3" = ["wintun/**/*"] }
 
 [tool.setuptools.packages.find]
 exclude = ["docs*", "tests*"]
 
+[tool.setuptools.dynamic]
+version = {attr = "pytun_pmd3._version.__version__"}
+
+[tool.setuptools_scm]
+version_file = "pytun_pmd3/_version.py"
+
 [build-system]
-requires = ["setuptools>=43.0.0", "wheel"]
+requires = ["setuptools>=43.0.0", "setuptools_scm>=8", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `pytun-pmd3-2.0.3/pytun_pmd3/wintun/LICENSE.txt` & `pytun-pmd3-2.0.4/pytun_pmd3/wintun/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/pytun_pmd3/wintun/README.md` & `pytun-pmd3-2.0.4/pytun_pmd3/wintun/README.md`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/pytun_pmd3/wintun/bin/amd64/wintun.dll` & `pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/amd64/wintun.dll`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/pytun_pmd3/wintun/bin/arm/wintun.dll` & `pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/arm/wintun.dll`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/pytun_pmd3/wintun/bin/arm64/wintun.dll` & `pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/arm64/wintun.dll`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/pytun_pmd3/wintun/bin/x86/wintun.dll` & `pytun-pmd3-2.0.4/pytun_pmd3/wintun/bin/x86/wintun.dll`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/pytun_pmd3/wintun/include/wintun.h` & `pytun-pmd3-2.0.4/pytun_pmd3/wintun/include/wintun.h`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-2.0.3/pytun_pmd3/wintun.py` & `pytun-pmd3-2.0.4/pytun_pmd3/wintun.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ctypes
 import platform
 import subprocess
 from ctypes import POINTER, Structure, WinDLL, byref, c_ubyte, c_ulonglong, c_void_p, create_unicode_buffer, \
     get_last_error, string_at
-from ctypes.wintypes import BOOL, BOOLEAN, BYTE, DWORD, HANDLE, LARGE_INTEGER, LPCWSTR, ULARGE_INTEGER, ULONG, USHORT
+from ctypes.wintypes import BOOL, BOOLEAN, BYTE, DWORD, HANDLE, LARGE_INTEGER, LPCWSTR, ULONG, USHORT
 from pathlib import Path
 from socket import AF_INET6
 from uuid import uuid4
 
 from pytun_pmd3.exceptions import PyWinTunException
 
 DEFAULT_ADAPTER_NAME = 'pywintun'
```

### Comparing `pytun-pmd3-2.0.3/pytun_pmd3.egg-info/PKG-INFO` & `pytun-pmd3-2.0.4/pytun_pmd3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytun-pmd3
-Version: 2.0.3
+Version: 2.0.4
 Summary: python-pytun fork with darwin and windows support (IPv6-ONLY)
 Author-email: doronz88 <doron88@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>
 License: Copyright (c) 2011, montag451.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pytun-pmd3-2.0.3/pytun_pmd3.egg-info/SOURCES.txt` & `pytun-pmd3-2.0.4/pytun_pmd3.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -30,58 +30,54 @@
 .git/info/exclude
 .git/logs/HEAD
 .git/objects/00/17794f4638f1a1b4e469619a9824accac6ccea
 .git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82
 .git/objects/0b/87183182ca91979436d9e9965719d62cda4b12
 .git/objects/16/e6a680fefc2fc02952634fce616297c1725157
 .git/objects/2a/b97dba062208bcb6ffc32bef8347d586751038
-.git/objects/30/b9ae6f25de9828b7a1473270fe3154cbbb67f8
 .git/objects/34/0815e53a01e17a3d4682f7d020696fb3a587da
-.git/objects/3f/6f4a46b79728f3726b519a2a6a9ff5cd80947a
 .git/objects/48/2f0e082621cd6d9d699c4cdfa55ba322166de4
 .git/objects/4d/76d949a3568d0ff1d0f73fe6858f1dfe6af0a6
 .git/objects/51/caff11e470f0cfa91e2d07b67ccf52a285824e
 .git/objects/52/06f67ae5433525c632716e1e595eb02e6856ef
 .git/objects/55/d441f4a8017b2ea30eae55137c52f2829dba5f
 .git/objects/56/d9c426af16617a614e2e17ba6e01afe9b2c9c0
+.git/objects/5f/8e3b9fcde01a609d1b1e37c79ecf6b8a50d1e3
 .git/objects/5f/b524da018127adcf64a2ffa97bf9be86e9ecb2
+.git/objects/6f/8a30c5db31dd360fff4542eef776f4ff397144
 .git/objects/71/beb6065e5d841f0bb2b7a1d0be99436fe906d4
+.git/objects/77/b5124b5ab694ecdedd659e0ce18d872174afc3
 .git/objects/7f/f8524670c0aed9f1a4439279b78a5e7c137f6f
 .git/objects/81/7d73b0ac42a4dfc956fd81fd9e130a4ab61aaa
+.git/objects/83/36f281235488a0f2cca5aeca510a71efc4a7da
 .git/objects/89/ee237a05bde1829e0487347488ad23244ebfea
-.git/objects/8d/e62c37cc8fcf845ecd68838240936924cf9906
-.git/objects/9d/c66440808b749982929c6dd762241cf8018032
-.git/objects/a6/1e7914203018dfa21514b06f0646981d71d067
-.git/objects/a9/de0cc5100692d182a38a2e85ee739bdd771c7a
 .git/objects/ae/e04e77bfbd6601adbcd5a46435f059e31cf6e4
 .git/objects/af/348689d62b32e0021ab0d82c0f8fc156db4728
-.git/objects/b4/9ac67e351cffd016971fe56eb32564da10b8da
 .git/objects/b5/77e4de768ad66f0d36c258491c30b8f89d64a0
 .git/objects/bc/8d3f0e60565567a8b8598972614dce7d4ffccd
 .git/objects/c0/26fe934c3c8d26d252e3541da2d4fe539a7503
 .git/objects/c0/93c88fd653a207aea042daeabd98f6666ed72a
 .git/objects/c5/8a3c8a6e3b698ea353d97545c477154a0d3e0b
-.git/objects/d4/cb4438b5bf15e244a6c5873db243ab511cac0b
+.git/objects/d7/600902847a6ed081b86ebb3ac97ce1c242c4df
 .git/objects/dc/4e4aeeb1400f75fa40bfd4d2503a029c03c52c
-.git/objects/e4/a5cdad357c9b4d558acba154c6279163cbfa98
 .git/objects/ed/bf62e5089214fd1852188ed807854a0f6693c0
 .git/objects/f4/2f5d6747f39938e3b2cf67d0dce66b54b1dc73
-.git/refs/tags/v2.0.3
+.git/objects/fd/f4f4d078cf8140de00025b32a172080017d76d
+.git/refs/tags/v2.0.4
 .github/workflows/python-publish-macos-and-linux.yml
 .github/workflows/python-publish-windows.yml
 pytun_pmd3/__init__.py
+pytun_pmd3/_version.py
 pytun_pmd3/exceptions.py
 pytun_pmd3/wintun.py
 pytun_pmd3.egg-info/PKG-INFO
 pytun_pmd3.egg-info/SOURCES.txt
 pytun_pmd3.egg-info/dependency_links.txt
 pytun_pmd3.egg-info/requires.txt
 pytun_pmd3.egg-info/top_level.txt
 pytun_pmd3/wintun/LICENSE.txt
 pytun_pmd3/wintun/README.md
 pytun_pmd3/wintun/bin/amd64/wintun.dll
 pytun_pmd3/wintun/bin/arm/wintun.dll
 pytun_pmd3/wintun/bin/arm64/wintun.dll
 pytun_pmd3/wintun/bin/x86/wintun.dll
-pytun_pmd3/wintun/include/wintun.h
-test/test_tap.py
-test/test_tun.py
+pytun_pmd3/wintun/include/wintun.h
```

### Comparing `pytun-pmd3-2.0.3/setup.py` & `pytun-pmd3-2.0.4/setup.py`

 * *Files identical despite different names*

