# Comparing `tmp/stytch-9.0.0.tar.gz` & `tmp/stytch-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stytch-9.0.0.tar", last modified: Tue Apr  9 16:18:32 2024, max compression
+gzip compressed data, was "stytch-9.1.0.tar", last modified: Thu Apr 11 14:35:33 2024, max compression
```

## Comparing `stytch-9.0.0.tar` & `stytch-9.1.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:32.161071 stytch-9.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-09 16:18:11.000000 stytch-9.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-09 16:18:32.161071 stytch-9.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-09 16:18:11.000000 stytch-9.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 16:18:32.161071 stytch-9.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-09 16:18:11.000000 stytch-9.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:32.141071 stytch-9.0.0/stytch/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:32.141071 stytch-9.0.0/stytch/b2b/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:32.149071 stytch-9.0.0/stytch/b2b/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    31578 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    52376 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    54059 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/organizations_members_oauth_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)    26141 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    28071 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)    22956 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/scim.py
--rw-r--r--   0 runner    (1001) docker     (127)    16205 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/scim_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    38402 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:32.153071 stytch-9.0.0/stytch/b2b/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/organizations_members_oauth_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/scim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/scim_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/b2b/models/totps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:32.153071 stytch-9.0.0/stytch/consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:32.157071 stytch-9.0.0/stytch/consumer/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)    18335 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/m2m_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/m2m_clients_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    33050 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)    16939 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    17491 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)    30883 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)    32914 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    26192 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/api/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:32.161071 stytch-9.0.0/stytch/consumer/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/m2m_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/m2m_clients_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)    15941 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/consumer/models/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:32.161071 stytch-9.0.0/stytch/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/core/api_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/core/client_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:32.161071 stytch-9.0.0/stytch/core/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/core/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/core/http/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/core/response_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:32.161071 stytch-9.0.0/stytch/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/shared/jwt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/shared/lazy_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/shared/method_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/shared/policy_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/shared/rbac_local.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 16:18:11.000000 stytch-9.0.0/stytch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:32.161071 stytch-9.0.0/stytch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-09 16:18:32.000000 stytch-9.0.0/stytch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-09 16:18:32.000000 stytch-9.0.0/stytch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:18:32.000000 stytch-9.0.0/stytch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 16:18:32.000000 stytch-9.0.0/stytch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 16:18:32.000000 stytch-9.0.0/stytch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:18:32.161071 stytch-9.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-04-09 16:18:11.000000 stytch-9.0.0/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-04-09 16:18:11.000000 stytch-9.0.0/test/test_integration_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-11 14:35:20.000000 stytch-9.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-11 14:35:33.359014 stytch-9.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-11 14:35:20.000000 stytch-9.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-11 14:35:33.359014 stytch-9.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-11 14:35:20.000000 stytch-9.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.339014 stytch-9.1.0/stytch/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.343014 stytch-9.1.0/stytch/b2b/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.347014 stytch-9.1.0/stytch/b2b/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31578 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52376 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54059 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/organizations_members_oauth_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26141 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28071 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22956 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/scim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/scim_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44453 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.351014 stytch-9.1.0/stytch/b2b/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19720 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/organizations_members_oauth_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/scim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/scim_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/totps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.351014 stytch-9.1.0/stytch/consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.355014 stytch-9.1.0/stytch/consumer/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18335 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/m2m_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/m2m_clients_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33050 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16939 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17491 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30883 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32914 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26192 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/stytch/consumer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/m2m_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/m2m_clients_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15941 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/stytch/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/core/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/core/client_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/stytch/core/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/core/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/core/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/core/response_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/stytch/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/shared/jwt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/shared/lazy_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/shared/method_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/shared/policy_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/shared/rbac_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/stytch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-11 14:35:33.000000 stytch-9.1.0/stytch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-11 14:35:33.000000 stytch-9.1.0/stytch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:35:33.000000 stytch-9.1.0/stytch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 14:35:33.000000 stytch-9.1.0/stytch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 14:35:33.000000 stytch-9.1.0/stytch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-04-11 14:35:20.000000 stytch-9.1.0/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-04-11 14:35:20.000000 stytch-9.1.0/test/test_integration_async.py
```

### Comparing `stytch-9.0.0/LICENSE.txt` & `stytch-9.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/PKG-INFO` & `stytch-9.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 9.0.0
+Version: 9.1.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-9.0.0/README.md` & `stytch-9.1.0/README.md`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/setup.py` & `stytch-9.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/discovery.py` & `stytch-9.1.0/stytch/b2b/api/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/discovery_intermediate_sessions.py` & `stytch-9.1.0/stytch/b2b/api/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/discovery_organizations.py` & `stytch-9.1.0/stytch/b2b/api/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/magic_links.py` & `stytch-9.1.0/stytch/b2b/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/magic_links_discovery.py` & `stytch-9.1.0/stytch/b2b/api/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/magic_links_email.py` & `stytch-9.1.0/stytch/b2b/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/magic_links_email_discovery.py` & `stytch-9.1.0/stytch/b2b/api/magic_links_email_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/oauth.py` & `stytch-9.1.0/stytch/b2b/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/oauth_discovery.py` & `stytch-9.1.0/stytch/b2b/api/oauth_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/organizations.py` & `stytch-9.1.0/stytch/b2b/api/organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/organizations_members.py` & `stytch-9.1.0/stytch/b2b/api/organizations_members.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/organizations_members_oauth_providers.py` & `stytch-9.1.0/stytch/b2b/api/organizations_members_oauth_providers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/otp.py` & `stytch-9.1.0/stytch/b2b/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/otp_sms.py` & `stytch-9.1.0/stytch/b2b/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/passwords.py` & `stytch-9.1.0/stytch/b2b/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/passwords_email.py` & `stytch-9.1.0/stytch/b2b/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/passwords_existing_password.py` & `stytch-9.1.0/stytch/b2b/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/passwords_session.py` & `stytch-9.1.0/stytch/b2b/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/rbac.py` & `stytch-9.1.0/stytch/b2b/api/rbac.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/recovery_codes.py` & `stytch-9.1.0/stytch/b2b/api/recovery_codes.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/scim.py` & `stytch-9.1.0/stytch/b2b/api/scim.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/scim_connections.py` & `stytch-9.1.0/stytch/b2b/api/scim_connections.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,21 +7,28 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Union
 
 from stytch.b2b.models.scim import SCIMGroupImplicitRoleAssignments
 from stytch.b2b.models.scim_connections import (
     CreateRequestIdp,
+    CreateRequestOptions,
     CreateResponse,
+    DeleteRequestOptions,
     DeleteResponse,
+    GetRequestOptions,
     GetResponse,
+    RotateCancelRequestOptions,
     RotateCancelResponse,
+    RotateCompleteRequestOptions,
     RotateCompleteResponse,
+    RotateStartRequestOptions,
     RotateStartResponse,
     UpdateRequestIdp,
+    UpdateRequestOptions,
     UpdateResponse,
 )
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
 class Connections:
@@ -37,25 +44,28 @@
         organization_id: str,
         connection_id: str,
         display_name: Optional[str] = None,
         identity_provider: Optional[Union[UpdateRequestIdp, str]] = None,
         scim_group_implicit_role_assignments: Optional[
             List[SCIMGroupImplicitRoleAssignments]
         ] = None,
+        method_options: Optional[UpdateRequestOptions] = None,
     ) -> UpdateResponse:
         """Update a SCIM Connection. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - connection_id: The ID of the SCIM connection.
           - display_name: A human-readable display name for the connection.
           - identity_provider: (no documentation yet)
           - scim_group_implicit_role_assignments: (no documentation yet)
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
         }
         if display_name is not None:
             data["display_name"] = display_name
         if identity_provider is not None:
@@ -76,25 +86,28 @@
         organization_id: str,
         connection_id: str,
         display_name: Optional[str] = None,
         identity_provider: Optional[UpdateRequestIdp] = None,
         scim_group_implicit_role_assignments: Optional[
             List[SCIMGroupImplicitRoleAssignments]
         ] = None,
+        method_options: Optional[UpdateRequestOptions] = None,
     ) -> UpdateResponse:
         """Update a SCIM Connection. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - connection_id: The ID of the SCIM connection.
           - display_name: A human-readable display name for the connection.
           - identity_provider: (no documentation yet)
           - scim_group_implicit_role_assignments: (no documentation yet)
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
         }
         if display_name is not None:
             data["display_name"] = display_name
         if identity_provider is not None:
@@ -110,22 +123,25 @@
         res = await self.async_client.put(url, data, headers)
         return UpdateResponse.from_json(res.response.status, res.json)
 
     def delete(
         self,
         organization_id: str,
         connection_id: str,
+        method_options: Optional[DeleteRequestOptions] = None,
     ) -> DeleteResponse:
         """Deletes a SCIM Connection. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
-          - connection_id: Globally unique UUID that identifies a specific SSO `connection_id` for a Member.
+          - connection_id: The ID of the SCIM connection.
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
         }
 
         url = self.api_base.url_for(
             "/v1/b2b/scim/{organization_id}/connections/{connection_id}", data
@@ -133,22 +149,25 @@
         res = self.sync_client.delete(url, headers)
         return DeleteResponse.from_json(res.response.status_code, res.json)
 
     async def delete_async(
         self,
         organization_id: str,
         connection_id: str,
+        method_options: Optional[DeleteRequestOptions] = None,
     ) -> DeleteResponse:
         """Deletes a SCIM Connection. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
-          - connection_id: Globally unique UUID that identifies a specific SSO `connection_id` for a Member.
+          - connection_id: The ID of the SCIM connection.
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
         }
 
         url = self.api_base.url_for(
             "/v1/b2b/scim/{organization_id}/connections/{connection_id}", data
@@ -156,22 +175,25 @@
         res = await self.async_client.delete(url, headers)
         return DeleteResponse.from_json(res.response.status, res.json)
 
     def rotate_start(
         self,
         organization_id: str,
         connection_id: str,
+        method_options: Optional[RotateStartRequestOptions] = None,
     ) -> RotateStartResponse:
         """Start a SCIM token rotation. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - connection_id: The ID of the SCIM connection.
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
         }
 
         url = self.api_base.url_for(
             "/v1/b2b/scim/{organization_id}/connections/{connection_id}/rotate/start",
@@ -180,22 +202,25 @@
         res = self.sync_client.post(url, data, headers)
         return RotateStartResponse.from_json(res.response.status_code, res.json)
 
     async def rotate_start_async(
         self,
         organization_id: str,
         connection_id: str,
+        method_options: Optional[RotateStartRequestOptions] = None,
     ) -> RotateStartResponse:
         """Start a SCIM token rotation. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - connection_id: The ID of the SCIM connection.
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
         }
 
         url = self.api_base.url_for(
             "/v1/b2b/scim/{organization_id}/connections/{connection_id}/rotate/start",
@@ -204,22 +229,25 @@
         res = await self.async_client.post(url, data, headers)
         return RotateStartResponse.from_json(res.response.status, res.json)
 
     def rotate_complete(
         self,
         organization_id: str,
         connection_id: str,
+        method_options: Optional[RotateCompleteRequestOptions] = None,
     ) -> RotateCompleteResponse:
         """Completes a SCIM token rotation. This will complete the current token rotation process and update the active token to be the new token supplied in the [start SCIM token rotation](https://stytch.com/docs/b2b/api/scim-rotate-token-start) response. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - connection_id: The ID of the SCIM connection.
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
         }
 
         url = self.api_base.url_for(
             "/v1/b2b/scim/{organization_id}/connections/{connection_id}/rotate/complete",
@@ -228,22 +256,25 @@
         res = self.sync_client.post(url, data, headers)
         return RotateCompleteResponse.from_json(res.response.status_code, res.json)
 
     async def rotate_complete_async(
         self,
         organization_id: str,
         connection_id: str,
+        method_options: Optional[RotateCompleteRequestOptions] = None,
     ) -> RotateCompleteResponse:
         """Completes a SCIM token rotation. This will complete the current token rotation process and update the active token to be the new token supplied in the [start SCIM token rotation](https://stytch.com/docs/b2b/api/scim-rotate-token-start) response. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - connection_id: The ID of the SCIM connection.
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
         }
 
         url = self.api_base.url_for(
             "/v1/b2b/scim/{organization_id}/connections/{connection_id}/rotate/complete",
@@ -252,22 +283,25 @@
         res = await self.async_client.post(url, data, headers)
         return RotateCompleteResponse.from_json(res.response.status, res.json)
 
     def rotate_cancel(
         self,
         organization_id: str,
         connection_id: str,
+        method_options: Optional[RotateCancelRequestOptions] = None,
     ) -> RotateCancelResponse:
         """Cancel a SCIM token rotation. This will cancel the current token rotation process, keeping the original token active. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - connection_id: The ID of the SCIM connection.
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
         }
 
         url = self.api_base.url_for(
             "/v1/b2b/scim/{organization_id}/connections/{connection_id}/rotate/cancel",
@@ -276,22 +310,25 @@
         res = self.sync_client.post(url, data, headers)
         return RotateCancelResponse.from_json(res.response.status_code, res.json)
 
     async def rotate_cancel_async(
         self,
         organization_id: str,
         connection_id: str,
+        method_options: Optional[RotateCancelRequestOptions] = None,
     ) -> RotateCancelResponse:
         """Cancel a SCIM token rotation. This will cancel the current token rotation process, keeping the original token active. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - connection_id: The ID of the SCIM connection.
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
         }
 
         url = self.api_base.url_for(
             "/v1/b2b/scim/{organization_id}/connections/{connection_id}/rotate/cancel",
@@ -301,23 +338,26 @@
         return RotateCancelResponse.from_json(res.response.status, res.json)
 
     def create(
         self,
         organization_id: str,
         display_name: Optional[str] = None,
         identity_provider: Optional[Union[CreateRequestIdp, str]] = None,
+        method_options: Optional[CreateRequestOptions] = None,
     ) -> CreateResponse:
         """Create a new SCIM Connection. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - display_name: A human-readable display name for the connection.
           - identity_provider: (no documentation yet)
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
         if display_name is not None:
             data["display_name"] = display_name
         if identity_provider is not None:
             data["identity_provider"] = identity_provider
@@ -327,23 +367,26 @@
         return CreateResponse.from_json(res.response.status_code, res.json)
 
     async def create_async(
         self,
         organization_id: str,
         display_name: Optional[str] = None,
         identity_provider: Optional[CreateRequestIdp] = None,
+        method_options: Optional[CreateRequestOptions] = None,
     ) -> CreateResponse:
         """Create a new SCIM Connection. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - display_name: A human-readable display name for the connection.
           - identity_provider: (no documentation yet)
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
         if display_name is not None:
             data["display_name"] = display_name
         if identity_provider is not None:
             data["identity_provider"] = identity_provider
@@ -351,39 +394,45 @@
         url = self.api_base.url_for("/v1/b2b/scim/{organization_id}/connections", data)
         res = await self.async_client.post(url, data, headers)
         return CreateResponse.from_json(res.response.status, res.json)
 
     def get(
         self,
         organization_id: str,
+        method_options: Optional[GetRequestOptions] = None,
     ) -> GetResponse:
         """Get SCIM Connections. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
 
         url = self.api_base.url_for("/v1/b2b/scim/{organization_id}/connections", data)
         res = self.sync_client.get(url, data, headers)
         return GetResponse.from_json(res.response.status_code, res.json)
 
     async def get_async(
         self,
         organization_id: str,
+        method_options: Optional[GetRequestOptions] = None,
     ) -> GetResponse:
         """Get SCIM Connections. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
         """  # noqa
         headers: Dict[str, str] = {}
+        if method_options is not None:
+            headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
 
         url = self.api_base.url_for("/v1/b2b/scim/{organization_id}/connections", data)
         res = await self.async_client.get(url, data, headers)
         return GetResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-9.0.0/stytch/b2b/api/sessions.py` & `stytch-9.1.0/stytch/b2b/api/sessions.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     AuthorizationCheck,
     ExchangeRequestLocale,
     ExchangeResponse,
     GetJWKSResponse,
     GetResponse,
     LocalJWTResponse,
     MemberSession,
+    MigrateResponse,
     RevokeResponse,
 )
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 from stytch.shared import jwt_helpers, rbac_local
 from stytch.shared.policy_cache import PolicyCache
 
@@ -412,14 +413,96 @@
         if locale is not None:
             data["locale"] = locale
 
         url = self.api_base.url_for("/v1/b2b/sessions/exchange", data)
         res = await self.async_client.post(url, data, headers)
         return ExchangeResponse.from_json(res.response.status, res.json)
 
+    def migrate(
+        self,
+        session_token: str,
+        organization_id: str,
+        session_duration_minutes: Optional[int] = None,
+        session_custom_claims: Optional[Dict[str, Any]] = None,
+    ) -> MigrateResponse:
+        """Migrate a session from an external endpoint. Stytch will call the UserInfo endpoint specified in your project settings, performing a lookup using the session token passed in. If the endpoint repsonds and the response contains a valid email, Stytch will attempt to match that email with a member in your organization, and create a Stytch Session for you.
+
+        Fields:
+          - session_token: The authorization token Stytch will pass in to the external userinfo endpoint.
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
+
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
+
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
+
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
+        """  # noqa
+        headers: Dict[str, str] = {}
+        data: Dict[str, Any] = {
+            "session_token": session_token,
+            "organization_id": organization_id,
+        }
+        if session_duration_minutes is not None:
+            data["session_duration_minutes"] = session_duration_minutes
+        if session_custom_claims is not None:
+            data["session_custom_claims"] = session_custom_claims
+
+        url = self.api_base.url_for("/v1/b2b/sessions/migrate", data)
+        res = self.sync_client.post(url, data, headers)
+        return MigrateResponse.from_json(res.response.status_code, res.json)
+
+    async def migrate_async(
+        self,
+        session_token: str,
+        organization_id: str,
+        session_duration_minutes: Optional[int] = None,
+        session_custom_claims: Optional[Dict[str, Any]] = None,
+    ) -> MigrateResponse:
+        """Migrate a session from an external endpoint. Stytch will call the UserInfo endpoint specified in your project settings, performing a lookup using the session token passed in. If the endpoint repsonds and the response contains a valid email, Stytch will attempt to match that email with a member in your organization, and create a Stytch Session for you.
+
+        Fields:
+          - session_token: The authorization token Stytch will pass in to the external userinfo endpoint.
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
+
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
+
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
+
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
+        """  # noqa
+        headers: Dict[str, str] = {}
+        data: Dict[str, Any] = {
+            "session_token": session_token,
+            "organization_id": organization_id,
+        }
+        if session_duration_minutes is not None:
+            data["session_duration_minutes"] = session_duration_minutes
+        if session_custom_claims is not None:
+            data["session_custom_claims"] = session_custom_claims
+
+        url = self.api_base.url_for("/v1/b2b/sessions/migrate", data)
+        res = await self.async_client.post(url, data, headers)
+        return MigrateResponse.from_json(res.response.status, res.json)
+
     def get_jwks(
         self,
         project_id: str,
     ) -> GetJWKSResponse:
         """Get the JSON Web Key Set (JWKS) for a project.
 
         JWKS are rotated every ~6 months. Upon rotation, new JWTs will be signed using the new key set, and both key sets will be returned by this endpoint for a period of 1 month.
```

### Comparing `stytch-9.0.0/stytch/b2b/api/sso.py` & `stytch-9.1.0/stytch/b2b/api/sso.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/sso_oidc.py` & `stytch-9.1.0/stytch/b2b/api/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/sso_saml.py` & `stytch-9.1.0/stytch/b2b/api/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/api/totps.py` & `stytch-9.1.0/stytch/b2b/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/client.py` & `stytch-9.1.0/stytch/b2b/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/discovery.py` & `stytch-9.1.0/stytch/b2b/models/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/discovery_intermediate_sessions.py` & `stytch-9.1.0/stytch/b2b/models/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/discovery_organizations.py` & `stytch-9.1.0/stytch/b2b/models/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/magic_links.py` & `stytch-9.1.0/stytch/b2b/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/magic_links_discovery.py` & `stytch-9.1.0/stytch/b2b/models/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/magic_links_email.py` & `stytch-9.1.0/stytch/b2b/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/mfa.py` & `stytch-9.1.0/stytch/b2b/models/mfa.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/oauth.py` & `stytch-9.1.0/stytch/b2b/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/oauth_discovery.py` & `stytch-9.1.0/stytch/b2b/models/oauth_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/organizations.py` & `stytch-9.1.0/stytch/b2b/models/organizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,36 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
+import datetime
 import enum
 from typing import Any, Dict, List, Optional
 
 import pydantic
 
 from stytch.core.response_base import ResponseBase
 from stytch.shared.method_options import Authorization
 
 
 class SearchQueryOperator(str, enum.Enum):
     OR = "OR"
     AND = "AND"
 
 
+class ActiveSCIMConnection(pydantic.BaseModel):
+    connection_id: str
+    display_name: str
+    bearer_token_last_four: str
+    bearer_token_expires_at: Optional[datetime.datetime] = None
+
+
 class ActiveSSOConnection(pydantic.BaseModel):
     """
     Fields:
       - connection_id: Globally unique UUID that identifies a specific SSO `connection_id` for a Member.
       - display_name: A human-readable display name for the connection.
     """  # noqa
 
@@ -213,14 +221,15 @@
       `ALL_ALLOWED` – the default setting which allows all authentication methods to be used.
 
       `RESTRICTED` – only methods that comply with `allowed_mfa_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
       - allowed_mfa_methods: An array of allowed MFA authentication methods. This list is enforced when `mfa_methods` is set to `RESTRICTED`.
       The list's accepted values are: `sms_otp` and `totp`.
 
+      - scim_active_connections: (no documentation yet)
       - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
       - sso_default_connection_id: The default connection used for SSO when there are multiple active connections.
     """  # noqa
 
     organization_id: str
     organization_name: str
     organization_logo_url: str
@@ -233,14 +242,15 @@
     email_invites: str
     auth_methods: str
     allowed_auth_methods: List[str]
     mfa_policy: str
     rbac_email_implicit_role_assignments: List[EmailImplicitRoleAssignment]
     mfa_methods: str
     allowed_mfa_methods: List[str]
+    scim_active_connections: List[ActiveSCIMConnection]
     trusted_metadata: Optional[Dict[str, Any]] = None
     sso_default_connection_id: Optional[str] = None
 
 
 class ResultsMetadata(pydantic.BaseModel):
     """
     Fields:
```

### Comparing `stytch-9.0.0/stytch/b2b/models/organizations_members.py` & `stytch-9.1.0/stytch/b2b/models/organizations_members.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/organizations_members_oauth_providers.py` & `stytch-9.1.0/stytch/b2b/models/organizations_members_oauth_providers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/otp_sms.py` & `stytch-9.1.0/stytch/b2b/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/passwords.py` & `stytch-9.1.0/stytch/b2b/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/passwords_email.py` & `stytch-9.1.0/stytch/b2b/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/passwords_existing_password.py` & `stytch-9.1.0/stytch/b2b/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/passwords_session.py` & `stytch-9.1.0/stytch/b2b/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/rbac.py` & `stytch-9.1.0/stytch/b2b/models/rbac.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/recovery_codes.py` & `stytch-9.1.0/stytch/b2b/models/recovery_codes.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/scim.py` & `stytch-9.1.0/stytch/b2b/models/scim.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/scim_connections.py` & `stytch-9.1.0/stytch/b2b/models/sso_oidc.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,96 +2,66 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-import enum
-from typing import List, Optional
-
-from stytch.b2b.models.scim import (
-    SCIMConnection,
-    SCIMConnectionWithNextToken,
-    SCIMConnectionWithToken,
-)
-from stytch.core.response_base import ResponseBase
-
-
-class CreateRequestIdp(str, enum.Enum):
-    UNKNOWN = "unknown"
-    OKTA = "okta"
-    MICROSOFTENTRA = "microsoft-entra"
-    CYBERARK = "cyberark"
-    JUMPCLOUD = "jumpcloud"
-    ONELOGIN = "onelogin"
-    PINGFEDERATE = "pingfederate"
-    RIPPLING = "rippling"
-
-
-class UpdateRequestIdp(str, enum.Enum):
-    UNKNOWN = "unknown"
-    OKTA = "okta"
-    MICROSOFTENTRA = "microsoft-entra"
+from typing import Dict, Optional
 
+import pydantic
 
-class CreateResponse(ResponseBase):
-    """Response type for `Connections.create`.
-    Fields:
-      - connection: The `SCIM Connection` object affected by this API call. See the [SCIM Connection Object](https://stytch.com/docs/b2b/api/scim-connection-object) for complete response field details.
-    """  # noqa
-
-    connection: Optional[SCIMConnectionWithToken] = None
+from stytch.b2b.models.sso import OIDCConnection
+from stytch.core.response_base import ResponseBase
+from stytch.shared.method_options import Authorization
 
 
-class DeleteResponse(ResponseBase):
-    """Response type for `Connections.delete`.
+class CreateConnectionRequestOptions(pydantic.BaseModel):
+    """
     Fields:
-      - connection_id: The `connection_id` that was deleted as part of the delete request.
+      - authorization: Optional authorization object.
+    Pass in an active Stytch Member session token or session JWT and the request
+    will be run using that member's permissions.
     """  # noqa
 
-    connection_id: str
+    authorization: Optional[Authorization] = None
 
-
-class GetResponse(ResponseBase):
-    """Response type for `Connections.get`.
-    Fields:
-      - connections: (no documentation yet)
-    """  # noqa
-
-    connections: List[SCIMConnection]
+    def add_headers(self, headers: Dict[str, str]) -> Dict[str, str]:
+        if self.authorization is not None:
+            headers = self.authorization.add_headers(headers)
+        return headers
 
 
-class RotateCancelResponse(ResponseBase):
-    """Response type for `Connections.rotate_cancel`.
+class UpdateConnectionRequestOptions(pydantic.BaseModel):
+    """
     Fields:
-      - connection: The `SCIM Connection` object affected by this API call. See the [SCIM Connection Object](https://stytch.com/docs/b2b/api/scim-connection-object) for complete response field details.
+      - authorization: Optional authorization object.
+    Pass in an active Stytch Member session token or session JWT and the request
+    will be run using that member's permissions.
     """  # noqa
 
-    connection: Optional[SCIMConnection] = None
-
-
-class RotateCompleteResponse(ResponseBase):
-    """Response type for `Connections.rotate_complete`.
-    Fields:
-      - connection: The `SCIM Connection` object affected by this API call. See the [SCIM Connection Object](https://stytch.com/docs/b2b/api/scim-connection-object) for complete response field details.
-    """  # noqa
+    authorization: Optional[Authorization] = None
 
-    connection: Optional[SCIMConnection] = None
+    def add_headers(self, headers: Dict[str, str]) -> Dict[str, str]:
+        if self.authorization is not None:
+            headers = self.authorization.add_headers(headers)
+        return headers
 
 
-class RotateStartResponse(ResponseBase):
-    """Response type for `Connections.rotate_start`.
+class CreateConnectionResponse(ResponseBase):
+    """Response type for `OIDC.create_connection`.
     Fields:
-      - connection: The `SCIM Connection` object affected by this API call. See the [SCIM Connection Object](https://stytch.com/docs/b2b/api/scim-connection-object) for complete response field details.
+      - connection: The `OIDC Connection` object affected by this API call. See the [OIDC Connection Object](https://stytch.com/docs/b2b/api/oidc-connection-object) for complete response field details.
     """  # noqa
 
-    connection: Optional[SCIMConnectionWithNextToken] = None
+    connection: Optional[OIDCConnection] = None
 
 
-class UpdateResponse(ResponseBase):
-    """Response type for `Connections.update`.
+class UpdateConnectionResponse(ResponseBase):
+    """Response type for `OIDC.update_connection`.
     Fields:
-      - connection: The `SAML Connection` object affected by this API call. See the [SAML Connection Object](https://stytch.com/docs/b2b/api/saml-connection-object) for complete response field details.
+      - connection: The `OIDC Connection` object affected by this API call. See the [OIDC Connection Object](https://stytch.com/docs/b2b/api/oidc-connection-object) for complete response field details.
+      - warning: If it is not possible to resolve the well-known metadata document from the OIDC issuer, this field will explain what went wrong if the request is successful otherwise. In other words, even if the overall request succeeds, there could be relevant warnings related to the connection update.
     """  # noqa
 
-    connection: Optional[SCIMConnection] = None
+    connection: Optional[OIDCConnection] = None
+    warning: Optional[str] = None
```

### Comparing `stytch-9.0.0/stytch/b2b/models/sessions.py` & `stytch-9.1.0/stytch/b2b/models/sessions.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,14 +148,33 @@
     Fields:
       - member_sessions: An array of [Session objects](https://stytch.com/docs/b2b/api/session-object).
     """  # noqa
 
     member_sessions: List[MemberSession]
 
 
+class MigrateResponse(ResponseBase):
+    """Response type for `Sessions.migrate`.
+    Fields:
+      - member_id: Globally unique UUID that identifies a specific Member.
+      - session_token: A secret token for a given Stytch Session.
+      - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
+      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object)
+      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
+      - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
+    """  # noqa
+
+    member_id: str
+    session_token: str
+    session_jwt: str
+    member: Member
+    organization: Organization
+    member_session: Optional[MemberSession] = None
+
+
 class RevokeResponse(ResponseBase):
     """Response type for `Sessions.revoke`.
     Fields:
     """  # noqa
 
 
 # MANUAL(LocalJWTResponse)(Types)
```

### Comparing `stytch-9.0.0/stytch/b2b/models/sso.py` & `stytch-9.1.0/stytch/b2b/models/sso.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/b2b/models/sso_oidc.py` & `stytch-9.1.0/stytch/b2b/models/sso_saml.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from __future__ import annotations
 
 from typing import Dict, Optional
 
 import pydantic
 
-from stytch.b2b.models.sso import OIDCConnection
+from stytch.b2b.models.sso import SAMLConnection
 from stytch.core.response_base import ResponseBase
 from stytch.shared.method_options import Authorization
 
 
 class CreateConnectionRequestOptions(pydantic.BaseModel):
     """
     Fields:
@@ -27,14 +27,46 @@
 
     def add_headers(self, headers: Dict[str, str]) -> Dict[str, str]:
         if self.authorization is not None:
             headers = self.authorization.add_headers(headers)
         return headers
 
 
+class DeleteVerificationCertificateRequestOptions(pydantic.BaseModel):
+    """
+    Fields:
+      - authorization: Optional authorization object.
+    Pass in an active Stytch Member session token or session JWT and the request
+    will be run using that member's permissions.
+    """  # noqa
+
+    authorization: Optional[Authorization] = None
+
+    def add_headers(self, headers: Dict[str, str]) -> Dict[str, str]:
+        if self.authorization is not None:
+            headers = self.authorization.add_headers(headers)
+        return headers
+
+
+class UpdateByURLRequestOptions(pydantic.BaseModel):
+    """
+    Fields:
+      - authorization: Optional authorization object.
+    Pass in an active Stytch Member session token or session JWT and the request
+    will be run using that member's permissions.
+    """  # noqa
+
+    authorization: Optional[Authorization] = None
+
+    def add_headers(self, headers: Dict[str, str]) -> Dict[str, str]:
+        if self.authorization is not None:
+            headers = self.authorization.add_headers(headers)
+        return headers
+
+
 class UpdateConnectionRequestOptions(pydantic.BaseModel):
     """
     Fields:
       - authorization: Optional authorization object.
     Pass in an active Stytch Member session token or session JWT and the request
     will be run using that member's permissions.
     """  # noqa
@@ -44,24 +76,40 @@
     def add_headers(self, headers: Dict[str, str]) -> Dict[str, str]:
         if self.authorization is not None:
             headers = self.authorization.add_headers(headers)
         return headers
 
 
 class CreateConnectionResponse(ResponseBase):
-    """Response type for `OIDC.create_connection`.
+    """Response type for `SAML.create_connection`.
+    Fields:
+      - connection: The `SAML Connection` object affected by this API call. See the [SAML Connection Object](https://stytch.com/docs/b2b/api/saml-connection-object) for complete response field details.
+    """  # noqa
+
+    connection: Optional[SAMLConnection] = None
+
+
+class DeleteVerificationCertificateResponse(ResponseBase):
+    """Response type for `SAML.delete_verification_certificate`.
+    Fields:
+      - certificate_id: The ID of the certificate that was deleted.
+    """  # noqa
+
+    certificate_id: str
+
+
+class UpdateByURLResponse(ResponseBase):
+    """Response type for `SAML.update_by_url`.
     Fields:
-      - connection: The `OIDC Connection` object affected by this API call. See the [OIDC Connection Object](https://stytch.com/docs/b2b/api/oidc-connection-object) for complete response field details.
+      - connection: The `SAML Connection` object affected by this API call. See the [SAML Connection Object](https://stytch.com/docs/b2b/api/saml-connection-object) for complete response field details.
     """  # noqa
 
-    connection: Optional[OIDCConnection] = None
+    connection: Optional[SAMLConnection] = None
 
 
 class UpdateConnectionResponse(ResponseBase):
-    """Response type for `OIDC.update_connection`.
+    """Response type for `SAML.update_connection`.
     Fields:
-      - connection: The `OIDC Connection` object affected by this API call. See the [OIDC Connection Object](https://stytch.com/docs/b2b/api/oidc-connection-object) for complete response field details.
-      - warning: If it is not possible to resolve the well-known metadata document from the OIDC issuer, this field will explain what went wrong if the request is successful otherwise. In other words, even if the overall request succeeds, there could be relevant warnings related to the connection update.
+      - connection: The `SAML Connection` object affected by this API call. See the [SAML Connection Object](https://stytch.com/docs/b2b/api/saml-connection-object) for complete response field details.
     """  # noqa
 
-    connection: Optional[OIDCConnection] = None
-    warning: Optional[str] = None
+    connection: Optional[SAMLConnection] = None
```

### Comparing `stytch-9.0.0/stytch/b2b/models/sso_saml.py` & `stytch-9.1.0/stytch/b2b/models/scim_connections.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,24 +2,46 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-from typing import Dict, Optional
+import enum
+from typing import Dict, List, Optional
 
 import pydantic
 
-from stytch.b2b.models.sso import SAMLConnection
+from stytch.b2b.models.scim import (
+    SCIMConnection,
+    SCIMConnectionWithNextToken,
+    SCIMConnectionWithToken,
+)
 from stytch.core.response_base import ResponseBase
 from stytch.shared.method_options import Authorization
 
 
-class CreateConnectionRequestOptions(pydantic.BaseModel):
+class CreateRequestIdp(str, enum.Enum):
+    UNKNOWN = "unknown"
+    OKTA = "okta"
+    MICROSOFTENTRA = "microsoft-entra"
+    CYBERARK = "cyberark"
+    JUMPCLOUD = "jumpcloud"
+    ONELOGIN = "onelogin"
+    PINGFEDERATE = "pingfederate"
+    RIPPLING = "rippling"
+
+
+class UpdateRequestIdp(str, enum.Enum):
+    UNKNOWN = "unknown"
+    OKTA = "okta"
+    MICROSOFTENTRA = "microsoft-entra"
+
+
+class CreateRequestOptions(pydantic.BaseModel):
     """
     Fields:
       - authorization: Optional authorization object.
     Pass in an active Stytch Member session token or session JWT and the request
     will be run using that member's permissions.
     """  # noqa
 
@@ -27,15 +49,15 @@
 
     def add_headers(self, headers: Dict[str, str]) -> Dict[str, str]:
         if self.authorization is not None:
             headers = self.authorization.add_headers(headers)
         return headers
 
 
-class DeleteVerificationCertificateRequestOptions(pydantic.BaseModel):
+class DeleteRequestOptions(pydantic.BaseModel):
     """
     Fields:
       - authorization: Optional authorization object.
     Pass in an active Stytch Member session token or session JWT and the request
     will be run using that member's permissions.
     """  # noqa
 
@@ -43,15 +65,15 @@
 
     def add_headers(self, headers: Dict[str, str]) -> Dict[str, str]:
         if self.authorization is not None:
             headers = self.authorization.add_headers(headers)
         return headers
 
 
-class UpdateByURLRequestOptions(pydantic.BaseModel):
+class GetRequestOptions(pydantic.BaseModel):
     """
     Fields:
       - authorization: Optional authorization object.
     Pass in an active Stytch Member session token or session JWT and the request
     will be run using that member's permissions.
     """  # noqa
 
@@ -59,15 +81,15 @@
 
     def add_headers(self, headers: Dict[str, str]) -> Dict[str, str]:
         if self.authorization is not None:
             headers = self.authorization.add_headers(headers)
         return headers
 
 
-class UpdateConnectionRequestOptions(pydantic.BaseModel):
+class RotateCancelRequestOptions(pydantic.BaseModel):
     """
     Fields:
       - authorization: Optional authorization object.
     Pass in an active Stytch Member session token or session JWT and the request
     will be run using that member's permissions.
     """  # noqa
 
@@ -75,41 +97,116 @@
 
     def add_headers(self, headers: Dict[str, str]) -> Dict[str, str]:
         if self.authorization is not None:
             headers = self.authorization.add_headers(headers)
         return headers
 
 
-class CreateConnectionResponse(ResponseBase):
-    """Response type for `SAML.create_connection`.
+class RotateCompleteRequestOptions(pydantic.BaseModel):
+    """
     Fields:
-      - connection: The `SAML Connection` object affected by this API call. See the [SAML Connection Object](https://stytch.com/docs/b2b/api/saml-connection-object) for complete response field details.
+      - authorization: Optional authorization object.
+    Pass in an active Stytch Member session token or session JWT and the request
+    will be run using that member's permissions.
     """  # noqa
 
-    connection: Optional[SAMLConnection] = None
+    authorization: Optional[Authorization] = None
+
+    def add_headers(self, headers: Dict[str, str]) -> Dict[str, str]:
+        if self.authorization is not None:
+            headers = self.authorization.add_headers(headers)
+        return headers
 
 
-class DeleteVerificationCertificateResponse(ResponseBase):
-    """Response type for `SAML.delete_verification_certificate`.
+class RotateStartRequestOptions(pydantic.BaseModel):
+    """
     Fields:
-      - certificate_id: The ID of the certificate that was deleted.
+      - authorization: Optional authorization object.
+    Pass in an active Stytch Member session token or session JWT and the request
+    will be run using that member's permissions.
     """  # noqa
 
-    certificate_id: str
+    authorization: Optional[Authorization] = None
+
+    def add_headers(self, headers: Dict[str, str]) -> Dict[str, str]:
+        if self.authorization is not None:
+            headers = self.authorization.add_headers(headers)
+        return headers
 
 
-class UpdateByURLResponse(ResponseBase):
-    """Response type for `SAML.update_by_url`.
+class UpdateRequestOptions(pydantic.BaseModel):
+    """
     Fields:
-      - connection: The `SAML Connection` object affected by this API call. See the [SAML Connection Object](https://stytch.com/docs/b2b/api/saml-connection-object) for complete response field details.
+      - authorization: Optional authorization object.
+    Pass in an active Stytch Member session token or session JWT and the request
+    will be run using that member's permissions.
+    """  # noqa
+
+    authorization: Optional[Authorization] = None
+
+    def add_headers(self, headers: Dict[str, str]) -> Dict[str, str]:
+        if self.authorization is not None:
+            headers = self.authorization.add_headers(headers)
+        return headers
+
+
+class CreateResponse(ResponseBase):
+    """Response type for `Connections.create`.
+    Fields:
+      - connection: The `SCIM Connection` object affected by this API call. See the [SCIM Connection Object](https://stytch.com/docs/b2b/api/scim-connection-object) for complete response field details.
+    """  # noqa
+
+    connection: Optional[SCIMConnectionWithToken] = None
+
+
+class DeleteResponse(ResponseBase):
+    """Response type for `Connections.delete`.
+    Fields:
+      - connection_id: The `connection_id` that was deleted as part of the delete request.
+    """  # noqa
+
+    connection_id: str
+
+
+class GetResponse(ResponseBase):
+    """Response type for `Connections.get`.
+    Fields:
+      - connections: (no documentation yet)
+    """  # noqa
+
+    connections: List[SCIMConnection]
+
+
+class RotateCancelResponse(ResponseBase):
+    """Response type for `Connections.rotate_cancel`.
+    Fields:
+      - connection: The `SCIM Connection` object affected by this API call. See the [SCIM Connection Object](https://stytch.com/docs/b2b/api/scim-connection-object) for complete response field details.
+    """  # noqa
+
+    connection: Optional[SCIMConnection] = None
+
+
+class RotateCompleteResponse(ResponseBase):
+    """Response type for `Connections.rotate_complete`.
+    Fields:
+      - connection: The `SCIM Connection` object affected by this API call. See the [SCIM Connection Object](https://stytch.com/docs/b2b/api/scim-connection-object) for complete response field details.
+    """  # noqa
+
+    connection: Optional[SCIMConnection] = None
+
+
+class RotateStartResponse(ResponseBase):
+    """Response type for `Connections.rotate_start`.
+    Fields:
+      - connection: The `SCIM Connection` object affected by this API call. See the [SCIM Connection Object](https://stytch.com/docs/b2b/api/scim-connection-object) for complete response field details.
     """  # noqa
 
-    connection: Optional[SAMLConnection] = None
+    connection: Optional[SCIMConnectionWithNextToken] = None
 
 
-class UpdateConnectionResponse(ResponseBase):
-    """Response type for `SAML.update_connection`.
+class UpdateResponse(ResponseBase):
+    """Response type for `Connections.update`.
     Fields:
       - connection: The `SAML Connection` object affected by this API call. See the [SAML Connection Object](https://stytch.com/docs/b2b/api/saml-connection-object) for complete response field details.
     """  # noqa
 
-    connection: Optional[SAMLConnection] = None
+    connection: Optional[SCIMConnection] = None
```

### Comparing `stytch-9.0.0/stytch/b2b/models/totps.py` & `stytch-9.1.0/stytch/b2b/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/crypto_wallets.py` & `stytch-9.1.0/stytch/consumer/api/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/m2m.py` & `stytch-9.1.0/stytch/consumer/api/m2m.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/m2m_clients.py` & `stytch-9.1.0/stytch/consumer/api/m2m_clients.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/m2m_clients_secrets.py` & `stytch-9.1.0/stytch/consumer/api/m2m_clients_secrets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/magic_links.py` & `stytch-9.1.0/stytch/consumer/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/magic_links_email.py` & `stytch-9.1.0/stytch/consumer/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/oauth.py` & `stytch-9.1.0/stytch/consumer/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/otp.py` & `stytch-9.1.0/stytch/consumer/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/otp_email.py` & `stytch-9.1.0/stytch/consumer/api/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/otp_sms.py` & `stytch-9.1.0/stytch/consumer/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/otp_whatsapp.py` & `stytch-9.1.0/stytch/consumer/api/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/passwords.py` & `stytch-9.1.0/stytch/consumer/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/passwords_email.py` & `stytch-9.1.0/stytch/consumer/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/passwords_existing_password.py` & `stytch-9.1.0/stytch/consumer/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/passwords_session.py` & `stytch-9.1.0/stytch/consumer/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/project.py` & `stytch-9.1.0/stytch/consumer/api/project.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/sessions.py` & `stytch-9.1.0/stytch/consumer/api/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/totps.py` & `stytch-9.1.0/stytch/consumer/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/users.py` & `stytch-9.1.0/stytch/consumer/api/users.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/api/webauthn.py` & `stytch-9.1.0/stytch/consumer/api/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/client.py` & `stytch-9.1.0/stytch/consumer/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/crypto_wallets.py` & `stytch-9.1.0/stytch/consumer/models/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/m2m.py` & `stytch-9.1.0/stytch/consumer/models/m2m.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/m2m_clients.py` & `stytch-9.1.0/stytch/consumer/models/m2m_clients.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/m2m_clients_secrets.py` & `stytch-9.1.0/stytch/consumer/models/m2m_clients_secrets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/magic_links.py` & `stytch-9.1.0/stytch/consumer/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/magic_links_email.py` & `stytch-9.1.0/stytch/consumer/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/oauth.py` & `stytch-9.1.0/stytch/consumer/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/otp.py` & `stytch-9.1.0/stytch/consumer/models/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/otp_email.py` & `stytch-9.1.0/stytch/consumer/models/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/otp_sms.py` & `stytch-9.1.0/stytch/consumer/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/otp_whatsapp.py` & `stytch-9.1.0/stytch/consumer/models/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/passwords.py` & `stytch-9.1.0/stytch/consumer/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/passwords_email.py` & `stytch-9.1.0/stytch/consumer/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/passwords_existing_password.py` & `stytch-9.1.0/stytch/consumer/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/passwords_session.py` & `stytch-9.1.0/stytch/consumer/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/project.py` & `stytch-9.1.0/stytch/consumer/models/project.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/sessions.py` & `stytch-9.1.0/stytch/consumer/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/totps.py` & `stytch-9.1.0/stytch/consumer/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/users.py` & `stytch-9.1.0/stytch/consumer/models/users.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/consumer/models/webauthn.py` & `stytch-9.1.0/stytch/consumer/models/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/core/api_base.py` & `stytch-9.1.0/stytch/core/api_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/core/client_base.py` & `stytch-9.1.0/stytch/core/client_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/core/http/client.py` & `stytch-9.1.0/stytch/core/http/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/core/response_base.py` & `stytch-9.1.0/stytch/core/response_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/shared/jwt_helpers.py` & `stytch-9.1.0/stytch/shared/jwt_helpers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/shared/lazy_cache.py` & `stytch-9.1.0/stytch/shared/lazy_cache.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/shared/method_options.py` & `stytch-9.1.0/stytch/shared/method_options.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/shared/policy_cache.py` & `stytch-9.1.0/stytch/shared/policy_cache.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch/shared/rbac_local.py` & `stytch-9.1.0/stytch/shared/rbac_local.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/stytch.egg-info/PKG-INFO` & `stytch-9.1.0/stytch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 9.0.0
+Version: 9.1.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-9.0.0/stytch.egg-info/SOURCES.txt` & `stytch-9.1.0/stytch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/test/test_integration.py` & `stytch-9.1.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `stytch-9.0.0/test/test_integration_async.py` & `stytch-9.1.0/test/test_integration_async.py`

 * *Files identical despite different names*

