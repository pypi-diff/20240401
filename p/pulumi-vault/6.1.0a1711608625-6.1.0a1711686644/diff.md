# Comparing `tmp/pulumi_vault-6.1.0a1711608625.tar.gz` & `tmp/pulumi_vault-6.1.0a1711686644.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_vault-6.1.0a1711608625.tar", last modified: Thu Mar 28 06:55:46 2024, max compression
+gzip compressed data, was "pulumi_vault-6.1.0a1711686644.tar", last modified: Fri Mar 29 04:35:32 2024, max compression
```

## Comparing `pulumi_vault-6.1.0a1711608625.tar` & `pulumi_vault-6.1.0a1711686644.tar`

### file list

```diff
@@ -1,285 +1,285 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.302578 pulumi_vault-6.1.0a1711608625/
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-03-28 06:55:46.302578 pulumi_vault-6.1.0a1711608625/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.258578 pulumi_vault-6.1.0a1711608625/pulumi_vault/
--rw-r--r--   0 runner    (1001) docker     (127)    30974 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73552 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.258578 pulumi_vault-6.1.0a1711608625/pulumi_vault/ad/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ad/get_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    92297 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ad/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    23836 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ad/secret_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    20632 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ad/secret_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.262578 pulumi_vault-6.1.0a1711608625/pulumi_vault/alicloud/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/alicloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45928 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/alicloud/auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.262578 pulumi_vault-6.1.0a1711608625/pulumi_vault/approle/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/approle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23505 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/approle/auth_backend_login.py
--rw-r--r--   0 runner    (1001) docker     (127)    56646 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/approle/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    31940 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/approle/auth_backend_role_secret_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/approle/get_auth_backend_role_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    20655 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/audit_request_header.py
--rw-r--r--   0 runner    (1001) docker     (127)    21605 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/auth_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.266578 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18369 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    32902 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23288 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_config_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_identity_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    43043 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_login.py
--rw-r--r--   0 runner    (1001) docker     (127)   110667 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    26592 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_role_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    16794 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_roletag_blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_sts_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12282 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/get_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/get_static_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    46971 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    48260 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    17927 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/secret_backend_static_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.266578 pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23762 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/auth_backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    64878 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    29406 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    39236 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    17943 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/get_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    83407 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/cert_auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.266578 pulumi_vault-6.1.0a1711608625/pulumi_vault/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/config/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42626 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22482 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/config/ui_custom_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.266578 pulumi_vault-6.1.0a1711608625/pulumi_vault/consul/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/consul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39828 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/consul/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    41615 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/consul/secret_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.270578 pulumi_vault-6.1.0a1711608625/pulumi_vault/database/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   298321 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/database/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   261078 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/database/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    73279 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/database/secret_backend_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    36912 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/database/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    30731 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/database/secret_backend_static_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    98130 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/database/secrets_mount.py
--rw-r--r--   0 runner    (1001) docker     (127)    16697 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/egp_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.270578 pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38638 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    73886 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/get_auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24908 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18919 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/secret_impersonated_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    26079 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/secret_roleset.py
--rw-r--r--   0 runner    (1001) docker     (127)    27423 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/secret_static_account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.274578 pulumi_vault-6.1.0a1711608625/pulumi_vault/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39221 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/generic/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    10380 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/generic/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/generic/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/get_auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/get_auth_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/get_nomad_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/get_policy_document.py
--rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/get_raft_autopilot_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.274578 pulumi_vault-6.1.0a1711608625/pulumi_vault/github/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/github/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    56571 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/github/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/github/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15482 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/github/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/github/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.278578 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19932 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    18641 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/entity_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    20083 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/entity_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    14491 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/get_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    18096 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/get_oidc_client_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/get_oidc_openid_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/get_oidc_public_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    37780 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    17404 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/group_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    20554 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/group_member_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    20180 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/group_member_group_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    20431 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/group_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    25146 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/mfa_duo.py
--rw-r--r--   0 runner    (1001) docker     (127)    23785 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/mfa_login_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (127)    23189 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/mfa_okta.py
--rw-r--r--   0 runner    (1001) docker     (127)    23924 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/mfa_pingid.py
--rw-r--r--   0 runner    (1001) docker     (127)    29583 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/mfa_totp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12422 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15261 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    29879 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21120 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_key_allowed_client_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    22020 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    14701 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.278578 pulumi_vault-6.1.0a1711608625/pulumi_vault/jwt/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/jwt/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    66520 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/jwt/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    97651 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/jwt/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/jwt/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.282578 pulumi_vault-6.1.0a1711608625/pulumi_vault/kmip/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kmip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37931 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kmip/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    54561 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kmip/secret_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    14926 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kmip/secret_scope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.282578 pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31330 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/auth_backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    57046 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/get_auth_backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    21357 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/get_auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/get_service_account_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    50850 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    50157 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/secret_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.286578 pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/get_secret_subkeys_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/get_secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/get_secrets_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/get_secrets_list_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/secret_backend_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    35933 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/secret_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.286578 pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    92297 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    16577 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/auth_backend_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/auth_backend_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/get_dynamic_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/get_static_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    77631 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    37953 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/secret_backend_dynamic_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/secret_backend_library_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    24131 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/secret_backend_static_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.286578 pulumi_vault-6.1.0a1711608625/pulumi_vault/managed/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/managed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29364 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/managed/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/managed/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    25252 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/managed/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28337 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/mfa_duo.py
--rw-r--r--   0 runner    (1001) docker     (127)    29601 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/mfa_okta.py
--rw-r--r--   0 runner    (1001) docker     (127)    31066 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/mfa_pingid.py
--rw-r--r--   0 runner    (1001) docker     (127)    25442 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/mfa_totp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.286578 pulumi_vault-6.1.0a1711608625/pulumi_vault/mongodbatlas/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/mongodbatlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16315 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/mongodbatlas/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    31758 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/mongodbatlas/secret_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    41533 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)    18077 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    42174 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/nomad_secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    20302 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/nomad_secret_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.290578 pulumi_vault-6.1.0a1711608625/pulumi_vault/okta/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38494 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/okta/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15131 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/okta/auth_backend_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    17093 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/okta/auth_backend_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/okta/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13760 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/password_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.294578 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16085 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/backend_config_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/get_backend_issuer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/get_backend_issuers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/get_backend_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/get_backend_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    49885 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    19122 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_config_ca.py
--rw-r--r--   0 runner    (1001) docker     (127)    17134 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_config_issuers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22199 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_config_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    36965 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_crl_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    62005 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    20552 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py
--rw-r--r--   0 runner    (1001) docker     (127)    36781 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_issuer.py
--rw-r--r--   0 runner    (1001) docker     (127)    25523 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_key.py
--rw-r--r--   0 runner    (1001) docker     (127)   116321 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    69049 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_root_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    58798 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (127)    48764 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_sign.py
--rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    42332 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21122 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/quota_lease_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    25727 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/quota_rate_limit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.294578 pulumi_vault-6.1.0a1711608625/pulumi_vault/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/rabbitmq/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/rabbitmq/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34778 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/rabbitmq/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    21960 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/rabbitmq/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    30215 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/raft_autopilot.py
--rw-r--r--   0 runner    (1001) docker     (127)    84163 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/raft_snapshot_agent_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14494 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/rgp_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.294578 pulumi_vault-6.1.0a1711608625/pulumi_vault/saml/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/saml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33638 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/saml/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    55597 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/saml/auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.298578 pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18776 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_association.py
--rw-r--r--   0 runner    (1001) docker     (127)    36080 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_aws_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    29826 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_azure_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    23697 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_gcp_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    29701 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_gh_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_github_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    24164 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_vercel_destination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.298578 pulumi_vault-6.1.0a1711608625/pulumi_vault/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ssh/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ssh/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18031 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ssh/secret_backend_ca.py
--rw-r--r--   0 runner    (1001) docker     (127)    72441 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/ssh/secret_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.298578 pulumi_vault-6.1.0a1711608625/pulumi_vault/terraformcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/terraformcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26449 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/terraformcloud/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18612 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/terraformcloud/secret_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)    22952 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/terraformcloud/secret_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    43519 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.298578 pulumi_vault-6.1.0a1711608625/pulumi_vault/tokenauth/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/tokenauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61380 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/tokenauth/auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.298578 pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13773 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/alphabet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/get_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/get_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)    14508 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    25649 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    26624 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.302578 pulumi_vault-6.1.0a1711608625/pulumi_vault/transit/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/transit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/transit/get_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/transit/get_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)    53364 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/transit/secret_backend_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault/transit/secret_cache_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 06:55:46.302578 pulumi_vault-6.1.0a1711608625/pulumi_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-03-28 06:55:46.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-03-28 06:55:46.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 06:55:46.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-28 06:55:46.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-28 06:55:46.000000 pulumi_vault-6.1.0a1711608625/pulumi_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-28 06:55:37.000000 pulumi_vault-6.1.0a1711608625/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 06:55:46.302578 pulumi_vault-6.1.0a1711608625/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.925255 pulumi_vault-6.1.0a1711686644/
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-03-29 04:35:32.925255 pulumi_vault-6.1.0a1711686644/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.885254 pulumi_vault-6.1.0a1711686644/pulumi_vault/
+-rw-r--r--   0 runner    (1001) docker     (127)    30974 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73552 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.885254 pulumi_vault-6.1.0a1711686644/pulumi_vault/ad/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ad/get_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92297 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ad/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23836 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ad/secret_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20632 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ad/secret_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.885254 pulumi_vault-6.1.0a1711686644/pulumi_vault/alicloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/alicloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45928 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/alicloud/auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.885254 pulumi_vault-6.1.0a1711686644/pulumi_vault/approle/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/approle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23505 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/approle/auth_backend_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56646 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/approle/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31940 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/approle/auth_backend_role_secret_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/approle/get_auth_backend_role_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20655 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/audit_request_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21605 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/auth_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.889255 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18369 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32902 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23288 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_config_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_identity_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43043 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110667 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26592 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_role_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16794 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_roletag_blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_sts_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12282 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/get_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/get_static_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46971 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48260 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17927 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/secret_backend_static_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.889255 pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23762 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/auth_backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64878 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29406 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39236 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17943 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/get_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83407 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/cert_auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.893255 pulumi_vault-6.1.0a1711686644/pulumi_vault/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/config/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42626 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22482 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/config/ui_custom_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.893255 pulumi_vault-6.1.0a1711686644/pulumi_vault/consul/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/consul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39828 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/consul/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41615 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/consul/secret_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.893255 pulumi_vault-6.1.0a1711686644/pulumi_vault/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   298321 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/database/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   261078 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/database/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73279 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/database/secret_backend_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36912 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/database/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30731 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/database/secret_backend_static_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98130 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/database/secrets_mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16697 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/egp_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.897255 pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38638 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73886 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/get_auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24908 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18919 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/secret_impersonated_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26079 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/secret_roleset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27423 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/secret_static_account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.897255 pulumi_vault-6.1.0a1711686644/pulumi_vault/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39221 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/generic/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10380 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/generic/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/generic/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/get_auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/get_auth_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/get_nomad_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/get_policy_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/get_raft_autopilot_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.897255 pulumi_vault-6.1.0a1711686644/pulumi_vault/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/github/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56571 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/github/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/github/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15482 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/github/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/github/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.901255 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19932 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18641 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/entity_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20083 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/entity_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14491 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/get_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18096 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/get_oidc_client_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/get_oidc_openid_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/get_oidc_public_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37780 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17404 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/group_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20554 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/group_member_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20180 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/group_member_group_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20431 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/group_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25146 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/mfa_duo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23785 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/mfa_login_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23189 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/mfa_okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23924 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/mfa_pingid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29583 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/mfa_totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12422 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15261 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29879 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21120 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_key_allowed_client_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22020 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14701 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.905255 pulumi_vault-6.1.0a1711686644/pulumi_vault/jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/jwt/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66520 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/jwt/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97651 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/jwt/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/jwt/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.905255 pulumi_vault-6.1.0a1711686644/pulumi_vault/kmip/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kmip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37931 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kmip/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54561 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kmip/secret_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14926 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kmip/secret_scope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.905255 pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31330 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/auth_backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57046 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/get_auth_backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21357 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/get_auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/get_service_account_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50850 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50157 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/secret_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.909255 pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/get_secret_subkeys_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/get_secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/get_secrets_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/get_secrets_list_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/secret_backend_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35933 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/secret_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.909255 pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92297 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16577 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/auth_backend_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/auth_backend_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/get_dynamic_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/get_static_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77631 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37953 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/secret_backend_dynamic_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/secret_backend_library_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24131 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/secret_backend_static_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.909255 pulumi_vault-6.1.0a1711686644/pulumi_vault/managed/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/managed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29364 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/managed/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/managed/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25252 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/managed/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28337 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/mfa_duo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29601 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/mfa_okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31066 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/mfa_pingid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25442 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/mfa_totp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.913255 pulumi_vault-6.1.0a1711686644/pulumi_vault/mongodbatlas/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/mongodbatlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16315 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/mongodbatlas/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31758 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/mongodbatlas/secret_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41533 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18077 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42174 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/nomad_secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20302 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/nomad_secret_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.913255 pulumi_vault-6.1.0a1711686644/pulumi_vault/okta/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38494 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/okta/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15131 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/okta/auth_backend_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17093 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/okta/auth_backend_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/okta/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13760 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/password_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.917255 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16085 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/backend_config_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/get_backend_issuer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/get_backend_issuers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/get_backend_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/get_backend_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49885 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19122 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_config_ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17134 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_config_issuers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22199 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_config_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36965 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_crl_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62005 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20552 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36781 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_issuer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25523 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116321 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69049 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_root_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58798 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48764 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42332 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21122 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/quota_lease_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25727 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/quota_rate_limit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.917255 pulumi_vault-6.1.0a1711686644/pulumi_vault/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/rabbitmq/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/rabbitmq/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34778 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/rabbitmq/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21960 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/rabbitmq/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30215 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/raft_autopilot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84163 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/raft_snapshot_agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14494 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/rgp_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.917255 pulumi_vault-6.1.0a1711686644/pulumi_vault/saml/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/saml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33638 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/saml/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55597 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/saml/auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.921255 pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18776 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36080 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_aws_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29826 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_azure_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23697 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_gcp_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29701 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_gh_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_github_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24164 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_vercel_destination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.921255 pulumi_vault-6.1.0a1711686644/pulumi_vault/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ssh/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ssh/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18031 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ssh/secret_backend_ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72441 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/ssh/secret_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.921255 pulumi_vault-6.1.0a1711686644/pulumi_vault/terraformcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/terraformcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26449 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/terraformcloud/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18612 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/terraformcloud/secret_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22952 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/terraformcloud/secret_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43519 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.921255 pulumi_vault-6.1.0a1711686644/pulumi_vault/tokenauth/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/tokenauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61380 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/tokenauth/auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.921255 pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13773 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/alphabet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/get_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/get_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14508 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25649 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26624 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.925255 pulumi_vault-6.1.0a1711686644/pulumi_vault/transit/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/transit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/transit/get_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/transit/get_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53364 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/transit/secret_backend_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault/transit/secret_cache_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:35:32.925255 pulumi_vault-6.1.0a1711686644/pulumi_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-03-29 04:35:32.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-03-29 04:35:32.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 04:35:32.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 04:35:32.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-29 04:35:32.000000 pulumi_vault-6.1.0a1711686644/pulumi_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-29 04:35:25.000000 pulumi_vault-6.1.0a1711686644/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 04:35:32.925255 pulumi_vault-6.1.0a1711686644/setup.cfg
```

### Comparing `pulumi_vault-6.1.0a1711608625/PKG-INFO` & `pulumi_vault-6.1.0a1711686644/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_vault
-Version: 6.1.0a1711608625
+Version: 6.1.0a1711686644
 Summary: A Pulumi package for creating and managing HashiCorp Vault cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-vault
 Keywords: pulumi,vault
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_vault-6.1.0a1711608625/README.md` & `pulumi_vault-6.1.0a1711686644/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/__init__.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/_inputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/_utilities.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ad/get_access_credentials.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ad/get_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ad/secret_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ad/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ad/secret_library.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ad/secret_library.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ad/secret_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ad/secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/alicloud/auth_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/alicloud/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/approle/auth_backend_login.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/approle/auth_backend_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/approle/auth_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/approle/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/approle/auth_backend_role_secret_id.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/approle/auth_backend_role_secret_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/approle/get_auth_backend_role_id.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/approle/get_auth_backend_role_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/audit.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/audit.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/audit_request_header.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/audit_request_header.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/auth_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/__init__.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_cert.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_client.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_config_identity.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_config_identity.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_identity_whitelist.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_identity_whitelist.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_login.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_role_tag.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_role_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_roletag_blacklist.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_roletag_blacklist.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/auth_backend_sts_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/auth_backend_sts_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/get_access_credentials.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/get_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/get_static_access_credentials.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/get_static_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/secret_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/secret_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/aws/secret_backend_static_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/aws/secret_backend_static_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/_inputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/auth_backend_config.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/auth_backend_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/auth_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/get_access_credentials.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/get_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/azure/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/azure/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/cert_auth_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/cert_auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/config/__init__.pyi` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/config/_inputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/config/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/config/ui_custom_message.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/config/ui_custom_message.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/config/vars.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/consul/secret_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/consul/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/consul/secret_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/consul/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/database/_inputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/database/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/database/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/database/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/database/secret_backend_connection.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/database/secret_backend_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/database/secret_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/database/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/database/secret_backend_static_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/database/secret_backend_static_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/database/secrets_mount.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/database/secrets_mount.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/egp_policy.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/egp_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/__init__.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/_inputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/auth_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/auth_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/get_auth_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/get_auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/secret_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/secret_impersonated_account.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/secret_impersonated_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/secret_roleset.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/secret_roleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/gcp/secret_static_account.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/gcp/secret_static_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/generic/endpoint.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/generic/endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/generic/get_secret.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/generic/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/generic/secret.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/generic/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/get_auth_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/get_auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/get_auth_backends.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/get_auth_backends.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/get_nomad_access_token.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/get_nomad_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/get_policy_document.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/get_policy_document.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/get_raft_autopilot_state.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/get_raft_autopilot_state.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/github/_inputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/github/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/github/auth_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/github/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/github/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/github/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/github/team.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/github/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/github/user.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/github/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/__init__.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/entity.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/entity.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/entity_alias.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/entity_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/entity_policies.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/entity_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/get_entity.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/get_entity.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/get_group.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/get_oidc_client_creds.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/get_oidc_client_creds.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/get_oidc_openid_config.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/get_oidc_openid_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/get_oidc_public_keys.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/get_oidc_public_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/group.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/group_alias.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/group_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/group_member_entity_ids.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/group_member_entity_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/group_member_group_ids.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/group_member_group_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/group_policies.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/group_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/mfa_duo.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/mfa_duo.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/mfa_login_enforcement.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/mfa_login_enforcement.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/mfa_okta.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/mfa_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/mfa_pingid.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/mfa_pingid.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/mfa_totp.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/mfa_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_assignment.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_client.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_key.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_key_allowed_client_id.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_key_allowed_client_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_provider.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/oidc_scope.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/oidc_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/identity/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/identity/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/jwt/_inputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/jwt/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/jwt/auth_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/jwt/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/jwt/auth_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/jwt/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/jwt/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/jwt/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kmip/secret_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kmip/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kmip/secret_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kmip/secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kmip/secret_scope.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kmip/secret_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/__init__.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/auth_backend_config.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/auth_backend_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/auth_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/get_auth_backend_config.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/get_auth_backend_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/get_auth_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/get_auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/get_service_account_token.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/get_service_account_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/secret_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kubernetes/secret_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kubernetes/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/__init__.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/_inputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/get_secret.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/get_secret_subkeys_v2.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/get_secret_subkeys_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/get_secret_v2.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/get_secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/get_secrets_list.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/get_secrets_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/get_secrets_list_v2.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/get_secrets_list_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/secret.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/secret_backend_v2.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/secret_backend_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/kv/secret_v2.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/kv/secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/__init__.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/auth_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/auth_backend_group.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/auth_backend_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/auth_backend_user.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/auth_backend_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/get_dynamic_credentials.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/get_dynamic_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/get_static_credentials.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/get_static_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/secret_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/secret_backend_dynamic_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/secret_backend_dynamic_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/secret_backend_library_set.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/secret_backend_library_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ldap/secret_backend_static_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ldap/secret_backend_static_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/managed/_inputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/managed/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/managed/keys.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/managed/keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/managed/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/managed/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/mfa_duo.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/mfa_duo.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/mfa_okta.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/mfa_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/mfa_pingid.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/mfa_pingid.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/mfa_totp.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/mfa_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/mongodbatlas/secret_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/mongodbatlas/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/mongodbatlas/secret_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/mongodbatlas/secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/mount.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/mount.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/namespace.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/nomad_secret_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/nomad_secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/nomad_secret_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/nomad_secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/okta/_inputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/okta/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/okta/auth_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/okta/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/okta/auth_backend_group.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/okta/auth_backend_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/okta/auth_backend_user.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/okta/auth_backend_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/okta/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/okta/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/password_policy.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/password_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/__init__.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/_inputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/backend_config_cluster.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/backend_config_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/get_backend_issuer.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/get_backend_issuer.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/get_backend_issuers.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/get_backend_issuers.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/get_backend_key.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/get_backend_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/get_backend_keys.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/get_backend_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_cert.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_config_ca.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_config_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_config_issuers.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_config_issuers.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_config_urls.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_config_urls.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_crl_config.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_crl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_issuer.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_issuer.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_key.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_root_cert.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_root_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/pkisecret/secret_backend_sign.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/pkisecret/secret_backend_sign.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/policy.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/provider.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/quota_lease_count.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/quota_lease_count.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/quota_rate_limit.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/quota_rate_limit.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/rabbitmq/_inputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/rabbitmq/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/rabbitmq/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/rabbitmq/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/rabbitmq/secret_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/rabbitmq/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/rabbitmq/secret_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/rabbitmq/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/raft_autopilot.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/raft_autopilot.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/raft_snapshot_agent_config.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/raft_snapshot_agent_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/rgp_policy.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/rgp_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/saml/auth_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/saml/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/saml/auth_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/saml/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/__init__.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_association.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_aws_destination.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_aws_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_azure_destination.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_azure_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_config.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_gcp_destination.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_gcp_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_gh_destination.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_gh_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_github_apps.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_github_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/secrets/sync_vercel_destination.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/secrets/sync_vercel_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ssh/_inputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ssh/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ssh/outputs.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ssh/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ssh/secret_backend_ca.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ssh/secret_backend_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/ssh/secret_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/ssh/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/terraformcloud/secret_backend.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/terraformcloud/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/terraformcloud/secret_creds.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/terraformcloud/secret_creds.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/terraformcloud/secret_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/terraformcloud/secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/token.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/tokenauth/auth_backend_role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/tokenauth/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/alphabet.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/alphabet.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/get_decode.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/get_decode.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/get_encode.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/get_encode.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/role.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/template.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/template.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/transform/transformation.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/transform/transformation.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/transit/get_decrypt.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/transit/get_decrypt.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/transit/get_encrypt.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/transit/get_encrypt.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/transit/secret_backend_key.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/transit/secret_backend_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault/transit/secret_cache_config.py` & `pulumi_vault-6.1.0a1711686644/pulumi_vault/transit/secret_cache_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault.egg-info/PKG-INFO` & `pulumi_vault-6.1.0a1711686644/pulumi_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_vault
-Version: 6.1.0a1711608625
+Version: 6.1.0a1711686644
 Summary: A Pulumi package for creating and managing HashiCorp Vault cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-vault
 Keywords: pulumi,vault
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_vault-6.1.0a1711608625/pulumi_vault.egg-info/SOURCES.txt` & `pulumi_vault-6.1.0a1711686644/pulumi_vault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.1.0a1711608625/pyproject.toml` & `pulumi_vault-6.1.0a1711686644/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_vault"
   description = "A Pulumi package for creating and managing HashiCorp Vault cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "vault"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "6.1.0a1711608625"
+  version = "6.1.0a1711686644"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-vault"
 
 [build-system]
```

