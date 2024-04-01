# Comparing `tmp/ostorlab-1.0.2.tar.gz` & `tmp/ostorlab-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ostorlab-1.0.2.tar", last modified: Thu Mar 28 13:50:54 2024, max compression
+gzip compressed data, was "ostorlab-1.0.3.tar", last modified: Mon Apr  1 20:11:53 2024, max compression
```

## Comparing `ostorlab-1.0.2.tar` & `ostorlab-1.0.3.tar`

### file list

```diff
@@ -1,1480 +1,1480 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.399589 ostorlab-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-28 13:50:44.000000 ostorlab-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-03-28 13:50:54.399589 ostorlab-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-03-28 13:50:44.000000 ostorlab-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-28 13:50:54.403589 ostorlab-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-28 13:50:44.000000 ostorlab-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.175591 ostorlab-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.219591 ostorlab-1.0.2/src/ostorlab/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.223591 ostorlab-1.0.2/src/ostorlab/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21209 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.223591 ostorlab-1.0.2/src/ostorlab/agent/kb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.223591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.187591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.179591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.223591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.223591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.223591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.223591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.179591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.227591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.227591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.227591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.227591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.227591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.179591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.227591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.227591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.183591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.227591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.231591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.231591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.231591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.231591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.231591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.231591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.231591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.231591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.235591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.235591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.235591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.235591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.235591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.235591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.235591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.235591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.235591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.239591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.239591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.239591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.239591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.239591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.239591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.239591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.239591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.243590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.243590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.243590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.243590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.243590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.243590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.243590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.243590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.243590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.247590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.247590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.247590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.247590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.247590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.247590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.247590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.247590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.251590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.251590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.251590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.251590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.251590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.251590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.183591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.251590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.251590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.255590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.255590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.255590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.255590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/context.md
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.255590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.255590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.255590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.255590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.187591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.259590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.259590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.259590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.259590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.259590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.259590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.259590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.259590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.263590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.263590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.263590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.263590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.263590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.263590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.263590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.267590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.267590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.267590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/context.md
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.187591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.267590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.267590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.267590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.187591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.267590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.267590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.271590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.271590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.191591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.187591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.271590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.271590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.187591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.271590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/context.md
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.271590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.191591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.271590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/context.md
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.275590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.275590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.275590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.275590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.275590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.275590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.275590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.275590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.279590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/context.md
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.279590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.279590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.279590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.279590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.191591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.279590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.191591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.279590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.283590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.191591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.283590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.283590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.191591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.283590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/context.md
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.283590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.283590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.283590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.287590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.287590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.287590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.287590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.287590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.287590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.287590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.287590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.291590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.291590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.291590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.291590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.291590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.291590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.291590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.291590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.295590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.295590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.295590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.295590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.295590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.295590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.295590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.295590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.299590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.299590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.299590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.299590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.299590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.299590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.299590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.303590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.303590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.303590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.303590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.303590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.303590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.303590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.303590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.307590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.307590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.307590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.195591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.307590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.199591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.307590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.307590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/recommendation.md
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.199591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.199591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.199591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.307590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.199591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.307590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.199591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.199591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.311590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.199591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.311590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.199591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.199591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.311590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.203591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.199591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.311590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.311590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.311590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.311590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.315590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.315590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.315590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.315590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.315590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.315590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.315590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.199591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.315590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.319590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.319590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.319590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.319590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.319590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.319590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.319590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.203591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.319590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.323590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.323590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.323590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.323590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.323590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.323590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.323590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.327590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.203591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.327590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.327590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.203591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.327590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.327590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.327590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.327590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.203591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.327590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.331590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.331590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.331590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.331590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.331590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.331590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.331590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.335590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.335590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.335590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.335590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.203591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.335590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.203591 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.335590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.335590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.335590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.339590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17461 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tests/kb_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.339590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tests/tools/kb_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.339590 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-03-28 13:50:45.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tools/kb_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/kb/kb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.339590 ostorlab-1.0.2/src/ostorlab/agent/message/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.339590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.339590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.339590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/common/x509/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/common/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/common/x509/x509_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.339590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.339590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.339590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/agent/agent_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.339590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.339590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/dns_record_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/domain_name_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.343590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/service_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.343590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/whois_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.343590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.343590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/android/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/android/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.343590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/aab_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.343590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/apk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/file_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.343590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/ios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/ios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.343590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/ipa_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.343590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/sbom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/sbom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/sbom/sbom_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.343590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/source/source_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.343590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/ip_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.343590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.343590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/geolocation_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.347590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/port_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.347590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.347590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/http_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/v4_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.347590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/whois_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.347590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.347590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/geolocation_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.347590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/port_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.347590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.347590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/http_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/v6_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.347590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/whois_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.347590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/link/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/link/link_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.347590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.351590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/android_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/android_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/android_store/android_store_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.351590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/developer_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.351590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.351590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/developer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/ios_store_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.351590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.351590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/artifact/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/artifact/artifact_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.351590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/filesystem/filesystem_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.351590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.351590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/http/request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/http/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/http/request/request_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.351590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/http/response/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/http/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/http/response/response_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.351590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/logs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/logs/logs_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.351590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/request_response/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/request_response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/request_response/request_response_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.351590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/ui_call/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/ui_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/ui_call/ui_call_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/control/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/control/control_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/x509_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/backend_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/feature_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/metadata_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/feature_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/file_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.355590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/backend_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/feature_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/metadata_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/x509_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/x509_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/healthcheck/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/healthcheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.359590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/healthcheck/ping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/healthcheck/ping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/healthcheck/ping/ping_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/cve/
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/cve/cve_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/done_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/start_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/timeout_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/done/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/done/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/done/done_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/start/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/start/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/start/start_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/timeout_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/status/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/status/status_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/vulnerability/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/vulnerability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/vulnerability/vulnerability_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/use/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/use/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.363590 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/use/device/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/use/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/use/device/device_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/proto_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/message/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.367590 ostorlab-1.0.2/src/ostorlab/agent/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/mixins/agent_healthcheck_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/mixins/agent_mq_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/mixins/agent_open_telemetry_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/mixins/agent_persist_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/mixins/agent_report_vulnerability_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.367590 ostorlab-1.0.2/src/ostorlab/agent/mixins/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/mixins/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/mixins/protocols/emit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.367590 ostorlab-1.0.2/src/ostorlab/agent/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/schema/agent_group_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/schema/agent_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/schema/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/schema/target_group_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/agent/schema/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.371590 ostorlab-1.0.2/src/ostorlab/apis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/add_scanner_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/agent_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/agent_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/agent_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/create_agent_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/create_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/revoke_api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.371590 ostorlab-1.0.2/src/ostorlab/apis/runners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/runners/authenticated_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/runners/login_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/runners/public_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/runners/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/scan_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/scan_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/scan_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/scan_stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/scanner_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/test_credentials_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/vulnz_describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/apis/vulnz_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.375590 ostorlab-1.0.2/src/ostorlab/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/TODO.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/android_aab.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/android_apk.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/android_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/ios_ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/ios_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/assets/link.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.375590 ostorlab-1.0.2/src/ostorlab/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.375590 ostorlab-1.0.2/src/ostorlab/cli/agent/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.375590 ostorlab-1.0.2/src/ostorlab/cli/agent/build/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/build/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/build/build_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.375590 ostorlab-1.0.2/src/ostorlab/cli/agent/delete/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/delete/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.375590 ostorlab-1.0.2/src/ostorlab/cli/agent/healthcheck/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/healthcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/healthcheck/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.379590 ostorlab-1.0.2/src/ostorlab/cli/agent/install/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/install/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/install/install_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.379590 ostorlab-1.0.2/src/ostorlab/cli/agent/list/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/list/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.379590 ostorlab-1.0.2/src/ostorlab/cli/agent/search/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent/search/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agent_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.379590 ostorlab-1.0.2/src/ostorlab/cli/agentgroup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agentgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/agentgroup/agentgroup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.379590 ostorlab-1.0.2/src/ostorlab/cli/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.379590 ostorlab-1.0.2/src/ostorlab/cli/auth/login/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/auth/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/auth/login/login.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.379590 ostorlab-1.0.2/src/ostorlab/cli/auth/revoke/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/auth/revoke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/auth/revoke/revoke.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.379590 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/ci_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.379590 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.383590 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/assets/android_aab.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/assets/android_apk.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/assets/ios_ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/assets/mobile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.383590 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/ci_logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/ci_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/ci_logger/circleci_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/ci_logger/console_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/ci_logger/github_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/ci_logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/docker_requirements_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/dumpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/input_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/install_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/rootcli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.383590 ostorlab-1.0.2/src/ostorlab/cli/scan/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.383590 ostorlab-1.0.2/src/ostorlab/cli/scan/list/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/list/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.383590 ostorlab-1.0.2/src/ostorlab/cli/scan/run/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.383590 ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/android_aab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/android_apk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/android_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/ios_ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/ios_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/link.py
--rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/run/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.387590 ostorlab-1.0.2/src/ostorlab/cli/scan/stop/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/stop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scan/stop/stop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.387590 ostorlab-1.0.2/src/ostorlab/cli/scanner/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/scanner/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.387590 ostorlab-1.0.2/src/ostorlab/cli/vulnz/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/vulnz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.387590 ostorlab-1.0.2/src/ostorlab/cli/vulnz/describe/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/vulnz/describe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/vulnz/describe/describe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.387590 ostorlab-1.0.2/src/ostorlab/cli/vulnz/dump/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/vulnz/dump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/vulnz/dump/dump.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.387590 ostorlab-1.0.2/src/ostorlab/cli/vulnz/list/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/vulnz/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/vulnz/list/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/cli/vulnz/vulnz.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.387590 ostorlab-1.0.2/src/ostorlab/runtimes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.387590 ostorlab-1.0.2/src/ostorlab/runtimes/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/cloud/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    14599 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.387590 ostorlab-1.0.2/src/ostorlab/runtimes/lite_local/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/lite_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/lite_local/agent_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    14379 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/lite_local/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.391589 ostorlab-1.0.2/src/ostorlab/runtimes/local/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13854 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/agent_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/log_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.391589 ostorlab-1.0.2/src/ostorlab/runtimes/local/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.391589 ostorlab-1.0.2/src/ostorlab/runtimes/local/models/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/models/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/models/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.391589 ostorlab-1.0.2/src/ostorlab/runtimes/local/models/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/models/alembic/versions/35cd577ef0e5_.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/models/alembic/versions/746c5eb3d181_add_vulnerability_location.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/models/alembic/versions/7d12204c3f27_add_references_field_to_vulnerability.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/models/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)    11189 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    30185 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.391589 ostorlab-1.0.2/src/ostorlab/runtimes/local/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.391589 ostorlab-1.0.2/src/ostorlab/runtimes/local/services/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/services/configurations/mq_advanced_conf.config
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/services/jaeger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/services/mq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/local/services/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.391589 ostorlab-1.0.2/src/ostorlab/runtimes/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/proto/agent_instance_settings_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/runtimes/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.391589 ostorlab-1.0.2/src/ostorlab/scanner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.391589 ostorlab-1.0.2/src/ostorlab/scanner/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.395589 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/aab_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/agent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/android_store_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/apk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/domain_name_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/ios_store_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/ip_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/ipa_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/link_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/network_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/v4_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/v6_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.395589 ostorlab-1.0.2/src/ostorlab/scanner/proto/scan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/scan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.395589 ostorlab-1.0.2/src/ostorlab/scanner/proto/scan/_location/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/scan/_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/proto/scan/_location/startAgentScan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/scan_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/scanner/scanner_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.395589 ostorlab-1.0.2/src/ostorlab/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/testing/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.399589 ostorlab-1.0.2/src/ostorlab/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/utils/defintions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/utils/dictionary_minifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/utils/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/utils/risk_rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/utils/scanner_state_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/utils/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-28 13:50:44.000000 ostorlab-1.0.2/src/ostorlab/utils/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:50:54.399589 ostorlab-1.0.2/src/ostorlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-03-28 13:50:54.000000 ostorlab-1.0.2/src/ostorlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    80112 2024-03-28 13:50:54.000000 ostorlab-1.0.2/src/ostorlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:50:54.000000 ostorlab-1.0.2/src/ostorlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-28 13:50:54.000000 ostorlab-1.0.2/src/ostorlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:50:53.000000 ostorlab-1.0.2/src/ostorlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-28 13:50:54.000000 ostorlab-1.0.2/src/ostorlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 13:50:54.000000 ostorlab-1.0.2/src/ostorlab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.857987 ostorlab-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 20:11:47.000000 ostorlab-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-04-01 20:11:53.853987 ostorlab-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-04-01 20:11:47.000000 ostorlab-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-01 20:11:53.857987 ostorlab-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-01 20:11:47.000000 ostorlab-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.649983 ostorlab-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.697984 ostorlab-1.0.3/src/ostorlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.701984 ostorlab-1.0.3/src/ostorlab/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21209 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.701984 ostorlab-1.0.3/src/ostorlab/agent/kb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.701984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.661983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.653983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.701984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.701984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.701984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.701984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.653983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.705984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.705984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.705984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.705984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.705984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.653983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.705984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.705984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.657983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.705984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.709984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.709984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.709984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.709984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.709984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.709984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.709984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.709984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.713984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.713984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.713984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.713984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.713984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.713984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.713984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.713984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.713984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.717984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.717984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.717984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.717984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.717984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.717984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.717984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.717984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.721984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.721984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.721984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.721984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.721984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.721984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.721984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.721984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.721984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.725984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.725984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.725984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.725984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.725984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.725984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.725984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.725984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.729985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.729985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.729985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.729985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.729985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.729985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.661983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.729985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.729985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.733985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.733985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.733985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.733985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.733985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.733985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.733985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.733985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.661983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.737985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.737985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.737985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.737985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.737985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.737985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.737985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.737985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.737985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.741985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.741985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.741985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.741985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.741985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.741985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.741985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.741985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.745985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.661983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.745985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.745985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.745985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.661983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.745985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.745985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.745985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.745985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.669983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.665983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.749985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.749985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.665983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.749985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.749985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.665983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.749985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.749985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.749985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.749985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.753985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.753985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.753985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.753985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.753985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.753985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.753985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.753985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.757985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.757985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.665983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.757985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.665983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.757985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.757985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.665983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.757985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.757985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.669983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.757985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.761985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.761985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.761985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.761985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.761985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.761985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.761985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.761985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.765985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.765985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.765985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.765985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.765985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.765985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.765985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.765985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.669983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.765985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.769985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.769985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.769985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.669983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.769985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.769985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.769985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.669983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.769985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.769985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.669983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.773985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.773985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.669983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.773985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.773985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.773985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.773985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.773985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.773985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.777985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.777985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.777985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.777985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.777985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.777985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.777985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.777985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.777985 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.781986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.781986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.781986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.781986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.781986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.781986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/recommendation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.781986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.781986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.781986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.785986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.673983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.785986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.681984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.677983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.785986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.785986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.785986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.785986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.785986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.785986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.785986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.785986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.789986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.789986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.789986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.677983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.789986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.789986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.789986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.789986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.789986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.789986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.793986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.793986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.677983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.793986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.793986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.793986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.793986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.793986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.793986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.793986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.793986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.797986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.677983 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.797986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.797986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.681984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.797986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.797986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.797986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.797986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.681984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.797986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.797986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.797986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.801986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.801986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.801986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.801986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.801986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.801986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.801986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.801986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.801986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.681984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.805986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.681984 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.805986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.805986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.805986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.805986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17461 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tests/kb_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.805986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tests/tools/kb_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.805986 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-04-01 20:11:48.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tools/kb_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/kb/kb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.805986 ostorlab-1.0.3/src/ostorlab/agent/message/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.805986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.805986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.805986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/common/x509/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/common/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/common/x509/x509_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.805986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.805986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/agent/agent_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/dns_record_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/domain_name_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/service_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/whois_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/android/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/android/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/aab_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/apk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/file_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/ios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/ipa_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/sbom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/sbom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/sbom/sbom_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/source/source_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/ip_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/geolocation_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.809986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/port_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/http_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/v4_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/whois_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/geolocation_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/port_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/http_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/v6_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/whois_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/link/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/link/link_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/android_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/android_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/android_store/android_store_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/developer_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/developer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/ios_store_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.813986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/artifact/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/artifact/artifact_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/filesystem/filesystem_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/http/request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/http/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/http/request/request_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/http/response/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/http/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/http/response/response_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/logs/logs_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/request_response/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/request_response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/request_response/request_response_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/ui_call/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/ui_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/ui_call/ui_call_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/control/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/control/control_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/x509_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/backend_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.817986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/feature_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/metadata_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/feature_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/file_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/backend_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/feature_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/metadata_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/x509_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/x509_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.821986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/healthcheck/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/healthcheck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/healthcheck/ping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/healthcheck/ping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/healthcheck/ping/ping_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/cve/
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/cve/cve_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/done_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/start_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/timeout_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/done/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/done/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/done/done_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/start/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/start/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/start/start_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/timeout_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/status/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/status/status_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/vulnerability/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/vulnerability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/vulnerability/vulnerability_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/use/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/use/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.825986 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/use/device/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/use/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/use/device/device_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/proto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/message/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.829987 ostorlab-1.0.3/src/ostorlab/agent/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/mixins/agent_healthcheck_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/mixins/agent_mq_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/mixins/agent_open_telemetry_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/mixins/agent_persist_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/mixins/agent_report_vulnerability_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.829987 ostorlab-1.0.3/src/ostorlab/agent/mixins/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/mixins/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/mixins/protocols/emit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.829987 ostorlab-1.0.3/src/ostorlab/agent/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/schema/agent_group_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/schema/agent_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/schema/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/schema/target_group_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/agent/schema/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.829987 ostorlab-1.0.3/src/ostorlab/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/add_scanner_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/agent_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/agent_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/agent_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/create_agent_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/create_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/revoke_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.833987 ostorlab-1.0.3/src/ostorlab/apis/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/runners/authenticated_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/runners/login_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/runners/public_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/runners/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/scan_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/scan_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/scan_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/scan_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/scanner_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/test_credentials_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/vulnz_describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/apis/vulnz_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.833987 ostorlab-1.0.3/src/ostorlab/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/android_aab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/android_apk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/android_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/ios_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/ios_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/assets/link.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.833987 ostorlab-1.0.3/src/ostorlab/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.833987 ostorlab-1.0.3/src/ostorlab/cli/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.837987 ostorlab-1.0.3/src/ostorlab/cli/agent/build/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/build/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/build/build_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.837987 ostorlab-1.0.3/src/ostorlab/cli/agent/delete/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/delete/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.837987 ostorlab-1.0.3/src/ostorlab/cli/agent/healthcheck/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/healthcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/healthcheck/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.837987 ostorlab-1.0.3/src/ostorlab/cli/agent/install/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/install/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/install/install_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.837987 ostorlab-1.0.3/src/ostorlab/cli/agent/list/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/list/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.837987 ostorlab-1.0.3/src/ostorlab/cli/agent/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agent_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.837987 ostorlab-1.0.3/src/ostorlab/cli/agentgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agentgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/agentgroup/agentgroup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.837987 ostorlab-1.0.3/src/ostorlab/cli/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.837987 ostorlab-1.0.3/src/ostorlab/cli/auth/login/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/auth/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/auth/login/login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.837987 ostorlab-1.0.3/src/ostorlab/cli/auth/revoke/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/auth/revoke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/auth/revoke/revoke.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.837987 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/ci_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.837987 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.837987 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/assets/android_aab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/assets/android_apk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/assets/ios_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/assets/mobile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.841987 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/ci_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/ci_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/ci_logger/circleci_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/ci_logger/console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/ci_logger/github_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/ci_logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/docker_requirements_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/input_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/install_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/rootcli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.841987 ostorlab-1.0.3/src/ostorlab/cli/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.841987 ostorlab-1.0.3/src/ostorlab/cli/scan/list/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/list/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.841987 ostorlab-1.0.3/src/ostorlab/cli/scan/run/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.841987 ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/android_aab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/android_apk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/android_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/ios_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/ios_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/run/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.841987 ostorlab-1.0.3/src/ostorlab/cli/scan/stop/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/stop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scan/stop/stop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.841987 ostorlab-1.0.3/src/ostorlab/cli/scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/scanner/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.841987 ostorlab-1.0.3/src/ostorlab/cli/vulnz/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/vulnz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.841987 ostorlab-1.0.3/src/ostorlab/cli/vulnz/describe/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/vulnz/describe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/vulnz/describe/describe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.845987 ostorlab-1.0.3/src/ostorlab/cli/vulnz/dump/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/vulnz/dump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/vulnz/dump/dump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.845987 ostorlab-1.0.3/src/ostorlab/cli/vulnz/list/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/vulnz/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/vulnz/list/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/cli/vulnz/vulnz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.845987 ostorlab-1.0.3/src/ostorlab/runtimes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.845987 ostorlab-1.0.3/src/ostorlab/runtimes/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/cloud/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14599 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.845987 ostorlab-1.0.3/src/ostorlab/runtimes/lite_local/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/lite_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/lite_local/agent_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14379 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/lite_local/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.845987 ostorlab-1.0.3/src/ostorlab/runtimes/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13854 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/agent_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/log_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.845987 ostorlab-1.0.3/src/ostorlab/runtimes/local/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.845987 ostorlab-1.0.3/src/ostorlab/runtimes/local/models/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/models/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/models/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.845987 ostorlab-1.0.3/src/ostorlab/runtimes/local/models/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/models/alembic/versions/35cd577ef0e5_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/models/alembic/versions/746c5eb3d181_add_vulnerability_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/models/alembic/versions/7d12204c3f27_add_references_field_to_vulnerability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/models/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    11189 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30185 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.845987 ostorlab-1.0.3/src/ostorlab/runtimes/local/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.845987 ostorlab-1.0.3/src/ostorlab/runtimes/local/services/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/services/configurations/mq_advanced_conf.config
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/services/jaeger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/services/mq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/local/services/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.849987 ostorlab-1.0.3/src/ostorlab/runtimes/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/proto/agent_instance_settings_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/runtimes/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.849987 ostorlab-1.0.3/src/ostorlab/scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.849987 ostorlab-1.0.3/src/ostorlab/scanner/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.849987 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/aab_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/agent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/android_store_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/apk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/domain_name_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/ios_store_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/ip_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/ipa_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/link_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/network_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/v4_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/v6_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.849987 ostorlab-1.0.3/src/ostorlab/scanner/proto/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/scan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.849987 ostorlab-1.0.3/src/ostorlab/scanner/proto/scan/_location/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/scan/_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/proto/scan/_location/startAgentScan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/scan_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/scanner/scanner_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.849987 ostorlab-1.0.3/src/ostorlab/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/testing/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.853987 ostorlab-1.0.3/src/ostorlab/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/utils/defintions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/utils/dictionary_minifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/utils/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/utils/risk_rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/utils/scanner_state_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/utils/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-01 20:11:47.000000 ostorlab-1.0.3/src/ostorlab/utils/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:11:53.853987 ostorlab-1.0.3/src/ostorlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-04-01 20:11:53.000000 ostorlab-1.0.3/src/ostorlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    80112 2024-04-01 20:11:53.000000 ostorlab-1.0.3/src/ostorlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:11:53.000000 ostorlab-1.0.3/src/ostorlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-01 20:11:53.000000 ostorlab-1.0.3/src/ostorlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:11:53.000000 ostorlab-1.0.3/src/ostorlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-01 20:11:53.000000 ostorlab-1.0.3/src/ostorlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 20:11:53.000000 ostorlab-1.0.3/src/ostorlab.egg-info/top_level.txt
```

### Comparing `ostorlab-1.0.2/LICENSE` & `ostorlab-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/PKG-INFO` & `ostorlab-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ostorlab
-Version: 1.0.2
+Version: 1.0.3
 Summary: OXO Scanner Orchestrator for the Modern Age.
 Home-page: https://github.com/Ostorlab/ostorlab
 Author: Ostorlab
 Author-email: oxo@ostorlab.dev
 License: Apache-2.0
 Project-URL: Documentation, https://oxo.ostorlab.co/
 Project-URL: Source, https://github.com/Ostorlab/oxo
@@ -29,32 +29,32 @@
 Requires-Dist: sqlalchemy~=1.4
 Requires-Dist: semver>=3.0.0
 Requires-Dist: markdownify
 Requires-Dist: alembic
 Requires-Dist: py-ubjson
 Requires-Dist: nats-py
 Provides-Extra: agent
-Requires-Dist: Werkzeug==2.3.7; extra == "agent"
+Requires-Dist: Werkzeug~=2.3; extra == "agent"
 Requires-Dist: aio-pika; extra == "agent"
 Requires-Dist: flask; extra == "agent"
 Requires-Dist: importlib-metadata; python_version < "3.8" and extra == "agent"
 Requires-Dist: jsonschema>=4.4.0; extra == "agent"
-Requires-Dist: protobuf==3.20.1; extra == "agent"
+Requires-Dist: protobuf~=3.20; extra == "agent"
 Requires-Dist: ruamel.yaml; extra == "agent"
 Requires-Dist: tenacity; extra == "agent"
 Requires-Dist: semver; extra == "agent"
 Requires-Dist: redis; extra == "agent"
 Requires-Dist: google-cloud-logging; extra == "agent"
 Requires-Dist: opentelemetry-distro; extra == "agent"
 Requires-Dist: opentelemetry-exporter-jaeger; extra == "agent"
 Requires-Dist: opentelemetry-exporter-gcp-trace; extra == "agent"
 Provides-Extra: google-cloud-logging
 Requires-Dist: google-cloud-logging; extra == "google-cloud-logging"
 Provides-Extra: testing
-Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: setuptools>=65.5.1; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-asyncio; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: pytest-timeout; extra == "testing"
 Requires-Dist: pytest-httpx; extra == "testing"
 Provides-Extra: scanner
```

### Comparing `ostorlab-1.0.2/README.md` & `ostorlab-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/setup.cfg` & `ostorlab-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author = Ostorlab
 author_email = oxo@ostorlab.dev
 license = Apache-2.0
 license_files = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Ostorlab/ostorlab
-version = 1.0.2
+version = 1.0.3
 project_urls = 
 	Documentation = https://oxo.ostorlab.co/
 	Source = https://github.com/Ostorlab/oxo
 	Changelog = https://github.com/Ostorlab/oxo/releases
 	Tracker = https://github.com/Ostorlab/oxo/issues
 	Twitter = https://twitter.com/OstorlabSec
 platforms = any
@@ -50,32 +50,32 @@
 	tests
 
 [options.package_data]
 * = *.json, *.md, *.config, py.typed, alembic.ini, script.py.mako
 
 [options.extras_require]
 agent = 
-	Werkzeug==2.3.7
+	Werkzeug~=2.3
 	aio-pika
 	flask
 	importlib-metadata; python_version<"3.8"
 	jsonschema>=4.4.0
-	protobuf==3.20.1
+	protobuf~=3.20
 	ruamel.yaml
 	tenacity
 	semver
 	redis
 	google-cloud-logging
 	opentelemetry-distro
 	opentelemetry-exporter-jaeger
 	opentelemetry-exporter-gcp-trace
 google-cloud-logging = 
 	google-cloud-logging
 testing = 
-	setuptools
+	setuptools>=65.5.1
 	pytest
 	pytest-cov
 	pytest-asyncio
 	pytest-mock
 	pytest-timeout
 	pytest-httpx
 scanner =
```

### Comparing `ostorlab-1.0.2/setup.py` & `ostorlab-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/__init__.py` & `ostorlab-1.0.3/src/ostorlab/__init__.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/agent.py` & `ostorlab-1.0.3/src/ostorlab/agent/agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/definitions.py` & `ostorlab-1.0.3/src/ostorlab/agent/definitions.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/context.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/context.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/context.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/context.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/context.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/context.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/context.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/context.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/context.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/context.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/context.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/context.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/README.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/README.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/recommendation.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/description.md` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/meta.json` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tests/kb_test.py` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tests/kb_test.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tests/tools/kb_generator_test.py` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tests/tools/kb_generator_test.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tests/utils.py` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/KB/tools/kb_generator.py` & `ostorlab-1.0.3/src/ostorlab/agent/kb/KB/tools/kb_generator.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/kb/kb.py` & `ostorlab-1.0.3/src/ostorlab/agent/kb/kb.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/message.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/message.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/common/x509/x509_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/common/x509/x509_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/agent/agent_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/agent/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/dns_record_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/dns_record_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/domain_name_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/domain_name_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/service_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/service_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/whois_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/whois_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/aab_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/aab_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/apk_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/apk_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/file_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/file_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/ipa_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/ipa_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/sbom/sbom_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/sbom/sbom_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/file/source/source_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/file/source/source_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/ip_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/ip_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/geolocation_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/geolocation_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/port_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/port_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/http_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/http_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/service_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/service_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/v4_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/v4_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/whois_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/whois_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/geolocation_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/geolocation_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/port_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/port_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/http_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/http_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/service_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/service_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/v6_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/v6_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/whois_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/whois_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/link/link_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/link/link_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/android_store/android_store_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/android_store/android_store_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/developer_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/developer_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/developer_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/developer_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/ios_store_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/ios_store_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/artifact/artifact_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/artifact/artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/filesystem/filesystem_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/filesystem/filesystem_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/http/request/request_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/http/request/request_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/http/response/response_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/http/response/response_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/logs/logs_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/logs/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/request_response/request_response_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/request_response/request_response_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/capture/ui_call/ui_call_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/capture/ui_call/ui_call_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/control/control_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/control/control_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/library_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/x509_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/x509_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/backend_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/backend_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/feature_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/library_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/metadata_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/feature_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/file_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/file_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/backend_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/backend_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/feature_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/library_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/metadata_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/library_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/library_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/x509_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/x509_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/library_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/x509_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/x509_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/healthcheck/ping/ping_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/healthcheck/ping/ping_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/cve/cve_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/cve/cve_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/done_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/done_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/start_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/start_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/timeout_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/timeout_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/done/done_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/done/done_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/start/start_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/start/start_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/timeout_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/timeout_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/status/status_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/status/status_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/report/vulnerability/vulnerability_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/report/vulnerability/vulnerability_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto/v3/use/device/device_pb2.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto/v3/use/device/device_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/proto_dict.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/proto_dict.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/message/serializer.py` & `ostorlab-1.0.3/src/ostorlab/agent/message/serializer.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/mixins/agent_healthcheck_mixin.py` & `ostorlab-1.0.3/src/ostorlab/agent/mixins/agent_healthcheck_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/mixins/agent_mq_mixin.py` & `ostorlab-1.0.3/src/ostorlab/agent/mixins/agent_mq_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/mixins/agent_open_telemetry_mixin.py` & `ostorlab-1.0.3/src/ostorlab/agent/mixins/agent_open_telemetry_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/mixins/agent_persist_mixin.py` & `ostorlab-1.0.3/src/ostorlab/agent/mixins/agent_persist_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/mixins/agent_report_vulnerability_mixin.py` & `ostorlab-1.0.3/src/ostorlab/agent/mixins/agent_report_vulnerability_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/mixins/protocols/emit.py` & `ostorlab-1.0.3/src/ostorlab/agent/mixins/protocols/emit.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/schema/agent_group_schema.json` & `ostorlab-1.0.3/src/ostorlab/agent/schema/agent_group_schema.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/schema/agent_schema.json` & `ostorlab-1.0.3/src/ostorlab/agent/schema/agent_schema.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/schema/loader.py` & `ostorlab-1.0.3/src/ostorlab/agent/schema/loader.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/schema/target_group_schema.json` & `ostorlab-1.0.3/src/ostorlab/agent/schema/target_group_schema.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/agent/schema/validator.py` & `ostorlab-1.0.3/src/ostorlab/agent/schema/validator.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/add_scanner_state.py` & `ostorlab-1.0.3/src/ostorlab/apis/add_scanner_state.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/agent_details.py` & `ostorlab-1.0.3/src/ostorlab/apis/agent_details.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/agent_group.py` & `ostorlab-1.0.3/src/ostorlab/apis/agent_group.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/agent_search.py` & `ostorlab-1.0.3/src/ostorlab/apis/agent_search.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/assets.py` & `ostorlab-1.0.3/src/ostorlab/apis/assets.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/create_agent_scan.py` & `ostorlab-1.0.3/src/ostorlab/apis/create_agent_scan.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/create_api_key.py` & `ostorlab-1.0.3/src/ostorlab/apis/create_api_key.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/login.py` & `ostorlab-1.0.3/src/ostorlab/apis/login.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/request.py` & `ostorlab-1.0.3/src/ostorlab/apis/request.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/revoke_api_key.py` & `ostorlab-1.0.3/src/ostorlab/apis/revoke_api_key.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/runners/authenticated_runner.py` & `ostorlab-1.0.3/src/ostorlab/apis/runners/authenticated_runner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/runners/login_runner.py` & `ostorlab-1.0.3/src/ostorlab/apis/runners/login_runner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/runners/public_runner.py` & `ostorlab-1.0.3/src/ostorlab/apis/runners/public_runner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/runners/runner.py` & `ostorlab-1.0.3/src/ostorlab/apis/runners/runner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/scan_create.py` & `ostorlab-1.0.3/src/ostorlab/apis/scan_create.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/scan_info.py` & `ostorlab-1.0.3/src/ostorlab/apis/scan_info.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/scan_list.py` & `ostorlab-1.0.3/src/ostorlab/apis/scan_list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/scan_stop.py` & `ostorlab-1.0.3/src/ostorlab/apis/scan_stop.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/scanner_config.py` & `ostorlab-1.0.3/src/ostorlab/apis/scanner_config.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/test_credentials_create.py` & `ostorlab-1.0.3/src/ostorlab/apis/test_credentials_create.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/vulnz_describe.py` & `ostorlab-1.0.3/src/ostorlab/apis/vulnz_describe.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/apis/vulnz_list.py` & `ostorlab-1.0.3/src/ostorlab/apis/vulnz_list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/assets/agent.py` & `ostorlab-1.0.3/src/ostorlab/assets/agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/assets/android_aab.py` & `ostorlab-1.0.3/src/ostorlab/assets/android_aab.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/assets/android_apk.py` & `ostorlab-1.0.3/src/ostorlab/assets/android_apk.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/assets/asset.py` & `ostorlab-1.0.3/src/ostorlab/assets/asset.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/assets/file.py` & `ostorlab-1.0.3/src/ostorlab/assets/file.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/assets/ios_ipa.py` & `ostorlab-1.0.3/src/ostorlab/assets/ios_ipa.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/assets/ip.py` & `ostorlab-1.0.3/src/ostorlab/assets/ip.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/assets/ipv4.py` & `ostorlab-1.0.3/src/ostorlab/assets/ipv4.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/assets/ipv6.py` & `ostorlab-1.0.3/src/ostorlab/assets/ipv6.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/agent/build/build.py` & `ostorlab-1.0.3/src/ostorlab/cli/agent/build/build.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/agent/build/build_progress.py` & `ostorlab-1.0.3/src/ostorlab/cli/agent/build/build_progress.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/agent/delete/delete.py` & `ostorlab-1.0.3/src/ostorlab/cli/agent/delete/delete.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/agent/healthcheck/healthcheck.py` & `ostorlab-1.0.3/src/ostorlab/cli/agent/healthcheck/healthcheck.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/agent/install/install.py` & `ostorlab-1.0.3/src/ostorlab/cli/agent/install/install.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/agent/install/install_progress.py` & `ostorlab-1.0.3/src/ostorlab/cli/agent/install/install_progress.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/agent/list/list.py` & `ostorlab-1.0.3/src/ostorlab/cli/agent/list/list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/agent/search/search.py` & `ostorlab-1.0.3/src/ostorlab/cli/agent/search/search.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/agent_fetcher.py` & `ostorlab-1.0.3/src/ostorlab/cli/agent_fetcher.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/auth/login/login.py` & `ostorlab-1.0.3/src/ostorlab/cli/auth/login/login.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/auth/revoke/revoke.py` & `ostorlab-1.0.3/src/ostorlab/cli/auth/revoke/revoke.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/assets/android_aab.py` & `ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/assets/android_aab.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/assets/android_apk.py` & `ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/assets/android_apk.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/assets/ios_ipa.py` & `ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/assets/ios_ipa.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/assets/mobile.py` & `ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/assets/mobile.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/ci_logger/circleci_logger.py` & `ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/ci_logger/circleci_logger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/ci_logger/console_logger.py` & `ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/ci_logger/console_logger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/ci_logger/github_logger.py` & `ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/ci_logger/github_logger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/ci_logger/logger.py` & `ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/ci_logger/logger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/ci_scan/run/run.py` & `ostorlab-1.0.3/src/ostorlab/cli/ci_scan/run/run.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/console.py` & `ostorlab-1.0.3/src/ostorlab/cli/console.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/docker_requirements_checker.py` & `ostorlab-1.0.3/src/ostorlab/cli/docker_requirements_checker.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/dumpers.py` & `ostorlab-1.0.3/src/ostorlab/cli/dumpers.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/input_validators.py` & `ostorlab-1.0.3/src/ostorlab/cli/input_validators.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/install_agent.py` & `ostorlab-1.0.3/src/ostorlab/cli/install_agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/rootcli.py` & `ostorlab-1.0.3/src/ostorlab/cli/rootcli.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/list/list.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/list/list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/__init__.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/agent.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/android_aab.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/android_aab.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/android_apk.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/android_apk.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/android_store.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/android_store.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/domain_name.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/domain_name.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/file.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/file.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/ios_ipa.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/ios_ipa.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/ios_store.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/ios_store.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/ip.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/ip.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/run/assets/link.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/run/assets/link.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/run/run.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/run/run.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/scan.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/scan.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scan/stop/stop.py` & `ostorlab-1.0.3/src/ostorlab/cli/scan/stop/stop.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/scanner/scanner.py` & `ostorlab-1.0.3/src/ostorlab/cli/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/types.py` & `ostorlab-1.0.3/src/ostorlab/cli/types.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/vulnz/describe/describe.py` & `ostorlab-1.0.3/src/ostorlab/cli/vulnz/describe/describe.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/vulnz/dump/dump.py` & `ostorlab-1.0.3/src/ostorlab/cli/vulnz/dump/dump.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/vulnz/list/list.py` & `ostorlab-1.0.3/src/ostorlab/cli/vulnz/list/list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/cli/vulnz/vulnz.py` & `ostorlab-1.0.3/src/ostorlab/cli/vulnz/vulnz.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/configuration_manager.py` & `ostorlab-1.0.3/src/ostorlab/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/cloud/runtime.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/cloud/runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/definitions.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/definitions.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/lite_local/agent_runtime.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/lite_local/agent_runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/lite_local/runtime.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/lite_local/runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/local/agent_runtime.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/local/agent_runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/local/log_streamer.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/local/log_streamer.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/local/models/alembic/env.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/local/models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/local/models/alembic/versions/35cd577ef0e5_.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/local/models/alembic/versions/35cd577ef0e5_.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/local/models/alembic.ini` & `ostorlab-1.0.3/src/ostorlab/runtimes/local/models/alembic.ini`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/local/models/models.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/local/models/models.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/local/runtime.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/local/runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/local/services/jaeger.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/local/services/jaeger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/local/services/mq.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/local/services/mq.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/local/services/redis.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/local/services/redis.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/proto/agent_instance_settings_pb2.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/proto/agent_instance_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/registry.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/registry.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/runtimes/runtime.py` & `ostorlab-1.0.3/src/ostorlab/runtimes/runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/callbacks.py` & `ostorlab-1.0.3/src/ostorlab/scanner/callbacks.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/handler.py` & `ostorlab-1.0.3/src/ostorlab/scanner/handler.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/aab_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/aab_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/agent_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/android_store_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/android_store_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/apk_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/apk_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/domain_name_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/domain_name_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/file_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/file_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/ios_store_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/ios_store_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/ip_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/ip_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/ipa_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/ipa_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/link_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/link_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/network_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/network_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/source_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/source_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/v4_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/v4_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/assets/v6_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/assets/v6_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/proto/scan/_location/startAgentScan_pb2.py` & `ostorlab-1.0.3/src/ostorlab/scanner/proto/scan/_location/startAgentScan_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/scan_handler.py` & `ostorlab-1.0.3/src/ostorlab/scanner/scan_handler.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/scanner/scanner_conf.py` & `ostorlab-1.0.3/src/ostorlab/scanner/scanner_conf.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/testing/agent.py` & `ostorlab-1.0.3/src/ostorlab/testing/agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/utils/defintions.py` & `ostorlab-1.0.3/src/ostorlab/utils/defintions.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/utils/dictionary_minifier.py` & `ostorlab-1.0.3/src/ostorlab/utils/dictionary_minifier.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/utils/risk_rating.py` & `ostorlab-1.0.3/src/ostorlab/utils/risk_rating.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/utils/scanner_state_reporter.py` & `ostorlab-1.0.3/src/ostorlab/utils/scanner_state_reporter.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/utils/strings.py` & `ostorlab-1.0.3/src/ostorlab/utils/strings.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/utils/styles.py` & `ostorlab-1.0.3/src/ostorlab/utils/styles.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/utils/system.py` & `ostorlab-1.0.3/src/ostorlab/utils/system.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/utils/version.py` & `ostorlab-1.0.3/src/ostorlab/utils/version.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab/utils/volumes.py` & `ostorlab-1.0.3/src/ostorlab/utils/volumes.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab.egg-info/PKG-INFO` & `ostorlab-1.0.3/src/ostorlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ostorlab
-Version: 1.0.2
+Version: 1.0.3
 Summary: OXO Scanner Orchestrator for the Modern Age.
 Home-page: https://github.com/Ostorlab/ostorlab
 Author: Ostorlab
 Author-email: oxo@ostorlab.dev
 License: Apache-2.0
 Project-URL: Documentation, https://oxo.ostorlab.co/
 Project-URL: Source, https://github.com/Ostorlab/oxo
@@ -29,32 +29,32 @@
 Requires-Dist: sqlalchemy~=1.4
 Requires-Dist: semver>=3.0.0
 Requires-Dist: markdownify
 Requires-Dist: alembic
 Requires-Dist: py-ubjson
 Requires-Dist: nats-py
 Provides-Extra: agent
-Requires-Dist: Werkzeug==2.3.7; extra == "agent"
+Requires-Dist: Werkzeug~=2.3; extra == "agent"
 Requires-Dist: aio-pika; extra == "agent"
 Requires-Dist: flask; extra == "agent"
 Requires-Dist: importlib-metadata; python_version < "3.8" and extra == "agent"
 Requires-Dist: jsonschema>=4.4.0; extra == "agent"
-Requires-Dist: protobuf==3.20.1; extra == "agent"
+Requires-Dist: protobuf~=3.20; extra == "agent"
 Requires-Dist: ruamel.yaml; extra == "agent"
 Requires-Dist: tenacity; extra == "agent"
 Requires-Dist: semver; extra == "agent"
 Requires-Dist: redis; extra == "agent"
 Requires-Dist: google-cloud-logging; extra == "agent"
 Requires-Dist: opentelemetry-distro; extra == "agent"
 Requires-Dist: opentelemetry-exporter-jaeger; extra == "agent"
 Requires-Dist: opentelemetry-exporter-gcp-trace; extra == "agent"
 Provides-Extra: google-cloud-logging
 Requires-Dist: google-cloud-logging; extra == "google-cloud-logging"
 Provides-Extra: testing
-Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: setuptools>=65.5.1; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-asyncio; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: pytest-timeout; extra == "testing"
 Requires-Dist: pytest-httpx; extra == "testing"
 Provides-Extra: scanner
```

### Comparing `ostorlab-1.0.2/src/ostorlab.egg-info/SOURCES.txt` & `ostorlab-1.0.3/src/ostorlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.2/src/ostorlab.egg-info/requires.txt` & `ostorlab-1.0.3/src/ostorlab.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 py-ubjson
 nats-py
 
 [:python_version < "3.8"]
 importlib-metadata
 
 [agent]
-Werkzeug==2.3.7
+Werkzeug~=2.3
 aio-pika
 flask
 jsonschema>=4.4.0
-protobuf==3.20.1
+protobuf~=3.20
 ruamel.yaml
 tenacity
 semver
 redis
 google-cloud-logging
 opentelemetry-distro
 opentelemetry-exporter-jaeger
@@ -38,14 +38,14 @@
 google-cloud-logging
 
 [scanner]
 psutil
 python-daemon
 
 [testing]
-setuptools
+setuptools>=65.5.1
 pytest
 pytest-cov
 pytest-asyncio
 pytest-mock
 pytest-timeout
 pytest-httpx
```

