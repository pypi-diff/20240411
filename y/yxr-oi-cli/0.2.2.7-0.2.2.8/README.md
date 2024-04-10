# Comparing `tmp/yxr_oi_cli-0.2.2.7.tar.gz` & `tmp/yxr_oi_cli-0.2.2.8.tar.gz`

## Comparing `yxr_oi_cli-0.2.2.7.tar` & `yxr_oi_cli-0.2.2.8.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/py.typed
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/abstract/HtmlTagAbstract.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/abstract/__init__.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/__init__.py
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/account.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/analyze.py
--rwxr-xr-x   0        0        0     1540 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/completion.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/config.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/constant.py
--rw-r--r--   0        0        0    12127 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/contest.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/init.py
--rwxr-xr-x   0        0        0     1280 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/lang.py
--rwxr-xr-x   0        0        0     1102 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/main.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/problem.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/reg_list.py
--rwxr-xr-x   0        0        0     4732 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/submit.py
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/template.py
--rwxr-xr-x   0        0        0     3613 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/test.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/AtCoderAdaptor.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/AtCoder_printList.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/ojman.py
--rw-r--r--   0        0        0    13778 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/Codeforces/Codeforces.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/Codeforces/CodeforcesAdaptor.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/Codeforces/__init__.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/Codeforces/contestList.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/Codeforces/standing.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/core/DI.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/core/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/core/problem.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/model/Account.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/model/Analyze.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/model/BaseOj.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/model/Contest.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/model/FolderState.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/model/LangKV.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/model/ParseProblemResult.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/model/Problem.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/model/ProblemMeta.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/model/Result.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/model/Template.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/model/TestCase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/model/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/FileUtil.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/HtmlTag.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/HttpUtil.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/HttpUtilCookiesHelper.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/Logger.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/OJUtil.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/Provider2.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/Singleton.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/__init__.py
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/account.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/analyze.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/async2sync.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/configFolder.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/db.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/diffTool.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/enc.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/force_symlink.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/start_terminal.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/template.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/utc2local.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/wsTool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/consts/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/consts/ids.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/oi_cli2/utils/consts/platforms.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/LICENSE
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/README.md
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/pyproject.toml
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.7/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/py.typed
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/abstract/HtmlTagAbstract.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/abstract/__init__.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/__init__.py
+-rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/account.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/analyze.py
+-rwxr-xr-x   0        0        0     1540 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/completion.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/config.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/constant.py
+-rw-r--r--   0        0        0    12127 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/contest.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/init.py
+-rwxr-xr-x   0        0        0     1280 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/lang.py
+-rwxr-xr-x   0        0        0     1102 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/main.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/problem.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/reg_list.py
+-rwxr-xr-x   0        0        0     4732 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/submit.py
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/template.py
+-rwxr-xr-x   0        0        0     3613 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/test.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/AtCoderAdaptor.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/AtCoder_printList.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/__init__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/ojman.py
+-rw-r--r--   0        0        0    13835 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/Codeforces/Codeforces.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/Codeforces/CodeforcesAdaptor.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/Codeforces/__init__.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/Codeforces/contestList.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/Codeforces/standing.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/core/DI.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/core/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/core/problem.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/model/Account.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/model/Analyze.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/model/BaseOj.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/model/Contest.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/model/FolderState.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/model/LangKV.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/model/ParseProblemResult.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/model/Problem.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/model/ProblemMeta.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/model/Result.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/model/Template.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/model/TestCase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/model/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/FileUtil.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/HtmlTag.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/HttpUtil.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/HttpUtilCookiesHelper.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/Logger.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/OJUtil.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/Provider2.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/Singleton.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/__init__.py
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/account.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/analyze.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/async2sync.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/configFolder.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/db.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/diffTool.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/enc.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/force_symlink.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/start_terminal.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/template.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/utc2local.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/wsTool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/consts/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/consts/ids.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/oi_cli2/utils/consts/platforms.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/LICENSE
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/README.md
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.8/PKG-INFO
```

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/abstract/HtmlTagAbstract.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/abstract/HtmlTagAbstract.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/account.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/account.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/analyze.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/completion.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/completion.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/config.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/config.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/constant.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/constant.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/contest.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/contest.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/init.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/init.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/lang.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/lang.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/main.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/main.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/problem.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/problem.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/submit.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/submit.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/template.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/template.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/test.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/test.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/AtCoderAdaptor.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/AtCoderAdaptor.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/AtCoder_printList.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/AtCoder_printList.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/ojman.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/ojman.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/Codeforces/Codeforces.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/Codeforces/Codeforces.py`

 * *Files 3% similar despite different names*

```diff
@@ -239,16 +239,16 @@
     # TODO add timeout for ws
     # TODO 可能有别人的? pc/cc?
     async for wsresult in create_contest_ws_task_yield(http=self.http,
                                                        contest_id=contest_id,
                                                        ws_handler=custom_handler,
                                                        logger=self.api_sub_logger):
       self.logger.debug('ws res:' + str(wsresult))
-      if fix_submit_id and wsresult.submit_id != fix_submit_id:
-        self.logger.debug('[skip]fixed id not match! continue')
+      if fix_submit_id and str(wsresult.submit_id) != fix_submit_id:
+        self.logger.debug(f'[skip]fixed id not match! continue, fixed[{fix_submit_id}], ws[{wsresult.submit_id}]]')
         continue
       data = ws_result_transform(wsresult)
       yield data
       if data.cur_status not in [SubmissionResult.Status.PENDING, SubmissionResult.Status.RUNNING]:
         return
 
     results = await async_fetch_submission_page(http=self.http, problem_url=problem_url)
```

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/Codeforces/CodeforcesAdaptor.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/Codeforces/CodeforcesAdaptor.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/Codeforces/contestList.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/Codeforces/contestList.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/cli/adaptor/Codeforces/standing.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/cli/adaptor/Codeforces/standing.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/core/problem.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/core/problem.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/model/Account.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/model/Account.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/model/Analyze.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/model/Analyze.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/model/BaseOj.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/model/BaseOj.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/model/Contest.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/model/Contest.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/model/FolderState.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/model/FolderState.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/model/ParseProblemResult.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/model/ParseProblemResult.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/model/Problem.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/model/Problem.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/model/ProblemMeta.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/model/ProblemMeta.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/model/Result.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/model/Result.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/model/Template.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/model/Template.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/FileUtil.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/FileUtil.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/HtmlTag.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/HtmlTag.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/HttpUtil.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/HttpUtil.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/HttpUtilCookiesHelper.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/HttpUtilCookiesHelper.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/Logger.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/Logger.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/OJUtil.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/OJUtil.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/Provider2.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/Provider2.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/account.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/account.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/analyze.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/analyze.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/async2sync.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/async2sync.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/configFolder.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/configFolder.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/db.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/db.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/diffTool.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/diffTool.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/enc.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/enc.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/template.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/template.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/oi_cli2/utils/wsTool.py` & `yxr_oi_cli-0.2.2.8/oi_cli2/utils/wsTool.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/.gitignore` & `yxr_oi_cli-0.2.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/LICENSE` & `yxr_oi_cli-0.2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/pyproject.toml` & `yxr_oi_cli-0.2.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.7/PKG-INFO` & `yxr_oi_cli-0.2.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yxr-oi-cli
-Version: 0.2.2.7
+Version: 0.2.2.8
 Summary: Simple Online Judge Cli Tool
 Project-URL: Homepage, https://github.com/CroMarmot/oiTerminal
 Project-URL: Bug Tracker, https://github.com/CroMarmot/oiTerminal/issues
 Author-email: YeXiaoRain <yexiaorain@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 陈鼫RWHTYFZ
```

