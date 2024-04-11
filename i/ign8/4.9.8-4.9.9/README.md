# Comparing `tmp/ign8-4.9.8.tar.gz` & `tmp/ign8-4.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ign8-4.9.8.tar", max compression
+gzip compressed data, was "ign8-4.9.9.tar", max compression
```

## Comparing `ign8-4.9.8.tar` & `ign8-4.9.9.tar`

### file list

```diff
@@ -1,227 +1,227 @@
--rw-r--r--   0        0        0     1083 2024-01-29 06:08:13.072060 ign8-4.9.8/LICENSE.txt
--rw-r--r--   0        0        0     6071 2024-01-29 06:08:13.072060 ign8-4.9.8/README.md
--rw-r--r--   0        0        0     2864 2024-04-11 11:06:21.286859 ign8-4.9.8/pyproject.toml
--rw-r--r--   0        0        0     2700 2024-04-08 07:05:32.385960 ign8-4.9.8/src/ign8/__init__.py
--rw-r--r--   0        0        0     1492 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/airflow/__init__.py
--rw-r--r--   0        0        0     5278 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/airflow/airflow.py
--rw-r--r--   0        0        0     3771 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/awx/__pycache__/awx_common.cpython-311.pyc
--rw-r--r--   0        0        0     4174 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/awx/__pycache__/awx_credential.cpython-311.pyc
--rw-r--r--   0        0        0     2864 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/awx/__pycache__/awx_organisation.cpython-311.pyc
--rw-r--r--   0        0        0     4443 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/awx/__pycache__/awx_project.cpython-311.pyc
--rw-r--r--   0        0        0     2676 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/awx/awx_common.py
--rw-r--r--   0        0        0     5230 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/awx/awx_credential.py
--rw-r--r--   0        0        0     1997 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/awx/awx_executionenvironments.py
--rw-r--r--   0        0        0     1251 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/awx/awx_hosts.py
--rw-r--r--   0        0        0     2320 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/awx/awx_organisation.py
--rw-r--r--   0        0        0     3474 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/awx/awx_project.py
--rw-r--r--   0        0        0    37171 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/awx/kalm.py
--rw-r--r--   0        0        0      999 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/bump/__init__.py
--rw-r--r--   0        0        0     3494 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/bump/bump.py
--rw-r--r--   0        0        0     4323 2024-04-08 07:11:51.256041 ign8-4.9.8/src/ign8/common.py
--rw-r--r--   0        0        0     3320 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/dns/__init__.py
--rw-r--r--   0        0        0     2146 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/dns/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    13524 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/dns/__pycache__/dns.cpython-311.pyc
--rw-r--r--   0        0        0     4968 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/dns/cloudflare.py
--rw-r--r--   0        0        0    15599 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/dns/dns.py
--rw-r--r--   0        0        0      855 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/fiile/__init__.py
--rw-r--r--   0        0        0      188 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/fiile/file.py
--rw-r--r--   0        0        0      830 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/gitea/__init__.py
--rw-r--r--   0        0        0     5396 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/gitea/git.py
--rw-r--r--   0        0        0    58332 2024-04-08 05:48:22.333690 ign8-4.9.8/src/ign8/homeassistant/after.json
--rw-r--r--   0        0        0      435 2024-04-08 05:48:22.333690 ign8-4.9.8/src/ign8/homeassistant/after.lst
--rw-r--r--   0        0        0      132 2024-04-08 05:48:22.333690 ign8-4.9.8/src/ign8/homeassistant/aut.sh
--rw-r--r--   0        0        0    58332 2024-04-08 05:48:22.333690 ign8-4.9.8/src/ign8/homeassistant/before.json
--rw-r--r--   0        0        0      435 2024-04-08 05:48:22.333690 ign8-4.9.8/src/ign8/homeassistant/before.lst
--rw-r--r--   0        0        0       98 2024-04-08 05:48:22.333690 ign8-4.9.8/src/ign8/homeassistant/hue.env
--rw-r--r--   0        0        0     2680 2024-04-08 05:48:22.333690 ign8-4.9.8/src/ign8/homeassistant/hue.py
--rw-r--r--   0        0        0     1796 2024-04-08 05:48:22.333690 ign8-4.9.8/src/ign8/homeassistant/hue.test.py
--rw-r--r--   0        0        0     3944 2024-04-08 05:48:22.333690 ign8-4.9.8/src/ign8/homeassistant/logger.py
--rw-r--r--   0        0        0 49453399 2024-04-08 05:48:22.389691 ign8-4.9.8/src/ign8/homeassistant/os
--rw-r--r--   0        0        0      226 2024-04-08 05:48:22.389691 ign8-4.9.8/src/ign8/homeassistant/paused.conf
--rw-r--r--   0        0        0      419 2024-04-08 05:48:22.389691 ign8-4.9.8/src/ign8/homeassistant/requesttest.py
--rw-r--r--   0        0        0     5604 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/homeassistant/service.py
--rw-r--r--   0        0        0     1335 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/homeassistant/servicetest.py
--rw-r--r--   0        0        0       44 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/homeassistant/start.sh
--rw-r--r--   0        0        0      447 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/homeassistant/stash.py
--rw-r--r--   0        0        0    58332 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/homeassistant/test.json
--rw-r--r--   0        0        0       15 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/homeassistant/test.lst
--rw-r--r--   0        0        0      604 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/homeassistant/test.lst.org
--rwxr-xr-x   0        0        0      197 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/homeassistant/test.sh
--rw-r--r--   0        0        0      783 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/homeassistant/turnontest.py
--rw-r--r--   0        0        0      153 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/iad/__init__.py
--rw-r--r--   0        0        0      176 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/iad/iad.py
--rw-r--r--   0        0        0     1063 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/inabox/__init__.py
--rw-r--r--   0        0        0    11552 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/inabox/inabox.py
--rw-r--r--   0        0        0      329 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/inabox/virtlib.py
--rw-r--r--   0        0        0     1549 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/inthevault/__init__.py
--rw-r--r--   0        0        0     2454 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/inthevault/inthevault.py
--rw-r--r--   0        0        0     1415 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/jenkins/__init__.py
--rw-r--r--   0        0        0     1877 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/jenkins/jenkins.py
--rw-r--r--   0        0        0     1131 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/k3s/__init__.py
--rw-r--r--   0        0        0     1164 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/k3s/k3s.py
--rw-r--r--   0        0        0     3460 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/libsync/animated.gif
--rw-r--r--   0        0        0      571 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/libsync/test.py
--rw-r--r--   0        0        0     4211 2024-04-11 11:06:18.058810 ign8-4.9.8/src/ign8/main.py
--rw-r--r--   0        0        0     4881 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/netbox/__init__.py
--rw-r--r--   0        0        0    55964 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/netbox/netbox.py
--rw-r--r--   0        0        0        9 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/package_data.dat
--rw-r--r--   0        0        0     1370 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/pitv/__init__.py
--rw-r--r--   0        0        0     5822 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/pitv/pitv.py
--rw-r--r--   0        0        0      165 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/podman/__init__.py
--rw-r--r--   0        0        0     3012 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/podman/podman.py
--rw-r--r--   0        0        0      129 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/podman/serve.py
--rw-r--r--   0        0        0      828 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/pypi/__init__.py
--rw-r--r--   0        0        0     1132 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/pypi/pypi.py
--rw-r--r--   0        0        0     6242 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/README.md
--rw-r--r--   0        0        0      764 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/__init__.py
--rw-r--r--   0        0        0       22 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/ansible.cfg
--rwxr-xr-x   0        0        0     2905 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/files/seinfo.sh
--rw-r--r--   0        0        0       22 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/files/selinuxstatus.sh
--rw-r--r--   0        0        0     4343 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/files/testevent.py
--rw-r--r--   0        0        0     6322 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/files/testsetrouble.py
--rwxr-xr-x   0        0        0     3161 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/files/uploadseevent
--rw-r--r--   0        0        0      466 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/inventory
--rw-r--r--   0        0        0      249 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/inventory.new
--rw-r--r--   0        0        0      318 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/meta/main.yml
--rw-r--r--   0        0        0    15063 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/parse.py
--rw-r--r--   0        0        0      225 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/playbook.yml
--rw-r--r--   0        0        0      114 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/roles/requirements.yml
--rw-r--r--   0        0        0        0 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/script.sh
--rw-r--r--   0        0        0     1008 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/setup.py
--rw-r--r--   0        0        0     3986 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/tasks/main copy.yml
--rw-r--r--   0        0        0     4928 2024-01-29 06:08:13.076060 ign8-4.9.8/src/ign8/selinux/tasks/main.yml
--rw-r--r--   0        0        0      894 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/selinux/test.setrouble.py
--rw-r--r--   0        0        0     4343 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/selinux/testevent.py
--rw-r--r--   0        0        0      476 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/selinux/testevent.sh
--rw-r--r--   0        0        0     1234 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/selinux/testsetrouble.json
--rw-r--r--   0        0        0     1242 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/selinux/testsetrouble.small.json
--rw-r--r--   0        0        0      436 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/selinux/upload.sh
--rw-r--r--   0        0        0     1884 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/selinux/uptime.sh
--rw-r--r--   0        0        0      946 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/semaphore/__init__.py
--rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/semaphore/git.py
--rw-r--r--   0        0        0      525 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/semaphore/semaphore.py
--rw-r--r--   0        0        0    11737 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/semaphore/serve.py
--rw-r--r--   0        0        0     1008 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/setup.py
--rw-r--r--   0        0        0      689 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/terraform/__init__.py
--rw-r--r--   0        0        0      664 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/terraform/terraform.py
--rw-r--r--   0        0        0      929 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/traefik/__init__.py
--rw-r--r--   0        0        0     1156 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/traefik/traefik.py
--rw-r--r--   0        0        0       20 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/ui/__init__.py
--rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/ui/firewall.py
--rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/ui/init.py
--rw-r--r--   0        0        0     5841 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/ui/login.py
--rw-r--r--   0        0        0      714 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/ui/logout.py
--rw-r--r--   0        0        0    12288 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/.mail.swp
--rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ansible/__init__.py
--rw-r--r--   0        0        0       63 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ansible/admin.py
--rw-r--r--   0        0        0      146 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ansible/apps.py
--rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ansible/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ansible/models.py
--rw-r--r--   0        0        0       60 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ansible/tests.py
--rw-r--r--   0        0        0       63 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ansible/views.py
--rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/cmdb/__init__.py
--rw-r--r--   0        0        0       63 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/cmdb/admin.py
--rw-r--r--   0        0        0      140 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/cmdb/apps.py
--rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/cmdb/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/cmdb/models.py
--rw-r--r--   0        0        0       60 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/cmdb/tests.py
--rw-r--r--   0        0        0       63 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/cmdb/views.py
--rw-r--r--   0        0        0       34 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/gunicorn.conf
--rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ignite/__init__.py
--rw-r--r--   0        0        0      160 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ignite/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2361 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ignite/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0        0        0     1103 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ignite/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0        0        0      561 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ignite/__pycache__/wsgi.cpython-38.pyc
--rw-r--r--   0        0        0      389 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ignite/asgi.py
--rw-r--r--   0        0        0     4237 2024-02-05 11:00:47.891809 ign8-4.9.8/src/ign8/ui/project/ignite/ignite/settings.py
--rw-r--r--   0        0        0      173 2024-02-05 11:00:47.891809 ign8-4.9.8/src/ign8/ui/project/ignite/ignite/urls.py
--rw-r--r--   0        0        0      389 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/ignite/wsgi.py
--rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/main/__init__.py
--rw-r--r--   0        0        0      158 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/main/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      986 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/main/__pycache__/models.cpython-38.pyc
--rw-r--r--   0        0        0      372 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/main/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0        0        0      493 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/main/__pycache__/views.cpython-38.pyc
--rw-r--r--   0        0        0      343 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/main/admin.py
--rw-r--r--   0        0        0      140 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/main/apps.py
--rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/main/migrations/__init__.py
--rw-r--r--   0        0        0     1261 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/main/models.py
--rw-r--r--   0        0        0     2345 2024-01-29 12:02:52.421302 ign8-4.9.8/src/ign8/ui/project/ignite/main/templates/base.html
--rw-r--r--   0        0        0      692 2024-01-29 12:02:52.421302 ign8-4.9.8/src/ign8/ui/project/ignite/main/templates/main.html
--rw-r--r--   0        0        0      200 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/main/templates/projectdetail.html
--rw-r--r--   0        0        0      705 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/main/templates/projects.html
--rw-r--r--   0        0        0       60 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/main/tests.py
--rw-r--r--   0        0        0      144 2024-02-05 11:00:47.891809 ign8-4.9.8/src/ign8/ui/project/ignite/main/urls.py
--rw-r--r--   0        0        0      872 2024-02-05 11:00:47.891809 ign8-4.9.8/src/ign8/ui/project/ignite/main/views.py
--rwxr-xr-x   0        0        0      662 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/manage.py
--rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/__init__.py
--rw-r--r--   0        0        0      161 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      324 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/__pycache__/admin.cpython-38.pyc
--rw-r--r--   0        0        0      440 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0        0        0     2092 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/__pycache__/models.cpython-38.pyc
--rw-r--r--   0        0        0     1317 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0        0        0      710 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0        0        0     2515 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/__pycache__/views.cpython-38.pyc
--rw-r--r--   0        0        0      243 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/admin.py
--rw-r--r--   0        0        0      146 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/apps.py
--rw-r--r--   0        0        0      178 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/forms.py
--rw-r--r--   0        0        0     3123 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/migrations/__init__.py
--rw-r--r--   0        0        0     1651 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/migrations/__pycache__/0001_initial.cpython-38.pyc
--rw-r--r--   0        0        0      172 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/migrations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6583 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/models.py
--rw-r--r--   0        0        0      226 2024-02-05 11:00:47.895809 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/serializers.py
--rw-r--r--   0        0        0      879 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/SetroubleshootEntry_list.html
--rw-r--r--   0        0        0     2944 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/SetroubleshootEntry_list_full.html
--rw-r--r--   0        0        0     1774 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/base.html
--rw-r--r--   0        0        0      582 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/host_message_sugestion_template.html
--rw-r--r--   0        0        0     1105 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/host_message_template.html
--rw-r--r--   0        0        0      980 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/message_list.html
--rw-r--r--   0        0        0      960 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/selinux_event_list copy.html
--rw-r--r--   0        0        0      960 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/selinux_event_list.html
--rw-r--r--   0        0        0     1870 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/selinux_list.html
--rw-r--r--   0        0        0      687 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/suggestion_list.html
--rw-r--r--   0        0        0       60 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/tests.py
--rw-r--r--   0        0        0      472 2024-02-05 11:00:47.895809 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/urls.py
--rw-r--r--   0        0        0     4380 2024-02-05 11:00:47.895809 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/views.py
--rw-r--r--   0        0        0      297 2024-02-05 11:00:47.895809 ign8-4.9.8/src/ign8/ui/project/ignite/selinux/viewsets.py
--rw-r--r--   0        0        0     1495 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/ignite/templates/nginx.conf.j2
--rw-r--r--   0        0        0       10 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/inventory
--rw-r--r--   0        0        0     1253 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/nginx.conf
--rw-r--r--   0        0        0     1253 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/nginx.conf.j2
--rw-r--r--   0        0        0      530 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/playbook.yml
--rw-r--r--   0        0        0     1494 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/project/testupload.py
--rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/ui/selinux.py
--rw-r--r--   0        0        0      864 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/ui/serve.py
--rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/ui/setup.py
--rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/ui/start.py
--rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/ui/status.py
--rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/ui/stop.py
--rw-r--r--   0        0        0     1972 2024-04-08 05:48:22.393691 ign8-4.9.8/src/ign8/ui/ui.py
--rw-r--r--   0        0        0       72 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vault/__init__.py
--rw-r--r--   0        0        0     1259 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vault/vault.py
--rwxr-xr-x   0        0        0     4534 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/getvmsbycluster.py
--rwxr-xr-x   0        0        0     1800 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/helloworld.py
--rw-r--r--   0        0        0      131 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/requirements.txt
--rw-r--r--   0        0        0      341 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/README.md
--rw-r--r--   0        0        0      659 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/__init__.py
--rw-r--r--   0        0        0      177 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    13573 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     1607 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/__pycache__/service_instance.cpython-311.pyc
--rw-r--r--   0        0        0     5192 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/alarm.py
--rw-r--r--   0        0        0    15650 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/cli.py
--rw-r--r--   0        0        0     1074 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/cluster.py
--rw-r--r--   0        0        0     2679 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/datacenter.py
--rw-r--r--   0        0        0     1687 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/disk.py
--rw-r--r--   0        0        0     3849 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/interactive_wrapper.py
--rw-r--r--   0        0        0     2486 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/pbmhelper.py
--rw-r--r--   0        0        0     4516 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/pchelper.py
--rw-r--r--   0        0        0     1462 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/service_instance.py
--rw-r--r--   0        0        0     4134 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/serviceutil.py
--rw-r--r--   0        0        0     2365 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/tasks.py
--rw-r--r--   0        0        0     1865 2024-01-29 06:08:13.080060 ign8-4.9.8/src/ign8/vmware/tools/vm.py
--rw-r--r--   0        0        0     7429 2024-01-29 06:08:13.084060 ign8-4.9.8/src/ign8/vmware/vmware.py
--rw-r--r--   0        0        0      715 2024-01-29 06:08:13.084060 ign8-4.9.8/src/ign8/wireguard/__init__.py
--rw-r--r--   0        0        0     3053 2024-01-29 06:08:13.084060 ign8-4.9.8/src/ign8/wireguard/wireguard.py
--rw-r--r--   0        0        0     1135 2024-01-29 06:08:13.084060 ign8-4.9.8/src/ign8/zabbix/__init__.py
--rw-r--r--   0        0        0     7797 2024-01-29 06:08:13.084060 ign8-4.9.8/src/ign8/zabbix/zabbix.py
--rw-r--r--   0        0        0     7018 1970-01-01 00:00:00.000000 ign8-4.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-29 06:08:13.072060 ign8-4.9.9/LICENSE.txt
+-rw-r--r--   0        0        0     6071 2024-01-29 06:08:13.072060 ign8-4.9.9/README.md
+-rw-r--r--   0        0        0     2864 2024-04-11 11:09:35.845783 ign8-4.9.9/pyproject.toml
+-rw-r--r--   0        0        0     2700 2024-04-08 07:05:32.385960 ign8-4.9.9/src/ign8/__init__.py
+-rw-r--r--   0        0        0     1492 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/airflow/__init__.py
+-rw-r--r--   0        0        0     5278 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/airflow/airflow.py
+-rw-r--r--   0        0        0     3771 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/awx/__pycache__/awx_common.cpython-311.pyc
+-rw-r--r--   0        0        0     4174 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/awx/__pycache__/awx_credential.cpython-311.pyc
+-rw-r--r--   0        0        0     2864 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/awx/__pycache__/awx_organisation.cpython-311.pyc
+-rw-r--r--   0        0        0     4443 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/awx/__pycache__/awx_project.cpython-311.pyc
+-rw-r--r--   0        0        0     2676 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/awx/awx_common.py
+-rw-r--r--   0        0        0     5230 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/awx/awx_credential.py
+-rw-r--r--   0        0        0     1997 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/awx/awx_executionenvironments.py
+-rw-r--r--   0        0        0     1251 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/awx/awx_hosts.py
+-rw-r--r--   0        0        0     2320 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/awx/awx_organisation.py
+-rw-r--r--   0        0        0     3474 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/awx/awx_project.py
+-rw-r--r--   0        0        0    37171 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/awx/kalm.py
+-rw-r--r--   0        0        0      999 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/bump/__init__.py
+-rw-r--r--   0        0        0     3494 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/bump/bump.py
+-rw-r--r--   0        0        0     4323 2024-04-08 07:11:51.256041 ign8-4.9.9/src/ign8/common.py
+-rw-r--r--   0        0        0     3320 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/dns/__init__.py
+-rw-r--r--   0        0        0     2146 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/dns/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    13524 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/dns/__pycache__/dns.cpython-311.pyc
+-rw-r--r--   0        0        0     4968 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/dns/cloudflare.py
+-rw-r--r--   0        0        0    15599 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/dns/dns.py
+-rw-r--r--   0        0        0      855 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/fiile/__init__.py
+-rw-r--r--   0        0        0      188 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/fiile/file.py
+-rw-r--r--   0        0        0      830 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/gitea/__init__.py
+-rw-r--r--   0        0        0     5396 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/gitea/git.py
+-rw-r--r--   0        0        0    58332 2024-04-08 05:48:22.333690 ign8-4.9.9/src/ign8/homeassistant/after.json
+-rw-r--r--   0        0        0      435 2024-04-08 05:48:22.333690 ign8-4.9.9/src/ign8/homeassistant/after.lst
+-rw-r--r--   0        0        0      132 2024-04-08 05:48:22.333690 ign8-4.9.9/src/ign8/homeassistant/aut.sh
+-rw-r--r--   0        0        0    58332 2024-04-08 05:48:22.333690 ign8-4.9.9/src/ign8/homeassistant/before.json
+-rw-r--r--   0        0        0      435 2024-04-08 05:48:22.333690 ign8-4.9.9/src/ign8/homeassistant/before.lst
+-rw-r--r--   0        0        0       98 2024-04-08 05:48:22.333690 ign8-4.9.9/src/ign8/homeassistant/hue.env
+-rw-r--r--   0        0        0     2680 2024-04-08 05:48:22.333690 ign8-4.9.9/src/ign8/homeassistant/hue.py
+-rw-r--r--   0        0        0     1796 2024-04-08 05:48:22.333690 ign8-4.9.9/src/ign8/homeassistant/hue.test.py
+-rw-r--r--   0        0        0     3944 2024-04-08 05:48:22.333690 ign8-4.9.9/src/ign8/homeassistant/logger.py
+-rw-r--r--   0        0        0 49453399 2024-04-08 05:48:22.389691 ign8-4.9.9/src/ign8/homeassistant/os
+-rw-r--r--   0        0        0      226 2024-04-08 05:48:22.389691 ign8-4.9.9/src/ign8/homeassistant/paused.conf
+-rw-r--r--   0        0        0      419 2024-04-08 05:48:22.389691 ign8-4.9.9/src/ign8/homeassistant/requesttest.py
+-rw-r--r--   0        0        0     5604 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/homeassistant/service.py
+-rw-r--r--   0        0        0     1335 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/homeassistant/servicetest.py
+-rw-r--r--   0        0        0       44 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/homeassistant/start.sh
+-rw-r--r--   0        0        0      447 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/homeassistant/stash.py
+-rw-r--r--   0        0        0    58332 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/homeassistant/test.json
+-rw-r--r--   0        0        0       15 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/homeassistant/test.lst
+-rw-r--r--   0        0        0      604 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/homeassistant/test.lst.org
+-rwxr-xr-x   0        0        0      197 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/homeassistant/test.sh
+-rw-r--r--   0        0        0      783 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/homeassistant/turnontest.py
+-rw-r--r--   0        0        0      153 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/iad/__init__.py
+-rw-r--r--   0        0        0      176 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/iad/iad.py
+-rw-r--r--   0        0        0     1063 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/inabox/__init__.py
+-rw-r--r--   0        0        0    11552 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/inabox/inabox.py
+-rw-r--r--   0        0        0      329 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/inabox/virtlib.py
+-rw-r--r--   0        0        0     1549 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/inthevault/__init__.py
+-rw-r--r--   0        0        0     2454 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/inthevault/inthevault.py
+-rw-r--r--   0        0        0     1415 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/jenkins/__init__.py
+-rw-r--r--   0        0        0     1877 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/jenkins/jenkins.py
+-rw-r--r--   0        0        0     1131 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/k3s/__init__.py
+-rw-r--r--   0        0        0     1164 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/k3s/k3s.py
+-rw-r--r--   0        0        0     3460 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/libsync/animated.gif
+-rw-r--r--   0        0        0      571 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/libsync/test.py
+-rw-r--r--   0        0        0     4204 2024-04-11 11:09:24.837618 ign8-4.9.9/src/ign8/main.py
+-rw-r--r--   0        0        0     4881 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/netbox/__init__.py
+-rw-r--r--   0        0        0    55964 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/netbox/netbox.py
+-rw-r--r--   0        0        0        9 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/package_data.dat
+-rw-r--r--   0        0        0     1370 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/pitv/__init__.py
+-rw-r--r--   0        0        0     5822 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/pitv/pitv.py
+-rw-r--r--   0        0        0      165 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/podman/__init__.py
+-rw-r--r--   0        0        0     3012 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/podman/podman.py
+-rw-r--r--   0        0        0      129 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/podman/serve.py
+-rw-r--r--   0        0        0      828 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/pypi/__init__.py
+-rw-r--r--   0        0        0     1132 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/pypi/pypi.py
+-rw-r--r--   0        0        0     6242 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/README.md
+-rw-r--r--   0        0        0      764 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/__init__.py
+-rw-r--r--   0        0        0       22 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/ansible.cfg
+-rwxr-xr-x   0        0        0     2905 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/files/seinfo.sh
+-rw-r--r--   0        0        0       22 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/files/selinuxstatus.sh
+-rw-r--r--   0        0        0     4343 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/files/testevent.py
+-rw-r--r--   0        0        0     6322 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/files/testsetrouble.py
+-rwxr-xr-x   0        0        0     3161 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/files/uploadseevent
+-rw-r--r--   0        0        0      466 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/inventory
+-rw-r--r--   0        0        0      249 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/inventory.new
+-rw-r--r--   0        0        0      318 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/meta/main.yml
+-rw-r--r--   0        0        0    15063 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/parse.py
+-rw-r--r--   0        0        0      225 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/playbook.yml
+-rw-r--r--   0        0        0      114 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/roles/requirements.yml
+-rw-r--r--   0        0        0        0 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/script.sh
+-rw-r--r--   0        0        0     1008 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/setup.py
+-rw-r--r--   0        0        0     3986 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/tasks/main copy.yml
+-rw-r--r--   0        0        0     4928 2024-01-29 06:08:13.076060 ign8-4.9.9/src/ign8/selinux/tasks/main.yml
+-rw-r--r--   0        0        0      894 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/selinux/test.setrouble.py
+-rw-r--r--   0        0        0     4343 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/selinux/testevent.py
+-rw-r--r--   0        0        0      476 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/selinux/testevent.sh
+-rw-r--r--   0        0        0     1234 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/selinux/testsetrouble.json
+-rw-r--r--   0        0        0     1242 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/selinux/testsetrouble.small.json
+-rw-r--r--   0        0        0      436 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/selinux/upload.sh
+-rw-r--r--   0        0        0     1884 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/selinux/uptime.sh
+-rw-r--r--   0        0        0      946 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/semaphore/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/semaphore/git.py
+-rw-r--r--   0        0        0      525 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/semaphore/semaphore.py
+-rw-r--r--   0        0        0    11737 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/semaphore/serve.py
+-rw-r--r--   0        0        0     1008 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/setup.py
+-rw-r--r--   0        0        0      689 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/terraform/__init__.py
+-rw-r--r--   0        0        0      664 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/terraform/terraform.py
+-rw-r--r--   0        0        0      929 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/traefik/__init__.py
+-rw-r--r--   0        0        0     1156 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/traefik/traefik.py
+-rw-r--r--   0        0        0       20 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/ui/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/ui/firewall.py
+-rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/ui/init.py
+-rw-r--r--   0        0        0     5841 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/ui/login.py
+-rw-r--r--   0        0        0      714 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/ui/logout.py
+-rw-r--r--   0        0        0    12288 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/.mail.swp
+-rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ansible/__init__.py
+-rw-r--r--   0        0        0       63 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ansible/admin.py
+-rw-r--r--   0        0        0      146 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ansible/apps.py
+-rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ansible/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ansible/models.py
+-rw-r--r--   0        0        0       60 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ansible/tests.py
+-rw-r--r--   0        0        0       63 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ansible/views.py
+-rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/cmdb/__init__.py
+-rw-r--r--   0        0        0       63 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/cmdb/admin.py
+-rw-r--r--   0        0        0      140 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/cmdb/apps.py
+-rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/cmdb/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/cmdb/models.py
+-rw-r--r--   0        0        0       60 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/cmdb/tests.py
+-rw-r--r--   0        0        0       63 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/cmdb/views.py
+-rw-r--r--   0        0        0       34 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/gunicorn.conf
+-rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ignite/__init__.py
+-rw-r--r--   0        0        0      160 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ignite/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2361 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ignite/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0        0        0     1103 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ignite/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0        0        0      561 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ignite/__pycache__/wsgi.cpython-38.pyc
+-rw-r--r--   0        0        0      389 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ignite/asgi.py
+-rw-r--r--   0        0        0     4237 2024-02-05 11:00:47.891809 ign8-4.9.9/src/ign8/ui/project/ignite/ignite/settings.py
+-rw-r--r--   0        0        0      173 2024-02-05 11:00:47.891809 ign8-4.9.9/src/ign8/ui/project/ignite/ignite/urls.py
+-rw-r--r--   0        0        0      389 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/ignite/wsgi.py
+-rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/main/__init__.py
+-rw-r--r--   0        0        0      158 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/main/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      986 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/main/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0        0        0      372 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/main/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0        0        0      493 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/main/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0        0        0      343 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/main/admin.py
+-rw-r--r--   0        0        0      140 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/main/apps.py
+-rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/main/migrations/__init__.py
+-rw-r--r--   0        0        0     1261 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/main/models.py
+-rw-r--r--   0        0        0     2345 2024-01-29 12:02:52.421302 ign8-4.9.9/src/ign8/ui/project/ignite/main/templates/base.html
+-rw-r--r--   0        0        0      692 2024-01-29 12:02:52.421302 ign8-4.9.9/src/ign8/ui/project/ignite/main/templates/main.html
+-rw-r--r--   0        0        0      200 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/main/templates/projectdetail.html
+-rw-r--r--   0        0        0      705 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/main/templates/projects.html
+-rw-r--r--   0        0        0       60 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/main/tests.py
+-rw-r--r--   0        0        0      144 2024-02-05 11:00:47.891809 ign8-4.9.9/src/ign8/ui/project/ignite/main/urls.py
+-rw-r--r--   0        0        0      872 2024-02-05 11:00:47.891809 ign8-4.9.9/src/ign8/ui/project/ignite/main/views.py
+-rwxr-xr-x   0        0        0      662 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/manage.py
+-rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/__init__.py
+-rw-r--r--   0        0        0      161 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      324 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/__pycache__/admin.cpython-38.pyc
+-rw-r--r--   0        0        0      440 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0        0        0     2092 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0        0        0     1317 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0        0        0      710 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0        0        0     2515 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0        0        0      243 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/admin.py
+-rw-r--r--   0        0        0      146 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/apps.py
+-rw-r--r--   0        0        0      178 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/forms.py
+-rw-r--r--   0        0        0     3123 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/migrations/__init__.py
+-rw-r--r--   0        0        0     1651 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/migrations/__pycache__/0001_initial.cpython-38.pyc
+-rw-r--r--   0        0        0      172 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/migrations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6583 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/models.py
+-rw-r--r--   0        0        0      226 2024-02-05 11:00:47.895809 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/serializers.py
+-rw-r--r--   0        0        0      879 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/SetroubleshootEntry_list.html
+-rw-r--r--   0        0        0     2944 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/SetroubleshootEntry_list_full.html
+-rw-r--r--   0        0        0     1774 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/base.html
+-rw-r--r--   0        0        0      582 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/host_message_sugestion_template.html
+-rw-r--r--   0        0        0     1105 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/host_message_template.html
+-rw-r--r--   0        0        0      980 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/message_list.html
+-rw-r--r--   0        0        0      960 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/selinux_event_list copy.html
+-rw-r--r--   0        0        0      960 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/selinux_event_list.html
+-rw-r--r--   0        0        0     1870 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/selinux_list.html
+-rw-r--r--   0        0        0      687 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/suggestion_list.html
+-rw-r--r--   0        0        0       60 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/tests.py
+-rw-r--r--   0        0        0      472 2024-02-05 11:00:47.895809 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/urls.py
+-rw-r--r--   0        0        0     4380 2024-02-05 11:00:47.895809 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/views.py
+-rw-r--r--   0        0        0      297 2024-02-05 11:00:47.895809 ign8-4.9.9/src/ign8/ui/project/ignite/selinux/viewsets.py
+-rw-r--r--   0        0        0     1495 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/ignite/templates/nginx.conf.j2
+-rw-r--r--   0        0        0       10 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/inventory
+-rw-r--r--   0        0        0     1253 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/nginx.conf
+-rw-r--r--   0        0        0     1253 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/nginx.conf.j2
+-rw-r--r--   0        0        0      530 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/playbook.yml
+-rw-r--r--   0        0        0     1494 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/project/testupload.py
+-rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/ui/selinux.py
+-rw-r--r--   0        0        0      864 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/ui/serve.py
+-rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/ui/setup.py
+-rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/ui/start.py
+-rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/ui/status.py
+-rw-r--r--   0        0        0      732 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/ui/stop.py
+-rw-r--r--   0        0        0     1972 2024-04-08 05:48:22.393691 ign8-4.9.9/src/ign8/ui/ui.py
+-rw-r--r--   0        0        0       72 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vault/__init__.py
+-rw-r--r--   0        0        0     1259 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vault/vault.py
+-rwxr-xr-x   0        0        0     4534 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/getvmsbycluster.py
+-rwxr-xr-x   0        0        0     1800 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/helloworld.py
+-rw-r--r--   0        0        0      131 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/requirements.txt
+-rw-r--r--   0        0        0      341 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/README.md
+-rw-r--r--   0        0        0      659 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/__init__.py
+-rw-r--r--   0        0        0      177 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    13573 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0        0        0     1607 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/__pycache__/service_instance.cpython-311.pyc
+-rw-r--r--   0        0        0     5192 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/alarm.py
+-rw-r--r--   0        0        0    15650 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/cli.py
+-rw-r--r--   0        0        0     1074 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/cluster.py
+-rw-r--r--   0        0        0     2679 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/datacenter.py
+-rw-r--r--   0        0        0     1687 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/disk.py
+-rw-r--r--   0        0        0     3849 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/interactive_wrapper.py
+-rw-r--r--   0        0        0     2486 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/pbmhelper.py
+-rw-r--r--   0        0        0     4516 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/pchelper.py
+-rw-r--r--   0        0        0     1462 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/service_instance.py
+-rw-r--r--   0        0        0     4134 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/serviceutil.py
+-rw-r--r--   0        0        0     2365 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/tasks.py
+-rw-r--r--   0        0        0     1865 2024-01-29 06:08:13.080060 ign8-4.9.9/src/ign8/vmware/tools/vm.py
+-rw-r--r--   0        0        0     7429 2024-01-29 06:08:13.084060 ign8-4.9.9/src/ign8/vmware/vmware.py
+-rw-r--r--   0        0        0      715 2024-01-29 06:08:13.084060 ign8-4.9.9/src/ign8/wireguard/__init__.py
+-rw-r--r--   0        0        0     3053 2024-01-29 06:08:13.084060 ign8-4.9.9/src/ign8/wireguard/wireguard.py
+-rw-r--r--   0        0        0     1135 2024-01-29 06:08:13.084060 ign8-4.9.9/src/ign8/zabbix/__init__.py
+-rw-r--r--   0        0        0     7797 2024-01-29 06:08:13.084060 ign8-4.9.9/src/ign8/zabbix/zabbix.py
+-rw-r--r--   0        0        0     7018 1970-01-01 00:00:00.000000 ign8-4.9.9/PKG-INFO
```

### Comparing `ign8-4.9.8/LICENSE.txt` & `ign8-4.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/README.md` & `ign8-4.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/pyproject.toml` & `ign8-4.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ign8"
-version = "4.9.8"
+version = "4.9.9"
 description = "Knowit automation lifecycle management"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = [ "ign8", "awx", "ansible", "automation",]
 classifiers = [ "Development Status :: 3 - Alpha", "Intended Audience :: Developers", "Topic :: Software Development :: Libraries :: Python Modules", "License :: OSI Approved :: MIT License", "Programming Language :: Python :: 3",]
 dependencies = [ "redis", "flask", "psutil", "pynetbox", "wheel", "hvac", "xmltodict", "netbox", "urllib3", "cryptography", "PyYAML", "toml", "django", "djangorestframework", "gunicorn", "ansible", "ansible-core", "paramiko",]
 [[project.authors]]
@@ -51,15 +51,15 @@
 ign8_traefik = "ign8.traefik:main"
 ign8_ui = "ign8.ui:main"
 ign8_vault = "ign8.vault:main"
 ign8_zabbix = "ign8.zabbix:main"
 
 [tool.poetry]
 name = "ign8"
-version = "4.9.8"
+version = "4.9.9"
 description = "Ignite it all."
 readme = "README.md"
 authors = [ "Jakob Holst <jakob.holst@knowit.dk>",]
 license = "MIT"
 homepage = "https://ign8.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_ign8.git"
```

### Comparing `ign8-4.9.8/src/ign8/__init__.py` & `ign8-4.9.9/src/ign8/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/airflow/__init__.py` & `ign8-4.9.9/src/ign8/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/airflow/airflow.py` & `ign8-4.9.9/src/ign8/airflow/airflow.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/awx/__pycache__/awx_common.cpython-311.pyc` & `ign8-4.9.9/src/ign8/awx/__pycache__/awx_common.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/awx/__pycache__/awx_credential.cpython-311.pyc` & `ign8-4.9.9/src/ign8/awx/__pycache__/awx_credential.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/awx/__pycache__/awx_organisation.cpython-311.pyc` & `ign8-4.9.9/src/ign8/awx/__pycache__/awx_organisation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/awx/__pycache__/awx_project.cpython-311.pyc` & `ign8-4.9.9/src/ign8/awx/__pycache__/awx_project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/awx/awx_common.py` & `ign8-4.9.9/src/ign8/awx/awx_common.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/awx/awx_credential.py` & `ign8-4.9.9/src/ign8/awx/awx_credential.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/awx/awx_executionenvironments.py` & `ign8-4.9.9/src/ign8/awx/awx_executionenvironments.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/awx/awx_hosts.py` & `ign8-4.9.9/src/ign8/awx/awx_hosts.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/awx/awx_organisation.py` & `ign8-4.9.9/src/ign8/awx/awx_organisation.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/awx/awx_project.py` & `ign8-4.9.9/src/ign8/awx/awx_project.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/awx/kalm.py` & `ign8-4.9.9/src/ign8/awx/kalm.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/bump/__init__.py` & `ign8-4.9.9/src/ign8/bump/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/bump/bump.py` & `ign8-4.9.9/src/ign8/bump/bump.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/common.py` & `ign8-4.9.9/src/ign8/common.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/dns/__init__.py` & `ign8-4.9.9/src/ign8/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/dns/__pycache__/__init__.cpython-311.pyc` & `ign8-4.9.9/src/ign8/dns/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/dns/__pycache__/dns.cpython-311.pyc` & `ign8-4.9.9/src/ign8/dns/__pycache__/dns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/dns/cloudflare.py` & `ign8-4.9.9/src/ign8/dns/cloudflare.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/dns/dns.py` & `ign8-4.9.9/src/ign8/dns/dns.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/fiile/__init__.py` & `ign8-4.9.9/src/ign8/fiile/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/gitea/__init__.py` & `ign8-4.9.9/src/ign8/gitea/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/gitea/git.py` & `ign8-4.9.9/src/ign8/gitea/git.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/homeassistant/after.json` & `ign8-4.9.9/src/ign8/homeassistant/after.json`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/homeassistant/before.json` & `ign8-4.9.9/src/ign8/homeassistant/before.json`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/homeassistant/hue.py` & `ign8-4.9.9/src/ign8/homeassistant/hue.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/homeassistant/hue.test.py` & `ign8-4.9.9/src/ign8/homeassistant/hue.test.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/homeassistant/logger.py` & `ign8-4.9.9/src/ign8/homeassistant/logger.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/homeassistant/os` & `ign8-4.9.9/src/ign8/homeassistant/os`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/homeassistant/service.py` & `ign8-4.9.9/src/ign8/homeassistant/service.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/homeassistant/servicetest.py` & `ign8-4.9.9/src/ign8/homeassistant/servicetest.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/homeassistant/test.json` & `ign8-4.9.9/src/ign8/homeassistant/test.json`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/homeassistant/test.lst.org` & `ign8-4.9.9/src/ign8/homeassistant/test.lst.org`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/homeassistant/turnontest.py` & `ign8-4.9.9/src/ign8/homeassistant/turnontest.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/inabox/__init__.py` & `ign8-4.9.9/src/ign8/inabox/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/inabox/inabox.py` & `ign8-4.9.9/src/ign8/inabox/inabox.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/inthevault/__init__.py` & `ign8-4.9.9/src/ign8/inthevault/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/inthevault/inthevault.py` & `ign8-4.9.9/src/ign8/inthevault/inthevault.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/jenkins/__init__.py` & `ign8-4.9.9/src/ign8/jenkins/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/jenkins/jenkins.py` & `ign8-4.9.9/src/ign8/jenkins/jenkins.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/k3s/__init__.py` & `ign8-4.9.9/src/ign8/k3s/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/k3s/k3s.py` & `ign8-4.9.9/src/ign8/k3s/k3s.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/libsync/animated.gif` & `ign8-4.9.9/src/ign8/libsync/animated.gif`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/libsync/test.py` & `ign8-4.9.9/src/ign8/libsync/test.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/main.py` & `ign8-4.9.9/src/ign8/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,16 @@
     prettylog("INFO", f"Reading DNS TXT record for {domain}")
     result = subprocess.run(command, capture_output=True, shell=True)
     if result.returncode == 0:
         output = result.stdout.decode()
         start_index = output.find('"')
         end_index = output.rfind('"')
         txt_record = output[start_index:end_index + 1]
-        pprint.pprint(txt_record)
-
-        # Convert the TXT record to a dictionary
-        txt_dict = json.loads(txt_record)
+        txt_record_cleaned = txt_record.strip('"').replace('\\', '')
+        txt_dict = json.loads(txt_record_cleaned)
         return txt_dict
     else:
         prettylog("ERROR", f"Error reading DNS TXT record for {domain}")
         return False
     
 
 def cloudflare():
```

### Comparing `ign8-4.9.8/src/ign8/netbox/__init__.py` & `ign8-4.9.9/src/ign8/netbox/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/netbox/netbox.py` & `ign8-4.9.9/src/ign8/netbox/netbox.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/pitv/__init__.py` & `ign8-4.9.9/src/ign8/pitv/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/pitv/pitv.py` & `ign8-4.9.9/src/ign8/pitv/pitv.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/podman/podman.py` & `ign8-4.9.9/src/ign8/podman/podman.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/pypi/__init__.py` & `ign8-4.9.9/src/ign8/pypi/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/pypi/pypi.py` & `ign8-4.9.9/src/ign8/pypi/pypi.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/README.md` & `ign8-4.9.9/src/ign8/selinux/README.md`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/__init__.py` & `ign8-4.9.9/src/ign8/selinux/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/files/seinfo.sh` & `ign8-4.9.9/src/ign8/selinux/files/seinfo.sh`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/files/testevent.py` & `ign8-4.9.9/src/ign8/selinux/files/testevent.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/files/testsetrouble.py` & `ign8-4.9.9/src/ign8/selinux/files/testsetrouble.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/files/uploadseevent` & `ign8-4.9.9/src/ign8/selinux/files/uploadseevent`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/parse.py` & `ign8-4.9.9/src/ign8/selinux/parse.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/setup.py` & `ign8-4.9.9/src/ign8/selinux/setup.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/tasks/main copy.yml` & `ign8-4.9.9/src/ign8/selinux/tasks/main copy.yml`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/tasks/main.yml` & `ign8-4.9.9/src/ign8/selinux/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/test.setrouble.py` & `ign8-4.9.9/src/ign8/selinux/test.setrouble.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/testevent.py` & `ign8-4.9.9/src/ign8/selinux/testevent.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/testsetrouble.json` & `ign8-4.9.9/src/ign8/selinux/testsetrouble.json`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/testsetrouble.small.json` & `ign8-4.9.9/src/ign8/selinux/testsetrouble.small.json`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/selinux/uptime.sh` & `ign8-4.9.9/src/ign8/selinux/uptime.sh`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/semaphore/__init__.py` & `ign8-4.9.9/src/ign8/semaphore/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/semaphore/semaphore.py` & `ign8-4.9.9/src/ign8/semaphore/semaphore.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/semaphore/serve.py` & `ign8-4.9.9/src/ign8/semaphore/serve.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/setup.py` & `ign8-4.9.9/src/ign8/setup.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/terraform/__init__.py` & `ign8-4.9.9/src/ign8/terraform/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/terraform/terraform.py` & `ign8-4.9.9/src/ign8/terraform/terraform.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/traefik/__init__.py` & `ign8-4.9.9/src/ign8/traefik/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/traefik/traefik.py` & `ign8-4.9.9/src/ign8/traefik/traefik.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/firewall.py` & `ign8-4.9.9/src/ign8/ui/firewall.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/init.py` & `ign8-4.9.9/src/ign8/ui/init.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/login.py` & `ign8-4.9.9/src/ign8/ui/login.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/logout.py` & `ign8-4.9.9/src/ign8/ui/logout.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/.mail.swp` & `ign8-4.9.9/src/ign8/ui/project/ignite/.mail.swp`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/ignite/__pycache__/settings.cpython-38.pyc` & `ign8-4.9.9/src/ign8/ui/project/ignite/ignite/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/ignite/__pycache__/urls.cpython-38.pyc` & `ign8-4.9.9/src/ign8/ui/project/ignite/ignite/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/ignite/__pycache__/wsgi.cpython-38.pyc` & `ign8-4.9.9/src/ign8/ui/project/ignite/ignite/__pycache__/wsgi.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/ignite/settings.py` & `ign8-4.9.9/src/ign8/ui/project/ignite/ignite/settings.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/main/__pycache__/models.cpython-38.pyc` & `ign8-4.9.9/src/ign8/ui/project/ignite/main/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/main/models.py` & `ign8-4.9.9/src/ign8/ui/project/ignite/main/models.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/main/templates/base.html` & `ign8-4.9.9/src/ign8/ui/project/ignite/main/templates/base.html`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/main/templates/main.html` & `ign8-4.9.9/src/ign8/ui/project/ignite/main/templates/main.html`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/main/templates/projects.html` & `ign8-4.9.9/src/ign8/ui/project/ignite/main/templates/projects.html`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/main/views.py` & `ign8-4.9.9/src/ign8/ui/project/ignite/main/views.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/manage.py` & `ign8-4.9.9/src/ign8/ui/project/ignite/manage.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/__pycache__/models.cpython-38.pyc` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/__pycache__/serializers.cpython-38.pyc` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/__pycache__/serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/__pycache__/urls.cpython-38.pyc` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/__pycache__/views.cpython-38.pyc` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/migrations/0001_initial.py` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/migrations/__pycache__/0001_initial.cpython-38.pyc` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/migrations/__pycache__/0001_initial.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/models.py` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/models.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/SetroubleshootEntry_list.html` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/SetroubleshootEntry_list.html`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/SetroubleshootEntry_list_full.html` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/SetroubleshootEntry_list_full.html`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/base.html` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/base.html`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/host_message_sugestion_template.html` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/host_message_sugestion_template.html`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/host_message_template.html` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/host_message_template.html`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/message_list.html` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/message_list.html`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/selinux_event_list copy.html` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/selinux_event_list copy.html`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/selinux_event_list.html` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/selinux_event_list.html`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/selinux_list.html` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/selinux_list.html`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/templates/suggestion_list.html` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/templates/suggestion_list.html`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/selinux/views.py` & `ign8-4.9.9/src/ign8/ui/project/ignite/selinux/views.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/ignite/templates/nginx.conf.j2` & `ign8-4.9.9/src/ign8/ui/project/ignite/templates/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/nginx.conf` & `ign8-4.9.9/src/ign8/ui/project/nginx.conf`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/nginx.conf.j2` & `ign8-4.9.9/src/ign8/ui/project/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/playbook.yml` & `ign8-4.9.9/src/ign8/ui/project/playbook.yml`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/project/testupload.py` & `ign8-4.9.9/src/ign8/ui/project/testupload.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/selinux.py` & `ign8-4.9.9/src/ign8/ui/selinux.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/serve.py` & `ign8-4.9.9/src/ign8/ui/serve.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/setup.py` & `ign8-4.9.9/src/ign8/ui/setup.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/start.py` & `ign8-4.9.9/src/ign8/ui/start.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/status.py` & `ign8-4.9.9/src/ign8/ui/status.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/stop.py` & `ign8-4.9.9/src/ign8/ui/stop.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/ui/ui.py` & `ign8-4.9.9/src/ign8/ui/ui.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vault/vault.py` & `ign8-4.9.9/src/ign8/vault/vault.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/getvmsbycluster.py` & `ign8-4.9.9/src/ign8/vmware/getvmsbycluster.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/helloworld.py` & `ign8-4.9.9/src/ign8/vmware/helloworld.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/__init__.py` & `ign8-4.9.9/src/ign8/vmware/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/__pycache__/cli.cpython-311.pyc` & `ign8-4.9.9/src/ign8/vmware/tools/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/__pycache__/service_instance.cpython-311.pyc` & `ign8-4.9.9/src/ign8/vmware/tools/__pycache__/service_instance.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/alarm.py` & `ign8-4.9.9/src/ign8/vmware/tools/alarm.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/cli.py` & `ign8-4.9.9/src/ign8/vmware/tools/cli.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/cluster.py` & `ign8-4.9.9/src/ign8/vmware/tools/cluster.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/datacenter.py` & `ign8-4.9.9/src/ign8/vmware/tools/datacenter.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/disk.py` & `ign8-4.9.9/src/ign8/vmware/tools/disk.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/interactive_wrapper.py` & `ign8-4.9.9/src/ign8/vmware/tools/interactive_wrapper.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/pbmhelper.py` & `ign8-4.9.9/src/ign8/vmware/tools/pbmhelper.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/pchelper.py` & `ign8-4.9.9/src/ign8/vmware/tools/pchelper.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/service_instance.py` & `ign8-4.9.9/src/ign8/vmware/tools/service_instance.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/serviceutil.py` & `ign8-4.9.9/src/ign8/vmware/tools/serviceutil.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/tasks.py` & `ign8-4.9.9/src/ign8/vmware/tools/tasks.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/tools/vm.py` & `ign8-4.9.9/src/ign8/vmware/tools/vm.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/vmware/vmware.py` & `ign8-4.9.9/src/ign8/vmware/vmware.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/wireguard/__init__.py` & `ign8-4.9.9/src/ign8/wireguard/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/wireguard/wireguard.py` & `ign8-4.9.9/src/ign8/wireguard/wireguard.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/zabbix/__init__.py` & `ign8-4.9.9/src/ign8/zabbix/__init__.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/src/ign8/zabbix/zabbix.py` & `ign8-4.9.9/src/ign8/zabbix/zabbix.py`

 * *Files identical despite different names*

### Comparing `ign8-4.9.8/PKG-INFO` & `ign8-4.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ign8
-Version: 4.9.8
+Version: 4.9.9
 Summary: Ignite it all.
 Home-page: https://ign8.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
```

