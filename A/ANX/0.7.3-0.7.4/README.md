# Comparing `tmp/ANX-0.7.3.tar.gz` & `tmp/ANX-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANX-0.7.3.tar", last modified: Mon Apr  8 11:35:14 2024, max compression
+gzip compressed data, was "ANX-0.7.4.tar", last modified: Thu Apr 11 04:45:55 2024, max compression
```

## Comparing `ANX-0.7.3.tar` & `ANX-0.7.4.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.366819 ANX-0.7.3/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.336644 ANX-0.7.3/ANX.egg-info/
--rw-r--r--   0 1a         (501) staff       (20)      125 2024-04-08 11:35:14.000000 ANX-0.7.3/ANX.egg-info/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)     4882 2024-04-08 11:35:14.000000 ANX-0.7.3/ANX.egg-info/SOURCES.txt
--rw-r--r--   0 1a         (501) staff       (20)        1 2024-04-08 11:35:14.000000 ANX-0.7.3/ANX.egg-info/dependency_links.txt
--rw-r--r--   0 1a         (501) staff       (20)      108 2024-04-08 11:35:14.000000 ANX-0.7.3/ANX.egg-info/requires.txt
--rw-r--r--   0 1a         (501) staff       (20)       10 2024-04-08 11:35:14.000000 ANX-0.7.3/ANX.egg-info/top_level.txt
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.337351 ANX-0.7.3/AndroidQQ/
--rw-r--r--   0 1a         (501) staff       (20)    34763 2024-04-08 06:20:56.000000 ANX-0.7.3/AndroidQQ/Android.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.337700 ANX-0.7.3/AndroidQQ/Echo/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/Echo/Tcp.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/Echo/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     3878 2024-04-07 22:37:06.000000 ANX-0.7.3/AndroidQQ/Tcp.py
--rw-r--r--   0 1a         (501) staff       (20)       71 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.339696 ANX-0.7.3/AndroidQQ/http/
--rw-r--r--   0 1a         (501) staff       (20)     2195 2024-04-08 06:23:23.000000 ANX-0.7.3/AndroidQQ/http/ClientKey.py
--rw-r--r--   0 1a         (501) staff       (20)      138 2024-04-08 05:21:16.000000 ANX-0.7.3/AndroidQQ/http/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2009 2024-04-08 05:37:11.000000 ANX-0.7.3/AndroidQQ/http/accounts.py
--rw-r--r--   0 1a         (501) staff       (20)      820 2024-04-08 05:31:10.000000 ANX-0.7.3/AndroidQQ/http/cip.py
--rw-r--r--   0 1a         (501) staff       (20)     4061 2024-04-08 05:46:08.000000 ANX-0.7.3/AndroidQQ/http/friends.py
--rw-r--r--   0 1a         (501) staff       (20)     4697 2024-04-08 05:55:05.000000 ANX-0.7.3/AndroidQQ/http/game_credit.py
--rw-r--r--   0 1a         (501) staff       (20)      422 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/http/headers.py
--rw-r--r--   0 1a         (501) staff       (20)     7243 2024-04-08 05:40:22.000000 ANX-0.7.3/AndroidQQ/http/level.py
--rw-r--r--   0 1a         (501) staff       (20)    10305 2024-04-08 05:54:43.000000 ANX-0.7.3/AndroidQQ/http/music.py
--rw-r--r--   0 1a         (501) staff       (20)     1499 2024-04-08 05:42:12.000000 ANX-0.7.3/AndroidQQ/http/qqsignin.py
--rw-r--r--   0 1a         (501) staff       (20)     1325 2024-04-08 05:50:32.000000 ANX-0.7.3/AndroidQQ/http/weishi.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.339828 ANX-0.7.3/AndroidQQ/im/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.339914 ANX-0.7.3/AndroidQQ/im/oidb/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.340159 ANX-0.7.3/AndroidQQ/im/oidb/OidbSvc_0xc96/
--rw-r--r--   0 1a         (501) staff       (20)     2797 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)       34 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/OidbSvc_0xc96/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.341126 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x88d/
--rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x88d/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2139 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.341549 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x922/
--rw-r--r--   0 1a         (501) staff       (20)     1343 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x922/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1542 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.342045 ANX-0.7.3/AndroidQQ/im/oidb/cmd0xeb8/
--rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0xeb8/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1872 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.342511 ANX-0.7.3/AndroidQQ/im/oidb/oidb_0xc05/
--rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/oidb_0xc05/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2603 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.342963 ANX-0.7.3/AndroidQQ/im/oidb/oidb_sso/
--rw-r--r--   0 1a         (501) staff       (20)       27 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/oidb_sso/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1468 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.343402 ANX-0.7.3/AndroidQQ/im/oidb/qqconnect/
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/qqconnect/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2618 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.344059 ANX-0.7.3/AndroidQQ/im/oidb/scanlogin/
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/scanlogin/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1385 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.344385 ANX-0.7.3/AndroidQQ/log/
--rw-r--r--   0 1a         (501) staff       (20)       33 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/log/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.347595 ANX-0.7.3/AndroidQQ/pack/
--rw-r--r--   0 1a         (501) staff       (20)      395 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/Heartbeat_Alive.py
--rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py
--rw-r--r--   0 1a         (501) staff       (20)      733 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py
--rw-r--r--   0 1a         (501) staff       (20)     1368 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/OidbSvc_0x88d_1.py
--rw-r--r--   0 1a         (501) staff       (20)      986 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/OidbSvc_0xc05.py
--rw-r--r--   0 1a         (501) staff       (20)     1141 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/OidbSvc_0xc96.py
--rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/OidbSvc_0xeb8.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.348992 ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/
--rw-r--r--   0 1a         (501) staff       (20)       94 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1124 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/delUgc.py
--rw-r--r--   0 1a         (501) staff       (20)     2637 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/like.py
--rw-r--r--   0 1a         (501) staff       (20)     2631 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/publishmood.py
--rw-r--r--   0 1a         (501) staff       (20)     2152 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py
--rw-r--r--   0 1a         (501) staff       (20)     1116 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/StatSvc_register.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.349367 ANX-0.7.3/AndroidQQ/pack/SummaryCard/
--rw-r--r--   0 1a         (501) staff       (20)     1349 2024-03-07 10:14:41.000000 ANX-0.7.3/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/SummaryCard/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      402 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1383 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/friendlist.py
--rw-r--r--   0 1a         (501) staff       (20)      543 2024-03-06 13:46:02.000000 ANX-0.7.3/AndroidQQ/pack/test.py
--rw-r--r--   0 1a         (501) staff       (20)    46467 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.349963 ANX-0.7.3/AndroidQQ/proto/
--rw-r--r--   0 1a         (501) staff       (20)     4301 2024-02-12 04:07:38.000000 ANX-0.7.3/AndroidQQ/proto/IM_r_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)       67 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/proto/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1308 2023-10-29 17:25:21.000000 ANX-0.7.3/AndroidQQ/proto/wtlogin_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.352025 ANX-0.7.3/AndroidQQ/struct/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.352940 ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/
--rw-r--r--   0 1a         (501) staff       (20)      444 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/DestQQHeadInfo.py
--rw-r--r--   0 1a         (501) staff       (20)     1061 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      853 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py
--rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py
--rw-r--r--   0 1a         (501) staff       (20)     1028 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      894 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/MessageSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.353500 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_COMM/
--rw-r--r--   0 1a         (501) staff       (20)      373 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_COMM/UgcRightInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_COMM/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.356959 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/
--rw-r--r--   0 1a         (501) staff       (20)       70 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     3064 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py
--rw-r--r--   0 1a         (501) staff       (20)     1565 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py
--rw-r--r--   0 1a         (501) staff       (20)      565 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py
--rw-r--r--   0 1a         (501) staff       (20)      895 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py
--rw-r--r--   0 1a         (501) staff       (20)     1789 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)      451 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/s_arkshare.py
--rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py
--rw-r--r--   0 1a         (501) staff       (20)      728 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py
--rw-r--r--   0 1a         (501) staff       (20)      249 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/s_user.py
--rw-r--r--   0 1a         (501) staff       (20)     1163 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.359140 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/
--rw-r--r--   0 1a         (501) staff       (20)      479 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/Source.py
--rw-r--r--   0 1a         (501) staff       (20)      187 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      656 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py
--rw-r--r--   0 1a         (501) staff       (20)     1161 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py
--rw-r--r--   0 1a         (501) staff       (20)     1300 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py
--rw-r--r--   0 1a         (501) staff       (20)      560 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)     3031 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py
--rw-r--r--   0 1a         (501) staff       (20)      503 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)      594 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/OidbSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.361811 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/
--rw-r--r--   0 1a         (501) staff       (20)      504 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfBusiControl.py
--rw-r--r--   0 1a         (501) staff       (20)      630 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      714 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py
--rw-r--r--   0 1a         (501) staff       (20)      526 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py
--rw-r--r--   0 1a         (501) staff       (20)     1180 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py
--rw-r--r--   0 1a         (501) staff       (20)      489 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/RetryInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       87 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.362100 ANX-0.7.3/AndroidQQ/struct/QQService/
--rw-r--r--   0 1a         (501) staff       (20)     1112 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      878 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QQService/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1115 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/StatSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.362754 ANX-0.7.3/AndroidQQ/struct/SummaryCard/
--rw-r--r--   0 1a         (501) staff       (20)     2861 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py
--rw-r--r--   0 1a         (501) staff       (20)      493 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/SummaryCard/UserLocaleInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       61 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/SummaryCard/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)    15568 2024-03-05 18:40:23.000000 ANX-0.7.3/AndroidQQ/struct/Tlv.py
--rw-r--r--   0 1a         (501) staff       (20)     4784 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/Tlv_res.py
--rw-r--r--   0 1a         (501) staff       (20)      131 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.363479 ANX-0.7.3/AndroidQQ/struct/cooperation/
--rw-r--r--   0 1a         (501) staff       (20)       23 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/cooperation/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.363964 ANX-0.7.3/AndroidQQ/struct/cooperation/qzone/
--rw-r--r--   0 1a         (501) staff       (20)     4558 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/cooperation/qzone/WNSStream.py
--rw-r--r--   0 1a         (501) staff       (20)       26 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/cooperation/qzone/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.364217 ANX-0.7.3/AndroidQQ/struct/feedcomponent/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/feedcomponent/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1482 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/feedcomponent/model.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.364605 ANX-0.7.3/AndroidQQ/struct/friendlist/
--rw-r--r--   0 1a         (501) staff       (20)     2842 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/friendlist/AddFriendReq.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/friendlist/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     7428 2024-03-07 10:14:48.000000 ANX-0.7.3/AndroidQQ/struct/head.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.365079 ANX-0.7.3/AndroidQQ/struct/push/
--rw-r--r--   0 1a         (501) staff       (20)     3536 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/push/SvcReqRegister.py
--rw-r--r--   0 1a         (501) staff       (20)     2084 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/push/SvcRespRegister.py
--rw-r--r--   0 1a         (501) staff       (20)       31 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/push/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)    27313 2024-03-05 18:40:23.000000 ANX-0.7.3/AndroidQQ/struct/wtlogin.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.365872 ANX-0.7.3/AndroidQQ/utils/
--rw-r--r--   0 1a         (501) staff       (20)       20 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/utils/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      523 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/utils/build_device.py
--rw-r--r--   0 1a         (501) staff       (20)     1140 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/utils/ecdh.py
--rw-r--r--   0 1a         (501) staff       (20)     1379 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/utils/sso_server.py
--rw-r--r--   0 1a         (501) staff       (20)      735 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/utils/tool.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.366014 ANX-0.7.3/AndroidQQ/wlogin_sdk/
--rw-r--r--   0 1a         (501) staff       (20)       25 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/wlogin_sdk/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.366275 ANX-0.7.3/AndroidQQ/wlogin_sdk/request/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/wlogin_sdk/request/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      125 2024-04-08 11:35:14.366469 ANX-0.7.3/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)       34 2023-08-04 12:41:32.000000 ANX-0.7.3/README.md
--rw-r--r--   0 1a         (501) staff       (20)       38 2024-04-08 11:35:14.366889 ANX-0.7.3/setup.cfg
--rw-r--r--   0 1a         (501) staff       (20)      601 2024-04-08 11:35:10.000000 ANX-0.7.3/setup.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.298936 ANX-0.7.4/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.266043 ANX-0.7.4/ANX.egg-info/
+-rw-r--r--   0 1a         (501) staff       (20)      125 2024-04-11 04:45:55.000000 ANX-0.7.4/ANX.egg-info/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)     4882 2024-04-11 04:45:55.000000 ANX-0.7.4/ANX.egg-info/SOURCES.txt
+-rw-r--r--   0 1a         (501) staff       (20)        1 2024-04-11 04:45:55.000000 ANX-0.7.4/ANX.egg-info/dependency_links.txt
+-rw-r--r--   0 1a         (501) staff       (20)      108 2024-04-11 04:45:55.000000 ANX-0.7.4/ANX.egg-info/requires.txt
+-rw-r--r--   0 1a         (501) staff       (20)       10 2024-04-11 04:45:55.000000 ANX-0.7.4/ANX.egg-info/top_level.txt
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.266646 ANX-0.7.4/AndroidQQ/
+-rw-r--r--   0 1a         (501) staff       (20)    34763 2024-04-08 06:20:56.000000 ANX-0.7.4/AndroidQQ/Android.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.266975 ANX-0.7.4/AndroidQQ/Echo/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/Echo/Tcp.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/Echo/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     3878 2024-04-07 22:37:06.000000 ANX-0.7.4/AndroidQQ/Tcp.py
+-rw-r--r--   0 1a         (501) staff       (20)       71 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.269275 ANX-0.7.4/AndroidQQ/http/
+-rw-r--r--   0 1a         (501) staff       (20)     2195 2024-04-08 06:23:23.000000 ANX-0.7.4/AndroidQQ/http/ClientKey.py
+-rw-r--r--   0 1a         (501) staff       (20)      138 2024-04-08 05:21:16.000000 ANX-0.7.4/AndroidQQ/http/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2009 2024-04-08 05:37:11.000000 ANX-0.7.4/AndroidQQ/http/accounts.py
+-rw-r--r--   0 1a         (501) staff       (20)      820 2024-04-08 05:31:10.000000 ANX-0.7.4/AndroidQQ/http/cip.py
+-rw-r--r--   0 1a         (501) staff       (20)     4061 2024-04-08 05:46:08.000000 ANX-0.7.4/AndroidQQ/http/friends.py
+-rw-r--r--   0 1a         (501) staff       (20)     4770 2024-04-11 04:44:24.000000 ANX-0.7.4/AndroidQQ/http/game_credit.py
+-rw-r--r--   0 1a         (501) staff       (20)      422 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/http/headers.py
+-rw-r--r--   0 1a         (501) staff       (20)     7243 2024-04-08 05:40:22.000000 ANX-0.7.4/AndroidQQ/http/level.py
+-rw-r--r--   0 1a         (501) staff       (20)    10306 2024-04-11 04:45:28.000000 ANX-0.7.4/AndroidQQ/http/music.py
+-rw-r--r--   0 1a         (501) staff       (20)     1499 2024-04-08 05:42:12.000000 ANX-0.7.4/AndroidQQ/http/qqsignin.py
+-rw-r--r--   0 1a         (501) staff       (20)     1325 2024-04-08 05:50:32.000000 ANX-0.7.4/AndroidQQ/http/weishi.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.269402 ANX-0.7.4/AndroidQQ/im/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.269502 ANX-0.7.4/AndroidQQ/im/oidb/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.269889 ANX-0.7.4/AndroidQQ/im/oidb/OidbSvc_0xc96/
+-rw-r--r--   0 1a         (501) staff       (20)     2797 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)       34 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/OidbSvc_0xc96/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.270473 ANX-0.7.4/AndroidQQ/im/oidb/cmd0x88d/
+-rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/cmd0x88d/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2139 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.271432 ANX-0.7.4/AndroidQQ/im/oidb/cmd0x922/
+-rw-r--r--   0 1a         (501) staff       (20)     1343 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/cmd0x922/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1542 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.271881 ANX-0.7.4/AndroidQQ/im/oidb/cmd0xeb8/
+-rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/cmd0xeb8/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1872 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.272310 ANX-0.7.4/AndroidQQ/im/oidb/oidb_0xc05/
+-rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/oidb_0xc05/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2603 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.272769 ANX-0.7.4/AndroidQQ/im/oidb/oidb_sso/
+-rw-r--r--   0 1a         (501) staff       (20)       27 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/oidb_sso/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1468 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.273241 ANX-0.7.4/AndroidQQ/im/oidb/qqconnect/
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/qqconnect/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2618 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.274136 ANX-0.7.4/AndroidQQ/im/oidb/scanlogin/
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/scanlogin/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1385 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.274397 ANX-0.7.4/AndroidQQ/log/
+-rw-r--r--   0 1a         (501) staff       (20)       33 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/log/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.277864 ANX-0.7.4/AndroidQQ/pack/
+-rw-r--r--   0 1a         (501) staff       (20)      395 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/Heartbeat_Alive.py
+-rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py
+-rw-r--r--   0 1a         (501) staff       (20)      733 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py
+-rw-r--r--   0 1a         (501) staff       (20)     1368 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/OidbSvc_0x88d_1.py
+-rw-r--r--   0 1a         (501) staff       (20)      986 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/OidbSvc_0xc05.py
+-rw-r--r--   0 1a         (501) staff       (20)     1141 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/OidbSvc_0xc96.py
+-rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/OidbSvc_0xeb8.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.279229 ANX-0.7.4/AndroidQQ/pack/SQQzoneSvc/
+-rw-r--r--   0 1a         (501) staff       (20)       94 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/SQQzoneSvc/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1124 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/SQQzoneSvc/delUgc.py
+-rw-r--r--   0 1a         (501) staff       (20)     2637 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/SQQzoneSvc/like.py
+-rw-r--r--   0 1a         (501) staff       (20)     2631 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/SQQzoneSvc/publishmood.py
+-rw-r--r--   0 1a         (501) staff       (20)     2152 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1116 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/StatSvc_register.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.279686 ANX-0.7.4/AndroidQQ/pack/SummaryCard/
+-rw-r--r--   0 1a         (501) staff       (20)     1349 2024-03-07 10:14:41.000000 ANX-0.7.4/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/SummaryCard/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      402 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1383 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/friendlist.py
+-rw-r--r--   0 1a         (501) staff       (20)      543 2024-03-06 13:46:02.000000 ANX-0.7.4/AndroidQQ/pack/test.py
+-rw-r--r--   0 1a         (501) staff       (20)    46467 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.280387 ANX-0.7.4/AndroidQQ/proto/
+-rw-r--r--   0 1a         (501) staff       (20)     4301 2024-02-12 04:07:38.000000 ANX-0.7.4/AndroidQQ/proto/IM_r_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)       67 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/proto/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1308 2023-10-29 17:25:21.000000 ANX-0.7.4/AndroidQQ/proto/wtlogin_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.282729 ANX-0.7.4/AndroidQQ/struct/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.283757 ANX-0.7.4/AndroidQQ/struct/Avatarlnfo/
+-rw-r--r--   0 1a         (501) staff       (20)      444 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/Avatarlnfo/DestQQHeadInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1061 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      853 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py
+-rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py
+-rw-r--r--   0 1a         (501) staff       (20)     1028 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/Avatarlnfo/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      894 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/MessageSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.284305 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_COMM/
+-rw-r--r--   0 1a         (501) staff       (20)      373 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_COMM/UgcRightInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_COMM/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.288251 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/
+-rw-r--r--   0 1a         (501) staff       (20)       70 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     3064 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py
+-rw-r--r--   0 1a         (501) staff       (20)     1565 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py
+-rw-r--r--   0 1a         (501) staff       (20)      565 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      895 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py
+-rw-r--r--   0 1a         (501) staff       (20)     1789 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)      451 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/s_arkshare.py
+-rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py
+-rw-r--r--   0 1a         (501) staff       (20)      728 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py
+-rw-r--r--   0 1a         (501) staff       (20)      249 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/s_user.py
+-rw-r--r--   0 1a         (501) staff       (20)     1163 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.291203 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/
+-rw-r--r--   0 1a         (501) staff       (20)      479 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/Source.py
+-rw-r--r--   0 1a         (501) staff       (20)      187 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      656 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py
+-rw-r--r--   0 1a         (501) staff       (20)     1161 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py
+-rw-r--r--   0 1a         (501) staff       (20)     1300 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py
+-rw-r--r--   0 1a         (501) staff       (20)      560 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)     3031 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py
+-rw-r--r--   0 1a         (501) staff       (20)      503 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)      594 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/OidbSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.294211 ANX-0.7.4/AndroidQQ/struct/QMF_PROTOCAL/
+-rw-r--r--   0 1a         (501) staff       (20)      504 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/QMF_PROTOCAL/QmfBusiControl.py
+-rw-r--r--   0 1a         (501) staff       (20)      630 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      714 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py
+-rw-r--r--   0 1a         (501) staff       (20)      526 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1180 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py
+-rw-r--r--   0 1a         (501) staff       (20)      489 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/QMF_PROTOCAL/RetryInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       87 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/QMF_PROTOCAL/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.294570 ANX-0.7.4/AndroidQQ/struct/QQService/
+-rw-r--r--   0 1a         (501) staff       (20)     1112 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      878 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/QQService/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1115 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/StatSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.295292 ANX-0.7.4/AndroidQQ/struct/SummaryCard/
+-rw-r--r--   0 1a         (501) staff       (20)     2861 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py
+-rw-r--r--   0 1a         (501) staff       (20)      493 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/SummaryCard/UserLocaleInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       61 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/SummaryCard/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)    15568 2024-03-05 18:40:23.000000 ANX-0.7.4/AndroidQQ/struct/Tlv.py
+-rw-r--r--   0 1a         (501) staff       (20)     4784 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/Tlv_res.py
+-rw-r--r--   0 1a         (501) staff       (20)      131 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.296004 ANX-0.7.4/AndroidQQ/struct/cooperation/
+-rw-r--r--   0 1a         (501) staff       (20)       23 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/cooperation/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.296565 ANX-0.7.4/AndroidQQ/struct/cooperation/qzone/
+-rw-r--r--   0 1a         (501) staff       (20)     4558 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/cooperation/qzone/WNSStream.py
+-rw-r--r--   0 1a         (501) staff       (20)       26 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/cooperation/qzone/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.296807 ANX-0.7.4/AndroidQQ/struct/feedcomponent/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/feedcomponent/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1482 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/feedcomponent/model.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.297081 ANX-0.7.4/AndroidQQ/struct/friendlist/
+-rw-r--r--   0 1a         (501) staff       (20)     2842 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/friendlist/AddFriendReq.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/friendlist/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     7428 2024-03-07 10:14:48.000000 ANX-0.7.4/AndroidQQ/struct/head.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.297459 ANX-0.7.4/AndroidQQ/struct/push/
+-rw-r--r--   0 1a         (501) staff       (20)     3536 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/push/SvcReqRegister.py
+-rw-r--r--   0 1a         (501) staff       (20)     2084 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/push/SvcRespRegister.py
+-rw-r--r--   0 1a         (501) staff       (20)       31 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/struct/push/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)    27313 2024-03-05 18:40:23.000000 ANX-0.7.4/AndroidQQ/struct/wtlogin.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.298346 ANX-0.7.4/AndroidQQ/utils/
+-rw-r--r--   0 1a         (501) staff       (20)       20 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/utils/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      523 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/utils/build_device.py
+-rw-r--r--   0 1a         (501) staff       (20)     1140 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/utils/ecdh.py
+-rw-r--r--   0 1a         (501) staff       (20)     1379 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/utils/sso_server.py
+-rw-r--r--   0 1a         (501) staff       (20)      735 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/utils/tool.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.298495 ANX-0.7.4/AndroidQQ/wlogin_sdk/
+-rw-r--r--   0 1a         (501) staff       (20)       25 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/wlogin_sdk/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-11 04:45:55.298642 ANX-0.7.4/AndroidQQ/wlogin_sdk/request/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.4/AndroidQQ/wlogin_sdk/request/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      125 2024-04-11 04:45:55.298802 ANX-0.7.4/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)       34 2023-08-04 12:41:32.000000 ANX-0.7.4/README.md
+-rw-r--r--   0 1a         (501) staff       (20)       38 2024-04-11 04:45:55.298994 ANX-0.7.4/setup.cfg
+-rw-r--r--   0 1a         (501) staff       (20)      601 2024-04-11 04:45:49.000000 ANX-0.7.4/setup.py
```

### Comparing `ANX-0.7.3/ANX.egg-info/SOURCES.txt` & `ANX-0.7.4/ANX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/Android.py` & `ANX-0.7.4/AndroidQQ/Android.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/Tcp.py` & `ANX-0.7.4/AndroidQQ/Tcp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/http/ClientKey.py` & `ANX-0.7.4/AndroidQQ/http/ClientKey.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/http/accounts.py` & `ANX-0.7.4/AndroidQQ/http/accounts.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/http/cip.py` & `ANX-0.7.4/AndroidQQ/http/cip.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/http/friends.py` & `ANX-0.7.4/AndroidQQ/http/friends.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/http/game_credit.py` & `ANX-0.7.4/AndroidQQ/http/game_credit.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     def __init__(self, info, clientkey):
         # self.uin = '3484129139'
         # self.clientkey = '9f2677a5c3c9dd3571f4c14c3a796f06cd54ade8e7983f68b2e8bdb557e65eabc849b9b87cf8a6ed69f2a3e4b99d2dde'
         #
         self.gs_code = None
         self.uin = info.uin
         self.clientkey = clientkey
-        self.get_gs_code()
         self.info = info
+        self.get_gs_code()
 
     def get_gs_code(self):
         try:
             response = requests.get(url="https://ssl.ptlogin2.qq.com/jump",
                                     params={
                                         "keyindex": "19",
                                         "clientuin": self.uin,
@@ -34,16 +34,18 @@
                                         "pt_ua": "B0BFB00844CA89BF32B35D60533238A2",
                                         "pt_browser": "Chrome",
                                         "pt_3rd_aid": "102053620",
                                         "pt_openlogin_data": f"appid=716027609&pt_3rd_aid=102053620&daid=383&pt_skey_valid=0&style=35&s_url=https%3A%2F%2Fconnect.qq.com&refer_cgi=authorize&which=&sdkp=pcweb&sdkv=v1.0&time={str(int(time.time()))}&loginty=3&h5sig=G_tqev5eSttaANNnVgcw5gCN25vuzK7ef9fUPcYGmUY&state=qqconnect_1&client_id=102053620&response_type=code&scope=all&redirect_uri=https%3A%2F%2Fgamecredit.qq.com%2Flogin-ui%2Findex.html%3FcPageName%3Dmiddle%26type%3DQQ%26backUrl%3Dreload%26appId%3D102053620&pt_flex=1&loginfrom=&h5sig=G_tqev5eSttaANNnVgcw5gCN25vuzK7ef9fUPcYGmUY&loginty=3&",
                                     }
                                     ,
                                     allow_redirects=False,
-                                    proxies=self.info.proxy_proxies)
+                                    proxies=self.info.proxy_proxies
+                                    )
             Location = response.headers['Location']
+            print(response.headers)
 
             if Location is None:
                 return {'status': False, 'message': '没找到Location'}
             parsed_url = urlparse(Location)
             query_params = parse_qs(parsed_url.query)
             code = query_params.get('code')[0]
             response = requests.get(url=f'https://gamecredit.qq.com/connect?code={code}&appId=102053620&atype=QQ',
```

### Comparing `ANX-0.7.3/AndroidQQ/http/level.py` & `ANX-0.7.4/AndroidQQ/http/level.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/http/music.py` & `ANX-0.7.4/AndroidQQ/http/music.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,22 +44,23 @@
     t2 = ''.join(ls3).replace("/", "")
     sign = "zzb" + (t1 + t2 + t3).lower()
     return sign
 
 
 class Music:
     def __init__(self, info):
+        self.info = info
+
         self.qm_keyst = None
         self.cookies = None
         self.uin = info.uin
         self.client_key = info.cookies.client_key
         self.code = None
         self.g_tk = None
         self.psrf_qqopenid = None
-        self.info = info
 
     def get_Location_code(self):
         if not self.client_key:
             return {'status': False, 'message': '没有获取到clientkey'}
         try:
             response = requests.get(url="https://ssl.ptlogin2.qq.com/jump",
                                     params={
```

### Comparing `ANX-0.7.3/AndroidQQ/http/qqsignin.py` & `ANX-0.7.4/AndroidQQ/http/qqsignin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/http/weishi.py` & `ANX-0.7.4/AndroidQQ/http/weishi.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py` & `ANX-0.7.4/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py` & `ANX-0.7.4/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py` & `ANX-0.7.4/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py` & `ANX-0.7.4/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py` & `ANX-0.7.4/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py` & `ANX-0.7.4/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py` & `ANX-0.7.4/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py` & `ANX-0.7.4/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py` & `ANX-0.7.4/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py` & `ANX-0.7.4/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py` & `ANX-0.7.4/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/OidbSvc_0x88d_1.py` & `ANX-0.7.4/AndroidQQ/pack/OidbSvc_0x88d_1.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/OidbSvc_0xc05.py` & `ANX-0.7.4/AndroidQQ/pack/OidbSvc_0xc05.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/OidbSvc_0xc96.py` & `ANX-0.7.4/AndroidQQ/pack/OidbSvc_0xc96.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/OidbSvc_0xeb8.py` & `ANX-0.7.4/AndroidQQ/pack/OidbSvc_0xeb8.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/delUgc.py` & `ANX-0.7.4/AndroidQQ/pack/SQQzoneSvc/delUgc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/like.py` & `ANX-0.7.4/AndroidQQ/pack/SQQzoneSvc/like.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/publishmood.py` & `ANX-0.7.4/AndroidQQ/pack/SQQzoneSvc/publishmood.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py` & `ANX-0.7.4/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/StatSvc_register.py` & `ANX-0.7.4/AndroidQQ/pack/StatSvc_register.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py` & `ANX-0.7.4/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/friendlist.py` & `ANX-0.7.4/AndroidQQ/pack/friendlist.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/test.py` & `ANX-0.7.4/AndroidQQ/pack/test.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py` & `ANX-0.7.4/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/proto/IM_r_pb2.py` & `ANX-0.7.4/AndroidQQ/proto/IM_r_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/proto/wtlogin_pb2.py` & `ANX-0.7.4/AndroidQQ/proto/wtlogin_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py` & `ANX-0.7.4/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py` & `ANX-0.7.4/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py` & `ANX-0.7.4/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/__init__.py` & `ANX-0.7.4/AndroidQQ/struct/Avatarlnfo/__init__.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/MessageSvc.py` & `ANX-0.7.4/AndroidQQ/struct/MessageSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py` & `ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py` & `ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py` & `ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py` & `ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py` & `ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py` & `ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py` & `ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py` & `ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py` & `ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py` & `ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py` & `ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py` & `ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py` & `ANX-0.7.4/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/OidbSvc.py` & `ANX-0.7.4/AndroidQQ/struct/OidbSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py` & `ANX-0.7.4/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py` & `ANX-0.7.4/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py` & `ANX-0.7.4/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py` & `ANX-0.7.4/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py` & `ANX-0.7.4/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/QQService/__init__.py` & `ANX-0.7.4/AndroidQQ/struct/QQService/__init__.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/StatSvc.py` & `ANX-0.7.4/AndroidQQ/struct/StatSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py` & `ANX-0.7.4/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/Tlv.py` & `ANX-0.7.4/AndroidQQ/struct/Tlv.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/Tlv_res.py` & `ANX-0.7.4/AndroidQQ/struct/Tlv_res.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/cooperation/qzone/WNSStream.py` & `ANX-0.7.4/AndroidQQ/struct/cooperation/qzone/WNSStream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/feedcomponent/model.py` & `ANX-0.7.4/AndroidQQ/struct/feedcomponent/model.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/friendlist/AddFriendReq.py` & `ANX-0.7.4/AndroidQQ/struct/friendlist/AddFriendReq.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/head.py` & `ANX-0.7.4/AndroidQQ/struct/head.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/push/SvcReqRegister.py` & `ANX-0.7.4/AndroidQQ/struct/push/SvcReqRegister.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/push/SvcRespRegister.py` & `ANX-0.7.4/AndroidQQ/struct/push/SvcRespRegister.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/struct/wtlogin.py` & `ANX-0.7.4/AndroidQQ/struct/wtlogin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/utils/build_device.py` & `ANX-0.7.4/AndroidQQ/utils/build_device.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/utils/ecdh.py` & `ANX-0.7.4/AndroidQQ/utils/ecdh.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/utils/sso_server.py` & `ANX-0.7.4/AndroidQQ/utils/sso_server.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/AndroidQQ/utils/tool.py` & `ANX-0.7.4/AndroidQQ/utils/tool.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.3/setup.py` & `ANX-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 setuptools.setup(
     name='ANX',
-    version='0.7.3',
+    version='0.7.4',
     url='https://github.com/grayrail000/AndroidQQ',
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
     license='',
     author='1x',
     author_email='',
     description='',
     install_requires=[
```

