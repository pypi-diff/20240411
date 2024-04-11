# Comparing `tmp/djangoldp_energiepartagee-1.2.9.tar.gz` & `tmp/djangoldp_energiepartagee-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_energiepartagee-1.2.9.tar", last modified: Wed Mar 27 18:15:20 2024, max compression
+gzip compressed data, was "dist/djangoldp_energiepartagee-2.0.0.tar", last modified: Thu Apr 11 16:57:25 2024, max compression
```

## Comparing `djangoldp_energiepartagee-1.2.9.tar` & `djangoldp_energiepartagee-2.0.0.tar`

### file list

```diff
@@ -1,222 +1,229 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/
--rw-rw-rw-   0 root         (0) root         (0)     2337 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      623 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2608 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2608 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)    11812 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/tests/
--rw-rw-rw-   0 root         (0) root         (0)    48719 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/tests/tests_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9483 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/tests/tests_post.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/oidc_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      353 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/registration/password_reset_email.html
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1347 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/registration/login.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/waiting_reminder.html
--rw-rw-rw-   0 root         (0) root         (0)     3630 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/actor_update.html
--rw-rw-rw-   0 root         (0) root         (0)     2455 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/new_join_request.html
--rw-rw-rw-   0 root         (0) root         (0)     3839 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/subscription_call.html
--rw-rw-rw-   0 root         (0) root         (0)     2615 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/join_actor_validated.html
--rw-rw-rw-   0 root         (0) root         (0)     3196 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/subscription_reminder.html
--rw-rw-rw-   0 root         (0) root         (0)     2429 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/join_actor_denied.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/txt/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/txt/actor_update.txt
--rw-rw-rw-   0 root         (0) root         (0)     1410 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/txt/subscription_call.txt
--rw-rw-rw-   0 root         (0) root         (0)      277 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/txt/waiting_reminder.txt
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/txt/new_join_request.txt
--rw-rw-rw-   0 root         (0) root         (0)      318 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/txt/join_actor_denied.txt
--rw-rw-rw-   0 root         (0) root         (0)     1022 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/txt/subscription_reminder.txt
--rw-rw-rw-   0 root         (0) root         (0)      450 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/txt/join_actor_validated.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)      766 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/oidc_provider/authorize.html
--rw-rw-rw-   0 root         (0) root         (0)     1161 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/django_registration/activation_email_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/django_registration/activation_email_body.txt
--rw-rw-rw-   0 root         (0) root         (0)      517 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/django_registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     2662 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/django_registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      378 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/django_registration/registration_complete.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/pdf/
--rw-rw-rw-   0 root         (0) root         (0)     4778 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/pdf/contribution_receipt.html
--rw-rw-rw-   0 root         (0) root         (0)     7355 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/pdf/contribution_call.html
--rw-rw-rw-   0 root         (0) root         (0)     2625 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2074 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-03-27 18:15:17.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/filters/
--rw-rw-rw-   0 root         (0) root         (0)      725 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/filters/related_actor_filter_backend.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/filters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      805 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/filters/contribution_filter_backend.py
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/css/
--rw-rw-rw-   0 root         (0) root         (0)     4344 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/css/registration.css
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/css/css_ep.css
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/css/css_amorce.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   224744 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/fonts/Inter-roman.var.woff2
--rw-rw-rw-   0 root         (0) root         (0)   240240 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/fonts/Inter-italic.var.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/img/
--rw-rw-rw-   0 root         (0) root         (0)    12656 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/img/Amorcelogo.svg
--rw-rw-rw-   0 root         (0) root         (0)     4916 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/img/EPlogo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/
--rw-rw-rw-   0 root         (0) root         (0)    18219 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/export_contributions_all.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/contributions_call.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/generate_pdf_receipt.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/plain_text_parser.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/contributions_reminder.py
--rw-rw-rw-   0 root         (0) root         (0)    18343 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/export_contributions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/utils/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/utils/render_to_pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     5825 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/waiting_members_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12008 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/contributions.py
--rw-rw-rw-   0 root         (0) root         (0)     1491 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/related_actor.py
--rw-rw-rw-   0 root         (0) root         (0)     3051 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/contributions_ventilation.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/contributions_actor_update.py
--rw-rw-rw-   0 root         (0) root         (0)     2361 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/generate_pdf_call.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/permissions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/permissions/generic_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/permissions/actor_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/permissions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/permissions/related_actor_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1532 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/permissions/contribution_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/auth/
--rw-rw-rw-   0 root         (0) root         (0)     1697 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/auth/backends.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/djangoldp_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      903 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0014_auto_20210121_1750.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0065_auto_20220302_1533.py
--rw-rw-rw-   0 root         (0) root         (0)      724 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0045_auto_20210222_2353.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0039_auto_20210216_1732.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0019_auto_20210124_1728.py
--rw-rw-rw-   0 root         (0) root         (0)     5894 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0082_alter_capitaldistribution_actor_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      692 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0055_auto_20210421_1500.py
--rw-rw-rw-   0 root         (0) root         (0)    19750 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0043_auto_20210219_1412.py
--rw-rw-rw-   0 root         (0) root         (0)     5436 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0076_alter_actor_options_alter_college_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      672 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0050_contribution_usercontact.py
--rw-rw-rw-   0 root         (0) root         (0)    10724 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0015_auto_20210122_1044.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0081_alter_citizenproject_status.py
--rw-rw-rw-   0 root         (0) root         (0)     4132 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0025_auto_20210129_1841.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0068_contribution_discount.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0072_alter_relatedactor_role.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0021_auto_20210125_1559.py
--rw-rw-rw-   0 root         (0) root         (0)     4527 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0007_auto_20210120_1213.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0032_auto_20210209_1238.py
--rw-rw-rw-   0 root         (0) root         (0)      740 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0070_contribution_updatereminderdate_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0058_auto_20211108_1909.py
--rw-rw-rw-   0 root         (0) root         (0)      691 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0009_auto_20210120_1439.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0059_auto_20220114_1050.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0073_relatedactor_reminderdate.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0084_citizenproject_postcode.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0013_merge_20210120_1916.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0048_auto_20210225_1136.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0085_citizenproject_wp_project_url_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0009_auto_20210120_1911.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0051_auto_20210323_1356.py
--rw-rw-rw-   0 root         (0) root         (0)     1201 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0011_auto_20210120_1450.py
--rw-rw-rw-   0 root         (0) root         (0)      972 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0031_auto_20210209_1235.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0071_relatedactor_createdate.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0077_alter_discount_options.py
--rw-rw-rw-   0 root         (0) root         (0)     5837 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0062_auto_20220128_1047.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0052_auto_20210323_1424.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0003_profile_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0053_auto_20210402_1014.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0030_contribution_contributionnumber.py
--rw-rw-rw-   0 root         (0) root         (0)      944 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0040_auto_20210216_2227.py
--rw-rw-rw-   0 root         (0) root         (0)     1518 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0061_auto_20220114_1140.py
--rw-rw-rw-   0 root         (0) root         (0)      362 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0002_auto_20210114_1101.py
--rw-rw-rw-   0 root         (0) root         (0)     1392 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0016_auto_20210122_1146.py
--rw-rw-rw-   0 root         (0) root         (0)     1034 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0060_auto_20220114_1113.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0027_auto_20210201_1617.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0004_auto_20210114_1652.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0022_auto_20210125_1606.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0080_alter_citizenproject_status.py
--rw-rw-rw-   0 root         (0) root         (0)      582 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0024_auto_20210125_2207.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0044_auto_20210219_1415.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0057_actor_visible.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0041_regionalnetwork_nationale.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0049_actor_updatedate.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0067_discount_actor_villageoise.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0017_actor_iban.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0012_auto_20210120_1553.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0035_auto_20210215_1329.py
--rw-rw-rw-   0 root         (0) root         (0)      746 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0047_auto_20210223_1059.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0038_auto_20210216_1721.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0063_auto_20220128_1051.py
--rw-rw-rw-   0 root         (0) root         (0)    54205 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0078_citizen_project_communication_profile_contract_type_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0006_auto_20210119_1237.py
--rw-rw-rw-   0 root         (0) root         (0)     3904 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0066_alter_actor_options_alter_college_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0010_auto_20210120_1442.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0036_auto_20210216_1714.py
--rw-rw-rw-   0 root         (0) root         (0)     1204 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0056_auto_20210430_1127.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0079_rename_capital_distribution_capitaldistribution_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      597 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0037_auto_20210216_1717.py
--rw-rw-rw-   0 root         (0) root         (0)    11607 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0083_alter_actor_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0075_alter_actor_visible.py
--rw-rw-rw-   0 root         (0) root         (0)     3246 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0005_auto_20210118_1407.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0064_auto_20220203_1721.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0029_auto_20210204_1428.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0023_auto_20210125_1646.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0074_alter_relatedactor_role.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0069_region_acronym.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0042_auto_20210219_1409.py
--rw-rw-rw-   0 root         (0) root         (0)      852 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0028_auto_20210202_1625.py
--rw-rw-rw-   0 root         (0) root         (0)      926 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0033_auto_20210209_1258.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0046_auto_20210223_1052.py
--rw-rw-rw-   0 root         (0) root         (0)      589 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0034_auto_20210209_1538.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0008_auto_20210120_1215.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0026_auto_20210201_1343.py
--rw-rw-rw-   0 root         (0) root         (0)     2185 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0018_auto_20210122_1229.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0020_auto_20210125_1131.py
--rw-rw-rw-   0 root         (0) root         (0)      692 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0054_auto_20210419_2106.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 18:15:20.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/
--rw-rw-rw-   0 root         (0) root         (0)     2140 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/communication_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     9764 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/actor.py
--rw-rw-rw-   0 root         (0) root         (0)     7013 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/contribution.py
--rw-rw-rw-   0 root         (0) root         (0)     3613 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/production_site.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/college.py
--rw-rw-rw-   0 root         (0) root         (0)     2972 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/capital_distribution.py
--rw-rw-rw-   0 root         (0) root         (0)      808 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/region.py
--rw-rw-rw-   0 root         (0) root         (0)      680 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/energy_buyer_type.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/college_epa.py
--rw-rw-rw-   0 root         (0) root         (0)     3642 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/regional_network.py
--rw-rw-rw-   0 root         (0) root         (0)     2755 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/energy_production.py
--rw-rw-rw-   0 root         (0) root         (0)     4709 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/citizen_project.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/testimony.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/intervention_zone.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/citizen_project_distinction.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/energy_buyer.py
--rw-rw-rw-   0 root         (0) root         (0)     1511 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/shareholder.py
--rw-rw-rw-   0 root         (0) root         (0)      756 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/legal_structure.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/partner_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3425 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/related_actor.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/partner_link.py
--rw-rw-rw-   0 root         (0) root         (0)     1650 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1080 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/partner.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/energy_type.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/payment_method.py
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/discount.py
--rw-rw-rw-   0 root         (0) root         (0)     7221 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/signals.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/integration_step.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-03-27 18:14:59.000000 djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/context_processors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      623 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2608 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2608 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)    12430 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    51152 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/tests/tests_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10086 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/tests/tests_post.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2232 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/oidc_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/registration/login.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/waiting_reminder.html
+-rw-rw-rw-   0 root         (0) root         (0)     3630 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/actor_update.html
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/new_join_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     3839 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/subscription_call.html
+-rw-rw-rw-   0 root         (0) root         (0)     2615 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/join_actor_validated.html
+-rw-rw-rw-   0 root         (0) root         (0)     3196 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/subscription_reminder.html
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/join_actor_denied.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/txt/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/txt/actor_update.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/txt/subscription_call.txt
+-rw-rw-rw-   0 root         (0) root         (0)      277 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/txt/waiting_reminder.txt
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/txt/new_join_request.txt
+-rw-rw-rw-   0 root         (0) root         (0)      318 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/txt/join_actor_denied.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/txt/subscription_reminder.txt
+-rw-rw-rw-   0 root         (0) root         (0)      450 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/txt/join_actor_validated.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)      766 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/oidc_provider/authorize.html
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/django_registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/django_registration/activation_email_body.txt
+-rw-rw-rw-   0 root         (0) root         (0)      517 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/django_registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     2662 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/django_registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/django_registration/registration_complete.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/pdf/
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/pdf/contribution_receipt.html
+-rw-rw-rw-   0 root         (0) root         (0)     7355 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/pdf/contribution_call.html
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2074 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-04-11 16:57:22.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/filters/
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/filters/related_actor_filter_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/filters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/filters/contribution_filter_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)     4344 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/css/registration.css
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/css/css_ep.css
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/css/css_amorce.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   224744 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/fonts/Inter-roman.var.woff2
+-rw-rw-rw-   0 root         (0) root         (0)   240240 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/fonts/Inter-italic.var.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)    12656 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/img/Amorcelogo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4916 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/img/EPlogo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/
+-rw-rw-rw-   0 root         (0) root         (0)    18245 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/export_contributions_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/contributions_call.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/generate_pdf_receipt.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/plain_text_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/contributions_reminder.py
+-rw-rw-rw-   0 root         (0) root         (0)    18367 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/export_contributions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/utils/render_to_pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5917 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/waiting_members_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12008 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/contributions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/contributions_ventilation.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/contributions_actor_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     2361 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/generate_pdf_call.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/permissions/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/permissions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/permissions/ep_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2905 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/permissions/ep_related_actor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/permissions/ep_contribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/permissions/ep_actor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/permissions/ep_regional_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/auth/
+-rw-rw-rw-   0 root         (0) root         (0)     1810 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/auth/backends.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/djangoldp_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      903 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0014_auto_20210121_1750.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0065_auto_20220302_1533.py
+-rw-rw-rw-   0 root         (0) root         (0)      724 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0045_auto_20210222_2353.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0039_auto_20210216_1732.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0019_auto_20210124_1728.py
+-rw-rw-rw-   0 root         (0) root         (0)     5894 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0082_alter_capitaldistribution_actor_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      692 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0055_auto_20210421_1500.py
+-rw-rw-rw-   0 root         (0) root         (0)    19750 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0043_auto_20210219_1412.py
+-rw-rw-rw-   0 root         (0) root         (0)     5436 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0076_alter_actor_options_alter_college_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0050_contribution_usercontact.py
+-rw-rw-rw-   0 root         (0) root         (0)    10724 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0015_auto_20210122_1044.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0081_alter_citizenproject_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0025_auto_20210129_1841.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0068_contribution_discount.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0072_alter_relatedactor_role.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0086_alter_productionsite_total_development_budget_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0021_auto_20210125_1559.py
+-rw-rw-rw-   0 root         (0) root         (0)     4527 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0007_auto_20210120_1213.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0088_alter_energyproduction_consumption_equivalence_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0032_auto_20210209_1238.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0087_alter_productionsite_progress_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0070_contribution_updatereminderdate_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0058_auto_20211108_1909.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0009_auto_20210120_1439.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0059_auto_20220114_1050.py
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0090_productionsite_postcode.py
+-rw-rw-rw-   0 root         (0) root         (0)      463 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0073_relatedactor_reminderdate.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0084_citizenproject_postcode.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0013_merge_20210120_1916.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0048_auto_20210225_1136.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0085_citizenproject_wp_project_url_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0009_auto_20210120_1911.py
+-rw-rw-rw-   0 root         (0) root         (0)      404 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0051_auto_20210323_1356.py
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0011_auto_20210120_1450.py
+-rw-rw-rw-   0 root         (0) root         (0)      972 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0031_auto_20210209_1235.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0071_relatedactor_createdate.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0077_alter_discount_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     5837 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0062_auto_20220128_1047.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0052_auto_20210323_1424.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0003_profile_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0053_auto_20210402_1014.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0030_contribution_contributionnumber.py
+-rw-rw-rw-   0 root         (0) root         (0)      944 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0040_auto_20210216_2227.py
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0061_auto_20220114_1140.py
+-rw-rw-rw-   0 root         (0) root         (0)      362 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0002_auto_20210114_1101.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0089_rename_effective_commissionning_yearl_productionsite_effective_commissionning_year_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1392 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0016_auto_20210122_1146.py
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0060_auto_20220114_1113.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0027_auto_20210201_1617.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0004_auto_20210114_1652.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0022_auto_20210125_1606.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0080_alter_citizenproject_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      582 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0024_auto_20210125_2207.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0090_region_admins.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0044_auto_20210219_1415.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0057_actor_visible.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0041_regionalnetwork_nationale.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0049_actor_updatedate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0067_discount_actor_villageoise.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0017_actor_iban.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0012_auto_20210120_1553.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0035_auto_20210215_1329.py
+-rw-rw-rw-   0 root         (0) root         (0)      746 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0047_auto_20210223_1059.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0038_auto_20210216_1721.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0063_auto_20220128_1051.py
+-rw-rw-rw-   0 root         (0) root         (0)    54205 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0078_citizen_project_communication_profile_contract_type_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0006_auto_20210119_1237.py
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0066_alter_actor_options_alter_college_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0010_auto_20210120_1442.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0036_auto_20210216_1714.py
+-rw-rw-rw-   0 root         (0) root         (0)     1204 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0056_auto_20210430_1127.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0079_rename_capital_distribution_capitaldistribution_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      597 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0037_auto_20210216_1717.py
+-rw-rw-rw-   0 root         (0) root         (0)    11607 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0083_alter_actor_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0075_alter_actor_visible.py
+-rw-rw-rw-   0 root         (0) root         (0)     3246 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0005_auto_20210118_1407.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0064_auto_20220203_1721.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0029_auto_20210204_1428.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0023_auto_20210125_1646.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0074_alter_relatedactor_role.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0069_region_acronym.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0042_auto_20210219_1409.py
+-rw-rw-rw-   0 root         (0) root         (0)      852 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0028_auto_20210202_1625.py
+-rw-rw-rw-   0 root         (0) root         (0)      926 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0033_auto_20210209_1258.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0046_auto_20210223_1052.py
+-rw-rw-rw-   0 root         (0) root         (0)      305 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0091_merge_0090_productionsite_postcode_0090_region_admins.py
+-rw-rw-rw-   0 root         (0) root         (0)      589 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0034_auto_20210209_1538.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0008_auto_20210120_1215.py
+-rw-rw-rw-   0 root         (0) root         (0)      787 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0026_auto_20210201_1343.py
+-rw-rw-rw-   0 root         (0) root         (0)     2185 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0018_auto_20210122_1229.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0020_auto_20210125_1131.py
+-rw-rw-rw-   0 root         (0) root         (0)      692 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0054_auto_20210419_2106.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:57:25.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/communication_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)    10065 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/actor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7080 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/contribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/production_site.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/college.py
+-rw-rw-rw-   0 root         (0) root         (0)     2993 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/capital_distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/region.py
+-rw-rw-rw-   0 root         (0) root         (0)      680 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/energy_buyer_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/college_epa.py
+-rw-rw-rw-   0 root         (0) root         (0)     3642 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/regional_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     2816 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/energy_production.py
+-rw-rw-rw-   0 root         (0) root         (0)     4910 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/citizen_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/testimony.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/intervention_zone.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/citizen_project_distinction.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/energy_buyer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/shareholder.py
+-rw-rw-rw-   0 root         (0) root         (0)      756 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/legal_structure.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/partner_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/related_actor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/partner_link.py
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/energy_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/payment_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      916 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/discount.py
+-rw-rw-rw-   0 root         (0) root         (0)     6891 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/integration_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-11 16:57:03.000000 djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/context_processors.py
```

### Comparing `djangoldp_energiepartagee-1.2.9/README.md` & `djangoldp_energiepartagee-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/setup.cfg` & `djangoldp_energiepartagee-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/PKG-INFO` & `djangoldp_energiepartagee-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoldp_energiepartagee
-Version: 1.2.9
+Version: 2.0.0
 Summary: Custom DjangoLDP based package for Energie Partagee
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee.egg-info/PKG-INFO` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoldp-energiepartagee
-Version: 1.2.9
+Version: 2.0.0
 Summary: Custom DjangoLDP based package for Energie Partagee
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee.egg-info/SOURCES.txt` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,21 @@
 djangoldp_energiepartagee/migrations/0079_rename_capital_distribution_capitaldistribution_and_more.py
 djangoldp_energiepartagee/migrations/0080_alter_citizenproject_status.py
 djangoldp_energiepartagee/migrations/0081_alter_citizenproject_status.py
 djangoldp_energiepartagee/migrations/0082_alter_capitaldistribution_actor_and_more.py
 djangoldp_energiepartagee/migrations/0083_alter_actor_options_and_more.py
 djangoldp_energiepartagee/migrations/0084_citizenproject_postcode.py
 djangoldp_energiepartagee/migrations/0085_citizenproject_wp_project_url_and_more.py
+djangoldp_energiepartagee/migrations/0086_alter_productionsite_total_development_budget_and_more.py
+djangoldp_energiepartagee/migrations/0087_alter_productionsite_progress_status.py
+djangoldp_energiepartagee/migrations/0088_alter_energyproduction_consumption_equivalence_and_more.py
+djangoldp_energiepartagee/migrations/0089_rename_effective_commissionning_yearl_productionsite_effective_commissionning_year_and_more.py
+djangoldp_energiepartagee/migrations/0090_productionsite_postcode.py
+djangoldp_energiepartagee/migrations/0090_region_admins.py
+djangoldp_energiepartagee/migrations/0091_merge_0090_productionsite_postcode_0090_region_admins.py
 djangoldp_energiepartagee/migrations/__init__.py
 djangoldp_energiepartagee/models/__init__.py
 djangoldp_energiepartagee/models/actor.py
 djangoldp_energiepartagee/models/capital_distribution.py
 djangoldp_energiepartagee/models/citizen_project.py
 djangoldp_energiepartagee/models/citizen_project_distinction.py
 djangoldp_energiepartagee/models/college.py
@@ -134,18 +141,19 @@
 djangoldp_energiepartagee/models/region.py
 djangoldp_energiepartagee/models/regional_network.py
 djangoldp_energiepartagee/models/related_actor.py
 djangoldp_energiepartagee/models/shareholder.py
 djangoldp_energiepartagee/models/signals.py
 djangoldp_energiepartagee/models/testimony.py
 djangoldp_energiepartagee/permissions/__init__.py
-djangoldp_energiepartagee/permissions/actor_permissions.py
-djangoldp_energiepartagee/permissions/contribution_permissions.py
-djangoldp_energiepartagee/permissions/generic_permissions.py
-djangoldp_energiepartagee/permissions/related_actor_permissions.py
+djangoldp_energiepartagee/permissions/ep_actor.py
+djangoldp_energiepartagee/permissions/ep_base.py
+djangoldp_energiepartagee/permissions/ep_contribution.py
+djangoldp_energiepartagee/permissions/ep_regional_admin.py
+djangoldp_energiepartagee/permissions/ep_related_actor.py
 djangoldp_energiepartagee/static/css/css_amorce.css
 djangoldp_energiepartagee/static/css/css_ep.css
 djangoldp_energiepartagee/static/css/registration.css
 djangoldp_energiepartagee/static/fonts/Inter-italic.var.woff2
 djangoldp_energiepartagee/static/fonts/Inter-roman.var.woff2
 djangoldp_energiepartagee/static/img/Amorcelogo.svg
 djangoldp_energiepartagee/static/img/EPlogo.svg
@@ -188,11 +196,10 @@
 djangoldp_energiepartagee/views/contributions_reminder.py
 djangoldp_energiepartagee/views/contributions_ventilation.py
 djangoldp_energiepartagee/views/export_contributions.py
 djangoldp_energiepartagee/views/export_contributions_all.py
 djangoldp_energiepartagee/views/generate_pdf_call.py
 djangoldp_energiepartagee/views/generate_pdf_receipt.py
 djangoldp_energiepartagee/views/plain_text_parser.py
-djangoldp_energiepartagee/views/related_actor.py
 djangoldp_energiepartagee/views/waiting_members_action.py
 djangoldp_energiepartagee/views/utils/__init__.py
 djangoldp_energiepartagee/views/utils/render_to_pdf.py
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/tests/tests_permissions.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/tests/tests_permissions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,1100 +1,1310 @@
-import uuid
 import json
-from django.db.models import signals
+import uuid
 
-from rest_framework.test import APITestCase, APIClient
+from django.db.models import signals
+from rest_framework.test import APIClient, APITestCase
 
 from djangoldp_energiepartagee.models import *
 from djangoldp_energiepartagee.tests.models import User
 
 
 class PermissionsTestCase(APITestCase):
     # Django runs setUp automatically before every test
     def setUp(self):
         # we have to create a client in order to test our API
         self.client = APIClient()
         # Disable all post_save signals
-        signals.post_save.disconnect(sender=User, dispatch_uid='test_perms_User')
-        signals.post_save.disconnect(sender=Contribution, dispatch_uid='test_perms_Contribution')
-        signals.post_save.disconnect(sender=Relatedactor, dispatch_uid='test_perms_Relatedactor')
-        signals.post_save.disconnect(sender=Actor, dispatch_uid='test_perms_Actor')
-        signals.pre_save.disconnect(sender=User, dispatch_uid='test_perms_User_pre')
-        signals.pre_save.disconnect(sender=Contribution, dispatch_uid='test_perms_Contribution_pre')
-        signals.pre_save.disconnect(sender=Relatedactor, dispatch_uid='test_perms_Relatedactor_pre')
-        signals.pre_save.disconnect(sender=Actor, dispatch_uid='test_perms_Actor_pre')
+        signals.post_save.disconnect(sender=User, dispatch_uid="test_perms_User")
+        signals.post_save.disconnect(
+            sender=Contribution, dispatch_uid="test_perms_Contribution"
+        )
+        signals.post_save.disconnect(
+            sender=Relatedactor, dispatch_uid="test_perms_Relatedactor"
+        )
+        signals.post_save.disconnect(sender=Actor, dispatch_uid="test_perms_Actor")
+        signals.pre_save.disconnect(sender=User, dispatch_uid="test_perms_User_pre")
+        signals.pre_save.disconnect(
+            sender=Contribution, dispatch_uid="test_perms_Contribution_pre"
+        )
+        signals.pre_save.disconnect(
+            sender=Relatedactor, dispatch_uid="test_perms_Relatedactor_pre"
+        )
+        signals.pre_save.disconnect(sender=Actor, dispatch_uid="test_perms_Actor_pre")
 
     # we have custom set up functions for things that we don't want to run before *every* test, e.g. often we want to
     # set up an authenticated user, but sometimes we want to run a test with an anonymous user
     def setUpLoggedInUser(self, is_superuser=False):
-        self.user = User(email='test@mactest.co.uk', first_name='Test', last_name='Mactest', username='test',
-                         password='glass onion', is_superuser=is_superuser)
+        self.user = User(
+            email="test@mactest.co.uk",
+            first_name="Test",
+            last_name="Mactest",
+            username="test",
+            is_superuser=is_superuser,
+        )
         self.user.save()
         # this means that our user is now logged in (as if they had typed username and password)
         self.client.force_authenticate(user=self.user)
 
     def setUpActor(self, owner_user=None):
         region = self._get_random_region()
         college = self._get_random_college()
         another_user = self._get_random_user()
-        self.actor = self._get_random_actor(region, college, another_user, owner_user=owner_user)
+        self.actor = self._get_random_actor(
+            region, college, another_user, owner_user=owner_user
+        )
 
     def setUpContribution(self):
         regionalnetwork = self._get_random_regionalnetwork()
         paymentmethod = self._get_random_paymentmethod()
-        self.contribution = self._get_random_contribution(self.actor, regionalnetwork, paymentmethod)
+        self.contribution = self._get_random_contribution(
+            self.actor, regionalnetwork, paymentmethod
+        )
 
     def _get_request_json(self, **kwargs):
         res = {
-            '@context': {
-                'rdfs': "http://www.w3.org/2000/01/rdf-schema#",
-                'name': "rdfs:label",
-                'isocode': "https://cdn.startinblox.com/owl#isocode",
-                'year': "https://cdn.startinblox.com/owl#year",
-                'amount': "https://cdn.startinblox.com/owl#amount",
-                'actor': "https://cdn.startinblox.com/owl#actor",
-                'presentation': "https://cdn.startinblox.com/owl#presentation",
-                'user': "https://cdn.startinblox.com/owl#user",
-                'postcode': "https://cdn.startinblox.com/owl#postcode",
-                'shortname': "https://cdn.startinblox.com/owl#shortname",
-                'longname': "https://cdn.startinblox.com/owl#longname",
-                'adhesiondate': "https://cdn.startinblox.com/owl#adhesiondate",
-                'mail': "https://cdn.startinblox.com/owl#mail",
-                'adhmail': "https://cdn.startinblox.com/owl#adhmail",
-                'address': "https://cdn.startinblox.com/owl#address",
-                'legalrepresentant': "https://cdn.startinblox.com/owl#legalrepresentant",
-                'managementcontact': "https://cdn.startinblox.com/owl#managementcontact",
-                'region': "https://cdn.startinblox.com/owl#region",
-                'college': "https://cdn.startinblox.com/owl#college",
-                'admincomment': "https://cdn.startinblox.com/owl#admincomment",
-                'role': "https://cdn.startinblox.com/owl#role"
+            "@context": {
+                "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
+                "name": "rdfs:label",
+                "isocode": "https://cdn.startinblox.com/owl#isocode",
+                "year": "https://cdn.startinblox.com/owl#year",
+                "amount": "https://cdn.startinblox.com/owl#amount",
+                "actor": "https://cdn.startinblox.com/owl#actor",
+                "presentation": "https://cdn.startinblox.com/owl#presentation",
+                "user": "https://cdn.startinblox.com/owl#user",
+                "postcode": "https://cdn.startinblox.com/owl#postcode",
+                "shortname": "https://cdn.startinblox.com/owl#shortname",
+                "longname": "https://cdn.startinblox.com/owl#longname",
+                "adhesiondate": "https://cdn.startinblox.com/owl#adhesiondate",
+                "mail": "https://cdn.startinblox.com/owl#mail",
+                "adhmail": "https://cdn.startinblox.com/owl#adhmail",
+                "address": "https://cdn.startinblox.com/owl#address",
+                "legalrepresentant": "https://cdn.startinblox.com/owl#legalrepresentant",
+                "managementcontact": "https://cdn.startinblox.com/owl#managementcontact",
+                "region": "https://cdn.startinblox.com/owl#region",
+                "college": "https://cdn.startinblox.com/owl#college",
+                "admincomment": "https://cdn.startinblox.com/owl#admincomment",
+                "role": "https://cdn.startinblox.com/owl#role",
             }
         }
 
         for kwarg in kwargs:
-            if kwarg in ['actor', 'user', 'region', 'college', 'stucturecollege', 'legalrepresentant', 'managementcontact']:
-                res.update({kwarg: {'@id': kwargs[kwarg]}})
+            if kwarg in [
+                "actor",
+                "user",
+                "region",
+                "college",
+                "stucturecollege",
+                "legalrepresentant",
+                "managementcontact",
+            ]:
+                res.update({kwarg: {"@id": kwargs[kwarg]}})
             else:
                 res.update({kwarg: kwargs[kwarg]})
 
         return res
 
     # we write functions like this for convenience - we can reuse between tests
     def _get_random_user(self):
         return User.objects.create(
-            email='{}@test.co.uk'.format(str(uuid.uuid4())), 
-            first_name='Test',
-            last_name='Test',
-            username=str(uuid.uuid4())
+            email="{}@test.co.uk".format(str(uuid.uuid4())),
+            first_name="Test",
+            last_name="Test",
+            username=str(uuid.uuid4()),
         )
 
-    def _get_random_region(self, name='TestRegion'):
+    def _get_random_region(self, name="TestRegion"):
         return Region.objects.create(name=name)
 
-    def _get_random_regionalnetwork(self, name='TestRegionalNetwork'):
+    def _get_random_regionalnetwork(self, name="TestRegionalNetwork"):
         return Regionalnetwork.objects.create(name=name)
 
-    def _get_random_college(self, name='TestCollege'):
-        return College.objects.create(name=name) 
+    def _get_random_college(self, name="TestCollege"):
+        return College.objects.create(name=name)
 
-    def _get_random_paymentmethod(self, name='TestPaymentMethod'):
-        return Paymentmethod.objects.create(name=name) 
+    def _get_random_paymentmethod(self, name="TestPaymentMethod"):
+        return Paymentmethod.objects.create(name=name)
 
-    def _get_random_actor(self, region=None, college=None, another_user=None, shortname='TestActor', longname='TestLongName', owner_user=None):
+    def _get_random_actor(
+        self,
+        region=None,
+        college=None,
+        another_user=None,
+        shortname="TestActor",
+        longname="TestLongName",
+        owner_user=None,
+    ):
         if region is None:
             region = self._get_random_region()
         if college is None:
             college = self._get_random_college()
         if another_user is None:
             another_user = self._get_random_user()
         if owner_user is None:
             owner_user = another_user
         return Actor.objects.create(
             shortname=shortname,
             longname=longname,
             region=region,
             college=college,
-            adhesiondate='1989',
+            adhesiondate="1989",
             legalrepresentant=another_user,
-            managementcontact=owner_user
+            managementcontact=owner_user,
         )
 
-    def _get_random_contribution(self, actor, regionalnetwork, paymentmethod, year=2020):
+    def _get_random_contribution(
+        self, actor, regionalnetwork, paymentmethod, year=2020
+    ):
         return Contribution.objects.create(
             year=year,
             actor=actor,
             paymentto=regionalnetwork,
             paymentmethod=paymentmethod,
             receivedby=regionalnetwork,
-            amount=30
+            amount=30,
         )
 
     def _get_random_profile(self, user):
-        return Profile.objects.create(
-            user=user
-        )
+        return Profile.objects.create(user=user)
 
-    def _get_relatedactor(self, user, actor, role='admin'):
-        return Relatedactor.objects.create(
-            user=user,
-            actor=actor,
-            role=role
-        )
+    def _get_relatedactor(self, user, actor, role="admin"):
+        return Relatedactor.objects.create(user=user, actor=actor, role=role)
 
     def _get_random_relatedactor(self):
         actor = self._get_random_actor()
         another_user = self._get_random_user()
         return self._get_relatedactor(actor=actor, user=another_user)
 
-    def _get_random_integrationstep(self, admincomment='TestAdminComment'):
+    def _get_random_integrationstep(self, admincomment="TestAdminComment"):
         return Integrationstep.objects.create(admincomment=admincomment)
 
-    def _get_random_interventionzone(self, name='TestInterventionzone'):
+    def _get_random_interventionzone(self, name="TestInterventionzone"):
         return Interventionzone.objects.create(name=name)
 
-    def _get_random_legalstructure(self, name='TestLegalstructure'):
+    def _get_random_legalstructure(self, name="TestLegalstructure"):
         return Legalstructure.objects.create(name=name)
 
-    def _get_random_collegeepa(self, name='TestCollegeepa'):
+    def _get_random_collegeepa(self, name="TestCollegeepa"):
         return Collegeepa.objects.create(name=name)
 
-
     # every function which starts with 'test_' will be ran by the Django test runner as a test (pass, fail, error)
     # pass is great, fail means that our assertion failed and error means that the test itself threw an error
     # we want one test for each behaviour
 
-# --- class Region:
+    # --- class Region:
     # superadmin : view
     def test_super_user_can_list_region(self):
         self.setUpLoggedInUser(is_superuser=True)
         region = self._get_random_region()
 
-        response = self.client.get('/regions/')
+        response = self.client.get("/regions/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # superadmin : change
     def test_super_user_can_modify_region(self):
         self.setUpLoggedInUser(is_superuser=True)
         region = self._get_random_region()
 
-        modified_data = self._get_request_json(name='Occitanie', isocode='FR-OCC')
-        response = self.client.patch('/regions/{}/'.format(region.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="Occitanie", isocode="FR-OCC")
+        response = self.client.patch(
+            "/regions/{}/".format(region.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         region = Region.objects.get(pk=region.pk)
-        self.assertEqual(region.name, 'Occitanie')
+        self.assertEqual(region.name, "Occitanie")
 
     # superadmin : add
     def test_super_user_can_post_region(self):
         self.setUpLoggedInUser(is_superuser=True)
 
-        new_data = self._get_request_json(name='Occitanie', isocode='FR-OCC')
-        response = self.client.post('/regions/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="Occitanie", isocode="FR-OCC")
+        response = self.client.post(
+            "/regions/", json.dumps(new_data), content_type="application/ld+json"
+        )
         self.assertEqual(response.status_code, 201)
 
     # admin or member : view
     def test_admin_or_member_can_list_region(self):
         self.setUpLoggedInUser(is_superuser=False)
         region = self._get_random_region()
 
-        response = self.client.get('/regions/')
+        response = self.client.get("/regions/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # admin or member : change denied
     def test_admin_or_member_cannot_modify_region(self):
         self.setUpLoggedInUser(is_superuser=False)
         region = self._get_random_region()
 
-        modified_data = self._get_request_json(name='Occitanie', isocode='FR-OCC')
-        response = self.client.patch('/regions/{}/'.format(region.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="Occitanie", isocode="FR-OCC")
+        response = self.client.patch(
+            "/regions/{}/".format(region.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 403)
 
     # admin or member : add denied
     def test_admin_or_member_can_post_region(self):
         self.setUpLoggedInUser(is_superuser=False)
 
-        new_data = self._get_request_json(name='Occitanie', isocode='FR-OCC')
-        response = self.client.post('/regions/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="Occitanie", isocode="FR-OCC")
+        response = self.client.post(
+            "/regions/", json.dumps(new_data), content_type="application/ld+json"
+        )
         self.assertEqual(response.status_code, 403)
-    
 
-# --- class Regionalnetwork:
+    # --- class Regionalnetwork:
     # superadmin : view, add, change
     def test_super_user_can_list_regionalnetwork(self):
         self.setUpLoggedInUser(is_superuser=True)
         regionalnetwork = self._get_random_regionalnetwork()
 
-        response = self.client.get('/regionalnetworks/')
+        response = self.client.get("/regionalnetworks/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     def test_super_user_can_modify_regionalnetwork(self):
         self.setUpLoggedInUser(is_superuser=True)
         regionalnetwork = self._get_random_regionalnetwork()
 
-        modified_data = self._get_request_json(name='HD-Occitanie')
-        response = self.client.patch('/regionalnetworks/{}/'.format(regionalnetwork.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="HD-Occitanie")
+        response = self.client.patch(
+            "/regionalnetworks/{}/".format(regionalnetwork.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         regionalnetwork = Regionalnetwork.objects.get(pk=regionalnetwork.pk)
-        self.assertEqual(regionalnetwork.name, 'HD-Occitanie')
+        self.assertEqual(regionalnetwork.name, "HD-Occitanie")
 
     def test_super_user_can_post_regionalnetwork(self):
         self.setUpLoggedInUser(is_superuser=True)
 
-        new_data = self._get_request_json(name='HD-Occitanie')
-        response = self.client.post('/regionalnetworks/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="HD-Occitanie")
+        response = self.client.post(
+            "/regionalnetworks/",
+            json.dumps(new_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 201)
 
     # admin or member : view
     def test_admin_or_member_can_list_regionalnetwork(self):
         self.setUpLoggedInUser(is_superuser=False)
         regionalnetwork = self._get_random_regionalnetwork()
 
-        response = self.client.get('/regionalnetworks/')
+        response = self.client.get("/regionalnetworks/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # admin or member: change denied
     def test_admin_or_member_cannot_change_regionalnetwork(self):
         self.setUpLoggedInUser(is_superuser=False)
         regionalnetwork = self._get_random_regionalnetwork()
 
-        modified_data = self._get_request_json(name='HD-Occitanie')
-        response = self.client.patch('/regionalnetworks/{}/'.format(regionalnetwork.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="HD-Occitanie")
+        response = self.client.patch(
+            "/regionalnetworks/{}/".format(regionalnetwork.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 403)
 
     # admin or member: add denied
     def test_admin_or_member_cannot_add_regionalnetwork(self):
         self.setUpLoggedInUser(is_superuser=False)
 
-        new_data = self._get_request_json(name='HD-Occitanie')
-        response = self.client.post('/regionalnetworks/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="HD-Occitanie")
+        response = self.client.post(
+            "/regionalnetworks/",
+            json.dumps(new_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 403)
 
     def test_anonymous_cannot_list_regionalnetwork(self):
         regionalnetwork = self._get_random_regionalnetwork()
 
-        response = self.client.get('/regionalnetworks/')
+        response = self.client.get("/regionalnetworks/")
         self.assertEqual(response.status_code, 403)
 
-
-# --- class Interventionzone:
+    # --- class Interventionzone:
     # superadmin : view, add, change
     def test_super_user_can_list_interventionzone(self):
         self.setUpLoggedInUser(is_superuser=True)
         interventionzone = self._get_random_interventionzone()
 
-        response = self.client.get('/interventionzones/')
+        response = self.client.get("/interventionzones/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     def test_super_user_can_modify_interventionzone(self):
         self.setUpLoggedInUser(is_superuser=True)
         interventionzone = self._get_random_interventionzone()
 
-        modified_data = self._get_request_json(name='NewInterventionzone')
-        response = self.client.patch('/interventionzones/{}/'.format(interventionzone.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="NewInterventionzone")
+        response = self.client.patch(
+            "/interventionzones/{}/".format(interventionzone.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         interventionzone = Interventionzone.objects.get(pk=interventionzone.pk)
-        self.assertEqual(interventionzone.name, 'NewInterventionzone')
+        self.assertEqual(interventionzone.name, "NewInterventionzone")
 
     def test_super_user_can_post_interventionzone(self):
         self.setUpLoggedInUser(is_superuser=True)
 
-        new_data = self._get_request_json(name='NewInterventionzone')
-        response = self.client.post('/interventionzones/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="NewInterventionzone")
+        response = self.client.post(
+            "/interventionzones/",
+            json.dumps(new_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 201)
 
     # admin or member : view
     def test_admin_or_member_can_list_interventionzone(self):
         self.setUpLoggedInUser(is_superuser=False)
         interventionzone = self._get_random_interventionzone()
 
-        response = self.client.get('/interventionzones/')
+        response = self.client.get("/interventionzones/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # admin or member: change denied
     def test_admin_or_member_cannot_change_interventionzone(self):
         self.setUpLoggedInUser(is_superuser=False)
         interventionzone = self._get_random_interventionzone()
 
-        modified_data = self._get_request_json(name='NewInterventionzone')
-        response = self.client.patch('/interventionzones/{}/'.format(interventionzone.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="NewInterventionzone")
+        response = self.client.patch(
+            "/interventionzones/{}/".format(interventionzone.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 403)
 
     # admin or member: add denied
     def test_admin_or_member_cannot_add_interventionzone(self):
         self.setUpLoggedInUser(is_superuser=False)
 
-        new_data = self._get_request_json(name='NewInterventionzone')
-        response = self.client.post('/interventionzones/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="NewInterventionzone")
+        response = self.client.post(
+            "/interventionzones/",
+            json.dumps(new_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 403)
 
     def test_anonymous_cannot_list_interventionzone(self):
         interventionzone = self._get_random_interventionzone()
 
-        response = self.client.get('/interventionzones/')
+        response = self.client.get("/interventionzones/")
         self.assertEqual(response.status_code, 403)
 
-
-# --- class Legalstructure:
+    # --- class Legalstructure:
     # superadmin : view, add, change
     def test_super_user_can_list_legalstructure(self):
         self.setUpLoggedInUser(is_superuser=True)
         legalstructure = self._get_random_legalstructure()
 
-        response = self.client.get('/legalstructures/')
+        response = self.client.get("/legalstructures/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     def test_super_user_can_modify_legalstructure(self):
         self.setUpLoggedInUser(is_superuser=True)
         legalstructure = self._get_random_legalstructure()
 
-        modified_data = self._get_request_json(name='NewLegalstructure')
-        response = self.client.patch('/legalstructures/{}/'.format(legalstructure.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="NewLegalstructure")
+        response = self.client.patch(
+            "/legalstructures/{}/".format(legalstructure.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         legalstructure = Legalstructure.objects.get(pk=legalstructure.pk)
-        self.assertEqual(legalstructure.name, 'NewLegalstructure')
+        self.assertEqual(legalstructure.name, "NewLegalstructure")
 
     def test_super_user_can_post_legalstructure(self):
         self.setUpLoggedInUser(is_superuser=True)
 
-        new_data = self._get_request_json(name='NewLegalstructure')
-        response = self.client.post('/legalstructures/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="NewLegalstructure")
+        response = self.client.post(
+            "/legalstructures/",
+            json.dumps(new_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 201)
 
     # admin or member : view
     def test_admin_or_member_can_list_legalstructure(self):
         self.setUpLoggedInUser(is_superuser=False)
         legalstructure = self._get_random_legalstructure()
 
-        response = self.client.get('/legalstructures/')
+        response = self.client.get("/legalstructures/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # admin or member: change denied
     def test_admin_or_member_cannot_change_legalstructure(self):
         self.setUpLoggedInUser(is_superuser=False)
         legalstructure = self._get_random_legalstructure()
 
-        modified_data = self._get_request_json(name='NewLegalstructure')
-        response = self.client.patch('/legalstructures/{}/'.format(legalstructure.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="NewLegalstructure")
+        response = self.client.patch(
+            "/legalstructures/{}/".format(legalstructure.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 403)
 
     # admin or member: add denied
     def test_admin_or_member_cannot_add_legalstructure(self):
         self.setUpLoggedInUser(is_superuser=False)
 
-        new_data = self._get_request_json(name='NewLegalstructure')
-        response = self.client.post('/legalstructures/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="NewLegalstructure")
+        response = self.client.post(
+            "/legalstructures/",
+            json.dumps(new_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 403)
 
     def test_anonymous_cannot_list_legalstructure(self):
         legalstructure = self._get_random_legalstructure()
 
-        response = self.client.get('/legalstructures/')
+        response = self.client.get("/legalstructures/")
         self.assertEqual(response.status_code, 403)
 
-
-# --- class Collegeepa:
+    # --- class Collegeepa:
     # superadmin : view, add, change
     def test_super_user_can_list_collegeepa(self):
         self.setUpLoggedInUser(is_superuser=True)
         collegeepa = self._get_random_collegeepa()
 
-        response = self.client.get('/collegeepas/')
+        response = self.client.get("/collegeepas/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     def test_super_user_can_modify_collegeepa(self):
         self.setUpLoggedInUser(is_superuser=True)
         collegeepa = self._get_random_collegeepa()
 
-        modified_data = self._get_request_json(name='NewCollegeepa')
-        response = self.client.patch('/collegeepas/{}/'.format(collegeepa.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="NewCollegeepa")
+        response = self.client.patch(
+            "/collegeepas/{}/".format(collegeepa.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         collegeepa = Collegeepa.objects.get(pk=collegeepa.pk)
-        self.assertEqual(collegeepa.name, 'NewCollegeepa')
+        self.assertEqual(collegeepa.name, "NewCollegeepa")
 
     def test_super_user_can_post_collegeepa(self):
         self.setUpLoggedInUser(is_superuser=True)
 
-        new_data = self._get_request_json(name='NewCollegeepa')
-        response = self.client.post('/collegeepas/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="NewCollegeepa")
+        response = self.client.post(
+            "/collegeepas/", json.dumps(new_data), content_type="application/ld+json"
+        )
         self.assertEqual(response.status_code, 201)
 
     # admin or member : view
     def test_admin_or_member_can_list_collegeepa(self):
         self.setUpLoggedInUser(is_superuser=False)
         collegeepa = self._get_random_collegeepa()
 
-        response = self.client.get('/collegeepas/')
+        response = self.client.get("/collegeepas/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # admin or member: change denied
     def test_admin_or_member_cannot_change_collegeepa(self):
         self.setUpLoggedInUser(is_superuser=False)
         collegeepa = self._get_random_collegeepa()
 
-        modified_data = self._get_request_json(name='NewCollegeepa')
-        response = self.client.patch('/collegeepas/{}/'.format(collegeepa.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="NewCollegeepa")
+        response = self.client.patch(
+            "/collegeepas/{}/".format(collegeepa.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 403)
 
     # admin or member: add denied
     def test_admin_or_member_cannot_add_collegeepa(self):
         self.setUpLoggedInUser(is_superuser=False)
 
-        new_data = self._get_request_json(name='NewCollegeepa')
-        response = self.client.post('/collegeepas/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="NewCollegeepa")
+        response = self.client.post(
+            "/collegeepas/", json.dumps(new_data), content_type="application/ld+json"
+        )
         self.assertEqual(response.status_code, 403)
 
     def test_anonymous_cannot_list_collegeepa(self):
         collegeepa = self._get_random_collegeepa()
 
-        response = self.client.get('/collegeepas/')
+        response = self.client.get("/collegeepas/")
         self.assertEqual(response.status_code, 403)
 
-
-# --- class College:
+    # --- class College:
     # superadmin : view, add, change
     def test_super_user_can_list_college(self):
         self.setUpLoggedInUser(is_superuser=True)
         college = self._get_random_college()
 
-        response = self.client.get('/colleges/')
+        response = self.client.get("/colleges/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     def test_super_user_can_modify_college(self):
         self.setUpLoggedInUser(is_superuser=True)
         college = self._get_random_college()
 
-        modified_data = self._get_request_json(name='NewCollege')
-        response = self.client.patch('/colleges/{}/'.format(college.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="NewCollege")
+        response = self.client.patch(
+            "/colleges/{}/".format(college.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         college = College.objects.get(pk=college.pk)
-        self.assertEqual(college.name, 'NewCollege')
+        self.assertEqual(college.name, "NewCollege")
 
     def test_super_user_can_post_college(self):
         self.setUpLoggedInUser(is_superuser=True)
 
-        new_data = self._get_request_json(name='NewCollege')
-        response = self.client.post('/colleges/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="NewCollege")
+        response = self.client.post(
+            "/colleges/", json.dumps(new_data), content_type="application/ld+json"
+        )
         self.assertEqual(response.status_code, 201)
 
     # admin or member : view
     def test_admin_or_member_can_list_college(self):
         self.setUpLoggedInUser(is_superuser=False)
         college = self._get_random_college()
 
-        response = self.client.get('/colleges/')
+        response = self.client.get("/colleges/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # admin or member: change denied
     def test_admin_or_member_cannot_change_college(self):
         self.setUpLoggedInUser(is_superuser=False)
         college = self._get_random_college()
 
-        modified_data = self._get_request_json(name='NewCollege')
-        response = self.client.patch('/colleges/{}/'.format(college.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="NewCollege")
+        response = self.client.patch(
+            "/colleges/{}/".format(college.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 403)
 
     # admin or member: add denied
     def test_admin_or_member_cannot_add_college(self):
         self.setUpLoggedInUser(is_superuser=False)
 
-        new_data = self._get_request_json(name='NewCollege')
-        response = self.client.post('/colleges/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="NewCollege")
+        response = self.client.post(
+            "/colleges/", json.dumps(new_data), content_type="application/ld+json"
+        )
         self.assertEqual(response.status_code, 403)
 
     def test_anonymous_cannot_list_college(self):
         college = self._get_random_college()
 
-        response = self.client.get('/colleges/')
+        response = self.client.get("/colleges/")
         self.assertEqual(response.status_code, 403)
 
-# --- class Paymentmethod:
+    # --- class Paymentmethod:
     # superadmin : view, add, change
     def test_super_user_can_list_paymentmethod(self):
         self.setUpLoggedInUser(is_superuser=True)
         paymentmethod = self._get_random_paymentmethod()
 
-        response = self.client.get('/paymentmethods/')
+        response = self.client.get("/paymentmethods/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     def test_super_user_can_modify_paymentmethod(self):
         self.setUpLoggedInUser(is_superuser=True)
         paymentmethod = self._get_random_paymentmethod()
 
-        modified_data = self._get_request_json(name='NewPaymentmethod')
-        response = self.client.patch('/paymentmethods/{}/'.format(paymentmethod.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="NewPaymentmethod")
+        response = self.client.patch(
+            "/paymentmethods/{}/".format(paymentmethod.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         paymentmethod = Paymentmethod.objects.get(pk=paymentmethod.pk)
-        self.assertEqual(paymentmethod.name, 'NewPaymentmethod')
+        self.assertEqual(paymentmethod.name, "NewPaymentmethod")
 
     def test_super_user_can_post_paymentmethod(self):
         self.setUpLoggedInUser(is_superuser=True)
 
         region = self._get_random_region()
-        new_data = self._get_request_json(name='NewPaymentmethod')
-        response = self.client.post('/paymentmethods/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="NewPaymentmethod")
+        response = self.client.post(
+            "/paymentmethods/", json.dumps(new_data), content_type="application/ld+json"
+        )
         self.assertEqual(response.status_code, 201)
 
     # admin or member : view
     def test_admin_or_member_can_list_paymentmethod(self):
         self.setUpLoggedInUser(is_superuser=False)
         paymentmethod = self._get_random_paymentmethod()
 
-        response = self.client.get('/paymentmethods/')
+        response = self.client.get("/paymentmethods/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # admin or member: change denied
     def test_admin_or_member_cannot_change_paymentmethod(self):
         self.setUpLoggedInUser(is_superuser=False)
         paymentmethod = self._get_random_paymentmethod()
 
-        modified_data = self._get_request_json(name='NewPaymentmethod')
-        response = self.client.patch('/paymentmethods/{}/'.format(paymentmethod.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(name="NewPaymentmethod")
+        response = self.client.patch(
+            "/paymentmethods/{}/".format(paymentmethod.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 403)
 
     # admin or member: add denied
     def test_admin_or_member_cannot_add_paymentmethod(self):
         self.setUpLoggedInUser(is_superuser=False)
 
-        new_data = self._get_request_json(name='NewPaymentmethod')
-        response = self.client.post('/paymentmethods/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(name="NewPaymentmethod")
+        response = self.client.post(
+            "/paymentmethods/", json.dumps(new_data), content_type="application/ld+json"
+        )
         self.assertEqual(response.status_code, 403)
 
     def test_anonymous_cannot_list_paymentmethod(self):
         paymentmethod = self._get_random_paymentmethod()
 
-        response = self.client.get('/paymentmethods/')
+        response = self.client.get("/paymentmethods/")
         self.assertEqual(response.status_code, 403)
 
-
-# --- class Profile ---
+    # --- class Profile ---
     # superadmin : view
     def test_super_user_can_list_profile(self):
         self.setUpLoggedInUser(is_superuser=True)
         another_user = self._get_random_user()
 
-        response = self.client.get('/profiles/')
+        response = self.client.get("/profiles/")
         self.assertEqual(response.status_code, 200)
-        self.assertGreaterEqual(len(response.data['ldp:contains']), 2)
+        self.assertGreaterEqual(len(response.data["ldp:contains"]), 2)
 
     # superadmin : change
     def test_super_user_can_change_profile(self):
         self.setUpLoggedInUser(is_superuser=True)
         another_user = self._get_random_user()
         another_profile = Profile.objects.get(user=another_user)
 
-        modified_data = self._get_request_json(presentation='Hello')
-        response = self.client.patch('/profiles/{}/'.format(another_profile.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(presentation="Hello")
+        response = self.client.patch(
+            "/profiles/{}/".format(another_profile.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         another_profile = Profile.objects.get(pk=another_profile.pk)
-        self.assertEqual(another_profile.presentation, 'Hello')  
+        self.assertEqual(another_profile.presentation, "Hello")
 
     # superadmin : add
     def test_super_user_can_add_profile(self):
-       self.setUpLoggedInUser(is_superuser=True)
-       another_user = self._get_random_user()
+        self.setUpLoggedInUser(is_superuser=True)
+        another_user = self._get_random_user()
 
-       new_data = self._get_request_json(user=another_user.urlid)
-       response = self.client.post('/profiles/', json.dumps(new_data), content_type='application/ld+json')
-       self.assertEqual(response.status_code, 201)
+        new_data = self._get_request_json(user=another_user.urlid)
+        response = self.client.post(
+            "/profiles/", json.dumps(new_data), content_type="application/ld+json"
+        )
+        self.assertEqual(response.status_code, 201)
 
     # admin or member : view only his own
     def test_user_can_list_only_its_profile(self):
         self.setUpLoggedInUser(is_superuser=False)
         ownprofile = Profile.objects.get(user=self.user)
         another_user = self._get_random_user()
         another_profile = Profile.objects.get(user=another_user)
 
-        response = self.client.get('/profiles/')
+        response = self.client.get("/profiles/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # admin or member : change only his own
     def test_user_can_change_only_its_profile(self):
         self.setUpLoggedInUser(is_superuser=False)
         ownprofile = Profile.objects.get(user=self.user)
         another_user = self._get_random_user()
         another_profile = Profile.objects.get(user=another_user)
 
-        modified_data = self._get_request_json(presentation='Hello')
-        response = self.client.patch('/profiles/{}/'.format(ownprofile.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(presentation="Hello")
+        response = self.client.patch(
+            "/profiles/{}/".format(ownprofile.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
-        response = self.client.patch('/profiles/{}/'.format(another_profile.pk), json.dumps(modified_data), content_type='application/ld+json')
+        response = self.client.patch(
+            "/profiles/{}/".format(another_profile.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 404)
 
         ownprofile = Profile.objects.get(pk=ownprofile.pk)
-        self.assertEqual(ownprofile.presentation, 'Hello')       
+        self.assertEqual(ownprofile.presentation, "Hello")
         another_profile = Profile.objects.get(pk=another_profile.pk)
         self.assertEqual(another_profile.presentation, None)
 
-# --- class Actor ---
+    # --- class Actor ---
     # superadmin : view
     def test_super_user_can_list_actor(self):
         self.setUpLoggedInUser(is_superuser=True)
         self._get_random_actor()
 
-        response = self.client.get('/actors/')
+        response = self.client.get("/actors/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # superadmin : change
     def test_super_user_can_change_actor(self):
         self.setUpLoggedInUser(is_superuser=True)
         actor = self._get_random_actor()
 
-        modified_data = self._get_request_json(postcode='33800')
-        response = self.client.patch('/actors/{}/'.format(actor.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(postcode="33800")
+        response = self.client.patch(
+            "/actors/{}/".format(actor.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         another_profile = Actor.objects.get(pk=actor.pk)
-        self.assertEqual(another_profile.postcode, '33800')
+        self.assertEqual(another_profile.postcode, "33800")
 
     # superadmin : add
     def test_super_user_can_add_actor(self):
         self.setUpLoggedInUser(is_superuser=True)
 
         region = self._get_random_region()
         college = self._get_random_college()
         another_user = self._get_random_user()
         new_data = self._get_request_json(
-            region=region.urlid, 
-            college=college.urlid, 
+            region=region.urlid,
+            college=college.urlid,
             legalrepresentant=another_user.urlid,
             managementcontact=another_user.urlid,
-            shortname='James',
-            longname='Bond',
-            adhesiondate='1968',
-            mail='jamesbond@mi6.uk',
-            adhmail='jamesbond@mi6.uk',
-            address='London'
-            )
-        response = self.client.post('/actors/', json.dumps(new_data), content_type='application/ld+json')
+            shortname="James",
+            longname="Bond",
+            adhesiondate="1968",
+            mail="jamesbond@mi6.uk",
+            adhmail="jamesbond@mi6.uk",
+            address="London",
+        )
+        response = self.client.post(
+            "/actors/", json.dumps(new_data), content_type="application/ld+json"
+        )
         self.assertEqual(response.status_code, 201)
 
     # admin : view
     def test_admin_can_list_all_actor(self):
         self.setUpLoggedInUser(is_superuser=False)
         self.setUpActor()
-        relatedactor = self._get_relatedactor(self.user, self.actor, 'admin')
-        
+        relatedactor = self._get_relatedactor(self.user, self.actor, "admin")
+
         another_actor = self._get_random_actor()
         another_user = self._get_random_user()
-        another_relatedactor = self._get_relatedactor(another_user, another_actor, 'admin')
+        another_relatedactor = self._get_relatedactor(
+            another_user, another_actor, "admin"
+        )
 
-        response = self.client.get('/actors/')
+        response = self.client.get("/actors/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 2)
+        self.assertEqual(len(response.data["ldp:contains"]), 2)
 
     # admin : change own
     def test_admin_can_change_own_actor(self):
         self.setUpLoggedInUser(is_superuser=False)
         self.setUpActor(self.user)
 
-        modified_data = self._get_request_json(postcode='33800')
-        response = self.client.patch('/actors/{}/'.format(self.actor.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(postcode="33800")
+        response = self.client.patch(
+            "/actors/{}/".format(self.actor.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         another_profile = Actor.objects.get(pk=self.actor.pk)
-        self.assertEqual(another_profile.postcode, '33800')
+        self.assertEqual(another_profile.postcode, "33800")
 
     def test_admin_cannot_change_other_actor(self):
         self.setUpLoggedInUser(is_superuser=False)
         self.setUpActor()
 
-        modified_data = self._get_request_json(postcode='33800')
-        response = self.client.patch('/actors/{}/'.format(self.actor.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(postcode="33800")
+        response = self.client.patch(
+            "/actors/{}/".format(self.actor.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 403)
 
     # member : view own
     def test_member_can_list_all_actor(self):
         self.setUpLoggedInUser(is_superuser=False)
         self.setUpActor()
-        relatedactor = self._get_relatedactor(self.user, self.actor, 'member')
+        self._get_relatedactor(self.user, self.actor, "member")
 
         another_actor = self._get_random_actor()
         another_user = self._get_random_user()
-        another_relatedactor = self._get_relatedactor(another_user, another_actor, 'member')
+        self._get_relatedactor(another_user, another_actor, "member")
 
-        response = self.client.get('/actors/')
+        response = self.client.get("/actors/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 2)
+        self.assertEqual(len(response.data["ldp:contains"]), 2)
 
     # member : change denied
     def test_member_cannot_change_own_actor(self):
+        another_user = self._get_random_user()
+        self.setUpActor(another_user)
+
         self.setUpLoggedInUser(is_superuser=False)
-        self.setUpActor()
-        relatedactor = self._get_relatedactor(self.user, self.actor, 'member')
+        self._get_relatedactor(self.user, self.actor, "member")
 
-        modified_data = self._get_request_json(postcode='33800')
-        response = self.client.patch('/actors/{}/'.format(self.actor.pk), json.dumps(modified_data), content_type='application/ld+json')
-        self.assertEqual(response.status_code, 403) 
+        modified_data = self._get_request_json(postcode="33800")
+        response = self.client.patch(
+            "/actors/{}/".format(self.actor.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
+        self.assertEqual(response.status_code, 403)
 
     def test_member_cannot_change_other_actor(self):
         self.setUpLoggedInUser(is_superuser=False)
         self.setUpActor()
 
-        modified_data = self._get_request_json(postcode='33800')
-        response = self.client.patch('/actors/{}/'.format(self.actor.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(postcode="33800")
+        response = self.client.patch(
+            "/actors/{}/".format(self.actor.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 403)
 
     # admin or member : add
     def test_admin_can_add_actor(self):
         self.setUpLoggedInUser(is_superuser=False)
         self.setUpActor()
 
         region = self._get_random_region()
         college = self._get_random_college()
         another_user = self._get_random_user()
         new_data = self._get_request_json(
-            region=region.urlid, 
-            college=college.urlid, 
+            region=region.urlid,
+            college=college.urlid,
             legalrepresentant=another_user.urlid,
             managementcontact=another_user.urlid,
-            shortname='James',
-            longname='Bond',
-            adhesiondate='1968',
-            mail='jamesbond@mi6.uk',
-            adhmail='jamesbond@mi6.uk',
-            address='London'
-            )
-        response = self.client.post('/actors/', json.dumps(new_data), content_type='application/ld+json')
+            shortname="James",
+            longname="Bond",
+            adhesiondate="1968",
+            mail="jamesbond@mi6.uk",
+            adhmail="jamesbond@mi6.uk",
+            address="London",
+        )
+        response = self.client.post(
+            "/actors/", json.dumps(new_data), content_type="application/ld+json"
+        )
         self.assertEqual(response.status_code, 201)
 
-# --- class Integrationstep  ---
+    # --- class Integrationstep  ---
     # superadmin : view
     def test_super_user_can_list_integrationstep(self):
         self.setUpLoggedInUser(is_superuser=True)
         integrationstep = self._get_random_integrationstep()
 
-        response = self.client.get('/integrationsteps/')
+        response = self.client.get("/integrationsteps/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # superadmin : add
     def test_super_user_can_add_integrationstep(self):
         self.setUpLoggedInUser(is_superuser=True)
         actor = self._get_random_actor()
 
-        new_data = self._get_request_json(admincomment='New comment')
-        response = self.client.post('/integrationsteps/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(admincomment="New comment")
+        response = self.client.post(
+            "/integrationsteps/",
+            json.dumps(new_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 201)
 
     # superadmin : change
     def test_super_user_can_change_integrationstep(self):
         self.setUpLoggedInUser(is_superuser=True)
         integrationstep = self._get_random_integrationstep()
 
-        modified_data = self._get_request_json(admincomment='New comment')
-        response = self.client.patch('/integrationsteps/{}/'.format(integrationstep.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(admincomment="New comment")
+        response = self.client.patch(
+            "/integrationsteps/{}/".format(integrationstep.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         integrationstep = Integrationstep.objects.get(pk=integrationstep.pk)
-        self.assertEqual(integrationstep.admincomment, 'New comment')   
+        self.assertEqual(integrationstep.admincomment, "New comment")
 
     # member or admin : view denied
     def test_member_or_admin_cannot_list_integrationstep(self):
         self.setUpLoggedInUser(is_superuser=False)
         integrationstep = self._get_random_integrationstep()
 
-        response = self.client.get('/integrationsteps/{}/'.format(integrationstep.pk))
+        response = self.client.get("/integrationsteps/{}/".format(integrationstep.pk))
         self.assertEqual(response.status_code, 403)
 
     def test_anonymous_cannot_list_integrationstep(self):
         integrationstep = self._get_random_integrationstep()
 
-        response = self.client.get('/integrationsteps/{}/'.format(integrationstep.pk))
+        response = self.client.get("/integrationsteps/{}/".format(integrationstep.pk))
         self.assertEqual(response.status_code, 403)
 
-
-# --- class Contribution ---
+    # --- class Contribution ---
     # superadmin : view
     def test_super_user_can_list_contribution(self):
         self.setUpLoggedInUser(is_superuser=True)
         self.setUpActor()
         # self.setUpContribution()
 
-        response = self.client.get('/contributions/')
+        response = self.client.get("/contributions/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # superadmin : add
     def test_super_user_can_add_contribution(self):
         self.setUpLoggedInUser(is_superuser=True)
         self.setUpActor()
 
-        new_data = self._get_request_json(year=2021,amount=43, actor=self.actor.urlid)
-        response = self.client.post('/contributions/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(year=2021, amount=43, actor=self.actor.urlid)
+        response = self.client.post(
+            "/contributions/", json.dumps(new_data), content_type="application/ld+json"
+        )
         self.assertEqual(response.status_code, 201)
 
     # superadmin : change
     def test_super_user_can_change_contribution(self):
         self.setUpLoggedInUser(is_superuser=True)
         self.setUpActor()
         self.setUpContribution()
 
-        modified_data = self._get_request_json(year=2021,amount=43)
-        response = self.client.patch('/contributions/{}/'.format(self.contribution.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(year=2021, amount=43)
+        response = self.client.patch(
+            "/contributions/{}/".format(self.contribution.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         contribution = Contribution.objects.get(pk=self.contribution.pk)
         self.assertEqual(contribution.year, 2021)
 
     # admin : view his own
     def test_admin_can_list_own_contribution(self):
         self.setUpLoggedInUser(is_superuser=False)
         self.setUpActor(self.user)
 
         self._get_random_actor()
 
-        response = self.client.get('/contributions/')
+        response = self.client.get("/contributions/")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(Contribution.objects.count(), 2)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
-
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # admin : view his own nested in actor
     def test_admin_can_list_own_nested_contribution(self):
         self.setUpLoggedInUser(is_superuser=False)
 
         another_actor = self._get_random_actor()
         another_user = self._get_random_user()
-        another_relatedactor = self._get_relatedactor(actor = another_actor, user = another_user, role = 'member')
+        another_relatedactor = self._get_relatedactor(
+            actor=another_actor, user=another_user, role="member"
+        )
 
         self.setUpActor(self.user)
 
-        response = self.client.get('/actors/{}/contributions/'.format(self.actor.pk))
+        response = self.client.get("/actors/{}/contributions/".format(self.actor.pk))
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
         a_third_actor = self._get_random_actor()
 
-        response = self.client.get('/actors/{}/contributions/'.format(a_third_actor.pk))
+        response = self.client.get("/actors/{}/contributions/".format(a_third_actor.pk))
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 0)
-    
+        self.assertEqual(len(response.data["ldp:contains"]), 0)
+
     # member: view denied
     def test_member_cannot_list_contributions(self):
-        self.setUpLoggedInUser(is_superuser=False)
-        self.setUpActor()
+        another_user = self._get_random_user()
+        self.setUpActor(another_user)
         self.setUpContribution()
-        relatedactor = self._get_relatedactor(self.user, self.actor, 'member')
 
-        response = self.client.get('/contributions/')
+        self.setUpLoggedInUser(is_superuser=False)
+        self._get_relatedactor(self.user, self.actor, "member")
+
+        response = self.client.get("/contributions/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 0)
+        self.assertEqual(len(response.data["ldp:contains"]), 0)
 
-    # admin or member : add denied   
+    # admin or member : add denied
     def test_non_super_user_cannot_change_contribution(self):
         self.setUpLoggedInUser(is_superuser=False)
         self.setUpActor()
         self.setUpContribution()
-        
-        modified_data = self._get_request_json(year=2021,amount=43)
-        response = self.client.patch('/contributions/{}/'.format(self.contribution.pk), json.dumps(modified_data), content_type='application/ld+json')
-        self.assertEqual(response.status_code, 403)
+
+        modified_data = self._get_request_json(year=2021, amount=43)
+        response = self.client.patch(
+            "/contributions/{}/".format(self.contribution.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
+        self.assertEqual(response.status_code, 404)
 
     # admin or member : add denied
     def test_non_super_user_cannot_add_contribution(self):
-        self.setUpLoggedInUser(is_superuser=False)
-        self.setUpActor()
-        relatedactor = self._get_relatedactor(self.user, self.actor, 'member')
+        another_user = self._get_random_user()
+        self.setUpActor(another_user)
 
-        new_data = self._get_request_json(year=2021,amount=43, actor=self.actor.urlid)
-        response = self.client.post('/contributions/', json.dumps(new_data), content_type='application/ld+json')
-        self.assertEqual(response.status_code, 403)   
+        self.setUpLoggedInUser(is_superuser=False)
 
+        new_data = self._get_request_json(year=2021, amount=43, actor=self.actor.urlid)
+        response = self.client.post(
+            "/contributions/", json.dumps(new_data), content_type="application/ld+json"
+        )
+        self.assertEqual(response.status_code, 403)
 
-# --- class RelatedActor
+    # --- class RelatedActor
     # superadmin: view
     def test_super_user_can_list_relatedactor(self):
         self.setUpLoggedInUser(is_superuser=True)
         # since creating an actor creates the relatedactor associated
         actor = self._get_random_actor()
 
-        response = self.client.get('/relatedactors/')
+        response = self.client.get("/relatedactors/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     # superadmin: add
     def test_super_user_can_add_relatedactor(self):
         self.setUpLoggedInUser(is_superuser=True)
         user = self._get_random_user()
         actor = self._get_random_actor()
 
-        new_data = self._get_request_json(
-            user=user.urlid,
-            actor=actor.urlid
-            )
-        response = self.client.post('/relatedactors/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(user=user.urlid, actor=actor.urlid)
+        response = self.client.post(
+            "/relatedactors/", json.dumps(new_data), content_type="application/ld+json"
+        )
         self.assertEqual(response.status_code, 201)
 
     # superadmin: change
     def test_super_user_can_change_relatedactor(self):
         self.setUpLoggedInUser(is_superuser=True)
         relatedactor = self._get_random_relatedactor()
         another_actor = self._get_random_actor()
 
         modified_data = self._get_request_json(actor=another_actor.urlid)
-        response = self.client.patch('/relatedactors/{}/'.format(relatedactor.pk), json.dumps(modified_data), content_type='application/ld+json')
+        response = self.client.patch(
+            "/relatedactors/{}/".format(relatedactor.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         relatedactor = Relatedactor.objects.get(pk=relatedactor.pk)
-        self.assertEqual(relatedactor.actor, another_actor)         
+        self.assertEqual(relatedactor.actor, another_actor)
 
     # admin: view relatedactors of its actor
     def test_admin_can_list_only_its_actor_relatedactors(self):
         # NB: creating an actor creates a relatedactor with the owner as admin
         # Actor and relatedactor with user as admin
         self.setUpLoggedInUser(is_superuser=False)
 
         # Here the user is both owner and admin of the actor
         actor = self._get_random_actor(owner_user=self.user)
 
         # Another relatedactor to the actor the self.user is admin
         another_user = self._get_random_user()
-        a_relatedactor_related_to_the_actor = self._get_relatedactor(actor=actor, user=another_user, role='member')
+        a_relatedactor_related_to_the_actor = self._get_relatedactor(
+            actor=actor, user=another_user, role="member"
+        )
 
         # An unrelated actor
         another_actor = self._get_random_actor()
 
         # 3 relatedactors are created but member can see only 2
         self.assertEqual(len(Relatedactor.objects.all()), 3)
-        response = self.client.get('/relatedactors/')
+        response = self.client.get("/relatedactors/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 2)
+        self.assertEqual(len(response.data["ldp:contains"]), 2)
 
     # admin: change relatedactors of its actor
     def test_admin_can_change_its_actor_relatedactors(self):
-        self.setUpLoggedInUser(is_superuser=False)       
+        self.setUpLoggedInUser(is_superuser=False)
         actor = self._get_random_actor(owner_user=self.user)
 
         another_user = self._get_random_user()
-        another_relatedactor = self._get_relatedactor(actor=actor, user=another_user, role='membre')
+        another_relatedactor = self._get_relatedactor(
+            actor=actor, user=another_user, role="membre"
+        )
 
-        modified_data = self._get_request_json(role='admin')
-        response = self.client.patch('/relatedactors/{}/'.format(another_relatedactor.pk), json.dumps(modified_data), content_type='application/ld+json')
+        modified_data = self._get_request_json(role="admin")
+        response = self.client.patch(
+            "/relatedactors/{}/".format(another_relatedactor.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 200)
 
         relatedactor = Relatedactor.objects.get(pk=another_relatedactor.pk)
-        self.assertEqual(relatedactor.role, 'admin')  
+        self.assertEqual(relatedactor.role, "admin")
 
     def test_admin_cannot_change_another_relatedactor(self):
         self.setUpLoggedInUser(is_superuser=False)
         actor = self._get_random_actor()
         another_user = self._get_random_user()
-        relatedactor = self._get_relatedactor(user=another_user, actor=actor, role='admin')
+        relatedactor = self._get_relatedactor(
+            user=another_user, actor=actor, role="admin"
+        )
 
         another_actor = self._get_random_actor()
         modified_data = self._get_request_json(actor=another_actor.urlid)
-        response = self.client.patch('/relatedactors/{}/'.format(relatedactor.pk), json.dumps(modified_data), content_type='application/ld+json')
+        response = self.client.patch(
+            "/relatedactors/{}/".format(relatedactor.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 404)
 
     # admin: add
     def test_admin_can_add_relatedactor(self):
         self.setUpLoggedInUser(is_superuser=False)
         self.setUpActor()
 
-        self._get_relatedactor(actor=self.actor, user=self.user, role='admin')
+        self._get_relatedactor(actor=self.actor, user=self.user, role="admin")
 
         another_user = self._get_random_user()
 
         new_data = self._get_request_json(
-            user=another_user.urlid,
-            actor=self.actor.urlid
+            user=another_user.urlid, actor=self.actor.urlid
+        )
+        response = self.client.post(
+            "/relatedactors/", json.dumps(new_data), content_type="application/ld+json"
         )
-        response = self.client.post('/relatedactors/', json.dumps(new_data), content_type='application/ld+json')
         self.assertEqual(response.status_code, 201)
 
     # member: view relatedactors of its actor
     def test_member_can_list_only_its_relatedactor(self):
         # NB: creating an actor creates a relatedactor with the owner as admin
         # Actor and relatedactor with user as member
         self.setUpLoggedInUser(is_superuser=False)
         actor = self._get_random_actor()
-        relatedactor = self._get_relatedactor(user=self.user, actor=actor, role='membre')
+        relatedactor = self._get_relatedactor(
+            user=self.user, actor=actor, role="membre"
+        )
 
         # Another relatedactor to the actor the self.user is member
         another_user = self._get_random_user()
-        a_relatedactor_related_to_the_actor = self._get_relatedactor(actor=actor, user=another_user, role='membre')
+        a_relatedactor_related_to_the_actor = self._get_relatedactor(
+            actor=actor, user=another_user, role="membre"
+        )
 
         # An unrelated actor
         another_actor = self._get_random_actor()
 
         # 4 relatedactors are created but member can see only 3
         self.assertEqual(len(Relatedactor.objects.all()), 4)
-        response = self.client.get('/relatedactors/')
+        response = self.client.get("/relatedactors/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 3)
+        self.assertEqual(len(response.data["ldp:contains"]), 3)
 
     # member: change denied
     def test_member_cannot_change_another_relatedactor(self):
         self.setUpLoggedInUser(is_superuser=False)
         actor = self._get_random_actor()
-        relatedactor = self._get_relatedactor(user=self.user, actor=actor, role='membre')
+        relatedactor = self._get_relatedactor(
+            user=self.user, actor=actor, role="membre"
+        )
 
         another_actor = self._get_random_actor()
         modified_data = self._get_request_json(actor=another_actor.urlid)
-        response = self.client.patch('/relatedactors/{}/'.format(relatedactor.pk), json.dumps(modified_data), content_type='application/ld+json')
+        response = self.client.patch(
+            "/relatedactors/{}/".format(relatedactor.pk),
+            json.dumps(modified_data),
+            content_type="application/ld+json",
+        )
         self.assertEqual(response.status_code, 403)
 
     # member: add
     def test_member_can_add_relatedactor(self):
         self.setUpLoggedInUser(is_superuser=False)
         self.setUpActor()
 
-        self._get_relatedactor(actor=self.actor, user=self.user, role='membre')
+        self._get_relatedactor(actor=self.actor, user=self.user, role="membre")
 
         another_user = self._get_random_user()
 
         new_data = self._get_request_json(
-            user=another_user.urlid,
-            actor=self.actor.urlid
+            user=another_user.urlid, actor=self.actor.urlid
+        )
+        response = self.client.post(
+            "/relatedactors/", json.dumps(new_data), content_type="application/ld+json"
         )
-        response = self.client.post('/relatedactors/', json.dumps(new_data), content_type='application/ld+json')
         self.assertEqual(response.status_code, 201)
 
-    # authenticated: can add with an empty role 
+    # authenticated: can add with an empty role
     def test_authenticated_user_can_add_relatedactor_with_empty_role(self):
         self.setUpLoggedInUser(is_superuser=False)
         actor = self._get_random_actor()
 
-        new_data = self._get_request_json(
-            user=self.user.urlid,
-            actor=actor.urlid
-            )
-        response = self.client.post('/relatedactors/', json.dumps(new_data), content_type='application/ld+json')
+        new_data = self._get_request_json(user=self.user.urlid, actor=actor.urlid)
+        response = self.client.post(
+            "/relatedactors/", json.dumps(new_data), content_type="application/ld+json"
+        )
 
         self.assertEqual(response.status_code, 201)
 
-    # authenticated: cannot add with a defined role 
+    # authenticated: cannot add with a defined role
     def test_authenticated_user_cannot_add_himself_as_actor_admin(self):
         self.setUpLoggedInUser(is_superuser=False)
         actor = self._get_random_actor()
 
         new_data = self._get_request_json(
-            user=self.user.urlid,
-            actor=actor.urlid,
-            role='admin'
+            user=self.user.urlid, actor=actor.urlid, role="admin"
+        )
+        response = self.client.post(
+            "/relatedactors/", json.dumps(new_data), content_type="application/ld+json"
         )
-        response = self.client.post('/relatedactors/', json.dumps(new_data), content_type='application/ld+json')
 
-        self.assertEqual(response.status_code, 403)
+        self.assertEqual(response.status_code, 403)
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/tests/tests_post.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/tests/tests_post.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,218 +1,259 @@
-import uuid
 import json
-from django.db.models import signals
+import uuid
 
-from rest_framework.test import APITestCase, APIClient
+from django.db.models import signals
+from rest_framework.test import APIClient, APITestCase
 
 from djangoldp_energiepartagee.models import *
 from djangoldp_energiepartagee.tests.models import User
 
 
 class PermissionsTestCase(APITestCase):
     # Django runs setUp automatically before every test
     def setUp(self):
         self.client = APIClient()
         # Disable all post_save signals
-        signals.post_save.disconnect(sender=User, dispatch_uid='test_perms_User')
-        signals.post_save.disconnect(sender=Contribution, dispatch_uid='test_perms_Contribution')
-        signals.post_save.disconnect(sender=Relatedactor, dispatch_uid='test_perms_Relatedactor')
-        signals.post_save.disconnect(sender=Actor, dispatch_uid='test_perms_Actor')
-        signals.pre_save.disconnect(sender=User, dispatch_uid='test_perms_User_pre')
-        signals.pre_save.disconnect(sender=Contribution, dispatch_uid='test_perms_Contribution_pre')
-        signals.pre_save.disconnect(sender=Relatedactor, dispatch_uid='test_perms_Relatedactor_pre')
-        signals.pre_save.disconnect(sender=Actor, dispatch_uid='test_perms_Actor_pre')
+        signals.post_save.disconnect(sender=User, dispatch_uid="test_perms_User")
+        signals.post_save.disconnect(
+            sender=Contribution, dispatch_uid="test_perms_Contribution"
+        )
+        signals.post_save.disconnect(
+            sender=Relatedactor, dispatch_uid="test_perms_Relatedactor"
+        )
+        signals.post_save.disconnect(sender=Actor, dispatch_uid="test_perms_Actor")
+        signals.pre_save.disconnect(sender=User, dispatch_uid="test_perms_User_pre")
+        signals.pre_save.disconnect(
+            sender=Contribution, dispatch_uid="test_perms_Contribution_pre"
+        )
+        signals.pre_save.disconnect(
+            sender=Relatedactor, dispatch_uid="test_perms_Relatedactor_pre"
+        )
+        signals.pre_save.disconnect(sender=Actor, dispatch_uid="test_perms_Actor_pre")
 
     # we have custom set up functions for things that we don't want to run before *every* test, e.g. often we want to
     # set up an authenticated user, but sometimes we want to run a test with an anonymous user
     def setUpLoggedInUser(self, is_superuser=False):
-        self.user = User(email='test@mactest.co.uk', first_name='Test', last_name='Mactest', username='test',
-                         password='glass onion', is_superuser=is_superuser)
+        self.user = User(
+            email="test@mactest.co.uk",
+            first_name="Test",
+            last_name="Mactest",
+            username="test",
+            password="glass onion",
+            is_superuser=is_superuser,
+        )
         self.user.save()
         # this means that our user is now logged in (as if they had typed username and password)
         self.client.force_authenticate(user=self.user)
 
     def setUpActor(self, owner_user=None):
         region = self._get_random_region()
         college = self._get_random_college()
         another_user = self._get_random_user()
-        self.actor = self._get_random_actor(region, college, another_user, owner_user=owner_user)
+        self.actor = self._get_random_actor(
+            region, college, another_user, owner_user=owner_user
+        )
 
     def setUpContribution(self):
         regionalnetwork = self._get_random_regionalnetwork()
         paymentmethod = self._get_random_paymentmethod()
-        self.contribution = self._get_random_contribution(self.actor, regionalnetwork, paymentmethod)
+        self.contribution = self._get_random_contribution(
+            self.actor, regionalnetwork, paymentmethod
+        )
 
     def _get_request_json(self, **kwargs):
         res = {
-            '@context': {
-                'rdfs': "http://www.w3.org/2000/01/rdf-schema#",
-                'name': "rdfs:label",
-                'isocode': "http://happy-dev.fr/owl/#isocode",
-                'year': "http://happy-dev.fr/owl/#year",
-                'amount': "http://happy-dev.fr/owl/#amount",
-                'actor': "http://happy-dev.fr/owl/#actor",
-                'presentation': "http://happy-dev.fr/owl/#presentation",
-                'user': "http://happy-dev.fr/owl/#user",
-                'postcode': "http://happy-dev.fr/owl/#postcode",
-                'shortname': "http://happy-dev.fr/owl/#shortname",
-                'longname': "http://happy-dev.fr/owl/#longname",
-                'adhesiondate': "http://happy-dev.fr/owl/#adhesiondate",
-                'mail': "http://happy-dev.fr/owl/#mail",
-                'adhmail': "http://happy-dev.fr/owl/#adhmail",
-                'address': "http://happy-dev.fr/owl/#address",
-                'legalrepresentant': "http://happy-dev.fr/owl/#legalrepresentant",
-                'managementcontact': "http://happy-dev.fr/owl/#managementcontact",
-                'region': "http://happy-dev.fr/owl/#region",
-                'college': "http://happy-dev.fr/owl/#college"
+            "@context": {
+                "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
+                "name": "rdfs:label",
+                "isocode": "http://startinblox.com/owl/#isocode",
+                "year": "http://startinblox.com/owl/#year",
+                "amount": "http://startinblox.com/owl/#amount",
+                "actor": "http://startinblox.com/owl/#actor",
+                "presentation": "http://startinblox.com/owl/#presentation",
+                "user": "http://startinblox.com/owl/#user",
+                "postcode": "http://startinblox.com/owl/#postcode",
+                "shortname": "http://startinblox.com/owl/#shortname",
+                "longname": "http://startinblox.com/owl/#longname",
+                "adhesiondate": "http://startinblox.com/owl/#adhesiondate",
+                "mail": "http://startinblox.com/owl/#mail",
+                "adhmail": "http://startinblox.com/owl/#adhmail",
+                "address": "http://startinblox.com/owl/#address",
+                "legalrepresentant": "http://startinblox.com/owl/#legalrepresentant",
+                "managementcontact": "http://startinblox.com/owl/#managementcontact",
+                "region": "http://startinblox.com/owl/#region",
+                "college": "http://startinblox.com/owl/#college",
             }
         }
 
         for kwarg in kwargs:
-            if kwarg in ['actor', 'user', 'region', 'college', 'stucturecollege', 'legalrepresentant', 'managementcontact']:
-                res.update({kwarg: {'@id': kwargs[kwarg]}})
+            if kwarg in [
+                "actor",
+                "user",
+                "region",
+                "college",
+                "stucturecollege",
+                "legalrepresentant",
+                "managementcontact",
+            ]:
+                res.update({kwarg: {"@id": kwargs[kwarg]}})
             else:
                 res.update({kwarg: kwargs[kwarg]})
 
         return res
 
     # we write functions like this for convenience - we can reuse between tests
     def _get_random_user(self):
         return User.objects.create(
-            email='{}@test.co.uk'.format(str(uuid.uuid4())),
-            first_name='Test',
-            last_name='Test',
-            username=str(uuid.uuid4())
+            email="{}@test.co.uk".format(str(uuid.uuid4())),
+            first_name="Test",
+            last_name="Test",
+            username=str(uuid.uuid4()),
         )
 
-    def _get_random_region(self, name='TestRegion'):
+    def _get_random_region(self, name="TestRegion"):
         return Region.objects.create(name=name)
 
-    def _get_random_regionalnetwork(self, name='TestRegion'):
+    def _get_random_regionalnetwork(self, name="TestRegion"):
         return Regionalnetwork.objects.create(name=name)
 
-    def _get_random_college(self, name='TestCollege'):
+    def _get_random_college(self, name="TestCollege"):
         return College.objects.create(name=name)
 
-    def _get_random_paymentmethod(self, name='TestPaymentMethod'):
+    def _get_random_paymentmethod(self, name="TestPaymentMethod"):
         return Paymentmethod.objects.create(name=name)
 
-    def _get_random_actor(self, region=None, college=None, another_user=None, shortname='TestActor', longname='TestLongName', owner_user=None):
+    def _get_random_actor(
+        self,
+        region=None,
+        college=None,
+        another_user=None,
+        shortname="TestActor",
+        longname="TestLongName",
+        owner_user=None,
+    ):
         if region is None:
             region = self._get_random_region()
         if college is None:
             college = self._get_random_college()
         if another_user is None:
             another_user = self._get_random_user()
         if owner_user is None:
             owner_user = another_user
         return Actor.objects.create(
             shortname=shortname,
             longname=longname,
             region=region,
             college=college,
-            adhesiondate='1989',
+            adhesiondate="1989",
             legalrepresentant=another_user,
-            managementcontact=owner_user
+            managementcontact=owner_user,
         )
 
-    def _get_random_contribution(self, actor, regionalnetwork, paymentmethod, year=2020):
+    def _get_random_contribution(
+        self, actor, regionalnetwork, paymentmethod, year=2020
+    ):
         return Contribution.objects.create(
             year=year,
             actor=actor,
             paymentto=regionalnetwork,
             paymentmethod=paymentmethod,
             receivedby=regionalnetwork,
-            amount=30
+            amount=30,
         )
 
     def _get_random_profile(self, user):
-        return Profile.objects.create(
-            user=user
-        )
+        return Profile.objects.create(user=user)
 
-    def _get_relatedactor(self, user, actor, role='admin'):
-        return Relatedactor.objects.create(
-            user=user,
-            actor=actor,
-            role=role
-        )
+    def _get_relatedactor(self, user, actor, role="admin"):
+        return Relatedactor.objects.create(user=user, actor=actor, role=role)
 
     def _get_random_relatedactor(self):
         actor = self._get_random_actor()
         another_user = self._get_random_user()
         return self._get_relatedactor(actor=actor, user=another_user)
 
     def _get_random_integrationstep(self):
         actor = self._get_random_actor()
         return Integrationstep.objects.create(actor=actor)
 
-    def _get_random_interventionzone(self, name='TestInterventionzone'):
+    def _get_random_interventionzone(self, name="TestInterventionzone"):
         return Interventionzone.objects.create(name=name)
 
-    def _get_random_legalstructure(self, name='TestLegalstructure'):
+    def _get_random_legalstructure(self, name="TestLegalstructure"):
         return Legalstructure.objects.create(name=name)
 
-    def _get_random_collegeepa(self, name='TestCollegeepa'):
+    def _get_random_collegeepa(self, name="TestCollegeepa"):
         return Collegeepa.objects.create(name=name)
 
-# --- class Region:
+    # --- class Region:
     # superadmin : view
     def test_super_user_can_list_region(self):
         self.setUpLoggedInUser(is_superuser=True)
         region = self._get_random_region()
 
-        response = self.client.get('/regions/')
+        response = self.client.get("/regions/")
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 1)
+        self.assertEqual(len(response.data["ldp:contains"]), 1)
 
     def test_post_actor_post_save_signal(self):
         self.setUpLoggedInUser(is_superuser=False)
         region = self._get_random_region()
         zone = self._get_random_interventionzone()
         regional_network = self._get_random_regionalnetwork()
         another_user = self._get_random_user()
         request = {
-            "longname":"It's raining again",
-            "shortname":"ITR35",
-            "location":"",
-            "address":"2 Allée de Villebon",
-            "postcode":44000,
-            "city":"Nantes",
-            "lat":47.2226512,
-            "lng":-1.5499481,
-            "complementaddress":"",
-            "region":{"@id": region.urlid},
-            "phone":"346758678Y9",
-            "adhmail":"",
-            "actortype":"soc_citoy",
-            "category":"porteur_exploit",
-            "legalstructure":"",
-            "siren":"",
-            "interventionzone":[{"@id": zone.urlid}],
-            "adhesiondate":"2019",
-            "regionalnetwork":{"@id": regional_network.urlid},
-            "numberpeople":"",
-            "numberemployees":"",
-            "turnover":"",
-            "collegeepa":"",
-            "college":"",
-            "iban":"",
-            "logo":"",
-            "presentation":"",
-            "website":"ww.sfgnfsf.fr",
-            "mail":"sympa@sympa.cool",
-            "legalrepresentant":{"@id":another_user.urlid},
-            "managementcontact":{"@id":another_user.urlid},
-            "@context":{"@vocab":"http://happy-dev.fr/owl/#",
-                        "rdf":"http://www.w3.org/1999/02/22-rdf-syntax-ns#",
-                        "rdfs":"http://www.w3.org/2000/01/rdf-schema#",
-                        "ldp":"http://www.w3.org/ns/ldp#",
-                        "foaf":"http://xmlns.com/foaf/0.1/","name":"rdfs:label","acl":"http://www.w3.org/ns/auth/acl#","permissions":"acl:accessControl","mode":"acl:mode","geo":"http://www.w3.org/2003/01/geo/wgs84_pos#","lat":"geo:lat","lng":"geo:long","subject":"http://happy-dev.fr/owl/#subject"}}
+            "longname": "It's raining again",
+            "shortname": "ITR35",
+            "location": "",
+            "address": "2 Allée de Villebon",
+            "postcode": 44000,
+            "city": "Nantes",
+            "lat": 47.2226512,
+            "lng": -1.5499481,
+            "complementaddress": "",
+            "region": {"@id": region.urlid},
+            "phone": "346758678Y9",
+            "adhmail": "",
+            "actortype": "soc_citoy",
+            "category": "porteur_exploit",
+            "legalstructure": "",
+            "siren": "",
+            "interventionzone": [{"@id": zone.urlid}],
+            "adhesiondate": "2019",
+            "regionalnetwork": {"@id": regional_network.urlid},
+            "numberpeople": "",
+            "numberemployees": "",
+            "turnover": "",
+            "collegeepa": "",
+            "college": "",
+            "iban": "",
+            "logo": "",
+            "presentation": "",
+            "website": "ww.sfgnfsf.fr",
+            "mail": "sympa@sympa.cool",
+            "legalrepresentant": {"@id": another_user.urlid},
+            "managementcontact": {"@id": another_user.urlid},
+            "@context": {
+                "@vocab": "http://startinblox.com/owl/#",
+                "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
+                "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
+                "ldp": "http://www.w3.org/ns/ldp#",
+                "foaf": "http://xmlns.com/foaf/0.1/",
+                "name": "rdfs:label",
+                "acl": "http://www.w3.org/ns/auth/acl#",
+                "permissions": "acl:accessControl",
+                "mode": "acl:mode",
+                "geo": "http://www.w3.org/2003/01/geo/wgs84_pos#",
+                "lat": "geo:lat",
+                "lng": "geo:long",
+                "subject": "http://startinblox.com/owl/#subject",
+            },
+        }
 
-        response = self.client.post('/actors/', data=json.dumps(request), content_type='application/ld+json')
+        response = self.client.post(
+            "/actors/", data=json.dumps(request), content_type="application/ld+json"
+        )
         self.assertEqual(response.status_code, 201)
         # test effects of signal receiver
         self.assertGreater(Relatedactor.objects.count(), 0)
         self.assertGreater(Contribution.objects.count(), 0)
-
-
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/tests/runner.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/tests/runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import sys
-import yaml
 
 import django
+import yaml
 from django.conf import settings as django_settings
 from djangoldp.conf.ldpsettings import LDPSettings
 from djangoldp.tests.server_settings import yaml_config
 
 # this is where we configure the server settings that we will run our tests with
 config = {
     # add the packages to the reference list
-    'ldppackages': ['djangoldp_energiepartagee', 'djangoldp_energiepartagee.tests'],
-
+    "ldppackages": ["djangoldp_energiepartagee", "djangoldp_energiepartagee.tests"],
     # required values for server
-    'server': {
-        'SECRET_KEY': "$r&)p-4k@h5b!1yrft6&q%j)_p$lxqh6#)jeeu0z1iag&y&wdu",
-        'AUTH_USER_MODEL': 'tests.User',
-        'REST_FRAMEWORK': {
-            'DEFAULT_PAGINATION_CLASS': 'djangoldp.pagination.LDPPagination',
-            'PAGE_SIZE': 5
+    "server": {
+        "SECRET_KEY": "$r&)p-4k@h5b!1yrft6&q%j)_p$lxqh6#)jeeu0z1iag&y&wdu",
+        "AUTH_USER_MODEL": "tests.User",
+        "REST_FRAMEWORK": {
+            "DEFAULT_PAGINATION_CLASS": "djangoldp.pagination.LDPPagination",
+            "PAGE_SIZE": 5,
         },
         # map the config of the core settings (avoid asserts to fail)
-        'SITE_URL': 'http://happy-dev.fr',
-        'BASE_URL': 'http://happy-dev.fr',
-        'SEND_BACKLINKS': False,
-        'JABBER_DEFAULT_HOST': None,
-        'PERMISSIONS_CACHE': False,
+        "SITE_URL": "http://startinblox.com",
+        "BASE_URL": "http://startinblox.com",
+        "SEND_BACKLINKS": False,
+        "JABBER_DEFAULT_HOST": None,
+        "PERMISSIONS_CACHE": False,
         # 'ANONYMOUS_USER_NAME': None,
-        'SERIALIZER_CACHE': False
-    }
+        "SERIALIZER_CACHE": False,
+    },
 }
 ldpsettings = LDPSettings(config)
 ldpsettings.config = yaml.safe_load(yaml_config)
 
 django_settings.configure(ldpsettings)
 
 django.setup()
 from django.test.runner import DiscoverRunner
 
 test_runner = DiscoverRunner(verbosity=1)
 
 # this is where we link our test classes to the runner
-failures = test_runner.run_tests([
-    'djangoldp_energiepartagee.tests.tests_permissions',
-    'djangoldp_energiepartagee.tests.tests_post',
-])
+failures = test_runner.run_tests(
+    [
+        "djangoldp_energiepartagee.tests.tests_permissions",
+        "djangoldp_energiepartagee.tests.tests_post",
+    ]
+)
 if failures:
     sys.exit(failures)
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/oidc_settings.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/oidc_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 from djangoldp_energiepartagee.models import Contribution
 from oidc_provider.views import userinfo
 from django.utils.translation import gettext_lazy as _
 from oidc_provider.lib.claims import ScopeClaims
 
+
 class ActorsScopeClaims(ScopeClaims):
     info_moncompte = (
-        _(u'Moncompte'),
-        _(u'This is the custom claim providing info on all EnergiePartagee information associated with the user.'),
+        _("Moncompte"),
+        _(
+            "This is the custom claim providing info on all EnergiePartagee information associated with the user."
+        ),
     )
 
     def scope_moncompte(self):
         # self.user - Django user instance.
         # self.userinfo - Dict returned by OIDC_USERINFO function.
         # self.scopes - List of scopes requested.
         # self.client - Client requesting this claims.
         dic = {}
 
         if self.user.is_authenticated:
             # Get list of related actors of current user
             from djangoldp_energiepartagee.models import Relatedactor, Contribution
+
             user_actors_id = Relatedactor.get_user_actors_id(user=self.user)
 
             # Get membership status of the actors
             activeContributions = Contribution.objects.filter(
                 actor_id__in=user_actors_id,
-                year = Contribution.get_current_contribution_year()
+                year=Contribution.get_current_contribution_year(),
             )
 
             if activeContributions.__len__() > 0:
                 dic = {
-                    'membership': 'active',
+                    "membership": "active",
                 }
             else:
                 dic = {
-                    'membership': 'inactive',
+                    "membership": "inactive",
                 }
 
         return dic
 
     # If you want to change the description of the profile scope, you can redefine it.
     info_profile = (
-        _(u'Profile'),
-        _(u'Another description.'),
+        _("Profile"),
+        _("Another description."),
     )
 
     def scope_profile(self):
         # self.user - Django user instance.
         # self.userinfo - Dict returned by OIDC_USERINFO function.
         # self.scopes - List of scopes requested.
         # self.client - Client requesting this claims.
         dic = {}
 
         if self.user.is_authenticated:
             dic = {
-                'username': self.user.username,
-                'email': self.user.email,
-                'first_name': self.user.first_name,
-                'last_name': self.user.last_name,
-                'name': self.user.get_full_name()
+                "username": self.user.username,
+                "email": self.user.email,
+                "first_name": self.user.first_name,
+                "last_name": self.user.last_name,
+                "name": self.user.get_full_name(),
             }
 
         return dic
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/registration/password_reset_form.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/registration/login.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/waiting_reminder.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/waiting_reminder.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/actor_update.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/actor_update.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/new_join_request.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/new_join_request.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/subscription_call.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/subscription_call.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/join_actor_validated.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/join_actor_validated.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/subscription_reminder.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/subscription_reminder.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/html/join_actor_denied.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/html/join_actor_denied.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/txt/actor_update.txt` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/txt/actor_update.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/txt/subscription_call.txt` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/txt/subscription_call.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/emails/txt/subscription_reminder.txt` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/emails/txt/subscription_reminder.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/oidc_provider/authorize.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/base.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/base.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/django_registration/activation_complete.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/django_registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/django_registration/registration_form.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/django_registration/registration_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/pdf/contribution_receipt.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/pdf/contribution_receipt.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/templates/pdf/contribution_call.html` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/templates/pdf/contribution_call.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/admin.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/djangoldp_urls.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/filters/related_actor_filter_backend.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/filters/related_actor_filter_backend.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from django.db.models import Q
 from rest_framework_guardian.filters import ObjectPermissionsFilter
 
 
 #######
 # Returns the related actors on which the user is admin
 # Or the complete list if the user is superuser
 #######
 class RelatedactorFilterBackend(ObjectPermissionsFilter):
     def filter_queryset(self, request, queryset, view):
         if not request.user.is_authenticated or request.user.is_anonymous:
             return queryset.none()
         elif request.user.is_superuser:
             return queryset
         else:
-            from djangoldp_energiepartagee.models.related_actor import Relatedactor
-
-            user_actors_id = Relatedactor.get_user_actors_id(user=request.user)
-            return queryset.filter(actor_id__in=user_actors_id)
+            return queryset.filter(
+                Q(actor__members__user=request.user)
+                | Q(actor__region__admins=request.user)
+            )
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/css/registration.css` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/css/registration.css`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/css/css_ep.css` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/css/css_ep.css`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/css/css_amorce.css` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/css/css_amorce.css`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/fonts/Inter-roman.var.woff2` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/fonts/Inter-roman.var.woff2`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/fonts/Inter-italic.var.woff2` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/fonts/Inter-italic.var.woff2`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/img/Amorcelogo.svg` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/img/Amorcelogo.svg`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/static/img/EPlogo.svg` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/static/img/EPlogo.svg`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/export_contributions_all.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/export_contributions_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import csv
 
 from django.http import HttpResponse
-
-from rest_framework.views import APIView
 from djangoldp.views import NoCSRFAuthentication
+from rest_framework.views import APIView
 
 from djangoldp_energiepartagee.filters import ContributionFilterBackend
-
 from djangoldp_energiepartagee.models.contribution import Contribution
-
+from djangoldp_energiepartagee.permissions import EPBasePermission
 from djangoldp_energiepartagee.views.plain_text_parser import PlainTextParser
 
-from djangoldp_energiepartagee.permissions import SuperUserOnlyPermissions
-
 
-#export csv all
+# export csv all
 class ExportContributionsAll(APIView):
     authentication_classes = [NoCSRFAuthentication]
-    permission_classes = [SuperUserOnlyPermissions]
+    permission_classes = [EPBasePermission]
     model = Contribution
     parser_classes = (PlainTextParser,)
 
     def dispatch(self, request, *args, **kwargs):
-        response = super(ExportContributionsAll, self).dispatch(request, *args, **kwargs)
-        response["Access-Control-Allow-Origin"] = request.headers.get('origin')
+        response = super(ExportContributionsAll, self).dispatch(
+            request, *args, **kwargs
+        )
+        response["Access-Control-Allow-Origin"] = request.headers.get("origin")
         response["Access-Control-Allow-Methods"] = "POST, GET"
-        response["Access-Control-Allow-Headers"] = "authorization, Content-Type, if-match, accept, sentry-trace, DPoP"
+        response["Access-Control-Allow-Headers"] = (
+            "authorization, Content-Type, if-match, accept, sentry-trace, DPoP"
+        )
         response["Access-Control-Expose-Headers"] = "Location, User"
-        response["Access-Control-Allow-Credentials"] = 'true'
+        response["Access-Control-Allow-Credentials"] = "true"
         response["Accept-Post"] = "application/json"
         response["Accept"] = "*/*"
 
         if request.user.is_authenticated:
             try:
-                response['User'] = request.user.webid()
+                response["User"] = request.user.webid()
             except AttributeError:
                 pass
         return response
 
-
     def post(self, request):
         delimiter_type = ";"
         response = HttpResponse(content_type="text/csv")
         response["Content-Disposition"] = 'attachment; filename="export_actors.csv"'
         response.write("\ufeff".encode("utf8"))
         writer = csv.writer(response, delimiter=delimiter_type)
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/contributions_call.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/contributions_call.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/generate_pdf_receipt.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/generate_pdf_receipt.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/contributions_reminder.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/contributions_reminder.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/export_contributions.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/export_contributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 
 # export csv - Old button (export selected lines)
 class ExportContributions(APIView):
     authentication_classes = (NoCSRFAuthentication,)
 
     def dispatch(self, request, *args, **kwargs):
         response = super(ExportContributions, self).dispatch(request, *args, **kwargs)
-        response["Access-Control-Allow-Origin"] = request.headers.get('origin')
+        response["Access-Control-Allow-Origin"] = request.headers.get("origin")
         response["Access-Control-Allow-Methods"] = "POST, GET"
-        response["Access-Control-Allow-Headers"] = "authorization, Content-Type, if-match, accept, sentry-trace, DPoP"
+        response["Access-Control-Allow-Headers"] = (
+            "authorization, Content-Type, if-match, accept, sentry-trace, DPoP"
+        )
         response["Access-Control-Expose-Headers"] = "Location, User"
-        response["Access-Control-Allow-Credentials"] = 'true'
+        response["Access-Control-Allow-Credentials"] = "true"
         response["Accept-Post"] = "application/json"
         response["Accept"] = "*/*"
 
         if request.user.is_authenticated:
             try:
-                response['User'] = request.user.webid()
+                response["User"] = request.user.webid()
             except AttributeError:
                 pass
         return response
 
     def post(self, request):
         delimiter_type = ";"
         response = HttpResponse(content_type="text/csv")
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/utils/render_to_pdf.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/utils/render_to_pdf.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/waiting_members_action.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/waiting_members_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,34 +50,37 @@
                     title = "Energie Partagée"
                     if getattr(settings, "IS_AMORCE", False):
                         title = "AMORCE"
                     if request.data == "reminder":
                         specificdata = {
                             "email_text": "emails/txt/waiting_reminder.txt",
                             "email_html": "emails/html/waiting_reminder.html",
-                            "email_title": title + " - Vous avez une demande en attente pour l'acteur ",
+                            "email_title": title
+                            + " - Vous avez une demande en attente pour l'acteur ",
                             "status": "",
                             "email": instance.actor.managementcontact.email,
                         }
                         obj.reminderdate = date.today()
                         obj.save()
                     else:
                         if request.data == "refuse":
                             specificdata = {
                                 "email_text": "emails/txt/join_actor_denied.txt",
                                 "email_html": "emails/html/join_actor_denied.html",
-                                "email_title": title + " - Votre demande de rejoindre l'acteur ",
+                                "email_title": title
+                                + " - Votre demande de rejoindre l'acteur ",
                                 "status": " a été refusée",
                                 "email": instance.user.email,
                             }
                         else:
                             specificdata = {
                                 "email_text": "emails/txt/join_actor_validated.txt",
                                 "email_html": "emails/html/join_actor_validated.html",
-                                "email_title": title + " - Votre demande de rejoindre l'acteur ",
+                                "email_title": title
+                                + " - Votre demande de rejoindre l'acteur ",
                                 "status": " a été acceptée",
                                 "email": instance.user.email,
                             }
                         obj.role = request.data
                         obj.save()
                 text_message = loader.render_to_string(
                     specificdata["email_text"],
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/contributions.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/contributions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/contributions_ventilation.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/contributions_ventilation.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/contributions_actor_update.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/contributions_actor_update.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/views/generate_pdf_call.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/views/generate_pdf_call.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/permissions/actor_permissions.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/permissions/ep_related_actor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,73 @@
-from djangoldp.permissions import LDPBasePermission
+from djangoldp_energiepartagee.filters import RelatedactorFilterBackend
 
+from .ep_actor import is_member
+from .ep_base import EPBasePermission
+from .ep_regional_admin import is_regional_admin
 
-####
-# Only the admin of an actor can modify it (and superusers of course)
-# Members can view the actor
-####
-class ActorPermissions(LDPBasePermission):
-    permissions = {"add"}
+
+class EPRelatedActorPermissions(EPBasePermission):
+    filter_backend = RelatedactorFilterBackend
 
     def get_permissions(self, user, model, obj=None):
         if user.is_anonymous:
-            return {}
+            return set()
 
-        """returns the permissions the user has on a given model or on a given object"""
-        perms = super().get_permissions(user, model, obj)
-        if user.is_superuser:
-            return perms.union({"view", "add", "change", "delete"})
+        if obj:
+            membership = is_member(user, obj)
+            if is_regional_admin(user, obj) or membership == "admin":
+                return {"view", "add", "change", "delete"}
+            elif membership == "membre":
+                return {"view", "add"}
+            elif membership:
+                return {"view"}
 
-        if obj and self.is_admin(user, obj):
-            return perms.union({"view", "add", "change", "delete"})
+        from djangoldp_energiepartagee.models.region import Region
 
-        if obj and self.is_member_or_admin(user, obj):
-            return perms.union({"view", "add"})
+        if Region.objects.filter(admins=user).exists():
+            return {"view", "add", "change", "delete"}
 
-        return perms
+        return {"view", "add"}
 
     def has_permission(self, request, view):
-        if request.method == "OPTIONS":
-            return True
         if request.user.is_anonymous:
             return False
-        # First, allow all GET requests by members or admins.
-        if request.method == "GET":
-            return self.is_member_or_admin(request.user)
-        # For PUT/PATCH requests, ensure the user is an admin.
-        elif request.method in ["PUT", "PATCH"]:
-            return self.is_admin(request.user)
-        # You can add logic for other methods if needed.
-        else:
-            return False
 
-    def has_object_permission(self, request, view, obj):
-        if request.method == "OPTIONS":
-            return True
-        if request.user.is_anonymous:
-            return False
-        # For GET requests, check if the user is a member or an admin for the given object.
-        if request.method == "GET":
-            return self.is_member_or_admin(request.user, obj)
-        # For PUT/PATCH requests, ensure the user is an admin for the given object.
-        elif request.method in ["PUT", "PATCH"]:
-            return self.is_admin(request.user, obj)
-        else:
-            return False
+        if request.method == "POST":
+            role = request.data.get("role")
+            if role in ("admin", "membre", "refused"):
+                actor_urlid = request.data.get("actor")["@id"]
+                if actor_urlid:
+                    if role == "admin":
+                        return request.user.relatedactor_set.filter(
+                            actor__urlid=actor_urlid,
+                            role__in=("admin"),
+                        ).exists()
+                    return request.user.relatedactor_set.filter(
+                        actor__urlid=actor_urlid,
+                        role__in=("admin", "members"),
+                    ).exists()
+                return False
+            elif role is None and request.user.is_authenticated:
+                return True
 
-    def is_member_or_admin(self, user, obj=None):
-        from djangoldp_energiepartagee.models.related_actor import Relatedactor
+        return super().has_permission(request, view)
 
-        """Check if the user is a member or admin. If obj is provided, check is specific to that object."""
-        role_filter = {"user": user, "role__in": ["membre", "admin"]}
-        if obj:
-            role_filter["actor"] = obj
-        return Relatedactor.objects.filter(**role_filter).exists()
-
-    def is_admin(self, user, obj=None):
-        from djangoldp_energiepartagee.models.related_actor import Relatedactor
-
-        """Check if the user is an admin. If obj is provided, check is specific to that object."""
-        role_filter = {"user": user, "role": "admin"}
+    def has_object_permission(self, request, view, obj):
         if obj:
-            role_filter["actor"] = obj
-        return Relatedactor.objects.filter(**role_filter).exists()
-
-
-class SuperUserOnlyPermissions(LDPBasePermission):
-    permissions = {"view", "add", "change", "delete"}
-
-    def check_permission(self, user, model, obj):
-        if user.is_superuser:
-            return True
+            # Direct permission if the user is the same as the object's user
+            if request.user == obj.user:
+                if obj.role == "admin":
+                    return request.method in ["GET", "PUT", "PATCH", "DELETE", "POST"]
+                elif obj.role == "membre" or obj.role is None or obj.role == "":
+                    return request.method == "GET"
+
+            # Additional checks for admin/member roles related to the actor
+            if hasattr(obj, "actor") and obj.actor is not None:
+                if obj.actor.members.filter(user=request.user, role="admin").exists():
+                    return request.method in ["GET", "PUT", "PATCH", "DELETE", "POST"]
+            return super().has_object_permission(
+                request, view, obj
+            ) or is_regional_admin(request.user, obj)
 
+        # Default to False if none of the above conditions are met
         return False
-
-    def has_object_permission(self, request, view, obj=None):
-        return self.check_permission(request.user, view.model, obj)
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/auth/backends.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/auth/backends.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,46 +6,50 @@
 from django.core.exceptions import ValidationError
 from rest_framework.exceptions import AuthenticationFailed
 from rest_framework import status
 from django.core.validators import validate_email
 from django.conf import settings
 from jwkest import BadSyntax
 from jwkest.jwt import JWT
-from jwt.utils import (base64url_decode, base64url_encode)
-from oidc_provider.lib.utils.dpop import verify_signature, verify_dpop_proof, verify_thumbprint
+from jwt.utils import base64url_decode, base64url_encode
+from oidc_provider.lib.utils.dpop import (
+    verify_signature,
+    verify_dpop_proof,
+    verify_thumbprint,
+)
 from oidc_provider.models import Token
 from oidc_provider.views import JwksView
 import inspect
 from oidc_provider.models import Client
 
 from djangoldp_account.auth.solid import Solid
 from djangoldp_account.errors import LDPLoginError
 
 UserModel = get_user_model()
 
-class BasicAuthBackend(AllowAllUsersModelBackend):
-  def validate_bearer_token(self, token):
-    try:
-        token = Token.objects.get(access_token=token)
-        if token:
-          client_email = token.client.contact_email
-          user = UserModel.objects.filter(email=client_email).first()
-
-          if self.user_can_authenticate(user):
-            return user
-    except Exception as e:
-        raise e
-
-    return None
-
-  def authenticate(self, request, *args, **kwargs):
-    if 'HTTP_AUTHORIZATION' in request.META:
-      jwt = request.META['HTTP_AUTHORIZATION']
 
-      if jwt.lower().startswith("bearer"):
-        jwt = jwt[7:]
+class BasicAuthBackend(AllowAllUsersModelBackend):
+    def validate_bearer_token(self, token):
+        try:
+            token = Token.objects.get(access_token=token)
+            if token:
+                client_email = token.client.contact_email
+                user = UserModel.objects.filter(email=client_email).first()
+
+                if self.user_can_authenticate(user):
+                    return user
+        except Exception as e:
+            raise e
+
+        return None
+
+    def authenticate(self, request, *args, **kwargs):
+        if "HTTP_AUTHORIZATION" in request.META:
+            jwt = request.META["HTTP_AUTHORIZATION"]
 
-        # make an attempt assuming Bearer token if not recognised or not specified
-        return self.validate_bearer_token(jwt)
+            if jwt.lower().startswith("bearer"):
+                jwt = jwt[7:]
 
-    return ModelBackend().authenticate(request, *args, **kwargs)
+                # make an attempt assuming Bearer token if not recognised or not specified
+                return self.validate_bearer_token(jwt)
 
+        return ModelBackend().authenticate(request, *args, **kwargs)
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0014_auto_20210121_1750.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0014_auto_20210121_1750.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0045_auto_20210222_2353.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0045_auto_20210222_2353.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0019_auto_20210124_1728.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0019_auto_20210124_1728.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0082_alter_capitaldistribution_actor_and_more.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0082_alter_capitaldistribution_actor_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0055_auto_20210421_1500.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0055_auto_20210421_1500.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0001_initial.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0076_alter_actor_options_alter_college_options_and_more.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0076_alter_actor_options_alter_college_options_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0050_contribution_usercontact.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0050_contribution_usercontact.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0015_auto_20210122_1044.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0015_auto_20210122_1044.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0081_alter_citizenproject_status.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0081_alter_citizenproject_status.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0025_auto_20210129_1841.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0025_auto_20210129_1841.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0068_contribution_discount.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0068_contribution_discount.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0072_alter_relatedactor_role.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0072_alter_relatedactor_role.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0021_auto_20210125_1559.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0021_auto_20210125_1559.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0007_auto_20210120_1213.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0007_auto_20210120_1213.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0032_auto_20210209_1238.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0032_auto_20210209_1238.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0070_contribution_updatereminderdate_and_more.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0070_contribution_updatereminderdate_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0058_auto_20211108_1909.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0058_auto_20211108_1909.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0009_auto_20210120_1439.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0009_auto_20210120_1439.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0059_auto_20220114_1050.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0059_auto_20220114_1050.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0048_auto_20210225_1136.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0048_auto_20210225_1136.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0085_citizenproject_wp_project_url_and_more.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0085_citizenproject_wp_project_url_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0009_auto_20210120_1911.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0009_auto_20210120_1911.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0011_auto_20210120_1450.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0011_auto_20210120_1450.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0031_auto_20210209_1235.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0031_auto_20210209_1235.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0071_relatedactor_createdate.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0071_relatedactor_createdate.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0062_auto_20220128_1047.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0062_auto_20220128_1047.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0052_auto_20210323_1424.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0052_auto_20210323_1424.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0003_profile_user.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0003_profile_user.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0053_auto_20210402_1014.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0053_auto_20210402_1014.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0040_auto_20210216_2227.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0040_auto_20210216_2227.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0061_auto_20220114_1140.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0061_auto_20220114_1140.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0016_auto_20210122_1146.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0016_auto_20210122_1146.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0060_auto_20220114_1113.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0060_auto_20220114_1113.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0027_auto_20210201_1617.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0027_auto_20210201_1617.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0004_auto_20210114_1652.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0004_auto_20210114_1652.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0080_alter_citizenproject_status.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0080_alter_citizenproject_status.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0024_auto_20210125_2207.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0024_auto_20210125_2207.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0067_discount_actor_villageoise.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0067_discount_actor_villageoise.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0012_auto_20210120_1553.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0012_auto_20210120_1553.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0035_auto_20210215_1329.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0035_auto_20210215_1329.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0047_auto_20210223_1059.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0047_auto_20210223_1059.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0038_auto_20210216_1721.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0038_auto_20210216_1721.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0063_auto_20220128_1051.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0063_auto_20220128_1051.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0078_citizen_project_communication_profile_contract_type_and_more.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0078_citizen_project_communication_profile_contract_type_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0006_auto_20210119_1237.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0006_auto_20210119_1237.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0066_alter_actor_options_alter_college_options_and_more.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0066_alter_actor_options_alter_college_options_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0010_auto_20210120_1442.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0010_auto_20210120_1442.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0036_auto_20210216_1714.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0036_auto_20210216_1714.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0056_auto_20210430_1127.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0056_auto_20210430_1127.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0079_rename_capital_distribution_capitaldistribution_and_more.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0079_rename_capital_distribution_capitaldistribution_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0037_auto_20210216_1717.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0037_auto_20210216_1717.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0083_alter_actor_options_and_more.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0083_alter_actor_options_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0005_auto_20210118_1407.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0005_auto_20210118_1407.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0064_auto_20220203_1721.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0064_auto_20220203_1721.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0029_auto_20210204_1428.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0029_auto_20210204_1428.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0023_auto_20210125_1646.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0023_auto_20210125_1646.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0074_alter_relatedactor_role.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0074_alter_relatedactor_role.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0042_auto_20210219_1409.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0042_auto_20210219_1409.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0028_auto_20210202_1625.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0028_auto_20210202_1625.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0033_auto_20210209_1258.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0033_auto_20210209_1258.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0034_auto_20210209_1538.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0034_auto_20210209_1538.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0008_auto_20210120_1215.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0008_auto_20210120_1215.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0026_auto_20210201_1343.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0026_auto_20210201_1343.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0018_auto_20210122_1229.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0018_auto_20210122_1229.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0020_auto_20210125_1131.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0020_auto_20210125_1131.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/migrations/0054_auto_20210419_2106.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/migrations/0054_auto_20210419_2106.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/communication_profile.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/communication_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-
 from djangoldp.models import Model
-from djangoldp.permissions import AuthenticatedOnly, ReadOnly
+from djangoldp.permissions import InheritPermissions
 
 from djangoldp_energiepartagee.models.citizen_project import CitizenProject
 
 COMMUNICATION_PROFILE_REPLICABILITY_CHOICES = [
     ("easy", "Facilement"),
     ("hard", "Difficilement"),
     ("no", "Non"),
@@ -53,14 +52,15 @@
     )
     additional_informations = models.CharField(
         max_length=250, blank=True, null=True, verbose_name="Infos diverses"
     )
 
     class Meta(Model.Meta):
         ordering = ["pk"]
-        permission_classes = [AuthenticatedOnly, ReadOnly]
+        permission_classes = [InheritPermissions]
+        inherit_permissions = ["citizen_project"]
         rdf_type = "energiepartagee:communication_profile"
         verbose_name = _("Profil de communication")
         verbose_name_plural = _("Profils de communication")
 
     def __str__(self):
         return self.urlid
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/actor.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/actor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from django.conf import settings
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-
 from djangoldp.models import Model
-from djangoldp.permissions import ReadAndCreate
-
-from djangoldp_energiepartagee.permissions import ActorPermissions
+from djangoldp.permissions import AnonymousReadOnly, ReadAndCreate
 
-from djangoldp_energiepartagee.models.region import *
 from djangoldp_energiepartagee.models.college import *
-from djangoldp_energiepartagee.models.regional_network import *
-from djangoldp_energiepartagee.models.intervention_zone import *
-from djangoldp_energiepartagee.models.legal_structure import *
 from djangoldp_energiepartagee.models.college_epa import *
-from djangoldp_energiepartagee.models.integration_step import *
 from djangoldp_energiepartagee.models.discount import *
+from djangoldp_energiepartagee.models.integration_step import *
+from djangoldp_energiepartagee.models.intervention_zone import *
+from djangoldp_energiepartagee.models.legal_structure import *
+from djangoldp_energiepartagee.models.region import *
+from djangoldp_energiepartagee.models.regional_network import *
+from djangoldp_energiepartagee.permissions import (
+    EPActorPermission,
+    EPRegionalAdminPermission,
+)
 
 ACTORTYPE_CHOICES = [
     ("soc_citoy", "Sociétés Citoyennes"),
     ("collectivite", "Collectivités"),
     ("structure", "Structures d’Accompagnement"),
     ("partenaire", "Partenaires"),
 ]
@@ -277,15 +278,22 @@
         # apply villageoise discount for the actors
         if self.villageoise is True:
             amount = amount * (100 - float(discountvillageoise)) / 100
         return amount
 
     class Meta(Model.Meta):
         ordering = ["shortname"]
-        permission_classes = [ReadAndCreate | ActorPermissions]
+        permission_classes = [
+            AnonymousReadOnly
+            & (EPActorPermission | EPRegionalAdminPermission | ReadAndCreate)
+        ]
+        permission_roles = {
+            "member": {"perms": {"view", "add"}},
+            "admin": {"perms": {"view", "add", "change", "delete"}},
+        }
         nested_fields = [
             "members",
             "integrationstep",
             "contributions",
             "capital_distributions",
             "partner_of",
             "founded_projects",
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/contribution.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/contribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from datetime import date
 
 from django.conf import settings
 from django.db import models
 from django.db.models import Max
 from django.utils.decorators import classonlymethod
 from django.utils.translation import gettext_lazy as _
-
 from djangoldp.models import Model
-from djangoldp.permissions import AuthenticatedOnly
-
-from djangoldp_energiepartagee.permissions import ContributionPermissions
 
-from djangoldp_energiepartagee.models.regional_network import *
-from djangoldp_energiepartagee.models.payment_method import *
-from djangoldp_energiepartagee.models.discount import *
 from djangoldp_energiepartagee.models.actor import *
 from djangoldp_energiepartagee.models.contribution import *
+from djangoldp_energiepartagee.models.discount import *
+from djangoldp_energiepartagee.models.payment_method import *
+from djangoldp_energiepartagee.models.regional_network import *
+from djangoldp_energiepartagee.permissions import EPContributionPermission
 
 CONTRIBUTION_CHOICES = [
     ("appel_a_envoye", "Appel à envoyer"),
     ("appel_ok", "Appel envoyé"),
     ("relance", "Relancé"),
     ("a_ventiler", "A ventiler"),
     ("valide", "Validé"),
@@ -192,15 +189,19 @@
             contributionnumber=Contribution._get_next_contribution_number(),
             paymentto=actor.regionalnetwork,
         )
         c.save()
 
     class Meta(Model.Meta):
         ordering = ["pk"]
-        permission_classes = [AuthenticatedOnly & ContributionPermissions]
+        permission_classes = [EPContributionPermission]
+        permission_roles = {
+            "member": {"perms": set()},
+            "admin": {"perms": {"view"}},
+        }
         rdf_type = "energiepartagee:contribution"
         serializer_fields = [
             "actor",
             "year",
             "numberpeople",
             "numberemployees",
             "turnover",
@@ -219,7 +220,8 @@
             "factureventilation",
             "callcontact",
             "amountincents",
             "updatereminderdate",
         ]
         verbose_name = _("Contribution")
         verbose_name_plural = _("Contributions")
+        depth = 2
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/production_site.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/citizen_project.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,150 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-
 from djangoldp.models import Model
-from djangoldp.permissions import AuthenticatedOnly, ReadOnly
+from djangoldp.permissions import InheritPermissions
 
-from djangoldp_energiepartagee.models.citizen_project import CitizenProject
+from djangoldp_energiepartagee.models.actor import Actor
 from djangoldp_energiepartagee.models.region import Region
+from djangoldp_energiepartagee.permissions import EPRegionalAdminPermission
+
+CITIZEN_PROJECT_STATUS_CHOICES = [
+    ("draft", "Brouillon"),
+    ("validation", "En cours de validation"),
+    ("published", "Publié"),
+    ("retired", "Dépublié"),
+]
 
 
-class ProductionSite(Model):
-    citizen_project = models.ForeignKey(
-        CitizenProject,
+class CitizenProject(Model):
+    founder = models.ForeignKey(
+        Actor,
         blank=True,
         null=True,
         on_delete=models.CASCADE,
-        verbose_name="Projet citoyen",
-        related_name="production_sites",
+        verbose_name="Fondateur",
+        related_name="founded_projects",
     )
     name = models.CharField(max_length=50, blank=True, null=True, verbose_name="Name")
-    description = models.TextField(blank=True, null=True, verbose_name="Description")
-    reference_unit = models.TextField(
-        blank=True, null=True, verbose_name="Unité de référence"
-    )
-    progress_status = models.TextField(
-        blank=True, null=True, verbose_name="Description"
-    )
-    total_development_budget = models.TextField(
-        blank=True, null=True, verbose_name="Description"
+    short_description = models.TextField(
+        blank=True, null=True, verbose_name="Courte description"
     )
-    total_investment_budget = models.TextField(
-        blank=True, null=True, verbose_name="Description"
-    )
-    yearly_turnover = models.TextField(
-        blank=True, null=True, verbose_name="Description"
+    city = models.CharField(max_length=50, blank=True, null=True, verbose_name="Ville")
+    postcode = models.CharField(
+        max_length=20, blank=True, null=True, verbose_name="Code Postal"
     )
     address = models.CharField(
         max_length=250, blank=True, null=True, verbose_name="Adresse"
     )
-    city = models.CharField(max_length=50, blank=True, null=True, verbose_name="Ville")
-    department = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Département"
-    )
+    # region = models.CharField(max_length=50, blank=True, null=True, verbose_name="Région")
     region = models.ForeignKey(
         Region,
         max_length=50,
         blank=True,
         null=True,
         on_delete=models.SET_NULL,
         verbose_name="Région",
-        related_name="production_sites",
+        related_name="projects",
     )
-    lat = models.DecimalField(
-        max_digits=30,
-        decimal_places=25,
-        blank=True,
-        null=True,
-        verbose_name="Lattitude",
+    department = models.CharField(
+        max_length=50, blank=True, null=True, verbose_name="Département"
     )
-    lng = models.DecimalField(
-        max_digits=30,
-        decimal_places=25,
+    action_territory = models.CharField(
+        max_length=50,
         blank=True,
         null=True,
-        verbose_name="Longitude",
+        verbose_name="Territoire d'action du projet",
+    )
+    picture = models.CharField(
+        max_length=250, blank=True, null=True, verbose_name="Photo"
+    )
+    video = models.CharField(
+        max_length=250, blank=True, null=True, verbose_name="Vidéo"
+    )
+    website = models.CharField(
+        max_length=50, blank=True, null=True, verbose_name="Site"
     )
-    expected_commissionning_yearl = models.CharField(
+    facebook_link = models.CharField(
+        max_length=250, blank=True, null=True, verbose_name="Facebook"
+    )
+    linkedin_link = models.CharField(
+        max_length=250, blank=True, null=True, verbose_name="LinkedIn"
+    )
+    twitter_link = models.CharField(
+        max_length=250, blank=True, null=True, verbose_name="Twitter"
+    )
+    instagram_link = models.CharField(
+        max_length=250, blank=True, null=True, verbose_name="Instragram"
+    )
+    contact_picture = models.CharField(
+        max_length=250, blank=True, null=True, verbose_name="Contact: Photo"
+    )
+    contact_name = models.CharField(
+        max_length=50, blank=True, null=True, verbose_name="Contact: Nom"
+    )
+    contact_first_name = models.CharField(
+        max_length=50, blank=True, null=True, verbose_name="Contact: Prénom"
+    )
+    contact_email = models.CharField(
+        max_length=50, blank=True, null=True, verbose_name="Contact: Email"
+    )
+    contact_phone = models.CharField(
+        max_length=50, blank=True, null=True, verbose_name="Contact: Téléphone"
+    )
+    contact_visibility = models.BooleanField(
+        blank=True, null=True, verbose_name="Visibilité du contact", default=False
+    )
+    status = models.CharField(
+        choices=CITIZEN_PROJECT_STATUS_CHOICES,
         max_length=50,
         blank=True,
         null=True,
-        verbose_name="Année de mise en service prévue",
+        verbose_name="Etat d'avancement du projet",
     )
-    effective_commissionning_yearl = models.CharField(
-        max_length=50,
+    lat = models.DecimalField(
+        max_digits=30,
+        decimal_places=25,
         blank=True,
         null=True,
-        verbose_name="Année de mise en service effective",
-    )
-    picture = models.CharField(
-        max_length=250, blank=True, null=True, verbose_name="Photo"
+        verbose_name="Latitude",
     )
-    investment_capacity_ratio = models.CharField(
-        max_length=50,
+    lng = models.DecimalField(
+        max_digits=30,
+        decimal_places=25,
         blank=True,
         null=True,
-        verbose_name="Ratio investissement par puissance €/kW",
+        verbose_name="Longitude",
     )
-    grants_earned_amount = models.CharField(
+    production_tracking_url = models.CharField(
         max_length=50,
         blank=True,
         null=True,
-        verbose_name="Montant des subventions reçues pour le Site de production (en €)",
+        verbose_name="URL monitoring du site de production",
     )
-    production_tracking_url = models.CharField(
+    wp_project_url = models.CharField(
         max_length=50,
         blank=True,
         null=True,
-        verbose_name="URL monitoring du site de production",
+        verbose_name="Lien du projet sur le site principal",
     )
 
     class Meta(Model.Meta):
         ordering = ["pk"]
-        permission_classes = [AuthenticatedOnly, ReadOnly]
-        rdf_type = "energiepartagee:production_site"
-        nested_fields = ["partner_links"]
-        verbose_name = _("Site de production")
-        verbose_name_plural = _("Sites de productions")
+        permission_classes = [InheritPermissions | EPRegionalAdminPermission]
+        inherit_permissions = ["founder"]
+        rdf_type = "energiepartagee:citizen_project"
+        nested_fields = [
+            "communication_profile",
+            "partnered_by",
+            "earned_distinctions",
+            "testimonies",
+            "production_sites",
+        ]
+        verbose_name = _("Projet Citoyen")
+        verbose_name_plural = _("Projets Citoyens")
+        depth = 2
 
     def __str__(self):
         if self.name:
             return self.name
         else:
             return self.urlid
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/college.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/college.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/capital_distribution.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/capital_distribution.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-
 from djangoldp.models import Model
-from djangoldp.permissions import AuthenticatedOnly, ReadOnly
+from djangoldp.permissions import InheritPermissions
 
 from djangoldp_energiepartagee.models.actor import Actor
 from djangoldp_energiepartagee.models.shareholder import Shareholder
 
 
 class CapitalDistribution(Model):
     actor = models.ForeignKey(
@@ -57,15 +56,16 @@
     )
     other_private_orgs_other_funds = models.DecimalField(
         max_digits=30, decimal_places=2, blank=True, null=True
     )
 
     class Meta(Model.Meta):
         ordering = ["pk"]
-        permission_classes = [AuthenticatedOnly, ReadOnly]
+        permission_classes = [InheritPermissions]
+        inherit_permissions = ["actor"]
         rdf_type = "energiepartagee:capital_distribution"
         serializer_fields = [
             "shareholder",
             "individuals_count",
             "individuals_capital",
             "other_funds_capital",
             "other_funds_residents",
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/__init__.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/__init__.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/region.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/region.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,29 @@
+from django.contrib.auth import get_user_model
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-
 from djangoldp.models import Model
-from djangoldp.permissions import ReadOnly, AnonymousReadOnly
+from djangoldp.permissions import ReadOnly
+
+from djangoldp_energiepartagee.permissions import EPRegionalAdminPermission
 
 
 class Region(Model):
     name = models.CharField(max_length=30, blank=True, null=True, verbose_name="Région")
     isocode = models.CharField(
         max_length=6, blank=True, null=True, verbose_name="code ISO"
     )
     acronym = models.CharField(
         max_length=6, blank=True, null=True, verbose_name="Acronyme"
     )
+    admins = models.ManyToManyField(get_user_model(), related_name="admin_regions")
 
     class Meta(Model.Meta):
         ordering = ["pk"]
-        permission_classes = [
-            AnonymousReadOnly & ReadOnly
-        ]  # |AuthenticatedOnly,ReadOnly
+        permission_classes = [ReadOnly | EPRegionalAdminPermission]
         rdf_type = "energiepartagee:region"
         serializer_fields = ["name", "isocode", "acronym"]
         verbose_name = _("Région")
         verbose_name_plural = _("Régions")
 
     def __str__(self):
         if self.name:
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/energy_buyer_type.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/energy_buyer_type.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/college_epa.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/college_epa.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/regional_network.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/regional_network.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/energy_production.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/energy_production.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-
 from djangoldp.models import Model
-from djangoldp.permissions import AuthenticatedOnly, ReadOnly
+from djangoldp.permissions import InheritPermissions
 
-from djangoldp_energiepartagee.models.production_site import ProductionSite
 from djangoldp_energiepartagee.models.energy_buyer import EnergyBuyer
 from djangoldp_energiepartagee.models.energy_type import EnergyType
+from djangoldp_energiepartagee.models.production_site import ProductionSite
 
 
 class EnergyProduction(Model):
     production_site = models.ForeignKey(
         ProductionSite,
         blank=True,
         null=True,
@@ -31,27 +30,30 @@
         blank=True,
         null=True,
         on_delete=models.CASCADE,
         verbose_name="Type d'énergie",
         related_name="energy_production",
     )
     energy_contract = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Contrat Energie"
+        max_length=50, blank=True, null=True, verbose_name="Contrat associé"
     )
     reference_unit = models.CharField(
         max_length=50, blank=True, null=True, verbose_name="Unité de référence"
     )
     estimated_capacity = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Capacité estimée"
+        max_length=50, blank=True, null=True, verbose_name="Puissance estimée"
     )
     installed_capacity = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Capacité installée"
+        max_length=50, blank=True, null=True, verbose_name="Puissance installée"
     )
     consumption_equivalence = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Equivalence en consommation"
+        max_length=50,
+        blank=True,
+        null=True,
+        verbose_name="Equivalence en nombre de foyers",
     )
     yearly_production = models.CharField(
         max_length=50, blank=True, null=True, verbose_name="Production annuelle"
     )
     estimated_yearly_production = models.CharField(
         max_length=50, blank=True, null=True, verbose_name="Production annuelle estimée"
     )
@@ -63,15 +65,16 @@
         blank=True,
         null=True,
         verbose_name="Capacité d'injection estimée",
     )
 
     class Meta(Model.Meta):
         ordering = ["pk"]
-        permission_classes = [AuthenticatedOnly, ReadOnly]
+        permission_classes = [InheritPermissions]
+        inherit_permissions = ["production_site"]
         rdf_type = "energiepartagee:energy_production"
         verbose_name = _("Énergie produite")
         verbose_name_plural = _("Énergies produites")
 
     def __str__(self):
         if self.production_site.name:
             return self.production_site.name
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/citizen_project.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/production_site.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,145 +1,152 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-
 from djangoldp.models import Model
-from djangoldp.permissions import AuthenticatedOnly, ReadOnly
+from djangoldp.permissions import InheritPermissions
 
-from djangoldp_energiepartagee.models.actor import Actor
+from djangoldp_energiepartagee.models.citizen_project import CitizenProject
 from djangoldp_energiepartagee.models.region import Region
+from djangoldp_energiepartagee.permissions import EPRegionalAdminPermission
 
 
-CITIZEN_PROJECT_STATUS_CHOICES = [
-    ("draft", "Brouillon"),
-    ("validation", "En cours de validation"),
-    ("published", "Publié"),
-    ("retired", "Dépublié"),
-]
-
-
-class CitizenProject(Model):
-    founder = models.ForeignKey(
-        Actor,
+class ProductionSite(Model):
+    citizen_project = models.ForeignKey(
+        CitizenProject,
         blank=True,
         null=True,
         on_delete=models.CASCADE,
-        verbose_name="Fondateur",
-        related_name="founded_projects",
+        verbose_name="Projet citoyen",
+        related_name="production_sites",
     )
     name = models.CharField(max_length=50, blank=True, null=True, verbose_name="Name")
-    short_description = models.TextField(
-        blank=True, null=True, verbose_name="Courte description"
-    )
-    city = models.CharField(max_length=50, blank=True, null=True, verbose_name="Ville")
-    postcode = models.CharField(
-        max_length=20, blank=True, null=True, verbose_name="Code Postal"
+    description = models.TextField(blank=True, null=True, verbose_name="Description")
+    # FIXME: Should be a property of produced energies
+    reference_unit = models.TextField(
+        blank=True, null=True, verbose_name="Unité de référence"
+    )
+    # FIXME: Should be a choice I think
+    progress_status = models.CharField(
+        max_length=248, blank=True, null=True, verbose_name="Progress status"
     )
-    address = models.CharField(
-        max_length=250, blank=True, null=True, verbose_name="Adresse"
-    )
-    # region = models.CharField(max_length=50, blank=True, null=True, verbose_name="Région")
-    region = models.ForeignKey(
-        Region,
+    total_development_budget = models.CharField(
         max_length=50,
         blank=True,
         null=True,
-        on_delete=models.SET_NULL,
-        verbose_name="Région",
-        related_name="projects",
-    )
-    department = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Département"
+        verbose_name="Budget total de développement",
     )
-    action_territory = models.CharField(
+    total_investment_budget = models.CharField(
         max_length=50,
         blank=True,
         null=True,
-        verbose_name="Territoire d'action du projet",
-    )
-    picture = models.CharField(
-        max_length=250, blank=True, null=True, verbose_name="Photo"
-    )
-    video = models.CharField(
-        max_length=250, blank=True, null=True, verbose_name="Vidéo"
-    )
-    website = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Site"
-    )
-    facebook_link = models.CharField(
-        max_length=250, blank=True, null=True, verbose_name="Facebook"
+        verbose_name="Budget total d'investissement",
     )
-    linkedin_link = models.CharField(
-        max_length=250, blank=True, null=True, verbose_name="LinkedIn"
+    yearly_turnover = models.CharField(
+        max_length=50, blank=True, null=True, verbose_name="Chiffre d'affaire annuel"
     )
-    twitter_link = models.CharField(
-        max_length=250, blank=True, null=True, verbose_name="Twitter"
-    )
-    instagram_link = models.CharField(
-        max_length=250, blank=True, null=True, verbose_name="Instragram"
-    )
-    contact_picture = models.CharField(
-        max_length=250, blank=True, null=True, verbose_name="Contact: Photo"
-    )
-    contact_name = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Contact: Nom"
-    )
-    contact_first_name = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Contact: Prénom"
-    )
-    contact_email = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Contact: Email"
+    address = models.CharField(
+        max_length=250, blank=True, null=True, verbose_name="Adresse"
     )
-    contact_phone = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Contact: Téléphone"
+    postcode = models.CharField(
+        max_length=20, blank=True, null=True, verbose_name="Code Postal"
     )
-    contact_visibility = models.BooleanField(
-        blank=True, null=True, verbose_name="Visibilité du contact", default=False
+    city = models.CharField(max_length=50, blank=True, null=True, verbose_name="Ville")
+    department = models.CharField(
+        max_length=50, blank=True, null=True, verbose_name="Département"
     )
-    status = models.CharField(
-        choices=CITIZEN_PROJECT_STATUS_CHOICES,
+    region = models.ForeignKey(
+        Region,
         max_length=50,
         blank=True,
         null=True,
-        verbose_name="Etat d'avancement du projet",
+        on_delete=models.SET_NULL,
+        verbose_name="Région",
+        related_name="production_sites",
     )
     lat = models.DecimalField(
         max_digits=30,
         decimal_places=25,
         blank=True,
         null=True,
-        verbose_name="Latitude",
+        verbose_name="Lattitude",
     )
     lng = models.DecimalField(
         max_digits=30,
         decimal_places=25,
         blank=True,
         null=True,
         verbose_name="Longitude",
     )
+    expected_commissionning_year = models.CharField(
+        max_length=50,
+        blank=True,
+        null=True,
+        verbose_name="Année de mise en service prévue",
+    )
+    effective_commissionning_year = models.CharField(
+        max_length=50,
+        blank=True,
+        null=True,
+        verbose_name="Année de mise en service effective",
+    )
+    picture = models.CharField(
+        max_length=250, blank=True, null=True, verbose_name="Photo"
+    )
+    investment_capacity_ratio = models.CharField(
+        max_length=50,
+        blank=True,
+        null=True,
+        verbose_name="Ratio investissement par puissance €/kW",
+    )
+    grants_earned_amount = models.CharField(
+        max_length=50,
+        blank=True,
+        null=True,
+        verbose_name="Montant des subventions reçues pour le Site de production (en €)",
+    )
     production_tracking_url = models.CharField(
         max_length=50,
         blank=True,
         null=True,
         verbose_name="URL monitoring du site de production",
     )
-    wp_project_url = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Lien du projet sur le site principal"
-    )
 
     class Meta(Model.Meta):
         ordering = ["pk"]
-        permission_classes = [AuthenticatedOnly, ReadOnly]
-        rdf_type = "energiepartagee:citizen_project"
+        permission_classes = [InheritPermissions | EPRegionalAdminPermission]
+        inherit_permissions = ["citizen_project"]
+        rdf_type = "energiepartagee:production_site"
         nested_fields = [
-            "communication_profile",
-            "partnered_by",
-            "earned_distinctions",
-            "testimonies",
+            "partner_links",
+            "energy_productions",
+        ]
+        serializer_fields = [
+            "name",
+            "description",
+            "reference_unit",
+            "progress_status",
+            "total_development_budget",
+            "total_investment_budget",
+            "yearly_turnover",
+            "address",
+            "city",
+            "department",
+            "region",
+            "lat",
+            "lng",
+            "expected_commissionning_year",
+            "effective_commissionning_year",
+            "picture",
+            "investment_capacity_ratio",
+            "grants_earned_amount",
+            "production_tracking_url",
+            "partner_links",
+            "energy_productions",
         ]
-        verbose_name = _("Projet Citoyen")
-        verbose_name_plural = _("Projets Citoyens")
+        verbose_name = _("Site de production")
+        verbose_name_plural = _("Sites de productions")
+        depth = 2
 
     def __str__(self):
         if self.name:
             return self.name
         else:
             return self.urlid
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/testimony.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/profile.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,54 @@
+from django.conf import settings
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from djangoldp.models import Model
-from djangoldp.permissions import AuthenticatedOnly, ReadOnly
+from djangoldp.permissions import OwnerPermissions
 
-from djangoldp_energiepartagee.models.citizen_project import CitizenProject
 
-
-class Testimony(Model):
-    citizen_project = models.ForeignKey(
-        CitizenProject,
+class Profile(Model):
+    user = models.OneToOneField(
+        settings.AUTH_USER_MODEL, on_delete=models.CASCADE, blank=True, null=True
+    )
+    phone = models.CharField(
+        max_length=20, blank=True, null=True, verbose_name="Numéro de téléphone"
+    )
+    presentation = models.TextField(
+        blank=True, null=True, verbose_name="Présentation de l'utilisateur"
+    )
+    picture = models.CharField(
         blank=True,
         null=True,
-        on_delete=models.CASCADE,
-        verbose_name="Projet",
-        related_name="testimonies",
-    )
-    author_name = models.CharField(
-        max_length=250, blank=True, null=True, verbose_name="Auteur"
+        max_length=250,
+        default="/img/default_avatar_user.svg",
+        verbose_name="Photo de l'utilisateur",
     )
-    author_picture = models.CharField(
-        max_length=250, blank=True, null=True, verbose_name="Auteur: Photo"
+    address = models.CharField(
+        max_length=250, blank=True, null=True, verbose_name="Adresse"
     )
-    content = models.CharField(
-        max_length=250, blank=True, null=True, verbose_name="Contenu"
+    postcode = models.CharField(
+        max_length=5, blank=True, null=True, verbose_name="Code Postal"
     )
+    city = models.CharField(max_length=30, blank=True, null=True, verbose_name="Ville")
 
     class Meta(Model.Meta):
         ordering = ["pk"]
-        permission_classes = [AuthenticatedOnly, ReadOnly]
-        rdf_type = "energiepartagee:testimony"
-        verbose_name = _("Témoignage")
-        verbose_name_plural = _("Témoignages")
+        owner_field = "user"
+        permission_classes = [OwnerPermissions]
+        rdf_type = "energiepartagee:profile"
+        serializer_fields = [
+            "phone",
+            "presentation",
+            "picture",
+            "address",
+            "postcode",
+            "city",
+        ]
+        verbose_name = _("Profil")
+        verbose_name_plural = _("Profils")
 
     def __str__(self):
-        return self.urlid
+        if self.user:
+            return str(self.user)
+        else:
+            return self.urlid
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/intervention_zone.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/intervention_zone.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/citizen_project_distinction.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/citizen_project_distinction.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/energy_buyer.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/partner_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from djangoldp.models import Model
 from djangoldp.permissions import AuthenticatedOnly, ReadOnly
 
-from djangoldp_energiepartagee.models.energy_buyer_type import ContractType
+from djangoldp_energiepartagee.models.partner import Partner
 
 
-class EnergyBuyer(Model):
-    name = models.CharField(max_length=250, blank=True, null=True, verbose_name="Nom")
-    contract_type = models.ForeignKey(
-        ContractType,
+class PartnerType(Model):
+    name = models.CharField(max_length=50, blank=True, null=True, verbose_name="Type")
+    partners = models.ManyToManyField(
+        Partner,
         blank=True,
-        null=True,
-        on_delete=models.CASCADE,
-        verbose_name="Type de contrat",
-        related_name="contract",
+        verbose_name="Partenaires",
+        related_name="types",
     )
 
     class Meta(Model.Meta):
-        ordering = ["pk"]
+        ordering = ["name"]
         permission_classes = [AuthenticatedOnly, ReadOnly]
-        rdf_type = "energiepartagee:energy_buyer"
-        verbose_name = _("Acheteur d'énergie")
-        verbose_name_plural = _("Acheteurs d'énergies")
+        rdf_type = "energiepartagee:partner_type"
+        serializer_fields = ["@id", "name"]
+        verbose_name = _("Type de partenaire")
+        verbose_name_plural = _("Types de partenaire")
 
     def __str__(self):
         if self.name:
             return self.name
         else:
             return self.urlid
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/shareholder.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/shareholder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-
 from djangoldp.models import Model
-from djangoldp.permissions import AuthenticatedOnly, ReadOnly
+from djangoldp.permissions import InheritPermissions
 
 
 class Shareholder(Model):
     structure_name = models.TextField(
         blank=True, null=True, verbose_name="Nom de la Structure"
     )
     capital_amount = models.TextField(
@@ -26,15 +25,15 @@
         null=True,
         verbose_name="Est un investissement relais?",
         default=False,
     )
 
     class Meta(Model.Meta):
         ordering = ["pk"]
-        permission_classes = [AuthenticatedOnly, ReadOnly]
+        permission_classes = [InheritPermissions]
         rdf_type = "energiepartagee:shareholder"
         serializer_fields = [
             "structure_name",
             "capital_amount",
             "capital_percentage",
             "other_funds_amount",
             "other_funds_percentage",
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/legal_structure.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/legal_structure.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/partner_type.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/integration_step.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-
 from djangoldp.models import Model
-from djangoldp.permissions import AuthenticatedOnly, ReadOnly
 
-from djangoldp_energiepartagee.models.partner import Partner
+from djangoldp_energiepartagee.permissions import EPRegionalAdminPermission
 
 
-class PartnerType(Model):
-    name = models.CharField(max_length=50, blank=True, null=True, verbose_name="Type")
-    partners = models.ManyToManyField(
-        Partner,
+class Integrationstep(Model):
+    packagestep = models.BooleanField(
+        blank=True, null=True, verbose_name="Colis accueil à envoyer", default=False
+    )
+    adhspacestep = models.BooleanField(
+        blank=True, null=True, verbose_name="Non inscrit sur espace Adh", default=False
+    )
+    adhliststep = models.BooleanField(
+        blank=True, null=True, verbose_name="Non inscrit sur liste Adh", default=False
+    )
+    regionalliststep = models.BooleanField(
         blank=True,
-        verbose_name="Partenaires",
-        related_name="types",
+        null=True,
+        verbose_name="Non inscrit sur liste régional",
+        default=False,
+    )
+    admincomment = models.TextField(
+        blank=True, null=True, verbose_name="Commentaires de l'administrateur"
     )
 
     class Meta(Model.Meta):
-        ordering = ["name"]
-        permission_classes = [AuthenticatedOnly, ReadOnly]
-        rdf_type = "energiepartagee:partner_type"
-        serializer_fields = ["@id", "name"]
-        verbose_name = _("Type de partenaire")
-        verbose_name_plural = _("Types de partenaire")
+        ordering = ["pk"]
+        rdf_type = "energiepartagee:integrationstep"
+        permission_classes = [EPRegionalAdminPermission]
+        serializer_fields = [
+            "packagestep",
+            "adhspacestep",
+            "adhliststep",
+            "regionalliststep",
+            "admincomment",
+        ]
+        verbose_name = _("Étapes d'intégration")
+        verbose_name_plural = _("Étapes d'intégration")
 
     def __str__(self):
-        if self.name:
-            return self.name
-        else:
-            return self.urlid
+        return str(self.id)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/partner_link.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/partner_link.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/partner.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/partner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-
 from djangoldp.models import Model
-from djangoldp.permissions import AuthenticatedOnly, ReadOnly
+from djangoldp.permissions import InheritPermissions
 
 from djangoldp_energiepartagee.models.actor import Actor
 from djangoldp_energiepartagee.models.citizen_project import CitizenProject
 
 
 class Partner(Model):
     actor = models.ForeignKey(
@@ -24,15 +23,16 @@
         on_delete=models.CASCADE,
         verbose_name="Projet Citoyen",
         related_name="partnered_by",
     )
 
     class Meta(Model.Meta):
         ordering = ["pk"]
-        permission_classes = [AuthenticatedOnly, ReadOnly]
+        permission_classes = [InheritPermissions]
+        inherit_permissions = ["actor", "citizen_project"]
         rdf_type = "energiepartagee:partner"
         nested_fields = ["types"]
         verbose_name = _("Partenaire")
         verbose_name_plural = _("Partenaires")
 
     def __str__(self):
         return self.urlid
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/energy_type.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/energy_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-
 from djangoldp.models import Model
-from djangoldp.permissions import AuthenticatedOnly, ReadOnly
+from djangoldp.permissions import InheritPermissions
 
 
 class EnergyType(Model):
     name = models.CharField(max_length=250, blank=True, null=True, verbose_name="Nom")
     installed_capacity_reference_unit = models.CharField(
         max_length=250, blank=True, null=True
     )
     yearly_proudction_ref_unit = models.CharField(max_length=250, blank=True, null=True)
     capacity_factor_ref_unit = models.CharField(max_length=250, blank=True, null=True)
 
     class Meta(Model.Meta):
         ordering = ["pk"]
-        permission_classes = [AuthenticatedOnly, ReadOnly]
+        permission_classes = [InheritPermissions]
+        inherit_permissions = ["energy_production"]
         rdf_type = "energiepartagee:energy_type"
         verbose_name = _("Type d'énergie")
         verbose_name_plural = _("Types d'énergies")
 
     def __str__(self):
         if self.name:
             return self.name
```

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/payment_method.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/discount.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/discount.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-1.2.9/djangoldp_energiepartagee/models/signals.py` & `djangoldp_energiepartagee-2.0.0/djangoldp_energiepartagee/models/signals.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.conf import settings
 from django.core.mail import send_mail
-from django.db.models.signals import pre_save, post_save
+from django.db.models.signals import post_save, pre_save
 from django.dispatch import receiver
 from django.template import loader
 from django.utils.translation import gettext_lazy as _
 
 from djangoldp_energiepartagee.models import *
 
 
@@ -18,15 +18,15 @@
 
 
 if not getattr(settings, "IS_AMORCE", False):
 
     @receiver(post_save, sender=Actor)
     def create_actor_contributions(sender, instance, created, **kwargs):
         if created:
-            if not instance.contributions or instance.contributions.exists() == False:
+            if not instance.contributions or not instance.contributions.exists():
                 amount = instance.get_next_contribution_amount()
 
                 contributionInstance = instance.contributions.create(
                     year=Contribution.get_current_contribution_year(),
                     numberpeople=instance.numberpeople,
                     numberemployees=instance.numberemployees,
                     turnover=instance.turnover,
@@ -54,46 +54,38 @@
         except sender.DoesNotExist:
             pass
         else:
             current_year_contribution = Contribution.objects.filter(
                 actor=instance, year=Contribution.get_current_contribution_year()
             ).first()
             if current_year_contribution:
-                # Detect change on Villageoise field
-                if old_instance.villageoise != instance.villageoise:
-                    if (
-                        current_year_contribution.contributionstatus
-                        != CONTRIBUTION_CHOICES[3][0]
-                        and current_year_contribution.contributionstatus
-                        != CONTRIBUTION_CHOICES[4][0]
-                    ):
-                        current_year_contribution.amount = (
-                            instance.get_next_contribution_amount()
-                        )
-                        # Check if the discount Villageoise is applied and apply it on
-                        villageoise = Discount.objects.filter(name="villageoise").all()[
-                            0
-                        ]
-                        if instance.villageoise == True:
-                            current_year_contribution.discount.add(villageoise)
-                        else:
-                            current_year_contribution.discount.remove(villageoise)
-                        current_year_contribution.save()
-                # Else, just update the contribution amount
-                elif (
+                if (
                     current_year_contribution.contributionstatus
                     == CONTRIBUTION_CHOICES[0][0]
                     or current_year_contribution.contributionstatus
                     == CONTRIBUTION_CHOICES[1][0]
                     or current_year_contribution.contributionstatus
                     == CONTRIBUTION_CHOICES[2][0]
                 ):
                     current_year_contribution.amount = (
                         instance.get_next_contribution_amount()
                     )
+                    current_year_contribution.numberpeople = instance.numberpeople
+                    current_year_contribution.numberemployees = instance.numberemployees
+                    current_year_contribution.turnover = instance.turnover
+                    # Detect change on Villageoise field
+                    if old_instance.villageoise != instance.villageoise:
+                        # Check if the discount Villageoise is applied and apply it on
+                        villageoise = Discount.objects.filter(name="villageoise").all()[
+                            0
+                        ]
+                        if instance.villageoise:
+                            current_year_contribution.discount.add(villageoise)
+                        else:
+                            current_year_contribution.discount.remove(villageoise)
                     current_year_contribution.save()
 
     @receiver(pre_save, sender=Contribution)
     def update_status_after_payment_change(sender, instance, **kwargs):
         try:
             old_instance = sender.objects.get(pk=instance.pk)
         except sender.DoesNotExist:
```

