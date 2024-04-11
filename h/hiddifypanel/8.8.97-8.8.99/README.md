# Comparing `tmp/hiddifypanel-8.8.97.tar.gz` & `tmp/hiddifypanel-8.8.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiddifypanel-8.8.97.tar", last modified: Fri Feb 23 11:41:31 2024, max compression
+gzip compressed data, was "hiddifypanel-8.8.99.tar", last modified: Sat Mar  2 13:10:18 2024, max compression
```

## Comparing `hiddifypanel-8.8.97.tar` & `hiddifypanel-8.8.99.tar`

### file list

```diff
@@ -1,832 +1,832 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.845200 hiddifypanel-8.8.97/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    42639 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)    19807 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-02-23 11:41:31.845200 hiddifypanel-8.8.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.701201 hiddifypanel-8.8.97/hiddifypanel/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/Events.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.701201 hiddifypanel-8.8.97/hiddifypanel/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/drivers/abstract_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/drivers/singbox_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/drivers/ssh_liberty_bridge_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/drivers/user_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/drivers/xray_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.705201 hiddifypanel-8.8.97/hiddifypanel/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/models/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/models/child.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/models/config_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/models/parent_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/models/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/models/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/models/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.705201 hiddifypanel-8.8.97/hiddifypanel/panel/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.709201 hiddifypanel-8.8.97/hiddifypanel/panel/admin/
--rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/Actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/AdminstratorAdmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/Backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/ChildAdmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/ConfigAdmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/Dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/DomainAdmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/ProxyAdmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/QuickSetup.py
--rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/SettingAdmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/Terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/UserAdmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/adminlte.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/commercial_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.709201 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/a.html
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/backup.html
--rw-r--r--   0 runner    (1001) docker     (127)    14994 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/base2.html
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/commercial_info.html
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/config.html
--rw-r--r--   0 runner    (1001) docker     (127)    10613 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/configfake.html
--rw-r--r--   0 runner    (1001) docker     (127)    13299 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/ltemaster.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.713201 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/model/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/model/admin_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/model/domain_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/model/user_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/parent_dash.html
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/proxy.html
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/quick_setup.html
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/result.html
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/admin_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/cf_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/clean_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.713201 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/ParentDomainAdmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/ProxyDetailsAdmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.713201 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/restapi/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/restapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/restapi/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/restapi/tgbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/restapi/tgmsg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.713201 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/telegrambot/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/telegrambot/DefaultResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/telegrambot/Usage.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/telegrambot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/telegrambot/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/telegrambot/information.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.713201 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/templates/configc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/commercial/templates/parent_dash.html
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/custom_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    31850 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/hiddify.py
--rw-r--r--   0 runner    (1001) docker     (127)    18746 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/init_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.713201 hiddifypanel-8.8.97/hiddifypanel/panel/user/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/link_maker.html
--rw-r--r--   0 runner    (1001) docker     (127)    30453 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/link_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.717201 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/all_configs copy.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/all_configs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/base_singbox_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/clash_config copy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/clash_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/clash_proxies copy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/clash_proxies.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.721201 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/all-configs.html
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/all-configs_old.html
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/android.html
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/auto_page.html
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/base2.html
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/clash-links copy.html
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/clash-links.html
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/doh.html
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/handle_smart.html
--rw-r--r--   0 runner    (1001) docker     (127)    12889 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/home.html
--rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/index copy.html
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/index_old.html
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/ios copy.html
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/ios.html
--rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/multi.html
--rw-r--r--   0 runner    (1001) docker     (127)    17154 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/one_click.html
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/speedtest.html
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/telegram.html
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/usage.html
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/windows.html
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/singbox_config.json
--rw-r--r--   0 runner    (1001) docker     (127)    15138 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/panel/user/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.721201 hiddifypanel-8.8.97/hiddifypanel/static/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/a.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.725201 hiddifypanel-8.8.97/hiddifypanel/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)  1665614 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/css/adminlte.css
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/css/adminlte.fa.css
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/css/adminlte.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   155845 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/css/bootstrap4-rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   163995 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/css/bootstrap5.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/css/custom-rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)   101895 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (127)   278568 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/css/lte.old
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.729201 hiddifypanel-8.8.97/hiddifypanel/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    92934 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Black.eot
--rw-r--r--   0 runner    (1001) docker     (127)    92764 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    53500 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Black.woff
--rw-r--r--   0 runner    (1001) docker     (127)    42308 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Black.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    91810 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Bold.eot
--rw-r--r--   0 runner    (1001) docker     (127)    91644 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    52676 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    41856 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   101090 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Light.eot
--rw-r--r--   0 runner    (1001) docker     (127)   100920 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    59988 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Light.woff
--rw-r--r--   0 runner    (1001) docker     (127)    48616 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Light.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   107842 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Medium.eot
--rw-r--r--   0 runner    (1001) docker     (127)   107668 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    63312 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Medium.woff
--rw-r--r--   0 runner    (1001) docker     (127)    51256 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    90482 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Thin.eot
--rw-r--r--   0 runner    (1001) docker     (127)    90316 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    51884 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Thin.woff
--rw-r--r--   0 runner    (1001) docker     (127)    41344 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Thin.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    85354 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir.eot
--rw-r--r--   0 runner    (1001) docker     (127)    85192 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    47972 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir.woff
--rw-r--r--   0 runner    (1001) docker     (127)    38004 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.733201 hiddifypanel-8.8.97/hiddifypanel/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/WhiteLogo.png
--rw-r--r--   0 runner    (1001) docker     (127)   103814 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   111125 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/hiddify-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    37408 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/hiddify.png
--rw-r--r--   0 runner    (1001) docker     (127)     8441 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/no_back_hiddify.png
--rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/pwa-icon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.733201 hiddifypanel-8.8.97/hiddifypanel/static/images/splash/
--rw-r--r--   0 runner    (1001) docker     (127)    75224 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/splash/ipad_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    85623 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/splash/ipadpro1_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)   121021 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/splash/ipadpro2_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    90886 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/splash/ipadpro3_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    28231 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/splash/iphone5_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    34920 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/splash/iphone6_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    68643 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/splash/iphoneplus_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    69743 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/splash/iphonex_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    45109 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/splash/iphonexr_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    80648 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/images/splash/iphonexsmax_splash.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.737201 hiddifypanel-8.8.97/hiddifypanel/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)   104260 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/adminlte.js
--rw-r--r--   0 runner    (1001) docker     (127)    49278 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/bootbox.all.js
--rw-r--r--   0 runner    (1001) docker     (127)    19021 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/bootbox.all.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    78743 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    60406 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/custom-protocol-check.js
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/custom-rtl.js
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/custom.js
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/demo.js
--rw-r--r--   0 runner    (1001) docker     (127)    89764 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/jquery-3.6.1.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/js.cookie.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    51465 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/moment.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19032 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/pwa-sw.js
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/pwa.js
--rw-r--r--   0 runner    (1001) docker     (127)    33168 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/js/qrcode.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.697201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.685201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.741201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (127)    37644 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (127)    28977 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   172839 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   140421 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.741201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (127)   210612 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)    70808 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   122441 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)    58072 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.737201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-slider/
--rw-r--r--   0 runner    (1001) docker     (127)    36164 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-slider/bootstrap-slider.js
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-slider/slider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.741201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-wysihtml5/
--rw-r--r--   0 runner    (1001) docker     (127)   566620 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js
--rw-r--r--   0 runner    (1001) docker     (127)   210932 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.685201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap4-editable/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.741201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap4-editable/css/
--rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap4-editable/css/bootstrap-editable.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.741201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap4-editable/img/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap4-editable/img/clear.png
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap4-editable/img/loading.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.741201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap4-editable/js/
--rw-r--r--   0 runner    (1001) docker     (127)   225176 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.js
--rw-r--r--   0 runner    (1001) docker     (127)    76077 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.745201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/chart.js/
--rw-r--r--   0 runner    (1001) docker     (127)   535484 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/chart.js/Chart.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   211133 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/chart.js/Chart.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   403941 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/chart.js/Chart.js
--rw-r--r--   0 runner    (1001) docker     (127)   159638 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/chart.js/Chart.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.745201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/chartjs-old/
--rw-r--r--   0 runner    (1001) docker     (127)   109613 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/chartjs-old/Chart.js
--rw-r--r--   0 runner    (1001) docker     (127)    52092 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/chartjs-old/Chart.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.745201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/
--rw-r--r--   0 runner    (1001) docker     (127)   433051 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/ckeditor.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.753201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ar.js
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ast.js
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/bg.js
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/cs.js
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/da.js
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/de.js
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/el.js
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/en-au.js
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/eo.js
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/es.js
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/et.js
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/eu.js
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/fi.js
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/fr.js
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/gl.js
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/gu.js
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/hr.js
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/hu.js
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/it.js
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ja.js
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/km.js
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/kn.js
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ko.js
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ku.js
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/nb.js
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ne.js
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/nl.js
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/oc.js
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/pl.js
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/pt-br.js
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/pt.js
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ro.js
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ru.js
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/si.js
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/sk.js
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/sq.js
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/sv.js
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/tr.js
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/tt.js
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ug.js
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/uk.js
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/zh-cn.js
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/zh.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.753201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.css
--rw-r--r--   0 runner    (1001) docker     (127)    33831 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.js
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.757201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/img/
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/img/alpha-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/img/alpha.png
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/img/hue-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/img/hue.png
--rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/img/saturation.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.757201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.css
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.689201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.757201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/Readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.757201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/dataTables.autoFill.css
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/dataTables.autoFill.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.757201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/filler.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.757201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/
--rw-r--r--   0 runner    (1001) docker     (127)    22645 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.js
--rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.757201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/License.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.757201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/dataTables.colReorder.css
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/dataTables.colReorder.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.757201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/insert.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.757201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/
--rw-r--r--   0 runner    (1001) docker     (127)    36311 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.js
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.761201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/License.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.761201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.css
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colvis.jqueryui.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.761201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/
--rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.js
--rw-r--r--   0 runner    (1001) docker     (127)    10109 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.761201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/License.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.761201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.css
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.761201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/
--rw-r--r--   0 runner    (1001) docker     (127)    40932 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.js
--rw-r--r--   0 runner    (1001) docker     (127)    14108 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.761201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/Readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.761201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/dataTables.fixedHeader.css
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/dataTables.fixedHeader.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.761201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/
--rw-r--r--   0 runner    (1001) docker     (127)    29308 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.js
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.761201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/KeyTable/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/KeyTable/Readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.761201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/dataTables.keyTable.css
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/dataTables.keyTable.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.765201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/
--rw-r--r--   0 runner    (1001) docker     (127)    29477 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.js
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.765201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/License.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.765201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.css
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/responsive.bootstrap4.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.765201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/
--rw-r--r--   0 runner    (1001) docker     (127)    25098 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.js
--rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/responsive.bootstrap4.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.765201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/Readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.765201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.css
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.765201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/loading-background.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.765201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/
--rw-r--r--   0 runner    (1001) docker     (127)    37984 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.js
--rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.765201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.765201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.css
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.769201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection.png
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy.png
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv.png
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf.png
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print.png
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls.png
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls_hover.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.769201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/
--rw-r--r--   0 runner    (1001) docker     (127)    84578 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.js
--rw-r--r--   0 runner    (1001) docker     (127)    31850 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.769201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls.swf
--rw-r--r--   0 runner    (1001) docker     (127)    58846 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls_pdf.swf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.769201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/images/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/images/sort_asc.png
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/images/sort_asc_disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/images/sort_both.png
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/images/sort_desc.png
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/images/sort_desc_disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)    15369 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/jquery.dataTables.css
--rw-r--r--   0 runner    (1001) docker     (127)    86551 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/jquery.dataTables.js
--rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    86551 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    14229 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/jquery.dataTables_themeroller.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.769201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/
--rw-r--r--   0 runner    (1001) docker     (127)    46838 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/bootstrap-datepicker.js
--rw-r--r--   0 runner    (1001) docker     (127)    33745 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/datepicker3.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.777201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ar.js
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.az.js
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.bg.js
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ca.js
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cs.js
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cy.js
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.da.js
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.de.js
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.el.js
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.es.js
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.et.js
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fa.js
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fi.js
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fr.js
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.gl.js
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.he.js
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hr.js
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hu.js
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.id.js
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.is.js
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.it.js
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ja.js
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ka.js
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kk.js
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kr.js
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lt.js
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lv.js
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.mk.js
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ms.js
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nb.js
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl-BE.js
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl.js
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.no.js
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pl.js
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt.js
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ro.js
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs-latin.js
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs.js
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ru.js
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sk.js
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sl.js
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sq.js
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sv.js
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sw.js
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.th.js
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.tr.js
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ua.js
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.vi.js
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-CN.js
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-TW.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.781201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/daterangepicker/
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/daterangepicker/daterangepicker-bs3.css
--rw-r--r--   0 runner    (1001) docker     (127)    53679 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/daterangepicker/daterangepicker.js
--rw-r--r--   0 runner    (1001) docker     (127)    99201 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/daterangepicker/moment.js
--rw-r--r--   0 runner    (1001) docker     (127)    34737 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/daterangepicker/moment.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.781201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/fastclick/
--rw-r--r--   0 runner    (1001) docker     (127)    25965 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/fastclick/fastclick.js
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/fastclick/fastclick.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.785201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/
--rw-r--r--   0 runner    (1001) docker     (127)    41944 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/excanvas.js
--rw-r--r--   0 runner    (1001) docker     (127)    19314 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/excanvas.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.colorhelpers.js
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.colorhelpers.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.canvas.js
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.categories.js
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.categories.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.js
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.js
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.js
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.image.js
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.image.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   121627 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.js
--rw-r--r--   0 runner    (1001) docker     (127)    52300 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    14190 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.navigate.js
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.navigate.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    23635 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.pie.js
--rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.pie.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.resize.js
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.resize.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.selection.js
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.selection.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.stack.js
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.stack.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.symbol.js
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.symbol.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.threshold.js
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.threshold.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.time.js
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.time.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.693201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.785201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/css/
--rw-r--r--   0 runner    (1001) docker     (127)    37414 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (127)    21778 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.789201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   134808 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.789201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/fullcalendar/
--rw-r--r--   0 runner    (1001) docker     (127)    22515 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/fullcalendar/fullcalendar.css
--rw-r--r--   0 runner    (1001) docker     (127)   279259 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/fullcalendar/fullcalendar.js
--rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    84823 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/fullcalendar/fullcalendar.print.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.789201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/all.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.797201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/
--rw-r--r--   0 runner    (1001) docker     (127)    13773 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/_all.css
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/aero.css
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/aero.png
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/blue.css
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/blue.png
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/flat.css
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/flat@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/green.css
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/green.png
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/grey.css
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/grey.png
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/orange.css
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/orange.png
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/pink.css
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/pink.png
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/purple.css
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/purple.png
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/red.css
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/red.png
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/yellow.css
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/yellow.png
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.797201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/futurico/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/futurico/futurico.css
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/futurico/futurico.png
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/futurico/futurico@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/icheck.js
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/icheck.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.797201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/
--rw-r--r--   0 runner    (1001) docker     (127)    21689 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/_all.css
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/aero.css
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/blue.css
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/green.css
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/grey.css
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/line.css
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/line.png
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/line@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/orange.css
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/pink.css
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/purple.css
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/red.css
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/yellow.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.805201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/
--rw-r--r--   0 runner    (1001) docker     (127)    14176 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/_all.css
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/aero.css
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/aero.png
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/blue.css
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/blue.png
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/green.css
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/green.png
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/grey.css
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/grey.png
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/minimal.css
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/minimal.png
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/minimal@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/orange.css
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/orange.png
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/pink.css
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/pink.png
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/purple.css
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/purple.png
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/red.css
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/red.png
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/yellow.css
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/yellow.png
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.805201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/polaris/
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/polaris/polaris.css
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/polaris/polaris.png
--rw-r--r--   0 runner    (1001) docker     (127)    16760 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/polaris/polaris@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.809201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/
--rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/_all.css
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/aero.css
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/aero.png
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/blue.css
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/blue.png
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/green.css
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/green.png
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/grey.css
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/grey.png
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/orange.css
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/orange.png
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/pink.css
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/pink.png
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/purple.css
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/purple.png
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/red.css
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/red.png
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/square.css
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/square.png
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/square@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/yellow.css
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/yellow.png
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.809201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/
--rw-r--r--   0 runner    (1001) docker     (127)    22814 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/jquery.inputmask.date.extensions.js
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/jquery.inputmask.extensions.js
--rw-r--r--   0 runner    (1001) docker     (127)    90539 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/jquery.inputmask.js
--rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/jquery.inputmask.numeric.extensions.js
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/jquery.inputmask.phone.extensions.js
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/jquery.inputmask.regex.extensions.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.813201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/phone-codes/
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/phone-codes/phone-be.json
--rw-r--r--   0 runner    (1001) docker     (127)    39492 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/phone-codes/phone-codes.json
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/phone-codes/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.813201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ionslider/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.813201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ionslider/img/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ionslider/img/sprite-skin-flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ionslider/img/sprite-skin-nice.png
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.css
--rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinFlat.css
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinNice.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.813201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jQueryUI/
--rw-r--r--   0 runner    (1001) docker     (127)   470596 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jQueryUI/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (127)   240427 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jQueryUI/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.817201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/
--rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/core.js
--rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)    86927 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   132370 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/jquery.min.map
--rw-r--r--   0 runner    (1001) docker     (127)   218897 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/jquery.slim.js
--rw-r--r--   0 runner    (1001) docker     (127)    69917 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/jquery.slim.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   105346 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/jquery.slim.min.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.817201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jvectormap/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.css
--rw-r--r--   0 runner    (1001) docker     (127)    33323 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    95062 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-usa-en.js
--rw-r--r--   0 runner    (1001) docker     (127)   144313 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-world-mill-en.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.817201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/knob/
--rw-r--r--   0 runner    (1001) docker     (127)    26222 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/knob/jquery.knob.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.817201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/morris/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/morris/morris.css
--rw-r--r--   0 runner    (1001) docker     (127)    66046 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/morris/morris.js
--rw-r--r--   0 runner    (1001) docker     (127)    35652 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/morris/morris.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.821200 hiddifypanel-8.8.97/hiddifypanel/static/plugins/pace/
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/pace/pace.css
--rw-r--r--   0 runner    (1001) docker     (127)    26566 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/pace/pace.js
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/pace/pace.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/pace/pace.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.821200 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.821200 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/esm/
--rw-r--r--   0 runner    (1001) docker     (127)    34601 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/esm/popper-utils.js
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/esm/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    84361 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/esm/popper.js
--rw-r--r--   0 runner    (1001) docker     (127)    20314 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/esm/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    32919 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/popper-utils.js
--rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    80829 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/popper.js
--rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.821200 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/umd/
--rw-r--r--   0 runner    (1001) docker     (127)    35703 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/umd/popper-utils.js
--rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/umd/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    84615 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/umd/popper.js
--rw-r--r--   0 runner    (1001) docker     (127)    20337 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/umd/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.825201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.833201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/az.js
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/bg.js
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/cs.js
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/da.js
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/de.js
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/en.js
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/es.js
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/et.js
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/eu.js
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/fa.js
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/fi.js
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/fr.js
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/gl.js
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/he.js
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/hi.js
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/hr.js
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/hu.js
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/id.js
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/is.js
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/it.js
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/ko.js
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/lt.js
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/lv.js
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/mk.js
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/nb.js
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/nl.js
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/pl.js
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/pt.js
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/ro.js
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/ru.js
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/sk.js
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/sr.js
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/sv.js
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/th.js
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/tr.js
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/uk.js
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/vi.js
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/zh-CN.js
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/zh-TW.js
--rw-r--r--   0 runner    (1001) docker     (127)    17062 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/select2.css
--rw-r--r--   0 runner    (1001) docker     (127)   152250 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/select2.full.js
--rw-r--r--   0 runner    (1001) docker     (127)    71172 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/select2.full.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   132348 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/select2.js
--rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    62834 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/select2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.833201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/slimScroll/
--rw-r--r--   0 runner    (1001) docker     (127)    14973 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.js
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.833201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/sparkline/
--rw-r--r--   0 runner    (1001) docker     (127)   123446 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/sparkline/jquery.sparkline.js
--rw-r--r--   0 runner    (1001) docker     (127)    43247 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/sparkline/jquery.sparkline.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.833201 hiddifypanel-8.8.97/hiddifypanel/static/plugins/timepicker/
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.css
--rw-r--r--   0 runner    (1001) docker     (127)    26014 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.js
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    15453 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.837200 hiddifypanel-8.8.97/hiddifypanel/static/webfonts/
--rw-r--r--   0 runner    (1001) docker     (127)   186124 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   107656 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62320 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    25236 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   397420 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   150516 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.837200 hiddifypanel-8.8.97/hiddifypanel/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/templates/a.html
--rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/templates/admin-layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/templates/admin.ht.old
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/templates/donation.html
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/templates/fake.html
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/templates/flaskadmin-layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.837200 hiddifypanel-8.8.97/hiddifypanel/templates/hiddify-flask-admin/
--rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/templates/hiddify-flask-admin/list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/templates/lte-master.html
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/templates/macros.html
--rw-r--r--   0 runner    (1001) docker     (127)    20924 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/templates/master.html
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/templates/static.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.697201 hiddifypanel-8.8.97/hiddifypanel/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.697201 hiddifypanel-8.8.97/hiddifypanel/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.837200 hiddifypanel-8.8.97/hiddifypanel/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    59298 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   186715 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.697201 hiddifypanel-8.8.97/hiddifypanel/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.841200 hiddifypanel-8.8.97/hiddifypanel/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    79666 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   212293 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.697201 hiddifypanel-8.8.97/hiddifypanel/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.841200 hiddifypanel-8.8.97/hiddifypanel/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    61220 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   183899 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.697201 hiddifypanel-8.8.97/hiddifypanel/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.841200 hiddifypanel-8.8.97/hiddifypanel/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    96994 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   237219 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.697201 hiddifypanel-8.8.97/hiddifypanel/translations/zh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.841200 hiddifypanel-8.8.97/hiddifypanel/translations/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    55973 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/translations/zh/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   171973 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/hiddifypanel/translations/zh/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:41:31.841200 hiddifypanel-8.8.97/hiddifypanel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-02-23 11:41:31.000000 hiddifypanel-8.8.97/hiddifypanel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    39275 2024-02-23 11:41:31.000000 hiddifypanel-8.8.97/hiddifypanel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 11:41:31.000000 hiddifypanel-8.8.97/hiddifypanel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-23 11:41:31.000000 hiddifypanel-8.8.97/hiddifypanel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-02-23 11:41:31.000000 hiddifypanel-8.8.97/hiddifypanel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-23 11:41:31.000000 hiddifypanel-8.8.97/hiddifypanel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 11:41:31.845200 hiddifypanel-8.8.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-02-23 11:41:17.000000 hiddifypanel-8.8.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.602640 hiddifypanel-8.8.99/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    42706 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19807 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-03-02 13:10:18.602640 hiddifypanel-8.8.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.462637 hiddifypanel-8.8.99/hiddifypanel/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/Events.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.466637 hiddifypanel-8.8.99/hiddifypanel/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/drivers/abstract_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/drivers/singbox_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/drivers/ssh_liberty_bridge_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/drivers/user_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/drivers/xray_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.466637 hiddifypanel-8.8.99/hiddifypanel/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/models/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/models/child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/models/config_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/models/parent_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/models/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/models/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/models/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.470637 hiddifypanel-8.8.99/hiddifypanel/panel/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.470637 hiddifypanel-8.8.99/hiddifypanel/panel/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/Actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/AdminstratorAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/Backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/ChildAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/ConfigAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/Dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/DomainAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/ProxyAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/QuickSetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/SettingAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/Terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/UserAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/adminlte.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/commercial_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.474637 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/a.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/backup.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14994 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/base2.html
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/commercial_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10613 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/configfake.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13299 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/ltemaster.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.474637 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/model/admin_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/model/domain_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/model/user_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/parent_dash.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/proxy.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/quick_setup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/result.html
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/admin_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/cf_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/clean_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.474637 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/ParentDomainAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/ProxyDetailsAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.474637 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/restapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/restapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/restapi/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/restapi/tgbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/restapi/tgmsg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.478637 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/telegrambot/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/telegrambot/DefaultResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/telegrambot/Usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/telegrambot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/telegrambot/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/telegrambot/information.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.478637 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/templates/configc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/commercial/templates/parent_dash.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/custom_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31850 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/hiddify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18746 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/init_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.478637 hiddifypanel-8.8.99/hiddifypanel/panel/user/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/link_maker.html
+-rw-r--r--   0 runner    (1001) docker     (127)    30453 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/link_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.478637 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/all_configs copy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/all_configs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/base_singbox_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/clash_config copy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/clash_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/clash_proxies copy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/clash_proxies.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.482637 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/all-configs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/all-configs_old.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/android.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/auto_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/base2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/clash-links copy.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/clash-links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/doh.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/handle_smart.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12889 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/home.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/index copy.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/index_old.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/ios copy.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/ios.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/multi.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17154 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/one_click.html
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/speedtest.html
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/telegram.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/usage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/windows.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/singbox_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15138 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/panel/user/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.482637 hiddifypanel-8.8.99/hiddifypanel/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/a.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.486637 hiddifypanel-8.8.99/hiddifypanel/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)  1665614 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/css/adminlte.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/css/adminlte.fa.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/css/adminlte.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   155845 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/css/bootstrap4-rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   163995 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/css/bootstrap5.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/css/custom-rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)   101895 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (127)   278568 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/css/lte.old
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.494638 hiddifypanel-8.8.99/hiddifypanel/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    92934 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Black.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    92764 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    53500 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Black.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    42308 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Black.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    91810 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Bold.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    91644 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    52676 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    41856 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   101090 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Light.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   100920 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    59988 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    48616 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Light.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   107842 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Medium.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   107668 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    63312 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Medium.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    51256 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    90482 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Thin.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    90316 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    51884 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Thin.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    41344 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Thin.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    85354 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    85192 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    47972 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    38004 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.494638 hiddifypanel-8.8.99/hiddifypanel/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/WhiteLogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   103814 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   111125 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/hiddify-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37408 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/hiddify.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8441 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/no_back_hiddify.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/pwa-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.498638 hiddifypanel-8.8.99/hiddifypanel/static/images/splash/
+-rw-r--r--   0 runner    (1001) docker     (127)    75224 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/splash/ipad_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    85623 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/splash/ipadpro1_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)   121021 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/splash/ipadpro2_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90886 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/splash/ipadpro3_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28231 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/splash/iphone5_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34920 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/splash/iphone6_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68643 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/splash/iphoneplus_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69743 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/splash/iphonex_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45109 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/splash/iphonexr_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    80648 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/images/splash/iphonexsmax_splash.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.502638 hiddifypanel-8.8.99/hiddifypanel/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   104260 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/adminlte.js
+-rw-r--r--   0 runner    (1001) docker     (127)    49278 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/bootbox.all.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19021 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/bootbox.all.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    78743 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    60406 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/custom-protocol-check.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/custom-rtl.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/custom.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/demo.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89764 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/jquery-3.6.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/js.cookie.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    51465 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/moment.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19032 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/pwa-sw.js
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/pwa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33168 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/js/qrcode.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.462637 hiddifypanel-8.8.99/hiddifypanel/static/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.450636 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.506638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    37644 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (127)    28977 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   172839 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   140421 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.506638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   210612 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)    70808 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   122441 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58072 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.502638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-slider/
+-rw-r--r--   0 runner    (1001) docker     (127)    36164 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-slider/bootstrap-slider.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-slider/slider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.502638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-wysihtml5/
+-rw-r--r--   0 runner    (1001) docker     (127)   566620 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js
+-rw-r--r--   0 runner    (1001) docker     (127)   210932 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.450636 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap4-editable/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.506638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap4-editable/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap4-editable/css/bootstrap-editable.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.506638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap4-editable/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap4-editable/img/clear.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap4-editable/img/loading.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.506638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap4-editable/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   225176 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.js
+-rw-r--r--   0 runner    (1001) docker     (127)    76077 2024-03-02 13:10:09.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.510638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/chart.js/
+-rw-r--r--   0 runner    (1001) docker     (127)   535484 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/chart.js/Chart.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   211133 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/chart.js/Chart.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   403941 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/chart.js/Chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)   159638 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/chart.js/Chart.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.510638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/chartjs-old/
+-rw-r--r--   0 runner    (1001) docker     (127)   109613 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/chartjs-old/Chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)    52092 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/chartjs-old/Chart.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.510638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/
+-rw-r--r--   0 runner    (1001) docker     (127)   433051 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/ckeditor.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.518638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ast.js
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/bg.js
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/cs.js
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/da.js
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/de.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/el.js
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/en-au.js
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/eo.js
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/es.js
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/et.js
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/eu.js
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/fi.js
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/fr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/gl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/gu.js
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/hr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/hu.js
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/it.js
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ja.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/km.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/kn.js
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ko.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ku.js
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/nb.js
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ne.js
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/nl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/oc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/pl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/pt-br.js
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/pt.js
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ro.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ru.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/si.js
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/sk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/sq.js
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/sv.js
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/tr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/tt.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ug.js
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/uk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/zh-cn.js
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/zh.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.518638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.css
+-rw-r--r--   0 runner    (1001) docker     (127)    33831 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.518638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/img/alpha-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/img/alpha.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/img/hue-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/img/hue.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/img/saturation.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.522638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.454637 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.522638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/Readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.522638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/dataTables.autoFill.css
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/dataTables.autoFill.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.522638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/filler.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.522638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    22645 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.522638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/License.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.522638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/dataTables.colReorder.css
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/dataTables.colReorder.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.522638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/insert.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.522638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    36311 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.522638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/License.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.522638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colvis.jqueryui.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.522638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10109 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.526638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/License.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.526638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.css
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.526638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    40932 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14108 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.526638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/Readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.526638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/dataTables.fixedHeader.css
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/dataTables.fixedHeader.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.526638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    29308 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.526638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/KeyTable/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/KeyTable/Readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.526638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/dataTables.keyTable.css
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/dataTables.keyTable.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.526638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    29477 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.526638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/License.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.526638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/responsive.bootstrap4.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.530638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    25098 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/responsive.bootstrap4.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.530638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/Readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.530638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.css
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.530638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/loading-background.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.530638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    37984 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.530638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.530638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.530638 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls_hover.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.534639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    84578 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31850 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.534639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls.swf
+-rw-r--r--   0 runner    (1001) docker     (127)    58846 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls_pdf.swf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.534639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/images/sort_asc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/images/sort_asc_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/images/sort_both.png
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/images/sort_desc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/images/sort_desc_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15369 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/jquery.dataTables.css
+-rw-r--r--   0 runner    (1001) docker     (127)    86551 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/jquery.dataTables.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    86551 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14229 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/jquery.dataTables_themeroller.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.534639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/
+-rw-r--r--   0 runner    (1001) docker     (127)    46838 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/bootstrap-datepicker.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33745 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/datepicker3.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.542639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.az.js
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.bg.js
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cs.js
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cy.js
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.da.js
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.de.js
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.el.js
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.es.js
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.et.js
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fa.js
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fi.js
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.gl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.he.js
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hu.js
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.id.js
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.is.js
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.it.js
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ja.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ka.js
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lt.js
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lv.js
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.mk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ms.js
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nb.js
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl-BE.js
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.no.js
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt.js
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ro.js
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs-latin.js
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs.js
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ru.js
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sq.js
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sv.js
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sw.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.th.js
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.tr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ua.js
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.vi.js
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-CN.js
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-TW.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.542639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/daterangepicker/
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/daterangepicker/daterangepicker-bs3.css
+-rw-r--r--   0 runner    (1001) docker     (127)    53679 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/daterangepicker/daterangepicker.js
+-rw-r--r--   0 runner    (1001) docker     (127)    99201 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/daterangepicker/moment.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34737 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/daterangepicker/moment.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.542639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/fastclick/
+-rw-r--r--   0 runner    (1001) docker     (127)    25965 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/fastclick/fastclick.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/fastclick/fastclick.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.550639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/
+-rw-r--r--   0 runner    (1001) docker     (127)    41944 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/excanvas.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19314 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/excanvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.colorhelpers.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.colorhelpers.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.canvas.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.categories.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.categories.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.image.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.image.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   121627 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.js
+-rw-r--r--   0 runner    (1001) docker     (127)    52300 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14190 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.navigate.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.navigate.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    23635 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.pie.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.pie.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.resize.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.resize.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.selection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.selection.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.stack.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.stack.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.symbol.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.symbol.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.threshold.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.threshold.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.time.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.time.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.458637 hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.550639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    37414 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (127)    21778 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.550639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   134808 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.554639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/fullcalendar/
+-rw-r--r--   0 runner    (1001) docker     (127)    22515 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/fullcalendar/fullcalendar.css
+-rw-r--r--   0 runner    (1001) docker     (127)   279259 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/fullcalendar/fullcalendar.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    84823 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/fullcalendar/fullcalendar.print.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.554639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/all.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.558639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/
+-rw-r--r--   0 runner    (1001) docker     (127)    13773 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/_all.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/aero.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/aero.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/blue.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/flat.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/flat@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/green.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/green.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/grey.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/orange.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/orange.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/pink.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/pink.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/purple.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/purple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/red.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/red.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.558639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/futurico/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/futurico/futurico.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/futurico/futurico.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/futurico/futurico@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/icheck.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/icheck.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.562639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/
+-rw-r--r--   0 runner    (1001) docker     (127)    21689 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/_all.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/aero.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/blue.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/green.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/grey.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/line.css
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/line.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/line@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/orange.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/pink.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/purple.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/red.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/yellow.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.566639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/
+-rw-r--r--   0 runner    (1001) docker     (127)    14176 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/_all.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/aero.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/aero.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/blue.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/green.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/green.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/grey.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/minimal.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/minimal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/minimal@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/orange.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/orange.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/pink.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/pink.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/purple.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/purple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/red.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/red.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.566639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/polaris/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/polaris/polaris.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/polaris/polaris.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16760 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/polaris/polaris@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.570639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/
+-rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/_all.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/aero.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/aero.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/blue.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/green.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/green.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/grey.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/orange.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/orange.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/pink.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/pink.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/purple.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/purple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/red.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/red.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/square.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/square.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/square@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.574639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/
+-rw-r--r--   0 runner    (1001) docker     (127)    22814 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/jquery.inputmask.date.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/jquery.inputmask.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (127)    90539 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/jquery.inputmask.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/jquery.inputmask.numeric.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/jquery.inputmask.phone.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/jquery.inputmask.regex.extensions.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.574639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/phone-codes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/phone-codes/phone-be.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39492 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/phone-codes/phone-codes.json
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/phone-codes/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.574639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ionslider/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.574639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ionslider/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ionslider/img/sprite-skin-flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ionslider/img/sprite-skin-nice.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinFlat.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinNice.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.574639 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jQueryUI/
+-rw-r--r--   0 runner    (1001) docker     (127)   470596 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jQueryUI/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (127)   240427 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jQueryUI/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.578640 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/core.js
+-rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)    86927 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   132370 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/jquery.min.map
+-rw-r--r--   0 runner    (1001) docker     (127)   218897 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/jquery.slim.js
+-rw-r--r--   0 runner    (1001) docker     (127)    69917 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/jquery.slim.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   105346 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/jquery.slim.min.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.578640 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jvectormap/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.css
+-rw-r--r--   0 runner    (1001) docker     (127)    33323 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95062 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-usa-en.js
+-rw-r--r--   0 runner    (1001) docker     (127)   144313 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-world-mill-en.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.578640 hiddifypanel-8.8.99/hiddifypanel/static/plugins/knob/
+-rw-r--r--   0 runner    (1001) docker     (127)    26222 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/knob/jquery.knob.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.578640 hiddifypanel-8.8.99/hiddifypanel/static/plugins/morris/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/morris/morris.css
+-rw-r--r--   0 runner    (1001) docker     (127)    66046 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/morris/morris.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35652 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/morris/morris.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.578640 hiddifypanel-8.8.99/hiddifypanel/static/plugins/pace/
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/pace/pace.css
+-rw-r--r--   0 runner    (1001) docker     (127)    26566 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/pace/pace.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/pace/pace.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/pace/pace.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.582640 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.582640 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/esm/
+-rw-r--r--   0 runner    (1001) docker     (127)    34601 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/esm/popper-utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/esm/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    84361 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/esm/popper.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20314 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/esm/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32919 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/popper-utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    80829 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/popper.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.582640 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/umd/
+-rw-r--r--   0 runner    (1001) docker     (127)    35703 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/umd/popper-utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/umd/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    84615 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/umd/popper.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20337 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/umd/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.582640 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.590640 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/az.js
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/bg.js
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/cs.js
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/da.js
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/de.js
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/en.js
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/es.js
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/et.js
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/eu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/fa.js
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/fi.js
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/fr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/gl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/he.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/hi.js
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/hr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/hu.js
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/id.js
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/is.js
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/it.js
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/ko.js
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/lt.js
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/lv.js
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/mk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/nb.js
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/nl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/pl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/pt.js
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/ro.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/ru.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/sk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/sr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/sv.js
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/th.js
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/tr.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/uk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/vi.js
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/zh-CN.js
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/zh-TW.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17062 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/select2.css
+-rw-r--r--   0 runner    (1001) docker     (127)   152250 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/select2.full.js
+-rw-r--r--   0 runner    (1001) docker     (127)    71172 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/select2.full.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   132348 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/select2.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    62834 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/select2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.590640 hiddifypanel-8.8.99/hiddifypanel/static/plugins/slimScroll/
+-rw-r--r--   0 runner    (1001) docker     (127)    14973 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.590640 hiddifypanel-8.8.99/hiddifypanel/static/plugins/sparkline/
+-rw-r--r--   0 runner    (1001) docker     (127)   123446 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/sparkline/jquery.sparkline.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43247 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/sparkline/jquery.sparkline.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.590640 hiddifypanel-8.8.99/hiddifypanel/static/plugins/timepicker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.css
+-rw-r--r--   0 runner    (1001) docker     (127)    26014 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15453 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.594640 hiddifypanel-8.8.99/hiddifypanel/static/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   186124 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   107656 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62320 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    25236 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   397420 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   150516 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.598640 hiddifypanel-8.8.99/hiddifypanel/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/templates/a.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/templates/admin-layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/templates/admin.ht.old
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/templates/donation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/templates/fake.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/templates/flaskadmin-layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.598640 hiddifypanel-8.8.99/hiddifypanel/templates/hiddify-flask-admin/
+-rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/templates/hiddify-flask-admin/list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/templates/lte-master.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20924 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/templates/master.html
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/templates/static.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.462637 hiddifypanel-8.8.99/hiddifypanel/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.462637 hiddifypanel-8.8.99/hiddifypanel/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.598640 hiddifypanel-8.8.99/hiddifypanel/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    59298 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   186715 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.462637 hiddifypanel-8.8.99/hiddifypanel/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.598640 hiddifypanel-8.8.99/hiddifypanel/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    79666 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   212293 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.462637 hiddifypanel-8.8.99/hiddifypanel/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.598640 hiddifypanel-8.8.99/hiddifypanel/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    61220 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   183899 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.462637 hiddifypanel-8.8.99/hiddifypanel/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.598640 hiddifypanel-8.8.99/hiddifypanel/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    96994 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   237219 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.462637 hiddifypanel-8.8.99/hiddifypanel/translations/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.598640 hiddifypanel-8.8.99/hiddifypanel/translations/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    55973 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/translations/zh/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   171973 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/hiddifypanel/translations/zh/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 13:10:18.598640 hiddifypanel-8.8.99/hiddifypanel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-03-02 13:10:18.000000 hiddifypanel-8.8.99/hiddifypanel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39275 2024-03-02 13:10:18.000000 hiddifypanel-8.8.99/hiddifypanel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 13:10:18.000000 hiddifypanel-8.8.99/hiddifypanel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-02 13:10:18.000000 hiddifypanel-8.8.99/hiddifypanel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-02 13:10:18.000000 hiddifypanel-8.8.99/hiddifypanel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-02 13:10:18.000000 hiddifypanel-8.8.99/hiddifypanel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 13:10:18.602640 hiddifypanel-8.8.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-02 13:10:10.000000 hiddifypanel-8.8.99/setup.py
```

### Comparing `hiddifypanel-8.8.97/HISTORY.md` & `hiddifypanel-8.8.99/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 # Changelog
 
 
+## 8.8.99 (2024-03-02)
+
+#### Fix
+
+* Bug (latest release on v8) 
+
+
+
 ## 8.8.96 (2024-02-21)
 
 #### New
 
 * Add more security for first setup. 
 
 #### Fix
```

### Comparing `hiddifypanel-8.8.97/LICENSE.md` & `hiddifypanel-8.8.99/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/PKG-INFO` & `hiddifypanel-8.8.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiddifypanel
-Version: 8.8.97
+Version: 8.8.99
 Summary: hiddifypanel multi proxy panel
 Home-page: https://github.com/hiddify/hiddify-server/
 Author: hiddify
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ansi2html==1.8.0
 Requires-Dist: async-timeout==4.0.3
```

### Comparing `hiddifypanel-8.8.97/README.md` & `hiddifypanel-8.8.99/README.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/Events.py` & `hiddifypanel-8.8.99/hiddifypanel/Events.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/base.py` & `hiddifypanel-8.8.99/hiddifypanel/base.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/cache.py` & `hiddifypanel-8.8.99/hiddifypanel/cache.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/drivers/singbox_api.py` & `hiddifypanel-8.8.99/hiddifypanel/drivers/singbox_api.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/drivers/ssh_liberty_bridge_api.py` & `hiddifypanel-8.8.99/hiddifypanel/drivers/ssh_liberty_bridge_api.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/drivers/user_driver.py` & `hiddifypanel-8.8.99/hiddifypanel/drivers/user_driver.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/drivers/xray_api.py` & `hiddifypanel-8.8.99/hiddifypanel/drivers/xray_api.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/models/__init__.py` & `hiddifypanel-8.8.99/hiddifypanel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/models/admin.py` & `hiddifypanel-8.8.99/hiddifypanel/models/admin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/models/child.py` & `hiddifypanel-8.8.99/hiddifypanel/models/child.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/models/config.py` & `hiddifypanel-8.8.99/hiddifypanel/models/config.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/models/config_enum.py` & `hiddifypanel-8.8.99/hiddifypanel/models/config_enum.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/models/domain.py` & `hiddifypanel-8.8.99/hiddifypanel/models/domain.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/models/parent_domain.py` & `hiddifypanel-8.8.99/hiddifypanel/models/parent_domain.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/models/proxy.py` & `hiddifypanel-8.8.99/hiddifypanel/models/proxy.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/models/report.py` & `hiddifypanel-8.8.99/hiddifypanel/models/report.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/models/usage.py` & `hiddifypanel-8.8.99/hiddifypanel/models/usage.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/models/user.py` & `hiddifypanel-8.8.99/hiddifypanel/models/user.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/Actions.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/Actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             link = f'https://{d}/{proxy_path}/{admin_secret}/admin/'
             admin_links += f"<li><a target='_blank' class='badge ltr' href='{link}'>{link}</a></li>"
 
         resp = render_template("result.html",
                                out_type="info",
                                out_msg=_("Success! Please wait around 4 minutes to make sure everything is updated. During this time, please save your proxy links which are:") +
                                admin_links,
-                               log_path=get_logpath("install.log"),
+                               log_path=get_logpath("0-install.log"),
                                show_success=True,
                                domains=get_domains(),
 
 
 
                                )
 
@@ -214,15 +214,15 @@
         res = "<table><tr><th>Domain</th><th>IP</th><th>Country</th><th>ASN</th><th>Ping (ms)</th><th>TCP ping (ms)</th></tr>"
         res += f"<tr><td>Your Server</td><td>{ipv4}</td><td>{server_country}</td><td>{server_asn}</td><td>0</td></tr>"
         import time
         start = time.time()
         for d in [test_domain, *hiddify.get_random_domains(30)]:
             if not d:
                 continue
-            if time.time()-start > 20:
+            if time.time() - start > 20:
                 break
             print(d)
             tcp_ping = hiddify.is_domain_reality_friendly(d)
             if tcp_ping:
                 dip = hiddify.get_domain_ip(d)
                 dip_country = (ipcountry.get(dip) or {}).get('country', {}).get('iso_code', 'unknown')
                 if dip_country == "IR":
@@ -233,15 +233,15 @@
                     if response_time:
                         response_time = int(response_time)
                 except:
                     pass
                 dip_asn = (ipasn.get(dip) or {}).get('autonomous_system_organization', 'unknown')
                 res += f"<tr><td>{d}</td><td>{dip}</td><td>{dip_country}</td><td>{dip_asn}</td><td>{response_time}</td><td>{tcp_ping}<td></tr>"
 
-        return res+"</table>"
+        return res + "</table>"
 
     @hiddify.super_admin
     def update_usage(self):
 
         import json
 
         return render_template("result.html",
```

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/AdminstratorAdmin.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/AdminstratorAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/Backup.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/Backup.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/ChildAdmin.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/ChildAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/ConfigAdmin.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/ConfigAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/Dashboard.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/Dashboard.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/DomainAdmin.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/DomainAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/ProxyAdmin.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/ProxyAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/QuickSetup.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/QuickSetup.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/SettingAdmin.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/SettingAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/Terminal.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/Terminal.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/UserAdmin.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/UserAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/__init__.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/adminlte.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/adminlte.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/commercial_info.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/commercial_info.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/backup.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/backup.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/base.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/base.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/base2.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/base2.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/config.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/config.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/configfake.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/configfake.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/index.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/index.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/ltemaster.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/ltemaster.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/model/admin_list.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/model/admin_list.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/model/user_list.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/model/user_list.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/parent_dash.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/parent_dash.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/proxy.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/proxy.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/quick_setup.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/quick_setup.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin/templates/result.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin/templates/result.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/admin_2.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/admin_2.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/cf_api.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/cf_api.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/clean_ip.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/clean_ip.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/cli.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/cli.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/commercial/ParentDomainAdmin.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/commercial/ParentDomainAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/commercial/ProxyDetailsAdmin.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/commercial/ProxyDetailsAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/commercial/__init__.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/commercial/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/commercial/restapi/__init__.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/commercial/restapi/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/commercial/restapi/resources.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/commercial/restapi/resources.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/commercial/restapi/tgbot.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/commercial/restapi/tgbot.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/commercial/restapi/tgmsg.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/commercial/restapi/tgmsg.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/commercial/telegrambot/Usage.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/commercial/telegrambot/Usage.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/commercial/telegrambot/admin.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/commercial/telegrambot/admin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/commercial/telegrambot/information.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/commercial/telegrambot/information.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/commercial/templates/configc.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/commercial/templates/configc.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/commercial/templates/parent_dash.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/commercial/templates/parent_dash.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/common.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/common.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/custom_widgets.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/hiddify.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/hiddify.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/init_db.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/init_db.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/usage.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/usage.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/__init__.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/link_maker.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/link_maker.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/all_configs.txt` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/all_configs.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/base_singbox_config.json` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/base_singbox_config.json`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/clash_config copy.yml` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/clash_config copy.yml`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/clash_config.yml` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/clash_config.yml`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/clash_proxies copy.yml` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/clash_proxies copy.yml`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/clash_proxies.yml` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/clash_proxies.yml`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/all-configs.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/all-configs.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/all-configs_old.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/all-configs_old.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/android.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/android.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/auto_page.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/auto_page.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/base2.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/base2.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/clash-links copy.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/clash-links copy.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/clash-links.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/clash-links.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/handle_smart.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/handle_smart.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/home.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/home.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/index copy.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/index copy.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/index_old.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/index_old.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/ios copy.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/ios copy.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/ios.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/ios.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/multi.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/multi.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/one_click.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/one_click.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/speedtest.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/speedtest.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/telegram.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/telegram.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/usage.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/usage.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/home/windows.html` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/home/windows.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/templates/singbox_config.json` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/templates/singbox_config.json`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/panel/user/user.py` & `hiddifypanel-8.8.99/hiddifypanel/panel/user/user.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/a.txt` & `hiddifypanel-8.8.99/hiddifypanel/static/a.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/css/adminlte.css` & `hiddifypanel-8.8.99/hiddifypanel/static/css/adminlte.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/css/adminlte.fa.css` & `hiddifypanel-8.8.99/hiddifypanel/static/css/adminlte.fa.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/css/adminlte.rtl.css` & `hiddifypanel-8.8.99/hiddifypanel/static/css/adminlte.rtl.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/css/bootstrap.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/css/bootstrap4-rtl.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/css/bootstrap4-rtl.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/css/bootstrap5.rtl.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/css/bootstrap5.rtl.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/css/custom.css` & `hiddifypanel-8.8.99/hiddifypanel/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/css/font-awesome.css` & `hiddifypanel-8.8.99/hiddifypanel/static/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/css/lte.old` & `hiddifypanel-8.8.99/hiddifypanel/static/css/lte.old`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Black.eot` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Black.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Black.ttf` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Black.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Black.woff` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Black.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Black.woff2` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Black.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Bold.eot` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Bold.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Bold.ttf` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Bold.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Bold.woff` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Bold.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Bold.woff2` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Bold.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Light.eot` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Light.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Light.ttf` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Light.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Light.woff` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Light.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Light.woff2` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Light.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Medium.eot` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Medium.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Medium.ttf` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Medium.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Medium.woff` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Medium.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Medium.woff2` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Medium.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Thin.eot` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Thin.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Thin.ttf` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Thin.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Thin.woff` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Thin.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir-Thin.woff2` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir-Thin.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir.eot` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir.ttf` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir.woff` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/fonts/Vazir.woff2` & `hiddifypanel-8.8.99/hiddifypanel/static/fonts/Vazir.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/WhiteLogo.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/WhiteLogo.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/favicon.ico` & `hiddifypanel-8.8.99/hiddifypanel/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/hiddify-dark.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/hiddify-dark.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/hiddify.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/hiddify.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/no_back_hiddify.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/no_back_hiddify.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/pwa-icon.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/pwa-icon.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/splash/ipad_splash.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/splash/ipad_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/splash/ipadpro1_splash.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/splash/ipadpro1_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/splash/ipadpro2_splash.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/splash/ipadpro2_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/splash/ipadpro3_splash.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/splash/ipadpro3_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/splash/iphone5_splash.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/splash/iphone5_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/splash/iphone6_splash.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/splash/iphone6_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/splash/iphoneplus_splash.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/splash/iphoneplus_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/splash/iphonex_splash.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/splash/iphonex_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/splash/iphonexr_splash.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/splash/iphonexr_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/images/splash/iphonexsmax_splash.png` & `hiddifypanel-8.8.99/hiddifypanel/static/images/splash/iphonexsmax_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/adminlte.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/adminlte.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/bootbox.all.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/bootbox.all.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/bootbox.all.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/bootbox.all.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/bootstrap.bundle.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/bootstrap.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/custom-protocol-check.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/custom-protocol-check.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/custom-rtl.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/custom-rtl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/custom.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/custom.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/demo.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/demo.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/jquery-3.6.1.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/jquery-3.6.1.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/js.cookie.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/js.cookie.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/moment.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/popper.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/pwa.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/pwa.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/js/qrcode.js` & `hiddifypanel-8.8.99/hiddifypanel/static/js/qrcode.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/css/bootstrap.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/css/bootstrap.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/js/bootstrap.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap/js/bootstrap.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-slider/bootstrap-slider.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-slider/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-slider/slider.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-slider/slider.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap4-editable/css/bootstrap-editable.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap4-editable/css/bootstrap-editable.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap4-editable/img/loading.gif` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap4-editable/img/loading.gif`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/chart.js/Chart.bundle.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/chart.js/Chart.bundle.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/chart.js/Chart.bundle.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/chart.js/Chart.bundle.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/chart.js/Chart.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/chart.js/Chart.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/chart.js/Chart.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/chart.js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/chartjs-old/Chart.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/chartjs-old/Chart.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/chartjs-old/Chart.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/chartjs-old/Chart.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/ckeditor.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/ckeditor.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ar.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ar.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ast.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ast.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/bg.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/bg.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/cs.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/cs.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/da.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/da.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/de.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/de.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/el.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/el.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/en-au.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/en-au.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/eo.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/eo.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/es.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/es.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/et.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/et.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/eu.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/eu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/fi.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/fi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/fr.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/fr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/gl.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/gl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/gu.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/gu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/hr.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/hr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/hu.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/hu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/it.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/it.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ja.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ja.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/km.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/km.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/kn.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/kn.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ko.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ko.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ku.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ku.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/nb.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/nb.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ne.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ne.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/nl.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/nl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/oc.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/oc.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/pl.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/pl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/pt-br.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/pt-br.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/pt.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/pt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ro.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ro.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ru.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ru.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/si.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/si.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/sk.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/sk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/sq.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/sq.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/sv.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/sv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/tr.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/tr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/tt.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/tt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/ug.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/ug.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/uk.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/uk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/zh-cn.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/zh-cn.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ckeditor/translations/zh.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ckeditor/translations/zh.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/img/alpha-horizontal.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/img/alpha-horizontal.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/img/alpha.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/img/alpha.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/img/hue-horizontal.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/img/hue-horizontal.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/img/hue.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/img/hue.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/colorpicker/img/saturation.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/colorpicker/img/saturation.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/Readme.txt` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/Readme.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/filler.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/filler.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/License.txt` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/License.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/Readme.md` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/Readme.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/insert.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/insert.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/License.txt` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/License.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/Readme.md` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/Readme.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colvis.jqueryui.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colvis.jqueryui.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/License.txt` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/License.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/Readme.md` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/Readme.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/Readme.txt` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/Readme.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/KeyTable/Readme.txt` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/KeyTable/Readme.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/License.txt` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/License.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.scss` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.scss`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/responsive.bootstrap4.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/responsive.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/responsive.bootstrap4.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/responsive.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/Readme.txt` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/Readme.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/loading-background.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/loading-background.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/Readme.md` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/Readme.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection_hover.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy_hover.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv_hover.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf_hover.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print_hover.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls_hover.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls.swf` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls.swf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls_pdf.swf` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls_pdf.swf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/jquery.dataTables.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/jquery.dataTables.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/jquery.dataTables.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datatables/jquery.dataTables_themeroller.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datatables/jquery.dataTables_themeroller.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/bootstrap-datepicker.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/datepicker3.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/datepicker3.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ar.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ar.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.az.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.az.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.bg.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.bg.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ca.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ca.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cs.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cs.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cy.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cy.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.da.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.da.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.de.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.de.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.el.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.el.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.es.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.es.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.et.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.et.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fa.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fa.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fi.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fr.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.gl.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.gl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.he.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.he.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hr.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hu.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.id.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.id.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.is.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.is.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.it.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.it.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ja.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ja.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ka.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ka.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kk.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kr.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lt.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lv.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.mk.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.mk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ms.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ms.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nb.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nb.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl-BE.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl-BE.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.no.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.no.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pl.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt-BR.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt-BR.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ro.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ro.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs-latin.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs-latin.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ru.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ru.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sk.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sl.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sq.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sq.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sv.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sw.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sw.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.th.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.th.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.tr.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.tr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ua.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ua.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.vi.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.vi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-CN.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-CN.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-TW.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-TW.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/daterangepicker/daterangepicker-bs3.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/daterangepicker/daterangepicker-bs3.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/daterangepicker/daterangepicker.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/daterangepicker/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/daterangepicker/moment.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/daterangepicker/moment.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/daterangepicker/moment.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/daterangepicker/moment.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/fastclick/fastclick.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/fastclick/fastclick.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/fastclick/fastclick.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/fastclick/fastclick.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/excanvas.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/excanvas.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/excanvas.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/excanvas.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.colorhelpers.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.colorhelpers.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.colorhelpers.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.colorhelpers.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.canvas.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.canvas.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.canvas.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.canvas.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.categories.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.categories.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.categories.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.categories.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.image.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.image.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.image.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.image.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.navigate.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.navigate.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.navigate.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.navigate.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.pie.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.pie.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.pie.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.pie.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.resize.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.resize.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.resize.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.resize.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.selection.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.selection.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.selection.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.selection.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.stack.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.stack.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.stack.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.stack.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.symbol.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.symbol.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.symbol.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.symbol.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.threshold.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.threshold.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.threshold.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.threshold.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.time.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.time.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/flot/jquery.flot.time.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/flot/jquery.flot.time.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css.map` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/css/font-awesome.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/fonts/FontAwesome.otf` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.eot` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.svg` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.ttf` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff2` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/fullcalendar/fullcalendar.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/fullcalendar/fullcalendar.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/fullcalendar/fullcalendar.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/fullcalendar/fullcalendar.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/fullcalendar/fullcalendar.print.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/fullcalendar/fullcalendar.print.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/all.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/_all.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/_all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/aero.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/aero.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/aero.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/aero.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/aero@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/aero@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/blue.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/blue.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/blue.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/blue.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/blue@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/blue@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/flat.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/flat.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/flat.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/flat.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/flat@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/flat@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/green.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/green.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/green.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/green.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/green@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/green@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/grey.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/grey.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/grey.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/grey.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/grey@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/grey@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/orange.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/orange.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/orange.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/orange.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/orange@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/orange@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/pink.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/pink.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/pink.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/pink.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/pink@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/pink@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/purple.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/purple.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/purple.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/purple.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/purple@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/purple@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/red.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/red.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/red.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/red.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/red@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/red@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/yellow.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/yellow.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/yellow.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/yellow.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/flat/yellow@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/flat/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/futurico/futurico.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/futurico/futurico.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/futurico/futurico.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/futurico/futurico.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/futurico/futurico@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/futurico/futurico@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/icheck.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/icheck.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/icheck.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/icheck.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/_all.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/_all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/aero.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/aero.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/blue.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/blue.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/green.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/green.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/grey.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/grey.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/line.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/line.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/line.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/line.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/line@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/line@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/orange.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/orange.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/pink.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/pink.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/purple.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/purple.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/red.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/red.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/line/yellow.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/line/yellow.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/_all.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/_all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/aero.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/aero.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/aero.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/aero.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/aero@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/aero@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/blue.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/blue.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/blue.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/blue.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/blue@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/blue@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/green.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/green.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/green.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/green.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/green@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/green@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/grey.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/grey.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/grey.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/grey.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/grey@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/grey@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/minimal.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/minimal.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/minimal.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/minimal.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/minimal@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/minimal@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/orange.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/orange.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/orange.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/orange.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/orange@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/orange@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/pink.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/pink.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/pink.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/pink.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/pink@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/pink@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/purple.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/purple.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/purple.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/purple.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/purple@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/purple@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/red.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/red.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/red.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/red.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/red@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/red@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/yellow.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/yellow.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/yellow.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/yellow.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/minimal/yellow@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/minimal/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/polaris/polaris.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/polaris/polaris.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/polaris/polaris.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/polaris/polaris.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/polaris/polaris@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/polaris/polaris@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/_all.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/_all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/aero.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/aero.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/aero.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/aero.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/aero@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/aero@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/blue.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/blue.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/blue.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/blue.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/blue@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/blue@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/green.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/green.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/green.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/green.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/green@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/green@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/grey.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/grey.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/grey.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/grey.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/grey@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/grey@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/orange.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/orange.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/orange.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/orange.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/orange@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/orange@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/pink.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/pink.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/pink.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/pink.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/pink@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/pink@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/purple.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/purple.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/purple.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/purple.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/purple@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/purple@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/red.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/red.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/red.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/red.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/red@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/red@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/square.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/square.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/square.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/square.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/square@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/square@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/yellow.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/yellow.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/yellow.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/yellow.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/iCheck/square/yellow@2x.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/iCheck/square/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/jquery.inputmask.date.extensions.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/jquery.inputmask.date.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/jquery.inputmask.extensions.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/jquery.inputmask.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/jquery.inputmask.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/jquery.inputmask.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/jquery.inputmask.numeric.extensions.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/jquery.inputmask.numeric.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/jquery.inputmask.phone.extensions.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/jquery.inputmask.phone.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/jquery.inputmask.regex.extensions.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/jquery.inputmask.regex.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/phone-codes/phone-be.json` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/phone-codes/phone-be.json`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/input-mask/phone-codes/phone-codes.json` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/input-mask/phone-codes/phone-codes.json`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ionslider/img/sprite-skin-nice.png` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ionslider/img/sprite-skin-nice.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinFlat.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinFlat.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinNice.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinNice.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/jQueryUI/jquery-ui.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/jQueryUI/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/jQueryUI/jquery-ui.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/jQueryUI/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/core.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/core.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/jquery.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/jquery.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/jquery.min.map` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/jquery.min.map`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/jquery.slim.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/jquery.slim.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/jquery.slim.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/jquery/jquery.slim.min.map` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/jquery/jquery.slim.min.map`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-usa-en.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-usa-en.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-world-mill-en.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-world-mill-en.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/knob/jquery.knob.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/knob/jquery.knob.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/morris/morris.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/morris/morris.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/morris/morris.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/morris/morris.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/pace/pace.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/pace/pace.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/pace/pace.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/pace/pace.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/pace/pace.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/pace/pace.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/pace/pace.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/pace/pace.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/esm/popper-utils.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/esm/popper-utils.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/esm/popper-utils.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/esm/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/esm/popper.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/esm/popper.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/esm/popper.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/esm/popper.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/popper-utils.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/popper-utils.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/popper-utils.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/popper.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/popper.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/popper.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/popper.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/umd/popper-utils.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/umd/popper-utils.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/umd/popper-utils.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/umd/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/umd/popper.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/umd/popper.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/popper/umd/popper.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/popper/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/az.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/az.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/bg.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/ca.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/cs.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/da.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/da.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/de.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/de.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/en.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/en.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/es.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/es.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/et.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/et.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/eu.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/fa.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/fi.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/fr.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/gl.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/he.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/he.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/hi.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/hr.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/hu.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/id.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/id.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/is.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/is.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/it.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/it.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/ko.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/lt.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/lv.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/mk.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/nb.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/nl.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/pl.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/pt-BR.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/pt.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/ro.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/ru.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/sk.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/sr.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/sv.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/th.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/th.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/tr.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/uk.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/vi.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/zh-CN.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/i18n/zh-TW.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/select2.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/select2.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/select2.full.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/select2.full.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/select2.full.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/select2.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/select2.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/select2.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/select2/select2.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/select2/select2.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/sparkline/jquery.sparkline.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/sparkline/jquery.sparkline.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/sparkline/jquery.sparkline.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/sparkline/jquery.sparkline.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.css` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.js` & `hiddifypanel-8.8.99/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-brands-400.ttf` & `hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-brands-400.woff2` & `hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-regular-400.ttf` & `hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-regular-400.woff2` & `hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-solid-900.ttf` & `hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-solid-900.woff2` & `hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-v4compatibility.ttf` & `hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/static/webfonts/fa-v4compatibility.woff2` & `hiddifypanel-8.8.99/hiddifypanel/static/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/templates/500.html` & `hiddifypanel-8.8.99/hiddifypanel/templates/500.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/templates/admin-layout.html` & `hiddifypanel-8.8.99/hiddifypanel/templates/admin-layout.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/templates/admin.ht.old` & `hiddifypanel-8.8.99/hiddifypanel/templates/admin.ht.old`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/templates/donation.html` & `hiddifypanel-8.8.99/hiddifypanel/templates/donation.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/templates/fake.html` & `hiddifypanel-8.8.99/hiddifypanel/templates/fake.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/templates/flaskadmin-layout.html` & `hiddifypanel-8.8.99/hiddifypanel/templates/flaskadmin-layout.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/templates/hiddify-flask-admin/list.html` & `hiddifypanel-8.8.99/hiddifypanel/templates/hiddify-flask-admin/list.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/templates/lte-master.html` & `hiddifypanel-8.8.99/hiddifypanel/templates/lte-master.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/templates/macros.html` & `hiddifypanel-8.8.99/hiddifypanel/templates/macros.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/templates/master.html` & `hiddifypanel-8.8.99/hiddifypanel/templates/master.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/translations/en/LC_MESSAGES/messages.mo` & `hiddifypanel-8.8.99/hiddifypanel/translations/en/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/translations/en/LC_MESSAGES/messages.po` & `hiddifypanel-8.8.99/hiddifypanel/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/translations/fa/LC_MESSAGES/messages.mo` & `hiddifypanel-8.8.99/hiddifypanel/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/translations/fa/LC_MESSAGES/messages.po` & `hiddifypanel-8.8.99/hiddifypanel/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/translations/pt/LC_MESSAGES/messages.mo` & `hiddifypanel-8.8.99/hiddifypanel/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/translations/pt/LC_MESSAGES/messages.po` & `hiddifypanel-8.8.99/hiddifypanel/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/translations/ru/LC_MESSAGES/messages.mo` & `hiddifypanel-8.8.99/hiddifypanel/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/translations/ru/LC_MESSAGES/messages.po` & `hiddifypanel-8.8.99/hiddifypanel/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/translations/zh/LC_MESSAGES/messages.mo` & `hiddifypanel-8.8.99/hiddifypanel/translations/zh/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel/translations/zh/LC_MESSAGES/messages.po` & `hiddifypanel-8.8.99/hiddifypanel/translations/zh/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel.egg-info/PKG-INFO` & `hiddifypanel-8.8.99/hiddifypanel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiddifypanel
-Version: 8.8.97
+Version: 8.8.99
 Summary: hiddifypanel multi proxy panel
 Home-page: https://github.com/hiddify/hiddify-server/
 Author: hiddify
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ansi2html==1.8.0
 Requires-Dist: async-timeout==4.0.3
```

### Comparing `hiddifypanel-8.8.97/hiddifypanel.egg-info/SOURCES.txt` & `hiddifypanel-8.8.99/hiddifypanel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/hiddifypanel.egg-info/requires.txt` & `hiddifypanel-8.8.99/hiddifypanel.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.8.97/setup.py` & `hiddifypanel-8.8.99/setup.py`

 * *Files identical despite different names*

