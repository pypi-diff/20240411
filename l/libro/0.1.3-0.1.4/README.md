# Comparing `tmp/libro-0.1.3.tar.gz` & `tmp/libro-0.1.4.tar.gz`

## Comparing `libro-0.1.3.tar` & `libro-0.1.4.tar`

### file list

```diff
@@ -1,534 +1,602 @@
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 libro-0.1.3/.npmrc
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libro-0.1.3/.python-version
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 libro-0.1.3/package.json
--rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/.package-lock.json
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/.bin/installServerIntoExtension -> ../vscode-languageserver/bin/installServerIntoExtension
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/.bin/libro-analyzer -> ../@difizen/libro-analyzer/index.js
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@difizen/libro-analyzer/LICENSE.txt
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@difizen/libro-analyzer/README.md
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@difizen/libro-analyzer/index.js
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@difizen/libro-analyzer/package.json
--rwxr-xr-x   0        0        0    10640 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/CHANGELOG.md
--rwxr-xr-x   0        0        0      752 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/LICENSE
--rwxr-xr-x   0        0        0    18226 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/README.md
--rwxr-xr-x   0        0        0     1650 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/index.d.ts
--rwxr-xr-x   0        0        0     2710 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/package.json
--rwxr-xr-x   0        0        0      863 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/parse-async.js
--rwxr-xr-x   0        0        0     1045 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/parse-pretty-error.js
--rwxr-xr-x   0        0        0     1625 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/parse-stream.js
--rwxr-xr-x   0        0        0      415 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/parse-string.js
--rwxr-xr-x   0        0        0      227 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/parse.js
--rwxr-xr-x   0        0        0     8292 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/stringify.js
--rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/toml.js
--rwxr-xr-x   0        0        0      485 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/create-date.js
--rwxr-xr-x   0        0        0      663 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/create-datetime-float.js
--rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/create-datetime.js
--rwxr-xr-x   0        0        0      508 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/create-time.js
--rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/format-num.js
--rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/parser-debug.js
--rwxr-xr-x   0        0        0     2975 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/parser.js
--rwxr-xr-x   0        0        0    45566 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/toml-parser.js
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@types/emscripten/LICENSE
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@types/emscripten/README.md
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@types/emscripten/index.d.ts
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@types/emscripten/package.json
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/package.json
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/AliasFS.d.ts
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/AliasFS.js
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/CwdFS.d.ts
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/CwdFS.js
--rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/FakeFS.d.ts
--rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/FakeFS.js
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/JailFS.d.ts
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/JailFS.js
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/LazyFS.d.ts
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/LazyFS.js
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NoFS.d.ts
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NoFS.js
--rw-r--r--   0        0        0     8845 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NodeFS.d.ts
--rw-r--r--   0        0        0    17379 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NodeFS.js
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NodePathFS.d.ts
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NodePathFS.js
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/PosixFS.d.ts
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/PosixFS.js
--rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ProxiedFS.d.ts
--rw-r--r--   0        0        0     9579 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ProxiedFS.js
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/VirtualFS.d.ts
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/VirtualFS.js
--rw-r--r--   0        0        0    11486 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ZipFS.d.ts
--rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ZipFS.js
--rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ZipOpenFS.d.ts
--rw-r--r--   0        0        0    36407 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ZipOpenFS.js
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/constants.d.ts
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/constants.js
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/errors.d.ts
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/errors.js
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/index.d.ts
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/index.js
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/path.d.ts
--rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/path.js
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/statUtils.d.ts
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/statUtils.js
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/xfs.d.ts
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/xfs.js
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/copyPromise.d.ts
--rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/copyPromise.js
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/opendir.d.ts
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/opendir.js
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile.d.ts
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile.js
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile/CustomStatWatcher.d.ts
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile/CustomStatWatcher.js
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/patchFs/FileHandle.d.ts
--rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/patchFs/FileHandle.js
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/patchFs/patchFs.d.ts
--rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/patchFs/patchFs.js
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/README.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/package.json
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/async.d.ts
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/async.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/emscripten.d.ts
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/libzipAsync.d.ts
--rw-r--r--   0        0        0   372811 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/libzipAsync.js
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/libzipSync.d.ts
--rw-r--r--   0        0        0   364127 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/libzipSync.js
--rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/makeInterface.d.ts
--rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/makeInterface.js
--rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/sync.d.ts
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/sync.js
--rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/ansi-styles/index.d.ts
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/ansi-styles/index.js
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/ansi-styles/license
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/ansi-styles/readme.md
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/anymatch/LICENSE
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/anymatch/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/anymatch/index.d.ts
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/anymatch/index.js
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/anymatch/package.json
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/array-back/LICENSE
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/array-back/README.hbs
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/array-back/README.md
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/array-back/index.mjs
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/array-back/package.json
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/binary-extensions.json
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/binary-extensions.json.d.ts
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/index.d.ts
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/index.js
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/license
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/package.json
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/readme.md
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/CHANGELOG.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/LICENSE
--rw-r--r--   0        0        0    21130 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/README.md
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/index.js
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/package.json
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/lib/compile.js
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/lib/constants.js
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/lib/expand.js
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/lib/parse.js
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/lib/stringify.js
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/lib/utils.js
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/buffer-from/LICENSE
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/buffer-from/index.js
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/buffer-from/package.json
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/buffer-from/readme.md
--rw-r--r--   0        0        0     8899 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/index.d.ts
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/license
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/package.json
--rw-r--r--   0        0        0    13365 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/readme.md
--rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/source/index.js
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/source/templates.js
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/source/util.js
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/LICENSE
--rw-r--r--   0        0        0    14392 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/README.md
--rw-r--r--   0        0        0    28379 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/index.js
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/package.json
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/lib/constants.js
--rw-r--r--   0        0        0    16368 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/lib/fsevents-handler.js
--rw-r--r--   0        0        0    20067 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/lib/nodefs-handler.js
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/types/index.d.ts
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/CHANGELOG.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/LICENSE
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/README.md
--rw-r--r--   0        0        0    17040 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/conversions.js
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/index.js
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/package.json
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/route.js
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-name/LICENSE
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-name/README.md
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-name/index.js
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-name/package.json
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/LICENSE
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/README.md
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/index.mjs
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/package.json
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/argv-parser.mjs
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/argv-tools.mjs
--rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/option-definition.mjs
--rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/option-definitions.mjs
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/option-flag.mjs
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/option.mjs
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/output-grouped.mjs
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/output.mjs
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fill-range/LICENSE
--rw-r--r--   0        0        0     7486 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fill-range/README.md
--rw-r--r--   0        0        0     6315 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fill-range/index.js
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fill-range/package.json
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/find-replace/LICENSE
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/find-replace/README.hbs
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/find-replace/README.md
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/find-replace/index.mjs
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/find-replace/package.json
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fsevents/LICENSE
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fsevents/README.md
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fsevents/fsevents.d.ts
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fsevents/fsevents.js
--rwxr-xr-x   0        0        0   163626 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fsevents/fsevents.node
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fsevents/package.json
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/glob-parent/CHANGELOG.md
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/glob-parent/LICENSE
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/glob-parent/README.md
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/glob-parent/index.js
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/glob-parent/package.json
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/has-flag/index.d.ts
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/has-flag/index.js
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/has-flag/license
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/has-flag/package.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/has-flag/readme.md
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-binary-path/index.d.ts
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-binary-path/index.js
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-binary-path/license
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-binary-path/package.json
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-binary-path/readme.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-extglob/LICENSE
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-extglob/README.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-extglob/index.js
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-extglob/package.json
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-glob/LICENSE
--rw-r--r--   0        0        0     7145 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-glob/README.md
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-glob/index.js
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-glob/package.json
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-number/LICENSE
--rw-r--r--   0        0        0     6514 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-number/README.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-number/index.js
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-number/package.json
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/CHANGELOG.md
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/LICENSE.md
--rw-r--r--   0        0        0    14129 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/README.md
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/SECURITY.md
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/package.json
--rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/main.d.ts
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/main.js
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/edit.js
--rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/format.js
--rw-r--r--   0        0        0    24708 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/parser.js
--rw-r--r--   0        0        0    19188 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/scanner.js
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/string-intern.js
--rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/main.d.ts
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/main.js
--rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/edit.js
--rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/format.js
--rw-r--r--   0        0        0    28290 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/parser.js
--rw-r--r--   0        0        0    21446 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/scanner.js
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/string-intern.js
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/leven/index.d.ts
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/leven/index.js
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/leven/license
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/leven/package.json
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/leven/readme.md
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/lodash.camelcase/LICENSE
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/lodash.camelcase/README.md
--rw-r--r--   0        0        0    18757 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/lodash.camelcase/index.js
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/lodash.camelcase/package.json
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/normalize-path/LICENSE
--rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/normalize-path/README.md
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/normalize-path/index.js
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/normalize-path/package.json
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/CHANGELOG.md
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/LICENSE
--rw-r--r--   0        0        0    27445 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/README.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/index.js
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/package.json
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/lib/constants.js
--rw-r--r--   0        0        0    27763 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/lib/parse.js
--rw-r--r--   0        0        0     9956 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/lib/picomatch.js
--rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/lib/scan.js
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/lib/utils.js
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/readdirp/LICENSE
--rw-r--r--   0        0        0     6942 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/readdirp/README.md
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/readdirp/index.d.ts
--rw-r--r--   0        0        0     8876 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/readdirp/index.js
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/readdirp/package.json
--rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/CHANGELOG.md
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/LICENSE
--rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/README.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/package.json
--rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/source-map.d.ts
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/source-map.js
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/array-set.js
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/base64-vlq.js
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/base64.js
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/binary-search.js
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/mapping-list.js
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/quick-sort.js
--rw-r--r--   0        0        0    40562 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/source-map-consumer.js
--rw-r--r--   0        0        0    14356 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/source-map-generator.js
--rw-r--r--   0        0        0    13808 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/source-node.js
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/util.js
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/LICENSE.md
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/README.md
--rw-r--r--   0        0        0    53583 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/browser-source-map-support.js
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/package.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/register-hook-require.js
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/register.js
--rw-r--r--   0        0        0    20223 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/source-map-support.js
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/supports-color/browser.js
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/supports-color/index.js
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/supports-color/license
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/supports-color/package.json
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/supports-color/readme.md
--rw-r--r--   0        0        0    16509 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tmp/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tmp/LICENSE
--rw-r--r--   0        0        0    12531 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tmp/README.md
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tmp/package.json
--rw-r--r--   0        0        0    22676 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tmp/lib/tmp.js
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/to-regex-range/LICENSE
--rw-r--r--   0        0        0    13585 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/to-regex-range/README.md
--rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/to-regex-range/index.js
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/to-regex-range/package.json
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/CopyrightNotice.txt
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/LICENSE.txt
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/README.md
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/package.json
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/tslib.d.ts
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/tslib.es6.html
--rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/tslib.es6.js
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/tslib.html
--rw-r--r--   0        0        0    13204 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/tslib.js
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/modules/index.js
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/typical/LICENSE
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/typical/README.hbs
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/typical/README.md
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/typical/index.mjs
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/typical/package.json
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/License.txt
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/README.md
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/browser.d.ts
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/browser.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/node.cmd
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/node.d.ts
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/node.js
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/package.json
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/thirdpartynotices.txt
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/browser/main.d.ts
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/browser/main.js
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/browser/ril.d.ts
--rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/browser/ril.js
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/api.d.ts
--rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/api.js
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/cancellation.d.ts
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/cancellation.js
--rw-r--r--   0        0        0    17906 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/connection.d.ts
--rw-r--r--   0        0        0    51184 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/connection.js
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/disposable.d.ts
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/disposable.js
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/encoding.d.ts
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/encoding.js
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/events.d.ts
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/events.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/is.d.ts
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/is.js
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/linkedMap.d.ts
--rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/linkedMap.js
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageBuffer.d.ts
--rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageBuffer.js
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageReader.d.ts
--rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageReader.js
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageWriter.d.ts
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageWriter.js
--rw-r--r--   0        0        0    12626 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messages.d.ts
--rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messages.js
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/ral.d.ts
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/ral.js
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/semaphore.d.ts
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/semaphore.js
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/sharedArrayCancellation.d.ts
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/sharedArrayCancellation.js
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/node/main.d.ts
--rw-r--r--   0        0        0     9778 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/node/main.js
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/node/ril.d.ts
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/node/ril.js
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/typings/thenable.d.ts
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/License.txt
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/README.md
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/browser.d.ts
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/browser.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/node.cmd
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/node.d.ts
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/node.js
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/package.json
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/thirdpartynotices.txt
--rwxr-xr-x   0        0        0     2754 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/bin/installServerIntoExtension
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/browser/main.d.ts
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/browser/main.js
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/api.d.ts
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/api.js
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/callHierarchy.d.ts
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/callHierarchy.js
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/configuration.d.ts
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/configuration.js
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/diagnostic.d.ts
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/diagnostic.js
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/fileOperations.d.ts
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/fileOperations.js
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/inlayHint.d.ts
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/inlayHint.js
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/inlineValue.d.ts
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/inlineValue.js
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/linkedEditingRange.d.ts
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/linkedEditingRange.js
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/moniker.d.ts
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/moniker.js
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/notebook.d.ts
--rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/notebook.js
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/progress.d.ts
--rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/progress.js
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/semanticTokens.d.ts
--rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/semanticTokens.js
--rw-r--r--   0        0        0    37013 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/server.d.ts
--rw-r--r--   0        0        0    34971 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/server.js
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/showDocument.d.ts
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/showDocument.js
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/textDocuments.d.ts
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/textDocuments.js
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/typeHierarchy.d.ts
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/typeHierarchy.js
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/workspaceFolder.d.ts
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/workspaceFolder.js
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/utils/is.d.ts
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/utils/is.js
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/utils/uuid.d.ts
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/utils/uuid.js
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/node/files.d.ts
--rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/node/files.js
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/node/main.d.ts
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/node/main.js
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/node/resolve.d.ts
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/node/resolve.js
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/typings/thenable.d.ts
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/License.txt
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/README.md
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/browser.d.ts
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/browser.js
--rw-r--r--   0        0        0    21796 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/metaModel.schema.json
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/node.cmd
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/node.d.ts
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/node.js
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/package.json
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/thirdpartynotices.txt
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/browser/main.d.ts
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/browser/main.js
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/api.d.ts
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/api.js
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/connection.d.ts
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/connection.js
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/messages.d.ts
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/messages.js
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.$.d.ts
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.$.js
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.callHierarchy.d.ts
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.callHierarchy.js
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.colorProvider.d.ts
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.colorProvider.js
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.configuration.d.ts
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.configuration.js
--rw-r--r--   0        0        0   112267 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.d.ts
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.declaration.d.ts
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.declaration.js
--rw-r--r--   0        0        0    10782 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.diagnostic.d.ts
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.diagnostic.js
--rw-r--r--   0        0        0     9616 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.fileOperations.d.ts
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.fileOperations.js
--rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.foldingRange.d.ts
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.foldingRange.js
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.implementation.d.ts
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.implementation.js
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlayHint.d.ts
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlayHint.js
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlineValue.d.ts
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlineValue.js
--rw-r--r--   0        0        0    55332 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.js
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.linkedEditingRange.d.ts
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.linkedEditingRange.js
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.moniker.d.ts
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.moniker.js
--rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.notebook.d.ts
--rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.notebook.js
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.progress.d.ts
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.progress.js
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.selectionRange.d.ts
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.selectionRange.js
--rw-r--r--   0        0        0     7994 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.semanticTokens.d.ts
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.semanticTokens.js
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.showDocument.d.ts
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.showDocument.js
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeDefinition.d.ts
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeDefinition.js
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeHierarchy.d.ts
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeHierarchy.js
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.workspaceFolder.d.ts
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.workspaceFolder.js
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/utils/is.d.ts
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/utils/is.js
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/node/main.d.ts
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/node/main.js
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/License.txt
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/README.md
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/package.json
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/thirdpartynotices.txt
--rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/lib/esm/main.d.ts
--rw-r--r--   0        0        0    11258 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/lib/esm/main.js
--rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/lib/umd/main.d.ts
--rw-r--r--   0        0        0    12811 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/lib/umd/main.js
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/License.txt
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/README.md
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/package.json
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/thirdpartynotices.txt
--rw-r--r--   0        0        0    97126 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/lib/esm/main.d.ts
--rw-r--r--   0        0        0    78825 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/lib/esm/main.js
--rw-r--r--   0        0        0    97126 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/lib/umd/main.d.ts
--rw-r--r--   0        0        0    92006 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/lib/umd/main.js
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/LICENSE.md
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/README.md
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/SECURITY.md
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/package.json
--rw-r--r--   0        0        0    10742 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/esm/index.mjs
--rw-r--r--   0        0        0    62941 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/esm/index.mjs.map
--rw-r--r--   0        0        0    11020 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/charCode.d.ts
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/charCode.js
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/index.d.ts
--rw-r--r--   0        0        0    11853 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/index.js
--rw-r--r--   0        0        0    62976 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/index.js.map
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/platform.d.ts
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/platform.js
--rw-r--r--   0        0        0     5843 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/uri.d.ts
--rw-r--r--   0        0        0    21939 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/uri.js
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/utils.d.ts
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/utils.js
--rw-r--r--   0        0        0    68855 2020-02-02 00:00:00.000000 libro-0.1.3/src/dev-config/jupyter_server_config.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/_version.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/app.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/handler.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/templates/error.html
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/templates/libro.html
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/templates/page.html
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 libro-0.1.3/.gitignore
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 libro-0.1.3/README.md
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 libro-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 libro-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 libro-0.1.4/.npmrc
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libro-0.1.4/.python-version
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 libro-0.1.4/package.json
+-rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/.package-lock.json
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/.bin/installServerIntoExtension -> ../vscode-languageserver/bin/installServerIntoExtension
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/.bin/libro-analyzer -> ../@difizen/libro-analyzer/index.js
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@difizen/libro-analyzer/LICENSE.txt
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@difizen/libro-analyzer/README.md
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@difizen/libro-analyzer/index.js
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@difizen/libro-analyzer/package.json
+-rwxr-xr-x   0        0        0    10640 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/CHANGELOG.md
+-rwxr-xr-x   0        0        0      752 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/LICENSE
+-rwxr-xr-x   0        0        0    18226 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/README.md
+-rwxr-xr-x   0        0        0     1650 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/index.d.ts
+-rwxr-xr-x   0        0        0     2710 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/package.json
+-rwxr-xr-x   0        0        0      863 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/parse-async.js
+-rwxr-xr-x   0        0        0     1045 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/parse-pretty-error.js
+-rwxr-xr-x   0        0        0     1625 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/parse-stream.js
+-rwxr-xr-x   0        0        0      415 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/parse-string.js
+-rwxr-xr-x   0        0        0      227 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/parse.js
+-rwxr-xr-x   0        0        0     8292 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/stringify.js
+-rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/toml.js
+-rwxr-xr-x   0        0        0      485 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/lib/create-date.js
+-rwxr-xr-x   0        0        0      663 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/lib/create-datetime-float.js
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/lib/create-datetime.js
+-rwxr-xr-x   0        0        0      508 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/lib/create-time.js
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/lib/format-num.js
+-rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/lib/parser-debug.js
+-rwxr-xr-x   0        0        0     2975 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/lib/parser.js
+-rwxr-xr-x   0        0        0    45566 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@iarna/toml/lib/toml-parser.js
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@types/emscripten/LICENSE
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@types/emscripten/README.md
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@types/emscripten/index.d.ts
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@types/emscripten/package.json
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/package.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/AliasFS.d.ts
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/AliasFS.js
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/CwdFS.d.ts
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/CwdFS.js
+-rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/FakeFS.d.ts
+-rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/FakeFS.js
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/JailFS.d.ts
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/JailFS.js
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/LazyFS.d.ts
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/LazyFS.js
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/NoFS.d.ts
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/NoFS.js
+-rw-r--r--   0        0        0     8845 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/NodeFS.d.ts
+-rw-r--r--   0        0        0    17379 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/NodeFS.js
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/NodePathFS.d.ts
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/NodePathFS.js
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/PosixFS.d.ts
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/PosixFS.js
+-rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/ProxiedFS.d.ts
+-rw-r--r--   0        0        0     9579 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/ProxiedFS.js
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/VirtualFS.d.ts
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/VirtualFS.js
+-rw-r--r--   0        0        0    11486 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/ZipFS.d.ts
+-rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/ZipFS.js
+-rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/ZipOpenFS.d.ts
+-rw-r--r--   0        0        0    36407 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/ZipOpenFS.js
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/constants.d.ts
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/constants.js
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/errors.d.ts
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/errors.js
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/index.d.ts
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/index.js
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/path.d.ts
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/path.js
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/statUtils.d.ts
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/statUtils.js
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/xfs.d.ts
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/xfs.js
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/copyPromise.d.ts
+-rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/copyPromise.js
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/opendir.d.ts
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/opendir.js
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile.d.ts
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile.js
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile/CustomStatWatcher.d.ts
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile/CustomStatWatcher.js
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/patchFs/FileHandle.d.ts
+-rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/patchFs/FileHandle.js
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/patchFs/patchFs.d.ts
+-rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/fslib/lib/patchFs/patchFs.js
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/libzip/README.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/libzip/package.json
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/libzip/lib/async.d.ts
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/libzip/lib/async.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/libzip/lib/emscripten.d.ts
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/libzip/lib/libzipAsync.d.ts
+-rw-r--r--   0        0        0   372811 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/libzip/lib/libzipAsync.js
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/libzip/lib/libzipSync.d.ts
+-rw-r--r--   0        0        0   364127 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/libzip/lib/libzipSync.js
+-rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/libzip/lib/makeInterface.d.ts
+-rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/libzip/lib/makeInterface.js
+-rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/libzip/lib/sync.d.ts
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/@yarnpkg/libzip/lib/sync.js
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/ansi-styles/index.d.ts
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/ansi-styles/index.js
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/ansi-styles/license
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/ansi-styles/readme.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/anymatch/LICENSE
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/anymatch/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/anymatch/index.d.ts
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/anymatch/index.js
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/anymatch/package.json
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/array-back/LICENSE
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/array-back/README.hbs
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/array-back/README.md
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/array-back/index.mjs
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/array-back/package.json
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/binary-extensions/binary-extensions.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/binary-extensions/binary-extensions.json.d.ts
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/binary-extensions/index.d.ts
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/binary-extensions/index.js
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/binary-extensions/license
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/binary-extensions/package.json
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/binary-extensions/readme.md
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/braces/CHANGELOG.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/braces/LICENSE
+-rw-r--r--   0        0        0    21130 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/braces/README.md
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/braces/index.js
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/braces/package.json
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/braces/lib/compile.js
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/braces/lib/constants.js
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/braces/lib/expand.js
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/braces/lib/parse.js
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/braces/lib/stringify.js
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/braces/lib/utils.js
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/buffer-from/LICENSE
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/buffer-from/index.js
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/buffer-from/package.json
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/buffer-from/readme.md
+-rw-r--r--   0        0        0     8899 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chalk/index.d.ts
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chalk/license
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chalk/package.json
+-rw-r--r--   0        0        0    13365 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chalk/readme.md
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chalk/source/index.js
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chalk/source/templates.js
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chalk/source/util.js
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chokidar/LICENSE
+-rw-r--r--   0        0        0    14392 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chokidar/README.md
+-rw-r--r--   0        0        0    28379 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chokidar/index.js
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chokidar/package.json
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chokidar/lib/constants.js
+-rw-r--r--   0        0        0    16368 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chokidar/lib/fsevents-handler.js
+-rw-r--r--   0        0        0    20067 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chokidar/lib/nodefs-handler.js
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/chokidar/types/index.d.ts
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/color-convert/CHANGELOG.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/color-convert/LICENSE
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/color-convert/README.md
+-rw-r--r--   0        0        0    17040 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/color-convert/conversions.js
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/color-convert/index.js
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/color-convert/package.json
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/color-convert/route.js
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/color-name/LICENSE
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/color-name/README.md
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/color-name/index.js
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/color-name/package.json
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/command-line-args/LICENSE
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/command-line-args/README.md
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/command-line-args/index.mjs
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/command-line-args/package.json
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/command-line-args/lib/argv-parser.mjs
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/command-line-args/lib/argv-tools.mjs
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/command-line-args/lib/option-definition.mjs
+-rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/command-line-args/lib/option-definitions.mjs
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/command-line-args/lib/option-flag.mjs
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/command-line-args/lib/option.mjs
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/command-line-args/lib/output-grouped.mjs
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/command-line-args/lib/output.mjs
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/fill-range/LICENSE
+-rw-r--r--   0        0        0     7486 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/fill-range/README.md
+-rw-r--r--   0        0        0     6315 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/fill-range/index.js
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/fill-range/package.json
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/find-replace/LICENSE
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/find-replace/README.hbs
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/find-replace/README.md
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/find-replace/index.mjs
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/find-replace/package.json
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/fsevents/LICENSE
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/fsevents/README.md
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/fsevents/fsevents.d.ts
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/fsevents/fsevents.js
+-rwxr-xr-x   0        0        0   163626 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/fsevents/fsevents.node
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/fsevents/package.json
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/glob-parent/CHANGELOG.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/glob-parent/LICENSE
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/glob-parent/README.md
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/glob-parent/index.js
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/has-flag/index.d.ts
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/has-flag/index.js
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/has-flag/license
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/has-flag/package.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/has-flag/readme.md
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-binary-path/index.d.ts
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-binary-path/index.js
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-binary-path/license
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-binary-path/package.json
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-binary-path/readme.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-extglob/LICENSE
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-extglob/README.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-extglob/index.js
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-extglob/package.json
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-glob/LICENSE
+-rw-r--r--   0        0        0     7145 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-glob/README.md
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-glob/index.js
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-glob/package.json
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-number/LICENSE
+-rw-r--r--   0        0        0     6514 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-number/README.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-number/index.js
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/is-number/package.json
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/CHANGELOG.md
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/LICENSE.md
+-rw-r--r--   0        0        0    14129 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/README.md
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/SECURITY.md
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/package.json
+-rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/esm/main.d.ts
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/esm/main.js
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/esm/impl/edit.js
+-rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/esm/impl/format.js
+-rw-r--r--   0        0        0    24708 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/esm/impl/parser.js
+-rw-r--r--   0        0        0    19188 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/esm/impl/scanner.js
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/esm/impl/string-intern.js
+-rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/umd/main.d.ts
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/umd/main.js
+-rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/umd/impl/edit.js
+-rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/umd/impl/format.js
+-rw-r--r--   0        0        0    28290 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/umd/impl/parser.js
+-rw-r--r--   0        0        0    21446 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/umd/impl/scanner.js
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/jsonc-parser/lib/umd/impl/string-intern.js
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/leven/index.d.ts
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/leven/index.js
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/leven/license
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/leven/package.json
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/leven/readme.md
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/lodash.camelcase/LICENSE
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/lodash.camelcase/README.md
+-rw-r--r--   0        0        0    18757 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/lodash.camelcase/index.js
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/lodash.camelcase/package.json
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/normalize-path/LICENSE
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/normalize-path/README.md
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/normalize-path/index.js
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/normalize-path/package.json
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/picomatch/CHANGELOG.md
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/picomatch/LICENSE
+-rw-r--r--   0        0        0    27445 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/picomatch/README.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/picomatch/index.js
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/picomatch/package.json
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/picomatch/lib/constants.js
+-rw-r--r--   0        0        0    27763 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/picomatch/lib/parse.js
+-rw-r--r--   0        0        0     9956 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/picomatch/lib/picomatch.js
+-rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/picomatch/lib/scan.js
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/picomatch/lib/utils.js
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/readdirp/LICENSE
+-rw-r--r--   0        0        0     6942 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/readdirp/README.md
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/readdirp/index.d.ts
+-rw-r--r--   0        0        0     8876 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/readdirp/index.js
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/readdirp/package.json
+-rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/CHANGELOG.md
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/LICENSE
+-rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/README.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/package.json
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/source-map.d.ts
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/source-map.js
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/lib/array-set.js
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/lib/base64-vlq.js
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/lib/base64.js
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/lib/binary-search.js
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/lib/mapping-list.js
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/lib/quick-sort.js
+-rw-r--r--   0        0        0    40562 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/lib/source-map-consumer.js
+-rw-r--r--   0        0        0    14356 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/lib/source-map-generator.js
+-rw-r--r--   0        0        0    13808 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/lib/source-node.js
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map/lib/util.js
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map-support/LICENSE.md
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map-support/README.md
+-rw-r--r--   0        0        0    53583 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map-support/browser-source-map-support.js
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map-support/package.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map-support/register-hook-require.js
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map-support/register.js
+-rw-r--r--   0        0        0    20223 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/source-map-support/source-map-support.js
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/supports-color/browser.js
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/supports-color/index.js
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/supports-color/license
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/supports-color/package.json
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/supports-color/readme.md
+-rw-r--r--   0        0        0    16509 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tmp/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tmp/LICENSE
+-rw-r--r--   0        0        0    12531 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tmp/README.md
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tmp/package.json
+-rw-r--r--   0        0        0    22676 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tmp/lib/tmp.js
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/to-regex-range/LICENSE
+-rw-r--r--   0        0        0    13585 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/to-regex-range/README.md
+-rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/to-regex-range/index.js
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/to-regex-range/package.json
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tslib/CopyrightNotice.txt
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tslib/LICENSE.txt
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tslib/README.md
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tslib/package.json
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tslib/tslib.d.ts
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tslib/tslib.es6.html
+-rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tslib/tslib.es6.js
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tslib/tslib.html
+-rw-r--r--   0        0        0    13204 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tslib/tslib.js
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tslib/modules/index.js
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tslib/modules/package.json
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/typical/LICENSE
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/typical/README.hbs
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/typical/README.md
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/typical/index.mjs
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/typical/package.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/License.txt
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/README.md
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/browser.d.ts
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/browser.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/node.cmd
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/node.d.ts
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/node.js
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/package.json
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/thirdpartynotices.txt
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/browser/main.d.ts
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/browser/main.js
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/browser/ril.d.ts
+-rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/browser/ril.js
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/api.d.ts
+-rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/api.js
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/cancellation.d.ts
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/cancellation.js
+-rw-r--r--   0        0        0    17906 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/connection.d.ts
+-rw-r--r--   0        0        0    51184 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/connection.js
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/disposable.d.ts
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/disposable.js
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/encoding.d.ts
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/encoding.js
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/events.d.ts
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/events.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/is.d.ts
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/is.js
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/linkedMap.d.ts
+-rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/linkedMap.js
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messageBuffer.d.ts
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messageBuffer.js
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messageReader.d.ts
+-rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messageReader.js
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messageWriter.d.ts
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messageWriter.js
+-rw-r--r--   0        0        0    12626 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messages.d.ts
+-rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messages.js
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/ral.d.ts
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/ral.js
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/semaphore.d.ts
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/semaphore.js
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/sharedArrayCancellation.d.ts
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/sharedArrayCancellation.js
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/node/main.d.ts
+-rw-r--r--   0        0        0     9778 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/node/main.js
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/node/ril.d.ts
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/lib/node/ril.js
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-jsonrpc/typings/thenable.d.ts
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/License.txt
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/README.md
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/browser.d.ts
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/browser.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/node.cmd
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/node.d.ts
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/node.js
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/package.json
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/thirdpartynotices.txt
+-rwxr-xr-x   0        0        0     2754 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/bin/installServerIntoExtension
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/browser/main.d.ts
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/browser/main.js
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/api.d.ts
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/api.js
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/callHierarchy.d.ts
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/callHierarchy.js
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/configuration.d.ts
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/configuration.js
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/diagnostic.d.ts
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/diagnostic.js
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/fileOperations.d.ts
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/fileOperations.js
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/inlayHint.d.ts
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/inlayHint.js
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/inlineValue.d.ts
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/inlineValue.js
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/linkedEditingRange.d.ts
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/linkedEditingRange.js
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/moniker.d.ts
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/moniker.js
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/notebook.d.ts
+-rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/notebook.js
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/progress.d.ts
+-rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/progress.js
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/semanticTokens.d.ts
+-rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/semanticTokens.js
+-rw-r--r--   0        0        0    37013 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/server.d.ts
+-rw-r--r--   0        0        0    34971 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/server.js
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/showDocument.d.ts
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/showDocument.js
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/textDocuments.d.ts
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/textDocuments.js
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/typeHierarchy.d.ts
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/typeHierarchy.js
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/workspaceFolder.d.ts
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/workspaceFolder.js
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/utils/is.d.ts
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/utils/is.js
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/utils/uuid.d.ts
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/common/utils/uuid.js
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/node/files.d.ts
+-rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/node/files.js
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/node/main.d.ts
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/node/main.js
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/node/resolve.d.ts
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/lib/node/resolve.js
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver/typings/thenable.d.ts
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/License.txt
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/README.md
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/browser.d.ts
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/browser.js
+-rw-r--r--   0        0        0    21796 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/metaModel.schema.json
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/node.cmd
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/node.d.ts
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/node.js
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/package.json
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/thirdpartynotices.txt
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/browser/main.d.ts
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/browser/main.js
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/api.d.ts
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/api.js
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/connection.d.ts
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/connection.js
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/messages.d.ts
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/messages.js
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.$.d.ts
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.$.js
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.callHierarchy.d.ts
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.callHierarchy.js
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.colorProvider.d.ts
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.colorProvider.js
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.configuration.d.ts
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.configuration.js
+-rw-r--r--   0        0        0   112267 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.d.ts
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.declaration.d.ts
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.declaration.js
+-rw-r--r--   0        0        0    10782 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.diagnostic.d.ts
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.diagnostic.js
+-rw-r--r--   0        0        0     9616 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.fileOperations.d.ts
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.fileOperations.js
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.foldingRange.d.ts
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.foldingRange.js
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.implementation.d.ts
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.implementation.js
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlayHint.d.ts
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlayHint.js
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlineValue.d.ts
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlineValue.js
+-rw-r--r--   0        0        0    55332 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.js
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.linkedEditingRange.d.ts
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.linkedEditingRange.js
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.moniker.d.ts
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.moniker.js
+-rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.notebook.d.ts
+-rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.notebook.js
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.progress.d.ts
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.progress.js
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.selectionRange.d.ts
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.selectionRange.js
+-rw-r--r--   0        0        0     7994 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.semanticTokens.d.ts
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.semanticTokens.js
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.showDocument.d.ts
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.showDocument.js
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeDefinition.d.ts
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeDefinition.js
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeHierarchy.d.ts
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeHierarchy.js
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.workspaceFolder.d.ts
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.workspaceFolder.js
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/utils/is.d.ts
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/utils/is.js
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/node/main.d.ts
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/node/main.js
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-textdocument/License.txt
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-textdocument/README.md
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-textdocument/package.json
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-textdocument/thirdpartynotices.txt
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-textdocument/lib/esm/main.d.ts
+-rw-r--r--   0        0        0    11258 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-textdocument/lib/esm/main.js
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-textdocument/lib/umd/main.d.ts
+-rw-r--r--   0        0        0    12811 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-textdocument/lib/umd/main.js
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-types/License.txt
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-types/README.md
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-types/package.json
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-types/thirdpartynotices.txt
+-rw-r--r--   0        0        0    97126 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-types/lib/esm/main.d.ts
+-rw-r--r--   0        0        0    78825 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-types/lib/esm/main.js
+-rw-r--r--   0        0        0    97126 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-types/lib/umd/main.d.ts
+-rw-r--r--   0        0        0    92006 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-languageserver-types/lib/umd/main.js
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/LICENSE.md
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/README.md
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/SECURITY.md
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/package.json
+-rw-r--r--   0        0        0    10742 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/lib/esm/index.mjs
+-rw-r--r--   0        0        0    62941 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/lib/esm/index.mjs.map
+-rw-r--r--   0        0        0    11020 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/lib/umd/charCode.d.ts
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/lib/umd/charCode.js
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/lib/umd/index.d.ts
+-rw-r--r--   0        0        0    11853 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/lib/umd/index.js
+-rw-r--r--   0        0        0    62976 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/lib/umd/index.js.map
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/lib/umd/platform.d.ts
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/lib/umd/platform.js
+-rw-r--r--   0        0        0     5843 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/lib/umd/uri.d.ts
+-rw-r--r--   0        0        0    21939 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/lib/umd/uri.js
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/lib/umd/utils.d.ts
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 libro-0.1.4/node_modules/vscode-uri/lib/umd/utils.js
+-rw-r--r--   0        0        0    68855 2020-02-02 00:00:00.000000 libro-0.1.4/src/dev-config/jupyter_server_config.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/_version.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/app.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/handler.py
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/1330.async.js
+-rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/1438.async.js
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/161.async.js
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/1639.async.js
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/1772.async.js
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/1838.async.js
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/2048.async.js
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/2118.async.js
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/2130.async.js
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/2999.async.js
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/3572.async.js
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/405.async.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/4113.async.js
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/4116.async.js
+-rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/4123.async.js
+-rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/417.async.js
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/4266.async.js
+-rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/4343.async.js
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/4541.async.js
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/4621.async.js
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/4658.async.js
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/4849.async.js
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/4887.async.js
+-rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/5250.async.js
+-rw-r--r--   0        0        0  9350375 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/5332.async.js
+-rw-r--r--   0        0        0 28196436 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/5622.async.js
+-rw-r--r--   0        0        0   255768 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/5622.chunk.css
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/610.async.js
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/628.async.js
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/6357.async.js
+-rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/6404.async.js
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/6486.async.js
+-rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/6730.async.js
+-rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/6962.async.js
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/6999.async.js
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/7162.async.js
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/7715.async.js
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/7851.async.js
+-rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/79.async.js
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/8227.async.js
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/8305.async.js
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/8370.async.js
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/8525.async.js
+-rw-r--r--   0        0        0    74158 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/8945.chunk.css
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/9095.async.js
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/9150.async.js
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/9402.async.js
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/9669.async.js
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/9674.async.js
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/9749.async.js
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/9905.async.js
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/index.html
+-rw-r--r--   0        0        0    10229 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/p__libro__index.async.js
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/p__libro__index.chunk.css
+-rw-r--r--   0        0        0   848011 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/umi.js
+-rw-r--r--   0        0        0    73464 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/static/codicon.589e0820.ttf
+-rw-r--r--   0        0        0    49764 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/static/devopicons.3c46801a.woff2
+-rw-r--r--   0        0        0    90680 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/static/file-icons.2cbb51ef.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/static/fontawesome-webfont.2b13baa7.eot
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/static/fontawesome-webfont.8a7cb27d.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/static/fontawesome-webfont.cf011583.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/static/fontawesome-webfont.e9955780.woff2
+-rw-r--r--   0        0        0   387787 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/static/fontawesome-webfont.f05dad85.svg
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/static/fontawesome.e9955780.woff2
+-rw-r--r--   0        0        0    24412 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/static/mfixx.8e0807ce.woff2
+-rw-r--r--   0        0        0    20248 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/static/octicons.c982f59d.woff2
+-rw-r--r--   0        0        0   466610 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/static/onig.25dd2e6f.wasm
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/static/static/plotly.eb7b9072.svg
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/templates/error.html
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/templates/libro.html
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 libro-0.1.4/src/libro_server/templates/page.html
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 libro-0.1.4/.gitignore
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 libro-0.1.4/README.md
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 libro-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 libro-0.1.4/PKG-INFO
```

### Comparing `libro-0.1.3/node_modules/.package-lock.json` & `libro-0.1.4/node_modules/.package-lock.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@difizen/libro-analyzer/LICENSE.txt` & `libro-0.1.4/node_modules/@difizen/libro-analyzer/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@difizen/libro-analyzer/README.md` & `libro-0.1.4/node_modules/@difizen/libro-analyzer/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@difizen/libro-analyzer/package.json` & `libro-0.1.4/node_modules/@difizen/libro-analyzer/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@iarna/toml/CHANGELOG.md` & `libro-0.1.4/node_modules/@iarna/toml/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@iarna/toml/LICENSE` & `libro-0.1.4/node_modules/@iarna/toml/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@iarna/toml/README.md` & `libro-0.1.4/node_modules/@iarna/toml/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@iarna/toml/index.d.ts` & `libro-0.1.4/node_modules/@iarna/toml/index.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@iarna/toml/package.json` & `libro-0.1.4/node_modules/@iarna/toml/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@iarna/toml/parse-async.js` & `libro-0.1.4/node_modules/@iarna/toml/parse-async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@iarna/toml/parse-pretty-error.js` & `libro-0.1.4/node_modules/@iarna/toml/parse-pretty-error.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@iarna/toml/parse-stream.js` & `libro-0.1.4/node_modules/@iarna/toml/parse-stream.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@iarna/toml/stringify.js` & `libro-0.1.4/node_modules/@iarna/toml/stringify.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@iarna/toml/lib/create-datetime-float.js` & `libro-0.1.4/node_modules/@iarna/toml/lib/create-datetime-float.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@iarna/toml/lib/parser-debug.js` & `libro-0.1.4/node_modules/@iarna/toml/lib/parser-debug.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@iarna/toml/lib/parser.js` & `libro-0.1.4/node_modules/@iarna/toml/lib/parser.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@iarna/toml/lib/toml-parser.js` & `libro-0.1.4/node_modules/@iarna/toml/lib/toml-parser.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@types/emscripten/LICENSE` & `libro-0.1.4/node_modules/@types/emscripten/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@types/emscripten/README.md` & `libro-0.1.4/node_modules/@types/emscripten/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@types/emscripten/index.d.ts` & `libro-0.1.4/node_modules/@types/emscripten/index.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@types/emscripten/package.json` & `libro-0.1.4/node_modules/@types/emscripten/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/README.md` & `libro-0.1.4/node_modules/@yarnpkg/fslib/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/package.json` & `libro-0.1.4/node_modules/@yarnpkg/fslib/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/AliasFS.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/AliasFS.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/AliasFS.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/AliasFS.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/CwdFS.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/CwdFS.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/CwdFS.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/CwdFS.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/FakeFS.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/FakeFS.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/FakeFS.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/FakeFS.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/JailFS.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/JailFS.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/JailFS.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/JailFS.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/LazyFS.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/LazyFS.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/LazyFS.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/LazyFS.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NoFS.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/NoFS.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NoFS.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/NoFS.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NodeFS.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/NodeFS.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NodeFS.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/NodeFS.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NodePathFS.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/NodePathFS.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NodePathFS.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/NodePathFS.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ProxiedFS.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/ProxiedFS.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ProxiedFS.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/ProxiedFS.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/VirtualFS.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/VirtualFS.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/VirtualFS.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/VirtualFS.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ZipFS.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/ZipFS.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ZipFS.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/ZipFS.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ZipOpenFS.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/ZipOpenFS.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ZipOpenFS.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/ZipOpenFS.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/constants.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/constants.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/errors.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/errors.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/errors.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/errors.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/index.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/index.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/index.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/path.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/path.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/path.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/path.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/statUtils.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/statUtils.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/statUtils.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/statUtils.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/xfs.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/xfs.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/xfs.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/xfs.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/copyPromise.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/copyPromise.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/copyPromise.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/copyPromise.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/opendir.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/opendir.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/opendir.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/opendir.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile/CustomStatWatcher.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile/CustomStatWatcher.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile/CustomStatWatcher.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile/CustomStatWatcher.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/patchFs/FileHandle.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/patchFs/FileHandle.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/patchFs/FileHandle.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/patchFs/FileHandle.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/fslib/lib/patchFs/patchFs.js` & `libro-0.1.4/node_modules/@yarnpkg/fslib/lib/patchFs/patchFs.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/libzip/package.json` & `libro-0.1.4/node_modules/@yarnpkg/libzip/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/libzip/lib/async.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/libzip/lib/async.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/libzip/lib/async.js` & `libro-0.1.4/node_modules/@yarnpkg/libzip/lib/async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/libzip/lib/libzipAsync.js` & `libro-0.1.4/node_modules/@yarnpkg/libzip/lib/libzipAsync.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/libzip/lib/libzipSync.js` & `libro-0.1.4/node_modules/@yarnpkg/libzip/lib/libzipSync.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/libzip/lib/makeInterface.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/libzip/lib/makeInterface.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/libzip/lib/makeInterface.js` & `libro-0.1.4/node_modules/@yarnpkg/libzip/lib/makeInterface.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/libzip/lib/sync.d.ts` & `libro-0.1.4/node_modules/@yarnpkg/libzip/lib/sync.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/@yarnpkg/libzip/lib/sync.js` & `libro-0.1.4/node_modules/@yarnpkg/libzip/lib/sync.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/ansi-styles/index.d.ts` & `libro-0.1.4/node_modules/ansi-styles/index.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/ansi-styles/index.js` & `libro-0.1.4/node_modules/ansi-styles/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/ansi-styles/license` & `libro-0.1.4/node_modules/ansi-styles/license`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/ansi-styles/package.json` & `libro-0.1.4/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/ansi-styles/readme.md` & `libro-0.1.4/node_modules/ansi-styles/readme.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/anymatch/LICENSE` & `libro-0.1.4/node_modules/anymatch/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/anymatch/README.md` & `libro-0.1.4/node_modules/anymatch/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/anymatch/index.d.ts` & `libro-0.1.4/node_modules/anymatch/index.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/anymatch/index.js` & `libro-0.1.4/node_modules/anymatch/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/anymatch/package.json` & `libro-0.1.4/node_modules/anymatch/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/array-back/LICENSE` & `libro-0.1.4/node_modules/array-back/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/array-back/README.hbs` & `libro-0.1.4/node_modules/array-back/README.hbs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/array-back/README.md` & `libro-0.1.4/node_modules/array-back/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/array-back/index.mjs` & `libro-0.1.4/node_modules/array-back/index.mjs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/array-back/package.json` & `libro-0.1.4/node_modules/array-back/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/binary-extensions/binary-extensions.json` & `libro-0.1.4/node_modules/binary-extensions/binary-extensions.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/binary-extensions/license` & `libro-0.1.4/node_modules/binary-extensions/license`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/binary-extensions/package.json` & `libro-0.1.4/node_modules/binary-extensions/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/binary-extensions/readme.md` & `libro-0.1.4/node_modules/binary-extensions/readme.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/braces/CHANGELOG.md` & `libro-0.1.4/node_modules/braces/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/braces/LICENSE` & `libro-0.1.4/node_modules/braces/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/braces/README.md` & `libro-0.1.4/node_modules/braces/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/braces/index.js` & `libro-0.1.4/node_modules/braces/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/braces/package.json` & `libro-0.1.4/node_modules/braces/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/braces/lib/compile.js` & `libro-0.1.4/node_modules/braces/lib/compile.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/braces/lib/constants.js` & `libro-0.1.4/node_modules/braces/lib/constants.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/braces/lib/expand.js` & `libro-0.1.4/node_modules/braces/lib/expand.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/braces/lib/parse.js` & `libro-0.1.4/node_modules/braces/lib/parse.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/braces/lib/stringify.js` & `libro-0.1.4/node_modules/braces/lib/stringify.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/braces/lib/utils.js` & `libro-0.1.4/node_modules/braces/lib/utils.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/buffer-from/LICENSE` & `libro-0.1.4/node_modules/buffer-from/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/buffer-from/index.js` & `libro-0.1.4/node_modules/buffer-from/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/buffer-from/readme.md` & `libro-0.1.4/node_modules/buffer-from/readme.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chalk/index.d.ts` & `libro-0.1.4/node_modules/chalk/index.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chalk/license` & `libro-0.1.4/node_modules/chalk/license`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chalk/package.json` & `libro-0.1.4/node_modules/chalk/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chalk/readme.md` & `libro-0.1.4/node_modules/chalk/readme.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chalk/source/index.js` & `libro-0.1.4/node_modules/chalk/source/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chalk/source/templates.js` & `libro-0.1.4/node_modules/chalk/source/templates.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chalk/source/util.js` & `libro-0.1.4/node_modules/chalk/source/util.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chokidar/LICENSE` & `libro-0.1.4/node_modules/chokidar/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chokidar/README.md` & `libro-0.1.4/node_modules/chokidar/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chokidar/index.js` & `libro-0.1.4/node_modules/chokidar/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chokidar/package.json` & `libro-0.1.4/node_modules/chokidar/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chokidar/lib/constants.js` & `libro-0.1.4/node_modules/chokidar/lib/constants.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chokidar/lib/fsevents-handler.js` & `libro-0.1.4/node_modules/chokidar/lib/fsevents-handler.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chokidar/lib/nodefs-handler.js` & `libro-0.1.4/node_modules/chokidar/lib/nodefs-handler.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/chokidar/types/index.d.ts` & `libro-0.1.4/node_modules/chokidar/types/index.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/color-convert/CHANGELOG.md` & `libro-0.1.4/node_modules/color-convert/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/color-convert/LICENSE` & `libro-0.1.4/node_modules/color-convert/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/color-convert/README.md` & `libro-0.1.4/node_modules/color-convert/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/color-convert/conversions.js` & `libro-0.1.4/node_modules/color-convert/conversions.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/color-convert/index.js` & `libro-0.1.4/node_modules/color-convert/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/color-convert/package.json` & `libro-0.1.4/node_modules/color-convert/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/color-convert/route.js` & `libro-0.1.4/node_modules/color-convert/route.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/color-name/LICENSE` & `libro-0.1.4/node_modules/color-name/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/color-name/index.js` & `libro-0.1.4/node_modules/color-name/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/color-name/package.json` & `libro-0.1.4/node_modules/color-name/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/command-line-args/LICENSE` & `libro-0.1.4/node_modules/command-line-args/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/command-line-args/README.md` & `libro-0.1.4/node_modules/command-line-args/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/command-line-args/index.mjs` & `libro-0.1.4/node_modules/command-line-args/index.mjs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/command-line-args/package.json` & `libro-0.1.4/node_modules/command-line-args/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/command-line-args/lib/argv-parser.mjs` & `libro-0.1.4/node_modules/command-line-args/lib/argv-parser.mjs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/command-line-args/lib/argv-tools.mjs` & `libro-0.1.4/node_modules/command-line-args/lib/argv-tools.mjs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/command-line-args/lib/option-definition.mjs` & `libro-0.1.4/node_modules/command-line-args/lib/option-definition.mjs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/command-line-args/lib/option-definitions.mjs` & `libro-0.1.4/node_modules/command-line-args/lib/option-definitions.mjs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/command-line-args/lib/option.mjs` & `libro-0.1.4/node_modules/command-line-args/lib/option.mjs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/command-line-args/lib/output-grouped.mjs` & `libro-0.1.4/node_modules/command-line-args/lib/output-grouped.mjs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/command-line-args/lib/output.mjs` & `libro-0.1.4/node_modules/command-line-args/lib/output.mjs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/fill-range/LICENSE` & `libro-0.1.4/node_modules/fill-range/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/fill-range/README.md` & `libro-0.1.4/node_modules/fill-range/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/fill-range/index.js` & `libro-0.1.4/node_modules/fill-range/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/fill-range/package.json` & `libro-0.1.4/node_modules/fill-range/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/find-replace/LICENSE` & `libro-0.1.4/node_modules/find-replace/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/find-replace/README.hbs` & `libro-0.1.4/node_modules/find-replace/README.hbs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/find-replace/README.md` & `libro-0.1.4/node_modules/find-replace/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/find-replace/index.mjs` & `libro-0.1.4/node_modules/find-replace/index.mjs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/find-replace/package.json` & `libro-0.1.4/node_modules/find-replace/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/fsevents/LICENSE` & `libro-0.1.4/node_modules/fsevents/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/fsevents/README.md` & `libro-0.1.4/node_modules/fsevents/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/fsevents/fsevents.d.ts` & `libro-0.1.4/node_modules/fsevents/fsevents.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/fsevents/fsevents.js` & `libro-0.1.4/node_modules/fsevents/fsevents.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/fsevents/fsevents.node` & `libro-0.1.4/node_modules/fsevents/fsevents.node`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/fsevents/package.json` & `libro-0.1.4/node_modules/fsevents/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/glob-parent/CHANGELOG.md` & `libro-0.1.4/node_modules/glob-parent/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/glob-parent/LICENSE` & `libro-0.1.4/node_modules/glob-parent/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/glob-parent/README.md` & `libro-0.1.4/node_modules/glob-parent/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/glob-parent/index.js` & `libro-0.1.4/node_modules/glob-parent/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/glob-parent/package.json` & `libro-0.1.4/node_modules/glob-parent/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/has-flag/index.d.ts` & `libro-0.1.4/node_modules/has-flag/index.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/has-flag/license` & `libro-0.1.4/node_modules/has-flag/license`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/has-flag/package.json` & `libro-0.1.4/node_modules/has-flag/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/has-flag/readme.md` & `libro-0.1.4/node_modules/has-flag/readme.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/is-binary-path/license` & `libro-0.1.4/node_modules/is-binary-path/license`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/is-binary-path/package.json` & `libro-0.1.4/node_modules/is-binary-path/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/is-binary-path/readme.md` & `libro-0.1.4/node_modules/is-binary-path/readme.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/is-extglob/LICENSE` & `libro-0.1.4/node_modules/is-extglob/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/is-extglob/README.md` & `libro-0.1.4/node_modules/is-extglob/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/is-extglob/package.json` & `libro-0.1.4/node_modules/is-extglob/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/is-glob/LICENSE` & `libro-0.1.4/node_modules/is-glob/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/is-glob/README.md` & `libro-0.1.4/node_modules/is-glob/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/is-glob/index.js` & `libro-0.1.4/node_modules/is-glob/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/is-glob/package.json` & `libro-0.1.4/node_modules/is-glob/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/is-number/LICENSE` & `libro-0.1.4/node_modules/is-number/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/is-number/README.md` & `libro-0.1.4/node_modules/is-number/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/is-number/package.json` & `libro-0.1.4/node_modules/is-number/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/CHANGELOG.md` & `libro-0.1.4/node_modules/jsonc-parser/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/LICENSE.md` & `libro-0.1.4/node_modules/jsonc-parser/LICENSE.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/README.md` & `libro-0.1.4/node_modules/jsonc-parser/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/SECURITY.md` & `libro-0.1.4/node_modules/jsonc-parser/SECURITY.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/package.json` & `libro-0.1.4/node_modules/jsonc-parser/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/esm/main.d.ts` & `libro-0.1.4/node_modules/jsonc-parser/lib/esm/main.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/esm/main.js` & `libro-0.1.4/node_modules/jsonc-parser/lib/esm/main.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/edit.js` & `libro-0.1.4/node_modules/jsonc-parser/lib/esm/impl/edit.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/format.js` & `libro-0.1.4/node_modules/jsonc-parser/lib/esm/impl/format.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/parser.js` & `libro-0.1.4/node_modules/jsonc-parser/lib/esm/impl/parser.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/scanner.js` & `libro-0.1.4/node_modules/jsonc-parser/lib/esm/impl/scanner.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/string-intern.js` & `libro-0.1.4/node_modules/jsonc-parser/lib/esm/impl/string-intern.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/umd/main.d.ts` & `libro-0.1.4/node_modules/jsonc-parser/lib/umd/main.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/umd/main.js` & `libro-0.1.4/node_modules/jsonc-parser/lib/umd/main.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/edit.js` & `libro-0.1.4/node_modules/jsonc-parser/lib/umd/impl/edit.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/format.js` & `libro-0.1.4/node_modules/jsonc-parser/lib/umd/impl/format.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/parser.js` & `libro-0.1.4/node_modules/jsonc-parser/lib/umd/impl/parser.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/scanner.js` & `libro-0.1.4/node_modules/jsonc-parser/lib/umd/impl/scanner.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/string-intern.js` & `libro-0.1.4/node_modules/jsonc-parser/lib/umd/impl/string-intern.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/leven/index.js` & `libro-0.1.4/node_modules/leven/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/leven/license` & `libro-0.1.4/node_modules/leven/license`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/leven/package.json` & `libro-0.1.4/node_modules/leven/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/leven/readme.md` & `libro-0.1.4/node_modules/leven/readme.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/lodash.camelcase/LICENSE` & `libro-0.1.4/node_modules/lodash.camelcase/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/lodash.camelcase/index.js` & `libro-0.1.4/node_modules/lodash.camelcase/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/lodash.camelcase/package.json` & `libro-0.1.4/node_modules/lodash.camelcase/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/normalize-path/LICENSE` & `libro-0.1.4/node_modules/normalize-path/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/normalize-path/README.md` & `libro-0.1.4/node_modules/normalize-path/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/normalize-path/index.js` & `libro-0.1.4/node_modules/normalize-path/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/normalize-path/package.json` & `libro-0.1.4/node_modules/normalize-path/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/picomatch/CHANGELOG.md` & `libro-0.1.4/node_modules/picomatch/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/picomatch/LICENSE` & `libro-0.1.4/node_modules/picomatch/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/picomatch/README.md` & `libro-0.1.4/node_modules/picomatch/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/picomatch/package.json` & `libro-0.1.4/node_modules/picomatch/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/picomatch/lib/constants.js` & `libro-0.1.4/node_modules/picomatch/lib/constants.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/picomatch/lib/parse.js` & `libro-0.1.4/node_modules/picomatch/lib/parse.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/picomatch/lib/picomatch.js` & `libro-0.1.4/node_modules/picomatch/lib/picomatch.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/picomatch/lib/scan.js` & `libro-0.1.4/node_modules/picomatch/lib/scan.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/picomatch/lib/utils.js` & `libro-0.1.4/node_modules/picomatch/lib/utils.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/readdirp/LICENSE` & `libro-0.1.4/node_modules/readdirp/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/readdirp/README.md` & `libro-0.1.4/node_modules/readdirp/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/readdirp/index.d.ts` & `libro-0.1.4/node_modules/readdirp/index.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/readdirp/index.js` & `libro-0.1.4/node_modules/readdirp/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/readdirp/package.json` & `libro-0.1.4/node_modules/readdirp/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/CHANGELOG.md` & `libro-0.1.4/node_modules/source-map/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/LICENSE` & `libro-0.1.4/node_modules/source-map/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/README.md` & `libro-0.1.4/node_modules/source-map/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/package.json` & `libro-0.1.4/node_modules/source-map/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/source-map.d.ts` & `libro-0.1.4/node_modules/source-map/source-map.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/lib/array-set.js` & `libro-0.1.4/node_modules/source-map/lib/array-set.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/lib/base64-vlq.js` & `libro-0.1.4/node_modules/source-map/lib/base64-vlq.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/lib/base64.js` & `libro-0.1.4/node_modules/source-map/lib/base64.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/lib/binary-search.js` & `libro-0.1.4/node_modules/source-map/lib/binary-search.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/lib/mapping-list.js` & `libro-0.1.4/node_modules/source-map/lib/mapping-list.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/lib/quick-sort.js` & `libro-0.1.4/node_modules/source-map/lib/quick-sort.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/lib/source-map-consumer.js` & `libro-0.1.4/node_modules/source-map/lib/source-map-consumer.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/lib/source-map-generator.js` & `libro-0.1.4/node_modules/source-map/lib/source-map-generator.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/lib/source-node.js` & `libro-0.1.4/node_modules/source-map/lib/source-node.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map/lib/util.js` & `libro-0.1.4/node_modules/source-map/lib/util.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map-support/LICENSE.md` & `libro-0.1.4/node_modules/source-map-support/LICENSE.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map-support/README.md` & `libro-0.1.4/node_modules/source-map-support/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map-support/browser-source-map-support.js` & `libro-0.1.4/node_modules/source-map-support/browser-source-map-support.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map-support/package.json` & `libro-0.1.4/node_modules/source-map-support/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/source-map-support/source-map-support.js` & `libro-0.1.4/node_modules/source-map-support/source-map-support.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/supports-color/index.js` & `libro-0.1.4/node_modules/supports-color/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/supports-color/license` & `libro-0.1.4/node_modules/supports-color/license`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/supports-color/package.json` & `libro-0.1.4/node_modules/supports-color/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/supports-color/readme.md` & `libro-0.1.4/node_modules/supports-color/readme.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tmp/CHANGELOG.md` & `libro-0.1.4/node_modules/tmp/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tmp/LICENSE` & `libro-0.1.4/node_modules/tmp/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tmp/README.md` & `libro-0.1.4/node_modules/tmp/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tmp/package.json` & `libro-0.1.4/node_modules/tmp/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tmp/lib/tmp.js` & `libro-0.1.4/node_modules/tmp/lib/tmp.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/to-regex-range/LICENSE` & `libro-0.1.4/node_modules/to-regex-range/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/to-regex-range/README.md` & `libro-0.1.4/node_modules/to-regex-range/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/to-regex-range/index.js` & `libro-0.1.4/node_modules/to-regex-range/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/to-regex-range/package.json` & `libro-0.1.4/node_modules/to-regex-range/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tslib/CopyrightNotice.txt` & `libro-0.1.4/node_modules/tslib/CopyrightNotice.txt`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tslib/LICENSE.txt` & `libro-0.1.4/node_modules/tslib/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tslib/README.md` & `libro-0.1.4/node_modules/tslib/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tslib/package.json` & `libro-0.1.4/node_modules/tslib/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tslib/tslib.d.ts` & `libro-0.1.4/node_modules/tslib/tslib.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tslib/tslib.es6.js` & `libro-0.1.4/node_modules/tslib/tslib.es6.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tslib/tslib.js` & `libro-0.1.4/node_modules/tslib/tslib.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tslib/modules/index.js` & `libro-0.1.4/node_modules/tslib/modules/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js` & `libro-0.1.4/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/typical/LICENSE` & `libro-0.1.4/node_modules/typical/LICENSE`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/typical/README.hbs` & `libro-0.1.4/node_modules/typical/README.hbs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/typical/README.md` & `libro-0.1.4/node_modules/typical/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/typical/index.mjs` & `libro-0.1.4/node_modules/typical/index.mjs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/typical/package.json` & `libro-0.1.4/node_modules/typical/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/License.txt` & `libro-0.1.4/node_modules/vscode-jsonrpc/License.txt`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/README.md` & `libro-0.1.4/node_modules/vscode-jsonrpc/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/package.json` & `libro-0.1.4/node_modules/vscode-jsonrpc/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/thirdpartynotices.txt` & `libro-0.1.4/node_modules/vscode-jsonrpc/thirdpartynotices.txt`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/browser/main.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/browser/main.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/browser/main.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/browser/main.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/browser/ril.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/browser/ril.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/api.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/api.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/api.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/api.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/cancellation.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/cancellation.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/cancellation.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/cancellation.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/connection.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/connection.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/connection.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/connection.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/disposable.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/disposable.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/encoding.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/encoding.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/encoding.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/encoding.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/events.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/events.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/events.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/events.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/is.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/is.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/linkedMap.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/linkedMap.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/linkedMap.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/linkedMap.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageBuffer.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messageBuffer.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageBuffer.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messageBuffer.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageReader.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messageReader.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageReader.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messageReader.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageWriter.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messageWriter.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageWriter.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messageWriter.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messages.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messages.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messages.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/messages.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/ral.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/ral.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/ral.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/ral.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/semaphore.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/semaphore.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/sharedArrayCancellation.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/sharedArrayCancellation.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/sharedArrayCancellation.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/common/sharedArrayCancellation.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/node/main.d.ts` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/node/main.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/node/main.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/node/main.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-jsonrpc/lib/node/ril.js` & `libro-0.1.4/node_modules/vscode-jsonrpc/lib/node/ril.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/License.txt` & `libro-0.1.4/node_modules/vscode-languageserver/License.txt`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/README.md` & `libro-0.1.4/node_modules/vscode-languageserver/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/package.json` & `libro-0.1.4/node_modules/vscode-languageserver/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/thirdpartynotices.txt` & `libro-0.1.4/node_modules/vscode-languageserver/thirdpartynotices.txt`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/bin/installServerIntoExtension` & `libro-0.1.4/node_modules/vscode-languageserver/bin/installServerIntoExtension`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/browser/main.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/browser/main.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/browser/main.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/browser/main.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/api.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/api.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/api.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/api.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/callHierarchy.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/callHierarchy.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/callHierarchy.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/callHierarchy.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/configuration.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/configuration.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/diagnostic.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/diagnostic.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/diagnostic.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/diagnostic.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/fileOperations.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/fileOperations.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/fileOperations.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/fileOperations.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/inlayHint.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/inlayHint.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/inlayHint.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/inlayHint.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/inlineValue.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/inlineValue.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/inlineValue.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/inlineValue.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/linkedEditingRange.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/linkedEditingRange.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/linkedEditingRange.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/linkedEditingRange.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/moniker.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/moniker.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/notebook.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/notebook.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/notebook.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/notebook.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/progress.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/progress.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/progress.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/progress.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/semanticTokens.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/semanticTokens.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/semanticTokens.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/semanticTokens.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/server.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/server.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/server.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/server.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/showDocument.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/showDocument.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/textDocuments.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/textDocuments.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/textDocuments.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/textDocuments.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/typeHierarchy.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/typeHierarchy.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/typeHierarchy.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/typeHierarchy.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/workspaceFolder.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/workspaceFolder.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/utils/is.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/utils/is.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/utils/is.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/utils/is.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/utils/uuid.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/utils/uuid.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/common/utils/uuid.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/common/utils/uuid.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/node/files.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/node/files.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/node/files.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/node/files.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/node/main.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver/lib/node/main.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/node/main.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/node/main.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver/lib/node/resolve.js` & `libro-0.1.4/node_modules/vscode-languageserver/lib/node/resolve.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/License.txt` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/License.txt`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/README.md` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/metaModel.schema.json` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/metaModel.schema.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/package.json` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/thirdpartynotices.txt` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/thirdpartynotices.txt`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/browser/main.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/browser/main.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/api.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/api.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/api.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/api.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/connection.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/connection.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/connection.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/connection.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/messages.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/messages.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/messages.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/messages.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.$.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.$.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.callHierarchy.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.callHierarchy.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.callHierarchy.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.callHierarchy.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.colorProvider.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.colorProvider.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.colorProvider.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.colorProvider.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.configuration.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.configuration.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.configuration.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.configuration.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.declaration.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.declaration.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.declaration.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.declaration.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.diagnostic.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.diagnostic.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.diagnostic.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.diagnostic.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.fileOperations.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.fileOperations.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.fileOperations.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.fileOperations.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.foldingRange.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.foldingRange.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.foldingRange.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.foldingRange.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.implementation.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.implementation.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.implementation.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.implementation.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlayHint.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlayHint.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlayHint.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlayHint.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlineValue.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlineValue.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlineValue.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlineValue.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.linkedEditingRange.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.linkedEditingRange.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.linkedEditingRange.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.linkedEditingRange.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.moniker.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.moniker.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.moniker.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.moniker.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.notebook.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.notebook.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.notebook.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.notebook.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.progress.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.progress.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.progress.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.progress.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.selectionRange.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.selectionRange.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.selectionRange.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.selectionRange.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.semanticTokens.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.semanticTokens.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.semanticTokens.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.semanticTokens.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.showDocument.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.showDocument.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.showDocument.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.showDocument.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeDefinition.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeDefinition.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeDefinition.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeDefinition.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeHierarchy.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeHierarchy.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeHierarchy.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeHierarchy.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.workspaceFolder.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.workspaceFolder.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.workspaceFolder.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/protocol.workspaceFolder.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/utils/is.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/utils/is.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/utils/is.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/common/utils/is.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/node/main.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/node/main.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/node/main.js` & `libro-0.1.4/node_modules/vscode-languageserver-protocol/lib/node/main.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-textdocument/License.txt` & `libro-0.1.4/node_modules/vscode-languageserver-textdocument/License.txt`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-textdocument/README.md` & `libro-0.1.4/node_modules/vscode-languageserver-textdocument/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-textdocument/package.json` & `libro-0.1.4/node_modules/vscode-languageserver-textdocument/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-textdocument/thirdpartynotices.txt` & `libro-0.1.4/node_modules/vscode-languageserver-textdocument/thirdpartynotices.txt`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-textdocument/lib/esm/main.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-textdocument/lib/esm/main.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-textdocument/lib/esm/main.js` & `libro-0.1.4/node_modules/vscode-languageserver-textdocument/lib/esm/main.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-textdocument/lib/umd/main.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-textdocument/lib/umd/main.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-textdocument/lib/umd/main.js` & `libro-0.1.4/node_modules/vscode-languageserver-textdocument/lib/umd/main.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-types/License.txt` & `libro-0.1.4/node_modules/vscode-languageserver-types/License.txt`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-types/README.md` & `libro-0.1.4/node_modules/vscode-languageserver-types/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-types/package.json` & `libro-0.1.4/node_modules/vscode-languageserver-types/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-types/thirdpartynotices.txt` & `libro-0.1.4/node_modules/vscode-languageserver-types/thirdpartynotices.txt`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-types/lib/esm/main.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-types/lib/esm/main.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-types/lib/esm/main.js` & `libro-0.1.4/node_modules/vscode-languageserver-types/lib/esm/main.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-types/lib/umd/main.d.ts` & `libro-0.1.4/node_modules/vscode-languageserver-types/lib/umd/main.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-languageserver-types/lib/umd/main.js` & `libro-0.1.4/node_modules/vscode-languageserver-types/lib/umd/main.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/LICENSE.md` & `libro-0.1.4/node_modules/vscode-uri/LICENSE.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/README.md` & `libro-0.1.4/node_modules/vscode-uri/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/SECURITY.md` & `libro-0.1.4/node_modules/vscode-uri/SECURITY.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/package.json` & `libro-0.1.4/node_modules/vscode-uri/package.json`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/lib/esm/index.mjs` & `libro-0.1.4/node_modules/vscode-uri/lib/esm/index.mjs`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/lib/esm/index.mjs.map` & `libro-0.1.4/node_modules/vscode-uri/lib/esm/index.mjs.map`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/lib/umd/charCode.d.ts` & `libro-0.1.4/node_modules/vscode-uri/lib/umd/charCode.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/lib/umd/index.js` & `libro-0.1.4/node_modules/vscode-uri/lib/umd/index.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/lib/umd/index.js.map` & `libro-0.1.4/node_modules/vscode-uri/lib/umd/index.js.map`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/lib/umd/platform.js` & `libro-0.1.4/node_modules/vscode-uri/lib/umd/platform.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/lib/umd/uri.d.ts` & `libro-0.1.4/node_modules/vscode-uri/lib/umd/uri.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/lib/umd/uri.js` & `libro-0.1.4/node_modules/vscode-uri/lib/umd/uri.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/lib/umd/utils.d.ts` & `libro-0.1.4/node_modules/vscode-uri/lib/umd/utils.d.ts`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/node_modules/vscode-uri/lib/umd/utils.js` & `libro-0.1.4/node_modules/vscode-uri/lib/umd/utils.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/src/dev-config/jupyter_server_config.py` & `libro-0.1.4/src/dev-config/jupyter_server_config.py`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/src/libro_server/app.py` & `libro-0.1.4/src/libro_server/app.py`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/src/libro_server/handler.py` & `libro-0.1.4/src/libro_server/handler.py`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/src/libro_server/templates/libro.html` & `libro-0.1.4/src/libro_server/templates/libro.html`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/src/libro_server/templates/page.html` & `libro-0.1.4/src/libro_server/templates/page.html`

 * *Files identical despite different names*

### Comparing `libro-0.1.3/pyproject.toml` & `libro-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "libro"
-version = "0.1.3"
+version = "0.1.4"
 description = "Libro notebook editor"
 authors = [
     { name = "zhanba", email = "c5e1856@gmail.com" },
     { name = "brokun", email = "brokun0128@gmail.com" }
 ]
 dependencies = [
     "jupyter-server>=2.13.0",
```

